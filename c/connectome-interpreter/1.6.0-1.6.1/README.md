# Comparing `tmp/connectome_interpreter-1.6.0.tar.gz` & `tmp/connectome_interpreter-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.6.0.tar", last modified: Sun Apr 28 18:02:12 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.6.1.tar", last modified: Sun Apr 28 18:55:03 2024, max compression
```

## Comparing `connectome_interpreter-1.6.0.tar` & `connectome_interpreter-1.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.129335 connectome_interpreter-1.6.0/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     1064 2024-04-28 18:02:12.126344 connectome_interpreter-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.055096 connectome_interpreter-1.6.0/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.0/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.6.0/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    21517 2024-04-28 17:52:40.000000 connectome_interpreter-1.6.0/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16141 2024-04-28 10:55:54.000000 connectome_interpreter-1.6.0/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.0/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.105548 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1064 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 18:02:12.129335 connectome_interpreter-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1675 2024-04-28 17:54:41.000000 connectome_interpreter-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.125349 connectome_interpreter-1.6.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.0/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.939546 connectome_interpreter-1.6.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     1088 2024-04-28 18:55:03.939546 connectome_interpreter-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.894189 connectome_interpreter-1.6.1/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.1/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.6.1/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.1/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16141 2024-04-28 10:55:54.000000 connectome_interpreter-1.6.1/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.1/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.935559 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1088 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 18:55:03.939546 connectome_interpreter-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1695 2024-04-28 18:51:25.000000 connectome_interpreter-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.937552 connectome_interpreter-1.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.1/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.1/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.6.0/LICENSE` & `connectome_interpreter-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/PKG-INFO` & `connectome_interpreter-1.6.1/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: connectome_interpreter
-Version: 1.6.0
+Name: connectome-interpreter
+Version: 1.6.1
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
@@ -16,11 +16,12 @@
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
+Requires-Dist: IPython
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.6.0/README.md` & `connectome_interpreter-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.6.1/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.6.1/connectome_interpreter/compress_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tqdm import tqdm
 import pandas as pd
 import plotly.express as px
 from scipy.sparse import issparse
 import ipywidgets as widgets
 import seaborn as sns
 import matplotlib.pyplot as plt
+from IPython.display import display
 
 from .utils import dynamic_representation, torch_sparse_where, to_nparray, tensor_to_csc
 
 
 def compress_paths(inprop, step_number, threshold=0, output_threshold=1e-4):
     """
     Performs iterative multiplication of a sparse matrix `inprop` for a specified number of steps, 
@@ -419,8 +420,8 @@
             df.sort_index(inplace=True)
         heatmaps.append(df)
 
     slider = widgets.IntSlider(value=1, min=1, max=len(heatmaps), step=1,
                                description='Path length', continuous_update=True)
 
     # Link the slider to the plotting function
-    widgets.interactive(plot_heatmap, index=slider)
+    display(widgets.interactive(plot_heatmap, index=slider))
```

### Comparing `connectome_interpreter-1.6.0/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.6.1/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/connectome_interpreter/utils.py` & `connectome_interpreter-1.6.1/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: connectome-interpreter
-Version: 1.6.0
+Name: connectome_interpreter
+Version: 1.6.1
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
@@ -16,11 +16,12 @@
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
+Requires-Dist: IPython
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.6.0/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.6.1/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/setup.py` & `connectome_interpreter-1.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.6.0',
+    version='1.6.1',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
         'torch',
         'tqdm',
         'plotly',
         'matplotlib',
         'networkx',
         'seaborn',
         'ipywidgets',
+        'IPython',
     ],
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
     author='Yijie Yin',
```

### Comparing `connectome_interpreter-1.6.0/tests/test_compress_paths.py` & `connectome_interpreter-1.6.1/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.0/tests/test_utils.py` & `connectome_interpreter-1.6.1/tests/test_utils.py`

 * *Files identical despite different names*

