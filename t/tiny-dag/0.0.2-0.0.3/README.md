# Comparing `tmp/tiny_dag-0.0.2.tar.gz` & `tmp/tiny_dag-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_dag-0.0.2.tar", last modified: Sat Apr 27 09:31:34 2024, max compression
+gzip compressed data, was "tiny_dag-0.0.3.tar", last modified: Sat Apr 27 13:59:18 2024, max compression
```

## Comparing `tiny_dag-0.0.2.tar` & `tiny_dag-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/LICENSE
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1410 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      872 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/README.md
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.2/pyproject.toml
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-27 09:31:34.060354 tiny_dag-0.0.2/setup.cfg
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/src/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/src/tiny_dag.egg-info/
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1410 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/SOURCES.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/dependency_links.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/requires.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/top_level.txt
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/src/tinydag/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/src/tinydag/__init__.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     5962 2024-04-27 08:13:34.000000 tiny_dag-0.0.2/src/tinydag/graph.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      711 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/src/tinydag/node.py
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 13:59:18.123643 tiny_dag-0.0.3/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.3/LICENSE
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1362 2024-04-27 13:59:18.123643 tiny_dag-0.0.3/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      824 2024-04-27 13:49:56.000000 tiny_dag-0.0.3/README.md
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.3/pyproject.toml
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-27 13:59:18.123643 tiny_dag-0.0.3/setup.cfg
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 13:59:18.119643 tiny_dag-0.0.3/src/
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 13:59:18.123643 tiny_dag-0.0.3/src/tiny_dag.egg-info/
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1362 2024-04-27 13:59:18.000000 tiny_dag-0.0.3/src/tiny_dag.egg-info/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2024-04-27 13:59:18.000000 tiny_dag-0.0.3/src/tiny_dag.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-27 13:59:18.000000 tiny_dag-0.0.3/src/tiny_dag.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-27 13:59:18.000000 tiny_dag-0.0.3/src/tiny_dag.egg-info/requires.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-27 13:59:18.000000 tiny_dag-0.0.3/src/tiny_dag.egg-info/top_level.txt
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 13:59:18.123643 tiny_dag-0.0.3/src/tinydag/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.3/src/tinydag/__init__.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     6227 2024-04-27 13:48:41.000000 tiny_dag-0.0.3/src/tinydag/graph.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      711 2024-04-27 07:53:55.000000 tiny_dag-0.0.3/src/tinydag/node.py
```

### Comparing `tiny_dag-0.0.2/LICENSE` & `tiny_dag-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_dag-0.0.2/PKG-INFO` & `tiny_dag-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.2
-Summary: Mimimal DAG implementation with Python
+Version: 0.0.3
+Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,18 +21,20 @@
 # Requirements
 
 - Python >= 3.6
 - graphviz
 
 # Installation
 
-Binary installers for the latest released version are available at the Python Package Index (PyPI):
-https://pypi.org/project/tiny-dag/
+Install graphviz (optional, needed for rendering)
+```
+sudo apt-get install graphviz
+```
 
-Install by typing
+Install tiny-dag
 ```
 pip3 install tiny-dag
 ```
 
 # Usage example
 
 ```
```

### Comparing `tiny_dag-0.0.2/README.md` & `tiny_dag-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 # Requirements
 
 - Python >= 3.6
 - graphviz
 
 # Installation
 
-Binary installers for the latest released version are available at the Python Package Index (PyPI):
-https://pypi.org/project/tiny-dag/
+Install graphviz (optional, needed for rendering)
+```
+sudo apt-get install graphviz
+```
 
-Install by typing
+Install tiny-dag
 ```
 pip3 install tiny-dag
 ```
 
 # Usage example
 
 ```
```

### Comparing `tiny_dag-0.0.2/setup.cfg` & `tiny_dag-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = tiny-dag
-version = 0.0.2
+version = 0.0.3
 author = Ossi Myllymäki
 author_email = omyllymaki@gmail.com
-description = Mimimal DAG implementation with Python
+description = Minimal DAG implementation with Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/omyllymaki/tiny-dag
 project_urls = 
 	Bug Tracker = https://github.com/omyllymaki/tiny-dag/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `tiny_dag-0.0.2/src/tiny_dag.egg-info/PKG-INFO` & `tiny_dag-0.0.3/src/tiny_dag.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.2
-Summary: Mimimal DAG implementation with Python
+Version: 0.0.3
+Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,18 +21,20 @@
 # Requirements
 
 - Python >= 3.6
 - graphviz
 
 # Installation
 
-Binary installers for the latest released version are available at the Python Package Index (PyPI):
-https://pypi.org/project/tiny-dag/
+Install graphviz (optional, needed for rendering)
+```
+sudo apt-get install graphviz
+```
 
-Install by typing
+Install tiny-dag
 ```
 pip3 install tiny-dag
 ```
 
 # Usage example
 
 ```
```

### Comparing `tiny_dag-0.0.2/src/tinydag/graph.py` & `tiny_dag-0.0.3/src/tinydag/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 import time
 from copy import copy
-from typing import List, Callable, Union
-
-import graphviz as graphviz
-from graphviz import Digraph
-
+from typing import List, Callable, Union, Optional
 from tinydag.node import Node
 
 logger = logging.getLogger(__name__)
 
+try:
+    import graphviz as graphviz
+    from graphviz import Digraph
+except ImportError:
+    logger.warning("Cannot import graphviz")
+
 
 class GraphError(Exception):
     pass
 
 
 class Graph:
     """
@@ -57,28 +59,33 @@
 
         self._check_nodes(nodes)
         self.nodes = nodes
         self.wrappers = wrappers
 
     def render(self,
                path: str = "graph.gv",
-               view: bool = True) -> Digraph:
+               view: bool = True) -> Optional[Digraph]:
         """
         Render graph.
         :param path: Path to save fig.
         :param view: Show graph fig.
         """
-        dot = graphviz.Digraph()
-        for node in self.nodes:
-            dot.node(node.name, node.name)
-        for node in self.nodes:
-            for node_input in node.inputs:
-                dot.edge(node_input, node.name)
-        dot.render(path, view=view)
-        return dot
+
+        try:
+            dot = graphviz.Digraph()
+            for node in self.nodes:
+                dot.node(node.name, node.name)
+            for node in self.nodes:
+                for node_input in node.inputs:
+                    dot.edge(node_input, node.name)
+            dot.render(path, view=view)
+            return dot
+        except Exception as e:
+            logger.warning(f"Graph cannot be rendered, error {e}")
+            return None
 
     def check(self, input_data: dict = None) -> None:
         """
         Check if graph can be executed. Raises Exception if graph is not valid.
 
         :param input_data: Input data for graph, where keys are names used in graph definition.
         """
```

### Comparing `tiny_dag-0.0.2/src/tinydag/node.py` & `tiny_dag-0.0.3/src/tinydag/node.py`

 * *Files identical despite different names*

