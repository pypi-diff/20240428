# Comparing `tmp/fastprop-1.0.0b4.tar.gz` & `tmp/fastprop-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastprop-1.0.0b4.tar", last modified: Tue Apr  2 19:02:04 2024, max compression
+gzip compressed data, was "fastprop-1.0.1.tar", last modified: Sun Apr 28 02:16:26 2024, max compression
```

## Comparing `fastprop-1.0.0b4.tar` & `fastprop-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.232006 fastprop-1.0.0b4/fastprop/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.232006 fastprop-1.0.0b4/fastprop/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/cli/fastprop_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    26470 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/fastprop_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/hopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/shap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.232006 fastprop-1.0.0b4/fastprop/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/calculate_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37956 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/descriptor_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/select_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/fastprop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/test/test_fastprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-28 02:16:23.000000 fastprop-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-04-28 02:16:26.712403 fastprop-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-04-28 02:16:23.000000 fastprop-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/fastprop/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/fastprop/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/fastprop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-28 02:16:23.000000 fastprop-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:16:26.712403 fastprop-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-28 02:16:23.000000 fastprop-1.0.1/test/test_fastprop.py
```

### Comparing `fastprop-1.0.0b4/LICENSE` & `fastprop-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b4/PKG-INFO` & `fastprop-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,149 +1,133 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.0b4
+Version: 1.0.1
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: lightning
+Requires-Dist: torch>=1.13
 Requires-Dist: mordredcommunity
 Requires-Dist: astartes[molecules]
 Requires-Dist: tensorboard
 Requires-Dist: psutil
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: hopt
 Requires-Dist: ray[train]; extra == "hopt"
 Requires-Dist: optuna; extra == "hopt"
 Provides-Extra: shap
-Requires-Dist: shap; extra == "shap"
+Requires-Dist: shap<0.45; extra == "shap"
 Requires-Dist: matplotlib; extra == "shap"
 Provides-Extra: bmark
 Requires-Dist: py2opsin; extra == "bmark"
 
 <p align="center">  
-  <img alt="fastproplogo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
+  <img alt="fastprop Logo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
 </p>
-<h2 align="center">Fast Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
+<h2 align="center">Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
+<h3 align="center">Fast, Scalable, and <500 LOC</h3>
  
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/fastprop?style=social">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastprop">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/fastprop">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/fastprop">
 </p>
 
-# Announcement - Open Beta!
-`fastprop` is currently in the version 3 open beta (1.0.0b3)!
+# Announcements
+## alphaXiv
+The `fastprop` paper is freely available online at [arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/2404.02058) - comments are appreciated!
+The source for the paper is stored in this repository under the `paper` directory.
+
+## Initial Release :tada:
+`fastprop` version 1 is officially released, meaning the API is now stable and ready for production use!
 Please try `fastprop` on your datasets and let us know what you think.
 Feature requests and bug reports are **very** appreciated!
 
-Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required!
-
-<a target="_blank" href="https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb">
-  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-</a>
-
 # Installing `fastprop`
 `fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.12.
-Installing from `pip` or `conda` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
+Installing from `pip` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
+Pending interest from users, a `conda` package will be added.
+
+Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb)
 
 ## `pip` [recommended]
 `fastprop` is available via PyPI with `pip install fastprop`.
 
 To make extending `fastprop` easier and keep the installation size down, dependencies required for hyperparameter optimization and SHAP analysis are _optional_.
 They can be installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them both.
 If you want to use `fastprop` but not write new code on top of it, you may want to install these now - you can always do so later, however, and `fastprop` will remind you.
 
-## `conda` - _coming soon!_
-~~`fastprop` is available from `conda-forge` with `conda install -c conda-forge fastprop`.~~
-
 ## Source
 To install `fastprop` from GitHub directly you can:
- 1. Run `pip install https://github.com/JacksonBurns/fastprop.git@main` to install from the `main` branch (or specify any other branch you like)
+ 1. Run `pip install https://github.com/JacksonBurns/fastprop.git@main` to install from the `main` branch (or specify any other branch you like).
  2. Clone the repository with `git clone https://github.com/JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run `pip install .`
 
 To contribute to `fastprop` please follow [this tutorial](https://opensource.com/article/19/7/create-pull-request-github) (or something similar) to set up a forked version of `fastprop` and open a pull request (similar to above option 2).
 All contributions are appreciated!
 See [Developing `fastprop`](#developing-fastprop) for more details.
 
 # About `fastprop`
 `fastprop` is a package for performing deep-QSPR (Quantitative Structure-Property Relationship) with minimal user intervention.
 By passing in a list of SMILES strings, `fastprop` will automatically generate and cache a set of molecular descriptors using [`mordredcommunity`](https://github.com/JacksonBurns/mordred-community) and train an FNN to predict the corresponding properties.
 See the `examples` and `benchmarks` directories to see how to run training - the rest of this documentation will focus on how you can run, configure, and customize `fastprop`.
 
-## Paper
-An academic paper has been prepared which describes the `fastprop` approach and walks through the `benchmarks` in greater detail.
-See the `paper` directory for more information.
-
 ## `fastprop` Framework
 There are four distinct steps in `fastprop` that define its framework:
  1. Featurization - transform the input molecules (as SMILES strings) into an array of molecular descriptors which are saved
  2. Preprocessing - clean the descriptors by removing or imputing missing values then rescaling the remainder
- 3. Training - send the processed input to the neural network, which is a sample FNN (sequential fully-connected layers with an activation function between)
+ 3. Training - send the processed input to the neural network, which is a simple FNN (sequential fully-connected layers with an activation function between)
  4. Prediction - save the trained model for future use
 
 ## Configurable Parameters
  1. Featurization
     - Input CSV file: comma separated values (CSV) file (with headers) containing SMILES strings representing the molecules and the targets
     - SMILES column name: name of the column containing the SMILES strings
     - Target column name(s): name(s) of the columns containing the targets
 
     _and_
     - Which `mordred` descriptors to calculate: 'all' or 'optimized' (a smaller set of descriptors; faster, but less accurate).
-    - Enable/Disable caching of calculated descriptors: `fastprop` will by default cache calculated descriptors based on the input filename and warn the user when it loads descriptors from the file rather than calculating on the fly
+    - Enable/Disable caching of calculated descriptors: `fastprop` will by default cache calculated descriptors based on the input filename and warn the user when it loads descriptors from the file rather than calculating on-the-fly
 
     _or_
     - Load precomputed descriptors: filepath to where descriptors are already cached either manually or by `fastprop`
  2. Preprocessing
-    - Enable/Disable dropping of zero-variance parameters (disabled by default; faster, but often less accurate)
-
-    ~~- Enable/Disable dropping of co-linear descriptors (disabled by default; faster, decreased accuracy)~~ _WIP_
-    - _not configurable_: `fastprop` will always rescale input features, drop columns with no values, and impute missing values with the per-feature mean
+    - _not configurable_: `fastprop` will always rescale input features, set invariant and missing features to zero, and impute missing values with the per-feature mean
  3. Training
     - Number of Repeats: How many times to split/train/test on the dataset (increments random seed by 1 each time).
 
     _and_
     - Number of FNN layers (default 2; repeated fully connected layers of hidden size)
     - Hidden Size: number of neurons per FNN layer (default 1800)
 
     _or_
     - Hyperparameter optimization: runs hyperparameter optimization identify the optimal number of layers and hidden size
 
     _generic NN training parameters_
     - Output Directory
     - Learning rate
     - Batch size
-
-    ~~- Checkpoint file to resume from (optional)~~ _WIP_
     - Problem type (one of: regression, binary, multiclass (start labels from 0), multilabel)
  4. Prediction
-    - Input SMILES: either a single SMILES or a CSV file
+    - Input SMILES: either a single SMILES or file of SMILES strings on individual lines
     - Output format: filepath to write the results or nothing, defaults to stdout
-    - Checkpoints directory: directory where previously trained model(s) are
-
-## Relationship to Chemprop
-In addition to having a similar name, `fastprop` and Chemprop do a similar things: map chemical structures to their corresponding properties in a user-friendly way using machine learning.
-I ([@JacksonBurns](https://github.com/jacksonburns)) am also a developer of Chemprop so some code is inevitably shared between the two (`fastprop`->Chemprop and vice versa).
-
-`fastprop` _feels_ a lot like Chemprop but without a lot of the clutter.
-The `fast` in `fastprop` (both in usage and execution time) comes from the basic architecture, the use of caching, and the reduced configurability of `fastprop` (i.e. I hope you like MSE loss for regression tasks, because that's the only training metric `fastprop` will use).
 
 # Using `fastprop`
 `fastprop` can be run from the command line or as a Python module.
 Regardless of the method of use the parameters described in [Configurable Parameters](#configurable-parameters) can be modified.
-Some system-specific configuration options can be specified in a `.fastpropconfig` file - see the [example file](https://github.com/JacksonBurns/fastprop/blob/main/.fastpropconfig).
 
 ## Command Line
 After installation, `fastprop` is accessible from the command line via `fastprop subcommand`, where `subcommand` is either `train`, `predict`, or `shap`.
  - `train` takes in the parameters described in [Configurable Parameters](#configurable-parameters) sections 1, 2, and 3 (featurization, preproccessing, and training) and trains `fastprop` model(s) on the input data.
  - `predict` uses the output of a call to `train` to make prediction on arbitrary SMILES strings.
  - `shap` performs SHAP analysis on a trained model to determine which of the input features are important.
 
@@ -157,43 +141,85 @@
 All of the options shown in the [Configuration File](#configuration-file-recommended) section can also be passed as command line flags instead of written to a file.
 When passing the arguments, replace all `_` (underscore) with `-` (hyphen), i.e. `fastprop train --number-epochs 100`
 See `fastprop train --help` or `fastprop predict --help` for more information.
 
 `fastprop shap` and `fastprop predict` have only a couple arguments and so do not use configuration files.
 
 ## Python Module
+
+### Example
+Here's an example of training `fastprop` as a Python module on the `Arockiaraj` Polycyclic Aromatic Hydrocarbon dataset, pulled largely from `fastprop/cli/train.py`.
+With `fastprop` installed you can copy and run this script as-is!
+
+```python
+import pandas as pd
+import torch
+
+from fastprop.data import (
+    clean_dataset,
+    fastpropDataLoader,
+    fastpropDataset,
+    split,
+    standard_scale,
+)
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
+from fastprop.descriptors import get_descriptors
+from fastprop.io import load_saved_descriptors, read_input_csv
+from fastprop.model import fastprop, train_and_test
+
+# prepare the dataset
+targets, smiles = read_input_csv("https://raw.githubusercontent.com/JacksonBurns/fastprop/main/benchmarks/pah/arockiaraj_pah_data.csv")
+targets, rdkit_mols = clean_dataset(targets, smiles)
+descriptors = get_descriptors(".", DESCRIPTOR_SET_LOOKUP["all"], rdkit_mols)
+descriptors = descriptors.to_numpy(dtype=float)
+descriptors = torch.tensor(descriptors, dtype=torch.float32)
+targets = torch.tensor(targets, dtype=torch.float32)
+# feature scaling
+train_indexes, val_indexes, test_indexes = split(smiles)
+descriptors[train_indexes], feature_means, feature_vars = standard_scale(descriptors[train_indexes])
+descriptors[val_indexes] = standard_scale(descriptors[val_indexes], feature_means, feature_vars)
+descriptors[test_indexes] = standard_scale(descriptors[test_indexes], feature_means, feature_vars)
+
+# initialize dataloaders and model, then train
+train_dataloader = fastpropDataLoader(fastpropDataset(descriptors[train_indexes], targets[train_indexes]), shuffle=True)
+val_dataloader = fastpropDataLoader(fastpropDataset(descriptors[val_indexes], targets[val_indexes]))
+test_dataloader = fastpropDataLoader(fastpropDataset(descriptors[test_indexes], targets[test_indexes]))
+model = fastprop(feature_means, feature_vars)
+test_results, validation_results = train_and_test(".", model, train_dataloader, val_dataloader, test_dataloader)
+
+```
+
+### Package Structure
 This section documents where the various modules and functions used in `fastprop` are located.
 Check each file listed for more information, as each contains additional inline documentation useful for development as a Python module.
 To use the core `fastprop` model and dataloaders in your own work, consider looking at `shap.py` or `train.py` which show how to import and instantiate the relevant classes.
 
-### `fastprop`
+#### `fastprop`
  - `defaults`: contains the function `init_logger` used to initialize loggers in different submodules, as well as the default configuration for training.
- - `fastprop_core`: the model itself and convenience functions.
- - `hopt`: hyperparameter optimization using Optuna and Ray\[tune\], used by the CLI.
- - `train`: performs model training, used by the CLI.
- - `predict`: loads models from their checkpoint and config files and runs inference, used by the CLI.
- - `shap`: performs SHAP analysis on a previously trained model, used by the CLI.
- - `preprocessing`: performs all of the preprocessing described above.
-
-### `fastprop.utils`
- - `calculate_descriptors`: wraps the `mordredcommunity` descriptor calculator.
- - `linear_baseline`: trains a basic linear model on the same inputs to `fastprop` to act as a baseline.
- - `descriptor_lists`: hardcoded lists of all of the descriptors implemented in `mordredcommunity`.
- - `select_descriptors`: the script to retrieve the `mordredcommunity` modules based on the strings in the above file (`mordredcommunity` has a weird interface; thus, it is wrapped).
- - `load_data`: short wrappers to `pandas` CSV loading utility, but specialized for the output from `mordredcommunity` and `fastprop`.
- - `validate_config`: _WIP_ validate the input from the command line.
+ - `model`: the model itself and a convenience function for training.
+ - `metrics`: wraps a number of common loss and score functions.
+ - `descriptors`: functions for calculating descriptors.
+ - `data`: functions for cleaning and scaling data.
+ - `io`: functions for loading data from files.
 
-### `fastprop.cli`
+#### `fastprop.cli`
 `fastprop_cli`` contains all the CLI code which is likely not useful in use from a script.
 If you wish to extend the CLI, check the inline documentation there.
 
 # Benchmarks
 The `benchmarks` directory contains the scripts needed to perform the studies (see `benchmarks/README.md` for more detail, they are a great way to learn how to use `fastprop`).
 To just see the results, checkout [`paper/paper.pdf`](https://github.com/JacksonBurns/fastprop/blob/main/paper/paper.pdf) (or `paper/paper.md` for the plain text version).
 
+# Relationship to Chemprop
+In addition to having a similar name, `fastprop` and Chemprop do a similar things: map chemical structures to their corresponding properties in a user-friendly way using machine learning.
+I ([@JacksonBurns](https://github.com/jacksonburns)) am also a developer of Chemprop so some code is inevitably shared between the two (`fastprop` to Chemprop and vice versa).
+
+`fastprop` _feels_ a lot like Chemprop but without a lot of the clutter.
+The `fast` in `fastprop` (both in usage and execution time) comes from the basic architecture, the use of caching, and the reduced configurability of `fastprop` (i.e. I hope you like MSE loss for regression tasks, because that's the only training metric `fastprop` will use via the CLI).
+
 # Developing `fastprop`
 Bug reports, feature requests, and pull requests are welcome and encouraged!
 Follow [this tutorial from GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) to get started.
 
 `fastprop` is built around PyTorch lightning, which defines a rigid API for implementing models that is followed here.
 See the [section on the package layout](#python-module) for information on where all the other functions are, and check out the docstrings and inline comments in each file for more information on what each does.
```

#### html2text {}

```diff
@@ -1,108 +1,98 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.0b4 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.1 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
-lightning Requires-Dist: mordredcommunity Requires-Dist: astartes[molecules]
-Requires-Dist: tensorboard Requires-Dist: psutil Provides-Extra: dev Requires-
-Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
-pytest; extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra ==
-"hopt" Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-
-Dist: shap; extra == "shap" Requires-Dist: matplotlib; extra == "shap"
-Provides-Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
-                                [fastproplogo]
-     ********** FFaasstt MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
+lightning Requires-Dist: torch>=1.13 Requires-Dist: mordredcommunity Requires-
+Dist: astartes[molecules] Requires-Dist: tensorboard Requires-Dist: psutil
+Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: isort;
+extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov;
+extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra == "hopt"
+Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-Dist:
+shap<0.45; extra == "shap" Requires-Dist: matplotlib; extra == "shap" Provides-
+Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
+                                [fastprop Logo]
+        ********** MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
+                    ******** FFaasstt,, SSccaallaabbllee,, aanndd <<550000 LLOOCC ********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
-# Announcement - Open Beta! `fastprop` is currently in the version 3 open beta
-(1.0.0b3)! Please try `fastprop` on your datasets and let us know what you
-think. Feature requests and bug reports are **very** appreciated! Check out the
-demo notebook for quick intro to `fastprop` via Google Colab - runs in your
-browser, GPU included, no install required! _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]# Installing
-`fastprop` `fastprop` supports Mac, Windows, and Linux on Python versions 3.8
-to 3.12. Installing from `pip` or `conda` is the best way to get `fastprop`,
+# Announcements ## alphaXiv The `fastprop` paper is freely available online at
+[arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are
+conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/
+2404.02058) - comments are appreciated! The source for the paper is stored in
+this repository under the `paper` directory. ## Initial Release :tada:
+`fastprop` version 1 is officially released, meaning the API is now stable and
+ready for production use! Please try `fastprop` on your datasets and let us
+know what you think. Feature requests and bug reports are **very** appreciated!
+# Installing `fastprop` `fastprop` supports Mac, Windows, and Linux on Python
+versions 3.8 to 3.12. Installing from `pip` is the best way to get `fastprop`,
 but if you need to check out a specific GitHub branch or you want to contribute
-to `fastprop` a source installation is recommended. ## `pip` [recommended]
-`fastprop` is available via PyPI with `pip install fastprop`. To make extending
-`fastprop` easier and keep the installation size down, dependencies required
-for hyperparameter optimization and SHAP analysis are _optional_. They can be
+to `fastprop` a source installation is recommended. Pending interest from
+users, a `conda` package will be added. Check out the demo notebook for quick
+intro to `fastprop` via Google Colab - runs in your browser, GPU included, no
+install required: [![Open In Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/JacksonBurns/
+fastprop/blob/main/fastprop_demo.ipynb) ## `pip` [recommended] `fastprop` is
+available via PyPI with `pip install fastprop`. To make extending `fastprop`
+easier and keep the installation size down, dependencies required for
+hyperparameter optimization and SHAP analysis are _optional_. They can be
 installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or
 `pip install fastprop[shap,hopt]` to install them both. If you want to use
 `fastprop` but not write new code on top of it, you may want to install these
 now - you can always do so later, however, and `fastprop` will remind you. ##
-`conda` - _coming soon!_ ~~`fastprop` is available from `conda-forge` with
-`conda install -c conda-forge fastprop`.~~ ## Source To install `fastprop` from
-GitHub directly you can: 1. Run `pip install https://github.com/JacksonBurns/
-fastprop.git@main` to install from the `main` branch (or specify any other
-branch you like) 2. Clone the repository with `git clone https://github.com/
-JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run
-`pip install .` To contribute to `fastprop` please follow [this tutorial]
-(https://opensource.com/article/19/7/create-pull-request-github) (or something
-similar) to set up a forked version of `fastprop` and open a pull request
-(similar to above option 2). All contributions are appreciated! See [Developing
-`fastprop`](#developing-fastprop) for more details. # About `fastprop`
-`fastprop` is a package for performing deep-QSPR (Quantitative Structure-
-Property Relationship) with minimal user intervention. By passing in a list of
-SMILES strings, `fastprop` will automatically generate and cache a set of
-molecular descriptors using [`mordredcommunity`](https://github.com/
-JacksonBurns/mordred-community) and train an FNN to predict the corresponding
-properties. See the `examples` and `benchmarks` directories to see how to run
-training - the rest of this documentation will focus on how you can run,
-configure, and customize `fastprop`. ## Paper An academic paper has been
-prepared which describes the `fastprop` approach and walks through the
-`benchmarks` in greater detail. See the `paper` directory for more information.
-## `fastprop` Framework There are four distinct steps in `fastprop` that define
-its framework: 1. Featurization - transform the input molecules (as SMILES
-strings) into an array of molecular descriptors which are saved 2.
+Source To install `fastprop` from GitHub directly you can: 1. Run `pip install
+https://github.com/JacksonBurns/fastprop.git@main` to install from the `main`
+branch (or specify any other branch you like). 2. Clone the repository with
+`git clone https://github.com/JacksonBurns/fastprop.git`, navigate to
+`fastprop` with `cd fastprop`, and run `pip install .` To contribute to
+`fastprop` please follow [this tutorial](https://opensource.com/article/19/7/
+create-pull-request-github) (or something similar) to set up a forked version
+of `fastprop` and open a pull request (similar to above option 2). All
+contributions are appreciated! See [Developing `fastprop`](#developing-
+fastprop) for more details. # About `fastprop` `fastprop` is a package for
+performing deep-QSPR (Quantitative Structure-Property Relationship) with
+minimal user intervention. By passing in a list of SMILES strings, `fastprop`
+will automatically generate and cache a set of molecular descriptors using
+[`mordredcommunity`](https://github.com/JacksonBurns/mordred-community) and
+train an FNN to predict the corresponding properties. See the `examples` and
+`benchmarks` directories to see how to run training - the rest of this
+documentation will focus on how you can run, configure, and customize
+`fastprop`. ## `fastprop` Framework There are four distinct steps in `fastprop`
+that define its framework: 1. Featurization - transform the input molecules (as
+SMILES strings) into an array of molecular descriptors which are saved 2.
 Preprocessing - clean the descriptors by removing or imputing missing values
 then rescaling the remainder 3. Training - send the processed input to the
-neural network, which is a sample FNN (sequential fully-connected layers with
+neural network, which is a simple FNN (sequential fully-connected layers with
 an activation function between) 4. Prediction - save the trained model for
 future use ## Configurable Parameters 1. Featurization - Input CSV file: comma
 separated values (CSV) file (with headers) containing SMILES strings
 representing the molecules and the targets - SMILES column name: name of the
 column containing the SMILES strings - Target column name(s): name(s) of the
 columns containing the targets _and_ - Which `mordred` descriptors to
 calculate: 'all' or 'optimized' (a smaller set of descriptors; faster, but less
 accurate). - Enable/Disable caching of calculated descriptors: `fastprop` will
 by default cache calculated descriptors based on the input filename and warn
-the user when it loads descriptors from the file rather than calculating on the
-fly _or_ - Load precomputed descriptors: filepath to where descriptors are
-already cached either manually or by `fastprop` 2. Preprocessing - Enable/
-Disable dropping of zero-variance parameters (disabled by default; faster, but
-often less accurate) ~~- Enable/Disable dropping of co-linear descriptors
-(disabled by default; faster, decreased accuracy)~~ _WIP_ - _not configurable_:
-`fastprop` will always rescale input features, drop columns with no values, and
-impute missing values with the per-feature mean 3. Training - Number of
-Repeats: How many times to split/train/test on the dataset (increments random
-seed by 1 each time). _and_ - Number of FNN layers (default 2; repeated fully
-connected layers of hidden size) - Hidden Size: number of neurons per FNN layer
-(default 1800) _or_ - Hyperparameter optimization: runs hyperparameter
-optimization identify the optimal number of layers and hidden size _generic NN
-training parameters_ - Output Directory - Learning rate - Batch size ~~-
-Checkpoint file to resume from (optional)~~ _WIP_ - Problem type (one of:
-regression, binary, multiclass (start labels from 0), multilabel) 4. Prediction
-- Input SMILES: either a single SMILES or a CSV file - Output format: filepath
-to write the results or nothing, defaults to stdout - Checkpoints directory:
-directory where previously trained model(s) are ## Relationship to Chemprop In
-addition to having a similar name, `fastprop` and Chemprop do a similar things:
-map chemical structures to their corresponding properties in a user-friendly
-way using machine learning. I ([@JacksonBurns](https://github.com/
-jacksonburns)) am also a developer of Chemprop so some code is inevitably
-shared between the two (`fastprop`->Chemprop and vice versa). `fastprop`
-_feels_ a lot like Chemprop but without a lot of the clutter. The `fast` in
-`fastprop` (both in usage and execution time) comes from the basic
-architecture, the use of caching, and the reduced configurability of `fastprop`
-(i.e. I hope you like MSE loss for regression tasks, because that's the only
-training metric `fastprop` will use). # Using `fastprop` `fastprop` can be run
-from the command line or as a Python module. Regardless of the method of use
-the parameters described in [Configurable Parameters](#configurable-parameters)
-can be modified. Some system-specific configuration options can be specified in
-a `.fastpropconfig` file - see the [example file](https://github.com/
-JacksonBurns/fastprop/blob/main/.fastpropconfig). ## Command Line After
+the user when it loads descriptors from the file rather than calculating on-
+the-fly _or_ - Load precomputed descriptors: filepath to where descriptors are
+already cached either manually or by `fastprop` 2. Preprocessing - _not
+configurable_: `fastprop` will always rescale input features, set invariant and
+missing features to zero, and impute missing values with the per-feature mean
+3. Training - Number of Repeats: How many times to split/train/test on the
+dataset (increments random seed by 1 each time). _and_ - Number of FNN layers
+(default 2; repeated fully connected layers of hidden size) - Hidden Size:
+number of neurons per FNN layer (default 1800) _or_ - Hyperparameter
+optimization: runs hyperparameter optimization identify the optimal number of
+layers and hidden size _generic NN training parameters_ - Output Directory -
+Learning rate - Batch size - Problem type (one of: regression, binary,
+multiclass (start labels from 0), multilabel) 4. Prediction - Input SMILES:
+either a single SMILES or file of SMILES strings on individual lines - Output
+format: filepath to write the results or nothing, defaults to stdout # Using
+`fastprop` `fastprop` can be run from the command line or as a Python module.
+Regardless of the method of use the parameters described in [Configurable
+Parameters](#configurable-parameters) can be modified. ## Command Line After
 installation, `fastprop` is accessible from the command line via `fastprop
 subcommand`, where `subcommand` is either `train`, `predict`, or `shap`. -
 `train` takes in the parameters described in [Configurable Parameters]
 (#configurable-parameters) sections 1, 2, and 3 (featurization, preproccessing,
 and training) and trains `fastprop` model(s) on the input data. - `predict`
 uses the output of a call to `train` to make prediction on arbitrary SMILES
 strings. - `shap` performs SHAP analysis on a trained model to determine which
@@ -113,48 +103,73 @@
 training. It is everything shown in the [Configurable Parameters]
 (#configurable-parameters) section. ### Arguments All of the options shown in
 the [Configuration File](#configuration-file-recommended) section can also be
 passed as command line flags instead of written to a file. When passing the
 arguments, replace all `_` (underscore) with `-` (hyphen), i.e. `fastprop train
 --number-epochs 100` See `fastprop train --help` or `fastprop predict --help`
 for more information. `fastprop shap` and `fastprop predict` have only a couple
-arguments and so do not use configuration files. ## Python Module This section
-documents where the various modules and functions used in `fastprop` are
-located. Check each file listed for more information, as each contains
-additional inline documentation useful for development as a Python module. To
-use the core `fastprop` model and dataloaders in your own work, consider
-looking at `shap.py` or `train.py` which show how to import and instantiate the
-relevant classes. ### `fastprop` - `defaults`: contains the function
-`init_logger` used to initialize loggers in different submodules, as well as
-the default configuration for training. - `fastprop_core`: the model itself and
-convenience functions. - `hopt`: hyperparameter optimization using Optuna and
-Ray\[tune\], used by the CLI. - `train`: performs model training, used by the
-CLI. - `predict`: loads models from their checkpoint and config files and runs
-inference, used by the CLI. - `shap`: performs SHAP analysis on a previously
-trained model, used by the CLI. - `preprocessing`: performs all of the
-preprocessing described above. ### `fastprop.utils` - `calculate_descriptors`:
-wraps the `mordredcommunity` descriptor calculator. - `linear_baseline`: trains
-a basic linear model on the same inputs to `fastprop` to act as a baseline. -
-`descriptor_lists`: hardcoded lists of all of the descriptors implemented in
-`mordredcommunity`. - `select_descriptors`: the script to retrieve the
-`mordredcommunity` modules based on the strings in the above file
-(`mordredcommunity` has a weird interface; thus, it is wrapped). - `load_data`:
-short wrappers to `pandas` CSV loading utility, but specialized for the output
-from `mordredcommunity` and `fastprop`. - `validate_config`: _WIP_ validate the
-input from the command line. ### `fastprop.cli` `fastprop_cli`` contains all
-the CLI code which is likely not useful in use from a script. If you wish to
-extend the CLI, check the inline documentation there. # Benchmarks The
-`benchmarks` directory contains the scripts needed to perform the studies (see
-`benchmarks/README.md` for more detail, they are a great way to learn how to
-use `fastprop`). To just see the results, checkout [`paper/paper.pdf`](https://
-github.com/JacksonBurns/fastprop/blob/main/paper/paper.pdf) (or `paper/
-paper.md` for the plain text version). # Developing `fastprop` Bug reports,
-feature requests, and pull requests are welcome and encouraged! Follow [this
-tutorial from GitHub](https://docs.github.com/en/get-started/exploring-
-projects-on-github/contributing-to-a-project) to get started. `fastprop` is
-built around PyTorch lightning, which defines a rigid API for implementing
-models that is followed here. See the [section on the package layout](#python-
-module) for information on where all the other functions are, and check out the
-docstrings and inline comments in each file for more information on what each
-does. Note that the `pyproject.toml` defines optional `dev` and `bmark`
-packages, which will get you setup with the same dependencies used for CI and
-benchmarking.
+arguments and so do not use configuration files. ## Python Module ### Example
+Here's an example of training `fastprop` as a Python module on the `Arockiaraj`
+Polycyclic Aromatic Hydrocarbon dataset, pulled largely from `fastprop/cli/
+train.py`. With `fastprop` installed you can copy and run this script as-is!
+```python import pandas as pd import torch from fastprop.data import
+( clean_dataset, fastpropDataLoader, fastpropDataset, split, standard_scale, )
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
+from fastprop.descriptors import get_descriptors from fastprop.io import
+load_saved_descriptors, read_input_csv from fastprop.model import fastprop,
+train_and_test # prepare the dataset targets, smiles = read_input_csv("https://
+raw.githubusercontent.com/JacksonBurns/fastprop/main/benchmarks/pah/
+arockiaraj_pah_data.csv") targets, rdkit_mols = clean_dataset(targets, smiles)
+descriptors = get_descriptors(".", DESCRIPTOR_SET_LOOKUP["all"], rdkit_mols)
+descriptors = descriptors.to_numpy(dtype=float) descriptors = torch.tensor
+(descriptors, dtype=torch.float32) targets = torch.tensor(targets,
+dtype=torch.float32) # feature scaling train_indexes, val_indexes, test_indexes
+= split(smiles) descriptors[train_indexes], feature_means, feature_vars =
+standard_scale(descriptors[train_indexes]) descriptors[val_indexes] =
+standard_scale(descriptors[val_indexes], feature_means, feature_vars)
+descriptors[test_indexes] = standard_scale(descriptors[test_indexes],
+feature_means, feature_vars) # initialize dataloaders and model, then train
+train_dataloader = fastpropDataLoader(fastpropDataset(descriptors
+[train_indexes], targets[train_indexes]), shuffle=True) val_dataloader =
+fastpropDataLoader(fastpropDataset(descriptors[val_indexes], targets
+[val_indexes])) test_dataloader = fastpropDataLoader(fastpropDataset
+(descriptors[test_indexes], targets[test_indexes])) model = fastprop
+(feature_means, feature_vars) test_results, validation_results = train_and_test
+(".", model, train_dataloader, val_dataloader, test_dataloader) ``` ### Package
+Structure This section documents where the various modules and functions used
+in `fastprop` are located. Check each file listed for more information, as each
+contains additional inline documentation useful for development as a Python
+module. To use the core `fastprop` model and dataloaders in your own work,
+consider looking at `shap.py` or `train.py` which show how to import and
+instantiate the relevant classes. #### `fastprop` - `defaults`: contains the
+function `init_logger` used to initialize loggers in different submodules, as
+well as the default configuration for training. - `model`: the model itself and
+a convenience function for training. - `metrics`: wraps a number of common loss
+and score functions. - `descriptors`: functions for calculating descriptors. -
+`data`: functions for cleaning and scaling data. - `io`: functions for loading
+data from files. #### `fastprop.cli` `fastprop_cli`` contains all the CLI code
+which is likely not useful in use from a script. If you wish to extend the CLI,
+check the inline documentation there. # Benchmarks The `benchmarks` directory
+contains the scripts needed to perform the studies (see `benchmarks/README.md`
+for more detail, they are a great way to learn how to use `fastprop`). To just
+see the results, checkout [`paper/paper.pdf`](https://github.com/JacksonBurns/
+fastprop/blob/main/paper/paper.pdf) (or `paper/paper.md` for the plain text
+version). # Relationship to Chemprop In addition to having a similar name,
+`fastprop` and Chemprop do a similar things: map chemical structures to their
+corresponding properties in a user-friendly way using machine learning. I (
+[@JacksonBurns](https://github.com/jacksonburns)) am also a developer of
+Chemprop so some code is inevitably shared between the two (`fastprop` to
+Chemprop and vice versa). `fastprop` _feels_ a lot like Chemprop but without a
+lot of the clutter. The `fast` in `fastprop` (both in usage and execution time)
+comes from the basic architecture, the use of caching, and the reduced
+configurability of `fastprop` (i.e. I hope you like MSE loss for regression
+tasks, because that's the only training metric `fastprop` will use via the
+CLI). # Developing `fastprop` Bug reports, feature requests, and pull requests
+are welcome and encouraged! Follow [this tutorial from GitHub](https://
+docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-
+project) to get started. `fastprop` is built around PyTorch lightning, which
+defines a rigid API for implementing models that is followed here. See the
+[section on the package layout](#python-module) for information on where all
+the other functions are, and check out the docstrings and inline comments in
+each file for more information on what each does. Note that the
+`pyproject.toml` defines optional `dev` and `bmark` packages, which will get
+you setup with the same dependencies used for CI and benchmarking.
```

### Comparing `fastprop-1.0.0b4/README.md` & `fastprop-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,101 @@
 <p align="center">  
-  <img alt="fastproplogo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
+  <img alt="fastprop Logo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
 </p>
-<h2 align="center">Fast Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
+<h2 align="center">Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
+<h3 align="center">Fast, Scalable, and <500 LOC</h3>
  
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/fastprop?style=social">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastprop">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/fastprop">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/fastprop">
 </p>
 
-# Announcement - Open Beta!
-`fastprop` is currently in the version 3 open beta (1.0.0b3)!
+# Announcements
+## alphaXiv
+The `fastprop` paper is freely available online at [arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/2404.02058) - comments are appreciated!
+The source for the paper is stored in this repository under the `paper` directory.
+
+## Initial Release :tada:
+`fastprop` version 1 is officially released, meaning the API is now stable and ready for production use!
 Please try `fastprop` on your datasets and let us know what you think.
 Feature requests and bug reports are **very** appreciated!
 
-Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required!
-
-<a target="_blank" href="https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb">
-  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-</a>
-
 # Installing `fastprop`
 `fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.12.
-Installing from `pip` or `conda` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
+Installing from `pip` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
+Pending interest from users, a `conda` package will be added.
+
+Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb)
 
 ## `pip` [recommended]
 `fastprop` is available via PyPI with `pip install fastprop`.
 
 To make extending `fastprop` easier and keep the installation size down, dependencies required for hyperparameter optimization and SHAP analysis are _optional_.
 They can be installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them both.
 If you want to use `fastprop` but not write new code on top of it, you may want to install these now - you can always do so later, however, and `fastprop` will remind you.
 
-## `conda` - _coming soon!_
-~~`fastprop` is available from `conda-forge` with `conda install -c conda-forge fastprop`.~~
-
 ## Source
 To install `fastprop` from GitHub directly you can:
- 1. Run `pip install https://github.com/JacksonBurns/fastprop.git@main` to install from the `main` branch (or specify any other branch you like)
+ 1. Run `pip install https://github.com/JacksonBurns/fastprop.git@main` to install from the `main` branch (or specify any other branch you like).
  2. Clone the repository with `git clone https://github.com/JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run `pip install .`
 
 To contribute to `fastprop` please follow [this tutorial](https://opensource.com/article/19/7/create-pull-request-github) (or something similar) to set up a forked version of `fastprop` and open a pull request (similar to above option 2).
 All contributions are appreciated!
 See [Developing `fastprop`](#developing-fastprop) for more details.
 
 # About `fastprop`
 `fastprop` is a package for performing deep-QSPR (Quantitative Structure-Property Relationship) with minimal user intervention.
 By passing in a list of SMILES strings, `fastprop` will automatically generate and cache a set of molecular descriptors using [`mordredcommunity`](https://github.com/JacksonBurns/mordred-community) and train an FNN to predict the corresponding properties.
 See the `examples` and `benchmarks` directories to see how to run training - the rest of this documentation will focus on how you can run, configure, and customize `fastprop`.
 
-## Paper
-An academic paper has been prepared which describes the `fastprop` approach and walks through the `benchmarks` in greater detail.
-See the `paper` directory for more information.
-
 ## `fastprop` Framework
 There are four distinct steps in `fastprop` that define its framework:
  1. Featurization - transform the input molecules (as SMILES strings) into an array of molecular descriptors which are saved
  2. Preprocessing - clean the descriptors by removing or imputing missing values then rescaling the remainder
- 3. Training - send the processed input to the neural network, which is a sample FNN (sequential fully-connected layers with an activation function between)
+ 3. Training - send the processed input to the neural network, which is a simple FNN (sequential fully-connected layers with an activation function between)
  4. Prediction - save the trained model for future use
 
 ## Configurable Parameters
  1. Featurization
     - Input CSV file: comma separated values (CSV) file (with headers) containing SMILES strings representing the molecules and the targets
     - SMILES column name: name of the column containing the SMILES strings
     - Target column name(s): name(s) of the columns containing the targets
 
     _and_
     - Which `mordred` descriptors to calculate: 'all' or 'optimized' (a smaller set of descriptors; faster, but less accurate).
-    - Enable/Disable caching of calculated descriptors: `fastprop` will by default cache calculated descriptors based on the input filename and warn the user when it loads descriptors from the file rather than calculating on the fly
+    - Enable/Disable caching of calculated descriptors: `fastprop` will by default cache calculated descriptors based on the input filename and warn the user when it loads descriptors from the file rather than calculating on-the-fly
 
     _or_
     - Load precomputed descriptors: filepath to where descriptors are already cached either manually or by `fastprop`
  2. Preprocessing
-    - Enable/Disable dropping of zero-variance parameters (disabled by default; faster, but often less accurate)
-
-    ~~- Enable/Disable dropping of co-linear descriptors (disabled by default; faster, decreased accuracy)~~ _WIP_
-    - _not configurable_: `fastprop` will always rescale input features, drop columns with no values, and impute missing values with the per-feature mean
+    - _not configurable_: `fastprop` will always rescale input features, set invariant and missing features to zero, and impute missing values with the per-feature mean
  3. Training
     - Number of Repeats: How many times to split/train/test on the dataset (increments random seed by 1 each time).
 
     _and_
     - Number of FNN layers (default 2; repeated fully connected layers of hidden size)
     - Hidden Size: number of neurons per FNN layer (default 1800)
 
     _or_
     - Hyperparameter optimization: runs hyperparameter optimization identify the optimal number of layers and hidden size
 
     _generic NN training parameters_
     - Output Directory
     - Learning rate
     - Batch size
-
-    ~~- Checkpoint file to resume from (optional)~~ _WIP_
     - Problem type (one of: regression, binary, multiclass (start labels from 0), multilabel)
  4. Prediction
-    - Input SMILES: either a single SMILES or a CSV file
+    - Input SMILES: either a single SMILES or file of SMILES strings on individual lines
     - Output format: filepath to write the results or nothing, defaults to stdout
-    - Checkpoints directory: directory where previously trained model(s) are
-
-## Relationship to Chemprop
-In addition to having a similar name, `fastprop` and Chemprop do a similar things: map chemical structures to their corresponding properties in a user-friendly way using machine learning.
-I ([@JacksonBurns](https://github.com/jacksonburns)) am also a developer of Chemprop so some code is inevitably shared between the two (`fastprop`->Chemprop and vice versa).
-
-`fastprop` _feels_ a lot like Chemprop but without a lot of the clutter.
-The `fast` in `fastprop` (both in usage and execution time) comes from the basic architecture, the use of caching, and the reduced configurability of `fastprop` (i.e. I hope you like MSE loss for regression tasks, because that's the only training metric `fastprop` will use).
 
 # Using `fastprop`
 `fastprop` can be run from the command line or as a Python module.
 Regardless of the method of use the parameters described in [Configurable Parameters](#configurable-parameters) can be modified.
-Some system-specific configuration options can be specified in a `.fastpropconfig` file - see the [example file](https://github.com/JacksonBurns/fastprop/blob/main/.fastpropconfig).
 
 ## Command Line
 After installation, `fastprop` is accessible from the command line via `fastprop subcommand`, where `subcommand` is either `train`, `predict`, or `shap`.
  - `train` takes in the parameters described in [Configurable Parameters](#configurable-parameters) sections 1, 2, and 3 (featurization, preproccessing, and training) and trains `fastprop` model(s) on the input data.
  - `predict` uses the output of a call to `train` to make prediction on arbitrary SMILES strings.
  - `shap` performs SHAP analysis on a trained model to determine which of the input features are important.
 
@@ -127,43 +109,85 @@
 All of the options shown in the [Configuration File](#configuration-file-recommended) section can also be passed as command line flags instead of written to a file.
 When passing the arguments, replace all `_` (underscore) with `-` (hyphen), i.e. `fastprop train --number-epochs 100`
 See `fastprop train --help` or `fastprop predict --help` for more information.
 
 `fastprop shap` and `fastprop predict` have only a couple arguments and so do not use configuration files.
 
 ## Python Module
+
+### Example
+Here's an example of training `fastprop` as a Python module on the `Arockiaraj` Polycyclic Aromatic Hydrocarbon dataset, pulled largely from `fastprop/cli/train.py`.
+With `fastprop` installed you can copy and run this script as-is!
+
+```python
+import pandas as pd
+import torch
+
+from fastprop.data import (
+    clean_dataset,
+    fastpropDataLoader,
+    fastpropDataset,
+    split,
+    standard_scale,
+)
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
+from fastprop.descriptors import get_descriptors
+from fastprop.io import load_saved_descriptors, read_input_csv
+from fastprop.model import fastprop, train_and_test
+
+# prepare the dataset
+targets, smiles = read_input_csv("https://raw.githubusercontent.com/JacksonBurns/fastprop/main/benchmarks/pah/arockiaraj_pah_data.csv")
+targets, rdkit_mols = clean_dataset(targets, smiles)
+descriptors = get_descriptors(".", DESCRIPTOR_SET_LOOKUP["all"], rdkit_mols)
+descriptors = descriptors.to_numpy(dtype=float)
+descriptors = torch.tensor(descriptors, dtype=torch.float32)
+targets = torch.tensor(targets, dtype=torch.float32)
+# feature scaling
+train_indexes, val_indexes, test_indexes = split(smiles)
+descriptors[train_indexes], feature_means, feature_vars = standard_scale(descriptors[train_indexes])
+descriptors[val_indexes] = standard_scale(descriptors[val_indexes], feature_means, feature_vars)
+descriptors[test_indexes] = standard_scale(descriptors[test_indexes], feature_means, feature_vars)
+
+# initialize dataloaders and model, then train
+train_dataloader = fastpropDataLoader(fastpropDataset(descriptors[train_indexes], targets[train_indexes]), shuffle=True)
+val_dataloader = fastpropDataLoader(fastpropDataset(descriptors[val_indexes], targets[val_indexes]))
+test_dataloader = fastpropDataLoader(fastpropDataset(descriptors[test_indexes], targets[test_indexes]))
+model = fastprop(feature_means, feature_vars)
+test_results, validation_results = train_and_test(".", model, train_dataloader, val_dataloader, test_dataloader)
+
+```
+
+### Package Structure
 This section documents where the various modules and functions used in `fastprop` are located.
 Check each file listed for more information, as each contains additional inline documentation useful for development as a Python module.
 To use the core `fastprop` model and dataloaders in your own work, consider looking at `shap.py` or `train.py` which show how to import and instantiate the relevant classes.
 
-### `fastprop`
+#### `fastprop`
  - `defaults`: contains the function `init_logger` used to initialize loggers in different submodules, as well as the default configuration for training.
- - `fastprop_core`: the model itself and convenience functions.
- - `hopt`: hyperparameter optimization using Optuna and Ray\[tune\], used by the CLI.
- - `train`: performs model training, used by the CLI.
- - `predict`: loads models from their checkpoint and config files and runs inference, used by the CLI.
- - `shap`: performs SHAP analysis on a previously trained model, used by the CLI.
- - `preprocessing`: performs all of the preprocessing described above.
-
-### `fastprop.utils`
- - `calculate_descriptors`: wraps the `mordredcommunity` descriptor calculator.
- - `linear_baseline`: trains a basic linear model on the same inputs to `fastprop` to act as a baseline.
- - `descriptor_lists`: hardcoded lists of all of the descriptors implemented in `mordredcommunity`.
- - `select_descriptors`: the script to retrieve the `mordredcommunity` modules based on the strings in the above file (`mordredcommunity` has a weird interface; thus, it is wrapped).
- - `load_data`: short wrappers to `pandas` CSV loading utility, but specialized for the output from `mordredcommunity` and `fastprop`.
- - `validate_config`: _WIP_ validate the input from the command line.
+ - `model`: the model itself and a convenience function for training.
+ - `metrics`: wraps a number of common loss and score functions.
+ - `descriptors`: functions for calculating descriptors.
+ - `data`: functions for cleaning and scaling data.
+ - `io`: functions for loading data from files.
 
-### `fastprop.cli`
+#### `fastprop.cli`
 `fastprop_cli`` contains all the CLI code which is likely not useful in use from a script.
 If you wish to extend the CLI, check the inline documentation there.
 
 # Benchmarks
 The `benchmarks` directory contains the scripts needed to perform the studies (see `benchmarks/README.md` for more detail, they are a great way to learn how to use `fastprop`).
 To just see the results, checkout [`paper/paper.pdf`](https://github.com/JacksonBurns/fastprop/blob/main/paper/paper.pdf) (or `paper/paper.md` for the plain text version).
 
+# Relationship to Chemprop
+In addition to having a similar name, `fastprop` and Chemprop do a similar things: map chemical structures to their corresponding properties in a user-friendly way using machine learning.
+I ([@JacksonBurns](https://github.com/jacksonburns)) am also a developer of Chemprop so some code is inevitably shared between the two (`fastprop` to Chemprop and vice versa).
+
+`fastprop` _feels_ a lot like Chemprop but without a lot of the clutter.
+The `fast` in `fastprop` (both in usage and execution time) comes from the basic architecture, the use of caching, and the reduced configurability of `fastprop` (i.e. I hope you like MSE loss for regression tasks, because that's the only training metric `fastprop` will use via the CLI).
+
 # Developing `fastprop`
 Bug reports, feature requests, and pull requests are welcome and encouraged!
 Follow [this tutorial from GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) to get started.
 
 `fastprop` is built around PyTorch lightning, which defines a rigid API for implementing models that is followed here.
 See the [section on the package layout](#python-module) for information on where all the other functions are, and check out the docstrings and inline comments in each file for more information on what each does.
```

#### html2text {}

```diff
@@ -1,96 +1,85 @@
-                                [fastproplogo]
-     ********** FFaasstt MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
+                                [fastprop Logo]
+        ********** MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
+                    ******** FFaasstt,, SSccaallaabbllee,, aanndd <<550000 LLOOCC ********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
-# Announcement - Open Beta! `fastprop` is currently in the version 3 open beta
-(1.0.0b3)! Please try `fastprop` on your datasets and let us know what you
-think. Feature requests and bug reports are **very** appreciated! Check out the
-demo notebook for quick intro to `fastprop` via Google Colab - runs in your
-browser, GPU included, no install required! _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]# Installing
-`fastprop` `fastprop` supports Mac, Windows, and Linux on Python versions 3.8
-to 3.12. Installing from `pip` or `conda` is the best way to get `fastprop`,
+# Announcements ## alphaXiv The `fastprop` paper is freely available online at
+[arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are
+conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/
+2404.02058) - comments are appreciated! The source for the paper is stored in
+this repository under the `paper` directory. ## Initial Release :tada:
+`fastprop` version 1 is officially released, meaning the API is now stable and
+ready for production use! Please try `fastprop` on your datasets and let us
+know what you think. Feature requests and bug reports are **very** appreciated!
+# Installing `fastprop` `fastprop` supports Mac, Windows, and Linux on Python
+versions 3.8 to 3.12. Installing from `pip` is the best way to get `fastprop`,
 but if you need to check out a specific GitHub branch or you want to contribute
-to `fastprop` a source installation is recommended. ## `pip` [recommended]
-`fastprop` is available via PyPI with `pip install fastprop`. To make extending
-`fastprop` easier and keep the installation size down, dependencies required
-for hyperparameter optimization and SHAP analysis are _optional_. They can be
+to `fastprop` a source installation is recommended. Pending interest from
+users, a `conda` package will be added. Check out the demo notebook for quick
+intro to `fastprop` via Google Colab - runs in your browser, GPU included, no
+install required: [![Open In Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/JacksonBurns/
+fastprop/blob/main/fastprop_demo.ipynb) ## `pip` [recommended] `fastprop` is
+available via PyPI with `pip install fastprop`. To make extending `fastprop`
+easier and keep the installation size down, dependencies required for
+hyperparameter optimization and SHAP analysis are _optional_. They can be
 installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or
 `pip install fastprop[shap,hopt]` to install them both. If you want to use
 `fastprop` but not write new code on top of it, you may want to install these
 now - you can always do so later, however, and `fastprop` will remind you. ##
-`conda` - _coming soon!_ ~~`fastprop` is available from `conda-forge` with
-`conda install -c conda-forge fastprop`.~~ ## Source To install `fastprop` from
-GitHub directly you can: 1. Run `pip install https://github.com/JacksonBurns/
-fastprop.git@main` to install from the `main` branch (or specify any other
-branch you like) 2. Clone the repository with `git clone https://github.com/
-JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run
-`pip install .` To contribute to `fastprop` please follow [this tutorial]
-(https://opensource.com/article/19/7/create-pull-request-github) (or something
-similar) to set up a forked version of `fastprop` and open a pull request
-(similar to above option 2). All contributions are appreciated! See [Developing
-`fastprop`](#developing-fastprop) for more details. # About `fastprop`
-`fastprop` is a package for performing deep-QSPR (Quantitative Structure-
-Property Relationship) with minimal user intervention. By passing in a list of
-SMILES strings, `fastprop` will automatically generate and cache a set of
-molecular descriptors using [`mordredcommunity`](https://github.com/
-JacksonBurns/mordred-community) and train an FNN to predict the corresponding
-properties. See the `examples` and `benchmarks` directories to see how to run
-training - the rest of this documentation will focus on how you can run,
-configure, and customize `fastprop`. ## Paper An academic paper has been
-prepared which describes the `fastprop` approach and walks through the
-`benchmarks` in greater detail. See the `paper` directory for more information.
-## `fastprop` Framework There are four distinct steps in `fastprop` that define
-its framework: 1. Featurization - transform the input molecules (as SMILES
-strings) into an array of molecular descriptors which are saved 2.
+Source To install `fastprop` from GitHub directly you can: 1. Run `pip install
+https://github.com/JacksonBurns/fastprop.git@main` to install from the `main`
+branch (or specify any other branch you like). 2. Clone the repository with
+`git clone https://github.com/JacksonBurns/fastprop.git`, navigate to
+`fastprop` with `cd fastprop`, and run `pip install .` To contribute to
+`fastprop` please follow [this tutorial](https://opensource.com/article/19/7/
+create-pull-request-github) (or something similar) to set up a forked version
+of `fastprop` and open a pull request (similar to above option 2). All
+contributions are appreciated! See [Developing `fastprop`](#developing-
+fastprop) for more details. # About `fastprop` `fastprop` is a package for
+performing deep-QSPR (Quantitative Structure-Property Relationship) with
+minimal user intervention. By passing in a list of SMILES strings, `fastprop`
+will automatically generate and cache a set of molecular descriptors using
+[`mordredcommunity`](https://github.com/JacksonBurns/mordred-community) and
+train an FNN to predict the corresponding properties. See the `examples` and
+`benchmarks` directories to see how to run training - the rest of this
+documentation will focus on how you can run, configure, and customize
+`fastprop`. ## `fastprop` Framework There are four distinct steps in `fastprop`
+that define its framework: 1. Featurization - transform the input molecules (as
+SMILES strings) into an array of molecular descriptors which are saved 2.
 Preprocessing - clean the descriptors by removing or imputing missing values
 then rescaling the remainder 3. Training - send the processed input to the
-neural network, which is a sample FNN (sequential fully-connected layers with
+neural network, which is a simple FNN (sequential fully-connected layers with
 an activation function between) 4. Prediction - save the trained model for
 future use ## Configurable Parameters 1. Featurization - Input CSV file: comma
 separated values (CSV) file (with headers) containing SMILES strings
 representing the molecules and the targets - SMILES column name: name of the
 column containing the SMILES strings - Target column name(s): name(s) of the
 columns containing the targets _and_ - Which `mordred` descriptors to
 calculate: 'all' or 'optimized' (a smaller set of descriptors; faster, but less
 accurate). - Enable/Disable caching of calculated descriptors: `fastprop` will
 by default cache calculated descriptors based on the input filename and warn
-the user when it loads descriptors from the file rather than calculating on the
-fly _or_ - Load precomputed descriptors: filepath to where descriptors are
-already cached either manually or by `fastprop` 2. Preprocessing - Enable/
-Disable dropping of zero-variance parameters (disabled by default; faster, but
-often less accurate) ~~- Enable/Disable dropping of co-linear descriptors
-(disabled by default; faster, decreased accuracy)~~ _WIP_ - _not configurable_:
-`fastprop` will always rescale input features, drop columns with no values, and
-impute missing values with the per-feature mean 3. Training - Number of
-Repeats: How many times to split/train/test on the dataset (increments random
-seed by 1 each time). _and_ - Number of FNN layers (default 2; repeated fully
-connected layers of hidden size) - Hidden Size: number of neurons per FNN layer
-(default 1800) _or_ - Hyperparameter optimization: runs hyperparameter
-optimization identify the optimal number of layers and hidden size _generic NN
-training parameters_ - Output Directory - Learning rate - Batch size ~~-
-Checkpoint file to resume from (optional)~~ _WIP_ - Problem type (one of:
-regression, binary, multiclass (start labels from 0), multilabel) 4. Prediction
-- Input SMILES: either a single SMILES or a CSV file - Output format: filepath
-to write the results or nothing, defaults to stdout - Checkpoints directory:
-directory where previously trained model(s) are ## Relationship to Chemprop In
-addition to having a similar name, `fastprop` and Chemprop do a similar things:
-map chemical structures to their corresponding properties in a user-friendly
-way using machine learning. I ([@JacksonBurns](https://github.com/
-jacksonburns)) am also a developer of Chemprop so some code is inevitably
-shared between the two (`fastprop`->Chemprop and vice versa). `fastprop`
-_feels_ a lot like Chemprop but without a lot of the clutter. The `fast` in
-`fastprop` (both in usage and execution time) comes from the basic
-architecture, the use of caching, and the reduced configurability of `fastprop`
-(i.e. I hope you like MSE loss for regression tasks, because that's the only
-training metric `fastprop` will use). # Using `fastprop` `fastprop` can be run
-from the command line or as a Python module. Regardless of the method of use
-the parameters described in [Configurable Parameters](#configurable-parameters)
-can be modified. Some system-specific configuration options can be specified in
-a `.fastpropconfig` file - see the [example file](https://github.com/
-JacksonBurns/fastprop/blob/main/.fastpropconfig). ## Command Line After
+the user when it loads descriptors from the file rather than calculating on-
+the-fly _or_ - Load precomputed descriptors: filepath to where descriptors are
+already cached either manually or by `fastprop` 2. Preprocessing - _not
+configurable_: `fastprop` will always rescale input features, set invariant and
+missing features to zero, and impute missing values with the per-feature mean
+3. Training - Number of Repeats: How many times to split/train/test on the
+dataset (increments random seed by 1 each time). _and_ - Number of FNN layers
+(default 2; repeated fully connected layers of hidden size) - Hidden Size:
+number of neurons per FNN layer (default 1800) _or_ - Hyperparameter
+optimization: runs hyperparameter optimization identify the optimal number of
+layers and hidden size _generic NN training parameters_ - Output Directory -
+Learning rate - Batch size - Problem type (one of: regression, binary,
+multiclass (start labels from 0), multilabel) 4. Prediction - Input SMILES:
+either a single SMILES or file of SMILES strings on individual lines - Output
+format: filepath to write the results or nothing, defaults to stdout # Using
+`fastprop` `fastprop` can be run from the command line or as a Python module.
+Regardless of the method of use the parameters described in [Configurable
+Parameters](#configurable-parameters) can be modified. ## Command Line After
 installation, `fastprop` is accessible from the command line via `fastprop
 subcommand`, where `subcommand` is either `train`, `predict`, or `shap`. -
 `train` takes in the parameters described in [Configurable Parameters]
 (#configurable-parameters) sections 1, 2, and 3 (featurization, preproccessing,
 and training) and trains `fastprop` model(s) on the input data. - `predict`
 uses the output of a call to `train` to make prediction on arbitrary SMILES
 strings. - `shap` performs SHAP analysis on a trained model to determine which
@@ -101,48 +90,73 @@
 training. It is everything shown in the [Configurable Parameters]
 (#configurable-parameters) section. ### Arguments All of the options shown in
 the [Configuration File](#configuration-file-recommended) section can also be
 passed as command line flags instead of written to a file. When passing the
 arguments, replace all `_` (underscore) with `-` (hyphen), i.e. `fastprop train
 --number-epochs 100` See `fastprop train --help` or `fastprop predict --help`
 for more information. `fastprop shap` and `fastprop predict` have only a couple
-arguments and so do not use configuration files. ## Python Module This section
-documents where the various modules and functions used in `fastprop` are
-located. Check each file listed for more information, as each contains
-additional inline documentation useful for development as a Python module. To
-use the core `fastprop` model and dataloaders in your own work, consider
-looking at `shap.py` or `train.py` which show how to import and instantiate the
-relevant classes. ### `fastprop` - `defaults`: contains the function
-`init_logger` used to initialize loggers in different submodules, as well as
-the default configuration for training. - `fastprop_core`: the model itself and
-convenience functions. - `hopt`: hyperparameter optimization using Optuna and
-Ray\[tune\], used by the CLI. - `train`: performs model training, used by the
-CLI. - `predict`: loads models from their checkpoint and config files and runs
-inference, used by the CLI. - `shap`: performs SHAP analysis on a previously
-trained model, used by the CLI. - `preprocessing`: performs all of the
-preprocessing described above. ### `fastprop.utils` - `calculate_descriptors`:
-wraps the `mordredcommunity` descriptor calculator. - `linear_baseline`: trains
-a basic linear model on the same inputs to `fastprop` to act as a baseline. -
-`descriptor_lists`: hardcoded lists of all of the descriptors implemented in
-`mordredcommunity`. - `select_descriptors`: the script to retrieve the
-`mordredcommunity` modules based on the strings in the above file
-(`mordredcommunity` has a weird interface; thus, it is wrapped). - `load_data`:
-short wrappers to `pandas` CSV loading utility, but specialized for the output
-from `mordredcommunity` and `fastprop`. - `validate_config`: _WIP_ validate the
-input from the command line. ### `fastprop.cli` `fastprop_cli`` contains all
-the CLI code which is likely not useful in use from a script. If you wish to
-extend the CLI, check the inline documentation there. # Benchmarks The
-`benchmarks` directory contains the scripts needed to perform the studies (see
-`benchmarks/README.md` for more detail, they are a great way to learn how to
-use `fastprop`). To just see the results, checkout [`paper/paper.pdf`](https://
-github.com/JacksonBurns/fastprop/blob/main/paper/paper.pdf) (or `paper/
-paper.md` for the plain text version). # Developing `fastprop` Bug reports,
-feature requests, and pull requests are welcome and encouraged! Follow [this
-tutorial from GitHub](https://docs.github.com/en/get-started/exploring-
-projects-on-github/contributing-to-a-project) to get started. `fastprop` is
-built around PyTorch lightning, which defines a rigid API for implementing
-models that is followed here. See the [section on the package layout](#python-
-module) for information on where all the other functions are, and check out the
-docstrings and inline comments in each file for more information on what each
-does. Note that the `pyproject.toml` defines optional `dev` and `bmark`
-packages, which will get you setup with the same dependencies used for CI and
-benchmarking.
+arguments and so do not use configuration files. ## Python Module ### Example
+Here's an example of training `fastprop` as a Python module on the `Arockiaraj`
+Polycyclic Aromatic Hydrocarbon dataset, pulled largely from `fastprop/cli/
+train.py`. With `fastprop` installed you can copy and run this script as-is!
+```python import pandas as pd import torch from fastprop.data import
+( clean_dataset, fastpropDataLoader, fastpropDataset, split, standard_scale, )
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
+from fastprop.descriptors import get_descriptors from fastprop.io import
+load_saved_descriptors, read_input_csv from fastprop.model import fastprop,
+train_and_test # prepare the dataset targets, smiles = read_input_csv("https://
+raw.githubusercontent.com/JacksonBurns/fastprop/main/benchmarks/pah/
+arockiaraj_pah_data.csv") targets, rdkit_mols = clean_dataset(targets, smiles)
+descriptors = get_descriptors(".", DESCRIPTOR_SET_LOOKUP["all"], rdkit_mols)
+descriptors = descriptors.to_numpy(dtype=float) descriptors = torch.tensor
+(descriptors, dtype=torch.float32) targets = torch.tensor(targets,
+dtype=torch.float32) # feature scaling train_indexes, val_indexes, test_indexes
+= split(smiles) descriptors[train_indexes], feature_means, feature_vars =
+standard_scale(descriptors[train_indexes]) descriptors[val_indexes] =
+standard_scale(descriptors[val_indexes], feature_means, feature_vars)
+descriptors[test_indexes] = standard_scale(descriptors[test_indexes],
+feature_means, feature_vars) # initialize dataloaders and model, then train
+train_dataloader = fastpropDataLoader(fastpropDataset(descriptors
+[train_indexes], targets[train_indexes]), shuffle=True) val_dataloader =
+fastpropDataLoader(fastpropDataset(descriptors[val_indexes], targets
+[val_indexes])) test_dataloader = fastpropDataLoader(fastpropDataset
+(descriptors[test_indexes], targets[test_indexes])) model = fastprop
+(feature_means, feature_vars) test_results, validation_results = train_and_test
+(".", model, train_dataloader, val_dataloader, test_dataloader) ``` ### Package
+Structure This section documents where the various modules and functions used
+in `fastprop` are located. Check each file listed for more information, as each
+contains additional inline documentation useful for development as a Python
+module. To use the core `fastprop` model and dataloaders in your own work,
+consider looking at `shap.py` or `train.py` which show how to import and
+instantiate the relevant classes. #### `fastprop` - `defaults`: contains the
+function `init_logger` used to initialize loggers in different submodules, as
+well as the default configuration for training. - `model`: the model itself and
+a convenience function for training. - `metrics`: wraps a number of common loss
+and score functions. - `descriptors`: functions for calculating descriptors. -
+`data`: functions for cleaning and scaling data. - `io`: functions for loading
+data from files. #### `fastprop.cli` `fastprop_cli`` contains all the CLI code
+which is likely not useful in use from a script. If you wish to extend the CLI,
+check the inline documentation there. # Benchmarks The `benchmarks` directory
+contains the scripts needed to perform the studies (see `benchmarks/README.md`
+for more detail, they are a great way to learn how to use `fastprop`). To just
+see the results, checkout [`paper/paper.pdf`](https://github.com/JacksonBurns/
+fastprop/blob/main/paper/paper.pdf) (or `paper/paper.md` for the plain text
+version). # Relationship to Chemprop In addition to having a similar name,
+`fastprop` and Chemprop do a similar things: map chemical structures to their
+corresponding properties in a user-friendly way using machine learning. I (
+[@JacksonBurns](https://github.com/jacksonburns)) am also a developer of
+Chemprop so some code is inevitably shared between the two (`fastprop` to
+Chemprop and vice versa). `fastprop` _feels_ a lot like Chemprop but without a
+lot of the clutter. The `fast` in `fastprop` (both in usage and execution time)
+comes from the basic architecture, the use of caching, and the reduced
+configurability of `fastprop` (i.e. I hope you like MSE loss for regression
+tasks, because that's the only training metric `fastprop` will use via the
+CLI). # Developing `fastprop` Bug reports, feature requests, and pull requests
+are welcome and encouraged! Follow [this tutorial from GitHub](https://
+docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-
+project) to get started. `fastprop` is built around PyTorch lightning, which
+defines a rigid API for implementing models that is followed here. See the
+[section on the package layout](#python-module) for information on where all
+the other functions are, and check out the docstrings and inline comments in
+each file for more information on what each does. Note that the
+`pyproject.toml` defines optional `dev` and `bmark` packages, which will get
+you setup with the same dependencies used for CI and benchmarking.
```

### Comparing `fastprop-1.0.0b4/fastprop/cli/fastprop_cli.py` & `fastprop-1.0.1/fastprop/cli/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 import datetime
 import sys
 from importlib.metadata import version
 from time import perf_counter
 
 import yaml
 
-from fastprop import (
-    DEFAULT_TRAINING_CONFIG,
-    hopt_fastprop,
-    predict_fastprop,
-    shap_fastprop,
-    train_fastprop,
-)
+from fastprop import DEFAULT_TRAINING_CONFIG
 from fastprop.defaults import init_logger
-from fastprop.utils import validate_config
+
+from .predict import predict_fastprop
+from .shap import shap_fastprop
+from .train import train_fastprop
 
 logger = init_logger(__name__)
 
 
 def main():
     cli_start = perf_counter()
     parser = argparse.ArgumentParser(description="fastprop command line interface - try 'fastprop subcommand --help'")
@@ -30,23 +27,18 @@
     train_subparser = subparsers.add_parser("train")
     train_subparser.add_argument("config_file", nargs="?", help="YAML configuration file")
     train_subparser.add_argument("-od", "--output-directory", help="directory for fastprop output")
     # featurization
     train_subparser.add_argument("-if", "--input-file", help="csv of SMILES and targets")
     train_subparser.add_argument("-tc", "--target-columns", nargs="+", help="column name(s) for target(s)")
     train_subparser.add_argument("-sc", "--smiles-column", help="column name for SMILES")
-    train_subparser.add_argument("-d", "--descriptors", help="descriptors to calculate (one of all, optimized, smallest, or search)")
+    train_subparser.add_argument("-d", "--descriptors", help="descriptors to calculate (one of all, optimized, or debug)")
     train_subparser.add_argument("-ec", "--enable-cache", type=bool, help="allow saving and loading of cached descriptors")
     train_subparser.add_argument("-p", "--precomputed", help="precomputed descriptors from fastprop or mordred")
 
-    # preprocessing
-    train_subparser.add_argument("-r", "--rescaling", type=bool, help="rescale descriptors between 0 and 1 (default to True)")
-    train_subparser.add_argument("-zvd", "--zero-variance-drop", type=bool, help="drop zero variance descriptors (defaults to True)")
-    train_subparser.add_argument("-cd", "--colinear-drop", type=bool, help="drop colinear descriptors (defaults to False)")
-
     # training
     train_subparser.add_argument("-op", "--optimize", action="store_true", help="run hyperparameter optimization", default=False)
     train_subparser.add_argument("-fl", "--fnn-layers", type=int, help="number of fnn layers")
     train_subparser.add_argument("-lr", "--learning-rate", type=float, help="learning rate")
     train_subparser.add_argument("-bs", "--batch-size", type=int, help="batch size")
     train_subparser.add_argument("-ne", "--number-epochs", type=int, help="number of epochs")
     train_subparser.add_argument("-nr", "--number-repeats", type=int, help="number of repeats")
@@ -54,30 +46,36 @@
     train_subparser.add_argument("-ns", "--train-size", type=float, help="train size")
     train_subparser.add_argument("-vs", "--val-size", type=float, help="val size")
     train_subparser.add_argument("-ts", "--test-size", type=float, help="test size")
     train_subparser.add_argument("-s", "--sampler", help="choice of sampler, i.e. random, kmeans, etc.")
     train_subparser.add_argument("-rs", "--random-seed", type=int, help="random seed for sampling and pytorch seed")
     train_subparser.add_argument("-pc", "--patience", type=int, help="number of epochs to wait before early stopping")
 
+    # inference
     predict_subparser = subparsers.add_parser("predict")
     predict_subparser.add_argument("checkpoints_dir", help="directory of checkpoint file(s) for predictions")
     input_group = predict_subparser.add_mutually_exclusive_group()
-    input_group.add_argument("-s", "--smiles", nargs="+", help="SMILES string for prediction")
-    input_group.add_argument("-i", "--input-file", help="file containing SMILES strings")
+    input_group.add_argument("-ss", "--smiles-strings", nargs="+", type=str, help="SMILES string(s) for prediction")
+    input_group.add_argument("-sf", "--smiles-file", help="file containing SMILES strings only")
+    input_group = predict_subparser.add_mutually_exclusive_group(required=True)
+    input_group.add_argument("-ds", "--descriptor-set", help="descriptors to calculate (one of all, optimized, or debug)")
+    input_group.add_argument("-pd", "--precomputed-descriptors", help="precomputed descriptors")
     predict_subparser.add_argument("-o", "--output", required=False, help="output file for predictions (defaults to stdout)")
 
+    # feature importance
     shap_subparser = subparsers.add_parser("shap")
     shap_subparser.add_argument("checkpoints_dir", help="directory of checkpoint file(s) for SHAP analysis")
-    shap_subparser.add_argument("input_file", help="csv of SMILES and targets used during training")
+    shap_subparser.add_argument("cached_descriptors", help="csv of calculated descriptors cached by fastprop")
+    shap_subparser.add_argument("descriptor_set", help="descriptors in the cache file (one of all, optimized, or debug)")
     shap_subparser.add_argument(
         "-it",
         "--importance-threshold",
         default=0.75,
         type=float,
-        help="[0-1] hide features below (most important feature) x this",
+        help="[0-1] include top fraction of features, default 0.75",
     )
 
     # no args provided - print the help text
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(0)
 
@@ -88,48 +86,39 @@
 
     # cast to a dict
     args = vars(args)
     subcommand = args.pop("subcommand")
     args.pop("version")
     if subcommand == "train":
         training_default = dict(DEFAULT_TRAINING_CONFIG)
-        # exit with help if no args given
-        if not sum(map(lambda i: i is not None, args.values())):
-            train_subparser.print_help()
-            exit(0)
         optim_requested = args.pop("optimize")
         if args["config_file"] is not None:
             if sum(map(lambda i: i is not None, args.values())) > 1:
                 raise parser.error("Cannot specify config_file with other command line arguments (except --optimize).")
             with open(args["config_file"], "r") as f:
                 cfg = yaml.safe_load(f)
                 cfg["target_columns"] = cfg["target_columns"].split(" ")
                 training_default.update(cfg)
         else:
             training_default.update({k: v for k, v in args.items() if v is not None})
 
-        optim_requested = training_default.pop("optimize") or optim_requested
+        optim_requested = training_default.pop("hopt") or optim_requested
         logger.info(f"Training Parameters:\n{yaml.dump(training_default, sort_keys=False)}")
-        # validate this dictionary, i.e. layer counts are positive, etc.
-        # cannot specify both precomputed and descriptors or enable/cache
-        validate_config(training_default)
         if optim_requested:
-            training_default.pop("fnn_layers")
-            training_default.pop("hidden_size")
-            if any((args.get("fnn_layers") is not None, args.get("hidden_size") is not None)):
-                logger.warning("Hidden Size/FNN Layers specified with optimize and are ignored.")
-            hopt_fastprop(**training_default)
+            if args.get("fnn_layers", None) is not None:
+                logger.warning("--fnn-layers specified with --optimize - ignored.")
+            if args.get("hidden_size", None) is not None:
+                logger.warning("--hidden-size specified with --optimize - ignored.")
+            train_fastprop(**training_default, hopt=True)
         else:
             train_fastprop(**training_default)
     elif subcommand == "shap":
         shap_fastprop(**args)
     elif subcommand == "predict":
-        if args["smiles"] is None and args["input_file"] is None:
-            raise parser.error("One of -i/--input-file or -s/--smiles must be provided.")
         logger.info(f"Predict Parameters:\n {yaml.dump(args, sort_keys=False)}")
         predict_fastprop(**args)
     else:
         logger.critical(f"Unrecognized subcommand '{subcommand}', printing help and exiting.")
         parser.print_help()
         sys.exit(0)
-    logger.info("If you use fastprop in published work, please cite: ...WIP...")
+    logger.info("If you use fastprop in published work, please cite https://arxiv.org/abs/2404.02058")
     logger.info("Total elapsed time: " + str(datetime.timedelta(seconds=perf_counter() - cli_start)))
```

### Comparing `fastprop-1.0.0b4/fastprop/predict.py` & `fastprop-1.0.1/fastprop/cli/predict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,67 @@
 import os
-import pickle
+from typing import List, Optional
 
 import numpy as np
 import pandas as pd
-import yaml
-from rdkit import Chem
-
-from fastprop.defaults import init_logger
-from fastprop.utils import calculate_mordred_desciptors
-from fastprop.utils.select_descriptors import mordred_descriptors_from_strings
-
-from .fastprop_core import fastprop
+import torch
+from pytorch_lightning import Trainer
+from torch.utils.data import TensorDataset
+
+from fastprop.data import clean_dataset, fastpropDataLoader
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, init_logger
+from fastprop.descriptors import get_descriptors
+from fastprop.io import load_saved_descriptors
+from fastprop.model import fastprop
 
 logger = init_logger(__name__)
 
 
-def _safe_yaml_open(dir, fname):
-    try:
-        with open(os.path.join(dir, fname)) as file:
-            return yaml.safe_load(file)
-    except FileNotFoundError:
-        logger.error(f"checkpoints directory is missing '{fname}'. Re-execute training.")
-
-
-def predict_fastprop(checkpoints_dir, smiles, input_file, output=None):
-    """Prediction CLI.
-
-    Loads a model and runs inference on the input.
-
-    Args:
-        checkpoints_dir (str): 'checkpoints' directory from a previous fastprop train.
-        smiles (str or list[str]): SMILES strings for prediction.
-        input_file (str): Input file containing only SMILES strings for prediction.
-        output (str or None): Either save to a file or just print result.
-    """
-    if input_file:
-        raise NotImplementedError("TODO: please pass as command line options, loading from file is a WIP")
-    if type(smiles) is str:
-        smiles = [smiles]
-    checkpoint_dir_contents = os.listdir(checkpoints_dir)
-    config_dict = _safe_yaml_open(checkpoints_dir, "fastprop_config.yml")
-    descs = calculate_mordred_desciptors(
-        mordred_descriptors_from_strings(config_dict["descriptors"]),
-        [Chem.MolFromSmiles(i) for i in smiles],
-        n_procs=0,  # ignored for "strategy='low-memory'"
-        strategy="low-memory",
-    )
+def predict_fastprop(
+    checkpoints_dir: str,
+    smiles_strings: List[str],
+    descriptor_set: str,
+    smiles_file: Optional[str] = None,
+    precomputed_descriptors: Optional[np.ndarray] = None,
+    output: Optional[str] = None,
+):
+    if smiles_file is not None:
+        if smiles_strings:
+            raise RuntimeError("Specify either smiles_strings or smiles_file, not both.")
+        smiles_strings = [s.strip() for s in open(smiles_file, "r").readlines()]
+
+    # load the models
+    if precomputed_descriptors is None:
+        _, rdkit_mols = clean_dataset(np.zeros((1, len(smiles_strings))), np.array(smiles_strings))
+        descs = get_descriptors(cache_filepath=False, descriptors=DESCRIPTOR_SET_LOOKUP[descriptor_set], rdkit_mols=rdkit_mols)
+        descs = descs.to_numpy(dtype=float)
+    else:
+        descs = load_saved_descriptors(precomputed_descriptors)
+
     all_models = []
-    for checkpoint in checkpoint_dir_contents:
-        if not checkpoint.endswith(".ckpt"):
-            continue
-        model = fastprop.load_from_checkpoint(
-            os.path.join(checkpoints_dir, checkpoint),
-            cleaned_data=None,
-            targets=None,
-            smiles=None,
-        )
-        scalers = _safe_yaml_open(checkpoints_dir, f"repetition_{checkpoint.split('-')[1]}_scalers.yml")
-        model.target_scaler = pickle.loads(scalers["target_scaler"])
-        model.mean_imputer = pickle.loads(scalers["mean_imputer"])
-        model.feature_scaler = pickle.loads(scalers["feature_scaler"])
+    for checkpoint in os.listdir(checkpoints_dir):
+        model = fastprop.load_from_checkpoint(os.path.join(checkpoints_dir, checkpoint))
         all_models.append(model)
+
+    descs = torch.tensor(descs, dtype=torch.float32)
+    predict_dataloader = fastpropDataLoader(TensorDataset(descs))
+    # run inference
     # axis: contents
     # 0: smiles
     # 1: predictions
     # 2: per-model
-    all_predictions = np.stack([model.predict_step(descs) for model in all_models], axis=2)
+    trainer = Trainer(logger=False)
+    all_predictions = np.stack([torch.vstack(trainer.predict(model, predict_dataloader)).numpy(force=True) for model in all_models], axis=2)
     perf = np.mean(all_predictions, axis=2)
     err = np.std(all_predictions, axis=2)
     # interleave the columns of these arrays, thanks stackoverflow.com/a/75519265
     res = np.empty((len(perf), perf.shape[1] * 2), dtype=perf.dtype)
     res[:, 0::2] = perf
     res[:, 1::2] = err
     column_names = []
-    for target in config_dict["targets"]:
+    for target in [f"task_{i}" for i in range(all_predictions.shape[1])]:
         column_names.extend([target, target + "_stdev"])
-    out = pd.DataFrame(res, columns=column_names, index=smiles)
+    out = pd.DataFrame(res, columns=column_names, index=smiles_strings)
     if output is None:
         print("\n", out)
     else:
         out.to_csv(output)
```

### Comparing `fastprop-1.0.0b4/fastprop/shap.py` & `fastprop-1.0.1/fastprop/cli/shap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,91 @@
 import os
-import pickle
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
-import yaml
 from tqdm import tqdm
 
-from fastprop.defaults import init_logger
-from fastprop.fastprop_core import fastprop
-from fastprop.utils import calculate_mordred_desciptors, load_from_csv
-from fastprop.utils.select_descriptors import mordred_descriptors_from_strings
+from fastprop.data import standard_scale
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, init_logger
+from fastprop.io import load_saved_descriptors
+from fastprop.model import fastprop
 
 shap = None
 try:
     import shap
 except ImportError as ie:
     shape_error = ie
 
 
 logger = init_logger(__name__)
 
 
-def shap_fastprop(checkpoints_dir, input_file, importance_threshold=0.75):
+def shap_fastprop(
+    checkpoints_dir: str,
+    cached_descriptors: str,
+    descriptor_set: str,
+    importance_threshold: float = 0.75,
+):
     if shap is None:
         raise RuntimeError("Unable to import shap dependencies, please install fastprop[shap]. Original error: " + str(shape_error))
-    # get the configuration file with some run metadata
-    checkpoint_dir_contents = os.listdir(checkpoints_dir)
-    with open(os.path.join(checkpoints_dir, "fastprop_config.yml")) as file:
-        config_dict = yaml.safe_load(file)
+    # load the models
+    all_models = []
+    for checkpoint in os.listdir(checkpoints_dir):
+        model = fastprop.load_from_checkpoint(os.path.join(checkpoints_dir, checkpoint))
+        all_models.append(model)
 
-    # calculate the features in the same way the model did when training,
     # downsampling to the shap suggested size where required
     # (also see https://github.com/shap/shap/issues/955 for an explanation of
     # Why the thresholds are the way they are)
-    targets, mols, smiles = load_from_csv(input_file, config_dict["smiles"], config_dict["targets"])
-    num_mols = len(mols)
+    descs = load_saved_descriptors(cached_descriptors)
+    num_mols = descs.shape[0]
     threshold_1 = 200
     threshold_2 = 2000
     if num_mols > threshold_1:
         rng = np.random.default_rng(42)
         target = threshold_1 if num_mols < threshold_2 else threshold_2
         logger.info(f"Randomly downsampling to {target} molecules.")
-        mols = rng.choice(mols, size=target, replace=False)
-    descs = calculate_mordred_desciptors(
-        mordred_descriptors_from_strings(config_dict["descriptors"]),
-        mols,
-        n_procs=0,  # ignored for "strategy='low-memory'"
-        strategy="low-memory",
-    )
+        idxs = rng.choice(num_mols, size=target, replace=False)
+        descs = descs[idxs]
 
-    # load each of the models in the group
-    all_models = []
-    for checkpoint in checkpoint_dir_contents:
-        if not checkpoint.endswith(".ckpt"):
-            continue
-        model = fastprop.load_from_checkpoint(
-            os.path.join(checkpoints_dir, checkpoint),
-            cleaned_data=None,
-            targets=None,
-            smiles=None,
-        )
-        try:
-            with open(os.path.join(checkpoints_dir, f"repetition_{checkpoint.split('-')[1]}_scalers.yml")) as file:
-                scalers = yaml.safe_load(file)
-        except FileNotFoundError:
-            logger.error(f"checkpoints directory is missing 'repetition_{checkpoint.split('-')[1]}_scalers.yml'. Re-execute training.")
-        model.target_scaler = pickle.loads(scalers["target_scaler"])
-        model.mean_imputer = pickle.loads(scalers["mean_imputer"])
-        model.feature_scaler = pickle.loads(scalers["feature_scaler"])
-        all_models.append(model)
+    descs = torch.tensor(descs, dtype=torch.float32, device=all_models[0].device)
+    X = standard_scale(descs, all_models[0].feature_means, all_models[0].feature_vars)
 
     # we will use half of the data for 'integrating', and the other half for getting shap values
     halfway_idx = descs.shape[0] // 2
 
     # shap terminology explanation:
     # background: 100 to 1000 random samples from the training data
     # X: 100+ other samples
     # run shap on each of these models, then average the results
     per_model_shap = []
     for model in tqdm(all_models, desc="Calculating SHAP values for each model"):
         # now scale and send the data to whatever device lightning put the model on
-        X = torch.tensor(model.feature_scaler.transform(model.mean_imputer.transform(descs)), dtype=torch.float32).to(model.device)
         e = shap.DeepExplainer(model, X[:halfway_idx])
         model_shap_values = e.shap_values(X[halfway_idx:])
         # returns a list for multi-target problems, cast for uniformity
         if not isinstance(model_shap_values, list):
             model_shap_values = [model_shap_values]
         per_model_shap.append(model_shap_values)
     all_shap_values = np.mean(np.array(per_model_shap), axis=0)
-    # TODO: write these to a file, sorted by highest absolute SHAP on first target.
 
     # for each target, create a plot of the most important features
-    for i, target_name in enumerate(config_dict["targets"]):
+    for i, target_name in enumerate(f"task_{i}" for i in range(all_models[0].readout.out_features)):
         shap_values = all_shap_values[i]
         # include features until the shap value is half the highest, aka half as important
         avg_shaps = np.mean(np.abs(shap_values), axis=0)
-        avg_shaps, names, keep_idxs = zip(*sorted(zip(avg_shaps, config_dict["descriptors"], list(range(len(avg_shaps)))), reverse=True))
+        avg_shaps, names, keep_idxs = zip(*sorted(zip(avg_shaps, DESCRIPTOR_SET_LOOKUP[descriptor_set], list(range(len(avg_shaps)))), reverse=True))
         include_idx = 0
         for val in avg_shaps[1:]:
             if val > avg_shaps[0] * importance_threshold:
                 include_idx += 1
             else:
                 break
         explanation = shap.Explanation(values=shap_values[:, keep_idxs[:include_idx]], feature_names=names[0:include_idx])
         plt.cla()
-        axes = shap.plots.beeswarm(explanation, max_display=include_idx + 1, color_bar=False, color="shap_red", show=False)
+        _ = shap.plots.beeswarm(explanation, max_display=include_idx + 1, color_bar=False, color="shap_red", show=False)
         out_fname = target_name + "_feature_importance_beeswarm.png"
         if os.path.exists(out_fname):
             logger.warning(f"Output file exists! {__name__} will overwrite '{out_fname}'.")
         plt.savefig(out_fname, pad_inches=0.5, bbox_inches="tight")
     logger.info("Visit the mordred-community docs to lookup descriptors: https://jacksonburns.github.io/mordred-community/descriptors.html")
```

### Comparing `fastprop-1.0.0b4/fastprop/utils/descriptor_lists.py` & `fastprop-1.0.1/fastprop/defaults.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,71 @@
+import logging
+import os
+import warnings
+from types import MappingProxyType
+
+warnings.filterwarnings(action="ignore", message=".*does not have many workers.*")
+
+_logging_format = dict(
+    format="[%(asctime)s %(name)s] %(levelname)s: %(message)s",
+    datefmt="%m/%d/%Y %I:%M:%S %p",
+    level=logging.INFO,
+)
+
+
+def _init_loggers(outpath: str):
+    """Sets up a duplicate logging output to a text file in the given directory.
+
+    Args:
+        outpath (str): Destination directory for log file.
+    """
+    logging.basicConfig(
+        **_logging_format,
+        handlers=[logging.FileHandler(os.path.join(outpath, "fastprop_log.txt")), logging.StreamHandler()],
+    )
+
+
+def init_logger(module_name: str) -> logging.Logger:
+    """Returns a logger instance at appropriate level given with the given name.
+
+    Args:
+        module_name (str): Module name.
+
+    Returns:
+        logging.logger: Logger instance.
+    """
+    logger = logging.getLogger(module_name)
+    logger.setLevel(logging.DEBUG)
+    return logger
+
+
+# immutable default settings
+DEFAULT_TRAINING_CONFIG = MappingProxyType(
+    dict(
+        descriptor_set="all",
+        enable_cache=True,
+        precomputed=None,
+        fnn_layers=2,
+        learning_rate=0.0001,
+        batch_size=2048,
+        number_epochs=30,
+        number_repeats=1,
+        problem_type="regression",
+        train_size=0.8,
+        val_size=0.1,
+        test_size=0.1,
+        sampler="random",
+        random_seed=42,
+        hidden_size=1800,
+        hopt=False,
+        patience=5,
+    )
+)
+
+
 # Complete list of 2D descriptors implemented in Mordred as well as a subset
 # of those descriptors which are often useful for fastprop after preprocessing
 
 ALL_2D = [
     "ABC",
     "ABCGG",
     "nAcid",
@@ -1613,15 +1677,14 @@
     "WPol",
     "Zagreb1",
     "Zagreb2",
     "mZagreb1",
     "mZagreb2",
 ]
 
-
 SUBSET_947 = [
     "ABC",
     "ABCGG",
     "nBase",
     "SpAbs_A",
     "SpMax_A",
     "SpDiam_A",
@@ -2564,11 +2627,24 @@
     "WPol",
     "Zagreb1",
     "Zagreb2",
     "mZagreb1",
     "mZagreb2",
 ]
 
-descriptors_lookup = dict(
+DEBUG = [
+    "MATS8pe",
+    "MATS1are",
+    "MATS2are",
+    "MATS3are",
+    "MATS4are",
+    "MATS5are",
+    "MATS6are",
+    "MATS7are",
+    "MATS8are",
+]
+
+DESCRIPTOR_SET_LOOKUP = dict(
     optimized=SUBSET_947,
     all=ALL_2D,
+    debug=DEBUG,
 )
```

### Comparing `fastprop-1.0.0b4/fastprop.egg-info/PKG-INFO` & `fastprop-1.0.1/fastprop.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,149 +1,133 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.0b4
+Version: 1.0.1
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: lightning
+Requires-Dist: torch>=1.13
 Requires-Dist: mordredcommunity
 Requires-Dist: astartes[molecules]
 Requires-Dist: tensorboard
 Requires-Dist: psutil
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: hopt
 Requires-Dist: ray[train]; extra == "hopt"
 Requires-Dist: optuna; extra == "hopt"
 Provides-Extra: shap
-Requires-Dist: shap; extra == "shap"
+Requires-Dist: shap<0.45; extra == "shap"
 Requires-Dist: matplotlib; extra == "shap"
 Provides-Extra: bmark
 Requires-Dist: py2opsin; extra == "bmark"
 
 <p align="center">  
-  <img alt="fastproplogo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
+  <img alt="fastprop Logo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
 </p>
-<h2 align="center">Fast Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
+<h2 align="center">Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
+<h3 align="center">Fast, Scalable, and <500 LOC</h3>
  
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/fastprop?style=social">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastprop">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/fastprop">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/fastprop">
 </p>
 
-# Announcement - Open Beta!
-`fastprop` is currently in the version 3 open beta (1.0.0b3)!
+# Announcements
+## alphaXiv
+The `fastprop` paper is freely available online at [arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/2404.02058) - comments are appreciated!
+The source for the paper is stored in this repository under the `paper` directory.
+
+## Initial Release :tada:
+`fastprop` version 1 is officially released, meaning the API is now stable and ready for production use!
 Please try `fastprop` on your datasets and let us know what you think.
 Feature requests and bug reports are **very** appreciated!
 
-Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required!
-
-<a target="_blank" href="https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb">
-  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-</a>
-
 # Installing `fastprop`
 `fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.12.
-Installing from `pip` or `conda` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
+Installing from `pip` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
+Pending interest from users, a `conda` package will be added.
+
+Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb)
 
 ## `pip` [recommended]
 `fastprop` is available via PyPI with `pip install fastprop`.
 
 To make extending `fastprop` easier and keep the installation size down, dependencies required for hyperparameter optimization and SHAP analysis are _optional_.
 They can be installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them both.
 If you want to use `fastprop` but not write new code on top of it, you may want to install these now - you can always do so later, however, and `fastprop` will remind you.
 
-## `conda` - _coming soon!_
-~~`fastprop` is available from `conda-forge` with `conda install -c conda-forge fastprop`.~~
-
 ## Source
 To install `fastprop` from GitHub directly you can:
- 1. Run `pip install https://github.com/JacksonBurns/fastprop.git@main` to install from the `main` branch (or specify any other branch you like)
+ 1. Run `pip install https://github.com/JacksonBurns/fastprop.git@main` to install from the `main` branch (or specify any other branch you like).
  2. Clone the repository with `git clone https://github.com/JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run `pip install .`
 
 To contribute to `fastprop` please follow [this tutorial](https://opensource.com/article/19/7/create-pull-request-github) (or something similar) to set up a forked version of `fastprop` and open a pull request (similar to above option 2).
 All contributions are appreciated!
 See [Developing `fastprop`](#developing-fastprop) for more details.
 
 # About `fastprop`
 `fastprop` is a package for performing deep-QSPR (Quantitative Structure-Property Relationship) with minimal user intervention.
 By passing in a list of SMILES strings, `fastprop` will automatically generate and cache a set of molecular descriptors using [`mordredcommunity`](https://github.com/JacksonBurns/mordred-community) and train an FNN to predict the corresponding properties.
 See the `examples` and `benchmarks` directories to see how to run training - the rest of this documentation will focus on how you can run, configure, and customize `fastprop`.
 
-## Paper
-An academic paper has been prepared which describes the `fastprop` approach and walks through the `benchmarks` in greater detail.
-See the `paper` directory for more information.
-
 ## `fastprop` Framework
 There are four distinct steps in `fastprop` that define its framework:
  1. Featurization - transform the input molecules (as SMILES strings) into an array of molecular descriptors which are saved
  2. Preprocessing - clean the descriptors by removing or imputing missing values then rescaling the remainder
- 3. Training - send the processed input to the neural network, which is a sample FNN (sequential fully-connected layers with an activation function between)
+ 3. Training - send the processed input to the neural network, which is a simple FNN (sequential fully-connected layers with an activation function between)
  4. Prediction - save the trained model for future use
 
 ## Configurable Parameters
  1. Featurization
     - Input CSV file: comma separated values (CSV) file (with headers) containing SMILES strings representing the molecules and the targets
     - SMILES column name: name of the column containing the SMILES strings
     - Target column name(s): name(s) of the columns containing the targets
 
     _and_
     - Which `mordred` descriptors to calculate: 'all' or 'optimized' (a smaller set of descriptors; faster, but less accurate).
-    - Enable/Disable caching of calculated descriptors: `fastprop` will by default cache calculated descriptors based on the input filename and warn the user when it loads descriptors from the file rather than calculating on the fly
+    - Enable/Disable caching of calculated descriptors: `fastprop` will by default cache calculated descriptors based on the input filename and warn the user when it loads descriptors from the file rather than calculating on-the-fly
 
     _or_
     - Load precomputed descriptors: filepath to where descriptors are already cached either manually or by `fastprop`
  2. Preprocessing
-    - Enable/Disable dropping of zero-variance parameters (disabled by default; faster, but often less accurate)
-
-    ~~- Enable/Disable dropping of co-linear descriptors (disabled by default; faster, decreased accuracy)~~ _WIP_
-    - _not configurable_: `fastprop` will always rescale input features, drop columns with no values, and impute missing values with the per-feature mean
+    - _not configurable_: `fastprop` will always rescale input features, set invariant and missing features to zero, and impute missing values with the per-feature mean
  3. Training
     - Number of Repeats: How many times to split/train/test on the dataset (increments random seed by 1 each time).
 
     _and_
     - Number of FNN layers (default 2; repeated fully connected layers of hidden size)
     - Hidden Size: number of neurons per FNN layer (default 1800)
 
     _or_
     - Hyperparameter optimization: runs hyperparameter optimization identify the optimal number of layers and hidden size
 
     _generic NN training parameters_
     - Output Directory
     - Learning rate
     - Batch size
-
-    ~~- Checkpoint file to resume from (optional)~~ _WIP_
     - Problem type (one of: regression, binary, multiclass (start labels from 0), multilabel)
  4. Prediction
-    - Input SMILES: either a single SMILES or a CSV file
+    - Input SMILES: either a single SMILES or file of SMILES strings on individual lines
     - Output format: filepath to write the results or nothing, defaults to stdout
-    - Checkpoints directory: directory where previously trained model(s) are
-
-## Relationship to Chemprop
-In addition to having a similar name, `fastprop` and Chemprop do a similar things: map chemical structures to their corresponding properties in a user-friendly way using machine learning.
-I ([@JacksonBurns](https://github.com/jacksonburns)) am also a developer of Chemprop so some code is inevitably shared between the two (`fastprop`->Chemprop and vice versa).
-
-`fastprop` _feels_ a lot like Chemprop but without a lot of the clutter.
-The `fast` in `fastprop` (both in usage and execution time) comes from the basic architecture, the use of caching, and the reduced configurability of `fastprop` (i.e. I hope you like MSE loss for regression tasks, because that's the only training metric `fastprop` will use).
 
 # Using `fastprop`
 `fastprop` can be run from the command line or as a Python module.
 Regardless of the method of use the parameters described in [Configurable Parameters](#configurable-parameters) can be modified.
-Some system-specific configuration options can be specified in a `.fastpropconfig` file - see the [example file](https://github.com/JacksonBurns/fastprop/blob/main/.fastpropconfig).
 
 ## Command Line
 After installation, `fastprop` is accessible from the command line via `fastprop subcommand`, where `subcommand` is either `train`, `predict`, or `shap`.
  - `train` takes in the parameters described in [Configurable Parameters](#configurable-parameters) sections 1, 2, and 3 (featurization, preproccessing, and training) and trains `fastprop` model(s) on the input data.
  - `predict` uses the output of a call to `train` to make prediction on arbitrary SMILES strings.
  - `shap` performs SHAP analysis on a trained model to determine which of the input features are important.
 
@@ -157,43 +141,85 @@
 All of the options shown in the [Configuration File](#configuration-file-recommended) section can also be passed as command line flags instead of written to a file.
 When passing the arguments, replace all `_` (underscore) with `-` (hyphen), i.e. `fastprop train --number-epochs 100`
 See `fastprop train --help` or `fastprop predict --help` for more information.
 
 `fastprop shap` and `fastprop predict` have only a couple arguments and so do not use configuration files.
 
 ## Python Module
+
+### Example
+Here's an example of training `fastprop` as a Python module on the `Arockiaraj` Polycyclic Aromatic Hydrocarbon dataset, pulled largely from `fastprop/cli/train.py`.
+With `fastprop` installed you can copy and run this script as-is!
+
+```python
+import pandas as pd
+import torch
+
+from fastprop.data import (
+    clean_dataset,
+    fastpropDataLoader,
+    fastpropDataset,
+    split,
+    standard_scale,
+)
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
+from fastprop.descriptors import get_descriptors
+from fastprop.io import load_saved_descriptors, read_input_csv
+from fastprop.model import fastprop, train_and_test
+
+# prepare the dataset
+targets, smiles = read_input_csv("https://raw.githubusercontent.com/JacksonBurns/fastprop/main/benchmarks/pah/arockiaraj_pah_data.csv")
+targets, rdkit_mols = clean_dataset(targets, smiles)
+descriptors = get_descriptors(".", DESCRIPTOR_SET_LOOKUP["all"], rdkit_mols)
+descriptors = descriptors.to_numpy(dtype=float)
+descriptors = torch.tensor(descriptors, dtype=torch.float32)
+targets = torch.tensor(targets, dtype=torch.float32)
+# feature scaling
+train_indexes, val_indexes, test_indexes = split(smiles)
+descriptors[train_indexes], feature_means, feature_vars = standard_scale(descriptors[train_indexes])
+descriptors[val_indexes] = standard_scale(descriptors[val_indexes], feature_means, feature_vars)
+descriptors[test_indexes] = standard_scale(descriptors[test_indexes], feature_means, feature_vars)
+
+# initialize dataloaders and model, then train
+train_dataloader = fastpropDataLoader(fastpropDataset(descriptors[train_indexes], targets[train_indexes]), shuffle=True)
+val_dataloader = fastpropDataLoader(fastpropDataset(descriptors[val_indexes], targets[val_indexes]))
+test_dataloader = fastpropDataLoader(fastpropDataset(descriptors[test_indexes], targets[test_indexes]))
+model = fastprop(feature_means, feature_vars)
+test_results, validation_results = train_and_test(".", model, train_dataloader, val_dataloader, test_dataloader)
+
+```
+
+### Package Structure
 This section documents where the various modules and functions used in `fastprop` are located.
 Check each file listed for more information, as each contains additional inline documentation useful for development as a Python module.
 To use the core `fastprop` model and dataloaders in your own work, consider looking at `shap.py` or `train.py` which show how to import and instantiate the relevant classes.
 
-### `fastprop`
+#### `fastprop`
  - `defaults`: contains the function `init_logger` used to initialize loggers in different submodules, as well as the default configuration for training.
- - `fastprop_core`: the model itself and convenience functions.
- - `hopt`: hyperparameter optimization using Optuna and Ray\[tune\], used by the CLI.
- - `train`: performs model training, used by the CLI.
- - `predict`: loads models from their checkpoint and config files and runs inference, used by the CLI.
- - `shap`: performs SHAP analysis on a previously trained model, used by the CLI.
- - `preprocessing`: performs all of the preprocessing described above.
-
-### `fastprop.utils`
- - `calculate_descriptors`: wraps the `mordredcommunity` descriptor calculator.
- - `linear_baseline`: trains a basic linear model on the same inputs to `fastprop` to act as a baseline.
- - `descriptor_lists`: hardcoded lists of all of the descriptors implemented in `mordredcommunity`.
- - `select_descriptors`: the script to retrieve the `mordredcommunity` modules based on the strings in the above file (`mordredcommunity` has a weird interface; thus, it is wrapped).
- - `load_data`: short wrappers to `pandas` CSV loading utility, but specialized for the output from `mordredcommunity` and `fastprop`.
- - `validate_config`: _WIP_ validate the input from the command line.
+ - `model`: the model itself and a convenience function for training.
+ - `metrics`: wraps a number of common loss and score functions.
+ - `descriptors`: functions for calculating descriptors.
+ - `data`: functions for cleaning and scaling data.
+ - `io`: functions for loading data from files.
 
-### `fastprop.cli`
+#### `fastprop.cli`
 `fastprop_cli`` contains all the CLI code which is likely not useful in use from a script.
 If you wish to extend the CLI, check the inline documentation there.
 
 # Benchmarks
 The `benchmarks` directory contains the scripts needed to perform the studies (see `benchmarks/README.md` for more detail, they are a great way to learn how to use `fastprop`).
 To just see the results, checkout [`paper/paper.pdf`](https://github.com/JacksonBurns/fastprop/blob/main/paper/paper.pdf) (or `paper/paper.md` for the plain text version).
 
+# Relationship to Chemprop
+In addition to having a similar name, `fastprop` and Chemprop do a similar things: map chemical structures to their corresponding properties in a user-friendly way using machine learning.
+I ([@JacksonBurns](https://github.com/jacksonburns)) am also a developer of Chemprop so some code is inevitably shared between the two (`fastprop` to Chemprop and vice versa).
+
+`fastprop` _feels_ a lot like Chemprop but without a lot of the clutter.
+The `fast` in `fastprop` (both in usage and execution time) comes from the basic architecture, the use of caching, and the reduced configurability of `fastprop` (i.e. I hope you like MSE loss for regression tasks, because that's the only training metric `fastprop` will use via the CLI).
+
 # Developing `fastprop`
 Bug reports, feature requests, and pull requests are welcome and encouraged!
 Follow [this tutorial from GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) to get started.
 
 `fastprop` is built around PyTorch lightning, which defines a rigid API for implementing models that is followed here.
 See the [section on the package layout](#python-module) for information on where all the other functions are, and check out the docstrings and inline comments in each file for more information on what each does.
```

#### html2text {}

```diff
@@ -1,108 +1,98 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.0b4 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.1 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
-lightning Requires-Dist: mordredcommunity Requires-Dist: astartes[molecules]
-Requires-Dist: tensorboard Requires-Dist: psutil Provides-Extra: dev Requires-
-Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
-pytest; extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra ==
-"hopt" Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-
-Dist: shap; extra == "shap" Requires-Dist: matplotlib; extra == "shap"
-Provides-Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
-                                [fastproplogo]
-     ********** FFaasstt MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
+lightning Requires-Dist: torch>=1.13 Requires-Dist: mordredcommunity Requires-
+Dist: astartes[molecules] Requires-Dist: tensorboard Requires-Dist: psutil
+Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: isort;
+extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov;
+extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra == "hopt"
+Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-Dist:
+shap<0.45; extra == "shap" Requires-Dist: matplotlib; extra == "shap" Provides-
+Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
+                                [fastprop Logo]
+        ********** MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
+                    ******** FFaasstt,, SSccaallaabbllee,, aanndd <<550000 LLOOCC ********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
-# Announcement - Open Beta! `fastprop` is currently in the version 3 open beta
-(1.0.0b3)! Please try `fastprop` on your datasets and let us know what you
-think. Feature requests and bug reports are **very** appreciated! Check out the
-demo notebook for quick intro to `fastprop` via Google Colab - runs in your
-browser, GPU included, no install required! _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]# Installing
-`fastprop` `fastprop` supports Mac, Windows, and Linux on Python versions 3.8
-to 3.12. Installing from `pip` or `conda` is the best way to get `fastprop`,
+# Announcements ## alphaXiv The `fastprop` paper is freely available online at
+[arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are
+conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/
+2404.02058) - comments are appreciated! The source for the paper is stored in
+this repository under the `paper` directory. ## Initial Release :tada:
+`fastprop` version 1 is officially released, meaning the API is now stable and
+ready for production use! Please try `fastprop` on your datasets and let us
+know what you think. Feature requests and bug reports are **very** appreciated!
+# Installing `fastprop` `fastprop` supports Mac, Windows, and Linux on Python
+versions 3.8 to 3.12. Installing from `pip` is the best way to get `fastprop`,
 but if you need to check out a specific GitHub branch or you want to contribute
-to `fastprop` a source installation is recommended. ## `pip` [recommended]
-`fastprop` is available via PyPI with `pip install fastprop`. To make extending
-`fastprop` easier and keep the installation size down, dependencies required
-for hyperparameter optimization and SHAP analysis are _optional_. They can be
+to `fastprop` a source installation is recommended. Pending interest from
+users, a `conda` package will be added. Check out the demo notebook for quick
+intro to `fastprop` via Google Colab - runs in your browser, GPU included, no
+install required: [![Open In Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/JacksonBurns/
+fastprop/blob/main/fastprop_demo.ipynb) ## `pip` [recommended] `fastprop` is
+available via PyPI with `pip install fastprop`. To make extending `fastprop`
+easier and keep the installation size down, dependencies required for
+hyperparameter optimization and SHAP analysis are _optional_. They can be
 installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or
 `pip install fastprop[shap,hopt]` to install them both. If you want to use
 `fastprop` but not write new code on top of it, you may want to install these
 now - you can always do so later, however, and `fastprop` will remind you. ##
-`conda` - _coming soon!_ ~~`fastprop` is available from `conda-forge` with
-`conda install -c conda-forge fastprop`.~~ ## Source To install `fastprop` from
-GitHub directly you can: 1. Run `pip install https://github.com/JacksonBurns/
-fastprop.git@main` to install from the `main` branch (or specify any other
-branch you like) 2. Clone the repository with `git clone https://github.com/
-JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run
-`pip install .` To contribute to `fastprop` please follow [this tutorial]
-(https://opensource.com/article/19/7/create-pull-request-github) (or something
-similar) to set up a forked version of `fastprop` and open a pull request
-(similar to above option 2). All contributions are appreciated! See [Developing
-`fastprop`](#developing-fastprop) for more details. # About `fastprop`
-`fastprop` is a package for performing deep-QSPR (Quantitative Structure-
-Property Relationship) with minimal user intervention. By passing in a list of
-SMILES strings, `fastprop` will automatically generate and cache a set of
-molecular descriptors using [`mordredcommunity`](https://github.com/
-JacksonBurns/mordred-community) and train an FNN to predict the corresponding
-properties. See the `examples` and `benchmarks` directories to see how to run
-training - the rest of this documentation will focus on how you can run,
-configure, and customize `fastprop`. ## Paper An academic paper has been
-prepared which describes the `fastprop` approach and walks through the
-`benchmarks` in greater detail. See the `paper` directory for more information.
-## `fastprop` Framework There are four distinct steps in `fastprop` that define
-its framework: 1. Featurization - transform the input molecules (as SMILES
-strings) into an array of molecular descriptors which are saved 2.
+Source To install `fastprop` from GitHub directly you can: 1. Run `pip install
+https://github.com/JacksonBurns/fastprop.git@main` to install from the `main`
+branch (or specify any other branch you like). 2. Clone the repository with
+`git clone https://github.com/JacksonBurns/fastprop.git`, navigate to
+`fastprop` with `cd fastprop`, and run `pip install .` To contribute to
+`fastprop` please follow [this tutorial](https://opensource.com/article/19/7/
+create-pull-request-github) (or something similar) to set up a forked version
+of `fastprop` and open a pull request (similar to above option 2). All
+contributions are appreciated! See [Developing `fastprop`](#developing-
+fastprop) for more details. # About `fastprop` `fastprop` is a package for
+performing deep-QSPR (Quantitative Structure-Property Relationship) with
+minimal user intervention. By passing in a list of SMILES strings, `fastprop`
+will automatically generate and cache a set of molecular descriptors using
+[`mordredcommunity`](https://github.com/JacksonBurns/mordred-community) and
+train an FNN to predict the corresponding properties. See the `examples` and
+`benchmarks` directories to see how to run training - the rest of this
+documentation will focus on how you can run, configure, and customize
+`fastprop`. ## `fastprop` Framework There are four distinct steps in `fastprop`
+that define its framework: 1. Featurization - transform the input molecules (as
+SMILES strings) into an array of molecular descriptors which are saved 2.
 Preprocessing - clean the descriptors by removing or imputing missing values
 then rescaling the remainder 3. Training - send the processed input to the
-neural network, which is a sample FNN (sequential fully-connected layers with
+neural network, which is a simple FNN (sequential fully-connected layers with
 an activation function between) 4. Prediction - save the trained model for
 future use ## Configurable Parameters 1. Featurization - Input CSV file: comma
 separated values (CSV) file (with headers) containing SMILES strings
 representing the molecules and the targets - SMILES column name: name of the
 column containing the SMILES strings - Target column name(s): name(s) of the
 columns containing the targets _and_ - Which `mordred` descriptors to
 calculate: 'all' or 'optimized' (a smaller set of descriptors; faster, but less
 accurate). - Enable/Disable caching of calculated descriptors: `fastprop` will
 by default cache calculated descriptors based on the input filename and warn
-the user when it loads descriptors from the file rather than calculating on the
-fly _or_ - Load precomputed descriptors: filepath to where descriptors are
-already cached either manually or by `fastprop` 2. Preprocessing - Enable/
-Disable dropping of zero-variance parameters (disabled by default; faster, but
-often less accurate) ~~- Enable/Disable dropping of co-linear descriptors
-(disabled by default; faster, decreased accuracy)~~ _WIP_ - _not configurable_:
-`fastprop` will always rescale input features, drop columns with no values, and
-impute missing values with the per-feature mean 3. Training - Number of
-Repeats: How many times to split/train/test on the dataset (increments random
-seed by 1 each time). _and_ - Number of FNN layers (default 2; repeated fully
-connected layers of hidden size) - Hidden Size: number of neurons per FNN layer
-(default 1800) _or_ - Hyperparameter optimization: runs hyperparameter
-optimization identify the optimal number of layers and hidden size _generic NN
-training parameters_ - Output Directory - Learning rate - Batch size ~~-
-Checkpoint file to resume from (optional)~~ _WIP_ - Problem type (one of:
-regression, binary, multiclass (start labels from 0), multilabel) 4. Prediction
-- Input SMILES: either a single SMILES or a CSV file - Output format: filepath
-to write the results or nothing, defaults to stdout - Checkpoints directory:
-directory where previously trained model(s) are ## Relationship to Chemprop In
-addition to having a similar name, `fastprop` and Chemprop do a similar things:
-map chemical structures to their corresponding properties in a user-friendly
-way using machine learning. I ([@JacksonBurns](https://github.com/
-jacksonburns)) am also a developer of Chemprop so some code is inevitably
-shared between the two (`fastprop`->Chemprop and vice versa). `fastprop`
-_feels_ a lot like Chemprop but without a lot of the clutter. The `fast` in
-`fastprop` (both in usage and execution time) comes from the basic
-architecture, the use of caching, and the reduced configurability of `fastprop`
-(i.e. I hope you like MSE loss for regression tasks, because that's the only
-training metric `fastprop` will use). # Using `fastprop` `fastprop` can be run
-from the command line or as a Python module. Regardless of the method of use
-the parameters described in [Configurable Parameters](#configurable-parameters)
-can be modified. Some system-specific configuration options can be specified in
-a `.fastpropconfig` file - see the [example file](https://github.com/
-JacksonBurns/fastprop/blob/main/.fastpropconfig). ## Command Line After
+the user when it loads descriptors from the file rather than calculating on-
+the-fly _or_ - Load precomputed descriptors: filepath to where descriptors are
+already cached either manually or by `fastprop` 2. Preprocessing - _not
+configurable_: `fastprop` will always rescale input features, set invariant and
+missing features to zero, and impute missing values with the per-feature mean
+3. Training - Number of Repeats: How many times to split/train/test on the
+dataset (increments random seed by 1 each time). _and_ - Number of FNN layers
+(default 2; repeated fully connected layers of hidden size) - Hidden Size:
+number of neurons per FNN layer (default 1800) _or_ - Hyperparameter
+optimization: runs hyperparameter optimization identify the optimal number of
+layers and hidden size _generic NN training parameters_ - Output Directory -
+Learning rate - Batch size - Problem type (one of: regression, binary,
+multiclass (start labels from 0), multilabel) 4. Prediction - Input SMILES:
+either a single SMILES or file of SMILES strings on individual lines - Output
+format: filepath to write the results or nothing, defaults to stdout # Using
+`fastprop` `fastprop` can be run from the command line or as a Python module.
+Regardless of the method of use the parameters described in [Configurable
+Parameters](#configurable-parameters) can be modified. ## Command Line After
 installation, `fastprop` is accessible from the command line via `fastprop
 subcommand`, where `subcommand` is either `train`, `predict`, or `shap`. -
 `train` takes in the parameters described in [Configurable Parameters]
 (#configurable-parameters) sections 1, 2, and 3 (featurization, preproccessing,
 and training) and trains `fastprop` model(s) on the input data. - `predict`
 uses the output of a call to `train` to make prediction on arbitrary SMILES
 strings. - `shap` performs SHAP analysis on a trained model to determine which
@@ -113,48 +103,73 @@
 training. It is everything shown in the [Configurable Parameters]
 (#configurable-parameters) section. ### Arguments All of the options shown in
 the [Configuration File](#configuration-file-recommended) section can also be
 passed as command line flags instead of written to a file. When passing the
 arguments, replace all `_` (underscore) with `-` (hyphen), i.e. `fastprop train
 --number-epochs 100` See `fastprop train --help` or `fastprop predict --help`
 for more information. `fastprop shap` and `fastprop predict` have only a couple
-arguments and so do not use configuration files. ## Python Module This section
-documents where the various modules and functions used in `fastprop` are
-located. Check each file listed for more information, as each contains
-additional inline documentation useful for development as a Python module. To
-use the core `fastprop` model and dataloaders in your own work, consider
-looking at `shap.py` or `train.py` which show how to import and instantiate the
-relevant classes. ### `fastprop` - `defaults`: contains the function
-`init_logger` used to initialize loggers in different submodules, as well as
-the default configuration for training. - `fastprop_core`: the model itself and
-convenience functions. - `hopt`: hyperparameter optimization using Optuna and
-Ray\[tune\], used by the CLI. - `train`: performs model training, used by the
-CLI. - `predict`: loads models from their checkpoint and config files and runs
-inference, used by the CLI. - `shap`: performs SHAP analysis on a previously
-trained model, used by the CLI. - `preprocessing`: performs all of the
-preprocessing described above. ### `fastprop.utils` - `calculate_descriptors`:
-wraps the `mordredcommunity` descriptor calculator. - `linear_baseline`: trains
-a basic linear model on the same inputs to `fastprop` to act as a baseline. -
-`descriptor_lists`: hardcoded lists of all of the descriptors implemented in
-`mordredcommunity`. - `select_descriptors`: the script to retrieve the
-`mordredcommunity` modules based on the strings in the above file
-(`mordredcommunity` has a weird interface; thus, it is wrapped). - `load_data`:
-short wrappers to `pandas` CSV loading utility, but specialized for the output
-from `mordredcommunity` and `fastprop`. - `validate_config`: _WIP_ validate the
-input from the command line. ### `fastprop.cli` `fastprop_cli`` contains all
-the CLI code which is likely not useful in use from a script. If you wish to
-extend the CLI, check the inline documentation there. # Benchmarks The
-`benchmarks` directory contains the scripts needed to perform the studies (see
-`benchmarks/README.md` for more detail, they are a great way to learn how to
-use `fastprop`). To just see the results, checkout [`paper/paper.pdf`](https://
-github.com/JacksonBurns/fastprop/blob/main/paper/paper.pdf) (or `paper/
-paper.md` for the plain text version). # Developing `fastprop` Bug reports,
-feature requests, and pull requests are welcome and encouraged! Follow [this
-tutorial from GitHub](https://docs.github.com/en/get-started/exploring-
-projects-on-github/contributing-to-a-project) to get started. `fastprop` is
-built around PyTorch lightning, which defines a rigid API for implementing
-models that is followed here. See the [section on the package layout](#python-
-module) for information on where all the other functions are, and check out the
-docstrings and inline comments in each file for more information on what each
-does. Note that the `pyproject.toml` defines optional `dev` and `bmark`
-packages, which will get you setup with the same dependencies used for CI and
-benchmarking.
+arguments and so do not use configuration files. ## Python Module ### Example
+Here's an example of training `fastprop` as a Python module on the `Arockiaraj`
+Polycyclic Aromatic Hydrocarbon dataset, pulled largely from `fastprop/cli/
+train.py`. With `fastprop` installed you can copy and run this script as-is!
+```python import pandas as pd import torch from fastprop.data import
+( clean_dataset, fastpropDataLoader, fastpropDataset, split, standard_scale, )
+from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
+from fastprop.descriptors import get_descriptors from fastprop.io import
+load_saved_descriptors, read_input_csv from fastprop.model import fastprop,
+train_and_test # prepare the dataset targets, smiles = read_input_csv("https://
+raw.githubusercontent.com/JacksonBurns/fastprop/main/benchmarks/pah/
+arockiaraj_pah_data.csv") targets, rdkit_mols = clean_dataset(targets, smiles)
+descriptors = get_descriptors(".", DESCRIPTOR_SET_LOOKUP["all"], rdkit_mols)
+descriptors = descriptors.to_numpy(dtype=float) descriptors = torch.tensor
+(descriptors, dtype=torch.float32) targets = torch.tensor(targets,
+dtype=torch.float32) # feature scaling train_indexes, val_indexes, test_indexes
+= split(smiles) descriptors[train_indexes], feature_means, feature_vars =
+standard_scale(descriptors[train_indexes]) descriptors[val_indexes] =
+standard_scale(descriptors[val_indexes], feature_means, feature_vars)
+descriptors[test_indexes] = standard_scale(descriptors[test_indexes],
+feature_means, feature_vars) # initialize dataloaders and model, then train
+train_dataloader = fastpropDataLoader(fastpropDataset(descriptors
+[train_indexes], targets[train_indexes]), shuffle=True) val_dataloader =
+fastpropDataLoader(fastpropDataset(descriptors[val_indexes], targets
+[val_indexes])) test_dataloader = fastpropDataLoader(fastpropDataset
+(descriptors[test_indexes], targets[test_indexes])) model = fastprop
+(feature_means, feature_vars) test_results, validation_results = train_and_test
+(".", model, train_dataloader, val_dataloader, test_dataloader) ``` ### Package
+Structure This section documents where the various modules and functions used
+in `fastprop` are located. Check each file listed for more information, as each
+contains additional inline documentation useful for development as a Python
+module. To use the core `fastprop` model and dataloaders in your own work,
+consider looking at `shap.py` or `train.py` which show how to import and
+instantiate the relevant classes. #### `fastprop` - `defaults`: contains the
+function `init_logger` used to initialize loggers in different submodules, as
+well as the default configuration for training. - `model`: the model itself and
+a convenience function for training. - `metrics`: wraps a number of common loss
+and score functions. - `descriptors`: functions for calculating descriptors. -
+`data`: functions for cleaning and scaling data. - `io`: functions for loading
+data from files. #### `fastprop.cli` `fastprop_cli`` contains all the CLI code
+which is likely not useful in use from a script. If you wish to extend the CLI,
+check the inline documentation there. # Benchmarks The `benchmarks` directory
+contains the scripts needed to perform the studies (see `benchmarks/README.md`
+for more detail, they are a great way to learn how to use `fastprop`). To just
+see the results, checkout [`paper/paper.pdf`](https://github.com/JacksonBurns/
+fastprop/blob/main/paper/paper.pdf) (or `paper/paper.md` for the plain text
+version). # Relationship to Chemprop In addition to having a similar name,
+`fastprop` and Chemprop do a similar things: map chemical structures to their
+corresponding properties in a user-friendly way using machine learning. I (
+[@JacksonBurns](https://github.com/jacksonburns)) am also a developer of
+Chemprop so some code is inevitably shared between the two (`fastprop` to
+Chemprop and vice versa). `fastprop` _feels_ a lot like Chemprop but without a
+lot of the clutter. The `fast` in `fastprop` (both in usage and execution time)
+comes from the basic architecture, the use of caching, and the reduced
+configurability of `fastprop` (i.e. I hope you like MSE loss for regression
+tasks, because that's the only training metric `fastprop` will use via the
+CLI). # Developing `fastprop` Bug reports, feature requests, and pull requests
+are welcome and encouraged! Follow [this tutorial from GitHub](https://
+docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-
+project) to get started. `fastprop` is built around PyTorch lightning, which
+defines a rigid API for implementing models that is followed here. See the
+[section on the package layout](#python-module) for information on where all
+the other functions are, and check out the docstrings and inline comments in
+each file for more information on what each does. Note that the
+`pyproject.toml` defines optional `dev` and `bmark` packages, which will get
+you setup with the same dependencies used for CI and benchmarking.
```

### Comparing `fastprop-1.0.0b4/pyproject.toml` & `fastprop-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastprop"
-version = "1.0.0b4"
+version = "1.0.1"
 authors = [
     { name = "Jackson Burns" },
 ]
 license = { text = "MIT" }
 description = "Fast Molecular Property Prediction with mordredcommunity"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 urls = { Homepage = "https://github.com/JacksonBurns/fastprop" }
 requires-python = ">=3.8"
-dependencies = ["pyyaml", "lightning", "mordredcommunity", "astartes[molecules]", "tensorboard", "psutil"]
+dependencies = ["pyyaml", "lightning", "torch>=1.13", "mordredcommunity", "astartes[molecules]", "tensorboard", "psutil"]
 
 [project.optional-dependencies]
-dev = ["black", "isort", "pytest"]
+dev = ["black", "isort", "pytest", "pytest-cov"]
 hopt = ["ray[train]", "optuna"]
-shap = ["shap", "matplotlib"]
+shap = ["shap<0.45", "matplotlib"]
 bmark = ["py2opsin"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
-fastprop = "fastprop.cli.fastprop_cli:main"
+fastprop = "fastprop.cli.base:main"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 150
 
+[tool.autopep8]
+max_line_length = 150
+in-place = true
+recursive = true
+aggressive = 3
+
+[tool.pytest.ini_options]
+addopts = "--cov fastprop"
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["fastprop*"]
 exclude = ["benchmarks*", "examples*", "test*"]
```

### Comparing `fastprop-1.0.0b4/test/test_fastprop.py` & `fastprop-1.0.1/test/test_fastprop.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import shutil
 import unittest
 from pathlib import Path
 
 import yaml
 
-from fastprop import train_fastprop
+from fastprop import DEFAULT_TRAINING_CONFIG
+from fastprop.cli.train import train_fastprop
 
 
 class Test_fastprop(unittest.TestCase):
     """
     Run a shorter benchmark as a functional test, check for regression.
     """
 
@@ -17,21 +18,23 @@
     def setUpClass(cls):
         cls.benchmark_dir = os.path.join(Path(os.path.dirname(__file__)).parent, "benchmarks")
         cls.config_file = os.path.join(cls.benchmark_dir, "pah", "pah.yml")
         cls.temp_dirname = os.path.join(os.path.dirname(__file__), "temp")
 
     def test_pah(self):
         """Run the PAH benchmark."""
+        train_args = dict(DEFAULT_TRAINING_CONFIG)
         with open(self.config_file, "r") as f:
             fastprop_args = yaml.safe_load(f)
             fastprop_args["target_columns"] = fastprop_args["target_columns"].split(" ")
             fastprop_args["output_directory"] = self.temp_dirname
             fastprop_args["input_file"] = os.path.join(self.benchmark_dir, "pah", "arockiaraj_pah_data.csv")
-            res, _ = train_fastprop(**fastprop_args)
-            assert res.describe().loc["mean", "test_r2"] > 0.95
+            train_args.update(fastprop_args)
+            res = train_fastprop(**train_args)
+            assert res.describe().loc["mean", "test_r2_score"] > 0.90
 
     @classmethod
     def tearDownClass(cls):
         shutil.rmtree(cls.temp_dirname, ignore_errors=True)
 
 
 if __name__ == "__main__":
```

