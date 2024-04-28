# Comparing `tmp/plugget-qt-0.0.5.tar.gz` & `tmp/plugget_qt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget-qt-0.0.5.tar", last modified: Sun Dec 17 19:45:59 2023, max compression
+gzip compressed data, was "plugget_qt-0.0.6.tar", last modified: Sun Apr 28 10:10:46 2024, max compression
```

## Comparing `plugget-qt-0.0.5.tar` & `plugget_qt-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:45:59.295305 plugget-qt-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:45:59.291305 plugget-qt-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:45:59.295305 plugget-qt-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-17 19:45:49.000000 plugget-qt-0.0.5/.github/workflows/PyPI-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-17 19:45:49.000000 plugget-qt-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-12-17 19:45:59.295305 plugget-qt-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-12-17 19:45:49.000000 plugget-qt-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:45:59.295305 plugget-qt-0.0.5/plugget_qt/
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2023-12-17 19:45:49.000000 plugget-qt-0.0.5/plugget_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:45:59.295305 plugget-qt-0.0.5/plugget_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-12-17 19:45:59.000000 plugget-qt-0.0.5/plugget_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-17 19:45:59.000000 plugget-qt-0.0.5/plugget_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 19:45:59.000000 plugget-qt-0.0.5/plugget_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-17 19:45:59.000000 plugget-qt-0.0.5/plugget_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-17 19:45:59.000000 plugget-qt-0.0.5/plugget_qt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-17 19:45:49.000000 plugget-qt-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-17 19:45:49.000000 plugget-qt-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 19:45:59.295305 plugget-qt-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.690345 plugget_qt-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.690345 plugget_qt-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/.github/workflows/PyPI-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.690345 plugget_qt-0.0.6/plugget_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/plugget_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/plugget_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/sample_config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/setup.cfg
```

### Comparing `plugget-qt-0.0.5/.github/workflows/PyPI-publish.yml` & `plugget_qt-0.0.6/.github/workflows/PyPI-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget-qt-0.0.5/.gitignore` & `plugget_qt-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget-qt-0.0.5/PKG-INFO` & `plugget_qt-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: plugget-qt
-Version: 0.0.5
+Version: 0.0.6
 Summary: a qt widget to search for plugget packages
 Author: Hannes Delbeke
 Project-URL: Homepage, https://github.com/plugget/plugget-qt
 Project-URL: Documentation, https://github.com/plugget/plugget-qt
 Keywords: dcc,pipeline,qt,widget,plugget,package,manifest,search,installer
 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version < "3.4"
 Requires-Dist: plugget
-Requires-Dist: qtpy
 
 # Plugget Qt [![PyPI](https://img.shields.io/pypi/v/plugget-qt)](https://pypi.org/project/plugget-qt/)
 
 Plugget Qt is a UI for [plugget](https://github.com/plugget/plugget).  
 Easily search, list & (un)install [plugget packages](https://github.com/plugget/plugget-pkgs).  
 
 Plugget qt is used by:  
 <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="32" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
 <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="32" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
+- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin) A Maya plugin that launches the Plugget Qt UI window
+- [plugget qt substance painter](https://github.com/plugget/plugget-substance-painter-plugin)
+
 
 ## Instructions
 To show the qt window:
 ```python
 import plugget_qt
 w = plugget_qt.show()  # store reference in w, to prevent garbage collection
 ``` 
@@ -35,15 +39,15 @@
 ### Installation
 (depending on the app, you might want to replace python for the app's python interpreter, and maybe also use `--target "install/path/to/folder" --no-user` to install your python package to a custom folder)
 ```
 python -m pip install plugget-qt
 ```
 
 ### Dependencies
-- `plugget` Python module.
-- `qtpy` Qt wrapper for PySide & PyQt
+- [plugget](https://github.com/plugget/plugget) (Apache 2.0) Python module.
+- [qtpy](https://pypi.org/project/QtPy/) (MIT) Qt wrapper for PySide & PyQt
 
 
 
 
 If this tool is helpfull, you can ⭐ star it on the github page,
 just click the ⭐ star button in the top-right of this page.
```

### Comparing `plugget-qt-0.0.5/README.md` & `plugget_qt-0.0.6/plugget_qt.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,34 @@
+Metadata-Version: 2.1
+Name: plugget-qt
+Version: 0.0.6
+Summary: a qt widget to search for plugget packages
+Author: Hannes Delbeke
+Project-URL: Homepage, https://github.com/plugget/plugget-qt
+Project-URL: Documentation, https://github.com/plugget/plugget-qt
+Keywords: dcc,pipeline,qt,widget,plugget,package,manifest,search,installer
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib-metadata; python_version < "3.4"
+Requires-Dist: plugget
+
 # Plugget Qt [![PyPI](https://img.shields.io/pypi/v/plugget-qt)](https://pypi.org/project/plugget-qt/)
 
 Plugget Qt is a UI for [plugget](https://github.com/plugget/plugget).  
 Easily search, list & (un)install [plugget packages](https://github.com/plugget/plugget-pkgs).  
 
 Plugget qt is used by:  
 <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="32" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
 <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="32" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
+- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin) A Maya plugin that launches the Plugget Qt UI window
+- [plugget qt substance painter](https://github.com/plugget/plugget-substance-painter-plugin)
+
 
 ## Instructions
 To show the qt window:
 ```python
 import plugget_qt
 w = plugget_qt.show()  # store reference in w, to prevent garbage collection
 ``` 
@@ -20,15 +39,15 @@
 ### Installation
 (depending on the app, you might want to replace python for the app's python interpreter, and maybe also use `--target "install/path/to/folder" --no-user` to install your python package to a custom folder)
 ```
 python -m pip install plugget-qt
 ```
 
 ### Dependencies
-- `plugget` Python module.
-- `qtpy` Qt wrapper for PySide & PyQt
+- [plugget](https://github.com/plugget/plugget) (Apache 2.0) Python module.
+- [qtpy](https://pypi.org/project/QtPy/) (MIT) Qt wrapper for PySide & PyQt
 
 
 
 
 If this tool is helpfull, you can ⭐ star it on the github page,
 just click the ⭐ star button in the top-right of this page.
```

### Comparing `plugget-qt-0.0.5/pyproject.toml` & `plugget_qt-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 description = "a qt widget to search for plugget packages"
 readme = "README.md"
 requires-python = ">=3.4"
 keywords = ["dcc", "pipeline", "qt", "widget", "plugget", "package", "manifest", "search", "installer"]
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.4",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     'importlib-metadata; python_version<"3.4"',
     'plugget',
-    'qtpy',
 ]
 
 # dynamic = ["version"]
-version = "0.0.5"
+version = "0.0.6"
 
 # [project.optional-dependencies]
 # pyside2 = ["PySide2"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

