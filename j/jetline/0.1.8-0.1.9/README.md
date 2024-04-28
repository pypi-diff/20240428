# Comparing `tmp/jetline-0.1.8.tar.gz` & `tmp/jetline-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.1.8.tar", last modified: Sun Apr 28 16:46:10 2024, max compression
+gzip compressed data, was "jetline-0.1.9.tar", last modified: Sun Apr 28 16:50:12 2024, max compression
```

## Comparing `jetline-0.1.8.tar` & `jetline-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.804414 jetline-0.1.8/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:46:10.804158 jetline-0.1.8/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.8/README.md
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.797351 jetline-0.1.8/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.800745 jetline-0.1.8/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.8/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.8/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10211 2024-04-28 16:43:19.000000 jetline-0.1.8/jetline/commands/create_viz.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.8/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.8/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.8/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.801476 jetline-0.1.8/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-28 16:10:21.000000 jetline-0.1.8/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.8/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.8/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.802273 jetline-0.1.8/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1685 2024-04-28 16:41:05.000000 jetline-0.1.8/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.8/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.803500 jetline-0.1.8/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      271 2024-04-28 16:45:03.000000 jetline-0.1.8/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.8/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.8/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      533 2024-04-28 16:45:49.000000 jetline-0.1.8/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.803831 jetline-0.1.8/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      308 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:46:10.804476 jetline-0.1.8/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1630 2024-04-28 16:46:06.000000 jetline-0.1.8/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.632384 jetline-0.1.9/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:50:12.632123 jetline-0.1.9/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.9/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.622449 jetline-0.1.9/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.625436 jetline-0.1.9/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.9/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.9/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10211 2024-04-28 16:43:19.000000 jetline-0.1.9/jetline/commands/create_viz.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.9/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.9/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.9/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.627537 jetline-0.1.9/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-28 16:10:21.000000 jetline-0.1.9/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.9/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.9/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.628619 jetline-0.1.9/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1686 2024-04-28 16:49:06.000000 jetline-0.1.9/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6042 2024-04-28 16:49:35.000000 jetline-0.1.9/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.630662 jetline-0.1.9/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      271 2024-04-28 16:45:03.000000 jetline-0.1.9/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.9/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.9/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      533 2024-04-28 16:45:49.000000 jetline-0.1.9/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.631616 jetline-0.1.9/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      308 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:50:12.632563 jetline-0.1.9/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1630 2024-04-28 16:50:02.000000 jetline-0.1.9/setup.py
```

### Comparing `jetline-0.1.8/PKG-INFO` & `jetline-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.8/README.md` & `jetline-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/_helper.py` & `jetline-0.1.9/jetline/commands/_helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/create_pipe.py` & `jetline-0.1.9/jetline/commands/create_pipe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/create_viz.py` & `jetline-0.1.9/jetline/commands/create_viz.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/info.py` & `jetline-0.1.9/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/installer.py` & `jetline-0.1.9/jetline/commands/installer.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/run_pipeline.py` & `jetline-0.1.9/jetline/commands/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/commands/to_exe.py` & `jetline-0.1.9/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/data/data.py` & `jetline-0.1.9/jetline/data/data.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline/pipeline/node.py` & `jetline-0.1.9/jetline/pipeline/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         outputs (list or None): A list of output names for the function. If None, the node does not have outputs.
 
     Methods:
         execute(data_manager):
         Executes the function of the node using input data from the data manager. If outputs are specified, updates the data manager with the results.
 
     """
-    def __init__(self,function, inputs, outputs=None, viz=None):
+    def __init__(self, function, inputs, outputs=None, viz=None):
         self.function = function
         self.inputs = inputs
         self.outputs = outputs
         self.viz = viz
 
     def execute(self, data_manager):
         """
```

### Comparing `jetline-0.1.8/jetline/pipeline/pipeline.py` & `jetline-0.1.9/jetline/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Pipeline:
     def __init__(self, nodes=None, data_manager=None):
         """
         Initialize the Pipeline with a list of nodes and a data manager.
         """
-        self.nodes = {node.name: node for node in nodes} if nodes else {}
+        self.nodes = {node.function: node for node in nodes} if nodes else {}
         self.data_manager = data_manager
         self.outputs = {}
 
     def run(self):
         """
         Runs the execute method of each node in the self.nodes dictionary
         and stores the output in the self.outputs dictionary.
```

### Comparing `jetline-0.1.8/jetline/templates/pipeline.py` & `jetline-0.1.9/jetline/templates/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/jetline.egg-info/PKG-INFO` & `jetline-0.1.9/jetline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.8/jetline.egg-info/SOURCES.txt` & `jetline-0.1.9/jetline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jetline-0.1.8/setup.py` & `jetline-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'vulture'
     
 
 ]
 
 setup(
     name='jetline',
-    version='0.1.8',
+    version='0.1.9',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
     classifiers=classifiers,
     keywords='pipeline automation',
```

