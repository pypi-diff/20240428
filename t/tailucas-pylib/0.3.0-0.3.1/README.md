# Comparing `tmp/tailucas_pylib-0.3.0.tar.gz` & `tmp/tailucas_pylib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.3.0.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.3.1.tar", max compression
```

## Comparing `tailucas_pylib-0.3.0.tar` & `tailucas_pylib-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.0/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.0/README.md
--rw-r--r--   0        0        0      537 2024-04-28 09:26:35.881596 tailucas_pylib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5721 2024-04-28 09:25:52.661596 tailucas_pylib-0.3.0/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.0/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.0/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.0/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.0/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.0/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.0/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.0/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.0/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.0/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.3.0/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.0/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.3.0/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.1/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.1/README.md
+-rw-r--r--   0        0        0      537 2024-04-28 11:35:54.381593 tailucas_pylib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5989 2024-04-28 11:35:06.381594 tailucas_pylib-0.3.1/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.1/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.1/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.1/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.1/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.1/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.1/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.1/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.1/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.1/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.3.1/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.1/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.3.1/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.1/PKG-INFO
```

### Comparing `tailucas_pylib-0.3.0/LICENSE` & `tailucas_pylib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/README.md` & `tailucas_pylib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/pyproject.toml` & `tailucas_pylib-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.3.0"
+version = "0.3.1"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/__init__.py` & `tailucas_pylib-0.3.1/tailucas_pylib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,19 +100,23 @@
         if hasattr(builtins, 'SENTRY_EXTRAS'):
             integrations = builtins.SENTRY_EXTRAS  # type: ignore
         else:
             log.warning(f'Define a list builtins.SENTRY_EXTRAS in __main__ to enable Sentry.io extras.')
         sentry_environment = None
         if hasattr(builtins, 'SENTRY_ENVIRONMENT'):
             sentry_environment = builtins.SENTRY_ENVIRONMENT  # type: ignore
+        sentry_default_integrations = True
+        if hasattr(builtins, 'SENTRY_DEFAULT_INTEGRATIONS'):
+            sentry_default_integrations = builtins.SENTRY_DEFAULT_INTEGRATIONS  # type: ignore
         import sentry_sdk
         sentry_sdk.init(
             dsn=creds.sentry_dsn,  # type: ignore
             environment=sentry_environment,  # type: ignore
-            integrations=integrations
+            integrations=integrations,
+            sentry_default_integrations=sentry_default_integrations
         )
     else:
         log.warning(f'Add sentry_dsn to CredsConfig in __main__ to enable Sentry.io ticketing.')
 
     # Cronitor
     if app_creds_config and hasattr(app_creds_config, 'cronitor_token'):
         import cronitor
```

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/app.py` & `tailucas_pylib-0.3.1/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.3.1/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.3.1/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.3.1/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.3.1/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/data.py` & `tailucas_pylib-0.3.1/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/datetime.py` & `tailucas_pylib-0.3.1/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/handler.py` & `tailucas_pylib-0.3.1/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/process.py` & `tailucas_pylib-0.3.1/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.3.1/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/threads.py` & `tailucas_pylib-0.3.1/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/tailucas_pylib/zmq.py` & `tailucas_pylib-0.3.1/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.0/PKG-INFO` & `tailucas_pylib-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

