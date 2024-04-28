# Comparing `tmp/dot_proxy-0.1.0.tar.gz` & `tmp/dot_proxy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dot_proxy-0.1.0.tar", last modified: Sun Apr 28 04:55:29 2024, max compression
+gzip compressed data, was "dot_proxy-0.2.0.tar", last modified: Sun Apr 28 05:43:10 2024, max compression
```

## Comparing `dot_proxy-0.1.0.tar` & `dot_proxy-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 04:55:29.026848 dot_proxy-0.1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-04-28 02:24:07.000000 dot_proxy-0.1.0/.env
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-28 04:26:56.000000 dot_proxy-0.1.0/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      288 2024-04-28 04:24:49.000000 dot_proxy-0.1.0/Dockerfile
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1056 2024-04-28 04:22:32.000000 dot_proxy-0.1.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2877 2024-04-28 04:55:29.026848 dot_proxy-0.1.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1286 2024-04-28 04:53:27.000000 dot_proxy-0.1.0/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)      170 2024-04-28 02:54:36.000000 dot_proxy-0.1.0/docker-compose.yml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 04:55:29.026848 dot_proxy-0.1.0/dot_proxy.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2877 2024-04-28 04:55:29.000000 dot_proxy-0.1.0/dot_proxy.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      291 2024-04-28 04:55:29.000000 dot_proxy-0.1.0/dot_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 04:55:29.000000 dot_proxy-0.1.0/dot_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-28 04:55:29.000000 dot_proxy-0.1.0/dot_proxy.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-28 04:55:29.000000 dot_proxy-0.1.0/dot_proxy.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2024-04-28 04:55:29.000000 dot_proxy-0.1.0/dot_proxy.egg-info/top_level.txt
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     5792 2024-04-28 04:54:09.000000 dot_proxy-0.1.0/dot_proxy.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      714 2024-04-28 04:28:46.000000 dot_proxy-0.1.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-28 04:55:29.026848 dot_proxy-0.1.0/setup.cfg
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 05:43:10.228111 dot_proxy-0.2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-04-28 02:24:07.000000 dot_proxy-0.2.0/.env
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-28 04:26:56.000000 dot_proxy-0.2.0/.gitignore
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      288 2024-04-28 04:24:49.000000 dot_proxy-0.2.0/Dockerfile
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1056 2024-04-28 04:22:32.000000 dot_proxy-0.2.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3070 2024-04-28 05:43:10.228111 dot_proxy-0.2.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1479 2024-04-28 05:13:41.000000 dot_proxy-0.2.0/README.md
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      170 2024-04-28 02:54:36.000000 dot_proxy-0.2.0/docker-compose.yml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 05:43:10.228111 dot_proxy-0.2.0/dot_proxy.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3070 2024-04-28 05:43:10.000000 dot_proxy-0.2.0/dot_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      291 2024-04-28 05:43:10.000000 dot_proxy-0.2.0/dot_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 05:43:10.000000 dot_proxy-0.2.0/dot_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-28 05:43:10.000000 dot_proxy-0.2.0/dot_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-28 05:43:10.000000 dot_proxy-0.2.0/dot_proxy.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2024-04-28 05:43:10.000000 dot_proxy-0.2.0/dot_proxy.egg-info/top_level.txt
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     5456 2024-04-28 05:42:17.000000 dot_proxy-0.2.0/dot_proxy.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      714 2024-04-28 04:28:46.000000 dot_proxy-0.2.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-28 05:43:10.228111 dot_proxy-0.2.0/setup.cfg
```

### Comparing `dot_proxy-0.1.0/LICENSE` & `dot_proxy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dot_proxy-0.1.0/PKG-INFO` & `dot_proxy-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dot-proxy
-Version: 0.1.0
+Version: 0.2.0
 Summary: DNS over TLS Proxy Server
 Author: Sergey M
 License: Copyright 2024 Sergey M
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,14 +21,16 @@
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # README
 
+[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]()
+
 DNS over TLS Proxy Server for Non-Systemd Distros.
 
 ## Install and Run
 
 Via Docker Compose:
 
 ```bash
```

### Comparing `dot_proxy-0.1.0/README.md` & `dot_proxy-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # README
 
+[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]()
+
 DNS over TLS Proxy Server for Non-Systemd Distros.
 
 ## Install and Run
 
 Via Docker Compose:
 
 ```bash
```

### Comparing `dot_proxy-0.1.0/dot_proxy.egg-info/PKG-INFO` & `dot_proxy-0.2.0/dot_proxy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dot-proxy
-Version: 0.1.0
+Version: 0.2.0
 Summary: DNS over TLS Proxy Server
 Author: Sergey M
 License: Copyright 2024 Sergey M
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,14 +21,16 @@
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # README
 
+[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]()
+
 DNS over TLS Proxy Server for Non-Systemd Distros.
 
 ## Install and Run
 
 Via Docker Compose:
 
 ```bash
```

### Comparing `dot_proxy-0.1.0/dot_proxy.py` & `dot_proxy-0.2.0/dot_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python
 # pylint: disable=C,R,W
 """DNS over TLS Proxy Server"""
 import argparse
 import asyncio
 import logging
 import ssl
-import uuid
 from collections import deque
 from contextlib import asynccontextmanager
 from dataclasses import dataclass, field
 from typing import Any, AsyncIterator, Sequence
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __author__ = "Sergey M"
 
 
 @dataclass
 class DOTClient:
     host: str
     port: int = 853
-    id: str = field(default_factory=lambda: str(uuid.uuid4()))
     reader: asyncio.StreamReader = None
     writer: asyncio.StreamWriter = None
 
     async def connect(self) -> None:
         sslctx = ssl.create_default_context()
         self.reader, self.writer = await asyncio.open_connection(
             self.host, self.port, ssl=sslctx
@@ -48,25 +46,23 @@
     ) -> None:
         self._pool = deque(maxlen=max_clients)  # asyncio.Queue(max_clients)
         for _ in range(max_clients):
             client = DOTClient(*args, **kwargs)
             self._pool.append(client)
 
     @asynccontextmanager
-    async def get_client(
-        self, timeout: float = 0.1
-    ) -> AsyncIterator[DOTClient]:
-        client = await self.acquire_client(timeout)
-        logging.debug("get client: %r", client)
+    async def client(self, timeout: float = 0.1) -> AsyncIterator[DOTClient]:
+        client = await self.get_client(timeout)
+        logging.debug("get client: 0x%x", id(client))
         try:
             yield client
         finally:
             self.release_client(client)
 
-    async def acquire_client(self, timeout: float) -> DOTClient:
+    async def get_client(self, timeout: float) -> DOTClient:
         while True:
             try:
                 return self._pool.popleft()
             except IndexError:
                 await asyncio.sleep(timeout)
 
     def release_client(self, client: DOTClient) -> None:
@@ -78,47 +74,41 @@
         self,
         remote_host: str,
         remote_port: int = 853,
         max_clients: int = 10,
     ) -> None:
         self.client_pool = DOTClientPool(max_clients, remote_host, remote_port)
         self.done = asyncio.get_event_loop().create_future()
-        self.request_queue = asyncio.Queue()
-        self.task = asyncio.create_task(self.process())
 
     def connection_made(self, transport: asyncio.DatagramTransport) -> None:
         self.transport = transport
 
     def datagram_received(
         self, data: bytes, addr: tuple[str | Any, int]
     ) -> None:
         logging.debug("received from %s#%i: %s", *addr, data.hex(" "))
-        self.request_queue.put_nowait((data, addr))
+        asyncio.create_task(self.process(data, addr))
+
+    async def process(self, data: bytes, addr: tuple[str, int]) -> None:
+        async with self.client_pool.client() as client:
+            await client.send_message(data)
+            message = await client.recieve_message()
+            logging.debug("message from remote: %s", message.hex(" "))
+            self.transport.sendto(message, addr)
 
     def error_received(self, exc: Exception) -> None:
         logging.exception(exc)
         if not self.done.done():
             self.done.set_exception(exc)
-            self.task.cancel()
 
     def connection_lost(self, exc: Exception | None) -> None:
         if exc:
             logging.exception(exc)
         if not self.done.done():
             self.done.set_result(None)
-            self.task.cancel()
-
-    async def process(self) -> None:
-        while not self.done.done():
-            data, addr = await self.request_queue.get()
-            async with self.client_pool.get_client() as client:
-                await client.send_message(data)
-                message = await client.recieve_message()
-                logging.debug("message from remote: %s", message.hex(" "))
-                self.transport.sendto(message, addr)
 
 
 class NameSpace(argparse.Namespace):
     host: str
     port: int
     remote_host: str
     remote_port: int
```

### Comparing `dot_proxy-0.1.0/pyproject.toml` & `dot_proxy-0.2.0/pyproject.toml`

 * *Files identical despite different names*

