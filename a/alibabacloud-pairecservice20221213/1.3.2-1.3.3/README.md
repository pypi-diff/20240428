# Comparing `tmp/alibabacloud_pairecservice20221213-1.3.2.tar.gz` & `tmp/alibabacloud_pairecservice20221213-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pairecservice20221213-1.3.2.tar", last modified: Fri Mar 22 03:30:17 2024, max compression
+gzip compressed data, was "dist/alibabacloud_pairecservice20221213-1.3.3.tar", last modified: Sun Apr 28 01:34:03 2024, max compression
```

## Comparing `alibabacloud_pairecservice20221213-1.3.2.tar` & `alibabacloud_pairecservice20221213-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/
--rw-r--r--   0 root         (0) root         (0)     7278 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1135 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1220 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213/__init__.py
--rw-r--r--   0 root         (0) root         (0)   348615 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213/client.py
--rw-r--r--   0 root         (0) root         (0)   464329 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-22 03:30:17.000000 alibabacloud_pairecservice20221213-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2661 2024-03-22 03:30:16.000000 alibabacloud_pairecservice20221213-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)     7354 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   348615 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/client.py
+-rw-r--r--   0 root         (0) root         (0)   464329 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/setup.py
```

### Comparing `alibabacloud_pairecservice20221213-1.3.2/ChangeLog.md` & `alibabacloud_pairecservice20221213-1.3.3/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-03-22 Version: 1.3.2
+- Generated python 2022-12-13 for PaiRecService.
+
 2024-03-20 Version: 1.3.1
 - Update API CreateExperimentGroup: add param RegionId.
 - Update API CreateExperimentGroup: update param body.
 - Update API GetExperimentGroup: add param RegionId.
 - Update API GetExperimentGroup: update response param.
 - Update API GetLayer: add param RegionId.
 - Update API GetLayer: update response param.
```

### Comparing `alibabacloud_pairecservice20221213-1.3.2/LICENSE` & `alibabacloud_pairecservice20221213-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.2/PKG-INFO` & `alibabacloud_pairecservice20221213-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pairecservice20221213
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud PaiRecService (20221213) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pairecservice20221213-1.3.2/README-CN.md` & `alibabacloud_pairecservice20221213-1.3.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.2/README.md` & `alibabacloud_pairecservice20221213-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213/client.py` & `alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213/models.py` & `alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.2/alibabacloud_pairecservice20221213.egg-info/PKG-INFO` & `alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pairecservice20221213
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud PaiRecService (20221213) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pairecservice20221213-1.3.2/setup.py` & `alibabacloud_pairecservice20221213-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pairecservice20221213.
 
-Created on 22/03/2024
+Created on 28/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pairecservice20221213"
 NAME = "alibabacloud_pairecservice20221213" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PaiRecService (20221213) SDK Library for Python"
```

