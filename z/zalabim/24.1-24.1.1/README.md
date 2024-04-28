# Comparing `tmp/zalabim-24.1.tar.gz` & `tmp/zalabim-24.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalabim-24.1.tar", last modified: Sun Apr 28 13:00:57 2024, max compression
+gzip compressed data, was "zalabim-24.1.1.tar", last modified: Sun Apr 28 13:10:03 2024, max compression
```

## Comparing `zalabim-24.1.tar` & `zalabim-24.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:00:57.980659 zalabim-24.1/
--rw-rw-rw-   0        0        0     3042 2024-04-28 13:00:57.979097 zalabim-24.1/PKG-INFO
--rw-rw-rw-   0        0        0     2521 2024-04-28 12:42:18.000000 zalabim-24.1/README.md
--rw-rw-rw-   0        0        0      676 2024-04-28 13:00:52.000000 zalabim-24.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 13:00:57.980659 zalabim-24.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 13:00:57.964290 zalabim-24.1/tests/
--rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 zalabim-24.1/tests/test_cap_now.py
--rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 zalabim-24.1/tests/test_componentgenerator.py
--rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 zalabim-24.1/tests/test_datetime.py
--rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 zalabim-24.1/tests/test_distributions.py
--rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 zalabim-24.1/tests/test_misc.py
--rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 zalabim-24.1/tests/test_monitor.py
--rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 zalabim-24.1/tests/test_process.py
--rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 zalabim-24.1/tests/test_queue.py
--rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 zalabim-24.1/tests/test_salabim.py
--rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 zalabim-24.1/tests/test_state.py
--rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 zalabim-24.1/tests/test_store.py
--rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 zalabim-24.1/tests/test_timeunit.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:00:57.965387 zalabim-24.1/zalabim/
--rw-rw-rw-   0        0        0  1093582 2024-04-28 13:00:47.000000 zalabim-24.1/zalabim/zalabim.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:00:57.978097 zalabim-24.1/zalabim.egg-info/
--rw-rw-rw-   0        0        0     3042 2024-04-28 13:00:57.000000 zalabim-24.1/zalabim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-04-28 13:00:57.000000 zalabim-24.1/zalabim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:00:57.000000 zalabim-24.1/zalabim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-28 13:00:57.000000 zalabim-24.1/zalabim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.416637 zalabim-24.1.1/
+-rw-rw-rw-   0        0        0     3044 2024-04-28 13:10:03.415626 zalabim-24.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2521 2024-04-28 12:42:18.000000 zalabim-24.1.1/README.md
+-rw-rw-rw-   0        0        0      678 2024-04-28 13:09:58.000000 zalabim-24.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:10:03.416637 zalabim-24.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.400505 zalabim-24.1.1/tests/
+-rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 zalabim-24.1.1/tests/test_cap_now.py
+-rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 zalabim-24.1.1/tests/test_componentgenerator.py
+-rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 zalabim-24.1.1/tests/test_datetime.py
+-rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 zalabim-24.1.1/tests/test_distributions.py
+-rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 zalabim-24.1.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 zalabim-24.1.1/tests/test_monitor.py
+-rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 zalabim-24.1.1/tests/test_process.py
+-rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 zalabim-24.1.1/tests/test_queue.py
+-rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 zalabim-24.1.1/tests/test_salabim.py
+-rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 zalabim-24.1.1/tests/test_state.py
+-rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 zalabim-24.1.1/tests/test_store.py
+-rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 zalabim-24.1.1/tests/test_timeunit.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.401950 zalabim-24.1.1/zalabim/
+-rw-rw-rw-   0        0        0  1093582 2024-04-28 13:00:47.000000 zalabim-24.1.1/zalabim/zalabim.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:10:03.414614 zalabim-24.1.1/zalabim.egg-info/
+-rw-rw-rw-   0        0        0     3044 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 13:10:03.000000 zalabim-24.1.1/zalabim.egg-info/top_level.txt
```

### Comparing `zalabim-24.1/PKG-INFO` & `zalabim-24.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalabim
-Version: 24.1
+Version: 24.1.1
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/zalabim
 Project-URL: Repository, https://github.com/salabim/zalabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `zalabim-24.1/README.md` & `zalabim-24.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/pyproject.toml` & `zalabim-24.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "zalabim"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "salabim - discrete event simulation in Python"
-version = "24.1"
+version = "24.1.1"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `zalabim-24.1/tests/test_cap_now.py` & `zalabim-24.1.1/tests/test_cap_now.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_componentgenerator.py` & `zalabim-24.1.1/tests/test_componentgenerator.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_datetime.py` & `zalabim-24.1.1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_distributions.py` & `zalabim-24.1.1/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_misc.py` & `zalabim-24.1.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_monitor.py` & `zalabim-24.1.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_process.py` & `zalabim-24.1.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_queue.py` & `zalabim-24.1.1/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_state.py` & `zalabim-24.1.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/tests/test_timeunit.py` & `zalabim-24.1.1/tests/test_timeunit.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/zalabim/zalabim.py` & `zalabim-24.1.1/zalabim/zalabim.py`

 * *Files identical despite different names*

### Comparing `zalabim-24.1/zalabim.egg-info/PKG-INFO` & `zalabim-24.1.1/zalabim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalabim
-Version: 24.1
+Version: 24.1.1
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/zalabim
 Project-URL: Repository, https://github.com/salabim/zalabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

