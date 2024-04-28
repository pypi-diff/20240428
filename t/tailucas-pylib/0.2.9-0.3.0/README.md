# Comparing `tmp/tailucas_pylib-0.2.9.tar.gz` & `tmp/tailucas_pylib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.2.9.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.3.0.tar", max compression
```

## Comparing `tailucas_pylib-0.2.9.tar` & `tailucas_pylib-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.9/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.9/README.md
--rw-r--r--   0        0        0      570 2024-04-28 09:02:09.241593 tailucas_pylib-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.9/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.9/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.9/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.9/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.9/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.9/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.9/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.9/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.9/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.9/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.9/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.2.9/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.2.9/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12343 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.0/README.md
+-rw-r--r--   0        0        0      537 2024-04-28 09:26:35.881596 tailucas_pylib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5721 2024-04-28 09:25:52.661596 tailucas_pylib-0.3.0/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.0/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.0/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.0/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.0/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.0/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.0/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.0/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.0/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.0/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.3.0/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.0/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.3.0/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.0/PKG-INFO
```

### Comparing `tailucas_pylib-0.2.9/LICENSE` & `tailucas_pylib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/README.md` & `tailucas_pylib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/pyproject.toml` & `tailucas_pylib-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.2.9"
+version = "0.3.0"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -15,13 +15,12 @@
 pika = "^1.3.2"
 python-dateutil = "^2.9.0.post0"
 pytz = "^2024.1"
 pyzmq = "^26.0.2"
 sentry-sdk = "^2.0.1"
 simplejson = "^3.19.2"
 pyyaml = "^6.0.1"
-onepasswordconnectsdk = "^1.5.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/__init__.py` & `tailucas_pylib-0.3.0/tailucas_pylib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,31 +65,34 @@
 
     # 1Password credentials
     creds = None
     app_creds_config = None
     op_connect_server_env = 'OP_CONNECT_SERVER'
     if op_connect_server_env in os.environ:
         if hasattr(builtins, 'creds_config'):
-            app_creds_config = builtins.creds_config
-            import onepasswordconnectsdk
-            from onepasswordconnectsdk.client import (
-                Client,
-                new_client_from_environment
-            )
-            op_connect_server = os.environ[op_connect_server_env]
-            creds_client: Client = new_client_from_environment(url=op_connect_server)
-            creds_vaults = creds_client.get_vaults()
-            if creds_vaults:
-                for vault in creds_vaults:
-                    log.info(f"Credential vault {vault.name} contains {vault.items} credentials.")
-            else:
-                log.error(f'No vaults found on 1Password server {op_connect_server}. Fix or remove environment variable {op_connect_server_env}.')
-                sys.exit(1)
-            creds = onepasswordconnectsdk.load(client=creds_client, config=app_creds_config)
-            builtins.creds = creds  # type: ignore
+            try:
+                app_creds_config = builtins.creds_config
+                import onepasswordconnectsdk
+                from onepasswordconnectsdk.client import (
+                    Client,
+                    new_client_from_environment
+                )
+                op_connect_server = os.environ[op_connect_server_env]
+                creds_client: Client = new_client_from_environment(url=op_connect_server)
+                creds_vaults = creds_client.get_vaults()
+                if creds_vaults:
+                    for vault in creds_vaults:
+                        log.info(f"Credential vault {vault.name} contains {vault.items} credentials.")
+                else:
+                    log.error(f'No vaults found on 1Password server {op_connect_server}. Fix or remove environment variable {op_connect_server_env}.')
+                    sys.exit(1)
+                creds = onepasswordconnectsdk.load(client=creds_client, config=app_creds_config)
+                builtins.creds = creds  # type: ignore
+            except ModuleNotFoundError:
+                log.error('1Password configuration is set but onepasswordconnectsdk is not available or missing from package configuration.')
         else:
             log.warning(f'Assign CredsConfig to builtins.creds_config in __main__ to enable 1Password credential services.')
     else:
         log.warning(f'Set environment variable {op_connect_server_env} to enable 1Password credential services.')
 
     # Sentry
     if app_creds_config and hasattr(app_creds_config, 'sentry_dsn'):
```

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/app.py` & `tailucas_pylib-0.3.0/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.3.0/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.3.0/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.3.0/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.3.0/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/data.py` & `tailucas_pylib-0.3.0/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/datetime.py` & `tailucas_pylib-0.3.0/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/handler.py` & `tailucas_pylib-0.3.0/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/process.py` & `tailucas_pylib-0.3.0/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.3.0/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/threads.py` & `tailucas_pylib-0.3.0/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/tailucas_pylib/zmq.py` & `tailucas_pylib-0.3.0/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.9/PKG-INFO` & `tailucas_pylib-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.2.9
+Version: 0.3.0
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.93,<2.0.0)
 Requires-Dist: botoflow (>=0.8,<0.9)
 Requires-Dist: cronitor (>=4.7.1,<5.0.0)
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
-Requires-Dist: onepasswordconnectsdk (>=1.5.1,<2.0.0)
 Requires-Dist: pika (>=1.3.2,<2.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (>=26.0.2,<27.0.0)
 Requires-Dist: sentry-sdk (>=2.0.1,<3.0.0)
 Requires-Dist: simplejson (>=3.19.2,<4.0.0)
```

