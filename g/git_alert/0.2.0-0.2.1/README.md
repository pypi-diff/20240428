# Comparing `tmp/git_alert-0.2.0.tar.gz` & `tmp/git_alert-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_alert-0.2.0.tar", max compression
+gzip compressed data, was "git_alert-0.2.1.tar", max compression
```

## Comparing `git_alert-0.2.0.tar` & `git_alert-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2024-04-24 20:33:52.776556 git_alert-0.2.0/LICENSE
--rw-r--r--   0        0        0     3416 2024-04-24 20:33:52.776556 git_alert-0.2.0/README.md
--rw-r--r--   0        0        0      142 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/__init__.py
--rw-r--r--   0        0        0      393 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/__main__.py
--rw-r--r--   0        0        0     1128 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/argument_parser.py
--rw-r--r--   0        0        0     1285 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/repositories.py
--rw-r--r--   0        0        0      433 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/scripts/git_alert.py
--rw-r--r--   0        0        0     1552 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/traverse.py
--rw-r--r--   0        0        0      657 2024-04-24 20:33:52.780556 git_alert-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3900 1970-01-01 00:00:00.000000 git_alert-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-28 21:20:43.864705 git_alert-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3416 2024-04-28 21:20:43.864705 git_alert-0.2.1/README.md
+-rw-r--r--   0        0        0      142 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/__main__.py
+-rw-r--r--   0        0        0     1128 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/argument_parser.py
+-rw-r--r--   0        0        0     1285 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/repositories.py
+-rw-r--r--   0        0        0      433 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/scripts/git_alert.py
+-rw-r--r--   0        0        0     1552 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/traverse.py
+-rw-r--r--   0        0        0      657 2024-04-28 21:20:43.864705 git_alert-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3900 1970-01-01 00:00:00.000000 git_alert-0.2.1/PKG-INFO
```

### Comparing `git_alert-0.2.0/LICENSE` & `git_alert-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.0/README.md` & `git_alert-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.0/git_alert/argument_parser.py` & `git_alert-0.2.1/git_alert/argument_parser.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.0/git_alert/repositories.py` & `git_alert-0.2.1/git_alert/repositories.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.0/git_alert/traverse.py` & `git_alert-0.2.1/git_alert/traverse.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.0/pyproject.toml` & `git_alert-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git_alert"
-version = "0.2.0"
+version = "0.2.1"
 description = "Checks a given path and its sub-directories for dirty git repositories."
 authors = ["Simon Antonius Lauer <simon.lauer@posteo.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "git_alert"}]
 
 [tool.poetry.dependencies]
```

### Comparing `git_alert-0.2.0/PKG-INFO` & `git_alert-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_alert
-Version: 0.2.0
+Version: 0.2.1
 Summary: Checks a given path and its sub-directories for dirty git repositories.
 License: MIT
 Author: Simon Antonius Lauer
 Author-email: simon.lauer@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

