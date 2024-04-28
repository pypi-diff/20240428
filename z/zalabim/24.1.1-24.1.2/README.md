# Comparing `tmp/zalabim-24.1.1.tar.gz` & `tmp/zalabim-24.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalabim-24.1.1.tar", last modified: Sun Apr 28 13:10:03 2024, max compression
+gzip compressed data, was "zalabim-24.1.2.tar", last modified: Sun Apr 28 15:14:09 2024, max compression
```

## Comparing `zalabim-24.1.1.tar` & `zalabim-24.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.416637 zalabim-24.1.1/
--rw-rw-rw-   0        0        0     3044 2024-04-28 13:10:03.415626 zalabim-24.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2521 2024-04-28 12:42:18.000000 zalabim-24.1.1/README.md
--rw-rw-rw-   0        0        0      678 2024-04-28 13:09:58.000000 zalabim-24.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 13:10:03.416637 zalabim-24.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.400505 zalabim-24.1.1/tests/
--rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 zalabim-24.1.1/tests/test_cap_now.py
--rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 zalabim-24.1.1/tests/test_componentgenerator.py
--rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 zalabim-24.1.1/tests/test_datetime.py
--rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 zalabim-24.1.1/tests/test_distributions.py
--rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 zalabim-24.1.1/tests/test_misc.py
--rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 zalabim-24.1.1/tests/test_monitor.py
--rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 zalabim-24.1.1/tests/test_process.py
--rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 zalabim-24.1.1/tests/test_queue.py
--rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 zalabim-24.1.1/tests/test_salabim.py
--rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 zalabim-24.1.1/tests/test_state.py
--rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 zalabim-24.1.1/tests/test_store.py
--rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 zalabim-24.1.1/tests/test_timeunit.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.401950 zalabim-24.1.1/zalabim/
--rw-rw-rw-   0        0        0  1093582 2024-04-28 13:00:47.000000 zalabim-24.1.1/zalabim/zalabim.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.414614 zalabim-24.1.1/zalabim.egg-info/
--rw-rw-rw-   0        0        0     3044 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 15:14:09.139481 zalabim-24.1.2/
+-rw-rw-rw-   0        0        0     3045 2024-04-28 15:14:09.136502 zalabim-24.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2024-04-28 13:15:29.000000 zalabim-24.1.2/README.md
+-rw-rw-rw-   0        0        0      686 2024-04-28 15:14:02.000000 zalabim-24.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 15:14:09.139481 zalabim-24.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 15:14:09.120660 zalabim-24.1.2/tests/
+-rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 zalabim-24.1.2/tests/test_cap_now.py
+-rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 zalabim-24.1.2/tests/test_componentgenerator.py
+-rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 zalabim-24.1.2/tests/test_datetime.py
+-rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 zalabim-24.1.2/tests/test_distributions.py
+-rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 zalabim-24.1.2/tests/test_misc.py
+-rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 zalabim-24.1.2/tests/test_monitor.py
+-rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 zalabim-24.1.2/tests/test_process.py
+-rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 zalabim-24.1.2/tests/test_queue.py
+-rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 zalabim-24.1.2/tests/test_salabim.py
+-rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 zalabim-24.1.2/tests/test_state.py
+-rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 zalabim-24.1.2/tests/test_store.py
+-rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 zalabim-24.1.2/tests/test_timeunit.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:14:09.123744 zalabim-24.1.2/zalabim/
+-rw-rw-rw-   0        0        0  1093582 2024-04-28 13:00:47.000000 zalabim-24.1.2/zalabim/zalabim.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:14:09.135373 zalabim-24.1.2/zalabim.egg-info/
+-rw-rw-rw-   0        0        0     3045 2024-04-28 15:14:09.000000 zalabim-24.1.2/zalabim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-04-28 15:14:09.000000 zalabim-24.1.2/zalabim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 15:14:09.000000 zalabim-24.1.2/zalabim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-28 15:14:09.000000 zalabim-24.1.2/zalabim.egg-info/top_level.txt
```

### Comparing `zalabim-24.1.1/PKG-INFO` & `zalabim-24.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalabim
-Version: 24.1.1
+Version: 24.1.2
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/zalabim
 Project-URL: Repository, https://github.com/salabim/zalabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,13 +52,13 @@
 
 Ruud van der Ham is available and willing to help users with issues related to the package and modeling in general. He also provides services such as code and model reviews, consultancy, and training.
 
 ## Getting Started
 
 To start using salabim, visit [www.salabim.org](www.salabim.org) for installation instructions and further details.
 
-# Badges
+## Badges
 
 ![PyPI](https://img.shields.io/pypi/v/zalabim) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zalabim) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/zalabim)
 
 ![PyPI - License](https://img.shields.io/pypi/l/zalabim) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
  ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/zalabim)
```

### Comparing `zalabim-24.1.1/README.md` & `zalabim-24.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,13 +39,13 @@
 
 Ruud van der Ham is available and willing to help users with issues related to the package and modeling in general. He also provides services such as code and model reviews, consultancy, and training.
 
 ## Getting Started
 
 To start using salabim, visit [www.salabim.org](www.salabim.org) for installation instructions and further details.
 
-# Badges
+## Badges
 
 ![PyPI](https://img.shields.io/pypi/v/zalabim) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zalabim) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/zalabim)
 
 ![PyPI - License](https://img.shields.io/pypi/l/zalabim) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
  ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/zalabim)
```

### Comparing `zalabim-24.1.1/pyproject.toml` & `zalabim-24.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 [project]
 name = "zalabim"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "salabim - discrete event simulation in Python"
-version = "24.1.1"
+version = "24.1.2"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only"
 ]
 [project.urls]
 Homepage = "https://github.com/salabim/zalabim"
 Repository = "https://github.com/salabim/zalabim"
 
 [tool.setuptools]
-packages = ["zalabim"]
+packages = ["zalabim","fonts"]
```

### Comparing `zalabim-24.1.1/tests/test_cap_now.py` & `zalabim-24.1.2/tests/test_cap_now.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_componentgenerator.py` & `zalabim-24.1.2/tests/test_componentgenerator.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_datetime.py` & `zalabim-24.1.2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_distributions.py` & `zalabim-24.1.2/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_misc.py` & `zalabim-24.1.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_monitor.py` & `zalabim-24.1.2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_process.py` & `zalabim-24.1.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_queue.py` & `zalabim-24.1.2/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_state.py` & `zalabim-24.1.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/tests/test_timeunit.py` & `zalabim-24.1.2/tests/test_timeunit.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/zalabim/zalabim.py` & `zalabim-24.1.2/zalabim/zalabim.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1.1/zalabim.egg-info/PKG-INFO` & `zalabim-24.1.2/zalabim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalabim
-Version: 24.1.1
+Version: 24.1.2
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/zalabim
 Project-URL: Repository, https://github.com/salabim/zalabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,13 +52,13 @@
 
 Ruud van der Ham is available and willing to help users with issues related to the package and modeling in general. He also provides services such as code and model reviews, consultancy, and training.
 
 ## Getting Started
 
 To start using salabim, visit [www.salabim.org](www.salabim.org) for installation instructions and further details.
 
-# Badges
+## Badges
 
 ![PyPI](https://img.shields.io/pypi/v/zalabim) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zalabim) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/zalabim)
 
 ![PyPI - License](https://img.shields.io/pypi/l/zalabim) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
  ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/zalabim)
```

