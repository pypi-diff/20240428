# Comparing `tmp/istr_python-0.1.6.tar.gz` & `tmp/istr_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.1.6.tar", last modified: Sun Apr 28 10:14:28 2024, max compression
+gzip compressed data, was "istr_python-0.1.7.tar", last modified: Sun Apr 28 10:19:56 2024, max compression
```

## Comparing `istr_python-0.1.6.tar` & `istr_python-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 10:14:28.213887 istr_python-0.1.6/
--rw-rw-rw-   0        0        0    10736 2024-04-28 10:14:28.212379 istr_python-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     9816 2024-04-28 10:12:50.000000 istr_python-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 10:14:28.184823 istr_python-0.1.6/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.6/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.6/istr/install istr.py
--rw-rw-rw-   0        0        0    18187 2024-04-28 09:43:05.000000 istr_python-0.1.6/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-28 10:14:28.210380 istr_python-0.1.6/istr_python.egg-info/
--rw-rw-rw-   0        0        0    10736 2024-04-28 10:14:28.000000 istr_python-0.1.6/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-28 10:14:28.000000 istr_python-0.1.6/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 10:14:28.000000 istr_python-0.1.6/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 10:14:28.000000 istr_python-0.1.6/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      658 2024-04-28 10:14:22.000000 istr_python-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 10:14:28.214896 istr_python-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 10:14:28.208379 istr_python-0.1.6/tests/
--rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.6/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:19:56.897481 istr_python-0.1.7/
+-rw-rw-rw-   0        0        0    10774 2024-04-28 10:19:56.894482 istr_python-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9853 2024-04-28 10:19:47.000000 istr_python-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 10:19:56.859832 istr_python-0.1.7/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.7/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.7/istr/install istr.py
+-rw-rw-rw-   0        0        0    18187 2024-04-28 09:43:05.000000 istr_python-0.1.7/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:19:56.890236 istr_python-0.1.7/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    10774 2024-04-28 10:19:56.000000 istr_python-0.1.7/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-28 10:19:56.000000 istr_python-0.1.7/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 10:19:56.000000 istr_python-0.1.7/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 10:19:56.000000 istr_python-0.1.7/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      658 2024-04-28 10:19:51.000000 istr_python-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 10:19:56.897991 istr_python-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 10:19:56.885757 istr_python-0.1.7/tests/
+-rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.7/tests/test_istr.py
```

### Comparing `istr_python-0.1.6/PKG-INFO` & `istr_python-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -416,11 +416,12 @@
 Remark: For bases other than 10, the string will never be reformatted!
 
 # Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
-![PyPI](https://img.shields.io/pypi/v/istr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr)
+# Badges
+![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
-![PyPI - License](https://img.shields.io/pypi/l/istr) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
+![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
  ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-0.1.6/README.md` & `istr_python-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -403,11 +403,12 @@
 Remark: For bases other than 10, the string will never be reformatted!
 
 # Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
-![PyPI](https://img.shields.io/pypi/v/istr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr)
+# Badges
+![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
-![PyPI - License](https://img.shields.io/pypi/l/istr) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
+![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
  ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-0.1.6/istr/install istr.py` & `istr_python-0.1.7/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.6/istr/istr.py` & `istr_python-0.1.7/istr/istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.6/istr_python.egg-info/PKG-INFO` & `istr_python-0.1.7/istr_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -416,11 +416,12 @@
 Remark: For bases other than 10, the string will never be reformatted!
 
 # Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
-![PyPI](https://img.shields.io/pypi/v/istr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr)
+# Badges
+![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
-![PyPI - License](https://img.shields.io/pypi/l/istr) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
+![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
  ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-0.1.6/pyproject.toml` & `istr_python-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.1.6"
+version = "0.1.7"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-0.1.6/tests/test_istr.py` & `istr_python-0.1.7/tests/test_istr.py`

 * *Files identical despite different names*

