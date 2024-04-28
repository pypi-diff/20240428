# Comparing `tmp/sdeper-1.1.0.tar.gz` & `tmp/sdeper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeper-1.1.0.tar", last modified: Sat Apr 20 13:07:25 2024, max compression
+gzip compressed data, was "sdeper-1.2.0.tar", last modified: Sun Apr 28 05:24:34 2024, max compression
```

## Comparing `sdeper-1.1.0.tar` & `sdeper-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:25.875962 sdeper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 13:07:17.000000 sdeper-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 13:07:17.000000 sdeper-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-20 13:07:25.875962 sdeper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-20 13:07:17.000000 sdeper-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-20 13:07:17.000000 sdeper-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 13:07:17.000000 sdeper-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:07:25.875962 sdeper-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-20 13:07:17.000000 sdeper-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:25.871962 sdeper-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/admm_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    37931 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/cvae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/cvaeglrm.py
--rw-r--r--   0 runner    (1001) docker     (127)    27000 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/hyper_parameter_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/imputation.py
--rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/local_fit_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    50641 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/parse_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/run_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:07:25.875962 sdeper-1.1.0/src/sdeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 13:07:25.000000 sdeper-1.1.0/src/sdeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23099 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 13:07:17.000000 sdeper-1.1.0/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:34.496528 sdeper-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-28 05:24:26.000000 sdeper-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-28 05:24:26.000000 sdeper-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-28 05:24:34.496528 sdeper-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-28 05:24:26.000000 sdeper-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-28 05:24:26.000000 sdeper-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 05:24:26.000000 sdeper-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:24:34.496528 sdeper-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-28 05:24:26.000000 sdeper-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:34.496528 sdeper-1.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/admm_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44389 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/cvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/cvaeglrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23811 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/diagnosis_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/hyper_parameter_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/local_fit_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52767 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/parse_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/run_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:34.496528 sdeper-1.2.0/src/sdeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23236 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/version.py
```

### Comparing `sdeper-1.1.0/LICENSE` & `sdeper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/PKG-INFO` & `sdeper-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.1.0
+Version: 1.2.0
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
@@ -28,21 +28,27 @@
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: umap-learn==0.5.3
 Requires-Dist: distinctipy==1.2.2
 Requires-Dist: reportlab==4.1.0
 Requires-Dist: opencv-python==4.6.0.66
 
 # SDePER
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
 
-SDePER can be installed via `pip`
+SDePER can be installed via conda
+
+```bash
+conda create -n sdeper-env -c bioconda -c conda-forge python=3.9.12 sdeper
+```
+
+or pip
 
 ```bash
 conda create -n sdeper-env python=3.9.12
 conda activate sdeper-env
 pip install sdeper
 ```
```

### Comparing `sdeper-1.1.0/README.md` & `sdeper-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # SDePER
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
 
-SDePER can be installed via `pip`
+SDePER can be installed via conda
+
+```bash
+conda create -n sdeper-env -c bioconda -c conda-forge python=3.9.12 sdeper
+```
+
+or pip
 
 ```bash
 conda create -n sdeper-env python=3.9.12
 conda activate sdeper-env
 pip install sdeper
 ```
```

### Comparing `sdeper-1.1.0/setup.py` & `sdeper-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/src/admm_fit.py` & `sdeper-1.2.0/src/admm_fit.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/src/config.py` & `sdeper-1.2.0/src/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     # for Docker image
     input_path = r'/data'  
     output_path = r'/data'
 else:
     input_path = ''
     output_path = os.getcwd()
 
+# diagnosis plots folder
+diagnosis_path = os.path.join(output_path, 'diagnosis')
 
 
 """
 define a small value to avoid divided by 0 or log(0)
 """
 min_val = 1e-12
```

### Comparing `sdeper-1.1.0/src/cvae.py` & `sdeper-1.2.0/src/cvae.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,223 +6,272 @@
 @author: hill103
 
 this script stores functions to build a CVAE for platform effect adjustment
 """
 
 
 
-import os
-from config import print, output_path
+from config import print
 import numpy as np
 import pandas as pd
 from utils import read_spatial_data, read_scRNA_data, run_DE
 from time import time
 import random
 from sklearn.preprocessing import MinMaxScaler
 import scanpy as sc
 sc.settings.verbosity = 0  # verbosity: errors (0), warnings (1), info (2), hints (3)
 
 import tensorflow.keras.backend as K
 from tensorflow.keras.layers import Lambda, Input, Dense, Activation, concatenate
-#from tensorflow.keras.layers import BatchNormalization
+from tensorflow.keras.layers import BatchNormalization
 from tensorflow.keras.models import Model
 from tensorflow.keras import optimizers
 from tensorflow.keras.callbacks import ReduceLROnPlateau, EarlyStopping
 from tensorflow.keras.utils import set_random_seed
 
 # dealing with the keras symbolic tensor error
 from tensorflow.python.framework.ops import disable_eager_execution
 disable_eager_execution()
 
 
 
-def build_CVAE(spatial_df, scRNA_df, scRNA_celltype, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, rerun_DE=True, filter_gene=True):
+def celltype2props(celltype_anno, celltype_order):
+    '''
+    calculate cell-type proportions matrix given one cell-type annotation
+
+    Parameters
+    ----------
+    celltype_anno : dataframe
+        cell-type annotations. Only 1 column named <celltype>
+    celltype_order : list
+        already sorted unique cell-types. Its order matters, and will be the order in cell-type proportions (columns) and cell-type gene expression profile (rows)
+
+    Returns
+    -------
+    celltype_prop : dataframe
+        cell-type proportions, columns are already sorted cell-types
     '''
-    build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
     
-    input gene expression in datasets only included genes needed for downstream analysis and already been normalized by sequencing depth
+    celltype_stats = []
+    for i in celltype_anno.index:
+        celltype_stats.append({celltype_anno.loc[i, 'celltype']: 1})
+    # transform to matrix
+    celltype_prop = pd.DataFrame(celltype_stats, columns=celltype_order, index=celltype_anno.index)
+    celltype_prop.fillna(0, inplace=True)
+    # calculate cell-type proportions, divides each element in a row by the sum of that row
+    celltype_prop = celltype_prop.div(celltype_prop.sum(axis=1), axis=0)
+    
+    return celltype_prop
+
+
+
+def generate_pseudo_spots(exp_df, celltype_anno, n_spot, celltype_order, pseudo_spot_min_cell, pseudo_spot_max_cell):
+    '''
+    generate pseudo-spots for CVAE training by randomly combining scRNA-seq cells
+    
+    UPDATE:
+    
+    now we separate the pseudo-spots and all scRNA-seq cells, i.e. we DO NOT add all cells to the end of the dataframe as special pseudo-spots with only one cell
+    
+    if n_spot=0, i.e. no pseudo-spots, then return an empty dataframe
 
     Parameters
     ----------
-    spatial_df : dataframe
-        normalized gene expression in spatial transcriptomic data (spots * genes).
-    scRNA_df : dataframe
-        normalized gene expression in scRNA-seq data (cells * genes).
-    scRNA_celltype : dataframe
+    exp_df : dataframe
+        normalized gene expression (cell * genes)
+    celltype_anno : dataframe or None
         cell-type annotations for cells in scRNA-seq data. Only 1 column named <celltype>
-    n_marker_per_cmp : int
-        number of TOP marker genes for each comparison in DE
+    n_spot : int
+        number of pseudo spots need to be generated, including training and validation set
+    celltype_order : list
+        already sorted unique cell-types. Its order matters, and will be the order in cell-type proportions (columns) and cell-type gene expression profile (rows)
     pseudo_spot_min_cell : int
         minimum value of cells in pseudo-spot
     pseudo_spot_max_cell : int
         maximum value of cells in pseudo-spot
-    seq_depth_scaler : int
-        a scaler of scRNA-seq sequencing depth
-    cvae_input_scaler : int
-        maximum value of the scaled input for CVAE
-    cvae_init_lr : float
-        initial learning rate for training CVAE
-    use_fdr : bool
-        whether to use FDR adjusted p value for filtering and sorting
-    p_val_cutoff : float
-        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering
-    fc_cutoff : float
-        threshold of fold change (without log transform!) in marker genes filtering
-    pct1_cutoff : float
-        threshold of pct.1 in marker genes filtering
-    pct2_cutoff : float
-        threshold of pct.2 in marker genes filtering
-    sortby_fc : bool
-        whether to sort marker genes by fold change
-    diagnosis : bool
-        if True save more information to files for diagnosis CVAE and hyper-parameter selection
-    rerun_DE : bool, optional
-        whether to rerun DE on the CVAE transformed scRNA-seq data, since the DE genes might be different with before CVAE transforming.
-    filter_gene : bool
-        whether to filter genes before DE.
-    
 
     Returns
     -------
-    spatial_transformed_df : dataframe
-        CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes)
-    scRNA_decode_df : dataframe
-        CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes)
-    new_markers : list or None
-        marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE (rerun_DE=False).
+    pseudo_spots_df : dataframe
+        pseudo-spot gene expression (pseudo-spots * genes; NO original cells included)
+    pseudo_spots_celltype_prop : dataframe
+        pseudo-spot cell-type proportions (pseudo-spots * cell-types; NO original cells included)
+    n_cell_in_spot : list
+        number of cells/spots in pseudo-spots (NO original cells included)
     '''
     
-    assert((scRNA_df.index == scRNA_celltype.index).all())
-    assert((spatial_df.columns == scRNA_df.columns).all())
-    
-    # some settings
-    # max number of pseudo spots (training+validation, without training single cells)
-    n_max_pseudo_spots = 5e5
-    # scaler to multiply the normalized gene values and transform back to raw nUMI counts
-    depth_scaler = seq_depth_scaler
-    # percentage of training pseudo spots
-    training_pct = 0.8
-    # max value when scaling the input gene expression of CVAE, while min is 0
-    input_max = cvae_input_scaler
-    
-    celltypes = sorted(list(scRNA_celltype.celltype.unique()))
-    n_celltype = len(celltypes)
-    celltype_count_dict = scRNA_celltype.celltype.value_counts().to_dict()
-    
-    # Randomly select cells into pseudo-spots, at most X pseudo-spots
-    print(f'generate pseudo-spots containing {pseudo_spot_min_cell} to {pseudo_spot_max_cell} cells from scRNA-seq cells...')
-    n_spot = int(min(100 * spatial_df.shape[0] * n_celltype, n_max_pseudo_spots))
-    n_train_spot = int(np.floor(n_spot * training_pct))
-    n_valid_spot = int(n_spot - n_train_spot)
+    if n_spot == 0:
+        return pd.DataFrame(columns=exp_df.columns), pd.DataFrame(columns=celltype_order), []
     
-    print(f'generate {n_train_spot} pseudo-spots for training and {n_valid_spot} pseudo-spots for validation')
-
     pseudo_spots = []
     celltype_stats = []
     n_cell_in_spot = []
     
     n_cell_list = list(range(pseudo_spot_min_cell, pseudo_spot_max_cell+1))
-    all_cell_index = scRNA_df.index.to_list()
     # cell barcode separated by cell-types
     type_cell_index = dict()
-    for one_celltype in celltypes:
-        type_cell_index[one_celltype] = scRNA_celltype[scRNA_celltype['celltype']==one_celltype].index.to_list()
+    for one_celltype in celltype_order:
+        type_cell_index[one_celltype] = celltype_anno[celltype_anno['celltype']==one_celltype].index.to_list()
+    
     
     # though it's possible to use multiprocessing to generate pseudo-spots parallelly, the big dataframe need to be shared across all subprocesses, and it may not be a good idea to share objects in multiprocessing as it may cause unknown problems. And the performance benefits by multiprocessing many not be such large
     # so considering the safety and performance benefits, just keep the simplest way to generate pseudo-spots one-by-one
     # to reduce randomness, pre-set the seed value for random
     random.seed(138)
+    
+    # Set to track the milestones to print
+    milestones = set(round((n_spot / 10) * i) for i in range(1, 11))
+    # Ensure that no milestone can exceed the total number of spots
+    milestones = {m for m in milestones if m <= n_spot}
+
     for i in range(n_spot):
+        
+        if i+1 in milestones:
+            # Calculate the current percentage, ensure it does not exceed 100%
+            cur_progress = min(round((i+1) / n_spot, 2), 1)
+            print(f'{cur_progress:.0%}...', end='')
+
         # first determine how many cells in this pseudo-spot
         this_num = random.sample(n_cell_list, 1)[0]
         n_cell_in_spot.append(this_num)
         
         this_cells = []
         for i in range(this_num):
             # select one cell-type
-            selected_celltype = random.sample(celltypes, 1)[0]
+            selected_celltype = random.sample(celltype_order, 1)[0]
             # from this selected cell-type, randomly select one cell belong to that cell-type
             this_cells.append(random.sample(type_cell_index[selected_celltype], 1)[0])
         
         # take average of selected cells
-        pseudo_spots.append(scRNA_df.loc[this_cells].mean(axis=0))
+        pseudo_spots.append(exp_df.loc[this_cells].mean(axis=0))
         
         # count the celltype of selected cells
-        celltype_stats.append(scRNA_celltype.loc[this_cells, 'celltype'].value_counts().to_dict())
+        celltype_stats.append(celltype_anno.loc[this_cells, 'celltype'].value_counts().to_dict())
     
-    # Add the scRNA-seq cells as pseudo-spots containing only one cell to the end
-    for this_cells in all_cell_index:
-        pseudo_spots.append(scRNA_df.loc[this_cells])
-        celltype_stats.append({scRNA_celltype.loc[this_cells, 'celltype']: 1})
-        n_cell_in_spot.append(1)
-
+    # make below prints in a newline
+    print('\n')
 
     # Build pseudo-spots dataframe
     # First n_valid_spot spots are used for validation, rest spots are used for training
     pseudo_spots_df = pd.concat(pseudo_spots, axis=1).transpose()
     pseudo_spots_df.reset_index(inplace=True, drop=True)
+    pseudo_spots_df.index = ['scrna_pseudo' + str(idx) for idx in pseudo_spots_df.index]
     
-    pseudo_spots_celltype = pd.DataFrame(celltype_stats, columns=celltypes)
-    pseudo_spots_celltype.fillna(0, inplace=True)
+    pseudo_spots_celltype_prop = pd.DataFrame(celltype_stats, columns=celltype_order, index=pseudo_spots_df.index)
+    pseudo_spots_celltype_prop.fillna(0, inplace=True)
     # calculate cell-type proportions
-    pseudo_spots_celltype = pseudo_spots_celltype.div(pseudo_spots_celltype.sum(axis=1), axis=0)
+    pseudo_spots_celltype_prop = pseudo_spots_celltype_prop.div(pseudo_spots_celltype_prop.sum(axis=1), axis=0)
     
     #import gc
     #import psutil
     #print(f'before gc and del variable RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
-    del pseudo_spots, celltype_stats
+    #del pseudo_spots, celltype_stats
     #print(f'del variable without gc RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
     #gc.collect()
     #print(f'after gc RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
     
+    return pseudo_spots_df, pseudo_spots_celltype_prop, n_cell_in_spot
+
+
+
+def combine_spatial_spots(exp_df, n_spot, pseudo_spot_min_cell, pseudo_spot_max_cell):
+    '''
+    we also generate "pseudo-spots" by combining spatial spots
     
-    # Build training and validation data
-    # nomalize to [0,input_max] with each dataset separately
-    # use only training pseudo spots + single cells for scRNA-seq dataset normalization
-    print(f'scaling inputs to range 0 to {input_max}')
-    spatial_min_max_scaler = MinMaxScaler(feature_range=[0,input_max])
-    tmp_spatial_data = spatial_min_max_scaler.fit_transform(spatial_df)
-    
-    scRNA_min_max_scaler = MinMaxScaler(feature_range=[0,input_max])
-    scRNA_min_max_scaler.fit(pseudo_spots_df.iloc[n_valid_spot:,:])
-    tmp_scRNA_data = scRNA_min_max_scaler.transform(pseudo_spots_df)
-    
-    # first n_valid_spot spots used for validation, rest spots used for training, as spots with only one cell are listed at the end
-    oversample_scale = 1
-    data = np.vstack((np.tile(tmp_spatial_data, (oversample_scale, 1)), tmp_scRNA_data[n_valid_spot:,:]))
-    labels = np.array([input_max]*tmp_spatial_data.shape[0]*oversample_scale + [0.]*tmp_scRNA_data[n_valid_spot:,:].shape[0])
-    labels = labels.reshape((len(labels), 1))
+    here we do not know the true cell-type proportions in spatial spots, so we also do not know the proportions in generated "pseudo-spots". We just ignore it, and only use the expressions for CVAE training
+
+    Parameters
+    ----------
+    exp_df : dataframe
+        normalized gene expression (spots * genes)
+    n_spot : int
+        number of pseudo spots need to be generated, including training and validation set
+    pseudo_spot_min_cell : int
+        minimum value of cells in pseudo-spot
+    pseudo_spot_max_cell : int
+        maximum value of cells in pseudo-spot
+
+    Returns
+    -------
+    pseudo_spots_df : dataframe
+        pseudo-spot gene expression (pseudo-spots * genes; NO original cells included)
+    '''
+    if n_spot == 0:
+        return pd.DataFrame(columns=exp_df.columns)
     
-    # validation data
-    valid_data = tmp_scRNA_data[:n_valid_spot,:]
-    valid_labels = np.array([0.]*n_valid_spot)
-    valid_labels = valid_labels.reshape((len(valid_labels), 1))
+    pseudo_spots = []
+    n_cell_list = list(range(pseudo_spot_min_cell, pseudo_spot_max_cell+1))
+    spot_index = exp_df.index.to_list()
     
-    n_scRNA_training_spot = tmp_scRNA_data[n_valid_spot:,:].shape[0]
-    n_spatial_training_spot = tmp_spatial_data.shape[0]*oversample_scale
-    print(f'in training -- spatial spots : pseudo-spots = {n_spatial_training_spot:d} : {n_scRNA_training_spot:d}')
+    # to reduce randomness, pre-set the seed value for random
+    random.seed(154)
     
-    del tmp_spatial_data, tmp_scRNA_data
+    # Set to track the milestones to print
+    milestones = set(round((n_spot / 10) * i) for i in range(1, 11))
+    # Ensure that no milestone can exceed the total number of spots
+    milestones = {m for m in milestones if m <= n_spot}
     
-    # re-weight spatial data to make sure the sample size equals spatial:scRNA = 1:10
-    sample_weight = np.ones((data.shape[0],))
-    # also increase the weight of scRNA-seq cells
-    #sample_weight = np.array([1.]*n_spatial_training_spot + [1.]*n_train_spot + [2.]*len(all_cell_index))
-
-    if n_spatial_training_spot < 0.1 * n_scRNA_training_spot:
-        sample_weight[:n_spatial_training_spot] *= 0.1 * n_scRNA_training_spot / n_spatial_training_spot
+    for i in range(n_spot):
+        
+        if i+1 in milestones:
+            # Calculate the current percentage, ensure it does not exceed 100%
+            cur_progress = min(round((i+1) / n_spot, 2), 1)
+            print(f'{cur_progress:.0%}...', end='')
+            
+        # first determine how many spots in this pseudo-spot
+        this_num = random.sample(n_cell_list, 1)[0]
+        # then randomly select these number of spots and take average
+        pseudo_spots.append(exp_df.loc[random.sample(spot_index, this_num)].mean(axis=0))
     
+    # make below prints in a newline
+    print('\n')
     
-    # Define CVAE
-    # number of nodes in input layer (equals number of celltypes)
-    p = data.shape[1]
-    # number of nodes in conditional node
-    p_cond = 1
+    # Build pseudo-spots dataframe
+    pseudo_spots_df = pd.concat(pseudo_spots, axis=1).transpose()
+    pseudo_spots_df.reset_index(inplace=True, drop=True)
+    pseudo_spots_df.index = ['spatial_pseudo' + str(idx) for idx in pseudo_spots_df.index]
     
+    return pseudo_spots_df
+
+
+
+def CVAE_keras_model(p, p_cond, latent_dim, p_encoder_lst, p_decoder_lst, hidden_act='elu', output_act='relu', use_batch_norm=True, cvae_init_lr=0.01):
+    '''
+    define a standard CVAE model based on Keras
+    need to build a decoder separately as can not extract it from the whole model
+
+    Parameters
+    ----------
+    p : int
+        number of nodes in input layer
+    p_cond : int
+        number of conditional nodes in input layer
+    latent_dim : int
+        number of nodes in latent space
+    p_encoder_lst : list of integers
+        including number of nodes in each hidden layer of encoder, the length of list is the number of hidden layers
+    p_decoder_lst : list of integers
+        including number of nodes in each hidden layer of decoder, the length of list is the number of hidden layers
+    hidden_act : string, optional
+        activation function of hidden layers. Default is elu function
+    output_act : string, optional
+        activation function of output layer. Default is relu function
+    use_batch_norm : bool, optional
+        whether to use batch normalization. Default if True, i.e. use batch normalization
+    cvae_init_lr : float
+        initial learning rate for training CVAE
     
+    Returns
+    -------
+    cvae : Keras model
+        CVAE model. Encoder can be extracted from it
+    decoder : Keras model
+        corresponding decoder, reset its weights after CVAE training
+    '''
+
     # Functions for CVAE
     # reparameterization trick
     # instead of sampling from Q(z|X), sample eps = N(0,I)
     # z = z_mean + sqrt(var)*eps
     def sampling(args):
         """Reparameterization trick by sampling fr an isotropic unit Gaussian.
         # Arguments:
@@ -235,365 +284,496 @@
         dim = K.int_shape(z_mean)[1]
         # by default, random_normal has mean=0 and std=1.0
         epsilon = K.random_normal(shape=(batch, dim), mean=0., stddev=1)
         return z_mean + K.exp(0.5 * z_log_var) * epsilon
 
     # the Keras framework support custom loss returning one value, but more correct way is returning an array of losses (one of sample in the input batch), and the reducing the done by Keras
     # when return an array of losses, we can also handle the specified sample_weight
-    def vae_loss(obs, pred):
-        # VAE loss = mse_loss or xent_loss + kl_loss
-        recon_loss = K.sum(K.square(obs - pred), axis=-1)
+    def KL_loss(obs, pred):
         kl_loss = 1 + z_log_var - K.square(z_mean) - K.exp(z_log_var)
         kl_loss = K.sum(kl_loss, axis=-1)
         kl_loss *= -0.5
-        return recon_loss + kl_loss
+        return kl_loss
     
+    def reconstruction_loss(obs, pred):
+        return K.sum(K.square(obs - pred), axis=-1)
     
-    # Hyper-parameters
-    latent_dim = n_celltype * 3
-    # hidden_dim = (latent_dim * np.floor(np.sqrt(p/latent_dim))).astype('int')
-    # use geometric mean of latent and input dimension
-    hidden_dim = np.floor(np.sqrt(p * latent_dim))
+    def vae_loss(obs, pred, C=1):
+        # currently we set weight C=1
+        return C*reconstruction_loss(obs, pred) + KL_loss(obs, pred)
     
     
     # Build encoder model
     X = Input(shape=(p,), name='encoder_input')
     cond = Input(shape=(p_cond,), name='cond_input')
     encoder_inputs = concatenate([X, cond])
-    # hidden layer 1
-    encoder_hidden = Dense(hidden_dim, use_bias=True)(encoder_inputs)
-    #encoder_hidden = BatchNormalization()(encoder_hidden)
-    encoder_hidden = Activation('elu')(encoder_hidden)
-    # encoding layer z_mean
-    z_mean_pre = Dense(latent_dim, use_bias=True)(encoder_hidden)
-    #z_mean_pre = BatchNormalization()(z_mean_pre)
-    z_mean = Activation('linear', name='z_mean')(z_mean_pre)
-    # encoding layer z_log_var
-    z_log_var_pre = Dense(latent_dim, use_bias=True)(encoder_hidden)
-    #z_log_var_pre = BatchNormalization()(z_log_var_pre)
-    z_log_var = Activation('linear', name='z_log_var')(z_log_var_pre)
+    
+    # add hidden layers
+    for i, num in enumerate(p_encoder_lst):
+        if i == 0:
+            # 1st hidden layer
+            if use_batch_norm:
+                encoder_hidden = Dense(num, use_bias=False, name=f'encoder_layer{i}_w')(encoder_inputs)
+                encoder_hidden = BatchNormalization(name=f'encoder_layer{i}_BN')(encoder_hidden)
+                encoder_hidden = Activation(hidden_act, name=f'encoder_layer{i}_act')(encoder_hidden)
+            else:
+                encoder_hidden = Dense(num, use_bias=True, name=f'encoder_layer{i}_w')(encoder_inputs)
+                encoder_hidden = Activation(hidden_act, name=f'encoder_layer{i}_act')(encoder_hidden)
+        else:
+            if use_batch_norm:
+                encoder_hidden = Dense(num, use_bias=False, name=f'encoder_layer{i}_w')(encoder_hidden)
+                encoder_hidden = BatchNormalization(name=f'encoder_layer{i}_BN')(encoder_hidden)
+                encoder_hidden = Activation(hidden_act, name=f'encoder_layer{i}_act')(encoder_hidden)
+            else:
+                encoder_hidden = Dense(num, use_bias=True, name=f'encoder_layer{i}_w')(encoder_hidden)
+                encoder_hidden = Activation(hidden_act, name=f'encoder_layer{i}_act')(encoder_hidden)
+    
+    
+    # latent layer of z_mean and z_log_var
+    if use_batch_norm:
+        z_mean_pre = Dense(latent_dim, use_bias=False)(encoder_hidden)
+        z_mean_pre = BatchNormalization()(z_mean_pre)
+        z_mean = Activation('linear', name='z_mean')(z_mean_pre)
+        
+        z_log_var_pre = Dense(latent_dim, use_bias=False)(encoder_hidden)
+        z_log_var_pre = BatchNormalization()(z_log_var_pre)
+        z_log_var = Activation('linear', name='z_log_var')(z_log_var_pre)
+    else:
+        z_mean_pre = Dense(latent_dim, use_bias=True)(encoder_hidden)
+        z_mean = Activation('linear', name='z_mean')(z_mean_pre)
+        
+        z_log_var_pre = Dense(latent_dim, use_bias=True)(encoder_hidden)
+        z_log_var = Activation('linear', name='z_log_var')(z_log_var_pre)
     
     # use reparameterization trick to push the sampling out as input
     # note that "output_shape" isn't necessary with the TensorFlow backend
     z = Lambda(sampling, output_shape=(latent_dim,), name='z')([z_mean, z_log_var])
     
     
     # Build decoder model
     latent_plus_cond = concatenate([z, cond])
-    # hidden layer 1
-    decoder_hidden = Dense(hidden_dim, use_bias=True, name='decoder_layer1_w')(latent_plus_cond)
-    #decoder_hidden = BatchNormalization(name='decoder_layer1_BN')(decoder_hidden)
-    decoder_hidden = Activation('elu', name='decoder_layer1_act')(decoder_hidden)
-    # output layer
-    decoder_hidden = Dense(p, use_bias=True, name='decoder_output_w')(decoder_hidden)
-    #decoder_hidden = BatchNormalization(name='decoder_output_BN')(decoder_hidden)
-    decoder_output = Activation('relu', name='decoder_output_act')(decoder_hidden)
     
-    # recorder the layer names which need to re-store weights
-    layer_names = ['decoder_layer1_w', 'decoder_output_w']
+    # add hidden layers
+    for i, num in enumerate(p_decoder_lst):
+        if i == 0:
+            # 1st hidden layer
+            if use_batch_norm:
+                decoder_hidden = Dense(num, use_bias=False, name=f'decoder_layer{i}_w')(latent_plus_cond)
+                decoder_hidden = BatchNormalization(name=f'decoder_layer{i}_BN')(decoder_hidden)
+                decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+            else:
+                decoder_hidden = Dense(num, use_bias=True, name=f'decoder_layer{i}_w')(latent_plus_cond)
+                decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+        else:
+            if use_batch_norm:
+                decoder_hidden = Dense(num, use_bias=False, name=f'decoder_layer{i}_w')(decoder_hidden)
+                decoder_hidden = BatchNormalization(name=f'decoder_layer{i}_BN')(decoder_hidden)
+                decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+            else:
+                decoder_hidden = Dense(num, use_bias=True, name=f'decoder_layer{i}_w')(decoder_hidden)
+                decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
     
     
+    # output layer
+    if use_batch_norm:
+        decoder_hidden = Dense(p, use_bias=False, name='decoder_output_w')(decoder_hidden)
+        decoder_hidden = BatchNormalization(name='decoder_output_BN')(decoder_hidden)
+        decoder_output = Activation(output_act, name='decoder_output_act')(decoder_hidden)
+    else:
+        decoder_hidden = Dense(p, use_bias=True, name='decoder_output_w')(decoder_hidden)
+        decoder_output = Activation(output_act, name='decoder_output_act')(decoder_hidden)
+    
+   
     # CVAE model = encoder + decoder
     # by using the Keras functional API, the variables will be created right away without needing to call .build(). When not using API, you can manually call `model.build()`
     cvae = Model([X, cond], decoder_output, name='cvae')
     
     # Optimazer
     adam = optimizers.Adam(learning_rate=cvae_init_lr, clipnorm=1.0, decay=0.0)
-    cvae.compile(optimizer=adam, loss=vae_loss, experimental_run_tf_function=True)
+    cvae.compile(optimizer=adam, loss=vae_loss, metrics=[reconstruction_loss, KL_loss], experimental_run_tf_function=True)
     
     
-    # learning rate decay
-    lrate = ReduceLROnPlateau(monitor='val_loss', factor=0.75, patience=15, min_lr=1e-5, cooldown=5, verbose=False)
+    # Subset the decoder (build another new decoder and re-store weights)
+    def build_new_decoder(p, p_cond, latent_dim, p_decoder_lst, hidden_act='elu', output_act='relu', use_batch_norm=False):
+        latent_inputs = Input(shape=(latent_dim,), name='z_sampling')
+        cond_input = Input(shape=(p_cond,), name='conditions')
+        latent_plus_cond = concatenate([latent_inputs, cond_input])
+        
+        # add hidden layers
+        for i, num in enumerate(p_decoder_lst):
+            if i == 0:
+                # 1st hidden layer
+                if use_batch_norm:
+                    decoder_hidden = Dense(num, use_bias=False, name=f'decoder_layer{i}_w')(latent_plus_cond)
+                    decoder_hidden = BatchNormalization(name=f'decoder_layer{i}_BN')(decoder_hidden)
+                    decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+                else:
+                    decoder_hidden = Dense(num, use_bias=True, name=f'decoder_layer{i}_w')(latent_plus_cond)
+                    decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+            else:
+                if use_batch_norm:
+                    decoder_hidden = Dense(num, use_bias=False, name=f'decoder_layer{i}_w')(decoder_hidden)
+                    decoder_hidden = BatchNormalization(name=f'decoder_layer{i}_BN')(decoder_hidden)
+                    decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+                else:
+                    decoder_hidden = Dense(num, use_bias=True, name=f'decoder_layer{i}_w')(decoder_hidden)
+                    decoder_hidden = Activation(hidden_act, name=f'decoder_layer{i}_act')(decoder_hidden)
+        
+        # output layer
+        if use_batch_norm:
+            decoder_hidden = Dense(p, use_bias=False, name='decoder_output_w')(decoder_hidden)
+            decoder_hidden = BatchNormalization(name='decoder_output_BN')(decoder_hidden)
+            decoder_output = Activation(output_act, name='decoder_output_act')(decoder_hidden)
+        else:
+            decoder_hidden = Dense(p, use_bias=True, name='decoder_output_w')(decoder_hidden)
+            decoder_output = Activation(output_act, name='decoder_output_act')(decoder_hidden)
+    
+        new_decoder = Model([latent_inputs, cond_input], decoder_output, name='new_decoder')
+        return new_decoder
+    
+    new_decoder = build_new_decoder(p, p_cond, latent_dim, p_decoder_lst, hidden_act, output_act, use_batch_norm)
+    
+    return cvae, new_decoder
+
+
+
+def build_CVAE(spatial_df, scRNA_df, scRNA_celltype, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, rerun_DE=True, filter_gene=True):
+    '''
+    build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
+    
+    input gene expression in datasets only included genes needed for downstream analysis and already been normalized by sequencing depth
+
+    Parameters
+    ----------
+    spatial_df : dataframe
+        normalized gene expression in spatial transcriptomic data (spots * genes).
+    scRNA_df : dataframe
+        normalized gene expression in scRNA-seq data (cells * genes).
+    scRNA_celltype : dataframe
+        cell-type annotations for cells in scRNA-seq data. Only 1 column named <celltype>.
+    n_marker_per_cmp : int
+        number of TOP marker genes for each comparison in DE.
+    n_pseudo_spot : int
+        number of pseudo-spots.
+    pseudo_spot_min_cell : int
+        minimum value of cells in pseudo-spot.
+    pseudo_spot_max_cell : int
+        maximum value of cells in pseudo-spot.
+    seq_depth_scaler : int
+        a scaler of scRNA-seq sequencing depth.
+    cvae_input_scaler : int
+        maximum value of the scaled input for CVAE.
+    cvae_init_lr : float
+        initial learning rate for training CVAE.
+    num_hidden_layer : int
+        number of hidden layers in encoder and decoder.
+    use_fdr : bool
+        whether to use FDR adjusted p value for filtering and sorting.
+    p_val_cutoff : float
+        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering.
+    fc_cutoff : float
+        threshold of fold change (without log transform!) in marker genes filtering.
+    pct1_cutoff : float
+        threshold of pct.1 in marker genes filtering.
+    pct2_cutoff : float
+        threshold of pct.2 in marker genes filtering.
+    sortby_fc : bool
+        whether to sort marker genes by fold change.
+    diagnosis : bool
+        if True save more information to files for diagnosis CVAE and hyper-parameter selection.
+    rerun_DE : bool, optional
+        whether to rerun DE on the CVAE transformed scRNA-seq data, since the DE genes might be different with before CVAE transforming.
+    filter_gene : bool
+        whether to filter genes before DE.
+    
+
+    Returns
+    -------
+    spatial_transformed_numi : dataframe
+        CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes).
+    scRNA_decode_avg_df : dataframe
+        CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes).
+    new_markers : list or None
+        marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE (rerun_DE=False).
+    '''
+    
+    assert((scRNA_df.index == scRNA_celltype.index).all())
+    assert((spatial_df.columns == scRNA_df.columns).all())
+    
+    # some settings
+    # max number of pseudo spots (training+validation, without training single cells)
+    n_max_pseudo_spots = n_pseudo_spot
+    # scaler to multiply the normalized gene values and transform back to raw nUMI counts
+    depth_scaler = seq_depth_scaler
+    # percentage of training pseudo spots
+    training_pct = 0.8
+    # max value when scaling the input gene expression of CVAE, while min is 0
+    input_max = cvae_input_scaler
+    # first log transform, then minmax scaling
+    use_log_transform = True
+    
+    # the order of celltypes matters, unify the order throughout whole pipeline, which will be determined here
+    celltype_order = sorted(list(scRNA_celltype.celltype.unique()))
+    n_celltype = len(celltype_order)
+    celltype_count_dict = scRNA_celltype.celltype.value_counts().to_dict()
+    
+    
+    # Randomly select cells into pseudo-spots, at most X pseudo-spots
+    # total number of generated pseudo-spots (including training and validation pseudo-spots, NOT include scRNA-seq cells)
+    n_spot_scrna = int(min(100 * spatial_df.shape[0] * n_celltype, n_max_pseudo_spots))
+    n_train_spot_scrna = int(np.floor(n_spot_scrna * training_pct))
+    n_valid_spot_scrna = int(n_spot_scrna - n_train_spot_scrna)
+    print(f'generate {n_spot_scrna} pseudo-spots containing {pseudo_spot_min_cell} to {pseudo_spot_max_cell} cells from scRNA-seq cells...')
+    # pseudo-spot gene expression (pseudo-spots * genes; NO scRNA-seq cells at the end)
+    # pseudo-spot cell-type proportions (pseudo-spots * cell-types; NO scRNA-seq cells at the end)
+    # number of cells in pseudo-spots (NO scRNA-seq cells at the end)
+    pseudo_spots_df, pseudo_spots_celltype_prop, n_cell_in_spot = generate_pseudo_spots(scRNA_df, scRNA_celltype, n_spot_scrna, celltype_order, pseudo_spot_min_cell, pseudo_spot_max_cell)
+    
+    # convert scRNA-seq cell-type annotation to proportions
+    scrna_cell_celltype_prop = celltype2props(scRNA_celltype, celltype_order)
+    
+    
+    # generate pseudo-spots by combining spatial spots
+    n_spot_spatial = int(0.5 * n_spot_scrna)
+    n_train_spot_spatial = int(np.floor(n_spot_spatial * training_pct))
+    n_valid_spot_spatial = int(n_spot_spatial - n_train_spot_spatial)
+    print(f'generate {n_spot_spatial} pseudo-spots containing 2 to 6 spots from spatial spots...')
+    pseudo_spatial_df = combine_spatial_spots(spatial_df, n_spot_spatial, 2, 6)
+    
+    
+    if use_log_transform:
+        # since the input dataframe is extracted from AnnData object, and will not be used in downstream analysis (we can extract from AnnData again), it's safe to modify them directly here
+        print('\nWARNING: first apply log transformation on sequencing depth normalized gene expressions, followed by Min-Max scaling')
+        spatial_df = np.log1p(spatial_df)
+        if pseudo_spots_df.shape[0] > 0:
+            pseudo_spots_df = np.log1p(pseudo_spots_df)
+        if pseudo_spatial_df.shape[0] > 0:
+            pseudo_spatial_df = np.log1p(pseudo_spatial_df)
+        # do not forget scRNA_df
+        scRNA_df = np.log1p(scRNA_df)
+    
+    
+    # Build training and validation data
+    # first spots used for validation, rest spots used for training
+    print(f'\n{"" : <24} | {"training": >9} | {"validation": >9}')
+    print(f'{"spatial spots" : <24} | {spatial_df.shape[0]: >9} | {0: >9}')
+    print(f'{"spatial pseudo-spots" : <24} | {n_train_spot_spatial: >9} | {n_valid_spot_spatial: >9}')
+    print(f'{"scRNA-seq cells" : <24} | {scRNA_df.shape[0]: >9} | {0: >9}')
+    print(f'{"scRNA-seq pseudo-spots" : <24} | {n_train_spot_scrna: >9} | {n_valid_spot_scrna: >9}\n')
+    
+    train_scrna_df = pd.concat([pseudo_spots_df.iloc[n_valid_spot_scrna:,:], scRNA_df], ignore_index=False)
+    valid_scrna_df = pseudo_spots_df.iloc[:n_valid_spot_scrna,:]
+    
+    train_spatial_df = pd.concat([pseudo_spatial_df.iloc[n_valid_spot_spatial:,:], spatial_df], ignore_index=False)
+    valid_spatial_df = pseudo_spatial_df.iloc[:n_valid_spot_spatial,:]
+    
+    assert train_scrna_df.shape[0] == (n_train_spot_scrna + scRNA_df.shape[0])
+    assert valid_scrna_df.shape[0] == n_valid_spot_scrna
+    assert train_spatial_df.shape[0] == (n_train_spot_spatial + spatial_df.shape[0])
+    assert valid_spatial_df.shape[0] == n_valid_spot_spatial
+    
+    # scaling to [0,input_max] with each dataset separately
+    # use only spatial spots + spatial pseudo-spots for spatial dataset scaling
+    print(f'scaling inputs to range 0 to {input_max}')
+    spatial_min_max_scaler = MinMaxScaler(feature_range=[0, input_max])
+    train_spatial_data = spatial_min_max_scaler.fit_transform(train_spatial_df)
+    if valid_spatial_df.shape[0] > 0:
+        valid_spatial_data = spatial_min_max_scaler.transform(valid_spatial_df)
+    else:
+        valid_spatial_data = valid_spatial_df.values
+    
+    # use only training pseudo spots + single cells for scRNA-seq dataset scaling
+    scRNA_min_max_scaler = MinMaxScaler(feature_range=[0, input_max])
+    train_scrna_data = scRNA_min_max_scaler.fit_transform(train_scrna_df)
+    if valid_scrna_df.shape[0] > 0:
+        valid_scrna_data = scRNA_min_max_scaler.transform(valid_scrna_df)
+    else:
+        valid_scrna_data = valid_scrna_df.values
+    
+    
+    # first spatial pseudo-spots then spatial spots then scRNA-seq pseudo-spots and scRNA-seq cells in data
+    # we also consider whether to duplicate spatial data since they are few
+    oversample_scale = 1
+    data = np.vstack((np.tile(train_spatial_data, (oversample_scale, 1)), train_scrna_data))
+    labels = np.array([input_max]*train_spatial_data.shape[0]*oversample_scale + [0.]*train_scrna_data.shape[0])
+    labels = labels.reshape((len(labels), 1))
+    
+    # validation data
+    valid_data = np.vstack((valid_spatial_data, valid_scrna_data))
+    valid_labels = np.array([input_max]*valid_spatial_data.shape[0] + [0.]*valid_scrna_data.shape[0])
+    valid_labels = valid_labels.reshape((len(valid_labels), 1))
+    
+    
+    # re-weight spatial data to make sure the sample size equals spatial:scRNA = 1:10
+    sample_weight = np.ones((data.shape[0],))
+
+    if train_spatial_df.shape[0] < 0.1 * train_scrna_data.shape[0]:
+        # spatial data are located in first part
+        sample_weight[:train_spatial_df.shape[0]] *= 0.1 * train_scrna_data.shape[0] / train_spatial_df.shape[0]
+    
+    del train_spatial_data, valid_spatial_data, train_scrna_data, valid_scrna_data
+    del train_spatial_df, valid_spatial_df, train_scrna_df, valid_scrna_df
+    
     
+    # Define CVAE
+    # number of nodes in input layer (equals number of celltypes)
+    p = data.shape[1]
+    # number of nodes in conditional node
+    p_cond = 1
+    # Hyper-parameters
+    latent_dim = n_celltype * 3
+    # use geometric mean of latent and input dimension (a geometric progression)
+    hidden_dim = list(np.floor(np.geomspace(latent_dim, p, num_hidden_layer+2)[1:num_hidden_layer+1]).astype('int'))
+    
+    print('\nCVAE structure:')
+    print(f'Encoder: {" - ".join([str(x) for x in ([p+p_cond] + hidden_dim[::-1] + [latent_dim])])}')
+    print(f'Decoder: {" - ".join([str(x) for x in ([latent_dim+p_cond] + hidden_dim + [p])])}\n')
+    
+    # note hidden layer in encoder is a reverse of the hidden_dim variable
+    cvae, new_decoder = CVAE_keras_model(p, p_cond, latent_dim, hidden_dim[::-1], hidden_dim, use_batch_norm=True, cvae_init_lr=cvae_init_lr)
+    
+    # learning rate decay
+    lrate = ReduceLROnPlateau(monitor='val_loss', factor=0.9, patience=10, min_lr=5e-4, cooldown=5, verbose=False)
     
     # early stopping based on validation loss
-    early_stop = EarlyStopping(monitor='val_loss', min_delta=0, patience=50, restore_best_weights=True, verbose=False)
+    early_stop = EarlyStopping(monitor='val_loss', min_delta=0, patience=30, restore_best_weights=True, verbose=False)
     
     
     # change tensorflow seed value, set the same seed value for sampling samples from latent space to decoder before training
     # still has unknown randomness source even set seed here...
     set_random_seed(1154)
     
     # Train CVAE
-    print('\nStart training...\n')
-    history_callback = cvae.fit([data, labels], data,
+    # note when there is no pseudo-spots, then there is no validation data
+    if valid_data.shape[0] == 0:
+        print('\nStart training without validation data...\n')
+        history_callback = cvae.fit([data, labels], data,
+                                epochs=500,
+                                batch_size=16384,
+                                shuffle=True,
+                                callbacks=[lrate, early_stop],
+                                sample_weight=sample_weight,
+                                verbose=True)
+    else:
+         print('\nStart training...\n')
+         history_callback = cvae.fit([data, labels], data,
                                 validation_data=([valid_data, valid_labels], valid_data),
-                                epochs=1000,
-                                batch_size=data.shape[0],
-                                shuffle=False,
+                                epochs=500,
+                                batch_size=16384,
+                                shuffle=True,
                                 callbacks=[lrate, early_stop],
                                 sample_weight=sample_weight,
                                 verbose=True)
     
     n_epoch = len(history_callback.history['loss'])
     
-    if n_epoch < 1000:
+    if n_epoch < 500:
         print(f'\ntraining finished in {n_epoch} epochs (early stop), transform data to adjust the platform effect...\n')
     else:
         print(f'\ntraining finished in {n_epoch} epochs (reach max pre-specified epoches), transform data to adjust the platform effect...\n')
 
     
     # postprocess the trained models
     # Subset the encoder
     encoder = Model([cvae.get_layer('encoder_input').input, cvae.get_layer('cond_input').input],
                     [cvae.get_layer('z_mean').output, cvae.get_layer('z_log_var').output],
                     name='encoder')
     
-    # Subset the decoder (build another new decoder and re-store weights)
-    def build_new_decoder(p, p_cond, latent_dim):
-        latent_inputs = Input(shape=(latent_dim,), name='z_sampling')
-        cond_input = Input(shape=(p_cond,), name='conditions')
-        latent_plus_cond = concatenate([latent_inputs, cond_input])
-        # hidden layer 1
-        decoder_hidden = Dense(hidden_dim, use_bias=True, name='decoder_layer1_w')(latent_plus_cond)
-        #decoder_hidden = BatchNormalization(name='decoder_layer1_BN')(decoder_hidden)
-        decoder_hidden = Activation('elu', name='decoder_layer1_act')(decoder_hidden)
-        # output layer
-        decoder_hidden = Dense(p, use_bias=True, name='decoder_output_w')(decoder_hidden)
-        #decoder_hidden = BatchNormalization(name='decoder_output_BN')(decoder_hidden)
-        decoder_output = Activation('relu', name='decoder_output_act')(decoder_hidden)
-    
-        new_decoder = Model([latent_inputs, cond_input], decoder_output, name='new_decoder')
-        return new_decoder
-
-    new_decoder = build_new_decoder(p, p_cond, latent_dim)
-    for layer_name in layer_names:
-        new_decoder.get_layer(layer_name).set_weights(cvae.get_layer(layer_name).get_weights())
+    # update layer weights for the decoder
+    for layer in new_decoder.layers:
+        if layer.name.endswith('w') or layer.name.endswith('BN'):
+            new_decoder.get_layer(layer.name).set_weights(cvae.get_layer(layer.name).get_weights())
     
+    '''
+    # double check decoder is correct
+    from utils import check_decoder
+    check_decoder(cvae, new_decoder, data, labels)
+    '''
     
     # Transform data to adjust platform effect
+    # note if log transform is applied, the data in spatial_df, pseudo_spatial_df, scRNA_df and pseudo_spots_df are already log transformed
+    
     # Decoder output of transformed latent embedding of spatial spot-level data
     spatial_embed = encoder.predict([spatial_min_max_scaler.transform(spatial_df), np.full((spatial_df.shape[0],1), input_max)])[0]
     
     tmp_output = new_decoder.predict([spatial_embed, np.full((spatial_embed.shape[0],1), 0)])
     
-    spatial_transformed_df = pd.DataFrame(np.rint(scRNA_min_max_scaler.inverse_transform(tmp_output) * depth_scaler),
+    spatial_transformed_df = pd.DataFrame(scRNA_min_max_scaler.inverse_transform(tmp_output),
                                           columns=spatial_df.columns,
                                           index=spatial_df.index)
+    
+    # log transformation back
+    if use_log_transform:
+        print('WARNING: when transforming data, after reversed Min-Max Scaling, apply exp transformation then multiple the factor and round to integer')
+        spatial_transformed_df = np.expm1(spatial_transformed_df)
+        
+    spatial_transformed_numi = np.rint(spatial_transformed_df * depth_scaler)
 
     
     # Decoder output of average marker gene expression of scRNA-seq cell-types
     scRNA_embed = encoder.predict([scRNA_min_max_scaler.transform(scRNA_df), np.full((scRNA_df.shape[0],1), 0)])[0]
     
     # decode it
     tmp_output = new_decoder.predict([scRNA_embed, np.full((scRNA_embed.shape[0],1), 0)])
     
     scRNA_decode_df = pd.DataFrame(scRNA_min_max_scaler.inverse_transform(tmp_output),
                                    columns=scRNA_df.columns,
                                    index=scRNA_df.index)
     
+    # log transformation back
+    if use_log_transform:
+        scRNA_decode_df = np.expm1(scRNA_decode_df)
+    
     # whether to rerun DE
     if rerun_DE:
         print('\nre-run DE on CVAE transformed scRNA-seq data!')
         from utils import rerun_DE
         new_markers = rerun_DE(scRNA_decode_df, scRNA_celltype, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_gene)
     else:
         new_markers = None
     
     # take average for all genes
-    scRNA_decode_df['celltype'] = scRNA_celltype.celltype
-    scRNA_decode_df = scRNA_decode_df.groupby(['celltype']).mean()
+    scRNA_decode_avg_df = scRNA_decode_df.copy()
+    scRNA_decode_avg_df['celltype'] = scRNA_celltype.celltype
+    scRNA_decode_avg_df = scRNA_decode_avg_df.groupby(['celltype']).mean()
+    
+    # re-order the rows to match the previous defined cell-type order
+    scRNA_decode_avg_df = scRNA_decode_avg_df.loc[celltype_order, :]
+    
     
     # whether to save models and transformed data
     if diagnosis:
-        print('\nsave variables related to CVAE to files!')
-        spatial_transformed_df.to_csv(os.path.join(output_path, 'spatial_spots_transformToscRNA_decoded.csv'))
-        scRNA_decode_df.to_csv(os.path.join(output_path, 'scRNA_decoded_avg_exp_bycelltypes.csv'))
-        cvae.save(os.path.join(output_path, 'CVAE_whole.h5'))
-        encoder.save(os.path.join(output_path, 'CVAE_encoder.h5'))
-        new_decoder.save(os.path.join(output_path, 'CVAE_decoder.h5'))
-        
-        
-        # plot variance of mu of spatial spots and scRNA-seq cells
-        import matplotlib
-        import matplotlib.pyplot as plt
-        import seaborn as sns
-        sns.set()
-        
-        latent_var = np.concatenate((spatial_embed, scRNA_embed), axis=0).var(axis=0)
-        plt.figure()
-        ax = sns.histplot(x=np.log10(latent_var))
-        ax.set(xlabel='log10(var(mu))')
-        plt.savefig(os.path.join(output_path, 'histogram of variance of latent neurons on spatial spots and scRNA-seq cells.png'))
-        plt.close()
-        
-        
-        # plot histogram of transformed spots nUMI sum
-        plt.figure()
-        ax = sns.histplot(x=np.sum(spatial_transformed_df.values, axis=1))
-        ax.set(xlabel='Sum of nUMI per spatial spot after transformation')
-        plt.savefig(os.path.join(output_path, 'histogram of sum of nUMI of spatial spots after transformation.png'))
-        plt.close()
-        
-        
-        # plot zero percentage of marker genes in spatial spots after transformation
-        plt.figure()
-        if new_markers is None:
-            tmp_mtx = spatial_transformed_df.values
+        
+        # also embed pseudo-spots for diagnosis
+        if n_spot_spatial == 0:
+            pseudo_spatial_embed = np.empty((0, spatial_embed.shape[1]))
         else:
-            tmp_mtx = spatial_transformed_df.loc[:, new_markers].values
-        ax = sns.histplot(x=np.sum(tmp_mtx==0, axis=1)/tmp_mtx.shape[1])
-        ax.set(xlabel=f'Zero percentage of {tmp_mtx.shape[1]} genes per spot after transformation')
-        ax.set_xlim(xmin=0, xmax=1)
-        plt.savefig(os.path.join(output_path, 'histogram of zero percentage of spatial spots after transformation.png'))
-        plt.close()
-        
-        
-        # plot umap of spatial spots and scRNA-seq cells plus pseudo spots
-        import umap
-        from distinctipy import distinctipy
-        
-        # embed of decoded average marker gene expression
-        marker_embed = encoder.predict([scRNA_min_max_scaler.transform(scRNA_decode_df), np.full((scRNA_decode_df.shape[0],1), 0)])[0]
-        
-        pseudo_spot_embed = encoder.predict([scRNA_min_max_scaler.transform(pseudo_spots_df.iloc[:n_spot, :]), np.full((n_spot,1), 0)])[0]
-        
-        # the order will affect the point overlay, first row draw first
-        # umap has embeded seed (default 42), by specify random_state, umap will use special mode to keep reproducibility
-        all_umap = umap.UMAP(random_state=42).fit_transform(np.concatenate((pseudo_spot_embed, scRNA_embed, marker_embed, spatial_embed), axis=0))
-        
-        # add cell/spot count in the annotation
-        plot_df = pd.DataFrame({'UMAP1': all_umap[:, 0],
-                                'UMAP2': all_umap[:, 1],
-                                'celltype': ['pseudo']*n_spot + [f'{x} ({celltype_count_dict[x]})' for x in scRNA_celltype.celltype.to_list()] + [f'{x} ({celltype_count_dict[x]})' for x in scRNA_decode_df.index.to_list()] + [f'spatial ({spatial_df.shape[0]})']*spatial_df.shape[0],
-                                'dot_type': ['pseudo spot']*n_spot + ['cell']*scRNA_df.shape[0] + ['marker']*scRNA_decode_df.shape[0] + ['spatial spot']*spatial_df.shape[0],
-                                'dataset': ['scRNA-seq']*(scRNA_df.shape[0]+scRNA_decode_df.shape[0]+n_spot) + ['spatial']*spatial_df.shape[0]
-                                },
-                               index = [f'pseudo{x}' for x in range(n_spot)] + scRNA_df.index.to_list() + [f'{x}-marker' for x in scRNA_decode_df.index.to_list()] + spatial_df.index.to_list())
-        
-        plot_sizes = {'cell': 20, 'spatial spot': 20, 'marker': 200, 'pseudo spot': 20}
-        plot_markers = {'cell': 'o', 'spatial spot': 'o', 'marker': 'X', 'pseudo spot': 'o'}
-        plot_colors = {}
-        for one_celltype, one_color in zip([f'spatial ({spatial_df.shape[0]})']+[f'{x} ({celltype_count_dict[x]})' for x in celltypes], distinctipy.get_colors(n_celltype+1)):
-            plot_colors[one_celltype] = one_color
-        # assign pseudo spots as gray80
-        plot_colors['pseudo'] = '#cccccc'
-        
-        #plt.figure(figsize=(6.4*2*2, 4.8*2))
-        sns.set_style("darkgrid")
-        
-        # relplot return a FacetGrid object
-        # specify figure size by Height (in inches) of each facet, and Aspect ratio of each facet
-        fgrid = sns.relplot(data=plot_df, x='UMAP1', y='UMAP2', hue='celltype', size='dot_type', style='dot_type', sizes=plot_sizes, markers=plot_markers, palette=plot_colors, kind='scatter', col='dataset', col_order=['scRNA-seq', 'spatial'], height=4.8*2, aspect=6.4/4.8)
-        fgrid.set(xlabel='Embedding Dimension 1', ylabel='Embedding Dimension 2')
-        # Put the legend out of the figure
-        #ax.legend(loc='center left', bbox_to_anchor=(1, 0.5))
-        
-        # add cell-type annotations around marker coordinates
-        # adjustText do not support seaborn relplot
-        #from adjustText import adjust_text
-        # fgrid.axes return an array of all axes in the figure
-        ax = fgrid.axes[0, 0]
-        texts = []
-        sub_plot_df = plot_df.loc[plot_df['dot_type']=='marker']
-        for one_row in sub_plot_df.index:
-            texts.append(ax.text(sub_plot_df.at[one_row, 'UMAP1'], sub_plot_df.at[one_row, 'UMAP2'], sub_plot_df.at[one_row, 'celltype'].split(' (')[0], weight='bold'))
-        #adjust_text(texts)
-        plt.savefig(os.path.join(output_path, 'UMAP of spatial spots and scRNA-seq cells with markers.png'))
-        plt.close()
-        
-        
-        # plot distribution of number of cells in pseudo-spots
-        # first n_spot + #scRNA-seq cells of the records are just the pseudo-spots + scRNA-seq data, with the row order matches
-        tmp_df = plot_df.iloc[:(n_spot+scRNA_df.shape[0]), :]
-        tmp_df = tmp_df.assign(n_cell_in_spot = n_cell_in_spot)
-     
-        # generate a colormap with a specified color for NA (spatial spots), but not work for relplot...
-        #my_cmap = sns.color_palette("viridis", as_cmap=True)
-        #my_cmap.set_bad(color=plot_colors[f'spatial ({spatial_df.shape[0]})'])
-        
-        # show the full legend of colorbar in relplot, otherwise it will only show a sample of evenly spaced values (The FacetGrid hue is categorical, not continuous)
-        #fgrid = sns.relplot(data=tmp_df, x='UMAP1', y='UMAP2', hue='#cell_in_spot', palette='viridis', kind='scatter', col='dataset', col_order=['scRNA-seq', 'spatial'], height=4.8*2, aspect=6.4/4.8, legend='full')
-        #fgrid.set(xlabel='Embedding Dimension 1', ylabel='Embedding Dimension 2')
-        
-        # instead use plt.subplots
-        fig, (ax1, ax2) = plt.subplots(1, 2, sharey=True, sharex=True, figsize=(6.4*4, 4.8*2))
-        # left panel: scatter plot of pseudo-spots
-        sc = ax1.scatter(tmp_df['UMAP1'], tmp_df['UMAP2'], c=tmp_df['n_cell_in_spot'], cmap='cubehelix', s=10, marker='o')
-        ax1.set_title('dataset = scRNA-seq')
-        ax1.set_xlabel('Embedding Dimension 1')
-        ax1.set_ylabel('Embedding Dimension 2')
-        
-        # right panel: scatter plot of spatial spots
-        tmp_df = plot_df.loc[plot_df['dot_type']=='spatial spot', :]
-        ax2.scatter(tmp_df['UMAP1'], tmp_df['UMAP2'], color=plot_colors[f'spatial ({spatial_df.shape[0]})'], s=10, marker='o')
-        ax2.set_title('dataset = spatial')
-        ax2.set_xlabel('Embedding Dimension 1')
-        ax2.set_ylabel('Embedding Dimension 2')
-        
-        # add colorbar with title to the most right (https://stackoverflow.com/questions/13784201/how-to-have-one-colorbar-for-all-subplots, conflict with tight_layout)
-        cbar = fig.colorbar(sc, ax=ax2)
-        cbar.ax.set_title('#cell in spot')
-        
-        fig.tight_layout()
-        fig.savefig(os.path.join(output_path, 'distribution of number of cells in pseudo-spots.png'))
-        plt.close()
-        
-        
-        # plot distribution of cell-type proportions of each cell-type
-        # tried to use PDF format, but encountered error TeX capacity exceeded, since too many dots in figure
-        for this_celltype in celltypes:
-            # first n_spot + #scRNA-seq cells of the records are just the pseudo-spots + scRNA-seq data, with the row order matches
-            tmp_df = plot_df.iloc[:(n_spot+scRNA_df.shape[0]), :]
-            # don't forget the .values
-            tmp_df = tmp_df.assign(proportion = pseudo_spots_celltype[this_celltype].values)
-            
-            # start to plot
-            fig, axes = plt.subplots(1, 2, sharey=True, sharex=True, figsize=(6.4*4, 4.8*2))
-            (ax1, ax2) = axes.flat
-            # left panel: scatter plot of pseudo-spots
-            sc = ax1.scatter(tmp_df['UMAP1'], tmp_df['UMAP2'], c=tmp_df['proportion'], cmap='cubehelix', s=10, marker='o', norm=matplotlib.colors.Normalize(vmin=0, vmax=1))
-            # plot marker gene profiles with different marker also color (same color is hard to recognize the cross)
-            ax1.scatter(plot_df.at[f'{this_celltype}-marker', 'UMAP1'], plot_df.at[f'{this_celltype}-marker', 'UMAP2'], color='red', s=120, marker='X')
-            ax1.set_title('dataset = scRNA-seq')
-            ax1.set_xlabel('Embedding Dimension 1')
-            ax1.set_ylabel('Embedding Dimension 2')
-            
-            # right panel: scatter plot of spatial spots
-            # interpolate the grid for contour plot
-            from scipy.interpolate import griddata
-            grid_x, grid_y = np.mgrid[tmp_df['UMAP1'].min():tmp_df['UMAP1'].max():0.025, tmp_df['UMAP2'].min():tmp_df['UMAP2'].max():0.025]
-            grid_z = griddata(tmp_df.loc[:, ['UMAP1', 'UMAP2']].values, tmp_df['proportion'].values, (grid_x, grid_y), method='linear',  fill_value=np.nan)
-            
-            try:
-                ax2.contourf(grid_x, grid_y, grid_z, cmap='cubehelix', norm=matplotlib.colors.Normalize(vmin=0, vmax=1), alpha=0.3)
-            except:
-                pass
-            
-            tmp_df2 = plot_df.loc[plot_df['dot_type']=='spatial spot', :]
-            ax2.scatter(tmp_df2['UMAP1'], tmp_df2['UMAP2'], color=plot_colors[f'spatial ({spatial_df.shape[0]})'], s=10, marker='o')
-            ax2.set_title('dataset = spatial')
-            ax2.set_xlabel('Embedding Dimension 1')
-            ax2.set_ylabel('Embedding Dimension 2')
-            
-            # add colorbar with title
-            cbar = fig.colorbar(sc, ax=ax2)
-            cbar.ax.set_title('proportion')
-            
-            fig.suptitle(this_celltype)
-            
-            fig.tight_layout()
-            
-            # make sure the file name is valid
-            fig.savefig(os.path.join(output_path, f'distribution of {"".join(x for x in this_celltype if (x.isalnum() or x in "._- "))} proportions.png'))
-            plt.close()
+            pseudo_spatial_embed = encoder.predict([spatial_min_max_scaler.transform(pseudo_spatial_df), np.full((pseudo_spatial_df.shape[0],1), input_max)])[0]
         
+        if n_spot_scrna == 0:
+            pseudo_spot_embed = np.empty((0, scRNA_embed.shape[1]))
+        else:
+            pseudo_spot_embed = encoder.predict([scRNA_min_max_scaler.transform(pseudo_spots_df), np.full((pseudo_spots_df.shape[0],1), 0)])[0]
         
-        # save spatial spot UMAP coordinates
-        plot_df.loc[plot_df['dot_type']=='spatial spot', ['UMAP1', 'UMAP2']].to_csv(os.path.join(output_path, 'spatial spots UMAP coordinates.csv'))
-        # save scRNA-seq cells UMAP coordinates
-        plot_df.loc[plot_df['dot_type']=='cell', ['UMAP1', 'UMAP2']].to_csv(os.path.join(output_path, 'scRNA-seq cells UMAP coordinates.csv'))
-    
+        
+        from diagnosis_plots import diagnosisCVAE
+        diagnosisCVAE(cvae, encoder, new_decoder,
+                      spatial_embed, spatial_transformed_df, spatial_transformed_numi, pseudo_spatial_embed,
+                      scRNA_celltype, celltype_order, celltype_count_dict, scrna_cell_celltype_prop, scRNA_embed,
+                      pseudo_spots_celltype_prop, n_cell_in_spot, pseudo_spot_embed,
+                      scRNA_decode_df, scRNA_decode_avg_df, new_markers)
+
+
     #print(f'before CVAE building function return RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
     
-    return spatial_transformed_df, scRNA_decode_df, new_markers
+    return spatial_transformed_numi, scRNA_decode_avg_df, new_markers
 
 
 
-def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene):
+def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene):
     '''
     read related CSV files, build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
@@ -602,52 +782,56 @@
     ref_anno_file : string
         full path of input csv file of cell-type annotations for all cells in scRNA-seq data.
     marker_file : string
         full path of input csv file of cell-typee marker gene expression (cell-types * genes).
     n_hv_gene : int
         number of highly variable genes for CVAE.
     n_marker_per_cmp : int
-        number of TOP marker genes for each comparison in DE
+        number of TOP marker genes for each comparison in DE.
+    n_pseudo_spot : int
+        number of pseudo-spots.
     pseudo_spot_min_cell : int
-        minimum value of cells in pseudo-spot
+        minimum value of cells in pseudo-spot.
     pseudo_spot_max_cell : int
-        maximum value of cells in pseudo-spot
+        maximum value of cells in pseudo-spot.
     seq_depth_scaler : int
-        a scaler of scRNA-seq sequencing depth
+        a scaler of scRNA-seq sequencing depth.
     cvae_input_scaler : int
-        maximum value of the scaled input for CVAE
+        maximum value of the scaled input for CVAE.
     cvae_init_lr : float
-        initial learning rate for training CVAE
+        initial learning rate for training CVAE.
+    num_hidden_layer : int
+        number of hidden layers in encoder and decoder.
     redo_de : bool
-        whether to redo DE after CVAE transformation
+        whether to redo DE after CVAE transformation.
     use_fdr : bool
-        whether to use FDR adjusted p value for filtering and sorting
+        whether to use FDR adjusted p value for filtering and sorting.
     p_val_cutoff : float
-        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering
+        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering.
     fc_cutoff : float
-        threshold of fold change (without log transform!) in marker genes filtering
+        threshold of fold change (without log transform!) in marker genes filtering.
     pct1_cutoff : float
-        threshold of pct.1 in marker genes filtering
+        threshold of pct.1 in marker genes filtering.
     pct2_cutoff : float
-        threshold of pct.2 in marker genes filtering
+        threshold of pct.2 in marker genes filtering.
     sortby_fc : bool
-        whether to sort marker genes by fold change
+        whether to sort marker genes by fold change.
     diagnosis : bool
-        if True save more information to files for diagnosis CVAE and hyper-parameter selection
+        if True save more information to files for diagnosis CVAE and hyper-parameter selection.
     filter_cell : bool
-        whether to filter cells before DE
+        whether to filter cells before DE.
     filter_gene : bool
-        whether to filter genes before DE
+        whether to filter genes before DE.
 
     Returns
     -------
-    spatial_transformed_df : dataframe
-        CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes)
-    scRNA_decode_df : dataframe
-        CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes)
+    spatial_transformed_numi : dataframe
+        CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes).
+    scRNA_decode_avg_df : dataframe
+        CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes).
     new_markers : list or None
         marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE.
     '''
     
     start_time = time()
     
     # read spatial data
@@ -700,30 +884,32 @@
             print(f'from user specified marker gene expression use {len(marker_genes)} marker genes overlapped with spatial + scRNA-seq data')
             # if len(marker_genes) < len(overlap_genes):
             #     print(f'{len(overlap_genes)-len(marker_genes)} genes in overlapped gene list between spatial and scRNA-seq data but not found in user provided marker gene expression: {", ".join(set(overlap_genes).difference(set(marker_genes)))}\n')
             
         else:
             # perform DE, return the marker gene expression
             print('no marker gene profile provided. Perform DE to get cell-type marker genes on scRNA-seq data...\n')
-            marker_genes = run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, 'DE celltype markers.csv')
+            marker_genes = run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, 'DE_celltype_markers.csv')
         
         # final gene list for downstream analysis
         final_gene_list = sorted(list(set(scrna_hv_genes).union(set(marker_genes))))
         print(f'\nuse union of highly variable gene list and cell-type marker gene list derived from scRNA-seq data, finally get {len(final_gene_list)} genes for downstream analysis')
     
     
     print('\nstart CVAE building...\n')
     scrna_celltype = sc.get.obs_df(scrna_obj, keys='celltype').to_frame()
     scrna_celltype['celltype'] = scrna_celltype['celltype'].astype(str)
     
     # build CVAE
-    spatial_df, scrna_avg_df, new_markers = build_CVAE(sc.get.obs_df(spatial_spot_obj, keys=final_gene_list),
-                                          sc.get.obs_df(scrna_obj, keys=final_gene_list),
-                                          scrna_celltype,
-                                          n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler,
-                                          cvae_input_scaler, cvae_init_lr,
-                                          use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc,
-                                          diagnosis, rerun_DE=redo_de, filter_gene=filter_gene)
+    (spatial_transformed_numi,
+     scRNA_decode_avg_df,
+     new_markers) = build_CVAE(sc.get.obs_df(spatial_spot_obj, keys=final_gene_list),
+                               sc.get.obs_df(scrna_obj, keys=final_gene_list),
+                               scrna_celltype,
+                               n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler,
+                               cvae_input_scaler, cvae_init_lr, num_hidden_layer,
+                               use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc,
+                               diagnosis, rerun_DE=redo_de, filter_gene=filter_gene)
     
     print(f'\nplatform effect adjustment by CVAE finished. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n\n')
     
-    return spatial_df, scrna_avg_df, new_markers
+    return spatial_transformed_numi, scRNA_decode_avg_df, new_markers
```

### Comparing `sdeper-1.1.0/src/cvaeglrm.py` & `sdeper-1.2.0/src/cvaeglrm.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
     session_conf = tf.compat.v1.ConfigProto(intra_op_parallelism_threads=paramdict['n_cores'], inter_op_parallelism_threads=paramdict['n_cores'])
     sess = tf.compat.v1.Session(graph=tf.compat.v1.get_default_graph(), config=session_conf)
     tf.compat.v1.keras.backend.set_session(sess)
     
     
     print('\n\n######### Preprocessing... #########\n')
-    data = preprocess(paramdict['spatial_file'], paramdict['ref_file'], paramdict['ref_celltype_file'], paramdict['marker_file'], paramdict['A_file'], paramdict['use_cvae'], paramdict['n_hv_gene'], paramdict['n_marker_per_cmp'], paramdict['pseudo_spot_min_cell'], paramdict['pseudo_spot_max_cell'], paramdict['seq_depth_scaler'], paramdict['cvae_input_scaler'], paramdict['cvae_init_lr'], paramdict['redo_de'], paramdict['use_fdr'], paramdict['p_val_cutoff'], paramdict['fc_cutoff'], paramdict['pct1_cutoff'], paramdict['pct2_cutoff'], paramdict['sortby_fc'], paramdict['filter_cell'], paramdict['filter_gene'], paramdict['diagnosis'])
+    data = preprocess(paramdict['spatial_file'], paramdict['ref_file'], paramdict['ref_celltype_file'], paramdict['marker_file'], paramdict['A_file'], paramdict['use_cvae'], paramdict['n_hv_gene'], paramdict['n_marker_per_cmp'], paramdict['n_pseudo_spot'], paramdict['pseudo_spot_min_cell'], paramdict['pseudo_spot_max_cell'], paramdict['seq_depth_scaler'], paramdict['cvae_input_scaler'], paramdict['cvae_init_lr'], paramdict['num_hidden_layer'], paramdict['redo_de'], paramdict['use_fdr'], paramdict['p_val_cutoff'], paramdict['fc_cutoff'], paramdict['pct1_cutoff'], paramdict['pct2_cutoff'], paramdict['sortby_fc'], paramdict['filter_cell'], paramdict['filter_gene'], paramdict['diagnosis'])
     
     
     # whether to estimate gamma_g, if CVAE is used then disable gamma_g estimation
     if paramdict['use_cvae']:
         estimate_gamma_g = False
     else:
         estimate_gamma_g = True
```

### Comparing `sdeper-1.1.0/src/hyper_parameter_optimization.py` & `sdeper-1.2.0/src/hyper_parameter_optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,23 @@
     
 in k-fold cross-validation, we random subset the GENEs, then predict the gene expression in validation fold
 the performance metric is RMSE of predicted gene expressions in validation fold
 """
 
 
 
-import os
 import networkx as nx
 import numpy as np
 from scipy import sparse
 from math import floor
 from time import time
 from admm_fit import one_admm_fit
 from local_fit_numba import update_theta, hv_wrapper
 from utils import reportRMSE, calcRMSE
-from config import print, output_path
+from config import print
 
 
 
 def checkEarlyStop(x, num=3):
     '''
     check whether we can early stop hyper-parameter tuning without test on rest candidates
     
@@ -305,35 +304,23 @@
     if use_likelihood:
         print(f'find optimal lambda_r {candidate_list[optimal_idx]:.3f} with average negative log-likelihood {avg_rmse_list[optimal_idx]:.4f} by {k} fold cross-validation. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n')
     else:
         print(f'find optimal lambda_r {candidate_list[optimal_idx]:.3f} with average RMSE {avg_rmse_list[optimal_idx]:.4f} by {k} fold cross-validation. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n')
         
     # draw plot
     if diagnosis:
-        import matplotlib.pyplot as plt
-        import seaborn as sns
-        sns.set()
-        
-        fig, ax = plt.subplots()
-        ax.plot(candidate_list[:len(avg_rmse_list)], avg_rmse_list, marker='o')
-        # log scale do not support 0, so use symlog
-        ax.set_xscale('symlog', linthresh=candidate_list[1])
-        ax.set_xticks(candidate_list)
-        ax.set_xticklabels(candidate_list, rotation=45)
-        ax.axvline(candidate_list[optimal_idx], color='red', linestyle='--')
         
-        ax.set_xlabel('lambda_r')
         if use_likelihood:
-            ax.set_ylabel('average negative log-likelihood')
+            y_label = 'average negative log-likelihood'
         else:
-            ax.set_ylabel('average theta RMSE')
+            y_label = 'average theta RMSE'
+        
+        from diagnosis_plots import diagnosisParamsTuning
+        diagnosisParamsTuning(candidate_list, avg_rmse_list, optimal_idx, 'lambda_r', y_label)
         
-        fig.tight_layout()
-        fig.savefig(os.path.join(output_path, 'tuning lambda_r.png'))
-        plt.close()
 
     return candidate_list[optimal_idx]
     
     
     
 def cv_find_lambda_g(data, G, theta_mask, gamma_g, sigma2, candidate_list, hybrid_version=True, opt_method='L-BFGS-B', hv_x=None, hv_log_p=None, use_admm=True, use_likelihood=True, k=5, use_cache=True, diagnosis=False):
     '''
@@ -531,30 +518,18 @@
     if use_likelihood:
         print(f'find optimal lambda_g {candidate_list[optimal_idx]:.3f} with average negative log-likelihood {avg_rmse_list[optimal_idx]:.4f} by {k} fold cross-validation. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n')
     else:
         print(f'find optimal lambda_g {candidate_list[optimal_idx]:.3f} with average RMSE {avg_rmse_list[optimal_idx]:.4f} by {k} fold cross-validation. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n')
         
     # draw plot
     if diagnosis:
-        import matplotlib.pyplot as plt
-        import seaborn as sns
-        sns.set()
-        
-        fig, ax = plt.subplots()
-        ax.plot(candidate_list[:len(avg_rmse_list)], avg_rmse_list, marker='o')
-        # log scale do not support 0, so use symlog
-        ax.set_xscale('symlog', linthresh=candidate_list[1])
-        ax.set_xticks(candidate_list)
-        ax.set_xticklabels(candidate_list, rotation=45)
-        ax.axvline(candidate_list[optimal_idx], color='red', linestyle='--')
         
-        ax.set_xlabel('lambda_g')
         if use_likelihood:
-            ax.set_ylabel('average negative log-likelihood')
+            y_label = 'average negative log-likelihood'
         else:
-            ax.set_ylabel('average theta RMSE')
+            y_label = 'average theta RMSE'
         
-        fig.tight_layout()
-        fig.savefig(os.path.join(output_path, 'tuning lambda_g.png'))
-        plt.close()
+        from diagnosis_plots import diagnosisParamsTuning
+        diagnosisParamsTuning(candidate_list, avg_rmse_list, optimal_idx, 'lambda_g', y_label)
+    
     
     return candidate_list[optimal_idx]
```

### Comparing `sdeper-1.1.0/src/imputation.py` & `sdeper-1.2.0/src/imputation.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/src/local_fit_numba.py` & `sdeper-1.2.0/src/local_fit_numba.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/src/model_fit.py` & `sdeper-1.2.0/src/model_fit.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/src/parse_opt.py` & `sdeper-1.2.0/src/parse_opt.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 
 # default value for options
 default_paramdict = {'spatial_file': None, 'ref_file': None, 'ref_celltype_file': None, 'marker_file': None, 'loc_file': None, 'A_file': None,
                      'n_cores': 1, 'threshold': 0, 'use_cvae': True, 'use_imputation': False, 'diagnosis': False, 'verbose': True,
                      'use_fdr': True, 'p_val_cutoff': 0.05, 'fc_cutoff': 1.2, 'pct1_cutoff': 0.3, 'pct2_cutoff': 0.1, 'sortby_fc': True, 'n_marker_per_cmp': 10, 'filter_cell': True, 'filter_gene': True,
-                     'n_hv_gene': 200,  'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.003, 'redo_de': True, 'seed': 383,
+                     'n_hv_gene': 200,  'n_pseudo_spot': 500000, 'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.01, 'num_hidden_layer': 2, 'redo_de': True, 'seed': 383,
                      'lambda_r': None, 'lambda_r_range_min': 0.1, 'lambda_r_range_max': 100, 'lambda_r_range_k': 8,
                      'lambda_g': None, 'lambda_g_range_min': 0.1, 'lambda_g_range_max': 100, 'lambda_g_range_k': 8,
                      'diameter': 200, 'impute_diameter': [160, 114, 80]
                     }
 
 
 
@@ -95,19 +95,21 @@
     
     
     --------------- CVAE related options ---------------
     
     We build Conditional Variational Autoencoder (CVAE) to adjust the platform effect between spatial transcriptomic and scRNA-seq data. The input of CVAE includes scRNA-seq cells, pseudo-spots generated by aggregating randomly selected cells and real spatial spots. To successfully train a neural network model is non-trivial, and model Topology together with most related hyper-parameters have been pre-fixed based on our experiences on analysis of various spatial transcriptomic datasets. The options can be tuned by users are listed as below:
     
     --n_hv_gene             number of highly variable genes identified in reference scRNA-seq data, and these HV genes will be used together with identified cell-type marker genes for building CVAE. Default number is {default_paramdict["n_hv_gene"]}. If the actual number of genes in scRNA-seq data is less than the specified value, all available genes in scRNA-seq data will be used for building CVAE.
+    --n_pseudo_spot         maximum number of pseudo-spots generated by randomly combining scRNA-seq cells into one pseudo-spot in CVAE training. Default value is {default_paramdict["n_pseudo_spot"]}.
     --pseudo_spot_min_cell  minimum value of cells in one pseudo-spot when combining cells into pseudo-spots. Default value is {default_paramdict["pseudo_spot_min_cell"]}.
     --pseudo_spot_max_cell  maximum value of cells in one pseudo-spot when combining cells into pseudo-spots. Default value is {default_paramdict["pseudo_spot_max_cell"]}.
     --seq_depth_scaler      a scaler of scRNA-seq sequencing depth to transform CVAE decoded values (sequencing depth normalized gene expressions) back to raw nUMI counts. Default value is {default_paramdict["seq_depth_scaler"]} for all cells.
     --cvae_input_scaler     maximum value of the scaled input for CVAE input layer. Default value is {default_paramdict["cvae_input_scaler"]}, i.e. linearly scale all the sequencing depth normalized gene expressions to range [0, {default_paramdict["cvae_input_scaler"]}].
     --cvae_init_lr          initial learning rate for training CVAE. Default value is {default_paramdict["cvae_init_lr"]}. Although learning rate will decreasing automatically during training, large initial learning rate will cause training failure at the very beginning of training. If loss function value do NOT monotonically decrease, please try smaller initial learning rate.
+    --num_hidden_layer      number of hidden layers in encoder and decoder of CVAE. Default value is {default_paramdict["num_hidden_layer"]}. The number of neurons in each hidden layer will be determined automatically.
     --redo_de               control whether to redo Differential analysis on CVAE transformed scRNA-seq gene expressions to get a new set of marker gene list of cell-types (true/false). Default value is {default_paramdict["redo_de"]}. It's recommended to redo Differential analysis since CVAE transformation may change the marker gene profile of cell-types.
     --seed                  seed value of TensorFlow to control the randomness in building CVAE. Default value is {default_paramdict["seed"]}.
     
     
     -------------- GLRM hyper-parameter related options ---------------
     
     We incorporate adaptive Lasso penalty and graph Laplacian penalty in GLRM, and use the hyper-parameters lambda_r and lambda_g to balance the strength of those two penalties respectively.
@@ -150,19 +152,21 @@
             n_cores : number of CPU cores used for parallel computing\n
             lambda_r : hyper-parameter for Adaptive Lasso\n
             lambda_g : hyper-parameter for graph weight, affecting the Laplacian Matrix\n
             use_cvae : whether to build CVAE\n
             threshold : threshold for hard thresholding estimated cell-type proportion theta\n
             n_hv_gene : number of highly variable genes for CVAE\n
             n_marker_per_cmp : number of TOP marker genes for each comparison in DE\n
+            n_pseudo_spot : number of pseudo-spots\n
             pseudo_spot_min_cell : minimum value of cells in pseudo-spot\n
             pseudo_spot_max_cell : maximum value of cells in pseudo-spot\n
             seq_depth_scaler : a scaler of scRNA-seq sequencing depth\n
             cvae_input_scaler : maximum value of the scaled input for CVAE\n
             cvae_init_lr : initial learning rate for training CVAE\n
+            num_hidden_layer : number of hidden layers in encoder and decoder\n
             redo_de : whether to redo DE after CVAE transformation\n
             seed : seed value for random in building CVAE\n
             diagnosis : True or False, if True save more information to files for diagnosis CVAE and hyper-parameter selection\n
             verbose : True or False, if True print more information during program running\n
             use_fdr : whether to use FDR adjusted p value for filtering and sorting\n
             p_val_cutoff : threshold of p value (or FDR if --use_fdr is true) in marker genes filtering\n
             fc_cutoff : threshold of fold change (without log transform!) in marker genes filtering\n
@@ -182,15 +186,15 @@
         print('Use -h or --help for detailed help!')
         sys.exit(1)
         
     # 定义命令行参数
     # 短选项名后的冒号(:)表示该选项必须有附加的参数
     # 长选项名后的等号(=)表示该选项必须有附加的参数
     shortargs = 'hq:r:c:m:l:a:o:n:v'
-    longargs = ['help', 'query=', 'ref=', 'ref_anno=', 'marker=', 'loc=', 'adjacency=', 'n_cores=', 'lambda_r=', 'lambda_r_range_min=', 'lambda_r_range_max=', 'lambda_r_range_k=', 'lambda_g=', 'lambda_g_range_min=', 'lambda_g_range_max=', 'lambda_g_range_k=', 'use_cvae=', 'threshold=', 'n_hv_gene=', 'n_marker_per_cmp=', 'pseudo_spot_min_cell=', 'pseudo_spot_max_cell=', 'seq_depth_scaler=', 'cvae_input_scaler=', 'cvae_init_lr=', 'redo_de=', 'seed=', 'diagnosis=', 'verbose=', 'use_fdr=', 'p_val_cutoff=', 'fc_cutoff=', 'pct1_cutoff=', 'pct2_cutoff=', 'sortby_fc=', 'filter_cell=', 'filter_gene=', 'use_imputation=', 'diameter=', 'impute_diameter=', 'version']
+    longargs = ['help', 'query=', 'ref=', 'ref_anno=', 'marker=', 'loc=', 'adjacency=', 'n_cores=', 'lambda_r=', 'lambda_r_range_min=', 'lambda_r_range_max=', 'lambda_r_range_k=', 'lambda_g=', 'lambda_g_range_min=', 'lambda_g_range_max=', 'lambda_g_range_k=', 'use_cvae=', 'threshold=', 'n_hv_gene=', 'n_marker_per_cmp=', 'n_pseudo_spot=', 'pseudo_spot_min_cell=', 'pseudo_spot_max_cell=', 'seq_depth_scaler=', 'cvae_input_scaler=', 'cvae_init_lr=', 'num_hidden_layer=', 'redo_de=', 'seed=', 'diagnosis=', 'verbose=', 'use_fdr=', 'p_val_cutoff=', 'fc_cutoff=', 'pct1_cutoff=', 'pct2_cutoff=', 'sortby_fc=', 'filter_cell=', 'filter_gene=', 'use_imputation=', 'diameter=', 'impute_diameter=', 'version']
     
   
     # 解析命令行参数
     # sys.argv[0]为python脚本名，后续全为参数
     # opts为分析出的参数信息，args为不符合格式信息的剩余参数
     opts, args = getopt(sys.argv[1:], shortargs, longargs)
     
@@ -433,14 +437,26 @@
                     print(f'WARNING: non-positive option value `{paramdict["n_marker_per_cmp"]}` for n_marker_per_cmp! Please use positve integer. Currently n_marker_per_cmp is set to be default value `{default_paramdict["n_marker_per_cmp"]}`!')
                     paramdict['n_marker_per_cmp'] = default_paramdict["n_marker_per_cmp"]
             except:
                 print(f'WARNING: unrecognized option value `{val}` for n_marker_per_cmp! Please use numeric value. Currently n_marker_per_cmp is set to be default value `{default_paramdict["n_marker_per_cmp"]}`!')
             continue
         
         
+        if opt in ('--n_pseudo_spot'):
+            try:
+                paramdict['n_pseudo_spot'] = int(float(val))
+                
+                if paramdict['n_pseudo_spot'] < 0:
+                    print(f'WARNING: negative option value `{paramdict["n_pseudo_spot"]}` for n_pseudo_spot! Please use non-negative integer. Currently n_pseudo_spot is set to be default value `{default_paramdict["n_pseudo_spot"]}`!')
+                    paramdict['n_pseudo_spot'] = default_paramdict["n_pseudo_spot"]
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for n_pseudo_spot! Please use numeric value. Currently n_pseudo_spot is set to be default value `{default_paramdict["n_pseudo_spot"]}`!')
+            continue
+        
+        
         if opt in ('--pseudo_spot_min_cell'):
             try:
                 paramdict['pseudo_spot_min_cell'] = int(float(val))
                 
                 if paramdict['pseudo_spot_min_cell'] < 2:
                     print(f'WARNING: invalid option value `{paramdict["pseudo_spot_min_cell"]}` for pseudo_spot_min_cell! Please use integer which >= 2. Currently pseudo_spot_min_cell is set to be value `2`!')
                     paramdict['pseudo_spot_min_cell'] = 2
@@ -490,14 +506,26 @@
                     print(f'WARNING: non-positive option value `{paramdict["cvae_init_lr"]}` for cvae_init_lr! Please use positve value. Currently cvae_init_lr is set to be default value `{default_paramdict["cvae_init_lr"]}`!')
                     paramdict['cvae_init_lr'] = default_paramdict["cvae_init_lr"]
             except:
                 print(f'WARNING: unrecognized option value `{val}` for cvae_init_lr! Please use numeric value. Currently cvae_init_lr is set to be default value `{default_paramdict["cvae_init_lr"]}`!')
             continue
         
         
+        if opt in ('--num_hidden_layer'):
+            try:
+                paramdict['num_hidden_layer'] = int(float(val))
+                
+                if paramdict['num_hidden_layer'] < 1:
+                    print(f'WARNING: invalid option value `{paramdict["num_hidden_layer"]}` for num_hidden_layer! Please use integer which >= 1. Currently num_hidden_layer is set to be value `1`!')
+                    paramdict['num_hidden_layer'] = 1
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for num_hidden_layer! Please use numeric value. Currently num_hidden_layer is set to be default value `{default_paramdict["num_hidden_layer"]}`!')
+            continue
+        
+        
         if opt in ('--redo_de'):
             if val.casefold() == 'true'.casefold():
                 paramdict['redo_de'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['redo_de'] = False
             else:
                 print(f'WARNING: unrecognized option value `{val}` for redo_de! Please use string of true or false. Currently redo_de is set to be default value `{default_paramdict["redo_de"]}`!')
```

### Comparing `sdeper-1.1.0/src/preprocess.py` & `sdeper-1.2.0/src/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import pandas as pd
 from cvae import build_CVAE_whole
 from utils import run_DE_only
 from config import print
 
 
 
-def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, filter_cell, filter_gene, diagnosis):
+def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, filter_cell, filter_gene, diagnosis):
     '''
     preprocess files
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
@@ -47,45 +47,49 @@
     A_file : string
         full path of input csv file of Adjacency Matrix of spots in spatial transcriptomic data (spots * spots).
     use_cvae : bool
         whether to build CVAE to adjust platform effect.
     n_hv_gene : int
         number of highly variable genes for CVAE.
     n_marker_per_cmp : int
-        number of TOP marker genes for each comparison in DE
+        number of TOP marker genes for each comparison in DE.
+    n_pseudo_spot : int
+        number of pseudo-spots.
     pseudo_spot_min_cell : int
-        minimum value of cells in pseudo-spot
+        minimum value of cells in pseudo-spot.
     pseudo_spot_max_cell : int
-        maximum value of cells in pseudo-spot
+        maximum value of cells in pseudo-spot.
     seq_depth_scaler : int
-        a scaler of scRNA-seq sequencing depth
+        a scaler of scRNA-seq sequencing depth.
     cvae_input_scaler : int
-        maximum value of the scaled input for CVAE
+        maximum value of the scaled input for CVAE.
     cvae_init_lr : float
-        initial learning rate for training CVAE
+        initial learning rate for training CVAE.
+    num_hidden_layer : int
+        number of hidden layers in encoder and decoder.
     redo_de : bool
-        whether to redo DE after CVAE transformation
+        whether to redo DE after CVAE transformation.
     use_fdr : bool
-        whether to use FDR adjusted p value for filtering and sorting
+        whether to use FDR adjusted p value for filtering and sorting.
     p_val_cutoff : float
-        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering
+        threshold of p value (or FDR if --use_fdr is true) in marker genes filtering.
     fc_cutoff : float
-        threshold of fold change (without log transform!) in marker genes filtering
+        threshold of fold change (without log transform!) in marker genes filtering.
     pct1_cutoff : float
-        threshold of pct.1 in marker genes filtering
+        threshold of pct.1 in marker genes filtering.
     pct2_cutoff : float
-        threshold of pct.2 in marker genes filtering
+        threshold of pct.2 in marker genes filtering.
     sortby_fc : bool
-        whether to sort marker genes by fold change
+        whether to sort marker genes by fold change.
     diagnosis : bool
-        if True save more information to files for diagnosis CVAE and hyper-parameter selection
+        if True save more information to files for diagnosis CVAE and hyper-parameter selection.
     filter_cell : bool
-        whether to filter cells before DE
+        whether to filter cells before DE.
     filter_gene : bool
-        whether to filter genes before DE
+        whether to filter genes before DE.
 
     Returns
     -------
     data : Dict
         a Dict contains all info need for modeling:
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
@@ -100,15 +104,15 @@
     # first determine whether to build CVAE
     if use_cvae:
         if ref_file is None or ref_anno_file is None:
             raise Exception('ERROR: building CVAE requires both reference scRNA-seq data and corresponding cell-type annotation specified! But at least one of them is not specified!')
             
         print('first build CVAE...\n')
         # build CVAE, and return the data dict including transformed spatial data and reference gene expression
-        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
+        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
         
         # calculate squencing depth, sum also works on sparse dataframe
         N = spatial_df.sum(axis=1)
     
     else:
         
         print('building CVAE skipped...\n')
```

### Comparing `sdeper-1.1.0/src/run_model.py` & `sdeper-1.2.0/src/run_model.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.1.0/src/sdeper.egg-info/PKG-INFO` & `sdeper-1.2.0/src/sdeper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.1.0
+Version: 1.2.0
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
@@ -28,21 +28,27 @@
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: umap-learn==0.5.3
 Requires-Dist: distinctipy==1.2.2
 Requires-Dist: reportlab==4.1.0
 Requires-Dist: opencv-python==4.6.0.66
 
 # SDePER
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
 
-SDePER can be installed via `pip`
+SDePER can be installed via conda
+
+```bash
+conda create -n sdeper-env -c bioconda -c conda-forge python=3.9.12 sdeper
+```
+
+or pip
 
 ```bash
 conda create -n sdeper-env python=3.9.12
 conda activate sdeper-env
 pip install sdeper
 ```
```

### Comparing `sdeper-1.1.0/src/sdeper.egg-info/SOURCES.txt` & `sdeper-1.2.0/src/sdeper.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements.txt
 setup.py
 src/__init__.py
 src/admm_fit.py
 src/config.py
 src/cvae.py
 src/cvaeglrm.py
+src/diagnosis_plots.py
 src/hyper_parameter_optimization.py
 src/imputation.py
 src/local_fit_numba.py
 src/model_fit.py
 src/parse_opt.py
 src/preprocess.py
 src/run_model.py
```

### Comparing `sdeper-1.1.0/src/utils.py` & `sdeper-1.2.0/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 
 
 import os
 import numpy as np
 import pandas as pd
-from config import print, output_path
+from config import print, diagnosis_path
 import scanpy as sc
 sc.settings.verbosity = 0  # verbosity: errors (0), warnings (1), info (2), hints (3)
 
 
 
 def calcRMSE(truth, predicted):
     '''
@@ -364,15 +364,16 @@
             tmp_df.rename(columns={'names': 'gene'}, inplace=True)
             de_result_list.append(tmp_df.loc[:, ['gene', 'logfoldchanges', 'pvals', 'pvals_adj', 'pct1', 'pct2', 'celltype1', 'celltype2', 'selected']].copy())
 
     scrna_marker_genes = sorted(list(set(scrna_marker_genes)))
     print(f'finally selected {len(scrna_marker_genes)} cell-type marker genes\n')
     
     if save_result:
-        pd.concat(de_result_list).to_csv(os.path.join(output_path, save_file_name), index=False)
+        os.makedirs(os.path.join(diagnosis_path, 'celltype_markers'), exist_ok=True)
+        pd.concat(de_result_list).to_csv(os.path.join(diagnosis_path, 'celltype_markers', save_file_name)+'.gz', index=False, compression='gzip')
     
     return scrna_marker_genes
 
 
 
 def run_DE_only(ref_file, ref_anno_file, spatial_genes, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result=False, filter_cell=True, filter_gene=True):
     '''
@@ -421,15 +422,15 @@
     overlap_genes = list(set(spatial_genes).intersection(set(scrna_obj.var_names)))
     #if len(overlap_genes) < len(spatial_genes):
         #print(f'{len(spatial_genes)-len(overlap_genes)} genes in spatial data but not found in scRNA-seq data: {", ".join(set(spatial_genes).difference(set(overlap_genes)))}\n')
     
     scrna_obj = scrna_obj[:, overlap_genes].copy()
     
     # DE
-    marker_genes = run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result, 'DE celltype markers.csv')
+    marker_genes = run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result, 'DE_celltype_markers.csv')
     
     # generate average gene expressions (gene signature) for cell-types based on normalized values
     tmp_df = sc.get.obs_df(scrna_obj, keys=marker_genes)
     
     tmp_df['celltype'] = scrna_obj.obs['celltype']
 
     tmp_df = tmp_df.groupby(['celltype']).mean()
@@ -493,15 +494,15 @@
         if pre_n_gene > scrna_obj.n_vars:
             print(f'filtering genes present in <10 cells: {pre_n_gene-scrna_obj.n_vars} genes removed\n')
         else:
             print('filtering genes present in <10 cells: No genes removed\n')
     
     # do not normalize by sequencing depth as it's already normalized
     # so directly run DE on values in AnnData.X
-    return run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result, 'redo DE celltype markers.csv')
+    return run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result, 'redo_DE_celltype_markers.csv')
 
 
 
 # check total size of a Python object such as a Dictionary
 # ref https://code.activestate.com/recipes/577504/
 def total_size(o, handlers={}, verbose=False):
     """
```

