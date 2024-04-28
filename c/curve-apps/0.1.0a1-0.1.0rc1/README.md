# Comparing `tmp/curve_apps-0.1.0a1.tar.gz` & `tmp/curve_apps-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curve_apps-0.1.0a1.tar", max compression
+gzip compressed data, was "curve_apps-0.1.0rc1.tar", max compression
```

## Comparing `curve_apps-0.1.0a1.tar` & `curve_apps-0.1.0rc1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      567 2024-04-17 17:14:59.471051 curve_apps-0.1.0a1/curve_apps/__init__.py
--rw-r--r--   0        0        0     3120 2024-04-17 17:14:59.471051 curve_apps-0.1.0a1/curve_apps/driver.py
--rw-r--r--   0        0        0      120 2024-04-17 17:14:59.471051 curve_apps-0.1.0a1/curve_apps/edge_detection/__init__.py
--rw-r--r--   0        0        0     6983 2024-04-17 17:14:59.471051 curve_apps-0.1.0a1/curve_apps/edge_detection/driver.py
--rw-r--r--   0        0        0     2433 2024-04-17 17:14:59.481144 curve_apps-0.1.0a1/curve_apps/edge_detection/params.py
--rw-r--r--   0        0        0      712 2024-04-17 17:14:59.481349 curve_apps-0.1.0a1/curve_apps/params.py
--rw-r--r--   0        0        0      120 2024-04-17 17:14:59.481349 curve_apps-0.1.0a1/curve_apps/trend_lines/__init__.py
--rw-r--r--   0        0        0     5509 2024-04-17 17:14:59.481349 curve_apps-0.1.0a1/curve_apps/trend_lines/driver.py
--rw-r--r--   0        0        0     1961 2024-04-17 17:14:59.481349 curve_apps-0.1.0a1/curve_apps/trend_lines/params.py
--rw-r--r--   0        0        0      120 2024-04-17 17:14:57.913738 curve_apps-0.1.0a1/curve_apps-assets/__init__.py
--rw-r--r--   0        0        0  4876334 2024-04-17 17:15:01.615042 curve_apps-0.1.0a1/curve_apps-assets/curve_apps_demo.geoh5
--rw-r--r--   0        0        0     3045 2024-04-17 17:14:59.471051 curve_apps-0.1.0a1/curve_apps-assets/uijson/edge_detection.ui.json
--rw-r--r--   0        0        0     2999 2024-04-17 17:14:59.471051 curve_apps-0.1.0a1/curve_apps-assets/uijson/trend_lines.ui.json
--rw-r--r--   0        0        0     3307 2024-04-17 19:15:15.250973 curve_apps-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     5944 2024-04-17 17:14:57.913738 curve_apps-0.1.0a1/README.rst
--rw-r--r--   0        0        0     7179 1970-01-01 00:00:00.000000 curve_apps-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      564 2024-04-28 03:43:27.707525 curve_apps-0.1.0rc1/curve_apps/__init__.py
+-rw-r--r--   0        0        0     3120 2024-04-23 21:07:08.257218 curve_apps-0.1.0rc1/curve_apps/driver.py
+-rw-r--r--   0        0        0      120 2024-04-23 21:07:08.257218 curve_apps-0.1.0rc1/curve_apps/edge_detection/__init__.py
+-rw-r--r--   0        0        0     6983 2024-04-23 21:07:08.258300 curve_apps-0.1.0rc1/curve_apps/edge_detection/driver.py
+-rw-r--r--   0        0        0     2433 2024-04-23 21:07:08.258361 curve_apps-0.1.0rc1/curve_apps/edge_detection/params.py
+-rw-r--r--   0        0        0      712 2024-04-23 21:07:08.258361 curve_apps-0.1.0rc1/curve_apps/params.py
+-rw-r--r--   0        0        0      120 2024-04-23 21:07:08.258897 curve_apps-0.1.0rc1/curve_apps/trend_lines/__init__.py
+-rw-r--r--   0        0        0     5509 2024-04-23 21:07:08.259478 curve_apps-0.1.0rc1/curve_apps/trend_lines/driver.py
+-rw-r--r--   0        0        0     1961 2024-04-23 21:07:08.259478 curve_apps-0.1.0rc1/curve_apps/trend_lines/params.py
+-rw-r--r--   0        0        0      120 2024-04-27 20:32:11.993663 curve_apps-0.1.0rc1/curve_apps-assets/__init__.py
+-rw-r--r--   0        0        0  4876334 2024-04-23 21:07:09.232019 curve_apps-0.1.0rc1/curve_apps-assets/curve_apps_demo.geoh5
+-rw-r--r--   0        0        0     3045 2024-04-23 21:07:08.256066 curve_apps-0.1.0rc1/curve_apps-assets/uijson/edge_detection.ui.json
+-rw-r--r--   0        0        0     2999 2024-04-23 21:07:08.256066 curve_apps-0.1.0rc1/curve_apps-assets/uijson/trend_lines.ui.json
+-rw-r--r--   0        0        0     1098 2024-04-23 21:07:36.644208 curve_apps-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     3868 2024-04-28 03:44:23.797495 curve_apps-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5944 2024-04-23 21:07:07.585841 curve_apps-0.1.0rc1/README.rst
+-rw-r--r--   0        0        0     7216 1970-01-01 00:00:00.000000 curve_apps-0.1.0rc1/PKG-INFO
```

### Comparing `curve_apps-0.1.0a1/curve_apps/__init__.py` & `curve_apps-0.1.0rc1/curve_apps/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #  All rights reserved.
 
 from __future__ import annotations
 
 from pathlib import Path
 
-__version__ = "0.1.0-alpha.1"
+__version__ = "0.1.0-rc.1"
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
 
     parent = Path(__file__).parent
     folder_name = f"{parent.name}-assets"
```

### Comparing `curve_apps-0.1.0a1/curve_apps/driver.py` & `curve_apps-0.1.0rc1/curve_apps/driver.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps/edge_detection/driver.py` & `curve_apps-0.1.0rc1/curve_apps/edge_detection/driver.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps/edge_detection/params.py` & `curve_apps-0.1.0rc1/curve_apps/edge_detection/params.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps/params.py` & `curve_apps-0.1.0rc1/curve_apps/params.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps/trend_lines/driver.py` & `curve_apps-0.1.0rc1/curve_apps/trend_lines/driver.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps/trend_lines/params.py` & `curve_apps-0.1.0rc1/curve_apps/trend_lines/params.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps-assets/curve_apps_demo.geoh5` & `curve_apps-0.1.0rc1/curve_apps-assets/curve_apps_demo.geoh5`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps-assets/uijson/edge_detection.ui.json` & `curve_apps-0.1.0rc1/curve_apps-assets/uijson/edge_detection.ui.json`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/curve_apps-assets/uijson/trend_lines.ui.json` & `curve_apps-0.1.0rc1/curve_apps-assets/uijson/trend_lines.ui.json`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/pyproject.toml` & `curve_apps-0.1.0rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 [tool.poetry]
-name = "curve_apps"
-version = "0.1.0-alpha.1"
+name = "curve-apps"
+version = "0.1.0-rc.1"
 license = "MIT"
 description = "Find edges on 2D grids or vertices."
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/curve_apps"
 homepage = "https://mirageoscience.com"
 readme = "README.rst"
 packages = [
      { include = "curve_apps" },
      { include = "curve_apps-assets" },
 ]
 
+include = [
+    "COPYING",
+    "COPYING.LESSER",
+    "LICENSE",
+    "README.rst",
+    "THIRD_PARTY_SOFTWARE.rst",
+]
+
 # TODO: adjust classifiers
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
@@ -26,40 +34,47 @@
     "Operating System :: MacOS",
     "Natural Language :: English",
 ]
 
 [tool.poetry.scripts]
 
 [tool.poetry.dependencies]
-pydantic = {version = "~2.5"}
 python = "^3.9, <3.11"
-numpy = "~1.23.5"  # also geoh5py
+
+numpy = "~1.23.5"  # also in geoh5py
+pydantic = "~2.5.2"
+scikit-image = "~0.20.0"
 scipy = "~1.10.1"
-scikit-image = "~0.19.0"
-tqdm = "~4.66.0"
+tqdm = "~4.66.1"
 
-## pip dependencies
-geoh5py = {version = "~0.9.0-alpha.3", source = "pypi", allow-prereleases = true}
-geoapps-utils = {version = "~0.3.0a2", source = "pypi", allow-prereleases = true}
-#geoapps-utils = { url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/GEOPY-1348.zip#sha256=" }
+## pip dependencies from Git repositories
+#----------------------------------------
+geoh5py = {version = "~0.9.0rc1", source = "pypi", allow-prereleases = true}
+#geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
+#geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
+
+geoapps-utils = {version = "~0.3.0rc1", source = "pypi", allow-prereleases = true}
+#geoapps-utils = {url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.3.0.zip#sha256="}
+#geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
-h5py = "*" # from geoh5py
-Pillow = "*" # from geoh5py
+#---------------------------------------------------------------------------------
+h5py = "^3.2.1"  # from geoh5py
+Pillow = "~10.1.0"  # from geoh5py
 
 ## about pip dependencies
 # to be specified to work with conda-lock
 # - from PyPI: my_package = { version = "1.2.3", source = "pypi" }
 # - from URL:
 #   - for a tags:   my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/tags/VERSION_TAG.zip#sha256=" }
 #   - for a branch: my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/heads/BRANCH.zip#sha256=" }
 # Note - conda-lock does not support the syntax: my_package = { git = ... }
 #        while poetry2conda supports only { git = "...", tag = "..." }, and not { url = ... }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 Pygments = "*"
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 sphinx = "*"
 sphinx-autodoc-typehints = "*"
 sphinx-rtd-theme = "*"
@@ -85,15 +100,16 @@
 ignore_missing_imports = true
 scripts_are_modules = true
 show_error_context = true
 show_column_numbers = true
 check_untyped_defs = true
 
 plugins = [
-    "numpy.typing.mypy_plugin"
+    "numpy.typing.mypy_plugin",
+    "pydantic.mypy"
 ]
 
 [tool.pytest.ini_options]
 
 [tool.coverage.run]
 branch = true
 source = ["curve_apps"]
```

### Comparing `curve_apps-0.1.0a1/README.rst` & `curve_apps-0.1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0a1/PKG-INFO` & `curve_apps-0.1.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: curve_apps
-Version: 0.1.0a1
+Name: curve-apps
+Version: 0.1.0rc1
 Summary: Find edges on 2D grids or vertices.
 Home-page: https://mirageoscience.com
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
@@ -18,23 +18,23 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: Pillow
-Requires-Dist: geoapps-utils (>=0.3.0a2,<0.4.0)
-Requires-Dist: geoh5py (>=0.9.0-alpha.3,<0.10.0)
-Requires-Dist: h5py
+Requires-Dist: Pillow (>=10.1.0,<10.2.0)
+Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
+Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
+Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Requires-Dist: pydantic (>=2.5,<2.6)
-Requires-Dist: scikit-image (>=0.19.0,<0.20.0)
+Requires-Dist: pydantic (>=2.5.2,<2.6.0)
+Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
-Requires-Dist: tqdm (>=4.66.0,<4.67.0)
+Requires-Dist: tqdm (>=4.66.1,<4.67.0)
 Project-URL: Repository, https://github.com/MiraGeoscience/curve_apps
 Description-Content-Type: text/x-rst
 
 |coverage| |maintainability| |precommit_ci| |docs| |style| |version| |status| |pyversions|
 
 
 .. |docs| image:: https://readthedocs.org/projects/curve-apps/badge/
```

