# Comparing `tmp/mira_omf-3.2.0a1.tar.gz` & `tmp/mira_omf-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mira_omf-3.2.0a1.tar", max compression
+gzip compressed data, was "mira_omf-3.2.0rc1.tar", max compression
```

## Comparing `mira_omf-3.2.0a1.tar` & `mira_omf-3.2.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1122 2023-10-10 18:38:14.946657 mira_omf-3.2.0a1/LICENSE
--rw-r--r--   0        0        0     1687 2024-04-23 17:10:17.046332 mira_omf-3.2.0a1/omf/__init__.py
--rw-r--r--   0        0        0     6754 2023-10-10 18:38:16.651487 mira_omf-3.2.0a1/omf/base.py
--rw-r--r--   0        0        0     8561 2023-10-10 18:38:16.652017 mira_omf-3.2.0a1/omf/data.py
--rw-r--r--   0        0        0      111 2023-10-10 18:38:16.652566 mira_omf-3.2.0a1/omf/fileio/__init__.py
--rw-r--r--   0        0        0     6049 2024-01-10 23:48:56.546364 mira_omf-3.2.0a1/omf/fileio/fileio.py
--rw-r--r--   0        0        0    43690 2024-01-10 23:48:56.547396 mira_omf-3.2.0a1/omf/fileio/geoh5.py
--rw-r--r--   0        0        0     1123 2023-10-10 18:38:16.653603 mira_omf-3.2.0a1/omf/fileio/utils.py
--rw-r--r--   0        0        0     1760 2023-10-10 18:38:16.653603 mira_omf-3.2.0a1/omf/lineset.py
--rw-r--r--   0        0        0     1411 2023-10-10 18:38:16.654144 mira_omf-3.2.0a1/omf/pointset.py
--rw-r--r--   0        0        0        0 2023-10-10 18:38:16.654677 mira_omf-3.2.0a1/omf/scripts/__init__.py
--rw-r--r--   0        0        0     1221 2024-04-23 17:10:17.046332 mira_omf-3.2.0a1/omf/scripts/geoh5_to_omf.py
--rw-r--r--   0        0        0     1729 2024-04-23 17:10:17.046332 mira_omf-3.2.0a1/omf/scripts/omf_to_geoh5.py
--rw-r--r--   0        0        0     3682 2023-10-10 18:38:16.655224 mira_omf-3.2.0a1/omf/serializers.py
--rw-r--r--   0        0        0     3736 2023-10-10 18:38:16.655732 mira_omf-3.2.0a1/omf/surface.py
--rw-r--r--   0        0        0      675 2023-10-10 18:38:16.656264 mira_omf-3.2.0a1/omf/texture.py
--rw-r--r--   0        0        0     2409 2023-10-10 18:38:16.656814 mira_omf-3.2.0a1/omf/volume.py
--rw-r--r--   0        0        0     1854 2024-04-23 17:11:09.514140 mira_omf-3.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     2789 2024-04-23 17:11:09.514140 mira_omf-3.2.0a1/README.rst
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 mira_omf-3.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1122 2024-04-23 21:18:33.429696 mira_omf-3.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     1684 2024-04-27 21:37:48.543607 mira_omf-3.2.0rc1/omf/__init__.py
+-rw-r--r--   0        0        0     6754 2024-04-23 21:18:33.550153 mira_omf-3.2.0rc1/omf/base.py
+-rw-r--r--   0        0        0     8561 2024-04-23 21:18:33.550153 mira_omf-3.2.0rc1/omf/data.py
+-rw-r--r--   0        0        0      111 2024-04-23 21:18:33.551152 mira_omf-3.2.0rc1/omf/fileio/__init__.py
+-rw-r--r--   0        0        0     6049 2024-04-23 21:18:33.551152 mira_omf-3.2.0rc1/omf/fileio/fileio.py
+-rw-r--r--   0        0        0    43690 2024-04-23 21:18:33.552162 mira_omf-3.2.0rc1/omf/fileio/geoh5.py
+-rw-r--r--   0        0        0     1123 2024-04-23 21:18:33.552162 mira_omf-3.2.0rc1/omf/fileio/utils.py
+-rw-r--r--   0        0        0     1760 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc1/omf/lineset.py
+-rw-r--r--   0        0        0     1411 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc1/omf/pointset.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc1/omf/scripts/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc1/omf/scripts/geoh5_to_omf.py
+-rw-r--r--   0        0        0     1729 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc1/omf/scripts/omf_to_geoh5.py
+-rw-r--r--   0        0        0     3682 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc1/omf/serializers.py
+-rw-r--r--   0        0        0     3736 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc1/omf/surface.py
+-rw-r--r--   0        0        0      675 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc1/omf/texture.py
+-rw-r--r--   0        0        0     2409 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc1/omf/volume.py
+-rw-r--r--   0        0        0     2255 2024-04-27 21:37:54.011682 mira_omf-3.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2467 2024-04-27 21:36:29.725597 mira_omf-3.2.0rc1/README.rst
+-rw-r--r--   0        0        0     3673 1970-01-01 00:00:00.000000 mira_omf-3.2.0rc1/PKG-INFO
```

### Comparing `mira_omf-3.2.0a1/LICENSE` & `mira_omf-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/__init__.py` & `mira_omf-3.2.0rc1/omf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .fileio import GeoH5Writer, OMFReader, OMFWriter
 from .lineset import LineSetElement, LineSetGeometry
 from .pointset import PointSetElement, PointSetGeometry
 from .surface import SurfaceElement, SurfaceGeometry, SurfaceGridGeometry
 from .texture import ImageTexture
 from .volume import VolumeElement, VolumeGridGeometry
 
-__version__ = "3.2.0-alpha.1"
+__version__ = "3.2.0-rc.1"
 __author__ = "Global Mining Standards and Guidelines Group"
 __license__ = "MIT License"
 __copyright__ = "Copyright 2017 Global Mining Standards and Guidelines Group"
 
 
 def _create_logger():
     error_handler = logging.StreamHandler(sys.stderr)
```

### Comparing `mira_omf-3.2.0a1/omf/base.py` & `mira_omf-3.2.0rc1/omf/base.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/data.py` & `mira_omf-3.2.0rc1/omf/data.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/fileio/fileio.py` & `mira_omf-3.2.0rc1/omf/fileio/fileio.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/fileio/geoh5.py` & `mira_omf-3.2.0rc1/omf/fileio/geoh5.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/fileio/utils.py` & `mira_omf-3.2.0rc1/omf/fileio/utils.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/lineset.py` & `mira_omf-3.2.0rc1/omf/lineset.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/pointset.py` & `mira_omf-3.2.0rc1/omf/pointset.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/scripts/geoh5_to_omf.py` & `mira_omf-3.2.0rc1/omf/scripts/geoh5_to_omf.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/scripts/omf_to_geoh5.py` & `mira_omf-3.2.0rc1/omf/scripts/omf_to_geoh5.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/serializers.py` & `mira_omf-3.2.0rc1/omf/serializers.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/surface.py` & `mira_omf-3.2.0rc1/omf/surface.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/texture.py` & `mira_omf-3.2.0rc1/omf/texture.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/omf/volume.py` & `mira_omf-3.2.0rc1/omf/volume.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0a1/pyproject.toml` & `mira_omf-3.2.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mira-omf"
-version = "3.2.0-alpha.1"
+version = "3.2.0-rc.1"
 description = "API Library for Open Mining Format"
 authors = [
     "Mira Geoscience <dominiquef@mirageoscience.com>",
     "Global Mining Standards and Guidelines Group <it@seequent.com>",
 ]
 repository = "https://github.com/MiraGeoscience/omf"
 homepage = "http://www.globalminingstandards.org/"
@@ -23,29 +23,44 @@
     'Natural Language :: English',
 ]
 
 packages = [
     { include = "omf" },
 ]
 
+include = [
+    "COPYING",
+    "COPYING.LESSER",
+    "LICENSE",
+    "README.rst",
+    "THIRD_PARTY_SOFTWARE.rst",
+]
+
 [tool.poetry.scripts]
 geoh5_to_omf = 'omf.scripts.geoh5_to_omf:main'
 omf_to_geoh5 = 'omf.scripts.omf_to_geoh5:main'
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
-geoh5py = {version = "~0.9.0-alpha.4", allow-prereleases = true}
-#geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
-numpy = "~1.23.5"
+
+numpy = "~1.23.5"  # also in geoh5py
 properties = "~0.6.0"
 pypng = "^0.20220715"
 six = "^1.16"
 vectormath = "~0.2.0"
 
-[tool.poetry.dev-dependencies]
+## dependencies from Git repositories
+#------------------------------------
+geoh5py = {version = "~0.9.0rc1", allow-prereleases = true}
+#geoh5py = {git = "https://github.com/MiraGeoscience/geoh5py.git", branch = "release/0.9.0"}
+#geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
+#geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
+
+[tool.poetry.group.dev.dependencies]
+Pygments = "*"
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 sphinx = "^5.3"
 tomli = "*"  # for tests only
 
 [tool.isort]
```

### Comparing `mira_omf-3.2.0a1/README.rst` & `mira_omf-3.2.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,21 @@
     :alt: MIT license
 
 .. image:: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml/badge.svg
     :target: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml
     :alt: pytest
 
 
-Version: 3.2.0-alpha.1
+Version: 3.2.0
 
 API library for Open Mining Format, a new standard for mining data backed by
 the `Global Mining Standards & Guidelines Group <https://gmggroup.org/>`_.
 
-.. warning::
-    **Pre-Release Notice**
-
-    This is a Beta release of the Open Mining Format (OMF) and the associated
-    Python API. The storage format and libraries might be changed in
-    backward-incompatible ways and are not subject to any SLA or deprecation
-    policy.
 
 .. warning::
-    **Alpha-Release Notice**
 
     This is a fork created by Mira Geoscience for interoperability with the
     geoh5 file format.
 
 Why?
 ----
```

### Comparing `mira_omf-3.2.0a1/PKG-INFO` & `mira_omf-3.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mira-omf
-Version: 3.2.0a1
+Version: 3.2.0rc1
 Summary: API Library for Open Mining Format
 Home-page: http://www.globalminingstandards.org/
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
 Author-email: dominiquef@mirageoscience.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: geoh5py (>=0.9.0-alpha.4,<0.10.0)
+Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: properties (>=0.6.0,<0.7.0)
 Requires-Dist: pypng (>=0.20220715,<0.20220716)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: vectormath (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/MiraGeoscience/omf
 Description-Content-Type: text/x-rst
@@ -46,29 +46,21 @@
     :alt: MIT license
 
 .. image:: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml/badge.svg
     :target: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml
     :alt: pytest
 
 
-Version: 3.2.0-alpha.1
+Version: 3.2.0
 
 API library for Open Mining Format, a new standard for mining data backed by
 the `Global Mining Standards & Guidelines Group <https://gmggroup.org/>`_.
 
-.. warning::
-    **Pre-Release Notice**
-
-    This is a Beta release of the Open Mining Format (OMF) and the associated
-    Python API. The storage format and libraries might be changed in
-    backward-incompatible ways and are not subject to any SLA or deprecation
-    policy.
 
 .. warning::
-    **Alpha-Release Notice**
 
     This is a fork created by Mira Geoscience for interoperability with the
     geoh5 file format.
 
 Why?
 ----
```

