# Comparing `tmp/pyvisjs-0.0.0.dev5.tar.gz` & `tmp/pyvisjs-0.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev5.tar", last modified: Sat Apr 27 15:43:50 2024, max compression
+gzip compressed data, was "pyvisjs-0.0.0.dev6.tar", last modified: Sun Apr 28 18:39:03 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev5.tar` & `pyvisjs-0.0.0.dev6.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.510591 pyvisjs-0.0.0.dev5/
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-27 15:43:50.510591 pyvisjs-0.0.0.dev5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.505591 pyvisjs-0.0.0.dev5/examples/
--rw-rw-rw-   0 root         (0) root         (0)      539 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.507591 pyvisjs-0.0.0.dev5/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.508591 pyvisjs-0.0.0.dev5/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.509590 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      596 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 15:43:50.510591 pyvisjs-0.0.0.dev5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.509590 pyvisjs-0.0.0.dev5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     6122 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.864136 pyvisjs-0.0.0.dev6/
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-28 18:39:03.863136 pyvisjs-0.0.0.dev6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.858136 pyvisjs-0.0.0.dev6/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/examples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.860136 pyvisjs-0.0.0.dev6/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.861136 pyvisjs-0.0.0.dev6/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.863136 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 18:39:03.864136 pyvisjs-0.0.0.dev6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.862136 pyvisjs-0.0.0.dev6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     7893 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev5/.gitignore` & `pyvisjs-0.0.0.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/.gitlab-ci.yml` & `pyvisjs-0.0.0.dev6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/CONTRIBUTING.md` & `pyvisjs-0.0.0.dev6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/LICENSE` & `pyvisjs-0.0.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/PKG-INFO` & `pyvisjs-0.0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev5
+Version: 0.0.0.dev6
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev5/README.md` & `pyvisjs-0.0.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/folder_structure.txt` & `pyvisjs-0.0.0.dev6/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/pyproject.toml` & `pyvisjs-0.0.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/pyvisjs/base_dictable.py` & `pyvisjs-0.0.0.dev6/pyvisjs/base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/pyvisjs/network.py` & `pyvisjs-0.0.0.dev6/pyvisjs/network.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,93 @@
 from .base_dictable import BaseDictable
 from .utils import open_file, save_file
 from .node import Node
 from .edge import Edge
+from .options import Options
 from jinja2 import Environment, PackageLoader, select_autoescape
-from typing import Dict
+from typing import List
 
 class Network(BaseDictable):
 
-    def __init__(self, name="Network", data:Dict = {"nodes": [], "edges": []}, width="600px", height="400px"):
-        only_show_data_attr = lambda attr: attr == "data"
-        super().__init__(attr_filter_func=only_show_data_attr)
+    def __init__(self, name="Network", nodes:List[Node]=None, edges:List[Edge]=None, options:Options=None):
+        only_use_data_attr = lambda attr: attr == "_data"
+        super().__init__(attr_filter_func=only_use_data_attr)
         self.name = name
-        self.width = width
-        self.height = height
-        self.data = data
+        self._initialize_data(nodes, edges, options)
         self.env = Environment(
             loader=PackageLoader("pyvisjs"),
             autoescape=select_autoescape()
         )
 
+    @property
+    def options(self) -> Options:
+        opt = self._data["options"]   
+        return opt if isinstance(opt, Options) else None
+    
+    @options.setter
+    def options(self, val:Options):
+        self._data["options"] = val
+    
+    @property
+    def nodes(self) -> List[Node]: 
+        return self._data["nodes"]  
+    
+    @property
+    def edges(self) -> List[Edge]: 
+        return self._data["edges"]  
+
+    def _initialize_data(self, nodes:List[Node]=None, edges:List[Edge]=None, options:Options=None):
+        default_data = {"nodes": [], "edges": [], "options": {}}
+
+        if nodes:
+            default_data.update({
+                "nodes": nodes,
+            })
+
+        if edges:
+            default_data.update({
+                "edges": edges,
+            })
+
+        if options:
+            default_data.update({
+                "options": options,
+            })
+
+        self._data = default_data
+
     def __repr__(self):
-        return f"Network(\'{self.name}\', \'{self.width}\', \'{self.height}\')"
+        return f"Network(\'{self.name}\')"
     
     def add_node(self, node_id, label=None):
-        if not [node.id for node in self.data["nodes"] if node.id == node_id]:
-            self.data["nodes"].append(Node(node_id, label))
+        if not [node.id for node in self.nodes if node.id == node_id]:
+            self.nodes.append(Node(node_id, label))
 
     def add_edge(self, from_id, to_id):
         self.add_node(from_id)
         self.add_node(to_id)
 
-        if not [edge.start for edge in self.data["edges"] if edge.start == from_id and edge.end == to_id]:
-            self.data["edges"].append(Edge(from_id, to_id))
+        if not [edge.start for edge in self.edges if edge.start == from_id and edge.end == to_id]:
+            self.edges.append(Edge(from_id, to_id))
 
     def to_dict(self):
-        return super().to_dict()["data"]
+        return super().to_dict()["_data"]
 
     def show(self, file_name):
         self.render_template(open_in_browser=True, output_filename=file_name)
 
     def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html") -> str:
+        network_dict = self.to_dict()
+        
         html_output = self.env \
             .get_template(template_filename) \
             .render(
-                width=self.width,
-                height=self.height,
-                data=self.to_dict()
+                width=network_dict["options"].get("width", "100%"),
+                height=network_dict["options"].get("height", "100%"),
+                data=network_dict
             )
 
         if save_to_output or open_in_browser:
             file_path = save_file(output_filename, html_output)
 
         if open_in_browser:
             open_file(file_path)
```

### Comparing `pyvisjs-0.0.0.dev5/pyvisjs/templates/basic.html` & `pyvisjs-0.0.0.dev6/pyvisjs/templates/basic.html`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     var container = document.getElementById('visjsnet');
 
     // provide the data in the vis format
     var data = {
         nodes: nodes,
         edges: edges
     };
-    var options = {};
+    var options = {{data["options"]|tojson}};
 
     // initialize your network!
     var network = new vis.Network(container, data, options);
 </script>
 </body>
 </html>
```

### Comparing `pyvisjs-0.0.0.dev5/pyvisjs/utils.py` & `pyvisjs-0.0.0.dev6/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-0.0.0.dev6/pyvisjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev5
+Version: 0.0.0.dev6
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev5/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-0.0.0.dev6/pyvisjs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 examples/readme_usage.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
 pyvisjs/base_dictable.py
 pyvisjs/edge.py
 pyvisjs/network.py
 pyvisjs/node.py
+pyvisjs/options.py
 pyvisjs/utils.py
 pyvisjs.egg-info/PKG-INFO
 pyvisjs.egg-info/SOURCES.txt
 pyvisjs.egg-info/dependency_links.txt
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
 pyvisjs/templates/basic.html
 tests/__init__.py
 tests/test_base_dictable.py
 tests/test_edge.py
 tests/test_network.py
 tests/test_node.py
+tests/test_options.py
 tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev5/tests/test_base_dictable.py` & `pyvisjs-0.0.0.dev6/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/tests/test_edge.py` & `pyvisjs-0.0.0.dev6/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/tests/test_network.py` & `pyvisjs-0.0.0.dev6/tests/test_network.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,124 @@
 import pytest
 from unittest.mock import patch
-from pyvisjs import Network
+from pyvisjs import Network, Node, Edge, Options
 
 def test_network_init():
     # init
-    DEFAULT_WIDTH = "600px"
-    DEFAULT_HEIGHT = "400px"
-
+    DEFAULT_DICT = {
+        "nodes": [],
+        "edges": [],
+        "options": {}
+    }
     # mock
 
 
     # call
     n = Network("Network2")
     
     # assert
     assert n.name == "Network2"
-    assert n.width == DEFAULT_WIDTH
-    assert n.height == DEFAULT_HEIGHT
     assert n.env is not None
-    assert n.data == {"nodes": [], "edges": []}
+    assert n.to_dict() == DEFAULT_DICT
+
+def test_network_init_with_data():
+    # init
+    NETWORK_DICT = {
+        "nodes": [
+            { "id": 1, "label": "node 1", "color": None, "shape": "dot", "size": None, "cid": None },
+            { "id": 2, "label": "node 2", "color": None, "shape": "dot", "size": None, "cid": None },
+            { "id": 3, "label": "node 3", "color": None, "shape": "dot", "size": None, "cid": None },
+        ],
+        "edges": [
+            { "from": 1, "to": 2 },
+            { "from": 2, "to": 3 },
+            { "from": 3, "to": 4 }
+        ],
+        "options": {
+            "width": "100%",
+            "height": "100%",
+            "edges": {"color": "GRAY", "smooth": False},
+            "nodes": {
+                "scaling": {
+                    "max": 60, 
+                    "min": 10
+                }
+            },
+            "physics": {
+                "barnesHut": {"gravitationalConstant": None},
+                "stabilization": {"iterations": None}
+            }
+        }
+    }
+    # mock
+
+
+    # call
+    nd1 = Node(1, "node 1")
+    nd2 = Node(2, "node 2")
+    nd3 = Node(3, "node 3")
+
+    eg1 = Edge(1, 2)
+    eg2 = Edge(2, 3)
+    eg3 = Edge(3, 4)
+
+    opt = Options()
+
+    n = Network("Network2", [nd1, nd2, nd3], [eg1, eg2, eg3], opt)
+    
+    # assert
+    assert n.name == "Network2"
+    assert n.env is not None
+    assert n.to_dict() == NETWORK_DICT
+
+def test_network_read_write_properties():
+    # init
+
+    # mock
+
+    # call
+    nd1 = Node(1, "node 1")
+    nd2 = Node(2, "node 2")
+    nd3 = Node(3, "node 3")
+
+    eg1 = Edge(1, 2)
+    eg2 = Edge(2, 3)
+    eg3 = Edge(3, 4)
+
+    opt = Options()
+
+    n = Network("Network2", [nd1, nd2], [eg1])
+    n.options = opt
+    n.nodes.append(nd3)
+    n.edges.append(eg2)
+    n.edges.append(eg3)
+
+    # assert
+    assert n.options == opt
+    assert n.nodes == [nd1, nd2, nd3]
+    assert n.edges == [eg1, eg2, eg3]
+
 
 def test_network_add_nodes():
     # init
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_node(2) # duplicate node
     
     # assert
-    assert len(n.data["nodes"]) == 2
-    assert n.data["nodes"][0].id == 1
-    assert n.data["nodes"][0].label == "1"
-    assert n.data["nodes"][1].id == 2
-    assert n.data["nodes"][1].label == "name2"
+    assert len(n.nodes) == 2
+    assert n.nodes[0].id == 1
+    assert n.nodes[0].label == "1"
+    assert n.nodes[1].id == 2
+    assert n.nodes[1].label == "name2"
 
 def test_network_add_edges():
     # init
 
     # mock
 
     # call
@@ -48,36 +126,37 @@
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_edge(1, 2) # both nodes exist
     n.add_edge(2, 3) # one node missing
     n.add_edge(2, 3) # duplicate edge
     
     # assert
-    assert n.data["nodes"][0].id == 1
-    assert n.data["nodes"][1].id == 2
-    assert n.data["nodes"][2].id == 3
-
-    assert len(n.data["edges"]) == 2
-    assert n.data["edges"][0].start == 1
-    assert n.data["edges"][0].end == 2
-    assert n.data["edges"][1].start == 2
-    assert n.data["edges"][1].end == 3
+    assert n.nodes[0].id == 1
+    assert n.nodes[1].id == 2
+    assert n.nodes[2].id == 3
+
+    assert len(n.edges) == 2
+    assert n.edges[0].start == 1
+    assert n.edges[0].end == 2
+    assert n.edges[1].start == 2
+    assert n.edges[1].end == 3
 
 def test_network_to_dict():
     # init
     NETWORK_DICT = {
         "nodes": [
             { "id": 1, "label": "1", "color": None, "shape": "dot", "size": None, "cid": None },
             { "id": 2, "label": "name2", "color": None, "shape": "dot", "size": None, "cid": None },
             { "id": 3, "label": "3", "color": None, "shape": "dot", "size": None, "cid": None },
         ],
         "edges": [
             { "from": 1, "to": 2 },
             { "from": 2, "to": 3 }
-        ]
+        ],
+        "options": {}
     }
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
```

### Comparing `pyvisjs-0.0.0.dev5/tests/test_node.py` & `pyvisjs-0.0.0.dev6/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev5/tests/test_utils.py` & `pyvisjs-0.0.0.dev6/tests/test_utils.py`

 * *Files identical despite different names*

