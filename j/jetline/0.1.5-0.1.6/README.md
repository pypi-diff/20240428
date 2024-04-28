# Comparing `tmp/jetline-0.1.5.tar.gz` & `tmp/jetline-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.1.5.tar", last modified: Sun Apr 28 16:04:44 2024, max compression
+gzip compressed data, was "jetline-0.1.6.tar", last modified: Sun Apr 28 16:11:02 2024, max compression
```

## Comparing `jetline-0.1.5.tar` & `jetline-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.184131 jetline-0.1.5/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:04:44.183932 jetline-0.1.5/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.5/README.md
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.178314 jetline-0.1.5/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.181001 jetline-0.1.5/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.5/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.5/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     9821 2024-04-28 15:55:37.000000 jetline-0.1.5/jetline/commands/create_viz.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.5/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.5/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.5/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.181672 jetline-0.1.5/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5190 2024-04-28 16:03:38.000000 jetline-0.1.5/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.5/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.5/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.182289 jetline-0.1.5/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1717 2024-04-28 11:42:42.000000 jetline-0.1.5/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.5/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.183356 jetline-0.1.5/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      226 2024-04-27 08:20:29.000000 jetline-0.1.5/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.5/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.5/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      406 2024-04-27 08:20:10.000000 jetline-0.1.5/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.183688 jetline-0.1.5/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:04:44.184181 jetline-0.1.5/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-28 16:04:33.000000 jetline-0.1.5/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.436151 jetline-0.1.6/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:11:02.435935 jetline-0.1.6/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.6/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.429880 jetline-0.1.6/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.6/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.432739 jetline-0.1.6/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.6/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.6/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.6/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     9821 2024-04-28 15:55:37.000000 jetline-0.1.6/jetline/commands/create_viz.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.6/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.6/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.6/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.6/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.433249 jetline-0.1.6/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.6/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-28 16:10:21.000000 jetline-0.1.6/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.6/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.6/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.433973 jetline-0.1.6/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.6/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1717 2024-04-28 11:42:42.000000 jetline-0.1.6/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.6/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.435277 jetline-0.1.6/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.6/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      226 2024-04-27 08:20:29.000000 jetline-0.1.6/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.6/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.6/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      406 2024-04-27 08:20:10.000000 jetline-0.1.6/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:11:02.435648 jetline-0.1.6/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:11:02.000000 jetline-0.1.6/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:11:02.000000 jetline-0.1.6/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:11:02.000000 jetline-0.1.6/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-28 16:11:02.000000 jetline-0.1.6/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:11:02.000000 jetline-0.1.6/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:11:02.000000 jetline-0.1.6/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:11:02.436196 jetline-0.1.6/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-28 16:10:49.000000 jetline-0.1.6/setup.py
```

### Comparing `jetline-0.1.5/PKG-INFO` & `jetline-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.5/README.md` & `jetline-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/_helper.py` & `jetline-0.1.6/jetline/commands/_helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/create_pipe.py` & `jetline-0.1.6/jetline/commands/create_pipe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/create_viz.py` & `jetline-0.1.6/jetline/commands/create_viz.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/info.py` & `jetline-0.1.6/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/installer.py` & `jetline-0.1.6/jetline/commands/installer.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/run_pipeline.py` & `jetline-0.1.6/jetline/commands/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/commands/to_exe.py` & `jetline-0.1.6/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/data/data.py` & `jetline-0.1.6/jetline/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     """
     A class representing data.
 
     Attributes:
         name (str): The name of the data.
         data (Any): The actual data stored.
     """
-    def __init__(self, data):
+    def __init__(self, name, data):
+        self.name = name
         self.data = data
    
 class DataManager:
     """
     The DataManager class is responsible for managing data objects. It ensures that only a single instance of the class is created.
```

### Comparing `jetline-0.1.5/jetline/pipeline/node.py` & `jetline-0.1.6/jetline/pipeline/node.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline/pipeline/pipeline.py` & `jetline-0.1.6/jetline/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/jetline.egg-info/PKG-INFO` & `jetline-0.1.6/jetline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.5/jetline.egg-info/SOURCES.txt` & `jetline-0.1.6/jetline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jetline-0.1.5/setup.py` & `jetline-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'vulture'
     
 
 ]
 
 setup(
     name='jetline',
-    version='0.1.5',
+    version='0.1.6',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
     classifiers=classifiers,
     keywords='pipeline automation',
```

