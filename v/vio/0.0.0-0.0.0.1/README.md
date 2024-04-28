# Comparing `tmp/vio-0.0.0.tar.gz` & `tmp/vio-0.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vio-0.0.0.tar", last modified: Sat Apr 27 14:22:59 2024, max compression
+gzip compressed data, was "vio-0.0.0.1.tar", last modified: Sat Apr 27 14:48:03 2024, max compression
```

## Comparing `vio-0.0.0.tar` & `vio-0.0.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 14:22:59.630000 vio-0.0.0/
--rw-rw-rw-   0        0        0      371 2024-04-27 14:23:00.000000 vio-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-27 14:23:00.000000 vio-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-04-27 14:22:50.000000 vio-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:22:59.640000 vio-0.0.0/vio.egg-info/
--rw-rw-rw-   0        0        0      371 2024-04-27 14:23:00.000000 vio-0.0.0/vio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      116 2024-04-27 14:23:00.000000 vio-0.0.0/vio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 14:23:00.000000 vio-0.0.0/vio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 14:23:00.000000 vio-0.0.0/vio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 14:48:03.150000 vio-0.0.0.1/
+-rw-rw-rw-   0        0        0      373 2024-04-27 14:48:04.000000 vio-0.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-27 14:48:04.000000 vio-0.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2024-04-27 14:47:52.000000 vio-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:48:03.150000 vio-0.0.0.1/vio.egg-info/
+-rw-rw-rw-   0        0        0      373 2024-04-27 14:48:04.000000 vio-0.0.0.1/vio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2024-04-27 14:48:04.000000 vio-0.0.0.1/vio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 14:48:04.000000 vio-0.0.0.1/vio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 14:48:04.000000 vio-0.0.0.1/vio.egg-info/top_level.txt
```

### Comparing `vio-0.0.0/setup.py` & `vio-0.0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='vio',
-    version='0.0.0',
+    version='0.0.0.1',
     description='virtual io ...',
     long_description="I'm trying to make a virtual io for python object getter.",
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
     # package_data={
```

