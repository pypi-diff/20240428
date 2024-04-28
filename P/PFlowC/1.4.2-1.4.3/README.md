# Comparing `tmp/PFlowC-1.4.2.tar.gz` & `tmp/PFlowC-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.4.2.tar", last modified: Sun Apr 28 09:43:53 2024, max compression
+gzip compressed data, was "PFlowC-1.4.3.tar", last modified: Sun Apr 28 10:51:14 2024, max compression
```

## Comparing `PFlowC-1.4.2.tar` & `PFlowC-1.4.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.582559 PFlowC-1.4.2/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.580366 PFlowC-1.4.2/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:43:41.000000 PFlowC-1.4.2/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1927 2024-04-28 09:29:46.000000 PFlowC-1.4.2/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.2/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.581613 PFlowC-1.4.2/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.2/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.2/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.582026 PFlowC-1.4.2/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.2/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.2/PFlowC/utils/logger.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.581290 PFlowC-1.4.2/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1183 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      361 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/requires.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1183 2024-04-28 09:43:53.582356 PFlowC-1.4.2/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.4.2/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:43:53.582602 PFlowC-1.4.2/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1681 2024-04-28 09:43:29.000000 PFlowC-1.4.2/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.557149 PFlowC-1.4.3/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.554326 PFlowC-1.4.3/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:39:09.000000 PFlowC-1.4.3/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     6067 2024-04-28 10:41:10.000000 PFlowC-1.4.3/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.3/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.555450 PFlowC-1.4.3/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.3/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.3/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.556131 PFlowC-1.4.3/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.3/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.3/PFlowC/utils/logger.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.555154 PFlowC-1.4.3/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1443 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      382 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1443 2024-04-28 10:51:14.556939 PFlowC-1.4.3/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      483 2024-04-28 10:51:03.000000 PFlowC-1.4.3/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:51:14.557189 PFlowC-1.4.3/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1634 2024-04-28 10:39:18.000000 PFlowC-1.4.3/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.556464 PFlowC-1.4.3/tests/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-1.4.3/tests/test-banner.py
```

### Comparing `PFlowC-1.4.2/PFlowC/proxy.py` & `PFlowC-1.4.3/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.2/PFlowC/proxy_helper/macosx.py` & `PFlowC-1.4.3/PFlowC/proxy_helper/macosx.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.2/PFlowC/utils/logger.py` & `PFlowC-1.4.3/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.2/PFlowC.egg-info/PKG-INFO` & `PFlowC-1.4.3/PFlowC.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.2
+Version: 1.4.3
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,8 +28,22 @@
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
 A net flow pilot in order to handle some proxy configuration automatically.
 
+* Install:
 
+    Run ``pip install PFlowC -U`` on the shell.
+
+* set on the proxy setting:
+
+    Run ``pflow-cli on`` on the shell.
+
+* set off the proxy setting:
+
+    Run ``pflow-cli off`` on the shell.
+
+* Ask for Help:
+
+    Run ``pflow-cli --help`` on the shell.
```

### Comparing `PFlowC-1.4.2/PKG-INFO` & `PFlowC-1.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.2
+Version: 1.4.3
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,8 +28,22 @@
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
 A net flow pilot in order to handle some proxy configuration automatically.
 
+* Install:
 
+    Run ``pip install PFlowC -U`` on the shell.
+
+* set on the proxy setting:
+
+    Run ``pflow-cli on`` on the shell.
+
+* set off the proxy setting:
+
+    Run ``pflow-cli off`` on the shell.
+
+* Ask for Help:
+
+    Run ``pflow-cli --help`` on the shell.
```

### Comparing `PFlowC-1.4.2/setup.py` & `PFlowC-1.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 """====================================
 @Author:Sadam·Sadik
 @Email：1903249375@qq.com
 @Date：2024/4/28
 @Software: PyCharm
 @disc:
 ======================================="""
-import pip
-import logging
-import pkg_resources
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.4.2',
+    version='1.4.3',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=['colorlog', 'click'],
```
