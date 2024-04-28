# Comparing `tmp/connectome_interpreter-1.5.0.tar.gz` & `tmp/connectome_interpreter-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.5.0.tar", last modified: Sun Apr 21 22:28:32 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.6.0.tar", last modified: Sun Apr 28 18:02:12 2024, max compression
```

## Comparing `connectome_interpreter-1.5.0.tar` & `connectome_interpreter-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.483544 connectome_interpreter-1.5.0/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      938 2024-04-21 22:28:32.483544 connectome_interpreter-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.438568 connectome_interpreter-1.5.0/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.5.0/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.5.0/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    17800 2024-04-21 21:48:11.000000 connectome_interpreter-1.5.0/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16261 2024-04-14 17:16:24.000000 connectome_interpreter-1.5.0/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.5.0/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.469242 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0      938 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 22:28:32.484539 connectome_interpreter-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1557 2024-04-20 17:52:45.000000 connectome_interpreter-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.481552 connectome_interpreter-1.5.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.5.0/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.5.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.129335 connectome_interpreter-1.6.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     1064 2024-04-28 18:02:12.126344 connectome_interpreter-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.055096 connectome_interpreter-1.6.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.6.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    21517 2024-04-28 17:52:40.000000 connectome_interpreter-1.6.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16141 2024-04-28 10:55:54.000000 connectome_interpreter-1.6.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.105548 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1064 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-28 18:02:11.000000 connectome_interpreter-1.6.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 18:02:12.129335 connectome_interpreter-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1675 2024-04-28 17:54:41.000000 connectome_interpreter-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:02:12.125349 connectome_interpreter-1.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.0/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.0/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.5.0/LICENSE` & `connectome_interpreter-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.5.0/PKG-INFO` & `connectome_interpreter-1.6.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
-Name: connectome_interpreter
-Version: 1.5.0
+Name: connectome-interpreter
+Version: 1.6.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
+Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
+Requires-Dist: seaborn
+Requires-Dist: ipywidgets
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.5.0/README.md` & `connectome_interpreter-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.5.0/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.6.0/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.5.0/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.6.0/connectome_interpreter/compress_paths.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 """
 
 import torch
 from tqdm import tqdm
 import pandas as pd
 import plotly.express as px
 from scipy.sparse import issparse
+import ipywidgets as widgets
+import seaborn as sns
+import matplotlib.pyplot as plt
 
 from .utils import dynamic_representation, torch_sparse_where, to_nparray, tensor_to_csc
 
 
 def compress_paths(inprop, step_number, threshold=0, output_threshold=1e-4):
     """
     Performs iterative multiplication of a sparse matrix `inprop` for a specified number of steps, 
@@ -207,16 +210,16 @@
     represented by their input and output indexes. The function calculates 
     the total synaptic input from presynaptic neuron groups to an average neuron in each 
     postsynaptic neuron group.
 
     Args:
         stepsn (scipy.sparse matrix or numpy.ndarray): Matrix representing the synaptic strengths 
             between neurons, can be dense or sparse.
-        inidx (numpy.ndarray): Array of indices representing the input (presynaptic) neurons, used to subset stepsn. nan values are removed.
-        outidx (numpy.ndarray): Array of indices representing the output (postsynaptic) neurons.
+        inidx (int, float, list, set, numpy.ndarray, or pandas.Series): Array of indices representing the input (presynaptic) neurons, used to subset stepsn. nan values are removed.
+        outidx (int, float, list, set, numpy.ndarray, or pandas.Series): Array of indices representing the output (postsynaptic) neurons.
         inidx_map (dict, optional): Mapping from indices to neuron groups for the input neurons. Defaults to None, in which case neurons are not grouped. 
         outidx_map (dict, optional): Mapping from indices to neuron groups for the output neurons.
             Defaults to None, in which case it is set to be the same as inidx_map.
         display_output (bool, optional): Whether to display the output in a coloured dataframe. Defaults to True.
         sort_by_column (str or list, optional): the column name(s) to sort the result by. If none is provided, then sort by the first column. 
         pre_in_column (bool, optional): Whether to have the presynaptic neuron groups as columns. Defaults to False (pre in rows, post in columns).
         display_threshold (float, optional): The threshold for displaying the output. Defaults to 0.
@@ -293,16 +296,16 @@
     different path lengths. This function calculates and visualizes the average input 
     received by a neuron in each postsynaptic neuron group from presynaptic ones, aggregated over specified 
     path lengths. Direct connections are in path_length 1.
 
     Args:
         steps (list of scipy.sparse matrices): List of sparse matrices, each representing 
             synaptic strengths for a specific path length.
-        inidx (numpy.ndarray): Array of indices representing input (presynaptic) neurons.
-        outidx (numpy.ndarray): Array of indices representing output (postsynaptic) neurons.
+        inidx (int, float, list, set, numpy.ndarray, or pandas.Series): Array of indices representing input (presynaptic) neurons.
+        outidx (int, float, list, set, numpy.ndarray, or pandas.Series): Array of indices representing output (postsynaptic) neurons.
         outidx_map (dict): Mapping from indices to postsynaptic neuron groups.
 
     Returns:
         None: Displays a line plot with path lengths on the x-axis, the average input 
             received on the y-axis, and lines differentiated by postsynaptic neuron groups.
             The plot represents how different postsynaptic neuron groups are influenced by 
             presynaptic neurons over various path lengths.
@@ -350,7 +353,74 @@
         xaxis=dict(
             tickmode='linear',
             tick0=1,
             dtick=1
         )
     )
     fig.show()
+
+
+def contribution_by_path_lengths_heatmap(steps, inidx, outidx, inidx_map=None, outidx_map=None,
+                                         sort_by_index=True, sort_by_column=None,
+                                         pre_in_column=False,
+                                         display_threshold=0,
+                                         cmap='viridis'):
+    """
+    Display the contribution from inidx to outidx, grouped by inidx_map and outidx_map, across different path lengths.
+
+    Args:
+        steps (list of scipy.sparse matrices): List of sparse matrices, each representing synaptic strengths for a specific path length.
+        inidx (int, float, list, set, numpy.ndarray, or pandas.Series): Array of indices representing input (presynaptic) neurons.
+        outidx (int, float, list, set, numpy.ndarray, or pandas.Series): Array of indices representing output (postsynaptic) neurons.
+        inidx_map (dict, optional): Mapping from indices to input neuron groups. Defaults to None, in which case neurons are not grouped.
+        outidx_map (dict, optional): Mapping from indices to output neuron groups. Defaults to None, in which case it is set to be the same as inidx_map.
+        sort_by_index (bool, optional): Whether to sort the output by index. Defaults to True.
+        sort_by_column (str or list, optional): the column name(s) to sort the result by. If none is provided, then sort by the first column.
+        pre_in_column (bool, optional): Whether to have the presynaptic neuron groups as columns. Defaults to False (pre in rows, post in columns).
+        display_threshold (float, optional): The threshold for displaying the output. Defaults to 0.
+        cmap (str, optional): The colormap to use for the heatmap. Defaults to 'viridis'.
+
+    Returns:
+        None: Displays an interactive heatmap showing the contribution from inidx to outidx, grouped by inidx_map and outidx_map, across different path lengths.
+
+    """
+
+    inidx = to_nparray(inidx)
+    outidx = to_nparray(outidx)
+
+    if inidx_map is None:
+        inidx_map = {idx: idx for idx in inidx}
+    if outidx_map is None:
+        outidx_map = inidx_map
+
+    def plot_heatmap(index):
+        plt.figure(figsize=(30, 15))
+        # plt.imshow(heatmaps[index], cmap='viridis', aspect = 'auto')
+        # Use seaborn's heatmap function which is a higher-level API for Matplotlib's imshow
+        sns.heatmap(heatmaps[index-1], annot=True, fmt=".2f",
+                    linewidths=.5, cmap=cmap)
+
+        # Rotate the tick labels for the columns to show them better
+        plt.xticks(rotation=90)
+        plt.yticks(rotation=0)
+
+        # Show the heatmap
+        plt.show()
+
+    heatmaps = []
+
+    for step in tqdm(steps):
+        df = result_summary(step, inidx, outidx,
+                            inidx_map, outidx_map,
+                            display_output=False,
+                            sort_by_column=sort_by_column,
+                            pre_in_column=pre_in_column,
+                            display_threshold=display_threshold)
+        if sort_by_index:
+            df.sort_index(inplace=True)
+        heatmaps.append(df)
+
+    slider = widgets.IntSlider(value=1, min=1, max=len(heatmaps), step=1,
+                               description='Path length', continuous_update=True)
+
+    # Link the slider to the plotting function
+    widgets.interactive(plot_heatmap, index=slider)
```

### Comparing `connectome_interpreter-1.5.0/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.6.0/connectome_interpreter/path_finding.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,31 +68,27 @@
     if top_n == -1:
         top_n_indices = np.argsort(thresholded_row_averages)
     else:
         top_n_indices = np.argsort(thresholded_row_averages)[-top_n:]
     # Get the original row indices corresponding to these top n averages
     top_n_row_indices = thresholded_intersect[top_n_indices]
 
-    # Initialize lists to store data for DataFrame
-    pre_list, post_list, weight_list = [], [], []
+    # make the edgelist
+    submatrix = inprop_csc[top_n_row_indices, :][:, outidx]
 
-    # Iterate through each possible combination and store only non-zero weights
-    for pre in top_n_row_indices:
-        for post in outidx:
-            weight = inprop_csc[pre, post]
-            if weight > 0:  # Only consider non-zero weights
-                pre_list.append(pre)
-                post_list.append(post)
-                weight_list.append(weight)
+    # Convert submatrix to COO format to efficiently find non-zero elements
+    coo_submatrix = submatrix.tocoo()
 
-    # Construct DataFrame from lists
+    # Create DataFrame directly from COO format data
     df = pd.DataFrame({
-        'pre': pre_list,
-        'post': post_list,
-        'weight': weight_list
+        # Map back to original indices
+        'pre': top_n_row_indices[coo_submatrix.row],
+        # Map back to original output indices
+        'post': outidx[coo_submatrix.col],
+        'weight': coo_submatrix.data
     })
 
     return df
 
 
 def find_path_iteratively(inprop_csc, steps_cpu, inidx, outidx, target_layer_number, top_n=-1, threshold=0):
     """
```

### Comparing `connectome_interpreter-1.5.0/connectome_interpreter/utils.py` & `connectome_interpreter-1.6.0/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.5.0/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
-Name: connectome-interpreter
-Version: 1.5.0
+Name: connectome_interpreter
+Version: 1.6.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
+Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
+Requires-Dist: seaborn
+Requires-Dist: ipywidgets
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.5.0/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.6.0/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.5.0/setup.py` & `connectome_interpreter-1.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.5.0',
+    version='1.6.0',
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
+        'seaborn',
+        'ipywidgets',
     ],
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
     author='Yijie Yin',
     author_email='yy432@cam.ac.uk',
     description='A tool for connectomics data interpretation',
     keywords=['connectomics', 'neural network',
               'mechanistic interpretability'],
     project_urls={
+        'Source': 'https: // github.com/YijieYin/connectome_interpreter',
         'Documentation': 'https://connectome-interpreter.readthedocs.io/en/latest/',
         'Larva connectome example': 'https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing',
         'Adult connectome example (FAFB)': 'https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing',
     },
     # url='https://connectome-interpreter.readthedocs.io/en/latest/',
     test_suite='tests'  # Project home page
 )
```

### Comparing `connectome_interpreter-1.5.0/tests/test_compress_paths.py` & `connectome_interpreter-1.6.0/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.5.0/tests/test_utils.py` & `connectome_interpreter-1.6.0/tests/test_utils.py`

 * *Files identical despite different names*

