# Comparing `tmp/pymatris-0.0.4.tar.gz` & `tmp/pymatris-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatris-0.0.4.tar", max compression
+gzip compressed data, was "pymatris-0.0.6.tar", max compression
```

## Comparing `pymatris-0.0.4.tar` & `pymatris-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2475 2024-04-28 09:35:29.636760 pymatris-0.0.4/README.md
--rw-r--r--   0        0        0      219 2024-04-27 07:16:12.969026 pymatris-0.0.4/pymatris/__init__.py
--rw-r--r--   0        0        0     1624 2024-04-28 09:19:15.477872 pymatris-0.0.4/pymatris/config.py
--rw-r--r--   0        0        0     9361 2024-04-28 08:12:47.055380 pymatris-0.0.4/pymatris/downloader.py
--rw-r--r--   0        0        0     2231 2024-04-26 19:42:44.665309 pymatris-0.0.4/pymatris/exceptions.py
--rw-r--r--   0        0        0     2888 2024-04-28 09:20:19.375576 pymatris-0.0.4/pymatris/main.py
--rw-r--r--   0        0        0      383 2024-04-27 07:15:55.830710 pymatris-0.0.4/pymatris/protocol_handler/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-27 07:02:20.960570 pymatris-0.0.4/pymatris/protocol_handler/base_handler.py
--rw-r--r--   0        0        0     3988 2024-04-28 09:16:43.135282 pymatris-0.0.4/pymatris/protocol_handler/ftp_handler.py
--rw-r--r--   0        0        0     5962 2024-04-28 07:46:54.106293 pymatris-0.0.4/pymatris/protocol_handler/http_handler.py
--rw-r--r--   0        0        0     4306 2024-04-28 09:16:50.944561 pymatris-0.0.4/pymatris/protocol_handler/sftp_handler.py
--rw-r--r--   0        0        0     2678 2024-04-27 14:26:25.268375 pymatris-0.0.4/pymatris/results.py
--rw-r--r--   0        0        0    11702 2024-04-28 09:20:02.646873 pymatris-0.0.4/pymatris/utils.py
--rw-r--r--   0        0        0      448 2024-04-28 07:42:56.434667 pymatris-0.0.4/pymatris/write_worker.py
--rw-r--r--   0        0        0     1144 2024-04-28 09:35:40.656849 pymatris-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 pymatris-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5386 2024-04-28 14:57:19.644363 pymatris-0.0.6/README.md
+-rw-r--r--   0        0        0      219 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/config.py
+-rw-r--r--   0        0        0     9423 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/downloader.py
+-rw-r--r--   0        0        0     2231 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/exceptions.py
+-rw-r--r--   0        0        0     3365 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/main.py
+-rw-r--r--   0        0        0      383 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/base_handler.py
+-rw-r--r--   0        0        0     3988 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/ftp_handler.py
+-rw-r--r--   0        0        0     5962 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/http_handler.py
+-rw-r--r--   0        0        0     4306 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/protocol_handler/sftp_handler.py
+-rw-r--r--   0        0        0     2678 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/results.py
+-rw-r--r--   0        0        0    11719 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/utils.py
+-rw-r--r--   0        0        0      448 2024-04-28 14:57:19.644363 pymatris-0.0.6/pymatris/write_worker.py
+-rw-r--r--   0        0        0     1144 2024-04-28 14:57:19.644363 pymatris-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6423 1970-01-01 00:00:00.000000 pymatris-0.0.6/PKG-INFO
```

### Comparing `pymatris-0.0.4/pymatris/config.py` & `pymatris-0.0.6/pymatris/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,40 +24,54 @@
 
 @dataclass
 class SessionConfig:
     headers: Optional[Dict[str, str]] = field(default_factory=_default_headers)
     chunksize: float = 1024
     file_progress: bool = True
     timeouts: int = 300  # Default to 5 min timeout
-    max_tries: int = 5
     log_level: Optional[str] = None
 
     def __post_init__(self):
         if self.log_level is None:
             self.log_level = "debug" if "PYMATRIS_DEBUG" in os.environ else None
 
+        # Default minimum values
+        if self.chunksize < 1:
+            self.chunksize = 1
+        if self.timeouts < 1:
+            self.timeouts = 1
+
 
 @dataclass
 class DownloaderConfig:
     """
     Hold all downloader session state.
     """
 
     max_parallel: int = 5
     max_splits: int = 5
+    max_tries: int = 5
     all_progress: bool = True
     overwrite: bool = True
     config: Optional[SessionConfig] = field(default_factory=SessionConfig)
 
     def __post_init__(self):
         if self.config is None:
             self.config = SessionConfig()
 
         # If all_progress is turned off, auto disable file progress as well
         if not self.all_progress:
             self.config.file_progress = False
 
+        # Default minimum values
+        if self.max_parallel < 1:
+            self.max_parallel = 1
+        if self.max_splits < 1:
+            self.max_splits = 1
+        if self.max_tries < 1:
+            self.max_tries = 1
+
     def __getattr__(self, __name: str):
         return getattr(self.config, __name)
 
     def aiohttp_client_session(self):
         return _default_aiohttp_session(self.config)
```

### Comparing `pymatris-0.0.4/pymatris/downloader.py` & `pymatris-0.0.6/pymatris/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 
 
 class Downloader:
     def __init__(
         self,
         max_parallel: int = 5,
         max_splits: int = 5,
+        max_tries: int = 5,
         all_progress: bool = True,
-        overwrite: bool = True,
+        overwrite: bool = False,
         session_config: Optional[SessionConfig] = None,
     ):
         self.config = DownloaderConfig(
             max_parallel=max_parallel,
             max_splits=max_splits,
+            max_tries=max_tries,
             all_progress=all_progress,
             overwrite=overwrite,
             config=session_config,
         )
         self.download_queue = _QueueList()  # Queue that will hold all download task
         self._configure_logging()  # Configure logging
         self.tqdm = tqdm_std  # Configure progress bar writer
```

### Comparing `pymatris-0.0.4/pymatris/exceptions.py` & `pymatris-0.0.6/pymatris/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.4/pymatris/main.py` & `pymatris-0.0.6/pymatris/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,41 +14,57 @@
         nargs="+",
         help="URLs of files to be downloaded.",
     )
     parser.add_argument(
         "--max-parallel",
         type=int,
         default=5,
+        dest="max_parallel",
         help="Maximum number of parallel file downloads.",
     )
     parser.add_argument(
         "--max-splits",
         type=int,
         default=5,
-        help="Maximum number of parallel connections per file (only used if supported by the server).",
+        dest="max_splits",
+        help="Maximum number of parallel connections per file (only if protocol and server is supported).",
+    )
+    parser.add_argument(
+        "--max-tries",
+        type=int,
+        default=5,
+        dest="max_tries",
+        help="Maximum number of download attempt per url.",
+    )
+    parser.add_argument(
+        "--timeouts",
+        type=int,
+        default=300,
+        dest="timeouts",
+        help="Maximum timeouts per url.",
     )
     parser.add_argument(
         "--dir",
         type=str,
         default="./",
         help="Directory to which downloaded files are saved.",
     )
     parser.add_argument(
         "--overwrite",
         action="store_const",
         const=True,
         default=False,
-        help="Overwrite if the file exists. Only one matched file will be overwritten",
+        help="Overwrite if file exists. Only one url with the clashing name will overwrite the file.",
     )
     parser.add_argument(
         "--quiet",
         action="store_const",
         const=True,
         default=False,
-        dest="quite",
+        dest="quiet",
         help="Show progress indicators and file retries if any during download.",
     )
     parser.add_argument(
         "--show-errors",
         action="store_const",
         const=True,
         default=False,
@@ -71,14 +87,16 @@
 
     return args
 
 
 def run_pymatris(args):
     log_level = "DEBUG" if args.verbose else None
     config = SessionConfig(
+        max_tries=args.max_tries,
+        timeouts=args.timeouts,
         file_progress=not args.quiet,
         log_level=log_level,
     )
 
     downloader = Downloader(
         max_parallel=args.max_parallel,
         max_splits=args.max_splits,
```

### Comparing `pymatris-0.0.4/pymatris/protocol_handler/base_handler.py` & `pymatris-0.0.6/pymatris/protocol_handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.4/pymatris/protocol_handler/ftp_handler.py` & `pymatris-0.0.6/pymatris/protocol_handler/ftp_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.4/pymatris/protocol_handler/http_handler.py` & `pymatris-0.0.6/pymatris/protocol_handler/http_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.4/pymatris/protocol_handler/sftp_handler.py` & `pymatris-0.0.6/pymatris/protocol_handler/sftp_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.4/pymatris/results.py` & `pymatris-0.0.6/pymatris/results.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.4/pymatris/utils.py` & `pymatris-0.0.6/pymatris/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,18 +263,18 @@
             try:
                 return await coro_func(self, *args, **kwargs)
             except asyncio.TimeoutError:
                 # From https://github.com/cshuaimin/aiodl
                 # Usually server has a fixed TCP timeout to clean dead
                 # connections, might have a lot of timeouts appear
                 # So retry it without checking the max retries.
+                message = "%s() timeout, retry in 1 second" % coro_func.__name__
                 # if config.file_progress:
-                #     tqdm_std.write(
-                #         "%s() timeout, retry in 1 second" % coro_func.__name__
-                #     )
+                #     tqdm_std.write(message)
+                pymatris.log.debug(message)
                 await asyncio.sleep(1)
             except (
                 MultiPartDownloadError,
                 FailedHTTPRequestError,
                 aiohttp.ClientError,
                 socket.gaierror,
             ) as exc:
@@ -318,19 +318,18 @@
         config = kwargs.pop("config")
         tried = 0
         while True:
             tried += 1
             try:
                 return await coro_func(self, *args, **kwargs)
             except asyncio.TimeoutError:
+                message = "%s() timeout, retry in 1 second" % coro_func.__name__
                 # if config.file_progress:
-                #     tqdm_std.write(
-                #         "%s() timeout, retry in 1 second" % coro_func.__name__
-                #     )
-                await asyncio.sleep(1)
+                #     tqdm_std.write(message)
+                pymatris.log.debug(message)
             except (
                 asyncssh.SFTPError,
                 aioftp.AIOFTPException,
                 socket.gaierror,
                 Exception,
             ) as exc:
                 if tried < max_tries:
```

### Comparing `pymatris-0.0.4/pyproject.toml` & `pymatris-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymatris"
-version = "0.0.4"
+version = "0.0.6"
 description = "Parallel download manager for HTTP/HTTPS/FTP/SFTP protocols."
 authors = ["zhuolisam <zhuolisam0627@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pymatris" }]
 keywords = ["downloader", "download-manager", "http/https", "sftp", "ftp"]
 classifiers = [
     "Programming Language :: Python",
```

