# Comparing `tmp/thonny_tunisiaschools-0.0.8.tar.gz` & `tmp/thonny_tunisiaschools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny_tunisiaschools-0.0.8.tar", last modified: Sun Apr 28 12:36:15 2024, max compression
+gzip compressed data, was "thonny_tunisiaschools-0.0.9.tar", last modified: Sun Apr 28 20:15:38 2024, max compression
```

## Comparing `thonny_tunisiaschools-0.0.8.tar` & `thonny_tunisiaschools-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.925639 thonny_tunisiaschools-0.0.8/thonnycontrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.925639 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/UIViewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.925639 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/designer_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/qt_16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/qt_32.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:38.748877 thonny_tunisiaschools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-28 20:15:38.748877 thonny_tunisiaschools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-28 20:15:38.748877 thonny_tunisiaschools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:38.748877 thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-28 20:15:38.000000 thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-28 20:15:38.000000 thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:15:38.000000 thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 20:15:38.000000 thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-28 20:15:38.000000 thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:38.744877 thonny_tunisiaschools-0.0.9/thonnycontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:38.748877 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/UIViewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:38.748877 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/res/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/res/designer_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/res/qt_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-28 20:15:31.000000 thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/res/qt_32.png
```

### Comparing `thonny_tunisiaschools-0.0.8/PKG-INFO` & `thonny_tunisiaschools-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-tunisiaschools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Thonny IDE plug-in that offers PyQt / QT / Python support for Tunisian computer science secondary teachers / students .
 Home-page: https://github.com/selmen2004/thonny-tunisiaschools
 Author: Selmen Arous
 Author-email: Selmen Arous <selmen.arous@gmail.com>
 License: GPL version 3
 Keywords: PyQt,QT,Tunisia,School,Teaching,Education
 Platform: Windows
```

### Comparing `thonny_tunisiaschools-0.0.8/README.md` & `thonny_tunisiaschools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.8/pyproject.toml` & `thonny_tunisiaschools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "thonny-tunisiaschools"
-version = "0.0.8"
+version = "0.0.9"
 description="A Thonny IDE plug-in that offers PyQt / QT / Python support for Tunisian computer science secondary teachers / students ."
 readme = "README.md"
 requires-python = ">=3.0"
 dependencies = [
   'thonny>=3.2.1',
 ]
 license ={text = "GPL version 3"}
```

### Comparing `thonny_tunisiaschools-0.0.8/setup.py` & `thonny_tunisiaschools-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/PKG-INFO` & `thonny_tunisiaschools-0.0.9/thonny_tunisiaschools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-tunisiaschools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Thonny IDE plug-in that offers PyQt / QT / Python support for Tunisian computer science secondary teachers / students .
 Home-page: https://github.com/selmen2004/thonny-tunisiaschools
 Author: Selmen Arous
 Author-email: Selmen Arous <selmen.arous@gmail.com>
 License: GPL version 3
 Keywords: PyQt,QT,Tunisia,School,Teaching,Education
 Platform: Windows
```

### Comparing `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/UIViewer.py` & `thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/UIViewer.py`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/__init__.py` & `thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 from datetime import date
-from thonny import get_workbench , get_thonny_user_dir
+from thonny import get_workbench
 from thonny.languages import tr
 from thonny.misc_utils import get_user_site_packages_dir_for_base
 from thonny.ui_utils import select_sequence,askopenfilename
 from .UIViewer import UiViewerPlugin
 
 from xml.dom import minidom
 global qt_ui_file
+qt_ui_file =""
 
 def usefull_commands(w):
     def add_cmd(w ,id, label , fct ):
         get_workbench()._publish_command(
                     "pyqt_text_"+w.attributes['name'].value+id,
                     "PyQt5",
                     label +w.attributes['name'].value ,
@@ -135,8 +136,8 @@
     if not os.path.exists(cwd):
         os.makedirs(cwd)
     get_workbench().set_local_cwd(cwd)
 
     # Ne pas ouvrir les derniers fichiers 
 
     get_workbench().set_option("file.current_file", "")
-    get_workbench().set_option("file.open_files", "")
+    get_workbench().set_option("file.open_files", "")
```

### Comparing `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/designer_16.png` & `thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/res/designer_16.png`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/qt_32.png` & `thonny_tunisiaschools-0.0.9/thonnycontrib/tunisiaschools/res/qt_32.png`

 * *Files identical despite different names*

