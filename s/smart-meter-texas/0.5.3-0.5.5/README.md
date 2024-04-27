# Comparing `tmp/smart_meter_texas-0.5.3.tar.gz` & `tmp/smart_meter_texas-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_texas-0.5.3.tar", last modified: Sat Jul 22 12:41:04 2023, max compression
+gzip compressed data, was "smart_meter_texas-0.5.5.tar", last modified: Sat Apr 27 23:23:02 2024, max compression
```

## Comparing `smart_meter_texas-0.5.3.tar` & `smart_meter_texas-0.5.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:41:04.364245 smart_meter_texas-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-22 12:41:04.364245 smart_meter_texas-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:41:04.364245 smart_meter_texas-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4974 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/smart_meter_texas.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-22 12:41:04.364245 smart_meter_texas-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:41:04.364245 smart_meter_texas-0.5.3/smart_meter_texas/
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/smart_meter_texas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/smart_meter_texas/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-22 12:40:49.000000 smart_meter_texas-0.5.3/smart_meter_texas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:41:04.364245 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-22 12:41:04.000000 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-22 12:41:04.000000 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:41:04.000000 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:41:04.000000 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 12:41:04.000000 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-22 12:41:04.000000 smart_meter_texas-0.5.3/smart_meter_texas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:23:02.889377 smart_meter_texas-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-27 23:23:02.889377 smart_meter_texas-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:23:02.889377 smart_meter_texas-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4974 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/smart_meter_texas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-27 23:23:02.889377 smart_meter_texas-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:23:02.889377 smart_meter_texas-0.5.5/smart_meter_texas/
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/smart_meter_texas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/smart_meter_texas/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-27 23:22:58.000000 smart_meter_texas-0.5.5/smart_meter_texas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:23:02.889377 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-27 23:23:02.000000 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-27 23:23:02.000000 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:23:02.000000 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:23:02.000000 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 23:23:02.000000 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 23:23:02.000000 smart_meter_texas-0.5.5/smart_meter_texas.egg-info/top_level.txt
```

### Comparing `smart_meter_texas-0.5.3/CONTRIBUTING.rst` & `smart_meter_texas-0.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/LICENSE` & `smart_meter_texas-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/PKG-INFO` & `smart_meter_texas-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_texas
-Version: 0.5.3
+Version: 0.5.5
 Summary: Package to connect to and retrieve data from the unofficial Smart Meter Texas API
 Home-page: https://github.com/grahamwetzler/smart-meter-texas
 Author: Graham Wetzler
 Author-email: graham@wetzler.dev
 License: MIT license
 Keywords: smart_meter_texas
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: aiohttp<4,>=3.7.4
+Requires-Dist: asn1>=2.4.1
+Requires-Dist: python-dateutil>=2.8.1
+Requires-Dist: tenacity>=8.0.1
 
 =================
 Smart Meter Texas
 =================
 
 
 .. image:: https://img.shields.io/pypi/v/smart_meter_texas.svg
```

### Comparing `smart_meter_texas-0.5.3/README.rst` & `smart_meter_texas-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/docs/Makefile` & `smart_meter_texas-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/docs/conf.py` & `smart_meter_texas-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/docs/installation.rst` & `smart_meter_texas-0.5.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/docs/make.bat` & `smart_meter_texas-0.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/setup.py` & `smart_meter_texas-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords="smart_meter_texas",
     name="smart_meter_texas",
     packages=find_packages(include=["smart_meter_texas", "smart_meter_texas.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/grahamwetzler/smart-meter-texas",
-    version="0.5.3",
+    version="0.5.5",
     zip_safe=False,
 )
```

### Comparing `smart_meter_texas-0.5.3/smart_meter_texas/__init__.py` & `smart_meter_texas-0.5.5/smart_meter_texas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 import asyncio
 import binascii
 import datetime
 import logging
 import socket
 import ssl
+import sys
 from random import randrange
 
 import asn1
 import certifi
 import dateutil.parser
 import OpenSSL.crypto as crypto
 from aiohttp import ClientSession
+from dateutil.tz import gettz
 from tenacity import retry, retry_if_exception_type
 
 from .const import (
     AUTH_ENDPOINT,
     BASE_ENDPOINT,
     BASE_HOSTNAME,
-    BASE_URL,
     CLIENT_HEADERS,
     INTERVAL_SYNCH,
     LATEST_OD_READ_ENDPOINT,
     METER_ENDPOINT,
     OD_READ_ENDPOINT,
     OD_READ_RETRY_TIME,
     TOKEN_EXPRIATION,
@@ -35,15 +36,15 @@
     SmartMeterTexasAuthError,
     SmartMeterTexasAuthExpired,
     SmartMeterTexasRateLimitError,
 )
 
 __author__ = "Graham Wetzler"
 __email__ = "graham@wetzler.dev"
-__version__ = "0.5.3"
+__version__ = "0.5.5"
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Meter:
     def __init__(self, meter: str, esiid: str, address: str):
         self.meter = meter
@@ -74,15 +75,15 @@
             except KeyError:
                 _LOGGER.error("Error reading meter: ", json_response)
                 raise SmartMeterTexasAPIError(
                     f"Error parsing response: {json_response}"
                 )
             else:
                 if status == "COMPLETED":
-                    _LOGGER.debug("Reading completed: %s", self.reading_data)
+                    _LOGGER.debug("Reading completed: %s", data)
                     self.reading_data = data
                     return self.reading_data
                 elif status == "PENDING":
                     _LOGGER.debug("Meter reading %s", status)
                     _LOGGER.debug("Sleeping for %s seconds", OD_READ_RETRY_TIME)
                     await asyncio.sleep(OD_READ_RETRY_TIME)
                 else:
@@ -166,16 +167,19 @@
     @property
     def reading(self):
         """Returns the latest meter reading in kWh."""
         return float(self.reading_data["odrread"])
 
     @property
     def reading_datetime(self):
-        """Returns the UTC datetime of the latest reading."""
-        date = dateutil.parser.parse(self.reading_data["odrdate"])
+        """Returns the UTC datetime of the latest reading.
+        'odrdate' is returned from the SMT API in America/Chicago timezone."""
+        date = dateutil.parser.parse(self.reading_data["odrdate"]).replace(
+            tzinfo=gettz("America/Chicago")
+        )
         date_as_utc = date.astimezone(datetime.timezone.utc)
         return date_as_utc
 
     @property
     def read_15min(self):
         """Returns the list of date/times and the consumption rate"""
         return self.interval
@@ -214,27 +218,25 @@
         self.ssl_context = ssl_context
 
     def _init_ssl_context(self):
         if self.ssl_context == None:
             new_ssl_context = ssl.create_default_context(capath=certifi.where())
             new_ssl_context.check_hostname = True
             new_ssl_context.verify_mode = ssl.CERT_REQUIRED
-            new_ssl_context.options |= (
-                ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1 | ssl.OP_NO_SSLv3 | ssl.OP_NO_SSLv2
-            )
+            if sys.version_info >= (3, 7):
+                new_ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
+            else:
+                new_ssl_context.options |= (
+                    ssl.OP_NO_TLSv1
+                    | ssl.OP_NO_TLSv1_1
+                    | ssl.OP_NO_SSLv3
+                    | ssl.OP_NO_SSLv2
+                )
             self.ssl_context = new_ssl_context
 
-    async def _init_websession(self):
-        """Make an initial GET request to initialize the session otherwise
-        future POST requests will timeout."""
-        self._init_ssl_context()
-        await self.websession.get(
-            BASE_URL, headers=self._agent_headers(), ssl=self.ssl_context
-        )
-
     def _agent_headers(self):
         """Build the user agent header."""
         if not self.user_agent:
             self.user_agent = USER_AGENT_TEMPLATE.format(
                 BUILD=randrange(1001, 9999), REV=randrange(12, 999)
             )
 
@@ -271,20 +273,17 @@
         json_response = await resp.json()
         return json_response
 
     async def authenticate(self):
         if not self.token_valid:
             _LOGGER.debug("Requesting login token")
 
-            # Make an initial GET request otherwise subsequent calls will timeout.
-            await self._init_websession()
-
             resp = await self.websession.request(
                 "POST",
-                f"{BASE_ENDPOINT}{AUTH_ENDPOINT}",
+                AUTH_ENDPOINT,
                 json={
                     "username": self.account.username,
                     "password": self.account.password,
                     "rememberMe": "true",
                 },
                 headers=self.headers,
                 ssl=self.ssl_context,
@@ -427,18 +426,20 @@
         except Exception as error:
             _LOGGER.error("Error loading certificate file into SSL Context")
             ssl_context = ssl.create_default_context(capath=certifi.where())
 
         # Enable strict checking
         ssl_context.check_hostname = True
         ssl_context.verify_mode = ssl.CERT_REQUIRED
-        # Disable SSL, TLSv1, TLSv1.1
-        ssl_context.options |= (
-            ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1 | ssl.OP_NO_SSLv3 | ssl.OP_NO_SSLv2
-        )
+        if sys.version_info >= (3, 7):
+            ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
+        else:
+            ssl_context.options |= (
+                ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1 | ssl.OP_NO_SSLv3 | ssl.OP_NO_SSLv2
+            )
 
         return ssl_context
 
     async def get_ssl_context(self):
         """Returns the default SSL Context"""
         ssl_context = None
         try:
```

### Comparing `smart_meter_texas-0.5.3/smart_meter_texas/exceptions.py` & `smart_meter_texas-0.5.5/smart_meter_texas/exceptions.py`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.3/smart_meter_texas.egg-info/PKG-INFO` & `smart_meter_texas-0.5.5/smart_meter_texas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smart-meter-texas
-Version: 0.5.3
+Name: smart_meter_texas
+Version: 0.5.5
 Summary: Package to connect to and retrieve data from the unofficial Smart Meter Texas API
 Home-page: https://github.com/grahamwetzler/smart-meter-texas
 Author: Graham Wetzler
 Author-email: graham@wetzler.dev
 License: MIT license
 Keywords: smart_meter_texas
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: aiohttp<4,>=3.7.4
+Requires-Dist: asn1>=2.4.1
+Requires-Dist: python-dateutil>=2.8.1
+Requires-Dist: tenacity>=8.0.1
 
 =================
 Smart Meter Texas
 =================
 
 
 .. image:: https://img.shields.io/pypi/v/smart_meter_texas.svg
```

### Comparing `smart_meter_texas-0.5.3/smart_meter_texas.egg-info/SOURCES.txt` & `smart_meter_texas-0.5.5/smart_meter_texas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

