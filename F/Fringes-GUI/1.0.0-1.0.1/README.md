# Comparing `tmp/fringes_gui-1.0.0.tar.gz` & `tmp/fringes_gui-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes_gui-1.0.0.tar", max compression
+gzip compressed data, was "fringes_gui-1.0.1.tar", max compression
```

## Comparing `fringes_gui-1.0.0.tar` & `fringes_gui-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      795 2024-04-20 16:22:10.414097 fringes_gui-1.0.0/fringes_gui/__init__.py
--rw-r--r--   0        0        0    16278 2024-04-20 16:26:29.615288 fringes_gui-1.0.0/fringes_gui/gui.py
--rw-r--r--   0        0        0    32094 2024-04-20 16:26:29.623157 fringes_gui-1.0.0/fringes_gui/logic.py
--rw-r--r--   0        0        0      129 2024-03-28 12:32:14.400050 fringes_gui-1.0.0/fringes_gui/main.py
--rw-r--r--   0        0        0     1607 2024-04-20 16:22:10.434257 fringes_gui-1.0.0/fringes_gui/numba-blue-icon-rgb.svg
--rw-r--r--   0        0        0    29338 2024-04-20 16:22:10.440709 fringes_gui-1.0.0/fringes_gui/params.py
--rw-r--r--   0        0        0      312 2024-04-20 16:22:10.447172 fringes_gui-1.0.0/fringes_gui/readme.txt
--rw-r--r--   0        0        0    33684 2024-04-20 16:22:10.453467 fringes_gui-1.0.0/fringes_gui/setters.py
--rw-r--r--   0        0        0     2832 2024-04-20 16:22:10.408001 fringes_gui-1.0.0/fringes_gui/Xi.svg
--rw-r--r--   0        0        0    21278 2024-04-20 16:22:10.396966 fringes_gui-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1241 2024-04-20 16:26:29.635685 fringes_gui-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2664 2024-04-20 16:26:29.608905 fringes_gui-1.0.0/README.md
--rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 fringes_gui-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      798 2024-04-20 19:18:26.035268 fringes_gui-1.0.1/fringes_gui/__init__.py
+-rw-r--r--   0        0        0    16278 2024-04-20 16:26:29.615288 fringes_gui-1.0.1/fringes_gui/gui.py
+-rw-r--r--   0        0        0    32094 2024-04-20 16:26:29.623157 fringes_gui-1.0.1/fringes_gui/logic.py
+-rw-r--r--   0        0        0      129 2024-03-28 12:32:14.400050 fringes_gui-1.0.1/fringes_gui/main.py
+-rw-r--r--   0        0        0     1607 2024-04-20 16:22:10.434257 fringes_gui-1.0.1/fringes_gui/numba-blue-icon-rgb.svg
+-rw-r--r--   0        0        0    29338 2024-04-20 16:22:10.440709 fringes_gui-1.0.1/fringes_gui/params.py
+-rw-r--r--   0        0        0      312 2024-04-20 16:22:10.447172 fringes_gui-1.0.1/fringes_gui/readme.txt
+-rw-r--r--   0        0        0    33684 2024-04-20 16:22:10.453467 fringes_gui-1.0.1/fringes_gui/setters.py
+-rw-r--r--   0        0        0     2832 2024-04-20 16:22:10.408001 fringes_gui-1.0.1/fringes_gui/Xi.svg
+-rw-r--r--   0        0        0    21278 2024-04-20 16:22:10.396966 fringes_gui-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1241 2024-04-20 19:21:02.129877 fringes_gui-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2664 2024-04-20 16:26:29.608905 fringes_gui-1.0.1/README.md
+-rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 fringes_gui-1.0.1/PKG-INFO
```

### Comparing `fringes_gui-1.0.0/fringes_gui/__init__.py` & `fringes_gui-1.0.1/fringes_gui/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 import os
-import importlib
-
 import toml
+import importlib
 
 from .gui import FringesGUI
 
 logger = logging.getLogger(__name__)
 
-# use verion string in pyproject.toml as the single source of truth
+# use version string in pyproject.toml as the single source of truth
 try:
     # in order not to confuse an installed version of a package with a local one,
     # first try the local one (not being installed)
     _meta = toml.load(os.path.join(os.path.dirname(__file__), "..", "pyproject.toml"))
     __version__ = _meta["project"]["version"]  # Python Packaging User Guide expects version here
 except KeyError:
     __version__ = _meta["tool"]["poetry"]["version"]  # Poetry expects version here
 except FileNotFoundError:
-    __version__ = importlib.metadata.version("fringes")  # installed version
+    __version__ = importlib.metadata.version("fringes-gui")  # installed version
 
 
 def run():
     gui = FringesGUI()
     gui.show()
```

### Comparing `fringes_gui-1.0.0/fringes_gui/gui.py` & `fringes_gui-1.0.1/fringes_gui/gui.py`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/fringes_gui/logic.py` & `fringes_gui-1.0.1/fringes_gui/logic.py`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/fringes_gui/numba-blue-icon-rgb.svg` & `fringes_gui-1.0.1/fringes_gui/numba-blue-icon-rgb.svg`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/fringes_gui/params.py` & `fringes_gui-1.0.1/fringes_gui/params.py`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/fringes_gui/setters.py` & `fringes_gui-1.0.1/fringes_gui/setters.py`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/fringes_gui/Xi.svg` & `fringes_gui-1.0.1/fringes_gui/Xi.svg`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/LICENSE.txt` & `fringes_gui-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/pyproject.toml` & `fringes_gui-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Fringes-GUI"
-version = "1.0.0"
+version = "1.0.1"
 description = "Graphical user interface for the 'fringes' package."
 license = "CC-BY-NC-SA-4.0"
 authors = ["Christian Kludt"]
 readme = "README.md"
 repository = "https://github.com/comimag/fringes-gui"
 documentation = "https://fringes.readthedocs.io/en/latest/getting_started/usage.html#graphical-user-interface"
 keywords = [
```

### Comparing `fringes_gui-1.0.0/README.md` & `fringes_gui-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fringes_gui-1.0.0/PKG-INFO` & `fringes_gui-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fringes-GUI
-Version: 1.0.0
+Version: 1.0.1
 Summary: Graphical user interface for the 'fringes' package.
 Home-page: https://github.com/comimag/fringes-gui
 License: CC-BY-NC-SA-4.0
 Keywords: phase shifting,phase unwrapping,fringe analysis,fringe projection,deflectometry,computational imaging
 Author: Christian Kludt
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Education
```

