# Comparing `tmp/pymatris-0.0.6.tar.gz` & `tmp/pymatris-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatris-0.0.6.tar", max compression
+gzip compressed data, was "pymatris-0.0.8.tar", max compression
```

## Comparing `pymatris-0.0.6.tar` & `pymatris-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5386 2024-04-28 14:57:19.644363 pymatris-0.0.6/README.md
--rw-r--r--   0        0        0      219 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/__init__.py
--rw-r--r--   0        0        0     2008 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/config.py
--rw-r--r--   0        0        0     9423 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/downloader.py
--rw-r--r--   0        0        0     2231 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/exceptions.py
--rw-r--r--   0        0        0     3365 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/main.py
--rw-r--r--   0        0        0      383 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/base_handler.py
--rw-r--r--   0        0        0     3988 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/ftp_handler.py
--rw-r--r--   0        0        0     5962 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/http_handler.py
--rw-r--r--   0        0        0     4306 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/sftp_handler.py
--rw-r--r--   0        0        0     2678 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/results.py
--rw-r--r--   0        0        0    11719 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/utils.py
--rw-r--r--   0        0        0      448 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/write_worker.py
--rw-r--r--   0        0        0     1144 2024-04-28 14:57:19.644363 pymatris-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6423 1970-01-01 00:00:00.000000 pymatris-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     5386 2024-04-28 16:02:23.088347 pymatris-0.0.8/README.md
+-rw-r--r--   0        0        0      219 2024-04-28 16:02:23.088347 pymatris-0.0.8/pymatris/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-28 16:02:23.088347 pymatris-0.0.8/pymatris/config.py
+-rw-r--r--   0        0        0     9423 2024-04-28 16:02:23.088347 pymatris-0.0.8/pymatris/downloader.py
+-rw-r--r--   0        0        0     2231 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/exceptions.py
+-rw-r--r--   0        0        0     3365 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/main.py
+-rw-r--r--   0        0        0      383 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/protocol_handler/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/protocol_handler/base_handler.py
+-rw-r--r--   0        0        0     3988 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/protocol_handler/ftp_handler.py
+-rw-r--r--   0        0        0     5962 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/protocol_handler/http_handler.py
+-rw-r--r--   0        0        0     4306 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/protocol_handler/sftp_handler.py
+-rw-r--r--   0        0        0     2678 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/results.py
+-rw-r--r--   0        0        0    11711 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/utils.py
+-rw-r--r--   0        0        0      448 2024-04-28 16:02:23.092347 pymatris-0.0.8/pymatris/write_worker.py
+-rw-r--r--   0        0        0     1144 2024-04-28 16:02:23.092347 pymatris-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6423 1970-01-01 00:00:00.000000 pymatris-0.0.8/PKG-INFO
```

### Comparing `pymatris-0.0.6/README.md` & `pymatris-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/config.py` & `pymatris-0.0.8/pymatris/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     chunksize: float = 1024
     file_progress: bool = True
     timeouts: int = 300  # Default to 5 min timeout
     log_level: Optional[str] = None
 
     def __post_init__(self):
         if self.log_level is None:
-            self.log_level = "debug" if "PYMATRIS_DEBUG" in os.environ else None
+            self.log_level = "DEBUG" if "PYMATRIS_DEBUG" in os.environ else None
 
         # Default minimum values
         if self.chunksize < 1:
             self.chunksize = 1
         if self.timeouts < 1:
             self.timeouts = 1
```

### Comparing `pymatris-0.0.6/pymatris/downloader.py` & `pymatris-0.0.8/pymatris/downloader.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/exceptions.py` & `pymatris-0.0.8/pymatris/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/main.py` & `pymatris-0.0.8/pymatris/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,23 +87,23 @@
 
     return args
 
 
 def run_pymatris(args):
     log_level = "DEBUG" if args.verbose else None
     config = SessionConfig(
-        max_tries=args.max_tries,
         timeouts=args.timeouts,
         file_progress=not args.quiet,
         log_level=log_level,
     )
 
     downloader = Downloader(
         max_parallel=args.max_parallel,
         max_splits=args.max_splits,
+        max_tries=args.max_tries,
         all_progress=not args.quiet,
         overwrite=args.overwrite,
         session_config=config,
     )
 
     for url in args.urls:
         downloader.enqueue_file(url, path=args.dir)
```

### Comparing `pymatris-0.0.6/pymatris/protocol_handler/base_handler.py` & `pymatris-0.0.8/pymatris/protocol_handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/protocol_handler/ftp_handler.py` & `pymatris-0.0.8/pymatris/protocol_handler/ftp_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/protocol_handler/http_handler.py` & `pymatris-0.0.8/pymatris/protocol_handler/http_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/protocol_handler/sftp_handler.py` & `pymatris-0.0.8/pymatris/protocol_handler/sftp_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/results.py` & `pymatris-0.0.8/pymatris/results.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.6/pymatris/utils.py` & `pymatris-0.0.8/pymatris/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,25 +337,25 @@
                     sec = tried / 2
                     message = "(%s) failed: retry in %.1f seconds (%d/%d)" % (
                         cur_url,
                         sec,
                         tried,
                         max_tries,
                     )
-                    # if config.file_progress:
-                    #     tqdm_std.write(message)
+                    if config.file_progress:
+                        tqdm_std.write(message)
                     pymatris.log.debug(message)
                     await asyncio.sleep(sec)
                 else:
                     message = "(%s) failed after %d tries: " % (
                         cur_url,
                         max_tries,
                     )
-                    # if config.file_progress:
-                    #     tqdm_std.write(message)
+                    if config.file_progress:
+                        tqdm_std.write(message)
                     pymatris.log.debug(message)
                     raise exc
 
     return wrapper
 
 
 def run_task_in_thread(loop: asyncio.BaseEventLoop, coro: asyncio.Task):
```

### Comparing `pymatris-0.0.6/pyproject.toml` & `pymatris-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymatris"
-version = "0.0.6"
+version = "0.0.8"
 description = "Parallel download manager for HTTP/HTTPS/FTP/SFTP protocols."
 authors = ["zhuolisam <zhuolisam0627@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pymatris" }]
 keywords = ["downloader", "download-manager", "http/https", "sftp", "ftp"]
 classifiers = [
     "Programming Language :: Python",
```

### Comparing `pymatris-0.0.6/PKG-INFO` & `pymatris-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatris
-Version: 0.0.6
+Version: 0.0.8
 Summary: Parallel download manager for HTTP/HTTPS/FTP/SFTP protocols.
 Keywords: downloader,download-manager,http/https,sftp,ftp
 Author: zhuolisam
 Author-email: zhuolisam0627@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

