# Comparing `tmp/stack_overflow_watchman-0.1.0.tar.gz` & `tmp/stack_overflow_watchman-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stack_overflow_watchman-0.1.0.tar", max compression
+gzip compressed data, was "stack_overflow_watchman-1.0.0.tar", max compression
```

## Comparing `stack_overflow_watchman-0.1.0.tar` & `stack_overflow_watchman-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       27 2024-04-27 19:10:53.379463 stack_overflow_watchman-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-27 19:10:53.381859 stack_overflow_watchman-0.1.0/LICENSE
--rw-r--r--   0        0        0     5316 2024-04-27 19:10:53.382805 stack_overflow_watchman-0.1.0/README.md
--rw-r--r--   0        0        0     1080 2024-04-27 19:10:53.384585 stack_overflow_watchman-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7593 2024-04-27 19:10:53.385454 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/__init__.py
--rw-r--r--   0        0        0       27 2024-04-27 19:10:53.386162 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/__main__.py
--rw-r--r--   0        0        0        0 2024-04-27 19:10:53.386316 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/clients/__init__.py
--rw-r--r--   0        0        0     4637 2024-04-27 19:10:53.387421 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/clients/stack_overflow_wrapper.py
--rw-r--r--   0        0        0      287 2024-04-27 19:10:53.388160 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/exceptions.py
--rw-r--r--   0        0        0    11431 2024-04-27 19:10:53.388927 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/loggers.py
--rw-r--r--   0        0        0        0 2024-04-27 19:10:53.389197 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/models/__init__.py
--rw-r--r--   0        0        0     2151 2024-04-27 19:10:53.390130 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/models/models.py
--rw-r--r--   0        0        0     2149 2024-04-27 19:10:53.390820 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/models/signature.py
--rw-r--r--   0        0        0     3594 2024-04-27 19:10:53.391685 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/signature_updater.py
--rw-r--r--   0        0        0     5449 2024-04-27 19:10:53.392511 stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/stack_overflow_search.py
--rw-r--r--   0        0        0     6087 1970-01-01 00:00:00.000000 stack_overflow_watchman-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5316 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/README.md
+-rw-r--r--   0        0        0     1080 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7593 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/clients/__init__.py
+-rw-r--r--   0        0        0     4637 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/clients/stack_overflow_wrapper.py
+-rw-r--r--   0        0        0      287 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/exceptions.py
+-rw-r--r--   0        0        0    11431 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/loggers.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/models/__init__.py
+-rw-r--r--   0        0        0     2151 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/models/models.py
+-rw-r--r--   0        0        0     2149 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/models/signature.py
+-rw-r--r--   0        0        0     3594 2024-04-28 18:36:28.013199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/signature_updater.py
+-rw-r--r--   0        0        0     5449 2024-04-28 18:36:28.017199 stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/stack_overflow_search.py
+-rw-r--r--   0        0        0     6087 1970-01-01 00:00:00.000000 stack_overflow_watchman-1.0.0/PKG-INFO
```

### Comparing `stack_overflow_watchman-0.1.0/LICENSE` & `stack_overflow_watchman-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/README.md` & `stack_overflow_watchman-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/pyproject.toml` & `stack_overflow_watchman-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stack-overflow-watchman"
-version = "0.1.0"
+version = "1.0.0"
 description = "Detecting exposed secrets in Stack Overflow Enterprise for Teams"
 authors = ["PaperMtn <papermtn@protonmail.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://papermtn.co.uk/category/tools/stack-overflow-watchman"
 repository = "https://github.com/PaperMtn/stack-overflow-watchman"
 packages = [{include = "stack_overflow_watchman", from = "src"}]
```

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/__init__.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/__init__.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/clients/stack_overflow_wrapper.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/clients/stack_overflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/loggers.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/loggers.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/models/models.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/models/models.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/models/signature.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/models/signature.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/signature_updater.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/signature_updater.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/src/stack_overflow_watchman/stack_overflow_search.py` & `stack_overflow_watchman-1.0.0/src/stack_overflow_watchman/stack_overflow_search.py`

 * *Files identical despite different names*

### Comparing `stack_overflow_watchman-0.1.0/PKG-INFO` & `stack_overflow_watchman-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stack-overflow-watchman
-Version: 0.1.0
+Version: 1.0.0
 Summary: Detecting exposed secrets in Stack Overflow Enterprise for Teams
 Home-page: https://papermtn.co.uk/category/tools/stack-overflow-watchman
 License: GPL-3.0
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

