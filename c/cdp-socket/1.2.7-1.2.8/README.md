# Comparing `tmp/cdp-socket-1.2.7.tar.gz` & `tmp/cdp-socket-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdp-socket-1.2.7.tar", last modified: Sun Feb 25 12:40:20 2024, max compression
+gzip compressed data, was "cdp-socket-1.2.8.tar", last modified: Sun Apr 28 09:54:48 2024, max compression
```

## Comparing `cdp-socket-1.2.7.tar` & `cdp-socket-1.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.854433 cdp-socket-1.2.7/
--rw-rw-rw-   0        0        0     1092 2024-01-24 22:25:32.000000 cdp-socket-1.2.7/LICENSE
--rw-rw-rw-   0        0        0       90 2023-12-31 18:18:59.000000 cdp-socket-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6087 2024-02-25 12:40:20.853436 cdp-socket-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4708 2024-01-29 18:12:52.000000 cdp-socket-1.2.7/README.md
--rw-rw-rw-   0        0        0      571 2023-11-27 07:27:45.000000 cdp-socket-1.2.7/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 cdp-socket-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       63 2024-01-24 23:12:32.000000 cdp-socket-1.2.7/requirements.txt
--rw-rw-rw-   0        0        0      121 2024-02-25 12:40:20.873008 cdp-socket-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1760 2024-01-24 22:36:35.000000 cdp-socket-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.812353 cdp-socket-1.2.7/src/
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.830452 cdp-socket-1.2.7/src/cdp_socket/
--rw-rw-rw-   0        0        0       92 2024-02-25 12:31:55.000000 cdp-socket-1.2.7/src/cdp_socket/__init__.py
--rw-rw-rw-   0        0        0      221 2023-12-16 14:03:12.000000 cdp-socket-1.2.7/src/cdp_socket/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.842431 cdp-socket-1.2.7/src/cdp_socket/files/
--rw-rw-rw-   0        0        0        0 2023-08-10 12:39:59.000000 cdp-socket-1.2.7/src/cdp_socket/files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.843431 cdp-socket-1.2.7/src/cdp_socket/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 cdp-socket-1.2.7/src/cdp_socket/scripts/__init__.py
--rw-rw-rw-   0        0        0      716 2023-08-13 13:15:19.000000 cdp-socket-1.2.7/src/cdp_socket/scripts/abstract.py
--rw-rw-rw-   0        0        0    11128 2024-02-25 12:30:48.000000 cdp-socket-1.2.7/src/cdp_socket/socket.py
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.847452 cdp-socket-1.2.7/src/cdp_socket/utils/
--rw-rw-rw-   0        0        0        0 2023-08-11 04:17:07.000000 cdp-socket-1.2.7/src/cdp_socket/utils/__init__.py
--rw-rw-rw-   0        0        0      995 2023-08-19 23:04:48.000000 cdp-socket-1.2.7/src/cdp_socket/utils/conn.py
--rw-rw-rw-   0        0        0     4140 2023-12-31 18:06:18.000000 cdp-socket-1.2.7/src/cdp_socket/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.851431 cdp-socket-1.2.7/src/cdp_socket.egg-info/
--rw-rw-rw-   0        0        0     6087 2024-02-25 12:40:20.000000 cdp-socket-1.2.7/src/cdp_socket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2024-02-25 12:40:20.000000 cdp-socket-1.2.7/src/cdp_socket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 12:40:20.000000 cdp-socket-1.2.7/src/cdp_socket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-02-25 12:40:20.000000 cdp-socket-1.2.7/src/cdp_socket.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-25 12:40:20.000000 cdp-socket-1.2.7/src/cdp_socket.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-25 12:40:20.850432 cdp-socket-1.2.7/tests/
--rw-rw-rw-   0        0        0      978 2023-12-31 18:17:22.000000 cdp-socket-1.2.7/tests/check_event.py
--rw-rw-rw-   0        0        0     3491 2023-12-31 18:14:04.000000 cdp-socket-1.2.7/tests/test_socket.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:48.064320 cdp-socket-1.2.8/
+-rw-rw-rw-   0        0        0     1092 2024-01-24 22:25:32.000000 cdp-socket-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0       90 2023-12-31 18:18:59.000000 cdp-socket-1.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5966 2024-04-28 09:54:48.064320 cdp-socket-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4708 2024-01-29 18:12:52.000000 cdp-socket-1.2.8/README.md
+-rw-rw-rw-   0        0        0      571 2023-11-27 07:27:45.000000 cdp-socket-1.2.8/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 cdp-socket-1.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2024-03-26 14:04:31.000000 cdp-socket-1.2.8/requirements.txt
+-rw-rw-rw-   0        0        0      121 2024-04-28 09:54:48.075319 cdp-socket-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2024-01-24 22:36:35.000000 cdp-socket-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:47.941329 cdp-socket-1.2.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:47.982424 cdp-socket-1.2.8/src/cdp_socket/
+-rw-rw-rw-   0        0        0       92 2024-04-28 09:54:10.000000 cdp-socket-1.2.8/src/cdp_socket/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-12-16 14:03:12.000000 cdp-socket-1.2.8/src/cdp_socket/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:48.038648 cdp-socket-1.2.8/src/cdp_socket/files/
+-rw-rw-rw-   0        0        0        0 2023-08-10 12:39:59.000000 cdp-socket-1.2.8/src/cdp_socket/files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:48.041646 cdp-socket-1.2.8/src/cdp_socket/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 cdp-socket-1.2.8/src/cdp_socket/scripts/__init__.py
+-rw-rw-rw-   0        0        0      716 2023-08-13 13:15:19.000000 cdp-socket-1.2.8/src/cdp_socket/scripts/abstract.py
+-rw-rw-rw-   0        0        0    11555 2024-04-28 09:50:58.000000 cdp-socket-1.2.8/src/cdp_socket/socket.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:48.051662 cdp-socket-1.2.8/src/cdp_socket/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-11 04:17:07.000000 cdp-socket-1.2.8/src/cdp_socket/utils/__init__.py
+-rw-rw-rw-   0        0        0      995 2023-08-19 23:04:48.000000 cdp-socket-1.2.8/src/cdp_socket/utils/conn.py
+-rw-rw-rw-   0        0        0     4140 2023-12-31 18:06:18.000000 cdp-socket-1.2.8/src/cdp_socket/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:48.035647 cdp-socket-1.2.8/src/cdp_socket.egg-info/
+-rw-rw-rw-   0        0        0     5966 2024-04-28 09:54:47.000000 cdp-socket-1.2.8/src/cdp_socket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2024-04-28 09:54:47.000000 cdp-socket-1.2.8/src/cdp_socket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:54:47.000000 cdp-socket-1.2.8/src/cdp_socket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-28 09:54:47.000000 cdp-socket-1.2.8/src/cdp_socket.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-28 09:54:47.000000 cdp-socket-1.2.8/src/cdp_socket.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:54:48.060303 cdp-socket-1.2.8/tests/
+-rw-rw-rw-   0        0        0    13617 2024-03-26 13:26:22.000000 cdp-socket-1.2.8/tests/check_event.py
+-rw-rw-rw-   0        0        0     3491 2024-03-26 13:27:50.000000 cdp-socket-1.2.8/tests/test_socket.py
```

### Comparing `cdp-socket-1.2.7/LICENSE` & `cdp-socket-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/PKG-INFO` & `cdp-socket-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdp-socket
-Version: 1.2.7
+Version: 1.2.8
 Summary: socket for handling chrome-developer-protocol connections
 Home-page: https://github.com/kaliiiiiiiiii/CDP-Socket
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 License: MIT
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/CDP-Socket
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/CDP-Socket/issues
@@ -21,20 +21,16 @@
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: websockets
-Requires-Dist: orjson
 Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
+License-File: LICENSE
 
 # CDP-Socket
 
 * Handle [Chrome-Developer-Protocol](https://chromedevtools.github.io/devtools-protocol/) connections
 
 ### Feel free to test my code!
```

### Comparing `cdp-socket-1.2.7/README.md` & `cdp-socket-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/build_upload.md` & `cdp-socket-1.2.8/build_upload.md`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/setup.py` & `cdp-socket-1.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/src/cdp_socket/scripts/abstract.py` & `cdp-socket-1.2.8/src/cdp_socket/scripts/abstract.py`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/src/cdp_socket/socket.py` & `cdp-socket-1.2.8/src/cdp_socket/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 import inspect
 import typing
 import json
 
 from cdp_socket.exceptions import CDPError, SocketExcitedError
 from cdp_socket.utils.conn import get_websock_url, get_json
 
+background_tasks = set()
+
+
+def safe_wrap_fut(fut: typing.Awaitable):
+    task = asyncio.ensure_future(fut)
+    background_tasks.add(task)
+    task.add_done_callback(background_tasks.discard)
+
 
 class SingleCDPSocket:
     def __init__(self, websock_url: str, timeout: float = 10, loop: asyncio.AbstractEventLoop = None,
                  max_size: int = 2 ** 20):
         self._task = None
         if not loop:
             loop = asyncio.get_running_loop()
@@ -113,27 +121,33 @@
             try:
                 del self._iter_callbacks[_id]
             except KeyError:
                 pass
             raise e
         return res
 
+    async def load_json(self, data):
+        try:
+            if sys.getsizeof(data) > 8000:
+                return await self._loop.run_in_executor(None, orjson.loads, data)
+            else:
+                return json.loads(data)
+        except orjson.JSONDecodeError:
+            return await self._loop.run_in_executor(None, json.loads, data)
+
     async def _rec_coro(self):
         # noinspection PyUnresolvedReferences
         try:
             async for data in self._ws:
                 try:
-                    if sys.getsizeof(data) > 8000:
-                        data = orjson.loads(data)
-                    else:
-                        data = json.loads(data)
+                    data = await self.load_json(data)
                 except Exception as e:
                     from cdp_socket import EXC_HANDLER
                     EXC_HANDLER(e)
-                    data = {"method":"DecodeError", "params":{"e":e}}
+                    data = {"method": "DecodeError", "params": {"e": e}}
                 err = data.get('error')
                 _id = data.get("id")
                 if err is None:
                     if _id is None:
                         method = data.get("method")
                         params = data.get("params")
                         callbacks: callable = self._events[method]
@@ -182,15 +196,15 @@
                     EXC_HANDLER(e)
             try:
                 res = callback(*args, **kwargs)
             except Exception as e:
                 EXC_HANDLER(e)
                 return
             if inspect.isawaitable(res):
-                asyncio.ensure_future(async_handle(res))
+                safe_wrap_fut(async_handle(res))
             return res
 
     async def close(self, code: int = 1000, reason: str = ''):
         if self._ws.open:
             try:
                 await self._ws.close(code=code, reason=reason)
             except AttributeError as e:
@@ -283,15 +297,14 @@
             def remove_sock(code, reason):
                 _id = socket.id
                 try:
                     del self._sockets[_id]
                 except KeyError:
                     pass
 
-
             socket.on_closed.append(remove_sock)
         return socket
 
     @property
     def host(self):
         return self._host
```

### Comparing `cdp-socket-1.2.7/src/cdp_socket/utils/conn.py` & `cdp-socket-1.2.8/src/cdp_socket/utils/conn.py`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/src/cdp_socket/utils/utils.py` & `cdp-socket-1.2.8/src/cdp_socket/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/src/cdp_socket.egg-info/PKG-INFO` & `cdp-socket-1.2.8/src/cdp_socket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdp-socket
-Version: 1.2.7
+Version: 1.2.8
 Summary: socket for handling chrome-developer-protocol connections
 Home-page: https://github.com/kaliiiiiiiiii/CDP-Socket
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 License: MIT
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/CDP-Socket
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/CDP-Socket/issues
@@ -21,20 +21,16 @@
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: websockets
-Requires-Dist: orjson
 Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
+License-File: LICENSE
 
 # CDP-Socket
 
 * Handle [Chrome-Developer-Protocol](https://chromedevtools.github.io/devtools-protocol/) connections
 
 ### Feel free to test my code!
```

### Comparing `cdp-socket-1.2.7/src/cdp_socket.egg-info/SOURCES.txt` & `cdp-socket-1.2.8/src/cdp_socket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdp-socket-1.2.7/tests/test_socket.py` & `cdp-socket-1.2.8/tests/test_socket.py`

 * *Files identical despite different names*

