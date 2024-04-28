# Comparing `tmp/goroutine-py-1.0.7.tar.gz` & `tmp/goroutine_py-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goroutine-py-1.0.7.tar", last modified: Thu Jan  4 14:43:52 2024, max compression
+gzip compressed data, was "goroutine_py-1.0.8.tar", last modified: Sun Apr 28 04:16:30 2024, max compression
```

## Comparing `goroutine-py-1.0.7.tar` & `goroutine_py-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/
--rw-r--r--   0 louis      (501) staff       (20)     1065 2024-01-03 09:03:13.000000 goroutine-py-1.0.7/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     2651 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     2120 2024-01-04 14:42:38.000000 goroutine-py-1.0.7/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/goroutine/
--rw-r--r--   0 louis      (501) staff       (20)      239 2024-01-03 09:03:13.000000 goroutine-py-1.0.7/goroutine/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     3640 2024-01-03 09:03:13.000000 goroutine-py-1.0.7/goroutine/app.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/goroutine_py.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     2651 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/goroutine_py.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      215 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/goroutine_py.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/goroutine_py.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       10 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/goroutine_py.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)      512 2024-01-04 14:43:27.000000 goroutine-py-1.0.7/pyproject.toml
--rw-r--r--   0 louis      (501) staff       (20)       38 2024-01-04 14:43:52.000000 goroutine-py-1.0.7/setup.cfg
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/
+-rw-r--r--   0 louis      (501) staff       (20)     1065 2024-01-03 09:03:13.000000 goroutine_py-1.0.8/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     2651 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     2120 2024-01-04 14:42:38.000000 goroutine_py-1.0.8/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/goroutine/
+-rw-r--r--   0 louis      (501) staff       (20)      239 2024-01-03 09:03:13.000000 goroutine_py-1.0.8/goroutine/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     3601 2024-04-28 04:11:13.000000 goroutine_py-1.0.8/goroutine/app.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/goroutine_py.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     2651 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/goroutine_py.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      215 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/goroutine_py.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/goroutine_py.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       10 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/goroutine_py.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)      512 2024-04-28 04:14:35.000000 goroutine_py-1.0.8/pyproject.toml
+-rw-r--r--   0 louis      (501) staff       (20)       38 2024-04-28 04:16:30.000000 goroutine_py-1.0.8/setup.cfg
```

### Comparing `goroutine-py-1.0.7/LICENSE` & `goroutine_py-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `goroutine-py-1.0.7/PKG-INFO` & `goroutine_py-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goroutine-py
-Version: 1.0.7
+Version: 1.0.8
 Summary: An Asyncio-based concurrency library for Python.
 Author-email: xudesoft <xudesoft@126.com>
 Project-URL: Homepage, https://github.com/purplegrapeZz/goroutine-py
 Project-URL: Issues, https://github.com/purplegrapeZz/goroutine-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `goroutine-py-1.0.7/README.md` & `goroutine_py-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `goroutine-py-1.0.7/goroutine/app.py` & `goroutine_py-1.0.8/goroutine/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 '''
 
 __author__ = 'ZIHAN MA (xudesoft@126.com)'
 
 import asyncio
 from threading import Thread
 import functools
-from concurrent.futures import Future
-from asyncio import coroutine
+from asyncio.futures import Future
 
 
 def _run() -> None:
     '''
     Start loop.
     '''
     _goroutine_loop.run_forever()
@@ -26,25 +25,25 @@
     Check if obj a coroutinefunction.
     Return:
         True or Fale.
     '''
     return asyncio.iscoroutinefunction(obj)
 
 
-async def _wrap_as_cor(obj: callable, *args) -> coroutine:
+async def _wrap_as_cor(obj: callable, *args) -> Future:
     '''
     Wrap a func as a coroutine.
     Return:
         A coroutine.
     '''
     res = await asyncio.to_thread(obj, *args)
     return res
 
 
-async def _wrap_as_cor_withlock(obj: callable, *args) -> coroutine:
+async def _wrap_as_cor_withlock(obj: callable, *args) -> Future:
     '''
     Wrap a func as a coroutine with lock. Means thread safe.
     Return:
         A coroutine.
     '''
     async with _goroutine_loop_lock:
         res = await asyncio.to_thread(obj, *args)
@@ -118,12 +117,12 @@
             'A callable func or coroutinefunction object is required')
 
 
 # An asyncio-lock.
 _goroutine_loop_lock = asyncio.Lock()
 
 # Getting loop.
-_goroutine_loop = asyncio.get_event_loop()
+_goroutine_loop = asyncio.new_event_loop()
 
 # Run the loop in a thread.
 T = Thread(target=_run, daemon=True)
 T.start()
```

### Comparing `goroutine-py-1.0.7/goroutine_py.egg-info/PKG-INFO` & `goroutine_py-1.0.8/goroutine_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goroutine-py
-Version: 1.0.7
+Version: 1.0.8
 Summary: An Asyncio-based concurrency library for Python.
 Author-email: xudesoft <xudesoft@126.com>
 Project-URL: Homepage, https://github.com/purplegrapeZz/goroutine-py
 Project-URL: Issues, https://github.com/purplegrapeZz/goroutine-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `goroutine-py-1.0.7/pyproject.toml` & `goroutine_py-1.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "goroutine-py"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="xudesoft", email="xudesoft@126.com" },
 ]
 description = "An Asyncio-based concurrency library for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

