# Comparing `tmp/decli-0.6.1.tar.gz` & `tmp/decli-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decli-0.6.1.tar", max compression
+gzip compressed data, was "decli-0.6.2.tar", max compression
```

## Comparing `decli-0.6.1.tar` & `decli-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-06-03 08:50:02.464636 decli-0.6.1/LICENSE
--rw-r--r--   0        0        0    17159 2023-06-03 08:50:02.464636 decli-0.6.1/README.rst
--rw-r--r--   0        0        0       72 2023-06-03 08:50:02.464636 decli-0.6.1/decli/__init__.py
--rw-r--r--   0        0        0     4607 2023-06-03 08:50:02.464636 decli-0.6.1/decli/application.py
--rw-r--r--   0        0        0        0 2023-06-03 08:50:02.464636 decli-0.6.1/decli/py.typed
--rw-r--r--   0        0        0      807 2023-06-03 08:50:02.464636 decli-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    17745 1970-01-01 00:00:00.000000 decli-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-28 17:40:44.284261 decli-0.6.2/LICENSE
+-rw-r--r--   0        0        0    17159 2024-04-28 17:40:44.284261 decli-0.6.2/README.rst
+-rw-r--r--   0        0        0       72 2024-04-28 17:40:44.284261 decli-0.6.2/decli/__init__.py
+-rw-r--r--   0        0        0     4607 2024-04-28 17:40:44.284261 decli-0.6.2/decli/application.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:40:44.284261 decli-0.6.2/decli/py.typed
+-rw-r--r--   0        0        0      892 2024-04-28 17:40:44.284261 decli-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    17796 1970-01-01 00:00:00.000000 decli-0.6.2/PKG-INFO
```

### Comparing `decli-0.6.1/LICENSE` & `decli-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decli-0.6.1/README.rst` & `decli-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `decli-0.6.1/decli/application.py` & `decli-0.6.2/decli/application.py`

 * *Files identical despite different names*

### Comparing `decli-0.6.1/pyproject.toml` & `decli-0.6.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decli"
-version = "0.6.1"
+version = "0.6.2"
 description = "Minimal, easy-to-use, declarative cli tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 readme = 'README.rst'
 
 [tool.poetry.dependencies]
 python = ">=3.7"
@@ -36,7 +36,11 @@
 version_type = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
 version_files = [
     "decli/__init__.py:__version__",
 ]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `decli-0.6.1/PKG-INFO` & `decli-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: decli
-Version: 0.6.1
+Version: 0.6.2
 Summary: Minimal, easy-to-use, declarative cli tool
 License: MIT
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 
 ======
 Decli
 ======
 
 Minimal declarative cli tool.
```

