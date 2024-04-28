# Comparing `tmp/thonny_tunisiaschools-0.0.7.tar.gz` & `tmp/thonny_tunisiaschools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny_tunisiaschools-0.0.7.tar", last modified: Sun Apr 21 20:18:28 2024, max compression
+gzip compressed data, was "thonny_tunisiaschools-0.0.8.tar", last modified: Sun Apr 28 12:36:15 2024, max compression
```

## Comparing `thonny_tunisiaschools-0.0.7.tar` & `thonny_tunisiaschools-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-21 20:18:28.000000 thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-21 20:18:28.000000 thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:18:28.000000 thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 20:18:28.000000 thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-21 20:18:28.000000 thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/thonnycontrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/UIViewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:18:28.685266 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/res/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/res/designer_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/res/qt_16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-21 20:18:24.000000 thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/res/qt_32.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.929639 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-28 12:36:15.000000 thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.925639 thonny_tunisiaschools-0.0.8/thonnycontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.925639 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/UIViewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:36:15.925639 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/designer_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/qt_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-28 12:36:11.000000 thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/qt_32.png
```

### Comparing `thonny_tunisiaschools-0.0.7/PKG-INFO` & `thonny_tunisiaschools-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-tunisiaschools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Thonny IDE plug-in that offers PyQt / QT / Python support for Tunisian computer science secondary teachers / students .
 Home-page: https://github.com/selmen2004/thonny-tunisiaschools
 Author: Selmen Arous
 Author-email: Selmen Arous <selmen.arous@gmail.com>
 License: GPL version 3
 Keywords: PyQt,QT,Tunisia,School,Teaching,Education
 Platform: Windows
@@ -38,18 +38,26 @@
 
 # thonny-tunisiaschools
 
 A Thonny plug-in which offers Tunisian computer science secondary teachers / students some help creating Python & PyQt Applications:
 
 - loads QT UI file and :
 
-  - adds needed code to load that file to current document
+  - adds needed code to load that file to current document:
 
   - creates empty functions binded to buttons’ clicks
  
+  ![image](https://github.com/selmen2004/thonny-tunisiaschools/assets/3520243/4e4037a8-3157-4f09-99db-1b4543bb6233)
+ 
   - Adds a view that displays the UI inside Thonny (currently supporting Labels , Text inputs and ttons only )
+ 
+![image](https://github.com/selmen2004/thonny-tunisiaschools/assets/3520243/a3bdb491-6f31-4b92-a5eb-d2842eec95f1)
+
+
+- adds on new menu (PyQt5) commands to insert call to usual functions ( text , setText , clear , show ) if widget is Label or LineEdit ( as in Tunisian Curriculum )
+
+![image](https://github.com/selmen2004/thonny-tunisiaschools/assets/3520243/3bbd2794-c3f1-4425-92d2-6b5b1933f897)
 
-  - adds on new menu (PyQt5) commands to insert call to usual functions ( text , setText , clear , show ) if widget is Label or LineEdit ( as in Tunisian Curriculum )
 
 - changes save location to c:/bac2024 as needed for final exams (baccalaureat)
 
 - disables opening last open files (to reduce risks of students overwriting other students work)
```

### Comparing `thonny_tunisiaschools-0.0.7/pyproject.toml` & `thonny_tunisiaschools-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "thonny-tunisiaschools"
-version = "0.0.7"
+version = "0.0.8"
 description="A Thonny IDE plug-in that offers PyQt / QT / Python support for Tunisian computer science secondary teachers / students ."
 readme = "README.md"
 requires-python = ">=3.0"
 dependencies = [
   'thonny>=3.2.1',
 ]
 license ={text = "GPL version 3"}
```

### Comparing `thonny_tunisiaschools-0.0.7/setup.py` & `thonny_tunisiaschools-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.7/thonny_tunisiaschools.egg-info/PKG-INFO` & `thonny_tunisiaschools-0.0.8/thonny_tunisiaschools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-tunisiaschools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Thonny IDE plug-in that offers PyQt / QT / Python support for Tunisian computer science secondary teachers / students .
 Home-page: https://github.com/selmen2004/thonny-tunisiaschools
 Author: Selmen Arous
 Author-email: Selmen Arous <selmen.arous@gmail.com>
 License: GPL version 3
 Keywords: PyQt,QT,Tunisia,School,Teaching,Education
 Platform: Windows
@@ -38,18 +38,26 @@
 
 # thonny-tunisiaschools
 
 A Thonny plug-in which offers Tunisian computer science secondary teachers / students some help creating Python & PyQt Applications:
 
 - loads QT UI file and :
 
-  - adds needed code to load that file to current document
+  - adds needed code to load that file to current document:
 
   - creates empty functions binded to buttons’ clicks
  
+  ![image](https://github.com/selmen2004/thonny-tunisiaschools/assets/3520243/4e4037a8-3157-4f09-99db-1b4543bb6233)
+ 
   - Adds a view that displays the UI inside Thonny (currently supporting Labels , Text inputs and ttons only )
+ 
+![image](https://github.com/selmen2004/thonny-tunisiaschools/assets/3520243/a3bdb491-6f31-4b92-a5eb-d2842eec95f1)
+
+
+- adds on new menu (PyQt5) commands to insert call to usual functions ( text , setText , clear , show ) if widget is Label or LineEdit ( as in Tunisian Curriculum )
+
+![image](https://github.com/selmen2004/thonny-tunisiaschools/assets/3520243/3bbd2794-c3f1-4425-92d2-6b5b1933f897)
 
-  - adds on new menu (PyQt5) commands to insert call to usual functions ( text , setText , clear , show ) if widget is Label or LineEdit ( as in Tunisian Curriculum )
 
 - changes save location to c:/bac2024 as needed for final exams (baccalaureat)
 
 - disables opening last open files (to reduce risks of students overwriting other students work)
```

### Comparing `thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/UIViewer.py` & `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/UIViewer.py`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/res/designer_16.png` & `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/designer_16.png`

 * *Files identical despite different names*

### Comparing `thonny_tunisiaschools-0.0.7/thonnycontrib/tunisiaschools/res/qt_32.png` & `thonny_tunisiaschools-0.0.8/thonnycontrib/tunisiaschools/res/qt_32.png`

 * *Files identical despite different names*

