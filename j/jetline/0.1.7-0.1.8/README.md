# Comparing `tmp/jetline-0.1.7.tar.gz` & `tmp/jetline-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.1.7.tar", last modified: Sun Apr 28 16:13:30 2024, max compression
+gzip compressed data, was "jetline-0.1.8.tar", last modified: Sun Apr 28 16:46:10 2024, max compression
```

## Comparing `jetline-0.1.7.tar` & `jetline-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.019161 jetline-0.1.7/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:13:30.018920 jetline-0.1.7/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.7/README.md
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.010867 jetline-0.1.7/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.7/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.015118 jetline-0.1.7/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.7/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.7/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.7/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     9821 2024-04-28 15:55:37.000000 jetline-0.1.7/jetline/commands/create_viz.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.7/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.7/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.7/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.7/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.015898 jetline-0.1.7/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.7/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-28 16:10:21.000000 jetline-0.1.7/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.7/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.7/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.016599 jetline-0.1.7/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.7/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1717 2024-04-28 11:42:42.000000 jetline-0.1.7/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.7/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.017984 jetline-0.1.7/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.7/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      226 2024-04-27 08:20:29.000000 jetline-0.1.7/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.7/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.7/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      406 2024-04-27 08:20:10.000000 jetline-0.1.7/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:13:30.018448 jetline-0.1.7/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:13:29.000000 jetline-0.1.7/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:13:30.000000 jetline-0.1.7/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:13:30.000000 jetline-0.1.7/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      308 2024-04-28 16:13:30.000000 jetline-0.1.7/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:13:30.000000 jetline-0.1.7/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:13:30.000000 jetline-0.1.7/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:13:30.019240 jetline-0.1.7/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1630 2024-04-28 16:13:08.000000 jetline-0.1.7/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.804414 jetline-0.1.8/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:46:10.804158 jetline-0.1.8/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.8/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.797351 jetline-0.1.8/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.800745 jetline-0.1.8/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.8/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.8/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10211 2024-04-28 16:43:19.000000 jetline-0.1.8/jetline/commands/create_viz.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.8/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.8/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.8/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.801476 jetline-0.1.8/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-28 16:10:21.000000 jetline-0.1.8/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.8/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.8/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.802273 jetline-0.1.8/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1685 2024-04-28 16:41:05.000000 jetline-0.1.8/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.8/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.803500 jetline-0.1.8/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.8/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      271 2024-04-28 16:45:03.000000 jetline-0.1.8/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.8/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.8/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      533 2024-04-28 16:45:49.000000 jetline-0.1.8/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:46:10.803831 jetline-0.1.8/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      308 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:46:10.000000 jetline-0.1.8/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:46:10.804476 jetline-0.1.8/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1630 2024-04-28 16:46:06.000000 jetline-0.1.8/setup.py
```

### Comparing `jetline-0.1.7/PKG-INFO` & `jetline-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.7/README.md` & `jetline-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/commands/_helper.py` & `jetline-0.1.8/jetline/commands/_helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/commands/create_pipe.py` & `jetline-0.1.8/jetline/commands/create_pipe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/commands/create_viz.py` & `jetline-0.1.8/jetline/commands/create_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         main_content = file.read()
 
     pipeline_order_match = re.search(r'PIPELINE_ORDER\s*=\s*\[([^\]]+)\]', main_content)
     if pipeline_order_match:
         return pipeline_order_match.group(1).replace("'", "").replace('"', "").split(',')
     return None
 
+def extract_class_name(class_code):
+    # Suchen Sie nach dem ersten Auftreten von 'name =' im Klassencode
+    match = re.search(r"name\s*=\s*[\"']([^\"']+)[\"']", class_code)
+    if match:
+        # Extrahieren Sie den Namen aus dem Regex-Match
+        class_name = match.group(1)
+        return class_name
 
 def extract_classes_with_parent(current_dir):
     """
     Extracts all classes with a given parent class from a file.
     """
     nodes = []
     file_path = os.path.join(current_dir, "data.py")
@@ -62,15 +69,15 @@
                             isinstance(inner_node, ast.ClassDef) and
                             inner_node.name == 'Meta'
                     )
                     for assign in inner_node.body
                     if isinstance(assign, ast.Assign)
                 }
                 class_code = astor.to_source(node)
-                node_name = meta.get("name")
+                node_name = extract_class_name(class_code)
                 nodes.append({
                     "id": node_name,
                     "data": {
                         "title": node_name,
                         "type": "data",
                         "description": meta.get("description", "No description provided"),
                         "outputs": node_name,
@@ -146,14 +153,15 @@
                         sorted_nodes[i]["data"]["inputs"] = format_node_parameters(inputs[i])
 
                     if i < len(outputs):
                         sorted_nodes[i]["data"]["outputs"] = format_node_parameters(outputs[i])
 
             for i, position_data in enumerate(viz):
                 x = int(position_data.split(",")[0].split(":")[1].strip())
+
                 y = int(position_data.split(",")[1].split(":")[1].strip())
                 source = position_data.split(",")[2].split(":")[1].strip().replace("'", "").replace('"', '')
 
                 sorted_nodes[i]["position"]["x"] = x
                 sorted_nodes[i]["position"]["y"] = y
 
                 edge_id = f"{source}->{node_name}"
@@ -256,15 +264,15 @@
     if os.path.exists(destination_folder) and os.path.isdir(destination_folder):
         shutil.rmtree(destination_folder)
 
     # Kopieren Sie das Verzeichnis visualization und dessen gesamten Inhalt in das current_dir
     if os.path.exists(viz_folder) and os.path.isdir(viz_folder):
         shutil.copytree(viz_folder, destination_folder)
 
-    # add json to dist
-    output_file_path = "visualization/dist/viz-data.json"
+    # add json to distvisualization/dist/viz-data.json"
+    output_file_path = os.path.join(current_dir, "visualization", "dist", "viz-data.json" )
     with open(output_file_path, "w") as outfile:
         json.dump({"nodes": new_nodes, "edges": new_edges}, outfile, indent=4)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jetline-0.1.7/jetline/commands/info.py` & `jetline-0.1.8/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/commands/installer.py` & `jetline-0.1.8/jetline/commands/installer.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/commands/run_pipeline.py` & `jetline-0.1.8/jetline/commands/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/commands/to_exe.py` & `jetline-0.1.8/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/data/data.py` & `jetline-0.1.8/jetline/data/data.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline/pipeline/node.py` & `jetline-0.1.8/jetline/pipeline/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,15 @@
         outputs (list or None): A list of output names for the function. If None, the node does not have outputs.
 
     Methods:
         execute(data_manager):
         Executes the function of the node using input data from the data manager. If outputs are specified, updates the data manager with the results.
 
     """
-    def __init__(self, name, function, inputs, outputs=None, viz=None):
-        self.name = name
+    def __init__(self,function, inputs, outputs=None, viz=None):
         self.function = function
         self.inputs = inputs
         self.outputs = outputs
         self.viz = viz
 
     def execute(self, data_manager):
         """
```

### Comparing `jetline-0.1.7/jetline/pipeline/pipeline.py` & `jetline-0.1.8/jetline/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/jetline.egg-info/PKG-INFO` & `jetline-0.1.8/jetline.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.7/jetline.egg-info/SOURCES.txt` & `jetline-0.1.8/jetline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jetline-0.1.7/setup.py` & `jetline-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'vulture'
     
 
 ]
 
 setup(
     name='jetline',
-    version='0.1.7',
+    version='0.1.8',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
     classifiers=classifiers,
     keywords='pipeline automation',
```

