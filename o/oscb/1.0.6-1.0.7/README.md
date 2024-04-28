# Comparing `tmp/oscb-1.0.6.tar.gz` & `tmp/oscb-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.0.6.tar", last modified: Sun Apr 28 01:03:20 2024, max compression
+gzip compressed data, was "oscb-1.0.7.tar", last modified: Sun Apr 28 03:56:51 2024, max compression
```

## Comparing `oscb-1.0.6.tar` & `oscb-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 01:03:20.209242 oscb-1.0.6/
--rw-rw-rw-   0        0        0      650 2024-04-28 01:03:20.209242 oscb-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 01:03:20.187679 oscb-1.0.6/oscb/
--rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.0.6/oscb/__init__.py
--rw-rw-rw-   0        0        0      650 2024-04-28 01:02:11.000000 oscb-1.0.6/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-04-28 01:03:20.206941 oscb-1.0.6/oscb.egg-info/
--rw-rw-rw-   0        0        0      650 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 01:03:20.209242 oscb-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1735 2024-04-28 01:02:44.000000 oscb-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 03:56:51.486747 oscb-1.0.7/
+-rw-rw-rw-   0        0        0      658 2024-04-28 03:56:51.485729 oscb-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 03:56:51.451465 oscb-1.0.7/oscb/
+-rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.0.7/oscb/__init__.py
+-rw-rw-rw-   0        0        0      650 2024-04-28 03:50:49.000000 oscb-1.0.7/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-04-28 03:56:51.484743 oscb-1.0.7/oscb.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 03:56:51.486747 oscb-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2024-04-28 03:50:39.000000 oscb-1.0.7/setup.py
```

### Comparing `oscb-1.0.6/PKG-INFO` & `oscb-1.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+
+Long description of your package
```

### Comparing `oscb-1.0.6/oscb/version.py` & `oscb-1.0.7/oscb/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.0.6/oscb.egg-info/PKG-INFO` & `oscb-1.0.7/oscb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+
+Long description of your package
```

