# Comparing `tmp/dot_proxy-0.2.2.tar.gz` & `tmp/dot_proxy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dot_proxy-0.2.2.tar", last modified: Sun Apr 28 07:36:21 2024, max compression
+gzip compressed data, was "dot_proxy-0.2.3.tar", last modified: Sun Apr 28 10:11:15 2024, max compression
```

## Comparing `dot_proxy-0.2.2.tar` & `dot_proxy-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 07:36:21.170104 dot_proxy-0.2.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-04-28 02:24:07.000000 dot_proxy-0.2.2/.env
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-28 04:26:56.000000 dot_proxy-0.2.2/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      288 2024-04-28 04:24:49.000000 dot_proxy-0.2.2/Dockerfile
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1056 2024-04-28 04:22:32.000000 dot_proxy-0.2.2/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3055 2024-04-28 07:36:21.170104 dot_proxy-0.2.2/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2024-04-28 07:35:55.000000 dot_proxy-0.2.2/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)      170 2024-04-28 02:54:36.000000 dot_proxy-0.2.2/docker-compose.yml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 07:36:21.166770 dot_proxy-0.2.2/dot_proxy.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3055 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      291 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/top_level.txt
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     5462 2024-04-28 07:36:06.000000 dot_proxy-0.2.2/dot_proxy.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      699 2024-04-28 07:34:21.000000 dot_proxy-0.2.2/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-28 07:36:21.170104 dot_proxy-0.2.2/setup.cfg
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 10:11:15.989836 dot_proxy-0.2.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-04-28 02:24:07.000000 dot_proxy-0.2.3/.env
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-28 04:26:56.000000 dot_proxy-0.2.3/.gitignore
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      288 2024-04-28 04:24:49.000000 dot_proxy-0.2.3/Dockerfile
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1056 2024-04-28 04:22:32.000000 dot_proxy-0.2.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3055 2024-04-28 10:11:15.989836 dot_proxy-0.2.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2024-04-28 07:35:55.000000 dot_proxy-0.2.3/README.md
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      170 2024-04-28 02:54:36.000000 dot_proxy-0.2.3/docker-compose.yml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 10:11:15.989836 dot_proxy-0.2.3/dot_proxy.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3055 2024-04-28 10:11:15.000000 dot_proxy-0.2.3/dot_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      291 2024-04-28 10:11:15.000000 dot_proxy-0.2.3/dot_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 10:11:15.000000 dot_proxy-0.2.3/dot_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-28 10:11:15.000000 dot_proxy-0.2.3/dot_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2024-04-28 10:11:15.000000 dot_proxy-0.2.3/dot_proxy.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2024-04-28 10:11:15.000000 dot_proxy-0.2.3/dot_proxy.egg-info/top_level.txt
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     5637 2024-04-28 10:10:25.000000 dot_proxy-0.2.3/dot_proxy.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      699 2024-04-28 07:34:21.000000 dot_proxy-0.2.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-28 10:11:15.989836 dot_proxy-0.2.3/setup.cfg
```

### Comparing `dot_proxy-0.2.2/LICENSE` & `dot_proxy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dot_proxy-0.2.2/PKG-INFO` & `dot_proxy-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dot-proxy
-Version: 0.2.2
+Version: 0.2.3
 Summary: DNS over TLS Proxy Server
 Author: Sergey M
 License: Copyright 2024 Sergey M
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `dot_proxy-0.2.2/README.md` & `dot_proxy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dot_proxy-0.2.2/dot_proxy.egg-info/PKG-INFO` & `dot_proxy-0.2.3/dot_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dot-proxy
-Version: 0.2.2
+Version: 0.2.3
 Summary: DNS over TLS Proxy Server
 Author: Sergey M
 License: Copyright 2024 Sergey M
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `dot_proxy-0.2.2/dot_proxy.py` & `dot_proxy-0.2.3/dot_proxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import ssl
 from collections import deque
 from contextlib import asynccontextmanager
 from dataclasses import dataclass, field
 from typing import Any, AsyncIterator, Sequence
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "Sergey M"
 
 
 @dataclass
 class DOTClient:
     host: str
     port: int = 853
@@ -46,58 +46,63 @@
     ) -> None:
         self._pool = deque(maxlen=max_clients)  # asyncio.Queue(max_clients)
         for _ in range(max_clients):
             client = DOTClient(*args, **kwargs)
             self._pool.append(client)
 
     @asynccontextmanager
-    async def client(self, timeout: float = 0.1) -> AsyncIterator[DOTClient]:
-        client = await self.get_client(timeout)
+    async def get_client(
+        self, timeout: float = 0.1
+    ) -> AsyncIterator[DOTClient]:
+        client = await self._get_client_from_pool(timeout)
         logging.debug("get client: 0x%X", id(client))
         try:
             yield client
         finally:
             self.release_client(client)
 
-    async def get_client(self, timeout: float) -> DOTClient:
+    async def _get_client_from_pool(self, timeout: float) -> DOTClient:
         while True:
             try:
-                return self._pool.popleft()
+                return self._pool.pop()
             except IndexError:
                 await asyncio.sleep(timeout)
 
     def release_client(self, client: DOTClient) -> None:
-        self._pool.appendleft(client)
+        """returm client to the pool"""
+        self._pool.append(client)
 
 
 class DOTProxyProtocol(asyncio.DatagramProtocol):
     def __init__(
         self,
         remote_host: str,
         remote_port: int = 853,
         max_clients: int = 10,
     ) -> None:
         self.client_pool = DOTClientPool(max_clients, remote_host, remote_port)
+        self.sem = asyncio.Semaphore(max_clients)
         self.done = asyncio.get_event_loop().create_future()
 
     def connection_made(self, transport: asyncio.DatagramTransport) -> None:
         self.transport = transport
 
     def datagram_received(
         self, data: bytes, addr: tuple[str | Any, int]
     ) -> None:
         logging.debug("received from %s#%i: %s", *addr, data.hex(" "))
         asyncio.create_task(self.process(data, addr))
 
     async def process(self, data: bytes, addr: tuple[str, int]) -> None:
-        async with self.client_pool.client() as client:
-            await client.send_message(data)
-            message = await client.recieve_message()
-            logging.debug("message from remote: %s", message.hex(" "))
-            self.transport.sendto(message, addr)
+        async with self.sem:
+            async with self.client_pool.get_client() as client:
+                await client.send_message(data)
+                message = await client.recieve_message()
+                logging.debug("message from remote: %s", message.hex(" "))
+                self.transport.sendto(message, addr)
 
     def error_received(self, exc: Exception) -> None:
         # logging.exception(exc)
         if not self.done.done():
             self.done.set_exception(exc)
 
     def connection_lost(self, exc: Exception | None) -> None:
```

### Comparing `dot_proxy-0.2.2/pyproject.toml` & `dot_proxy-0.2.3/pyproject.toml`

 * *Files identical despite different names*

