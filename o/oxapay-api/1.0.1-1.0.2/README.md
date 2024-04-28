# Comparing `tmp/oxapay_api-1.0.1.tar.gz` & `tmp/oxapay_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxapay_api-1.0.1.tar", last modified: Fri Apr 19 21:47:11 2024, max compression
+gzip compressed data, was "oxapay_api-1.0.2.tar", last modified: Sun Apr 28 12:55:54 2024, max compression
```

## Comparing `oxapay_api-1.0.1.tar` & `oxapay_api-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-19 21:47:11.430276 oxapay_api-1.0.1/
--rw-r--r--   0 rushifakami   (501) staff       (20)      911 2024-04-19 21:47:11.430105 oxapay_api-1.0.1/PKG-INFO
-drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-19 21:47:11.427433 oxapay_api-1.0.1/oxapay_api/
--rw-r--r--   0 rushifakami   (501) staff       (20)     8069 2024-04-19 21:43:44.000000 oxapay_api-1.0.1/oxapay_api/AsyncOxaPay.py
--rw-r--r--   0 rushifakami   (501) staff       (20)     7885 2024-04-19 21:43:59.000000 oxapay_api-1.0.1/oxapay_api/SyncOxaPay.py
--rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.1/oxapay_api/__init__.py
-drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-19 21:47:11.428743 oxapay_api-1.0.1/oxapay_api/clients/
--rw-r--r--   0 rushifakami   (501) staff       (20)      826 2024-04-19 20:29:02.000000 oxapay_api-1.0.1/oxapay_api/clients/AsyncClient.py
--rw-r--r--   0 rushifakami   (501) staff       (20)      698 2024-04-19 20:37:15.000000 oxapay_api-1.0.1/oxapay_api/clients/SyncClient.py
--rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.1/oxapay_api/clients/__init__.py
-drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-19 21:47:11.428905 oxapay_api-1.0.1/oxapay_api/clients/constants/
--rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.1/oxapay_api/clients/constants/__init__.py
--rw-r--r--   0 rushifakami   (501) staff       (20)       64 2024-04-19 20:02:59.000000 oxapay_api-1.0.1/oxapay_api/clients/constants/api_constants.py
-drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-19 21:47:11.429249 oxapay_api-1.0.1/oxapay_api/utils/
--rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.1/oxapay_api/utils/__init__.py
--rw-r--r--   0 rushifakami   (501) staff       (20)     1880 2024-04-15 18:26:45.000000 oxapay_api-1.0.1/oxapay_api/utils/response_models.py
-drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-19 21:47:11.429798 oxapay_api-1.0.1/oxapay_api.egg-info/
--rw-r--r--   0 rushifakami   (501) staff       (20)      911 2024-04-19 21:47:11.000000 oxapay_api-1.0.1/oxapay_api.egg-info/PKG-INFO
--rw-r--r--   0 rushifakami   (501) staff       (20)      501 2024-04-19 21:47:11.000000 oxapay_api-1.0.1/oxapay_api.egg-info/SOURCES.txt
--rw-r--r--   0 rushifakami   (501) staff       (20)        1 2024-04-19 21:47:11.000000 oxapay_api-1.0.1/oxapay_api.egg-info/dependency_links.txt
--rw-r--r--   0 rushifakami   (501) staff       (20)       25 2024-04-19 21:47:11.000000 oxapay_api-1.0.1/oxapay_api.egg-info/requires.txt
--rw-r--r--   0 rushifakami   (501) staff       (20)       11 2024-04-19 21:47:11.000000 oxapay_api-1.0.1/oxapay_api.egg-info/top_level.txt
--rw-r--r--   0 rushifakami   (501) staff       (20)       38 2024-04-19 21:47:11.430314 oxapay_api-1.0.1/setup.cfg
--rw-r--r--   0 rushifakami   (501) staff       (20)     1127 2024-04-19 21:46:25.000000 oxapay_api-1.0.1/setup.py
+drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-28 12:55:54.898390 oxapay_api-1.0.2/
+-rw-r--r--   0 rushifakami   (501) staff       (20)      911 2024-04-28 12:55:54.898213 oxapay_api-1.0.2/PKG-INFO
+drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-28 12:55:54.895733 oxapay_api-1.0.2/oxapay_api/
+-rw-r--r--   0 rushifakami   (501) staff       (20)    14964 2024-04-28 12:42:28.000000 oxapay_api-1.0.2/oxapay_api/AsyncOxaPay.py
+-rw-r--r--   0 rushifakami   (501) staff       (20)    14951 2024-04-28 12:32:35.000000 oxapay_api-1.0.2/oxapay_api/SyncOxaPay.py
+-rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.2/oxapay_api/__init__.py
+drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-28 12:55:54.897101 oxapay_api-1.0.2/oxapay_api/clients/
+-rw-r--r--   0 rushifakami   (501) staff       (20)      826 2024-04-19 20:29:02.000000 oxapay_api-1.0.2/oxapay_api/clients/AsyncClient.py
+-rw-r--r--   0 rushifakami   (501) staff       (20)      698 2024-04-19 20:37:15.000000 oxapay_api-1.0.2/oxapay_api/clients/SyncClient.py
+-rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.2/oxapay_api/clients/__init__.py
+drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-28 12:55:54.897288 oxapay_api-1.0.2/oxapay_api/clients/constants/
+-rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.2/oxapay_api/clients/constants/__init__.py
+-rw-r--r--   0 rushifakami   (501) staff       (20)       64 2024-04-19 20:02:59.000000 oxapay_api-1.0.2/oxapay_api/clients/constants/api_constants.py
+drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-28 12:55:54.897636 oxapay_api-1.0.2/oxapay_api/utils/
+-rw-r--r--   0 rushifakami   (501) staff       (20)        0 2024-04-19 20:25:31.000000 oxapay_api-1.0.2/oxapay_api/utils/__init__.py
+-rw-r--r--   0 rushifakami   (501) staff       (20)     1881 2024-04-28 12:38:03.000000 oxapay_api-1.0.2/oxapay_api/utils/response_models.py
+drwxr-xr-x   0 rushifakami   (501) staff       (20)        0 2024-04-28 12:55:54.898001 oxapay_api-1.0.2/oxapay_api.egg-info/
+-rw-r--r--   0 rushifakami   (501) staff       (20)      911 2024-04-28 12:55:54.000000 oxapay_api-1.0.2/oxapay_api.egg-info/PKG-INFO
+-rw-r--r--   0 rushifakami   (501) staff       (20)      501 2024-04-28 12:55:54.000000 oxapay_api-1.0.2/oxapay_api.egg-info/SOURCES.txt
+-rw-r--r--   0 rushifakami   (501) staff       (20)        1 2024-04-28 12:55:54.000000 oxapay_api-1.0.2/oxapay_api.egg-info/dependency_links.txt
+-rw-r--r--   0 rushifakami   (501) staff       (20)       25 2024-04-28 12:55:54.000000 oxapay_api-1.0.2/oxapay_api.egg-info/requires.txt
+-rw-r--r--   0 rushifakami   (501) staff       (20)       11 2024-04-28 12:55:54.000000 oxapay_api-1.0.2/oxapay_api.egg-info/top_level.txt
+-rw-r--r--   0 rushifakami   (501) staff       (20)       38 2024-04-28 12:55:54.898431 oxapay_api-1.0.2/setup.cfg
+-rw-r--r--   0 rushifakami   (501) staff       (20)     1127 2024-04-28 12:52:31.000000 oxapay_api-1.0.2/setup.py
```

### Comparing `oxapay_api-1.0.1/PKG-INFO` & `oxapay_api-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxapay_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial library for interacting with the OxaPay API. See github for more info: https://github.com/Rushifakami/oxapay_api
 Home-page: https://github.com/Rushifakami/oxapay_api
 Author: Rushifakami
 License: MIT
 Keywords: crypto,oxapay,gateway,payment,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `oxapay_api-1.0.1/oxapay_api/clients/AsyncClient.py` & `oxapay_api-1.0.2/oxapay_api/clients/AsyncClient.py`

 * *Files identical despite different names*

### Comparing `oxapay_api-1.0.1/oxapay_api/clients/SyncClient.py` & `oxapay_api-1.0.2/oxapay_api/clients/SyncClient.py`

 * *Files identical despite different names*

### Comparing `oxapay_api-1.0.1/oxapay_api/utils/response_models.py` & `oxapay_api-1.0.2/oxapay_api/utils/response_models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
         self.type = type
         self.txID = txID
         self.date = date
         self.expiredAt = expiredAt
         self.payDate = payDate
         self.email = email
         self.orderId = orderId
-        self.description = description
+        self.description = description
```

### Comparing `oxapay_api-1.0.1/oxapay_api.egg-info/PKG-INFO` & `oxapay_api-1.0.2/oxapay_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxapay_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial library for interacting with the OxaPay API. See github for more info: https://github.com/Rushifakami/oxapay_api
 Home-page: https://github.com/Rushifakami/oxapay_api
 Author: Rushifakami
 License: MIT
 Keywords: crypto,oxapay,gateway,payment,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `oxapay_api-1.0.1/setup.py` & `oxapay_api-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='oxapay_api',
-    version='1.0.1',
+    version='1.0.2',
     author='Rushifakami',
     description='Unofficial library for interacting with the OxaPay API. See github for more info: https://github.com/Rushifakami/oxapay_api',
     packages=find_packages(),
     install_requires=[
         'aiohttp',
         'requests',
         'urllib3'
```

