# Comparing `tmp/dot_proxy-0.2.1.tar.gz` & `tmp/dot_proxy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dot_proxy-0.2.1.tar", last modified: Sun Apr 28 07:34:42 2024, max compression
+gzip compressed data, was "dot_proxy-0.2.2.tar", last modified: Sun Apr 28 07:36:21 2024, max compression
```

## Comparing `dot_proxy-0.2.1.tar` & `dot_proxy-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 07:34:42.101290 dot_proxy-0.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-04-28 02:24:07.000000 dot_proxy-0.2.1/.env
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-28 04:26:56.000000 dot_proxy-0.2.1/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      288 2024-04-28 04:24:49.000000 dot_proxy-0.2.1/Dockerfile
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1056 2024-04-28 04:22:32.000000 dot_proxy-0.2.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3046 2024-04-28 07:34:42.101290 dot_proxy-0.2.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1479 2024-04-28 05:13:41.000000 dot_proxy-0.2.1/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)      170 2024-04-28 02:54:36.000000 dot_proxy-0.2.1/docker-compose.yml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 07:34:42.097956 dot_proxy-0.2.1/dot_proxy.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3046 2024-04-28 07:34:42.000000 dot_proxy-0.2.1/dot_proxy.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      291 2024-04-28 07:34:42.000000 dot_proxy-0.2.1/dot_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 07:34:42.000000 dot_proxy-0.2.1/dot_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-28 07:34:42.000000 dot_proxy-0.2.1/dot_proxy.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2024-04-28 07:34:42.000000 dot_proxy-0.2.1/dot_proxy.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2024-04-28 07:34:42.000000 dot_proxy-0.2.1/dot_proxy.egg-info/top_level.txt
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     5456 2024-04-28 07:34:34.000000 dot_proxy-0.2.1/dot_proxy.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      699 2024-04-28 07:34:21.000000 dot_proxy-0.2.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-28 07:34:42.101290 dot_proxy-0.2.1/setup.cfg
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 07:36:21.170104 dot_proxy-0.2.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-04-28 02:24:07.000000 dot_proxy-0.2.2/.env
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-28 04:26:56.000000 dot_proxy-0.2.2/.gitignore
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      288 2024-04-28 04:24:49.000000 dot_proxy-0.2.2/Dockerfile
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1056 2024-04-28 04:22:32.000000 dot_proxy-0.2.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3055 2024-04-28 07:36:21.170104 dot_proxy-0.2.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2024-04-28 07:35:55.000000 dot_proxy-0.2.2/README.md
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      170 2024-04-28 02:54:36.000000 dot_proxy-0.2.2/docker-compose.yml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 07:36:21.166770 dot_proxy-0.2.2/dot_proxy.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3055 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      291 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2024-04-28 07:36:21.000000 dot_proxy-0.2.2/dot_proxy.egg-info/top_level.txt
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     5462 2024-04-28 07:36:06.000000 dot_proxy-0.2.2/dot_proxy.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      699 2024-04-28 07:34:21.000000 dot_proxy-0.2.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-28 07:36:21.170104 dot_proxy-0.2.2/setup.cfg
```

### Comparing `dot_proxy-0.2.1/LICENSE` & `dot_proxy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dot_proxy-0.2.1/PKG-INFO` & `dot_proxy-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dot-proxy
-Version: 0.2.1
+Version: 0.2.2
 Summary: DNS over TLS Proxy Server
 Author: Sergey M
 License: Copyright 2024 Sergey M
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,15 +20,15 @@
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # README
 
-[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]()
+[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() <!-- [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]() -->
 
 DNS over TLS Proxy Server for Non-Systemd Distros.
 
 ## Install and Run
 
 Via Docker Compose:
```

### Comparing `dot_proxy-0.2.1/README.md` & `dot_proxy-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # README
 
-[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]()
+[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() <!-- [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]() -->
 
 DNS over TLS Proxy Server for Non-Systemd Distros.
 
 ## Install and Run
 
 Via Docker Compose:
```

### Comparing `dot_proxy-0.2.1/dot_proxy.egg-info/PKG-INFO` & `dot_proxy-0.2.2/dot_proxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dot-proxy
-Version: 0.2.1
+Version: 0.2.2
 Summary: DNS over TLS Proxy Server
 Author: Sergey M
 License: Copyright 2024 Sergey M
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,15 +20,15 @@
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # README
 
-[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]()
+[![PyPI - Version](https://img.shields.io/pypi/v/dot-proxy)]() <!-- [![PyPI - License](https://img.shields.io/pypi/l/dot-proxy)]() [![PyPI - Downloads](https://img.shields.io/pypi/dm/dot-proxy)]() -->
 
 DNS over TLS Proxy Server for Non-Systemd Distros.
 
 ## Install and Run
 
 Via Docker Compose:
```

### Comparing `dot_proxy-0.2.1/dot_proxy.py` & `dot_proxy-0.2.2/dot_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import ssl
 from collections import deque
 from contextlib import asynccontextmanager
 from dataclasses import dataclass, field
 from typing import Any, AsyncIterator, Sequence
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "Sergey M"
 
 
 @dataclass
 class DOTClient:
     host: str
     port: int = 853
@@ -92,21 +92,21 @@
         async with self.client_pool.client() as client:
             await client.send_message(data)
             message = await client.recieve_message()
             logging.debug("message from remote: %s", message.hex(" "))
             self.transport.sendto(message, addr)
 
     def error_received(self, exc: Exception) -> None:
-        logging.exception(exc)
+        # logging.exception(exc)
         if not self.done.done():
             self.done.set_exception(exc)
 
     def connection_lost(self, exc: Exception | None) -> None:
-        if exc:
-            logging.exception(exc)
+        # if exc:
+        #     logging.exception(exc)
         if not self.done.done():
             self.done.set_result(None)
 
 
 class NameSpace(argparse.Namespace):
     host: str
     port: int
```

### Comparing `dot_proxy-0.2.1/pyproject.toml` & `dot_proxy-0.2.2/pyproject.toml`

 * *Files identical despite different names*

