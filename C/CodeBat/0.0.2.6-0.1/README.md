# Comparing `tmp/codebat-0.0.2.6.tar.gz` & `tmp/codebat-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebat-0.0.2.6.tar", last modified: Sat Apr 27 16:12:17 2024, max compression
+gzip compressed data, was "codebat-0.1.tar", last modified: Sat Apr 27 16:16:27 2024, max compression
```

## Comparing `codebat-0.0.2.6.tar` & `codebat-0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 16:12:17.305369 codebat-0.0.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-27 16:12:17.274350 codebat-0.0.2.6/CodeBat/
--rw-rw-rw-   0        0        0     3892 2024-04-27 16:11:58.000000 codebat-0.0.2.6/CodeBat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 16:12:17.296113 codebat-0.0.2.6/CodeBat.egg-info/
--rw-rw-rw-   0        0        0      536 2024-04-27 16:12:17.000000 codebat-0.0.2.6/CodeBat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-27 16:12:17.000000 codebat-0.0.2.6/CodeBat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 16:12:17.000000 codebat-0.0.2.6/CodeBat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 16:12:17.000000 codebat-0.0.2.6/CodeBat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 16:12:17.000000 codebat-0.0.2.6/CodeBat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0      536 2024-04-27 16:12:17.300284 codebat-0.0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 04:18:15.000000 codebat-0.0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 16:12:17.306368 codebat-0.0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-27 16:11:58.000000 codebat-0.0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:16:27.825392 codebat-0.1/
+drwxrwxrwx   0        0        0        0 2024-04-27 16:16:27.804015 codebat-0.1/CodeBat/
+-rw-rw-rw-   0        0        0     3892 2024-04-27 16:16:15.000000 codebat-0.1/CodeBat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:16:27.819608 codebat-0.1/CodeBat.egg-info/
+-rw-rw-rw-   0        0        0      532 2024-04-27 16:16:27.000000 codebat-0.1/CodeBat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-27 16:16:27.000000 codebat-0.1/CodeBat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 16:16:27.000000 codebat-0.1/CodeBat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 16:16:27.000000 codebat-0.1/CodeBat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 16:16:27.000000 codebat-0.1/CodeBat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      532 2024-04-27 16:16:27.821662 codebat-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 04:18:15.000000 codebat-0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 16:16:27.825392 codebat-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      716 2024-04-27 16:15:59.000000 codebat-0.1/setup.py
```

### Comparing `codebat-0.0.2.6/CodeBat/__init__.py` & `codebat-0.1/CodeBat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import json
 
 info = {
     "version": "0.1",
     "author": "ShawnMerry",
-    "buildTime": "2404270236"
+    "buildTime": "2404280016"
 }
 
 
 def login(identity, password):
     response = requests.post("https://api.codemao.cn/tiger/v3/web/accounts/login",
                              json={"pid": "65edCTyg", "identity": identity, "password": password})
     return {"status": response.status_code, "data": json.loads(response.text)}
```

### Comparing `codebat-0.0.2.6/CodeBat.egg-info/PKG-INFO` & `codebat-0.1/CodeBat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeBat
-Version: 0.0.2.6
+Version: 0.1
 Summary: A Python Library about Codemao API.
 Home-page: https://github.com/ShawnMerryCode/CodeBat
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codebat-0.0.2.6/LICENSE.txt` & `codebat-0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codebat-0.0.2.6/PKG-INFO` & `codebat-0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeBat
-Version: 0.0.2.6
+Version: 0.1
 Summary: A Python Library about Codemao API.
 Home-page: https://github.com/ShawnMerryCode/CodeBat
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codebat-0.0.2.6/setup.py` & `codebat-0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="CodeBat",
-    version="0.0.2.6",
+    version="0.1",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library about Codemao API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShawnMerryCode/CodeBat",
     packages=find_packages(),
```

