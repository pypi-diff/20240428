# Comparing `tmp/istr_python-0.1.2.tar.gz` & `tmp/istr_python-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.1.2.tar", last modified: Sat Apr 27 16:58:03 2024, max compression
+gzip compressed data, was "istr_python-0.1.2a0.tar", last modified: Sun Apr 28 09:11:20 2024, max compression
```

## Comparing `istr_python-0.1.2.tar` & `istr_python-0.1.2a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.589473 istr_python-0.1.2/
--rw-rw-rw-   0        0        0    10334 2024-04-27 16:58:03.585523 istr_python-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9420 2024-04-26 11:01:42.000000 istr_python-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.537898 istr_python-0.1.2/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.2/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.2/istr/install istr.py
--rw-rw-rw-   0        0        0    18172 2024-04-27 16:04:34.000000 istr_python-0.1.2/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.582447 istr_python-0.1.2/istr_python.egg-info/
--rw-rw-rw-   0        0        0    10334 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      658 2024-04-27 16:57:58.000000 istr_python-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 16:58:03.591476 istr_python-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.579798 istr_python-0.1.2/tests/
--rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.2/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:11:20.515562 istr_python-0.1.2a0/
+-rw-rw-rw-   0        0        0    10340 2024-04-28 09:11:20.513029 istr_python-0.1.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     9424 2024-04-28 09:11:01.000000 istr_python-0.1.2a0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 09:11:20.468501 istr_python-0.1.2a0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.2a0/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.2a0/istr/install istr.py
+-rw-rw-rw-   0        0        0    18173 2024-04-28 09:10:53.000000 istr_python-0.1.2a0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:11:20.510638 istr_python-0.1.2a0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    10340 2024-04-28 09:11:20.000000 istr_python-0.1.2a0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-28 09:11:20.000000 istr_python-0.1.2a0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:11:20.000000 istr_python-0.1.2a0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 09:11:20.000000 istr_python-0.1.2a0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      659 2024-04-28 09:11:14.000000 istr_python-0.1.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:11:20.516581 istr_python-0.1.2a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 09:11:20.508549 istr_python-0.1.2a0/tests/
+-rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.2a0/tests/test_istr.py
```

### Comparing `istr_python-0.1.2/PKG-INFO` & `istr_python-0.1.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-<img src="https://www.salabim.org/istr1.png" width=500>
+<img src="https://www.salabim.org/istr_logo.png" width=500>
 
 # Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
```

### Comparing `istr_python-0.1.2/README.md` & `istr_python-0.1.2a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://www.salabim.org/istr1.png" width=500>
+<img src="https://www.salabim.org/istr_logo.png" width=500>
 
 # Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
```

### Comparing `istr_python-0.1.2/istr/install istr.py` & `istr_python-0.1.2a0/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.2/istr/istr.py` & `istr_python-0.1.2a0/istr/istr.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "0.1.2"
+__version__ = "0.1.2a"
 import functools
 import math
 
 """
 changelog
 
 version 0.1.2  2024-04-26
```

### Comparing `istr_python-0.1.2/istr_python.egg-info/PKG-INFO` & `istr_python-0.1.2a0/istr_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-<img src="https://www.salabim.org/istr1.png" width=500>
+<img src="https://www.salabim.org/istr_logo.png" width=500>
 
 # Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
```

### Comparing `istr_python-0.1.2/pyproject.toml` & `istr_python-0.1.2a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.1.2"
+version = "0.1.2a"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-0.1.2/tests/test_istr.py` & `istr_python-0.1.2a0/tests/test_istr.py`

 * *Files identical despite different names*

