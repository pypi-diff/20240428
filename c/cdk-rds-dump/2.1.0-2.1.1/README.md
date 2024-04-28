# Comparing `tmp/cdk-rds-dump-2.1.0.tar.gz` & `tmp/cdk-rds-dump-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-2.1.0.tar", last modified: Mon Apr  8 04:52:33 2024, max compression
+gzip compressed data, was "cdk-rds-dump-2.1.1.tar", last modified: Sun Apr 28 06:07:16 2024, max compression
```

## Comparing `cdk-rds-dump-2.1.0.tar` & `cdk-rds-dump-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.891008 cdk-rds-dump-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-08 04:52:33.891008 cdk-rds-dump-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:52:33.891008 cdk-rds-dump-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.883008 cdk-rds-dump-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.887008 cdk-rds-dump-2.1.0/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (127)    25150 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.887008 cdk-rds-dump-2.1.0/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2648201 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/_jsii/cdk-rds-dump@2.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.887008 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:07:16.380824 cdk-rds-dump-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-28 06:07:16.380824 cdk-rds-dump-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:07:16.380824 cdk-rds-dump-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:07:16.372824 cdk-rds-dump-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:07:16.376824 cdk-rds-dump-2.1.1/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (127)    25150 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:07:16.376824 cdk-rds-dump-2.1.1/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2629678 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump/_jsii/cdk-rds-dump@2.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:07:03.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:07:16.376824 cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-28 06:07:16.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-28 06:07:16.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:07:16.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-28 06:07:16.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 06:07:16.000000 cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-2.1.0/LICENSE` & `cdk-rds-dump-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.1.0/PKG-INFO` & `cdk-rds-dump-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 2.1.0
+Version: 2.1.1
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-rds-dump-2.1.0/README.md` & `cdk-rds-dump-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.1.0/setup.py` & `cdk-rds-dump-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "2.1.0",
+    "version": "2.1.1",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@2.1.0.jsii.tgz"
+            "cdk-rds-dump@2.1.1.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.125.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-rds-dump-2.1.0/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-2.1.1/src/cdk_rds_dump/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-2.1.1/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 2.1.0
+Version: 2.1.1
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

