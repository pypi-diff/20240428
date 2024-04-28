# Comparing `tmp/istr_python-0.1.3.tar.gz` & `tmp/istr_python-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.1.3.tar", last modified: Sun Apr 28 09:14:36 2024, max compression
+gzip compressed data, was "istr_python-0.1.3a0.tar", last modified: Sun Apr 28 09:20:18 2024, max compression
```

## Comparing `istr_python-0.1.3.tar` & `istr_python-0.1.3a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 09:14:36.500190 istr_python-0.1.3/
--rw-rw-rw-   0        0        0    10338 2024-04-28 09:14:36.494607 istr_python-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9424 2024-04-28 09:11:01.000000 istr_python-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 09:14:36.418242 istr_python-0.1.3/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.3/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.3/istr/install istr.py
--rw-rw-rw-   0        0        0    18172 2024-04-28 09:14:18.000000 istr_python-0.1.3/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:14:36.490605 istr_python-0.1.3/istr_python.egg-info/
--rw-rw-rw-   0        0        0    10338 2024-04-28 09:14:36.000000 istr_python-0.1.3/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-28 09:14:36.000000 istr_python-0.1.3/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 09:14:36.000000 istr_python-0.1.3/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 09:14:36.000000 istr_python-0.1.3/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      658 2024-04-28 09:14:27.000000 istr_python-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 09:14:36.501192 istr_python-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 09:14:36.485572 istr_python-0.1.3/tests/
--rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.3/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:20:18.259050 istr_python-0.1.3a0/
+-rw-rw-rw-   0        0        0    10340 2024-04-28 09:20:18.255099 istr_python-0.1.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     9424 2024-04-28 09:11:01.000000 istr_python-0.1.3a0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 09:20:18.216593 istr_python-0.1.3a0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.3a0/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.3a0/istr/install istr.py
+-rw-rw-rw-   0        0        0    18173 2024-04-28 09:20:08.000000 istr_python-0.1.3a0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:20:18.251825 istr_python-0.1.3a0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    10340 2024-04-28 09:20:18.000000 istr_python-0.1.3a0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-28 09:20:18.000000 istr_python-0.1.3a0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:20:18.000000 istr_python-0.1.3a0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 09:20:18.000000 istr_python-0.1.3a0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      659 2024-04-28 09:20:12.000000 istr_python-0.1.3a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:20:18.259435 istr_python-0.1.3a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 09:20:18.247274 istr_python-0.1.3a0/tests/
+-rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.3a0/tests/test_istr.py
```

### Comparing `istr_python-0.1.3/PKG-INFO` & `istr_python-0.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.3
+Version: 0.1.3a0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-0.1.3/README.md` & `istr_python-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.3/istr/install istr.py` & `istr_python-0.1.3a0/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.3/istr/istr.py` & `istr_python-0.1.3a0/istr/istr.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "0.1.3"
+__version__ = "0.1.3A"
 import functools
 import math
 
 """
 changelog
 
 version 0.1.2  2024-04-26
```

### Comparing `istr_python-0.1.3/istr_python.egg-info/PKG-INFO` & `istr_python-0.1.3a0/istr_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.3
+Version: 0.1.3a0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-0.1.3/pyproject.toml` & `istr_python-0.1.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.1.3"
+version = "0.1.3A"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-0.1.3/tests/test_istr.py` & `istr_python-0.1.3a0/tests/test_istr.py`

 * *Files identical despite different names*

