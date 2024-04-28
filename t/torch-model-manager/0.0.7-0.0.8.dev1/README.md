# Comparing `tmp/torch_model_manager-0.0.7.tar.gz` & `tmp/torch_model_manager-0.0.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.7.tar", last modified: Sun Apr 28 09:32:24 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.8.dev1.tar", last modified: Sun Apr 28 09:54:56 2024, max compression
```

## Comparing `torch_model_manager-0.0.7.tar` & `torch_model_manager-0.0.8.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.079480 torch_model_manager-0.0.7/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-28 09:32:24.079480 torch_model_manager-0.0.7/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1445 2024-04-28 09:32:12.000000 torch_model_manager-0.0.7/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.071480 torch_model_manager-0.0.7/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.071480 torch_model_manager-0.0.7/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22817 2024-04-28 09:24:10.000000 torch_model_manager-0.0.7/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.0.7/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-28 09:32:24.000000 torch_model_manager-0.0.7/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:32:24.075480 torch_model_manager-0.0.7/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.7/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6513 2024-04-28 09:23:28.000000 torch_model_manager-0.0.7/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.376918 torch_model_manager-0.0.8.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-28 09:54:56.376918 torch_model_manager-0.0.8.dev1/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-28 09:54:56.376918 torch_model_manager-0.0.8.dev1/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-04-28 09:54:51.000000 torch_model_manager-0.0.8.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.368918 torch_model_manager-0.0.8.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.368918 torch_model_manager-0.0.8.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.372918 torch_model_manager-0.0.8.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.372918 torch_model_manager-0.0.8.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22772 2024-04-28 09:53:53.000000 torch_model_manager-0.0.8.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.0.8.dev1/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.372918 torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-28 09:54:56.000000 torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-28 09:54:56.000000 torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-28 09:54:56.000000 torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-04-28 09:54:56.000000 torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-28 09:54:56.000000 torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 09:54:56.372918 torch_model_manager-0.0.8.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.0.8.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.7/PKG-INFO` & `torch_model_manager-0.0.8.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.7
+Version: 0.0.8.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.7/README.md` & `torch_model_manager-0.0.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.7/setup.py` & `torch_model_manager-0.0.8.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.0.7'
+version = '0.0.8.dev1'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.0.7/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.8.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.7/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.8.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.7/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.8.dev1/torch_model_manager/neptune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,32 +119,29 @@
                 source_files (list, optional): The source files of the run. Defaults to None.
                 capture_strerr (bool, optional): Whether to capture stderr. Defaults to True.
                 git_ref (str, optional): The git reference of the run. Defaults to None.
             """
             self.run = None
             # Try to read the JSON file
             try:
-
                 run_ids = helpers.read_json_file(NeptuneManager.run_ids_path)
-
                 # If the name of the run already exists in the JSON file, load the run with the same name.
-                if name in run_ids.keys(): 
-                    
+                if name in list(run_ids.keys()): 
                     if run_ids is not None:
                         self.run = neptune.init_run(
                             project=NeptuneManager.project_name,
                             api_token=NeptuneManager.api_token,
                             with_id=run_ids[name],
                             **kwargs
                         )
                         
                 else:
                     # Create a new run
                     # The names of the runs should all be different
-                    assert name not in run_ids.keys(), "Run with the same name already exists. Please choose a different name."    
+                    assert name not in list(run_ids.keys()), "Run with the same name already exists. Please choose a different name."    
                     
                     self.run = neptune.init_run(
                         project=NeptuneManager.project_name,
                         api_token=NeptuneManager.api_token,
                         name=name,
                         description=description,
                         tags=tags,
@@ -505,28 +502,29 @@
                                 names = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
                                 namespace=namespace,
                                 on_series=True)
                     
             print(Fore.GREEN+"The hidden conv2d layer outputs are successfully logged to Neptune.", Fore.WHITE)
             return result, row_index, col_index
             
-print(os.path.abspath("."))
-# nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-#                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-#                     run_ids_path="run_ids.json")
+
+
+nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
+                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
+                    run_ids_path="run_ids.json")
 
 # from torchvision import models
 # parameters = {
 #     "lr": 1e-2,
 #     "bs": 128,
 #     "input_sz": 32 * 32 * 3,
 #     "n_classes": 10,
 #     "model_filename": "basemodel",
 #     "device": torch.device("cuda" if torch.cuda.is_available() else "cpu"),
 #     "epochs": 2,
 # }
 
 
-# run = nm.Run(name="Test2")
+run = nm.Run(name="Test2")
 
 # model= models.vgg16()
 # run.log_hidden_conv2d(model, torch.randn(1, 3, 224, 224), indexes=[["features", 0], ["features", 1]], namespace="hidden_conv2d", method="layercam")
```

### Comparing `torch_model_manager-0.0.7/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.8.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.7/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.7
+Version: 0.0.8.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.7/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.8.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.7/utils/helpers.py` & `torch_model_manager-0.0.8.dev1/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Any
 import matplotlib.pyplot as plt
 import torch
 from torchvision import transforms
+import json
 
 def required_kernel(in_size: int, out_size:int, stride=1, padding=1):
     assert in_size > 0, "Input size must be greater than 0"
     assert out_size > 0, "Output size must be greater than 0"
     assert in_size >= out_size, "Input size must be greater than or equal to output size"
     assert stride > 0, "Stride must be greater than 0"
     assert padding >= 0, "Padding must be greater than or equal to 0"
```

