# Comparing `tmp/jinja2_async_environment-0.7.2.tar.gz` & `tmp/jinja2_async_environment-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_async_environment-0.7.2.tar", last modified: Mon Apr 15 14:10:09 2024, max compression
+gzip compressed data, was "jinja2_async_environment-0.7.3.tar", last modified: Sun Apr 28 09:03:41 2024, max compression
```

## Comparing `jinja2_async_environment-0.7.2.tar` & `jinja2_async_environment-0.7.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.7.2/LICENSE
--rw-r--r--   0        0        0      256 2023-08-18 15:51:25.740188 jinja2_async_environment-0.7.2/README.md
--rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.7.2/jinja2_async_environment/__init__.py
--rw-r--r--   0        0        0     1419 2024-03-03 12:44:33.505857 jinja2_async_environment-0.7.2/jinja2_async_environment/bccache.py
--rw-r--r--   0        0        0     4669 2024-03-03 08:37:52.586610 jinja2_async_environment-0.7.2/jinja2_async_environment/compiler.py
--rw-r--r--   0        0        0     3524 2024-03-03 13:52:16.395020 jinja2_async_environment-0.7.2/jinja2_async_environment/environment.py
--rw-r--r--   0        0        0     8520 2024-03-03 12:44:33.500636 jinja2_async_environment-0.7.2/jinja2_async_environment/loaders.py
--rw-r--r--   0        0        0     2095 2024-04-15 14:10:09.522522 jinja2_async_environment-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 jinja2_async_environment-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.7.3/LICENSE
+-rw-r--r--   0        0        0      256 2023-08-18 15:51:25.740188 jinja2_async_environment-0.7.3/README.md
+-rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.7.3/jinja2_async_environment/__init__.py
+-rw-r--r--   0        0        0     1419 2024-03-03 12:44:33.505857 jinja2_async_environment-0.7.3/jinja2_async_environment/bccache.py
+-rw-r--r--   0        0        0     4669 2024-03-03 08:37:52.586610 jinja2_async_environment-0.7.3/jinja2_async_environment/compiler.py
+-rw-r--r--   0        0        0     3524 2024-03-03 13:52:16.395020 jinja2_async_environment-0.7.3/jinja2_async_environment/environment.py
+-rw-r--r--   0        0        0     8520 2024-03-03 12:44:33.500636 jinja2_async_environment-0.7.3/jinja2_async_environment/loaders.py
+-rw-r--r--   0        0        0     2095 2024-04-28 09:03:41.651213 jinja2_async_environment-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 jinja2_async_environment-0.7.3/PKG-INFO
```

### Comparing `jinja2_async_environment-0.7.2/LICENSE` & `jinja2_async_environment-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.2/jinja2_async_environment/bccache.py` & `jinja2_async_environment-0.7.3/jinja2_async_environment/bccache.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.2/jinja2_async_environment/compiler.py` & `jinja2_async_environment-0.7.3/jinja2_async_environment/compiler.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.2/jinja2_async_environment/environment.py` & `jinja2_async_environment-0.7.3/jinja2_async_environment/environment.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.2/jinja2_async_environment/loaders.py` & `jinja2_async_environment-0.7.3/jinja2_async_environment/loaders.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.2/pyproject.toml` & `jinja2_async_environment-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,33 +37,33 @@
 
 [tool.creosote]
 paths = [
     "jinja2_async_environment",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
+    "pytest",
     "pdm",
-    "pdm-bump",
-    "pre-commit",
     "autotyping",
-    "pytest",
+    "pre-commit",
+    "pdm-bump",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "jinja2_async_environment",
 ]
 skips = [
-    "B603",
     "B404",
-    "B403",
     "B113",
+    "B603",
+    "B403",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "jinja2_async_environment",
 ]
@@ -84,15 +84,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "jinja2-async-environment"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 dependencies = [
     "jinja2>=3.1.2",
     "redis!=5.0.1,>=5.0.0",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
```

### Comparing `jinja2_async_environment-0.7.2/PKG-INFO` & `jinja2_async_environment-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-async-environment
-Version: 0.7.2
+Version: 0.7.3
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

