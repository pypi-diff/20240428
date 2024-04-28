# Comparing `tmp/torch_model_manager-0.0.6.dev9.tar.gz` & `tmp/torch_model_manager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev9.tar", last modified: Wed Apr 24 17:04:20 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.7.tar", last modified: Sun Apr 28 09:32:24 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev9.tar` & `torch_model_manager-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.324792 torch_model_manager-0.0.6.dev9/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 17:04:20.324792 torch_model_manager-0.0.6.dev9/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 17:03:55.000000 torch_model_manager-0.0.6.dev9/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.316792 torch_model_manager-0.0.6.dev9/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     4067 2024-04-24 17:04:15.000000 torch_model_manager-0.0.6.dev9/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16969 2024-04-24 16:47:11.000000 torch_model_manager-0.0.6.dev9/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev9/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.079480 torch_model_manager-0.0.7/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-28 09:32:24.079480 torch_model_manager-0.0.7/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1445 2024-04-28 09:32:12.000000 torch_model_manager-0.0.7/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.071480 torch_model_manager-0.0.7/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.071480 torch_model_manager-0.0.7/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22817 2024-04-28 09:24:10.000000 torch_model_manager-0.0.7/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.0.7/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6513 2024-04-28 09:23:28.000000 torch_model_manager-0.0.7/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev9/PKG-INFO` & `torch_model_manager-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev9
+Version: 0.0.7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
+Requires-Dist: torchcam
+Requires-Dist: neptune
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.0.6.dev9/README.md` & `torch_model_manager-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.7/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev9/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.7/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev9/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.7/torch_model_manager/torch_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,19 +406,19 @@
         for index in indexes:
             self.delete_layer_by_index(index)
 
     def visualize(self, shape, show_attrs: bool = True, show_saved: bool = True, **kwargs) -> None:
         x = torch.randn(shape)
         make_dot(self.model(x), 
                  params=dict(self.model.named_parameters()), 
-                 show_attrs=show_attrs, show_saved=show_saved).render(kwargs)
+                 show_attrs=show_attrs, show_saved=show_saved).render(**kwargs)
         
 
 
-    def show_hidden_layers(self, 
+    def show_hidden_conv2d(self, 
                            input_data: torch.Tensor, 
                            indexes, 
                            row_index: List[str] = None, 
                            show_figure: bool = True, 
                            figure_factor: float = 1.0,
                            save_path = None,
                            neptune_manager = None,
```

### Comparing `torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.7/torch_model_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev9
+Version: 0.0.7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
+Requires-Dist: torchcam
+Requires-Dist: neptune
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.7/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev9/utils/helpers.py` & `torch_model_manager-0.0.7/utils/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,8 +170,37 @@
     if mode == 'pre':
         concatenated_list = [char + str(item) for item in lst]
     elif mode == 'post':
         concatenated_list = [str(item) + char for item in lst]
     else:
         raise ValueError("Invalid mode. Use 'pre' or 'post'.")
 
-    return concatenated_list
+    return concatenated_list
+
+
+def add_to_json_file(file_path: str, key, value):
+    """
+    Add a key-value pair to a JSON file.
+
+    Args:
+        file_path (str): The path to the JSON file.
+        key: The key to add.
+        value: The value to add.
+    """
+    data = read_json_file(file_path)
+    data[key] = value
+    with open(file_path, 'w') as json_file:
+        json.dump(data, json_file)
+        
+def read_json_file(file_path):
+    """
+    Read a JSON file and return its content.
+
+    Args:
+        file_path: The path to the JSON file.
+
+    Returns:
+        The content of the JSON file.
+    """
+    with open(file_path, 'r') as json_file:
+        data = json.load(json_file)
+    return data
```

