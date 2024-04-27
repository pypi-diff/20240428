# Comparing `tmp/yoto_api-1.7.7.tar.gz` & `tmp/yoto_api-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.7.tar", last modified: Thu Apr 25 13:10:15 2024, max compression
+gzip compressed data, was "yoto_api-1.7.8.tar", last modified: Sat Apr 27 22:44:20 2024, max compression
```

## Comparing `yoto_api-1.7.7.tar` & `yoto_api-1.7.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:10:15.080860 yoto_api-1.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 13:09:46.000000 yoto_api-1.7.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-25 13:09:46.000000 yoto_api-1.7.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 13:09:46.000000 yoto_api-1.7.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 13:09:46.000000 yoto_api-1.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 13:09:46.000000 yoto_api-1.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 13:10:15.080860 yoto_api-1.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-25 13:09:46.000000 yoto_api-1.7.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 13:09:46.000000 yoto_api-1.7.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:10:15.080860 yoto_api-1.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 13:10:05.000000 yoto_api-1.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:10:15.076859 yoto_api-1.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:09:46.000000 yoto_api-1.7.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 13:09:46.000000 yoto_api-1.7.7/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:10:15.080860 yoto_api-1.7.7/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27737 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 13:09:46.000000 yoto_api-1.7.7/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:10:15.080860 yoto_api-1.7.7/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 13:10:15.000000 yoto_api-1.7.7/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-25 13:10:15.000000 yoto_api-1.7.7/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:10:15.000000 yoto_api-1.7.7/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:10:14.000000 yoto_api-1.7.7/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 13:10:15.000000 yoto_api-1.7.7/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 13:10:15.000000 yoto_api-1.7.7/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 22:43:58.000000 yoto_api-1.7.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-27 22:43:58.000000 yoto_api-1.7.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 22:43:58.000000 yoto_api-1.7.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 22:43:58.000000 yoto_api-1.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 22:43:58.000000 yoto_api-1.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-27 22:44:20.890488 yoto_api-1.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-27 22:43:58.000000 yoto_api-1.7.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 22:43:58.000000 yoto_api-1.7.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:44:20.890488 yoto_api-1.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-27 22:44:14.000000 yoto_api-1.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:43:58.000000 yoto_api-1.7.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 22:43:58.000000 yoto_api-1.7.8/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.7/CONTRIBUTING.rst` & `yoto_api-1.7.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.7/LICENSE` & `yoto_api-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.7/PKG-INFO` & `yoto_api-1.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.7
+Version: 1.7.8
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.7.7/README.rst` & `yoto_api-1.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.7/setup.py` & `yoto_api-1.7.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.7",
+    version="1.7.8",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.7/yoto_api/Card.py` & `yoto_api-1.7.8/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.7/yoto_api/YotoAPI.py` & `yoto_api-1.7.8/yoto_api/YotoAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,17 +183,17 @@
         valid_until = datetime.datetime.now(pytz.utc) + timedelta(
             seconds=response["expires_in"]
         )
         return Token(
             username=token.username,
             password=token.password,
             access_token=response["access_token"],
-            refresh_token=response["refresh_token"],
+            refresh_token=response["id_token"],
             token_type=response["token_type"],
-            scope=response["scope"],
+            scope=token.scope,
             valid_until=valid_until,
         )
 
     def _get_devices(self, token: Token) -> None:
         url = self.BASE_URL + "/device-v2/devices/mine"
 
         headers = self._get_authenticated_headers(token)
```

### Comparing `yoto_api-1.7.7/yoto_api/YotoManager.py` & `yoto_api-1.7.8/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.7/yoto_api/YotoPlayer.py` & `yoto_api-1.7.8/yoto_api/YotoPlayer.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.7/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.7.8/yoto_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.7
+Version: 1.7.8
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

