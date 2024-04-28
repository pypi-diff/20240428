# Comparing `tmp/alipay_faas_server_sdk-0.0.2.tar.gz` & `tmp/alipay_faas_server_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alipay_faas_server_sdk-0.0.2.tar", last modified: Fri Apr 26 10:27:27 2024, max compression
+gzip compressed data, was "alipay_faas_server_sdk-0.0.3.tar", last modified: Sun Apr 28 03:22:58 2024, max compression
```

## Comparing `alipay_faas_server_sdk-0.0.2.tar` & `alipay_faas_server_sdk-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.737603 alipay_faas_server_sdk-0.0.2/
--rw-r--r--   0 qy         (501) staff       (20)     1079 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/LICENSE
--rw-r--r--   0 qy         (501) staff       (20)     1396 2024-04-26 10:27:27.736859 alipay_faas_server_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 qy         (501) staff       (20)      473 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/README.md
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.723506 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/
--rw-r--r--   0 qy         (501) staff       (20)       70 2024-04-26 10:27:09.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/__init__.py
--rw-r--r--   0 qy         (501) staff       (20)     1321 2024-04-26 10:26:18.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/cloud.py
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.726472 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/config/
--rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/config/__init__.py
--rw-r--r--   0 qy         (501) staff       (20)     1718 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/config/cloud_config.py
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.728612 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/context/
--rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/context/__init__.py
--rw-r--r--   0 qy         (501) staff       (20)     1097 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/context/alipay_context.py
--rw-r--r--   0 qy         (501) staff       (20)      597 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/context/fn_context.py
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.730778 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/function/
--rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/function/__init__.py
--rw-r--r--   0 qy         (501) staff       (20)     3158 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/function/fn_client.py
--rw-r--r--   0 qy         (501) staff       (20)      324 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/function/fn_request.py
--rw-r--r--   0 qy         (501) staff       (20)      332 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/function/fn_response.py
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.733797 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/
--rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/__init__.py
--rw-r--r--   0 qy         (501) staff       (20)      467 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/http_client.py
--rw-r--r--   0 qy         (501) staff       (20)     1039 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/http_constants.py
--rw-r--r--   0 qy         (501) staff       (20)     2359 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/http_request.py
--rw-r--r--   0 qy         (501) staff       (20)      455 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/http_response.py
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.735310 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/utils/
--rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/utils/__init__.py
--rw-r--r--   0 qy         (501) staff       (20)      177 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/utils/env_util.py
--rw-r--r--   0 qy         (501) staff       (20)      698 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/utils/hash_util.py
-drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-26 10:27:27.736103 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/
--rw-r--r--   0 qy         (501) staff       (20)     1396 2024-04-26 10:27:27.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 qy         (501) staff       (20)     1071 2024-04-26 10:27:27.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 qy         (501) staff       (20)        1 2024-04-26 10:27:27.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 qy         (501) staff       (20)        9 2024-04-26 10:27:27.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/requires.txt
--rw-r--r--   0 qy         (501) staff       (20)       23 2024-04-26 10:27:27.000000 alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 qy         (501) staff       (20)       38 2024-04-26 10:27:27.737788 alipay_faas_server_sdk-0.0.2/setup.cfg
--rw-r--r--   0 qy         (501) staff       (20)     1920 2024-04-26 10:25:16.000000 alipay_faas_server_sdk-0.0.2/setup.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.930640 alipay_faas_server_sdk-0.0.3/
+-rw-r--r--   0 qy         (501) staff       (20)     1079 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/LICENSE
+-rw-r--r--   0 qy         (501) staff       (20)     1396 2024-04-28 03:22:58.929870 alipay_faas_server_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 qy         (501) staff       (20)      473 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/README.md
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.915300 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/
+-rw-r--r--   0 qy         (501) staff       (20)       70 2024-04-28 03:22:44.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/__init__.py
+-rw-r--r--   0 qy         (501) staff       (20)     1161 2024-04-28 03:21:43.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/cloud.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.918927 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/config/
+-rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/config/__init__.py
+-rw-r--r--   0 qy         (501) staff       (20)     1718 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/config/cloud_config.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.920777 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/context/
+-rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/context/__init__.py
+-rw-r--r--   0 qy         (501) staff       (20)     1097 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/context/alipay_context.py
+-rw-r--r--   0 qy         (501) staff       (20)      597 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/context/fn_context.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.922790 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/function/
+-rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/function/__init__.py
+-rw-r--r--   0 qy         (501) staff       (20)     3158 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/function/fn_client.py
+-rw-r--r--   0 qy         (501) staff       (20)      324 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/function/fn_request.py
+-rw-r--r--   0 qy         (501) staff       (20)      332 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/function/fn_response.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.925292 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/
+-rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/__init__.py
+-rw-r--r--   0 qy         (501) staff       (20)      467 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/http_client.py
+-rw-r--r--   0 qy         (501) staff       (20)     1039 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/http_constants.py
+-rw-r--r--   0 qy         (501) staff       (20)     2359 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/http_request.py
+-rw-r--r--   0 qy         (501) staff       (20)      455 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/http_response.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.927943 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/utils/
+-rw-r--r--   0 qy         (501) staff       (20)        0 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/utils/__init__.py
+-rw-r--r--   0 qy         (501) staff       (20)      177 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/utils/env_util.py
+-rw-r--r--   0 qy         (501) staff       (20)      698 2024-04-26 09:24:28.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/utils/hash_util.py
+drwxr-xr-x   0 qy         (501) staff       (20)        0 2024-04-28 03:22:58.928941 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/
+-rw-r--r--   0 qy         (501) staff       (20)     1396 2024-04-28 03:22:58.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 qy         (501) staff       (20)     1071 2024-04-28 03:22:58.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 qy         (501) staff       (20)        1 2024-04-28 03:22:58.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 qy         (501) staff       (20)        9 2024-04-28 03:22:58.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 qy         (501) staff       (20)       23 2024-04-28 03:22:58.000000 alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 qy         (501) staff       (20)       38 2024-04-28 03:22:58.930917 alipay_faas_server_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 qy         (501) staff       (20)     1920 2024-04-26 10:25:16.000000 alipay_faas_server_sdk-0.0.3/setup.py
```

### Comparing `alipay_faas_server_sdk-0.0.2/LICENSE` & `alipay_faas_server_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/PKG-INFO` & `alipay_faas_server_sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alipay-faas-server-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Alipay FaaS Server SDK
 Home-page: https://cloud.alipay.com
 Author: QiYuan
 Author-email: lj162403@alipay.com
 Project-URL: Site, https://cloud.alipay.com
 Project-URL: Repo, https://cloud.alipay.com
 Project-URL: Documentation, https://opendocs.alipay.com/mini/089c99?pathHash=5a879d9a
```

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/config/cloud_config.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/config/cloud_config.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/context/alipay_context.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/context/alipay_context.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/context/fn_context.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/context/fn_context.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/function/fn_client.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/function/fn_client.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/http_constants.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/http_constants.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/http/http_request.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/http/http_request.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk/utils/hash_util.py` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk/utils/hash_util.py`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/PKG-INFO` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alipay-faas-server-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Alipay FaaS Server SDK
 Home-page: https://cloud.alipay.com
 Author: QiYuan
 Author-email: lj162403@alipay.com
 Project-URL: Site, https://cloud.alipay.com
 Project-URL: Repo, https://cloud.alipay.com
 Project-URL: Documentation, https://opendocs.alipay.com/mini/089c99?pathHash=5a879d9a
```

### Comparing `alipay_faas_server_sdk-0.0.2/alipay_faas_server_sdk.egg-info/SOURCES.txt` & `alipay_faas_server_sdk-0.0.3/alipay_faas_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alipay_faas_server_sdk-0.0.2/setup.py` & `alipay_faas_server_sdk-0.0.3/setup.py`

 * *Files identical despite different names*

