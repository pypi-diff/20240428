# Comparing `tmp/gammarers.aws-secure-log-bucket-1.6.1.tar.gz` & `tmp/gammarers.aws-secure-log-bucket-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-log-bucket-1.6.1.tar", last modified: Tue Apr 23 05:46:47 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-log-bucket-1.6.2.tar", last modified: Sun Apr 28 18:22:59 2024, max compression
```

## Comparing `gammarers.aws-secure-log-bucket-1.6.1.tar` & `gammarers.aws-secure-log-bucket-1.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:46:47.066469 gammarers.aws-secure-log-bucket-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-23 05:46:47.066469 gammarers.aws-secure-log-bucket-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 05:46:47.066469 gammarers.aws-secure-log-bucket-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:46:47.062469 gammarers.aws-secure-log-bucket-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:46:47.062469 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:46:47.062469 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    12820 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:46:47.066469 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24025 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.6.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 05:46:35.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:46:47.062469 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-23 05:46:47.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-23 05:46:47.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 05:46:47.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 05:46:47.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 05:46:47.000000 gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:59.301999 gammarers.aws-secure-log-bucket-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-28 18:22:59.301999 gammarers.aws-secure-log-bucket-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:22:59.301999 gammarers.aws-secure-log-bucket-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:59.297999 gammarers.aws-secure-log-bucket-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:59.297999 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:59.301999 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    12820 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:59.301999 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.6.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:22:45.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:59.297999 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-28 18:22:59.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 18:22:59.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:22:59.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-28 18:22:59.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 18:22:59.000000 gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/LICENSE` & `gammarers.aws-secure-log-bucket-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/PKG-INFO` & `gammarers.aws-secure-log-bucket-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-log-bucket
-Version: 1.6.1
+Version: 1.6.2
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarers/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/README.md` & `gammarers.aws-secure-log-bucket-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/setup.py` & `gammarers.aws-secure-log-bucket-1.6.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-log-bucket",
-    "version": "1.6.1",
+    "version": "1.6.2",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_secure_log_bucket",
         "gammarers.aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@1.6.1.jsii.tgz"
+            "aws-secure-log-bucket@1.6.2.jsii.tgz"
         ],
         "gammarers.aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/__init__.py` & `gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py` & `gammarers.aws-secure-log-bucket-1.6.2/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-secure-log-bucket",
-    "1.6.1",
+    "1.6.2",
     __name__[0:-6],
-    "aws-secure-log-bucket@1.6.1.jsii.tgz",
+    "aws-secure-log-bucket@1.6.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO` & `gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-log-bucket
-Version: 1.6.1
+Version: 1.6.2
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarers/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.1/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt` & `gammarers.aws-secure-log-bucket-1.6.2/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt
 src/gammarers.aws_secure_log_bucket.egg-info/dependency_links.txt
 src/gammarers.aws_secure_log_bucket.egg-info/requires.txt
 src/gammarers.aws_secure_log_bucket.egg-info/top_level.txt
 src/gammarers/aws_secure_log_bucket/__init__.py
 src/gammarers/aws_secure_log_bucket/py.typed
 src/gammarers/aws_secure_log_bucket/_jsii/__init__.py
-src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.6.1.jsii.tgz
+src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.6.2.jsii.tgz
```
