# Comparing `tmp/clickhouse_arrow-0.3.0.tar.gz` & `tmp/clickhouse_arrow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse_arrow-0.3.0.tar", max compression
+gzip compressed data, was "clickhouse_arrow-0.4.0.tar", max compression
```

## Comparing `clickhouse_arrow-0.3.0.tar` & `clickhouse_arrow-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11361 2023-03-25 13:20:32.938480 clickhouse_arrow-0.3.0/LICENSE
--rw-r--r--   0        0        0     1275 2023-03-25 13:18:15.085427 clickhouse_arrow-0.3.0/README.md
--rw-r--r--   0        0        0     7477 2023-07-30 06:14:44.522060 clickhouse_arrow-0.3.0/clickhouse_arrow/__init__.py
--rw-r--r--   0        0        0      691 2023-07-30 06:14:44.522240 clickhouse_arrow-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 clickhouse_arrow-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11361 2023-03-25 13:20:32.938480 clickhouse_arrow-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1275 2023-03-25 13:18:15.085427 clickhouse_arrow-0.4.0/README.md
+-rw-r--r--   0        0        0     8879 2024-04-28 18:04:16.310426 clickhouse_arrow-0.4.0/clickhouse_arrow/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-28 18:04:16.311073 clickhouse_arrow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 clickhouse_arrow-0.4.0/PKG-INFO
```

### Comparing `clickhouse_arrow-0.3.0/LICENSE` & `clickhouse_arrow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.3.0/README.md` & `clickhouse_arrow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.3.0/clickhouse_arrow/__init__.py` & `clickhouse_arrow-0.4.0/clickhouse_arrow/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import collections.abc
 from typing import Any, Iterator
 from urllib.parse import urlencode
 
 import pyarrow as pa
 import urllib3
 from importlib.metadata import version
 
@@ -27,29 +28,32 @@
     A minimal client that uses the ClickHouse HTTP API and Apache Arrow.
 
     Args:
        url: (str) The host name of the server to connect to, defaults to `http://localhost:8123/`.
        user: (str) The optional username to authenticate with, defaults to `default`.
        password: (str) The optional password to authenticate with, defaults to empty.
        pool: (PoolManager) The optional HTTP connection pool to use.
+       default_settings: (dict) The optional default settings to include with every query.
     """
 
     def __init__(
         self,
         url: str = "http://localhost:8123/",
         user: str = "default",
         password: str = "",
         pool: urllib3.PoolManager = None,
+        default_settings: dict[str, Any] = None,
     ):
         self._url = url
         self._headers = {
             "X-ClickHouse-User": user,
             "X-ClickHouse-Key": password,
         }
         self._pool = pool or urllib3.PoolManager()
+        self._default_settings = default_settings
 
     def execute(
         self,
         query: str,
         params: dict[str, Any] = None,
         settings: dict[str, Any] = None,
     ):
@@ -179,25 +183,38 @@
         format_: str = None,
     ):
         if format_:
             query += f" FORMAT {format_}"
         fields = create_post_body(query, params)
         body, content_type = urllib3.encode_multipart_formdata(fields)
         headers = self._headers | {"Content-Type": content_type}
+        settings = self._combine_settings(settings)
         url = append_url(self._url, **settings) if settings else self._url
         response = self._pool.urlopen(
             "POST",
             url,
             body=body,
             headers=headers,
             preload_content=False,
         )
         ensure_success_status(response)
         return response
 
+    def _combine_settings(
+        self, settings: dict[str, Any] | None
+    ) -> dict[str, Any] | None:
+        match (settings, self._default_settings):
+            case (None, _):
+                return self._default_settings
+            case (_, None):
+                return settings
+            case (_, _):
+                return self._default_settings | settings
+        return None
+
 
 class ClickhouseException(Exception):
     """
     Occurs when a non-success response is received from Clickhouse.
 
     Args:
         status: (int) The response status code.
@@ -213,18 +230,38 @@
 def append_url(url: str, **query) -> str:
     return f"{url}?{urlencode(query)}"
 
 
 def create_post_body(query: str, params: dict[str, Any]):
     body = {"query": query}
     if params:
-        body.update({f"param_{k}": v for k, v in params.items()})
+        body.update({f"param_{k}": bind_param(v) for k, v in params.items()})
     return body
 
 
+def bind_param(value: Any, quote_strings=False) -> str:
+    # Inspired by clickhouse-connect.
+    if value is None:
+        return "NULL"
+    if isinstance(value, (bool, int, float)):
+        return str(value)
+    if isinstance(value, str):
+        return f"'{value}'" if quote_strings else value
+    if isinstance(value, tuple):
+        return f"({', '.join([bind_param(v, True) for v in value])})"
+    if isinstance(value, dict):
+        pairs = (
+            bind_param(k, True) + ":" + bind_param(v, True) for k, v in value.items()
+        )
+        return f"{{{', '.join(pairs)}}}"
+    if isinstance(value, collections.abc.Iterable):
+        return f"[{', '.join([bind_param(v, True) for v in value])}]"
+    return str(value)
+
+
 def ensure_success_status(response: urllib3.HTTPResponse):
     if response.status != 200:
         raise ClickhouseException(response.status, str(response.data))
 
 
 def serialize_ipc(table: pa.Table) -> bytes:
     buffer = pa.BufferOutputStream()
```

### Comparing `clickhouse_arrow-0.3.0/pyproject.toml` & `clickhouse_arrow-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clickhouse-arrow"
-version = "0.3.0"
+version = "0.4.0"
 description = "A minimal client that uses the ClickHouse HTTP API and Apache Arrow."
 authors = ["Martin Galpin <galpin@galpin.com>"]
 homepage = "https://github.com/galpin/clickhouse-arrow"
 repository = "https://github.com/galpin/clickhouse-arrow"
 readme = "README.md"
 
 
@@ -16,14 +16,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-benchmark = "^4.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest-docker = "^1.0.1"
 pandas = "^1.5.3"
+ruff = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `clickhouse_arrow-0.3.0/PKG-INFO` & `clickhouse_arrow-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: clickhouse-arrow
-Version: 0.3.0
+Version: 0.4.0
 Summary: A minimal client that uses the ClickHouse HTTP API and Apache Arrow.
 Home-page: https://github.com/galpin/clickhouse-arrow
 Author: Martin Galpin
 Author-email: galpin@galpin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: urllib3 (<2.0.0)
 Project-URL: Repository, https://github.com/galpin/clickhouse-arrow
 Description-Content-Type: text/markdown
 
 # Clickhouse Arrow 🏠 🏹
```

