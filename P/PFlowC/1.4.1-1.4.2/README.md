# Comparing `tmp/PFlowC-1.4.1.tar.gz` & `tmp/PFlowC-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.4.1.tar", last modified: Sun Apr 28 09:33:45 2024, max compression
+gzip compressed data, was "PFlowC-1.4.2.tar", last modified: Sun Apr 28 09:43:53 2024, max compression
```

## Comparing `PFlowC-1.4.1.tar` & `PFlowC-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.971889 PFlowC-1.4.1/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.969759 PFlowC-1.4.1/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:33:42.000000 PFlowC-1.4.1/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1927 2024-04-28 09:29:46.000000 PFlowC-1.4.1/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.1/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.970883 PFlowC-1.4.1/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.1/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.1/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.971328 PFlowC-1.4.1/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.1/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.1/PFlowC/utils/logger.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.970522 PFlowC-1.4.1/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      332 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:33:45.971703 PFlowC-1.4.1/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.4.1/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:33:45.971924 PFlowC-1.4.1/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2344 2024-04-28 09:33:35.000000 PFlowC-1.4.1/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.582559 PFlowC-1.4.2/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.580366 PFlowC-1.4.2/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:43:41.000000 PFlowC-1.4.2/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1927 2024-04-28 09:29:46.000000 PFlowC-1.4.2/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.2/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.581613 PFlowC-1.4.2/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.2/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.2/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.582026 PFlowC-1.4.2/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.2/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.2/PFlowC/utils/logger.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:43:53.581290 PFlowC-1.4.2/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1183 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      361 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 09:43:53.000000 PFlowC-1.4.2/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1183 2024-04-28 09:43:53.582356 PFlowC-1.4.2/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.4.2/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:43:53.582602 PFlowC-1.4.2/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1681 2024-04-28 09:43:29.000000 PFlowC-1.4.2/setup.py
```

### Comparing `PFlowC-1.4.1/PFlowC/main.py` & `PFlowC-1.4.2/PFlowC/main.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.1/PFlowC/proxy.py` & `PFlowC-1.4.2/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.1/PFlowC/proxy_helper/macosx.py` & `PFlowC-1.4.2/PFlowC/proxy_helper/macosx.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.1/PFlowC/utils/logger.py` & `PFlowC-1.4.2/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.1/PFlowC.egg-info/PKG-INFO` & `PFlowC-1.4.2/PFlowC.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.1
+Version: 1.4.2
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
+Requires-Dist: colorlog
+Requires-Dist: click
 
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
```

### Comparing `PFlowC-1.4.1/PKG-INFO` & `PFlowC-1.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.1
+Version: 1.4.2
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
+Requires-Dist: colorlog
+Requires-Dist: click
 
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
```

