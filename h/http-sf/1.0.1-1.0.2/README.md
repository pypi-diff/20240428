# Comparing `tmp/http-sf-1.0.1.tar.gz` & `tmp/http_sf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http-sf-1.0.1.tar", last modified: Thu Jan 25 06:12:42 2024, max compression
+gzip compressed data, was "http_sf-1.0.2.tar", last modified: Sun Apr 28 08:06:24 2024, max compression
```

## Comparing `http-sf-1.0.1.tar` & `http_sf-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:12:42.680508 http-sf-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-25 06:12:13.000000 http-sf-1.0.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-25 06:12:13.000000 http-sf-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-01-25 06:12:42.680508 http-sf-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-01-25 06:12:13.000000 http-sf-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:12:42.680508 http-sf-1.0.1/http_sf/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2542 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/bare_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/boolean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/byteseq.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/date.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/decimal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1995 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/display_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/innerlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/integer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/retrofit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1463 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/string.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-01-25 06:12:13.000000 http-sf-1.0.1/http_sf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:12:42.680508 http-sf-1.0.1/http_sf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-01-25 06:12:42.000000 http-sf-1.0.1/http_sf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-25 06:12:42.000000 http-sf-1.0.1/http_sf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 06:12:42.000000 http-sf-1.0.1/http_sf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-25 06:12:42.000000 http-sf-1.0.1/http_sf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-25 06:12:42.000000 http-sf-1.0.1/http_sf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-01-25 06:12:13.000000 http-sf-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 06:12:42.680508 http-sf-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:12:42.680508 http-sf-1.0.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3469 2024-01-25 06:12:13.000000 http-sf-1.0.1/test/harfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4950 2024-01-25 06:12:13.000000 http-sf-1.0.1/test/test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2197 2024-01-25 06:12:13.000000 http-sf-1.0.1/test/test_perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:06:24.913951 http_sf-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-28 08:06:05.000000 http_sf-1.0.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-28 08:06:05.000000 http_sf-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-28 08:06:24.913951 http_sf-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-28 08:06:05.000000 http_sf-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:06:24.909952 http_sf-1.0.2/http_sf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2542 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/bare_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/boolean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/byteseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/date.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/decimal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1999 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/display_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/innerlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/integer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/retrofit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1463 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/string.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-28 08:06:05.000000 http_sf-1.0.2/http_sf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:06:24.913951 http_sf-1.0.2/http_sf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-28 08:06:24.000000 http_sf-1.0.2/http_sf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-28 08:06:24.000000 http_sf-1.0.2/http_sf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 08:06:24.000000 http_sf-1.0.2/http_sf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 08:06:24.000000 http_sf-1.0.2/http_sf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 08:06:24.000000 http_sf-1.0.2/http_sf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-28 08:06:05.000000 http_sf-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 08:06:24.913951 http_sf-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:06:24.913951 http_sf-1.0.2/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3469 2024-04-28 08:06:05.000000 http_sf-1.0.2/test/harfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4034 2024-04-28 08:06:05.000000 http_sf-1.0.2/test/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2197 2024-04-28 08:06:05.000000 http_sf-1.0.2/test/test_perf.py
```

### Comparing `http-sf-1.0.1/LICENCE.md` & `http_sf-1.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/PKG-INFO` & `http_sf-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-sf
-Version: 1.0.1
+Version: 1.0.2
 Summary: Parse and serialise HTTP Structured Fields
 Author-email: Mark Nottingham <mnot@mnot.net>
 Project-URL: homepage, https://github.com/mnot/http-sf
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `http-sf-1.0.1/README.md` & `http_sf-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/__init__.py` & `http_sf-1.0.2/http_sf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from typing import Tuple, List, Dict, Optional
 
 from http_sf.dictionary import parse_dictionary, ser_dictionary
 from http_sf.item import parse_item, ser_item
 from http_sf.list import parse_list, ser_list
 from http_sf.retrofit import retrofit
```

### Comparing `http-sf-1.0.1/http_sf/__main__.py` & `http_sf-1.0.2/http_sf/__main__.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/bare_item.py` & `http_sf-1.0.2/http_sf/bare_item.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/byteseq.py` & `http_sf-1.0.2/http_sf/byteseq.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/decimal.py` & `http_sf-1.0.2/http_sf/decimal.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/dictionary.py` & `http_sf-1.0.2/http_sf/dictionary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Tuple, cast
 
-from http_sf.item import ser_item
-from http_sf.innerlist import parse_item_or_inner_list
+from http_sf.innerlist import parse_item_or_inner_list, ser_item_or_inner_list
 from http_sf.parameters import parse_params, ser_params
 from http_sf.types import DictionaryType, ItemType
 from http_sf.util import discard_http_ows, ser_key, parse_key
 
 
 EQUALS = ord(b"=")
 COMMA = ord(b",")
@@ -46,11 +45,11 @@
     if len(dictionary) == 0:
         raise ValueError("No contents; field should not be emitted")
     return ", ".join(
         [
             f"{ser_key(m)}"
             f"""{ser_params(n[1]) if
                 (isinstance(n, tuple) and n[0] is True)
-                else f'={ser_item(cast(ItemType, n))}'}"""
+                else f'={ser_item_or_inner_list(cast(ItemType, n))}'}"""
             for m, n in dictionary.items()
         ]
     )
```

### Comparing `http-sf-1.0.1/http_sf/display_string.py` & `http_sf-1.0.2/http_sf/display_string.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/innerlist.py` & `http_sf-1.0.2/http_sf/innerlist.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/integer.py` & `http_sf-1.0.2/http_sf/integer.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/item.py` & `http_sf-1.0.2/http_sf/item.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/list.py` & `http_sf-1.0.2/http_sf/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 COMMA = ord(b",")
 
 
 def parse_list(data: bytes) -> Tuple[int, ListType]:
     bytes_consumed = 0
     _list = []
     data_len = len(data)
-    while True:
+    while bytes_consumed < data_len:
         offset, member = parse_item_or_inner_list(data[bytes_consumed:])
         bytes_consumed += offset
         _list.append(member)
         bytes_consumed += discard_http_ows(data[bytes_consumed:])
         if bytes_consumed == data_len:
             return bytes_consumed, _list
         if data[bytes_consumed] != COMMA:
             raise ValueError("Trailing text after item in list")
         bytes_consumed += 1
         bytes_consumed += discard_http_ows(data[bytes_consumed:])
         if bytes_consumed == data_len:
             raise ValueError("Trailing comma at end of list")
+    return bytes_consumed, _list
 
 
 def ser_list(_list: ListType) -> str:
     if len(_list) == 0:
         raise ValueError("No contents; field should not be emitted")
     return ", ".join([ser_item_or_inner_list(m) for m in _list])
```

### Comparing `http-sf-1.0.1/http_sf/parameters.py` & `http_sf-1.0.2/http_sf/parameters.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/retrofit.py` & `http_sf-1.0.2/http_sf/retrofit.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/string.py` & `http_sf-1.0.2/http_sf/string.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/token.py` & `http_sf-1.0.2/http_sf/token.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf/types.py` & `http_sf-1.0.2/http_sf/types.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/http_sf.egg-info/PKG-INFO` & `http_sf-1.0.2/http_sf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-sf
-Version: 1.0.1
+Version: 1.0.2
 Summary: Parse and serialise HTTP Structured Fields
 Author-email: Mark Nottingham <mnot@mnot.net>
 Project-URL: homepage, https://github.com/mnot/http-sf
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `http-sf-1.0.1/http_sf.egg-info/SOURCES.txt` & `http_sf-1.0.2/http_sf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/pyproject.toml` & `http_sf-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/test/harfile.py` & `http_sf-1.0.2/test/harfile.py`

 * *Files identical despite different names*

### Comparing `http-sf-1.0.1/test/test_perf.py` & `http_sf-1.0.2/test/test_perf.py`

 * *Files identical despite different names*

