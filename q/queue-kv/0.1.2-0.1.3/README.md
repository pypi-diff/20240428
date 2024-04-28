# Comparing `tmp/queue_kv-0.1.2.tar.gz` & `tmp/queue_kv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_kv-0.1.2.tar", last modified: Thu Apr 25 16:54:40 2024, max compression
+gzip compressed data, was "queue_kv-0.1.3.tar", last modified: Sun Apr 28 09:02:23 2024, max compression
```

## Comparing `queue_kv-0.1.2.tar` & `queue_kv-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.263055 queue_kv-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-25 16:54:40.263055 queue_kv-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-04-24 13:02:36.000000 queue_kv-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      642 2024-04-25 16:54:37.000000 queue_kv-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 16:54:40.263055 queue_kv-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.253055 queue_kv-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.253055 queue_kv-0.1.2/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.253055 queue_kv-0.1.2/src/q/kv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-04-24 13:02:36.000000 queue_kv-0.1.2/src/q/kv/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-04-24 13:02:36.000000 queue_kv-0.1.2/src/q/kv/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2198 2024-04-25 16:50:10.000000 queue_kv-0.1.2/src/q/kv/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-04-25 07:26:10.000000 queue_kv-0.1.2/src/q/kv/append.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.263055 queue_kv-0.1.2/src/queue_kv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-28 09:02:23.564165 queue_kv-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-04-24 13:02:36.000000 queue_kv-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      642 2024-04-28 09:02:21.000000 queue_kv-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-28 09:02:23.564165 queue_kv-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/q/kv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-04-24 13:02:36.000000 queue_kv-0.1.3/src/q/kv/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-04-24 13:02:36.000000 queue_kv-0.1.3/src/q/kv/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2242 2024-04-28 09:02:10.000000 queue_kv-0.1.3/src/q/kv/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-04-25 07:26:10.000000 queue_kv-0.1.3/src/q/kv/append.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/queue_kv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/top_level.txt
```

### Comparing `queue_kv-0.1.2/PKG-INFO` & `queue_kv-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-kv
-Version: 0.1.2
+Version: 0.1.3
 Summary: Async Queue API implementation based on a Key-Value api
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
```

### Comparing `queue_kv-0.1.2/pyproject.toml` & `queue_kv-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-kv"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Async Queue API implementation based on a Key-Value api"
 dependencies = [
   "queue-api", "kv-api", "pydantic", "lazy-loader"
 ]
```

### Comparing `queue_kv-0.1.2/src/q/kv/api.py` & `queue_kv-0.1.3/src/q/kv/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,17 @@
       key = I.head((await self._kv.keys()).unsafe())
       if key is None:
         await asyncio.sleep(self.poll_interval.total_seconds())
         return await self._read(id, remove)
     else:
       key = id
 
-    value = (await self._kv.read(key)).unsafe()
+    value = (await self._kv.read(key)).get_or(None)
+    if value is None:
+      return None
     if remove:
       (await self._kv.delete(key)).unsafe()
     return key, value
     
   def _items(self) -> AsyncIter[tuple[str, A]]:
     return self._kv.items().map(E.unsafe)
```

### Comparing `queue_kv-0.1.2/src/q/kv/append.py` & `queue_kv-0.1.3/src/q/kv/append.py`

 * *Files identical despite different names*

### Comparing `queue_kv-0.1.2/src/queue_kv.egg-info/PKG-INFO` & `queue_kv-0.1.3/src/queue_kv.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-kv
-Version: 0.1.2
+Version: 0.1.3
 Summary: Async Queue API implementation based on a Key-Value api
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
```

