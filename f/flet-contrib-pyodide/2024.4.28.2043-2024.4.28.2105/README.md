# Comparing `tmp/flet_contrib_pyodide-2024.4.28.2043.tar.gz` & `tmp/flet_contrib_pyodide-2024.4.28.2105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_pyodide-2024.4.28.2043.tar", max compression
+gzip compressed data, was "flet_contrib_pyodide-2024.4.28.2105.tar", max compression
```

## Comparing `flet_contrib_pyodide-2024.4.28.2043.tar` & `flet_contrib_pyodide-2024.4.28.2105.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/README.md
--rw-r--r--   0        0        0      664 2024-04-28 20:43:17.485388 flet_contrib_pyodide-2024.4.28.2043/pyproject.toml
--rw-r--r--   0        0        0      193 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/flet.py
--rw-r--r--   0        0        0       55 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3581 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2024-04-28 20:42:33.189003 flet_contrib_pyodide-2024.4.28.2043/src/flet/version.py
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 flet_contrib_pyodide-2024.4.28.2043/PKG-INFO
+-rw-r--r--   0        0        0     2264 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/README.md
+-rw-r--r--   0        0        0      664 2024-04-28 21:05:47.818920 flet_contrib_pyodide-2024.4.28.2105/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3581 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2024-04-28 21:05:01.134652 flet_contrib_pyodide-2024.4.28.2105/src/flet/version.py
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 flet_contrib_pyodide-2024.4.28.2105/PKG-INFO
```

### Comparing `flet_contrib_pyodide-2024.4.28.2043/README.md` & `flet_contrib_pyodide-2024.4.28.2105/README.md`

 * *Files identical despite different names*

### Comparing `flet_contrib_pyodide-2024.4.28.2043/pyproject.toml` & `flet_contrib_pyodide-2024.4.28.2105/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-pyodide"
-version = "2024.04.28.2043"
+version = "2024.04.28.2105"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-flet-contrib-core = "2024.04.28.2043"
+flet-contrib-core = "2024.04.28.2105"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `flet_contrib_pyodide-2024.4.28.2043/src/flet/flet.py` & `flet_contrib_pyodide-2024.4.28.2105/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_pyodide-2024.4.28.2043/src/flet/pyodide_connection.py` & `flet_contrib_pyodide-2024.4.28.2105/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_pyodide-2024.4.28.2043/PKG-INFO` & `flet_contrib_pyodide-2024.4.28.2105/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: flet-contrib-pyodide
-Version: 2024.4.28.2043
+Version: 2024.4.28.2105
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: flet-contrib-core (==2024.04.28.2043)
+Requires-Dist: flet-contrib-core (==2024.04.28.2105)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

