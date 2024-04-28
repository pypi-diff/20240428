# Comparing `tmp/tailucas_pylib-0.2.8.tar.gz` & `tmp/tailucas_pylib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.2.8.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.2.9.tar", max compression
```

## Comparing `tailucas_pylib-0.2.8.tar` & `tailucas_pylib-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.8/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.8/README.md
--rw-r--r--   0        0        0      570 2024-04-27 06:25:58.535854 tailucas_pylib-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.8/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.8/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.8/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.8/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.8/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.8/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.8/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.8/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.8/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.8/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.8/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5225 2024-04-22 09:52:31.109505 tailucas_pylib-0.2.8/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.2.8/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12343 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.9/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.9/README.md
+-rw-r--r--   0        0        0      570 2024-04-28 09:02:09.241593 tailucas_pylib-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.9/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.9/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.9/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.9/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.9/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.9/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.9/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.9/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.9/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.9/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.9/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.2.9/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.2.9/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12343 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.9/PKG-INFO
```

### Comparing `tailucas_pylib-0.2.8/LICENSE` & `tailucas_pylib-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/README.md` & `tailucas_pylib-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/pyproject.toml` & `tailucas_pylib-0.2.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.2.8"
+version = "0.2.9"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 botoflow = "^0.8"
 boto3 = "^1.34.93"
 cronitor = "^4.7.1"
 msgpack = "^1.0.8"
-onepasswordconnectsdk = "^1.5.1"
 pika = "^1.3.2"
 python-dateutil = "^2.9.0.post0"
 pytz = "^2024.1"
 pyzmq = "^26.0.2"
 sentry-sdk = "^2.0.1"
 simplejson = "^3.19.2"
 pyyaml = "^6.0.1"
+onepasswordconnectsdk = "^1.5.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/__init__.py` & `tailucas_pylib-0.2.9/tailucas_pylib/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/app.py` & `tailucas_pylib-0.2.9/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.2.9/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.2.9/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.2.9/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.2.9/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/data.py` & `tailucas_pylib-0.2.9/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/datetime.py` & `tailucas_pylib-0.2.9/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/handler.py` & `tailucas_pylib-0.2.9/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/process.py` & `tailucas_pylib-0.2.9/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.2.9/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/threads.py` & `tailucas_pylib-0.2.9/tailucas_pylib/threads.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 import sys
 import threading
 import time
 import traceback
 
 from datetime import datetime
-
+from sentry_sdk import Hub
 from zmq.error import ZMQError
 
 from .aws.metrics import post_count_metric
 from .zmq import try_close, zmq_sockets
 
 
 log = logging.getLogger(APP_NAME)  # type: ignore
@@ -26,15 +26,19 @@
 trigger_exception = None
 
 
 def die(exception=None):
     global shutting_down
     global interruptable_sleep
     global trigger_exception
-    log.debug(f'Shutting down...')
+    log.debug(f'Shutting down Sentry...')
+    client = Hub.current.client
+    if client is not None:
+        client.close(timeout=2.0)
+    log.debug(f'Shutting down application...')
     shutting_down = True
     interruptable_sleep.set()
     # enforce latch so as not to unset later due to __main__ shutdown
     if exception is not None:
         trigger_exception = exception
```

### Comparing `tailucas_pylib-0.2.8/tailucas_pylib/zmq.py` & `tailucas_pylib-0.2.9/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.8/PKG-INFO` & `tailucas_pylib-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.2.8
+Version: 0.2.9
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

