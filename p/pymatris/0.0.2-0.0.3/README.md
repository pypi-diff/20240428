# Comparing `tmp/pymatris-0.0.2.tar.gz` & `tmp/pymatris-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatris-0.0.2.tar", max compression
+gzip compressed data, was "pymatris-0.0.3.tar", max compression
```

## Comparing `pymatris-0.0.2.tar` & `pymatris-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-24 15:10:23.511842 pymatris-0.0.2/README.md
--rw-r--r--   0        0        0      219 2024-04-27 07:16:12.969026 pymatris-0.0.2/pymatris/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-27 14:16:42.070918 pymatris-0.0.2/pymatris/config.py
--rw-r--r--   0        0        0     9341 2024-04-27 16:32:48.694720 pymatris-0.0.2/pymatris/downloader.py
--rw-r--r--   0        0        0     2231 2024-04-26 19:42:44.665309 pymatris-0.0.2/pymatris/exceptions.py
--rw-r--r--   0        0        0     3263 2024-04-27 17:10:38.232578 pymatris-0.0.2/pymatris/main.py
--rw-r--r--   0        0        0      383 2024-04-27 07:15:55.830710 pymatris-0.0.2/pymatris/protocol_handler/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-27 07:02:20.960570 pymatris-0.0.2/pymatris/protocol_handler/base_handler.py
--rw-r--r--   0        0        0     3922 2024-04-27 17:47:25.305324 pymatris-0.0.2/pymatris/protocol_handler/ftp_handler.py
--rw-r--r--   0        0        0     6037 2024-04-27 14:11:03.287274 pymatris-0.0.2/pymatris/protocol_handler/http_handler.py
--rw-r--r--   0        0        0     4632 2024-04-27 14:11:15.838959 pymatris-0.0.2/pymatris/protocol_handler/sftp_handler.py
--rw-r--r--   0        0        0     2678 2024-04-27 14:26:25.268375 pymatris-0.0.2/pymatris/results.py
--rw-r--r--   0        0        0    11575 2024-04-27 13:34:05.879408 pymatris-0.0.2/pymatris/utils.py
--rw-r--r--   0        0        0      448 2024-04-27 07:13:12.702212 pymatris-0.0.2/pymatris/write_worker.py
--rw-r--r--   0        0        0     1144 2024-04-28 06:37:38.266623 pymatris-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 pymatris-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2024-04-28 09:05:53.220166 pymatris-0.0.3/README.md
+-rw-r--r--   0        0        0      219 2024-04-27 07:16:12.969026 pymatris-0.0.3/pymatris/__init__.py
+-rw-r--r--   0        0        0     1585 2024-04-28 08:16:42.281544 pymatris-0.0.3/pymatris/config.py
+-rw-r--r--   0        0        0     9361 2024-04-28 08:12:47.055380 pymatris-0.0.3/pymatris/downloader.py
+-rw-r--r--   0        0        0     2231 2024-04-26 19:42:44.665309 pymatris-0.0.3/pymatris/exceptions.py
+-rw-r--r--   0        0        0     3121 2024-04-28 08:15:48.491740 pymatris-0.0.3/pymatris/main.py
+-rw-r--r--   0        0        0      383 2024-04-27 07:15:55.830710 pymatris-0.0.3/pymatris/protocol_handler/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-27 07:02:20.960570 pymatris-0.0.3/pymatris/protocol_handler/base_handler.py
+-rw-r--r--   0        0        0     3954 2024-04-28 07:47:18.435122 pymatris-0.0.3/pymatris/protocol_handler/ftp_handler.py
+-rw-r--r--   0        0        0     5962 2024-04-28 07:46:54.106293 pymatris-0.0.3/pymatris/protocol_handler/http_handler.py
+-rw-r--r--   0        0        0     4272 2024-04-28 07:46:19.109729 pymatris-0.0.3/pymatris/protocol_handler/sftp_handler.py
+-rw-r--r--   0        0        0     2678 2024-04-27 14:26:25.268375 pymatris-0.0.3/pymatris/results.py
+-rw-r--r--   0        0        0    11229 2024-04-28 08:11:13.617397 pymatris-0.0.3/pymatris/utils.py
+-rw-r--r--   0        0        0      448 2024-04-28 07:42:56.434667 pymatris-0.0.3/pymatris/write_worker.py
+-rw-r--r--   0        0        0     1144 2024-04-28 09:06:47.436604 pymatris-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 pymatris-0.0.3/PKG-INFO
```

### Comparing `pymatris-0.0.2/pymatris/config.py` & `pymatris-0.0.3/pymatris/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,22 +15,14 @@
         "User-Agent": f"Pymatris Agent"
         f" aiohttp/{aiohttp.__version__}"
         f" python/{platform.python_version()}"
     }
 
 
 def _default_aiohttp_session(config: "SessionConfig") -> aiohttp.ClientSession:
-    """
-    The aiohttp session with the kwargs stored by this config.
-
-    Notes
-    -----
-    `aiohttp.ClientSession` expects to be instantiated in a asyncio context
-    where it can get a running loop.
-    """
     return aiohttp.ClientSession(headers=config.headers)
 
 
 @dataclass
 class SessionConfig:
     headers: Optional[Dict[str, str]] = field(default_factory=_default_headers)
     chunksize: float = 1024
@@ -45,15 +37,15 @@
 
 @dataclass
 class DownloaderConfig:
     """
     Hold all downloader session state.
     """
 
-    max_conn: int = 5
+    max_parallel: int = 5
     max_splits: int = 5
     all_progress: bool = True
     overwrite: bool = True
     config: Optional[SessionConfig] = field(default_factory=SessionConfig)
 
     def __post_init__(self):
         if self.config is None:
```

### Comparing `pymatris-0.0.2/pymatris/downloader.py` & `pymatris-0.0.3/pymatris/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 import threading
 import warnings
 
 
 class Downloader:
     def __init__(
         self,
-        max_conn: int = 5,
+        max_parallel: int = 5,
         max_splits: int = 5,
         all_progress: bool = True,
         overwrite: bool = True,
         session_config: Optional[SessionConfig] = None,
     ):
         self.config = DownloaderConfig(
-            max_conn=max_conn,
+            max_parallel=max_parallel,
             max_splits=max_splits,
             all_progress=all_progress,
             overwrite=overwrite,
             config=session_config,
         )
         self.download_queue = _QueueList()  # Queue that will hold all download task
         self._configure_logging()  # Configure logging
@@ -82,16 +82,16 @@
         self.download_queue.append((url, filepath, overwrite, kwargs))
 
     @property
     def queued_downloads(self):
         return len(self.download_queue)
 
     def _generate_tokens(self):
-        queue = asyncio.Queue(maxsize=self.config.max_conn)
-        for i in range(self.config.max_conn):
+        queue = asyncio.Queue(maxsize=self.config.max_parallel)
+        for i in range(self.config.max_parallel):
             queue.put_nowait(Token(i + 1))
         return queue
 
     def _format_results_and_remove_tempfile(
         self, dl_results: Results, main_pb: Optional[tqdm_std]
     ):
         errors = sum([isinstance(i, FailedDownload) for i in dl_results])
```

### Comparing `pymatris-0.0.2/pymatris/exceptions.py` & `pymatris-0.0.3/pymatris/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.2/pymatris/main.py` & `pymatris-0.0.3/pymatris/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "urls",
         metavar="URLS",
         type=str,
         nargs="+",
         help="URLs of files to be downloaded.",
     )
     parser.add_argument(
-        "--max-conn",
+        "--max-parallel",
         type=int,
         default=5,
         help="Maximum number of parallel file downloads.",
     )
     parser.add_argument(
         "--max-splits",
         type=int,
@@ -52,22 +52,14 @@
         action="store_const",
         const=True,
         default=False,
         dest="no_file_progress",
         help="Show progress bar for each file.",
     )
     parser.add_argument(
-        "--print-filenames",
-        action="store_const",
-        const=True,
-        default=False,
-        dest="print_filenames",
-        help="Print successfully downloaded files's names to stdout.",
-    )
-    parser.add_argument(
         "--show-errors",
         action="store_const",
         const=True,
         default=False,
         dest="show_errors",
         help="Show failed downloads with its errors to stderr.",
     )
@@ -75,38 +67,44 @@
         "--verbose",
         action="store_const",
         const=True,
         default=False,
         help="Log debugging output while transferring the files.",
     )
     args = parser.parse_args(args)
+
+    # If no arguments are provided, print the help menu
+    if not args:
+        parser.print_help()
+        exit()
+
     return args
 
 
 def run_pymatris(args):
     log_level = "DEBUG" if args.verbose else None
     config = SessionConfig(
         file_progress=not args.no_file_progress,
         log_level=log_level,
     )
 
     downloader = Downloader(
-        max_conn=args.max_conn,
+        max_parallel=args.max_parallel,
         max_splits=args.max_splits,
         all_progress=not args.no_progress,
         overwrite=args.overwrite,
         session_config=config,
     )
+
     for url in args.urls:
         downloader.enqueue_file(url, path=args.directory)
     results = downloader.download()
 
-    if args.print_filenames:
-        for i in results:
-            print(i + " downloaded")
+    for i in results:
+        print(i + " downloaded")
 
     if args.show_errors:
         err_str = ""
         if results.errors:
             err_str += "\nErrors:\n"
             for err in results.errors:
                 err_str += f"{repr(err)}"
```

### Comparing `pymatris-0.0.2/pymatris/protocol_handler/base_handler.py` & `pymatris-0.0.3/pymatris/protocol_handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.2/pymatris/protocol_handler/ftp_handler.py` & `pymatris-0.0.3/pymatris/protocol_handler/ftp_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .base_handler import ProtocolHandler
 import urllib
 from pymatris.utils import (
     allocate_tempfile,
     get_filepath,
     get_ftp_size,
     cancel_task,
+    retry_ftp,
 )
 import pymatris
 from pymatris.exceptions import FailedDownload
 from pymatris.write_worker import async_write_worker
 import asyncio
 import aioftp
 
@@ -27,90 +28,104 @@
         max_splits=None,
         max_tries=None,
         pb_callback=None,
         **kwargs,
     ):
         filepath = tmpfilepath = writer = None
         chunksize = chunksize or config.chunksize
+
         parse = urllib.parse.urlparse(url)
+
+        # Prepare kwargs for retries handler
+        kwargs["max_tries"] = max_tries or config.max_tries
+        kwargs["url"] = url
+
+        # Prepare files
         filepath = get_filepath(filepath_partial(None, url), overwrite)
         tmpfilepath = allocate_tempfile(str(filepath))
 
         try:
-            async with aioftp.Client.context(
-                parse.hostname, parse.port, parse.username, parse.password
-            ) as client:
-                pymatris.log.debug(
-                    "Connected to ftp server %s with credentials %s %s",
-                    parse.hostname,
-                    parse.username,
-                    parse.password,
-                )
-                # if parse.username and parse.password:
-                #     await client.login(user=parse.username, password=parse.password)
-                #     pymatris.log.debug(
-                #         "Logged in to ftp server %s with credentials %s %s",
-                #         parse.username,
-                #         parse.password,
-                #     )
-
-                total_size = await get_ftp_size(client, parse.path)
-
-                if callable(file_pb):
-                    file_pb = file_pb(
-                        position=token.n,
-                        unit="B",
-                        unit_scale=True,
-                        desc=filepath.name,
-                        leave=False,
-                        total=total_size,
-                    )
-                else:
-                    file_pb = None
-                pymatris.log.debug(
-                    "Downloading ftp file %s from %s", parse.path, parse.hostname
-                )
-                async with client.download_stream(parse.path) as stream:
-                    downloaded_chunks_queue = asyncio.Queue()
-                    download_workers = []
-                    writer = asyncio.create_task(
-                        async_write_worker(
-                            downloaded_chunks_queue, file_pb, tmpfilepath
-                        )
-                    )
-
-                    download_workers.append(
-                        asyncio.create_task(
-                            self._download_worker(
-                                stream, chunksize, downloaded_chunks_queue
-                            )
-                        )
-                    )
-
-                    await asyncio.gather(*download_workers)
-                    await downloaded_chunks_queue.join()
-
-                    return url, str(filepath), str(tmpfilepath)
-
+            await self._connect_and_download(
+                parse=parse,
+                filepath=filepath,
+                tmpfilepath=tmpfilepath,
+                token=token,
+                file_pb=file_pb,
+                chunksize=chunksize,
+                writer=writer,
+                **kwargs,
+            )
+            return url, str(filepath), str(tmpfilepath)
         except (Exception, asyncio.CancelledError) as e:
             if writer is not None:
                 await cancel_task(writer)
                 writer = None
-
-            # if tmpfilepath is not None:
-            #     remove_file(str(tmpfilepath))
-
             raise FailedDownload(filepath or filepath_partial, url, e) from e
-
         finally:
             if writer is not None:
                 writer.cancel()
-
-            # replace_tempfile(str(tmpfilepath))
             pb_callback(file_pb)
 
+    @retry_ftp
+    async def _connect_and_download(
+        self,
+        parse,
+        filepath,
+        tmpfilepath,
+        token,
+        file_pb,
+        chunksize,
+        writer,
+        **kwargs,
+    ):
+        async with aioftp.Client.context(
+            parse.hostname, parse.port, parse.username, parse.password
+        ) as client:
+            pymatris.log.debug(
+                "Connected to ftp server %s with credentials %s %s",
+                parse.hostname,
+                parse.username,
+                parse.password,
+            )
+
+            total_size = await get_ftp_size(client, parse.path)
+
+            if callable(file_pb):
+                file_pb = file_pb(
+                    position=token.n,
+                    unit="B",
+                    unit_scale=True,
+                    desc=filepath.name,
+                    leave=False,
+                    total=total_size,
+                )
+            else:
+                file_pb = None
+            pymatris.log.debug(
+                "Downloading ftp file %s from %s", parse.path, parse.hostname
+            )
+            async with client.download_stream(parse.path) as stream:
+                downloaded_chunks_queue = asyncio.Queue()
+                download_workers = []
+                writer = asyncio.create_task(
+                    async_write_worker(downloaded_chunks_queue, file_pb, tmpfilepath)
+                )
+
+                download_workers.append(
+                    asyncio.create_task(
+                        self._download_worker(
+                            stream, chunksize, downloaded_chunks_queue
+                        )
+                    )
+                )
+
+                await asyncio.gather(*download_workers)
+                await downloaded_chunks_queue.join()
+                # Cleanup
+                writer.cancel()
+
     async def _download_worker(self, stream, chunksize, queue):
         offset = 0
         async for chunk in stream.iter_by_block(chunksize):
             # Write this chunk to the output file.
             await queue.put((offset, chunk))
             offset += len(chunk)
```

### Comparing `pymatris-0.0.2/pymatris/protocol_handler/http_handler.py` & `pymatris-0.0.3/pymatris/protocol_handler/http_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pymatris.utils import (
     get_filepath,
     allocate_tempfile,
     get_http_size,
     cancel_task,
-    retry,
+    retry_http,
     generate_range,
 )
 from pymatris.exceptions import (
     FailedDownload,
     FailedHTTPRequestError,
     MultiPartDownloadError,
 )
@@ -102,35 +102,33 @@
                             **kwargs,
                         )
                     )
                 )
 
             await asyncio.gather(*tasks)
             await downloaded_chunk_queue.join()
+
+            # Cleanup
+            writer.cancel()
             return url, str(filepath), str(tmpfilepath)
 
         except (Exception, asyncio.CancelledError) as e:
             for task in tasks:
                 task.cancel()
             if writer is not None:
                 await cancel_task(writer)
                 writer = None
-
-            # if tmpfilepath is not None:
-            #     remove_file(str(tmpfilepath))
-
             raise FailedDownload(filepath or filepath_partial, url, e) from e
         finally:
             # Cancel idle writer
             if writer is not None:
                 writer.cancel()
-            # replace_tempfile(str(tmpfilepath))
             pb_callback(file_pb)
 
-    @retry
+    @retry_http
     async def _get_download_info(self, config, session, url, **kwargs):
         additional_headers = kwargs.pop("headers", {})
         headers = {**config.headers, **additional_headers}
         # Might get no response at all, which is likely a client error, including ssl, proxy, auth, etc.
         # But they are handled in retry decorator.
         async with session.head(
             url,
@@ -152,15 +150,15 @@
                 resp.headers,
             )
             if resp.status < 200 or resp.status >= 400:
                 raise FailedHTTPRequestError(resp)
             redirectUrl = resp.headers.get("Location", url)
             return resp, redirectUrl
 
-    @retry
+    @retry_http
     async def _download_worker(
         self, config, session, url, chunksize, http_range, queue, **kwargs
     ):
         additionl_headers = kwargs.pop("headers", {})
         headers = {**config.headers, **additionl_headers}
         if http_range:
             headers["Range"] = "bytes={}-{}".format(*http_range)
```

### Comparing `pymatris-0.0.2/pymatris/protocol_handler/sftp_handler.py` & `pymatris-0.0.3/pymatris/protocol_handler/sftp_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .base_handler import ProtocolHandler
 import urllib
 from pymatris.utils import (
     allocate_tempfile,
     get_filepath,
     get_ftp_size,
     generate_range,
-    retry_sftp,
+    retry_ftp,
     cancel_task,
 )
 from pymatris.write_worker import async_write_worker
 from pymatris.exceptions import FailedDownload
 import asyncio
 import asyncssh
 
@@ -27,35 +27,31 @@
         file_pb=None,
         chunksize=None,
         max_splits=None,
         max_tries=None,
         pb_callback=None,
         **kwargs,
     ):
-        filepath = tmpfilepath = writer = conn = sftp_client = file = None
+        filepath = tmpfilepath = writer = conn = sftp_client = file_reader = None
         chunksize = chunksize or config.chunksize
         max_splits = max_splits or config.max_splits
+
+        parse = urllib.parse.urlparse(url)
+
+        # Prepare for retry handler
         kwargs["max_tries"] = max_tries or config.max_tries
         kwargs["url"] = url
 
-        parse = urllib.parse.urlparse(url)
+        # Prepare files
+        filepath = get_filepath(filepath_partial(None, url), overwrite)
+        tmpfilepath = allocate_tempfile(str(filepath))
+
         try:
             conn, sftp_client = await self._connect_host(parse, **kwargs)
-            # async with asyncssh.connect(
-            #     parse.hostname,
-            #     username=parse.username,
-            #     password=parse.password,
-            #     port=parse.port or 22,
-            #     known_hosts=None,
-            #     **kwargs,
-            # ) as conn:
-            #     async with conn.start_sftp_client() as sftp:
-            filepath = get_filepath(filepath_partial(None, url), overwrite)
-            tmpfilepath = allocate_tempfile(str(filepath))
-            # Can throw FileNotFoundError
+
             total_size = await get_ftp_size(sftp_client, parse.path)
 
             if callable(file_pb) and total_size:
                 file_pb = file_pb(
                     position=token.n,
                     unit="B",
                     unit_scale=True,
@@ -64,71 +60,70 @@
                     total=total_size,
                 )
             else:
                 file_pb = None
 
             # Generate tasks to read into queue
             ranges = generate_range(content_length=total_size, max_splits=max_splits)
-            file = await sftp_client.open(parse.path, "rb")
+            # open for random binary access
+            file_reader = await sftp_client.open(parse.path, "rb")
+
             downloaded_chunks_queue = asyncio.Queue()
             writer = asyncio.create_task(
                 async_write_worker(downloaded_chunks_queue, file_pb, tmpfilepath)
             )
             tasks = []
             pymatris.log.debug(
-                "Downloading sftp file %s from %s", parse.path, parse.hostname
+                "Downloading sftp file  %s from %s", parse.path, parse.hostname
             )
             for _range in ranges:
                 tasks.append(
                     asyncio.create_task(
                         self._download_worker(
-                            file, _range[0], chunksize, downloaded_chunks_queue
+                            file_reader, _range[0], chunksize, downloaded_chunks_queue
                         )
                     )
                 )
 
             await asyncio.gather(*tasks)
             await downloaded_chunks_queue.join()  # Ensure all chunks are written
 
-            await file.close()
+            # Cleanup
+            await file_reader.close()
             sftp_client.exit()
             conn.close()
+            writer.cancel()
             return url, str(filepath), str(tmpfilepath)
 
         except (Exception, asyncio.CancelledError) as e:
             if writer:
                 await cancel_task(writer)
                 writer = None
-                # if tmpfilepath is not None:
-                #     remove_file(tmpfilepath)
-                filepath = None
-            if file is not None:
-                await file.close()
+            if file_reader is not None:
+                await file_reader.close()
             if sftp_client is not None:
                 sftp_client.exit()
             if conn is not None:
                 conn.close()
             raise FailedDownload(filepath or filepath_partial, url, e) from e
         finally:
             if writer:
                 writer.cancel()
-
-            # replace_tempfile(str(tmpfilepath))
             pb_callback(file_pb)
 
-    async def _download_worker(self, file, offset, chunksize, queue):
+    async def _download_worker(self, file_reader, offset, chunksize, queue):
         while True:
-            await file.seek(offset)
-            chunk = await file.read(chunksize)
+            await file_reader.seek(offset)
+            chunk = await file_reader.read(chunksize)
             if not chunk:
                 break
             await queue.put((offset, chunk))
             offset += len(chunk)
 
-    @retry_sftp
+    @retry_ftp
     async def _connect_host(self, parse, **kwargs):
         conn = await asyncssh.connect(
             parse.hostname,
             username=parse.username,
             password=parse.password,
             port=parse.port or 22,
             known_hosts=None,
```

### Comparing `pymatris-0.0.2/pymatris/results.py` & `pymatris-0.0.3/pymatris/results.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.2/pymatris/utils.py` & `pymatris-0.0.3/pymatris/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,110 +246,107 @@
     mv = memoryview(b)
     with open(filename, "rb", buffering=0) as f:
         for n in iter(lambda: f.readinto(mv), 0):
             h.update(mv[:n])
     return h.hexdigest()
 
 
-def retry(coro_func):
+def retry_http(coro_func):
     async def wrapper(self, *args, **kwargs):
         max_tries = kwargs.pop(
             "max_tries"
         )  # Have to use this workaround to get the max_tries without using parameterized decorator
         cur_url = args[2]  # Get URL
         tried = 0
         while True:
             tried += 1
             try:
                 return await coro_func(self, *args, **kwargs)
+            except asyncio.TimeoutError:
+                # From https://github.com/cshuaimin/aiodl
+                # Usually server has a fixed TCP timeout to clean dead
+                # connections, might have a lot of timeouts appear
+                # So retry it without checking the max retries.
+                tqdm_std.write("%s() timeout, retry in 1 second" % coro_func.__name__)
+                await asyncio.sleep(1)
             except (
                 MultiPartDownloadError,
                 FailedHTTPRequestError,
                 aiohttp.ClientError,
                 socket.gaierror,
             ) as exc:
                 if tried < max_tries:
                     # Exponential backoff
                     sec = tried / 2
-                    message = "%s(%s) failed: retry in %.1f seconds (%d/%d)" % (
-                        coro_func.__name__,
+                    message = "(%s) failed: retry in %.1f seconds (%d/%d)" % (
                         cur_url,
                         sec,
                         tried,
                         max_tries,
                     )
                     tqdm_std.write(message)
                     pymatris.log.debug(message)
                     await asyncio.sleep(sec)
                 else:
-                    message = "%s(%s) failed after %d tries: " % (
-                        coro_func.__name__,
+                    message = "(%s) failed after %d tries: " % (
                         cur_url,
                         max_tries,
                     )
                     tqdm_std.write(message)
                     pymatris.log.debug(message)
                     if isinstance(
                         exec, (MultiPartDownloadError, FailedHTTPRequestError)
                     ):
                         exec.retry = tried
                         exec.max_retries = max_tries
                     raise exc
-            except asyncio.TimeoutError:
-                # Usually server has a fixed TCP timeout to clean dead
-                # connections, so you can see a lot of timeouts appear
-                # at the same time. I don't think this is an error,
-                # So retry it without checking the max retries.
-                tqdm_std.write("%s() timeout, retry in 1 second" % coro_func.__name__)
-                await asyncio.sleep(1)
 
     return wrapper
 
 
-def retry_sftp(coro_func):
+def retry_ftp(coro_func):
     async def wrapper(self, *args, **kwargs):
         max_tries = kwargs.pop(
             "max_tries"
         )  # Have to use this workaround to get the max_tries without using parameterized decorator
         cur_url = kwargs.pop("url")  # Get URL
         tried = 0
         while True:
             tried += 1
             try:
                 return await coro_func(self, *args, **kwargs)
-            except (asyncssh.SFTPError, socket.gaierror) as exc:
+            except asyncio.TimeoutError:
+                tqdm_std.write("%s() timeout, retry in 1 second" % coro_func.__name__)
+                await asyncio.sleep(1)
+            except (
+                asyncssh.SFTPError,
+                aioftp.AIOFTPException,
+                socket.gaierror,
+                Exception,
+            ) as exc:
                 if tried < max_tries:
                     # Exponential backoff
                     sec = tried / 2
-                    message = "%s(%s) failed: retry in %.1f seconds (%d/%d)" % (
-                        coro_func.__name__,
+                    message = "(%s) failed: retry in %.1f seconds (%d/%d)" % (
                         cur_url,
                         sec,
                         tried,
                         max_tries,
                     )
                     tqdm_std.write(message)
                     pymatris.log.debug(message)
                     await asyncio.sleep(sec)
                 else:
-                    message = "%s(%s) failed after %d tries: " % (
-                        coro_func.__name__,
+                    message = "(%s) failed after %d tries: " % (
                         cur_url,
                         max_tries,
                     )
                     tqdm_std.write(message)
                     pymatris.log.debug(message)
                     raise exc
-            except asyncio.TimeoutError:
-                # Usually server has a fixed TCP timeout to clean dead
-                # connections, so you can see a lot of timeouts appear
-                # at the same time. Since not network error so retry it
-                # without checking the max retries.
-                tqdm_std.write("%s() timeout, retry in 1 second" % coro_func.__name__)
-                await asyncio.sleep(1)
 
     return wrapper
 
 
 def run_task_in_thread(loop: asyncio.BaseEventLoop, coro: asyncio.Task):
     with ThreadPoolExecutor(max_workers=1) as aio_pool:
         try:
```

### Comparing `pymatris-0.0.2/pyproject.toml` & `pymatris-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymatris"
-version = "0.0.2"
+version = "0.0.3"
 description = "Parallel download manager for HTTP/HTTPS/FTP/SFTP protocols."
 authors = ["zhuolisam <zhuolisam0627@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pymatris" }]
 keywords = ["downloader", "download-manager", "http/https", "sftp", "ftp"]
 classifiers = [
     "Programming Language :: Python",
```

