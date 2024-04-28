# Comparing `tmp/smartlink-remote-restapi-0.0.8.tar.gz` & `tmp/smartlink-remote-restapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartlink-remote-restapi-0.0.8.tar", last modified: Mon Jan  8 07:17:25 2024, max compression
+gzip compressed data, was "smartlink-remote-restapi-0.0.9.tar", last modified: Mon Jan  8 21:28:16 2024, max compression
```

## Comparing `smartlink-remote-restapi-0.0.8.tar` & `smartlink-remote-restapi-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 07:17:25.209159 smartlink-remote-restapi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-08 07:17:25.209159 smartlink-remote-restapi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-08 07:16:56.000000 smartlink-remote-restapi-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 07:17:25.209159 smartlink-remote-restapi-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-08 07:16:56.000000 smartlink-remote-restapi-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 07:17:25.209159 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 07:17:25.209159 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 07:16:56.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-08 07:16:56.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi/src/smartlink_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 07:17:25.209159 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-08 07:17:25.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-08 07:17:25.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 07:17:25.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-08 07:17:25.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-08 07:17:25.000000 smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:16.956574 smartlink-remote-restapi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-08 21:28:16.956574 smartlink-remote-restapi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-08 21:27:48.000000 smartlink-remote-restapi-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-08 21:27:48.000000 smartlink-remote-restapi-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 21:28:16.956574 smartlink-remote-restapi-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-08 21:27:48.000000 smartlink-remote-restapi-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:16.952574 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:16.952574 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 21:27:48.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-08 21:27:48.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi/src/smartlink_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:16.956574 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-08 21:28:16.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-08 21:28:16.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 21:28:16.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-08 21:28:16.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-08 21:28:16.000000 smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/top_level.txt
```

### Comparing `smartlink-remote-restapi-0.0.8/PKG-INFO` & `smartlink-remote-restapi-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlink-remote-restapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles smartlink-remote-restapi Python
 Home-page: https://github.com/circles-zone/smartlink-remote-restapi-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -12,9 +12,10 @@
 Requires-Dist: pytest
 Requires-Dist: requests
 Requires-Dist: user-context-remote
 Requires-Dist: python-sdk-local
 Requires-Dist: python-dotenv
 Requires-Dist: logger-local
 Requires-Dist: url-remote
+Requires-Dist: smartlink-local
 
 PyPI Package for Circles smartlink-remote-restapi Python
```

### Comparing `smartlink-remote-restapi-0.0.8/README.md` & `smartlink-remote-restapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `smartlink-remote-restapi-0.0.8/setup.py` & `smartlink-remote-restapi-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "smartlink-remote-restapi"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles smartlink-remote-restapi Python",
     long_description="PyPI Package for Circles smartlink-remote-restapi Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/smartlink-remote-restapi-python-package",
     # packages=setuptools.find_packages(),
@@ -24,10 +24,11 @@
     install_requires=[
         'pytest',
         'requests',
         'user-context-remote',
         'python-sdk-local',
         'python-dotenv',
         'logger-local',
-        'url-remote'
+        'url-remote',
+        'smartlink-local'
     ],
 )
```

### Comparing `smartlink-remote-restapi-0.0.8/smartlink_remote_restapi/src/smartlink_remote.py` & `smartlink-remote-restapi-0.0.9/smartlink_remote_restapi/src/smartlink_remote.py`

 * *Files identical despite different names*

### Comparing `smartlink-remote-restapi-0.0.8/smartlink_remote_restapi.egg-info/PKG-INFO` & `smartlink-remote-restapi-0.0.9/smartlink_remote_restapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlink-remote-restapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles smartlink-remote-restapi Python
 Home-page: https://github.com/circles-zone/smartlink-remote-restapi-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -12,9 +12,10 @@
 Requires-Dist: pytest
 Requires-Dist: requests
 Requires-Dist: user-context-remote
 Requires-Dist: python-sdk-local
 Requires-Dist: python-dotenv
 Requires-Dist: logger-local
 Requires-Dist: url-remote
+Requires-Dist: smartlink-local
 
 PyPI Package for Circles smartlink-remote-restapi Python
```

