# Comparing `tmp/roodmus-0.0.24.tar.gz` & `tmp/roodmus-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roodmus-0.0.24.tar", last modified: Tue Dec  5 02:34:41 2023, max compression
+gzip compressed data, was "roodmus-0.0.31.tar", last modified: Sun Apr 28 19:08:55 2024, max compression
```

## Comparing `roodmus-0.0.24.tar` & `roodmus-0.0.31.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.286177 roodmus-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-05 02:34:24.000000 roodmus-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    57563 2023-12-05 02:34:41.286177 roodmus-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2023-12-05 02:34:24.000000 roodmus-0.0.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-12-05 02:34:24.000000 roodmus-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 02:34:41.286177 roodmus-0.0.24/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.270177 roodmus-0.0.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.270177 roodmus-0.0.24/src/roodmus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.274177 roodmus-0.0.24/src/roodmus/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/analyse_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    14492 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/plot_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/plot_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25045 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/plot_ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/plot_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)    99779 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/plot_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)    83099 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.274177 roodmus-0.0.24/src/roodmus/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/simulation/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/simulation/orientation_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    32908 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/simulation/run_parakeet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.274177 roodmus-0.0.24/src/roodmus/trajectory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/trajectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26902 2023-12-05 02:34:24.000000 roodmus-0.0.24/src/roodmus/trajectory/conformations_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:34:41.274177 roodmus-0.0.24/src/roodmus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    57563 2023-12-05 02:34:41.000000 roodmus-0.0.24/src/roodmus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-05 02:34:41.000000 roodmus-0.0.24/src/roodmus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 02:34:41.000000 roodmus-0.0.24/src/roodmus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-05 02:34:41.000000 roodmus-0.0.24/src/roodmus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-12-05 02:34:41.000000 roodmus-0.0.24/src/roodmus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-05 02:34:41.000000 roodmus-0.0.24/src/roodmus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.644628 roodmus-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 19:08:40.000000 roodmus-0.0.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    56574 2024-04-28 19:08:55.644628 roodmus-0.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-28 19:08:40.000000 roodmus-0.0.31/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-28 19:08:40.000000 roodmus-0.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:08:55.644628 roodmus-0.0.31/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.624628 roodmus-0.0.31/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.628628 roodmus-0.0.31/src/roodmus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.628628 roodmus-0.0.31/src/roodmus/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/analyse_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/plot_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/plot_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25045 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/plot_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/plot_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100034 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/plot_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91186 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.632628 roodmus-0.0.31/src/roodmus/heterogeneity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/hetRec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44184 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/het_ensemblecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54919 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/het_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/latent_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/plot_heterogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/heterogeneity/remove_hydrogens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.632628 roodmus-0.0.31/src/roodmus/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/simulation/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/simulation/orientation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32908 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/simulation/run_parakeet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20198 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/simulation/write_starfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.632628 roodmus-0.0.31/src/roodmus/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/trajectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28532 2024-04-28 19:08:40.000000 roodmus-0.0.31/src/roodmus/trajectory/conformations_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:08:55.632628 roodmus-0.0.31/src/roodmus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    56574 2024-04-28 19:08:55.000000 roodmus-0.0.31/src/roodmus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-28 19:08:55.000000 roodmus-0.0.31/src/roodmus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:08:55.000000 roodmus-0.0.31/src/roodmus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 19:08:55.000000 roodmus-0.0.31/src/roodmus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-28 19:08:55.000000 roodmus-0.0.31/src/roodmus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 19:08:55.000000 roodmus-0.0.31/src/roodmus.egg-info/top_level.txt
```

### Comparing `roodmus-0.0.24/LICENSE` & `roodmus-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/PKG-INFO` & `roodmus-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roodmus
-Version: 0.0.24
+Version: 0.0.31
 Summary: Synthetic SP micrograph creation and analysis
 Author-email: Joel Greer <joel.greer@stfc.ac.uk>, Maarten Joosten <m.j.joosten@tudelft.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -721,21 +721,22 @@
 Requires-Dist: fake-useragent==1.1.1
 Requires-Dist: fastjsonschema==2.17.1
 Requires-Dist: filelock==3.9.0
 Requires-Dist: fonttools==4.38.0
 Requires-Dist: fqdn==1.5.1
 Requires-Dist: fsspec==2023.1.0
 Requires-Dist: gemmi==0.5.4
+Requires-Dist: gemmi-program==0.6.5
 Requires-Dist: glob2==0.7
 Requires-Dist: guanaco==0.3.0
 Requires-Dist: h5py==3.8.0
 Requires-Dist: HeapDict==1.0.1
 Requires-Dist: identify==2.5.19
 Requires-Dist: idna==3.4
-Requires-Dist: imageio==2.25.0
+Requires-Dist: imageio==2.27.0
 Requires-Dist: importlib-metadata==6.0.0
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: ipykernel==6.24.0
 Requires-Dist: ipython==8.14.0
 Requires-Dist: isoduration==20.11.0
 Requires-Dist: jedi==0.18.2
 Requires-Dist: Jinja2==3.1.2
@@ -750,31 +751,34 @@
 Requires-Dist: jupyter-lsp==2.2.0
 Requires-Dist: jupyter-server==2.7.0
 Requires-Dist: jupyter-server-terminals==0.4.4
 Requires-Dist: jupyterlab==4.0.3
 Requires-Dist: jupyterlab-pygments==0.2.2
 Requires-Dist: jupyterlab-server==2.23.0
 Requires-Dist: kiwisolver==1.4.4
+Requires-Dist: llvmlite==0.41.1
 Requires-Dist: locket==1.0.0
 Requires-Dist: lxml==4.9.2
 Requires-Dist: maptools==0.3.5
 Requires-Dist: MarkupSafe==2.1.2
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: matplotlib-inline==0.1.6
-Requires-Dist: mdtraj==1.9.7
+Requires-Dist: MDAnalysis==2.6.1
+Requires-Dist: mdtraj==1.9.9
 Requires-Dist: mistune==3.0.1
 Requires-Dist: mrcfile==1.4.2
 Requires-Dist: msgpack==1.0.4
 Requires-Dist: nbclient==0.8.0
 Requires-Dist: nbconvert==7.6.0
 Requires-Dist: nbformat==5.9.1
 Requires-Dist: nest-asyncio==1.5.6
 Requires-Dist: networkx==3.0
 Requires-Dist: nodeenv==1.7.0
 Requires-Dist: notebook-shim==0.2.3
+Requires-Dist: numba==0.58.1
 Requires-Dist: numpy==1.23.0
 Requires-Dist: overrides==7.3.1
 Requires-Dist: packaging==23.0
 Requires-Dist: pandas==1.5.3
 Requires-Dist: pandas-stubs==1.5.3.230304
 Requires-Dist: pandocfilters==1.5.0
 Requires-Dist: parse==1.19.0
@@ -792,14 +796,15 @@
 Requires-Dist: psutil==5.9.4
 Requires-Dist: ptyprocess==0.7.0
 Requires-Dist: pure-eval==0.2.2
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==1.10.4
 Requires-Dist: pyee==8.2.2
 Requires-Dist: pygments==2.15.1
+Requires-Dist: pynndescent==0.5.10
 Requires-Dist: pyparsing==3.0.9
 Requires-Dist: pypdb==2.2
 Requires-Dist: pyppeteer==1.0.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-json-logger==2.0.7
@@ -810,38 +815,40 @@
 Requires-Dist: pyzmq==25.1.0
 Requires-Dist: referencing==0.29.1
 Requires-Dist: requests==2.28.2
 Requires-Dist: requests-html==0.10.0
 Requires-Dist: rfc3339-validator==0.1.4
 Requires-Dist: rfc3986-validator==0.1.1
 Requires-Dist: rpds-py==0.8.10
-Requires-Dist: scikit-image==0.19.3
-Requires-Dist: scikit-learn==1.2.1
+Requires-Dist: scikit-image==0.22.0
+Requires-Dist: scikit-learn==1.3.2
 Requires-Dist: scipy==1.9.3
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: send2trash==1.8.2
 Requires-Dist: six==1.16.0
 Requires-Dist: sniffio==1.3.0
 Requires-Dist: sortedcontainers==2.4.0
 Requires-Dist: soupsieve==2.3.2.post1
 Requires-Dist: stack-data==0.6.2
 Requires-Dist: starfile==0.4.11
+Requires-Dist: tbb==2021.10.0
 Requires-Dist: tblib==1.7.0
 Requires-Dist: terminado==0.17.1
 Requires-Dist: threadpoolctl==3.1.0
 Requires-Dist: tifffile==2023.2.3
 Requires-Dist: tinycss2==1.2.1
 Requires-Dist: tomli==2.0.1
 Requires-Dist: toolz==0.12.0
 Requires-Dist: tornado==6.2
 Requires-Dist: tqdm==4.64.0
 Requires-Dist: traitlets==5.9.0
 Requires-Dist: types-pytz==2022.7.1.2
 Requires-Dist: types-tabulate==0.9.0.1
 Requires-Dist: typing_extensions==4.4.0
+Requires-Dist: umap-learn==0.5.4
 Requires-Dist: uri-template==1.3.0
 Requires-Dist: urllib3==1.26.14
 Requires-Dist: virtualenv==20.20.0
 Requires-Dist: w3lib==2.1.1
 Requires-Dist: wcwidth==0.2.6
 Requires-Dist: webcolors==1.13
 Requires-Dist: webencodings==0.5.1
@@ -860,34 +867,33 @@
 
 WIP analysis tools:
 - analysis of latent spaces of heterogeneous reconstruction methods (CryoDRGN, cryoSPARC 3DFlex)
 - comparing the MD trajectory to a latent space
 
 
 ## How to use Roodmus
-The aim of roodmus is to turn an MD trajectory into a set of micrographs that can serve as ground-truth for testing cryo-EM (heterogeneous) reconstruction methods. The core of the micrograph simulation is done using parakeet. The program consists of three modules: 
+The aim of roodmus is to turn an MD trajectory into a set of micrographs that can serve as ground-truth for testing cryo-EM (heterogeneous) reconstruction methods. The core of the micrograph simulation is done using Parakeet. The program consists of three modules: 
 
 ### 1. Sample pdb/mmcif models from trajectory dataset
 Given a directory of trajectory files (in for example .nc or .dcd format) and a topology file (for example a .pdb file), this module saves a selection of frames from the trajectory as .pdb files. The general command used to run this module is:
 ```
 roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR
 ```
 Where N is the number of conformations to be samples from the trajectory. In case N is larger than the number of frames in the trajectory, N will be set equal to the number of frames.
 
-Sampling can be done either evenly or by waymarking. In case of even sampling, frames of the trajectory will be sampled at even intervals. In case of waymarking, a random starting point is selected and new frames are sampled if their rmsd with respect to the sampled frames is larger than a given threshold. The general command used to run conformation sampling in waymarking mode is:
+Sampling can be done in a configurable manner - frames of the trajectory can be sampled at even time intervals from the trajectory or from contiguous frames, from a given starting frame. The general command used to run conformation sampling in waymarking mode is:
 ```
-roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR --rmsd Threshold --sampling_method waymark
+roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR 
 ```
-Where Threshold is the rmsd threshold for sampling a new frame and SEED is the seed for the random starting point. The default value for Threshold is 0.3. More options are availble, see the help page for more information.
 
-Sampled conformations are saved as individual .pdb files in the output directory.
+Sampled conformations are saved as individual .pdb files in the output directory. More options are available as listed by `roodmus conformations_sampling --help`.
 
 
 ### 2. Generate SPA dataset using Parakeet python API:
-Given a directory containing (any) .pdb files, a desired number of images to simulate and a number of molecules per image, this module generates a configuration file to run parakeet and then executes the parakeet simulation. Each micrograph subsamples the .pdb files to the number of molecules to generate, if not enough .pdb files are available, multiple instances of the same file are used. The config file is saved as a .yaml file with the same name as the image it corresponds to. The general command for this module is:
+Given a directory containing (any) .pdb files, a desired number of images to simulate and a number of molecules per image, this module generates a configuration file to run parakeet and then executes the parakeet simulation. Each micrograph subsamples the .pdb files to the number of molecules to generate, if not enough .pdb files are available, multiple instances of files are used. The config file is saved as a .yaml file with the same name as the image it corresponds to. The general command for this module is:
 ```
 roodmus run_parakeet --pdb_dir PATH/TO/PDB/FILES --mrc_dir PATH/TO/OUTPUT/DIR -n N -m M --device "gpu or cpu" 
 ```
 Where N is the number of images to generate and M is the number of molecules per image. There are many more options available for configuring the parakeet simulation. Most have been set to reasonable defaults, but can be changed if desired. See the help page for more information. A list of the most important configuration options:
 - --acceleration_voltage: acceleration voltage in kV. Default: 300
 - --electrons_per_angstrom: total exposure in electrons per Angstrom. Default: 45
 - --dqe: detector quantum efficiency. Uses Parakeet's detector quantum efficiency model. Boolean
@@ -907,32 +913,32 @@
 ```
 Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. The 'scatter' plot type plots the estimated defocus values vs. true defocus for each particle. The 'ctf' plot type plots the CTF in the style of CTFFind4 for the first N micrographs, for both estimated and true defocus parameters.
 
 The second functionality is comparing picked particle positions and true particle positions. This can be done using the following command:
 ```
 roodmus plot_picking --config_dir PATH/TO/CONFIG/FILES --mrc_dir PATH/TO/MRC/FILES --metadata_file PATH/TO/METADATA/FILE.{star, cs} --job_types "particle picking" "2D classification" "..." --plot_dir PATH/TO/PLOT/DIR -N N --plot_types {label_truth, label_picked, label_truth_and_picked, precision, boundary, overlap} --particle_diamter D
 ```
-Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. Multiple metadata files can be loaded in at the same time. Each metadata file can be given a label using the job_types option. metadata files with the same label are grouped together. The labels are used as titles and axis labels in plots. D is the particle diamter in angstroms.
+Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. Multiple metadata files can be loaded in at the same time. Each metadata file can be given a label using the job_types option. Metadata files with the same label are grouped together. The labels are used as titles and axis labels in plots. D is the diameter (in angstroms) used for matching picked and truth particles.
 The 'label_truth' plot type plots the true particle positions on the micrograph for each metadata_file supplied. The 'label_picked' plot type plots the picked particle positions on the micrograph. The 'label_truth_and_picked' plot type plots both the true and picked particle positions on the micrograph. The 'precision' plot type plots the particle picking precision and recall for each job_type. Precision is defined as the number of picked particles closer than particle_diameter/2 to any true particle divided by the total number of picked particles. Recall is defined as the number of true particles with at least one picked particle closer than particle_diameter/2 divided by the total number of true particles.
 The 'boundary' plot type plots the distribution of particles in the micrographs in x-, y- and z-direction. The 'overlap' plot type plots the number of picked particles closer than r to any true particle for a range of r values.
 
 Other functionality includes comparing estimated particle orientations to true particle orientations and plotting precision for 2D classes. See the help page for more information:
 ```
 roodmus --help
 ```
 or
 ```
 roodmus {plot_picking, plot_ctf, plot_alignment, plot_2d_lasses, plot_frames} --help
 ```
 
 # Licensing
-Need to figure out what kind of license we want and when/how we need to get it for the repo. May have to use the same licence as parakeet.
+Roodmus is GPLv3 licensed. Please see the `LICENSE` file for information on usage, reproduction or adaptation of the Roodmus codebase.
 
 # Parakeet Compatibility
-Code is currently tested with parakeet commit `024b86ebf55adf737c1b1116b8adbb59ee7db491`. Functionality is expected to be easily extended to the most recent version as of 9/3/23. This may required a small number of Parakeet config variables to be added/modified in the configuration class.
+Code is currently tested with parakeet tag [v0.4.3.dev1](https://github.com/rosalindfranklininstitute/parakeet/releases/tag/v0.4.3.dev1). Functionality is expected to be easily extended to the most recent version as of 9/3/23. This may required a small number of Parakeet config variables to be added/modified in the configuration class.
 
 # flow chart of current structure of Roodmus
 ![flowchart](docs/flowchart.png)
 
 # Setting up Roodmus
 ## On a PC
 From creating a new python environment (assumed conda/anaconda installed) to being able to develop and run roodmus. They assume that FFTW is in the system path (used for python-multem/guanaco). The number used for CMAKE_CUDA_ARCHITECTURES number will depend on you GPU. <https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/> can be a useful reference to find it for your GPU.
@@ -969,28 +975,7 @@
 pip install -e .
 cd../
 
 cd ccpem-pipeliner
 pip install -e .
 ```
 After doing so, an editable install of roodmus should be set up with all requisite packages.
-
-# Updating roodmus As A pip Package
-I do this via twine:
-`python3 -m pip install --upgrade twine`
-
-If there's any updates, you need to update the version number (configured in the pyproject.toml). Make sure it is suitable according to pep conventions! Currently updating this is manual.
-
-Build the updated package via:
-
-`python3 -m pip install --upgrade build`
-
-`python3 -m build`
-
-Once you've done that, you can publish the package via:
-`python3 -m twine upload --repository testpypi dist/*<version>*`
-
-To do this you'll need an account and token (instructions here: <https://packaging.python.org/en/latest/tutorials/packaging-projects/>)
-
-If you want to download the pip package from the remote repository (currently the pypi test repo) and install it, you can do this via:
-`python3 -m pip install --extra-index-url https://test.pypi.org/simple/  roodmus --no-cache-dir`
-You can also pip install it via the tar'ed dist package or the pip wheel (.whl file) found in the dist directory.
```

### Comparing `roodmus-0.0.24/README.md` & `roodmus-0.0.31/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 WIP analysis tools:
 - analysis of latent spaces of heterogeneous reconstruction methods (CryoDRGN, cryoSPARC 3DFlex)
 - comparing the MD trajectory to a latent space
 
 
 ## How to use Roodmus
-The aim of roodmus is to turn an MD trajectory into a set of micrographs that can serve as ground-truth for testing cryo-EM (heterogeneous) reconstruction methods. The core of the micrograph simulation is done using parakeet. The program consists of three modules: 
+The aim of roodmus is to turn an MD trajectory into a set of micrographs that can serve as ground-truth for testing cryo-EM (heterogeneous) reconstruction methods. The core of the micrograph simulation is done using Parakeet. The program consists of three modules: 
 
 ### 1. Sample pdb/mmcif models from trajectory dataset
 Given a directory of trajectory files (in for example .nc or .dcd format) and a topology file (for example a .pdb file), this module saves a selection of frames from the trajectory as .pdb files. The general command used to run this module is:
 ```
 roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR
 ```
 Where N is the number of conformations to be samples from the trajectory. In case N is larger than the number of frames in the trajectory, N will be set equal to the number of frames.
 
-Sampling can be done either evenly or by waymarking. In case of even sampling, frames of the trajectory will be sampled at even intervals. In case of waymarking, a random starting point is selected and new frames are sampled if their rmsd with respect to the sampled frames is larger than a given threshold. The general command used to run conformation sampling in waymarking mode is:
+Sampling can be done in a configurable manner - frames of the trajectory can be sampled at even time intervals from the trajectory or from contiguous frames, from a given starting frame. The general command used to run conformation sampling in waymarking mode is:
 ```
-roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR --rmsd Threshold --sampling_method waymark
+roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR 
 ```
-Where Threshold is the rmsd threshold for sampling a new frame and SEED is the seed for the random starting point. The default value for Threshold is 0.3. More options are availble, see the help page for more information.
 
-Sampled conformations are saved as individual .pdb files in the output directory.
+Sampled conformations are saved as individual .pdb files in the output directory. More options are available as listed by `roodmus conformations_sampling --help`.
 
 
 ### 2. Generate SPA dataset using Parakeet python API:
-Given a directory containing (any) .pdb files, a desired number of images to simulate and a number of molecules per image, this module generates a configuration file to run parakeet and then executes the parakeet simulation. Each micrograph subsamples the .pdb files to the number of molecules to generate, if not enough .pdb files are available, multiple instances of the same file are used. The config file is saved as a .yaml file with the same name as the image it corresponds to. The general command for this module is:
+Given a directory containing (any) .pdb files, a desired number of images to simulate and a number of molecules per image, this module generates a configuration file to run parakeet and then executes the parakeet simulation. Each micrograph subsamples the .pdb files to the number of molecules to generate, if not enough .pdb files are available, multiple instances of files are used. The config file is saved as a .yaml file with the same name as the image it corresponds to. The general command for this module is:
 ```
 roodmus run_parakeet --pdb_dir PATH/TO/PDB/FILES --mrc_dir PATH/TO/OUTPUT/DIR -n N -m M --device "gpu or cpu" 
 ```
 Where N is the number of images to generate and M is the number of molecules per image. There are many more options available for configuring the parakeet simulation. Most have been set to reasonable defaults, but can be changed if desired. See the help page for more information. A list of the most important configuration options:
 - --acceleration_voltage: acceleration voltage in kV. Default: 300
 - --electrons_per_angstrom: total exposure in electrons per Angstrom. Default: 45
 - --dqe: detector quantum efficiency. Uses Parakeet's detector quantum efficiency model. Boolean
@@ -55,32 +54,32 @@
 ```
 Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. The 'scatter' plot type plots the estimated defocus values vs. true defocus for each particle. The 'ctf' plot type plots the CTF in the style of CTFFind4 for the first N micrographs, for both estimated and true defocus parameters.
 
 The second functionality is comparing picked particle positions and true particle positions. This can be done using the following command:
 ```
 roodmus plot_picking --config_dir PATH/TO/CONFIG/FILES --mrc_dir PATH/TO/MRC/FILES --metadata_file PATH/TO/METADATA/FILE.{star, cs} --job_types "particle picking" "2D classification" "..." --plot_dir PATH/TO/PLOT/DIR -N N --plot_types {label_truth, label_picked, label_truth_and_picked, precision, boundary, overlap} --particle_diamter D
 ```
-Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. Multiple metadata files can be loaded in at the same time. Each metadata file can be given a label using the job_types option. metadata files with the same label are grouped together. The labels are used as titles and axis labels in plots. D is the particle diamter in angstroms.
+Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. Multiple metadata files can be loaded in at the same time. Each metadata file can be given a label using the job_types option. Metadata files with the same label are grouped together. The labels are used as titles and axis labels in plots. D is the diameter (in angstroms) used for matching picked and truth particles.
 The 'label_truth' plot type plots the true particle positions on the micrograph for each metadata_file supplied. The 'label_picked' plot type plots the picked particle positions on the micrograph. The 'label_truth_and_picked' plot type plots both the true and picked particle positions on the micrograph. The 'precision' plot type plots the particle picking precision and recall for each job_type. Precision is defined as the number of picked particles closer than particle_diameter/2 to any true particle divided by the total number of picked particles. Recall is defined as the number of true particles with at least one picked particle closer than particle_diameter/2 divided by the total number of true particles.
 The 'boundary' plot type plots the distribution of particles in the micrographs in x-, y- and z-direction. The 'overlap' plot type plots the number of picked particles closer than r to any true particle for a range of r values.
 
 Other functionality includes comparing estimated particle orientations to true particle orientations and plotting precision for 2D classes. See the help page for more information:
 ```
 roodmus --help
 ```
 or
 ```
 roodmus {plot_picking, plot_ctf, plot_alignment, plot_2d_lasses, plot_frames} --help
 ```
 
 # Licensing
-Need to figure out what kind of license we want and when/how we need to get it for the repo. May have to use the same licence as parakeet.
+Roodmus is GPLv3 licensed. Please see the `LICENSE` file for information on usage, reproduction or adaptation of the Roodmus codebase.
 
 # Parakeet Compatibility
-Code is currently tested with parakeet commit `024b86ebf55adf737c1b1116b8adbb59ee7db491`. Functionality is expected to be easily extended to the most recent version as of 9/3/23. This may required a small number of Parakeet config variables to be added/modified in the configuration class.
+Code is currently tested with parakeet tag [v0.4.3.dev1](https://github.com/rosalindfranklininstitute/parakeet/releases/tag/v0.4.3.dev1). Functionality is expected to be easily extended to the most recent version as of 9/3/23. This may required a small number of Parakeet config variables to be added/modified in the configuration class.
 
 # flow chart of current structure of Roodmus
 ![flowchart](docs/flowchart.png)
 
 # Setting up Roodmus
 ## On a PC
 From creating a new python environment (assumed conda/anaconda installed) to being able to develop and run roodmus. They assume that FFTW is in the system path (used for python-multem/guanaco). The number used for CMAKE_CUDA_ARCHITECTURES number will depend on you GPU. <https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/> can be a useful reference to find it for your GPU.
@@ -117,28 +116,7 @@
 pip install -e .
 cd../
 
 cd ccpem-pipeliner
 pip install -e .
 ```
 After doing so, an editable install of roodmus should be set up with all requisite packages.
-
-# Updating roodmus As A pip Package
-I do this via twine:
-`python3 -m pip install --upgrade twine`
-
-If there's any updates, you need to update the version number (configured in the pyproject.toml). Make sure it is suitable according to pep conventions! Currently updating this is manual.
-
-Build the updated package via:
-
-`python3 -m pip install --upgrade build`
-
-`python3 -m build`
-
-Once you've done that, you can publish the package via:
-`python3 -m twine upload --repository testpypi dist/*<version>*`
-
-To do this you'll need an account and token (instructions here: <https://packaging.python.org/en/latest/tutorials/packaging-projects/>)
-
-If you want to download the pip package from the remote repository (currently the pypi test repo) and install it, you can do this via:
-`python3 -m pip install --extra-index-url https://test.pypi.org/simple/  roodmus --no-cache-dir`
-You can also pip install it via the tar'ed dist package or the pip wheel (.whl file) found in the dist directory.
```

### Comparing `roodmus-0.0.24/pyproject.toml` & `roodmus-0.0.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roodmus"
-version = "0.0.24"
+version = "0.0.31"
 authors = [
   { name="Joel Greer", email="joel.greer@stfc.ac.uk" },
   { name="Maarten Joosten", email="m.j.joosten@tudelft.nl" },
 ]
 description = "Synthetic SP micrograph creation and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
@@ -54,21 +54,22 @@
   "fake-useragent==1.1.1",
   "fastjsonschema==2.17.1",
   "filelock==3.9.0",
   "fonttools==4.38.0",
   "fqdn==1.5.1",
   "fsspec==2023.1.0",
   "gemmi==0.5.4",
+  "gemmi-program==0.6.5",
   "glob2==0.7",
   "guanaco==0.3.0",
   "h5py==3.8.0",
   "HeapDict==1.0.1",
   "identify==2.5.19",
   "idna==3.4",
-  "imageio==2.25.0",
+  "imageio==2.27.0",
   "importlib-metadata==6.0.0",
   "iniconfig==2.0.0",
   "ipykernel==6.24.0",
   "ipython==8.14.0",
   "isoduration==20.11.0",
   "jedi==0.18.2",
   "Jinja2==3.1.2",
@@ -83,31 +84,34 @@
   "jupyter-lsp==2.2.0",
   "jupyter-server==2.7.0",
   "jupyter-server-terminals==0.4.4",
   "jupyterlab==4.0.3",
   "jupyterlab-pygments==0.2.2",
   "jupyterlab-server==2.23.0",
   "kiwisolver==1.4.4",
+  "llvmlite==0.41.1",
   "locket==1.0.0",
   "lxml==4.9.2",
   "maptools==0.3.5",
   "MarkupSafe==2.1.2",
   "matplotlib==3.5.2",
   "matplotlib-inline==0.1.6",
-  "mdtraj==1.9.7",
+  "MDAnalysis==2.6.1",
+  "mdtraj==1.9.9",
   "mistune==3.0.1",
   "mrcfile==1.4.2",
   "msgpack==1.0.4",
   "nbclient==0.8.0",
   "nbconvert==7.6.0",
   "nbformat==5.9.1",
   "nest-asyncio==1.5.6",
   "networkx==3.0",
   "nodeenv==1.7.0",
   "notebook-shim==0.2.3",
+  "numba==0.58.1",
   "numpy==1.23.0",
   "overrides==7.3.1",
   "packaging==23.0",
   "pandas==1.5.3",
   "pandas-stubs==1.5.3.230304",
   "pandocfilters==1.5.0",
   "parse==1.19.0",
@@ -125,14 +129,15 @@
   "psutil==5.9.4",
   "ptyprocess==0.7.0",
   "pure-eval==0.2.2",
   "pycparser==2.21",
   "pydantic==1.10.4",
   "pyee==8.2.2",
   "pygments==2.15.1",
+  "pynndescent==0.5.10",
   "pyparsing==3.0.9",
   "pypdb==2.2",
   "pyppeteer==1.0.2",
   "pyquery==2.0.0",
   "pytest==7.4.0",
   "python-dateutil==2.8.2",
   "python-json-logger==2.0.7",
@@ -143,38 +148,40 @@
   "pyzmq==25.1.0",
   "referencing==0.29.1",
   "requests==2.28.2",
   "requests-html==0.10.0",
   "rfc3339-validator==0.1.4",
   "rfc3986-validator==0.1.1",
   "rpds-py==0.8.10",
-  "scikit-image==0.19.3",
-  "scikit-learn==1.2.1",
+  "scikit-image==0.22.0",
+  "scikit-learn==1.3.2",
   "scipy==1.9.3",
   "seaborn==0.12.2",
   "send2trash==1.8.2",
   "six==1.16.0",
   "sniffio==1.3.0",
   "sortedcontainers==2.4.0",
   "soupsieve==2.3.2.post1",
   "stack-data==0.6.2",
   "starfile==0.4.11",
+  "tbb==2021.10.0",
   "tblib==1.7.0",
   "terminado==0.17.1",
   "threadpoolctl==3.1.0",
   "tifffile==2023.2.3",
   "tinycss2==1.2.1",
   "tomli==2.0.1",
   "toolz==0.12.0",
   "tornado==6.2",
   "tqdm==4.64.0",
   "traitlets==5.9.0",
   "types-pytz==2022.7.1.2",
   "types-tabulate==0.9.0.1",
   "typing_extensions==4.4.0",
+  "umap-learn==0.5.4",
   "uri-template==1.3.0",
   "urllib3==1.26.14",
   "virtualenv==20.20.0",
   "w3lib==2.1.1",
   "wcwidth==0.2.6",
   "webcolors==1.13",
   "webencodings==0.5.1",
@@ -189,8 +196,8 @@
 
 [project.urls]
 "Homepage" = "https://github.com/ccpem/roodmus"
 "Bug Tracker" = "https://github.com/ccpem/roodmus/issues"
 
 [tool.licensecheck]
 using = "requirements:requirements.txt;requirements-dev.txt"
-format = "json"
+format = "json"
```

### Comparing `roodmus-0.0.24/src/roodmus/analysis/analyse_alignment.py` & `roodmus-0.0.31/src/roodmus/analysis/analyse_alignment.py`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/src/roodmus/analysis/extract_particles.py` & `roodmus-0.0.31/src/roodmus/analysis/extract_particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     return parser
 
 
 def get_name():
     return "extract_particles"
 
 
-def get_num_molecules(metadata):
+def get_num_molecules(metadata: dict) -> int:
     num_molecules = 0
     for molecule in metadata["sample"]["molecules"]["local"]:
         if type(molecule["instances"]) == int:
             num_molecules += int(molecule["instances"])
         elif type(molecule["instances"]) == list:
             num_molecules += len(molecule["instances"])
     return num_molecules
```

### Comparing `roodmus-0.0.24/src/roodmus/analysis/plot_alignment.py` & `roodmus-0.0.31/src/roodmus/analysis/plot_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,18 @@
 
 def true_pose_distribution_plot(
     df_truth: pd.DataFrame,
     vmin: float | None = None,
     vmax: float | None = None,
 ):
     df_truth["euler_phi"] = df_truth["euler_phi"].astype(float)
-    df_truth["euler_theta"] = -(
-        df_truth["euler_theta"].astype(float) - np.pi / 2
-    )
+    df_truth["euler_theta"] = df_truth["euler_theta"].astype(float)
+    # df_truth["euler_theta"] = -(
+    #     df_truth["euler_theta"].astype(float) - np.pi / 2
+    # )
     df_truth["euler_psi"] = df_truth["euler_psi"].astype(float)
 
     grid = sns.jointplot(
         x="euler_phi",
         y="euler_theta",
         data=df_truth,
         kind="hex",
@@ -190,31 +191,31 @@
             np.pi / 2,
             3 / 4 * np.pi,
             np.pi,
         ]
     )
     grid.ax_joint.set_xticklabels(
         [
-            "\u03C0",
+            "-\u03C0",
             "-3/4\u03C0",
             "-\u03C0/2",
             "-\u03C0/4",
             "0",
             "\u03C0/4",
             "\u03C0/2",
             "3/4\u03C0",
             "\u03C0",
         ]
     )
-    grid.ax_joint.set_yticks([-np.pi / 2, -np.pi / 4, 0, np.pi / 4, np.pi / 2])
+    grid.ax_joint.set_yticks([0, np.pi / 4, np.pi / 2, 3 / 4 * np.pi, np.pi])
     grid.ax_joint.set_yticklabels(
-        ["\u03C0/2", "\u03C0/4", "0", "\u03C0/4", "\u03C0/2"]
+        ["0", "\u03C0/4", "\u03C0/2", "3/4\u03C0", "\u03C0"]
     )
     grid.ax_joint.set_xlabel("Azimuth")
-    grid.ax_joint.set_ylabel("Elevation")
+    grid.ax_joint.set_ylabel("Tilt")
     # add new sublot to the right of the jointplot
     cbar_ax = grid.fig.add_axes([1, 0.15, 0.02, 0.7])
     # add colorbar to the new subplot
     grid.fig.colorbar(grid.ax_joint.collections[0], cax=cbar_ax, label="count")
     if vmin and vmax:
         # set limits of the colorbar to the same as for
         # the picked particles
@@ -271,15 +272,19 @@
             pd.DataFrame,
         ):
             for i, meta_file in enumerate(
                 self.plot_data["plot_picked_pose_distribution"]["df_picked"][
                     "metadata_filename"
                 ].unique()
             ):
-                self.grid, self.vmin, self.vmax = picked_pose_distribution(
+                (
+                    self.grid,
+                    self.vmin,
+                    self.vmax,
+                ) = picked_pose_distribution_plot(
                     self.plot_data["plot_picked_pose_distribution"][
                         "df_picked"
                     ],
                     meta_file,
                 )
 
                 if i == 0:
@@ -306,37 +311,37 @@
         self.grid.savefig(outfilename, dpi=self.dpi, bbox_inches="tight")
         if self.pdf:
             self.grid.savefig(
                 outfilename.replace(".png", ".pdf"), bbox_inches="tight"
             )
 
 
-def picked_pose_distribution(
+def picked_pose_distribution_plot(
     df_picked: pd.DataFrame,
     metadata_filename: str | List[str],
     vmin: float | None = None,
     vmax: float | None = None,
 ):
     # group the picked particles by metadata file
     if isinstance(metadata_filename, list):
         metadata_filename = metadata_filename[0]
     df_picked_grouped = df_picked.groupby("metadata_filename").get_group(
         metadata_filename
     )
 
     # change data type of column euler_phi to float
-    df_picked_grouped["euler_phi"] = df_picked_grouped["euler_phi"].astype(
-        float
-    )
-    df_picked_grouped["euler_theta"] = -(
-        df_picked_grouped["euler_theta"].astype(float) - np.pi / 2
-    )
-    df_picked_grouped["euler_psi"] = df_picked_grouped["euler_psi"].astype(
-        float
-    )
+    # df_picked_grouped["euler_phi"] = df_picked_grouped["euler_phi"].astype(
+    #     float
+    # )
+    # df_picked_grouped["euler_theta"] = -(
+    #     df_picked_grouped["euler_theta"].astype(float) - np.pi / 2
+    # )
+    # df_picked_grouped["euler_psi"] = df_picked_grouped["euler_psi"].astype(
+    #     float
+    # )
 
     # plot the alignment
     grid = sns.jointplot(
         x="euler_phi",
         y="euler_theta",
         data=df_picked_grouped,
         kind="hex",
@@ -359,31 +364,31 @@
             np.pi / 2,
             3 / 4 * np.pi,
             np.pi,
         ]
     )
     grid.ax_joint.set_xticklabels(
         [
-            "\u03C0",
+            "-\u03C0",
             "-3/4\u03C0",
             "-\u03C0/2",
             "-\u03C0/4",
             "0",
             "\u03C0/4",
             "\u03C0/2",
             "3/4\u03C0",
             "\u03C0",
         ]
     )
-    grid.ax_joint.set_yticks([-np.pi / 2, -np.pi / 4, 0, np.pi / 4, np.pi / 2])
+    grid.ax_joint.set_yticks([0, np.pi / 4, np.pi / 2, 3 / 4 * np.pi, np.pi])
     grid.ax_joint.set_yticklabels(
-        ["-\u03C0/2", "-\u03C0/4", "0", "\u03C0/4", "\u03C0/2"]
+        ["0", "\u03C0/4", "\u03C0/2", "3/4\u03C0", "\u03C0"]
     )
     grid.ax_joint.set_xlabel("Azimuth")
-    grid.ax_joint.set_ylabel("Elevation")
+    grid.ax_joint.set_ylabel("Tilt")
     # add new sublot to the right of the jointplot
     cbar_ax = grid.fig.add_axes([1, 0.15, 0.02, 0.7])
     # add colorbar to the new subplot
     grid.fig.colorbar(grid.ax_joint.collections[0], cax=cbar_ax, label="count")
     if vmin and vmax:
         # set limits of the colorbar to the
         # same as for the picked particles
```

### Comparing `roodmus-0.0.24/src/roodmus/analysis/plot_classes.py` & `roodmus-0.0.31/src/roodmus/analysis/plot_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 
 import argparse
 import os
 
+# from typing import Tuple, Dict, Any
+
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from scipy.ndimage import zoom
 
 from roodmus.analysis.utils import load_data, plotDataFrame
@@ -242,22 +244,23 @@
     }
     for groupname in df_grouped.groupby("class2D").groups.keys():
         precision = df_grouped.groupby("class2D").get_group(groupname)[
             "TP"
         ].sum() / (
             df_grouped.groupby("class2D").get_group(groupname)["TP"].size
         )
-        results["class2D"].append(int(groupname))
+        results["class2D"].append(groupname)
         results["precision"].append(precision)
         results["average defocus"].append(
             df_grouped.groupby("class2D")
             .get_group(groupname)["defocusU"]
             .mean()
         )
     df = pd.DataFrame(results)
+    df["class2D"] = df["class2D"].astype(int)
     fig, ax = plt.subplots(figsize=(7, 3.5))
     sns.barplot(x="class2D", y="precision", data=df, ax=ax, palette=palette)
     ax.set_xlabel("class2D", fontsize=12)
     ax.set_ylabel("precision", fontsize=12)
     ax.set_title(job_types[metadata_filename], fontsize=14)
     xticklabels = ax.get_xticklabels()
     ax.set_xticklabels(xticklabels, rotation=45, fontsize=6)
@@ -270,26 +273,37 @@
     metadata_filename: str,
     bin_factor: int = 100,
     palette="YlGnBu",
 ):
     df_filtered = df_picked.groupby("metadata_filename").get_group(
         metadata_filename
     )
-    df_grouped = df_filtered.groupby(["class2D", "closest_pdb_index"])
+    # df_grouped = df_filtered.groupby(["class2D", "closest_pdb_index"])
     heatmap = np.zeros(
         (
             int(np.max(df_filtered["class2D"])) + 1,
             int(np.max(df_filtered["closest_pdb_index"])) + 1,
         )
     )
-    for class_id, pdb_id in df_grouped.groups.keys():
-        if int(class_id) > 0 and int(pdb_id) > 0:
-            num = df_grouped.get_group((class_id, pdb_id)).size
-            if num != np.nan:
-                heatmap[int(class_id), int(pdb_id)] += num
+    # class_id: float
+    # pdb_id: float
+    # df_grouped.groups: Dict[Tuple[float, float], pd.Index[Any]]
+    # for class_id, pdb_id in df_grouped.groups.keys():
+    #     if not np.isnan(class_id) and not np.isnan(pdb_id):
+
+    for class_id in df_filtered["class2D"].unique():
+        for pdb_id in df_filtered["closest_pdb_index"].unique():
+            if not np.isnan(class_id) and not np.isnan(pdb_id):
+                # num = df_grouped.get_group((class_id, pdb_id)).size
+                num = df_filtered[
+                    (df_filtered["class2D"] == class_id)
+                    & (df_filtered["closest_pdb_index"] == pdb_id)
+                ].size
+                if num != np.nan:
+                    heatmap[int(class_id), int(pdb_id)] += num
 
     # apply binning to the heatmap
     heatmap = zoom(heatmap, [1, 1 / bin_factor], order=0)
     heatmap[heatmap == 0] = np.nan
 
     fig, ax = plt.subplots(figsize=(15, 5))
     sns.heatmap(heatmap, ax=ax, cmap=palette)
```

### Comparing `roodmus-0.0.24/src/roodmus/analysis/plot_ctf.py` & `roodmus-0.0.31/src/roodmus/analysis/plot_ctf.py`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/src/roodmus/analysis/plot_frames.py` & `roodmus-0.0.31/src/roodmus/analysis/plot_frames.py`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/src/roodmus/analysis/plot_picking.py` & `roodmus-0.0.31/src/roodmus/analysis/plot_picking.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 
 import os
-from typing import Tuple, Dict
+from typing import Tuple, Dict, List
 
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from matplotlib import patches
 import numpy as np
 import mrcfile
@@ -132,15 +132,15 @@
     return "plot_picking"
 
 
 class plotLabelTruth(plotDataFrame):
     def __init__(
         self,
         mrc_dir: str,
-        plot_data: dict[str, dict[str, pd.DataFrame]] | None = None,
+        plot_data: Dict[str, Dict[str, pd.DataFrame]] | None = None,
         plot_dir: str = "",
         num_ugraphs: int | None = None,
         box_width: float = 200,
         box_height: float = 200,
         dpi: int = 300,
         pdf: bool = False,
         verbose: bool = False,
@@ -1609,15 +1609,15 @@
     @staticmethod
     def _twoD_image_bboxs(
         particles_x: np.ndarray,
         particles_y: np.ndarray,
         box_width: float,
         box_height: float,
         verbose: bool = False,
-    ) -> list[list[float]]:
+    ) -> List[List[float]]:
         box_half_width = box_width / 2.0
         box_half_height = box_height / 2.0
 
         if verbose:
             print(
                 "Using box half width: {} and half height: {}".format(
                     box_half_width, box_half_height
@@ -1668,16 +1668,16 @@
             fig, ax = plt.subplots(figsize=[14, 14])
             ax.imshow(data[0], cmap="gray")
             fig.tight_layout()
 
             # Now that you've plotted the true central points of each particle,
             # also plot the boxes
             boxes = labelMicrograph._twoD_image_bboxs(
-                particles_ugraph["position_x"],
-                particles_ugraph["position_y"],
+                np.array(particles_ugraph["position_x"]),
+                np.array(particles_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -1735,16 +1735,16 @@
             fig, ax = plt.subplots(figsize=[14, 14])
             ax.imshow(data[0], cmap="gray")
             fig.tight_layout()
 
             # Now that you've plotted the true central points of each particle,
             # also plot the boxes
             boxes = labelMicrograph._twoD_image_bboxs(
-                particles_ugraph["position_x"],
-                particles_ugraph["position_y"],
+                np.array(particles_ugraph["position_x"]),
+                np.array(particles_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -1773,15 +1773,15 @@
             ax.set_xticklabels([])
             ax.set_yticklabels([])
         return fig, ax
 
     @staticmethod
     def label_micrograph_truth_and_picked(
         picked_particles: pd.DataFrame,
-        metadata_filename: str | list[str],
+        metadata_filename: str | List[str],
         truth_particles: pd.DataFrame,
         ugraph_index: int = 0,
         mrc_dir: str = "",
         box_width: float = 50,
         box_height: float = 50,
         picked_color: list = [1, 0, 0],
         truth_color: list = [0, 1, 0],
@@ -1813,16 +1813,16 @@
             fig, ax = plt.subplots(figsize=[14, 14])
             ax.imshow(data[0], cmap="gray")
             fig.tight_layout()
 
             # Now that you've plotted the true central points of each particle,
             # also plot the boxes
             boxes = labelMicrograph._twoD_image_bboxs(
-                picked_particles_ugraph["position_x"],
-                picked_particles_ugraph["position_y"],
+                np.array(picked_particles_ugraph["position_x"]),
+                np.array(picked_particles_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -1837,16 +1837,16 @@
                     linewidth=1,
                     edgecolor=picked_color,
                     facecolor="none",
                 )
                 ax.add_patch(rect)
 
             boxes = labelMicrograph._twoD_image_bboxs(
-                truth_particles_ugraph["position_x"],
-                truth_particles_ugraph["position_y"],
+                np.array(truth_particles_ugraph["position_x"]),
+                np.array(truth_particles_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -1903,16 +1903,16 @@
             fig, ax = plt.subplots(figsize=[14, 14])
             ax.imshow(data[0], cmap="gray")
             fig.tight_layout()
 
             # Now that you've plotted the true central points of each particle,
             # also plot the boxes
             boxes = labelMicrograph._twoD_image_bboxs(
-                truth_particles1_ugraph["position_x"],
-                truth_particles1_ugraph["position_y"],
+                np.array(truth_particles1_ugraph["position_x"]),
+                np.array(truth_particles1_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -1927,16 +1927,16 @@
                     linewidth=1,
                     edgecolor=truth_color1,
                     facecolor="none",
                 )
                 ax.add_patch(rect)
 
             boxes = labelMicrograph._twoD_image_bboxs(
-                truth_particles2_ugraph["position_x"],
-                truth_particles2_ugraph["position_y"],
+                np.array(truth_particles2_ugraph["position_x"]),
+                np.array(truth_particles2_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -1957,15 +1957,15 @@
             ax.set_yticklabels([])
         return fig, ax
 
     @staticmethod
     def label_micrograph_picked_and_picked(
         picked_particles1: pd.DataFrame,
         picked_particles2: pd.DataFrame,
-        metadata_filename: str | list[str],
+        metadata_filename: str | List[str],
         truth_particles: pd.DataFrame,
         ugraph_index: int = 0,
         mrc_dir: str = "",
         box_width: float = 50,
         box_height: float = 50,
         picked1_color: list = [1, 0, 0],
         picked2_color: list = [0, 1, 0],
@@ -2000,16 +2000,16 @@
             fig, ax = plt.subplots(figsize=[14, 14])
             ax.imshow(data[0], cmap="gray")
             fig.tight_layout()
 
             # Now that you've plotted the true central points of each particle,
             # also plot the boxes
             boxes = labelMicrograph._twoD_image_bboxs(
-                picked_particles1_ugraph["position_x"],
-                picked_particles1_ugraph["position_y"],
+                np.array(picked_particles1_ugraph["position_x"]),
+                np.array(picked_particles1_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -2024,16 +2024,16 @@
                     linewidth=1,
                     edgecolor=picked1_color,
                     facecolor="none",
                 )
                 ax.add_patch(rect)
 
             boxes = labelMicrograph._twoD_image_bboxs(
-                picked_particles2_ugraph["position_x"],
-                picked_particles2_ugraph["position_y"],
+                np.array(picked_particles2_ugraph["position_x"]),
+                np.array(picked_particles2_ugraph["position_y"]),
                 box_width,
                 box_height,
                 verbose,
             )
             if verbose:
                 print(f"number of boxes: {len(boxes)}")
 
@@ -2211,21 +2211,21 @@
         )
     # remove legend
     ax.legend().remove()
     # add colorbar
     sm = plt.cm.ScalarMappable(
         cmap="RdYlBu",
         norm=plt.Normalize(
-            vmin=df_precision["defocus"].min(),
-            vmax=df_precision["defocus"].max(),
+            vmin=df_precision["defocus"].min() / 10000,
+            vmax=df_precision["defocus"].max() / 10000,
         ),
     )
     sm._A = []
     cbar = fig.colorbar(sm, ax=ax)
-    cbar.set_label("defocus (Å)", rotation=270, labelpad=20, fontsize=12)
+    cbar.set_label("defocus (\u03bcm)", rotation=270, labelpad=20, fontsize=12)
     # add labels
     ax.set_xlabel("")
     ax.set_ylabel("precision", fontsize=14)
     ax.set_title("Precision for different job types", fontsize=16)
     fig.tight_layout()
     return fig, ax
 
@@ -2279,21 +2279,21 @@
         )
     # remove legend
     ax.legend().remove()
     # add colorbar
     sm = plt.cm.ScalarMappable(
         cmap="RdYlBu",
         norm=plt.Normalize(
-            vmin=df_precision["defocus"].min(),
-            vmax=df_precision["defocus"].max(),
+            vmin=df_precision["defocus"].min() / 10000,
+            vmax=df_precision["defocus"].max() / 10000,
         ),
     )
     sm._A = []
     cbar = fig.colorbar(sm, ax=ax)
-    cbar.set_label("defocus (Å)", rotation=270, labelpad=20, fontsize=12)
+    cbar.set_label("defocus (\u03bcm)", rotation=270, labelpad=20, fontsize=12)
     # add labels
     ax.set_xlabel("")
     ax.set_ylabel("recall", fontsize=14)
     ax.set_title("Recall for different job types", fontsize=16)
     fig.tight_layout()
     return fig, ax
 
@@ -2537,17 +2537,18 @@
     bin_width: int = 100,
     axis: str = "x",
 ):
     if isinstance(metadata_filename, list):
         metadata_filename = metadata_filename[0]
 
     particles_per_ugraph = (
-        df_truth.groupby("ugraph_filename")
-        .size()
-        .reset_index(name="particles_per_ugraph")
+        df_truth.groupby("ugraph_filename").size().reset_index()
+    )
+    particles_per_ugraph.rename(
+        columns={0: "particles_per_ugraph"}, inplace=True
     )
     avg_particles_per_ugraph = particles_per_ugraph[
         "particles_per_ugraph"
     ].mean()
     num_ugraphs = len(particles_per_ugraph)
     if axis != "z":
         particles_per_bin = (
@@ -2665,20 +2666,20 @@
                     )
                     outfilename = os.path.join(
                         self.plot_dir,
                         f"{meta_basename.split('.')[0]}_overlap.png",
                     )
                     self._save_plot(fig, ax, outfilename)
 
-                fig, ax = self.plot_overlap_investigation(
+                fig, ax = plot_overlap_investigation(
                     self.plot_data["plot_overlap"]["df_overlap"],
                     None,
                     self.job_types,
                 )  # plot all
-                outfilename = os.path.join(args.plot_dir, "overlap.png")
+                outfilename = os.path.join(self.plot_dir, "overlap.png")
                 self._save_plot(fig, ax, outfilename)
         else:
             raise TypeError("plot_overlap is not a pd.DataFrame!")
 
     def _save_plot(self, fig, ax, outfilename):
         # save the plot
         fig.savefig(outfilename, dpi=self.dpi, bbox_inches="tight")
```

### Comparing `roodmus-0.0.24/src/roodmus/analysis/utils.py` & `roodmus-0.0.31/src/roodmus/analysis/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 import time
 from collections.abc import KeysView as dict_keys
 from typing import Tuple, Any, List
 
 import yaml
 import numpy as np
 from scipy.spatial import cKDTree
+from scipy.spatial.transform import Rotation as R
 from tqdm import tqdm
 import pandas as pd
+import pickle
 
 from pipeliner.starfile_handler import DataStarFile
 
 
 class IO(object):
     """Class containing several functions to load metadata from .star (RELION)
     and .cs (CryoSPARC) files and the config file generated during the
@@ -54,34 +56,33 @@
             metadata (np.recarray): metadata from .cs file.
         """
         metadata = np.load(cs_path)
         return metadata
 
     @classmethod
     def get_ugraph_cs(self, metadata_cs: np.recarray) -> List[str]:
-        """Grab micrograph file paths from .cs data.
+        """Grab micrograph file paths from .cs data. if micrograph file
+        paths are not present in the metadata, return an empty list.
 
         Args:
             metadata_cs (np.recarray): .cs file metadata.
 
         Returns:
             ugraph_paths (List[str]): micrograph file paths.
         """
-        ugraph_paths = metadata_cs["location/micrograph_path"].tolist()
 
-        # elif "blob/path" in metadata_cs.dtype.names:
-        #     ugraph_paths = metadata_cs["blob/path"]
-        # removed None from within the function to stop mypy errors
-        # else:
-        #     return None
+        if "location/micrograph_path" in metadata_cs.dtype.names:
+            ugraph_paths = metadata_cs["location/micrograph_path"].tolist()
+            ugraph_paths = [
+                os.path.basename(path).decode("utf-8").split("_")[-1]
+                for path in ugraph_paths
+            ]
+        else:
+            ugraph_paths = []
 
-        ugraph_paths = [
-            os.path.basename(path).decode("utf-8").split("_")[-1]
-            for path in ugraph_paths
-        ]
         return ugraph_paths
 
     @classmethod
     def get_uid_cs(self, metadata_cs: np.recarray):
         """Grab uid from .cs metadata.
 
         Args:
@@ -159,21 +160,21 @@
             np.ndarray: Reconstructed particle rotation.
         """
         if "alignments3D/pose" in metadata_cs.dtype.names:
             pose = metadata_cs[
                 "alignments3D/pose"
             ]  # orientations as rodriques vectors
             # convert to euler angles
-            euler = np.array(
-                [geom.rot2euler(geom.expmap(p)) for p in pose],
-                dtype=float,
-            )
-            # euler = R.from_rotvec(pose).as_euler(
-            #     "zyx", degrees=False
-            # )  # convert to euler angles
+            # euler = np.array(
+            #     [geom.rot2euler(geom.expmap(p)) for p in pose],
+            #     dtype=float,
+            # )
+            euler = R.from_rotvec(pose).as_euler(
+                "ZYZ", degrees=False
+            )  # convert to euler angles
             if return_pose:
                 return euler, pose
             else:
                 return euler
         else:
             return None
 
@@ -200,25 +201,28 @@
         Args:
             metadata_cs (np.recarray): CryoSPARC metadata.
 
         Returns:
             np.ndarray: 2D class.
         """
         if "alignments2D/class" in metadata_cs.dtype.names:
-            class2d = metadata_cs["alignments2D/class"]
+            class2d = metadata_cs["alignments2D/class"].astype(int)
         else:
             class2d = None
         return class2d
 
     @classmethod
     def get_latents_cs(self, latent_file: str):
         latents = np.load(latent_file)
-        print(latents.dtype.names)
-        print(f"number of latents: {len(latents)}")
-        return latents
+        ndim = len([r for r in latents.dtype.names if "value" in r])
+        latent = []
+        for i in range(ndim):
+            latent.append(latents[f"components_mode_{i}/value"])
+        latents = np.stack(latent, axis=1)
+        return latents, ndim
 
     # Loading .star files and parsing the ctf parameters,
     # the particle positions and orientations
     @classmethod
     def load_star(self, star_path):
         """Load metadata from .star file.
 
@@ -351,32 +355,43 @@
         euler_psi = metadata_star.column_as_list("particles", "_rlnAnglePsi")
 
         num_particles = np.max(
             [len(euler_phi), len(euler_theta), len(euler_psi)]
         )
         if not euler_phi:  # if empty
             euler_phi = [np.nan] * num_particles
+        else:
+            euler_phi = [np.deg2rad(float(r)) for r in euler_phi]
         if not euler_theta:
             euler_theta = [np.nan] * num_particles
+        else:
+            euler_theta = [np.deg2rad(float(r)) for r in euler_theta]
         if not euler_psi:
             euler_psi = [np.nan] * num_particles
+        else:
+            euler_psi = [np.deg2rad(float(r)) for r in euler_psi]
         euler = np.stack([euler_phi, euler_theta, euler_psi], axis=1)
         return euler
 
     @classmethod
     def get_class2D_star(self, metadata_star):
         """Grab 2D class from Relion metadata.
 
         Args:
             metadata_star (DataStarFile): Loaded Relion metadata.
 
         Returns:
             class2d (np.ndarray): 2D class data.
         """
-        class2d = metadata_star.column_as_list("particles", "_rlnClassNumber")
+        class2d = [
+            int(r)
+            for r in metadata_star.column_as_list(
+                "particles", "_rlnClassNumber"
+            )
+        ]
         if class2d:
             return np.array(class2d)
         else:
             return None
 
     # loading the config file
     @classmethod
@@ -392,15 +407,24 @@
         with open(config_path, "r") as f:
             config = yaml.load(f, Loader=yaml.FullLoader)
         return config
 
     # loading latent space coordinates from cryoDRGN
     @classmethod
     def get_latents_cryodrgn(self, latent_file: str):
-        pass  # TODO
+        with open(latent_file, "rb") as lf:
+            z = pickle.load(lf)
+            # this should be np.ndarray shape [n_particles, n_latent_dims]
+            ndim = z.shape[1]
+            # now get all entries in this row so we can add a column to df
+            latent = []
+            for i in range(ndim):
+                latent.append(z[:, i])
+            latents = np.stack(latent, axis=1)
+            return latents, ndim
 
 
 class geom(object):
     """Adapted from the pyem package by Daniel Asarnow.
     Under the GNU General Public License v3.0
     """
 
@@ -560,15 +584,17 @@
         if self.meta_file is not None:
             self.add_data(
                 verbose=verbose,
                 enable_tqdm=enable_tqdm,
                 ignore_missing_files=ignore_missing_files,
             )
         else:
-            self.load_all_ground_truth()
+            self.load_all_ground_truth(
+                enable_tqdm=enable_tqdm, verbose=verbose
+            )
 
     def add_data(
         self,
         meta_file: str | List[str] = "",
         config_dir: str = "",
         ignore_missing_files: bool = False,
         verbose: bool = False,
@@ -717,15 +743,20 @@
                 print(
                     "Added {} particles from {}".format(
                         total_num_particles, self.config_dir
                     )
                 )
         return
 
-    def load_all_ground_truth(self, return_pose: bool = False):
+    def load_all_ground_truth(
+        self,
+        return_pose: bool = False,
+        enable_tqdm: bool = False,
+        verbose: bool = False,
+    ):
         """Load truth data from all yaml configuration files in the case
         that no reconstruction metadata is provided.
 
         Args:
             return_pose (bool, optional): Whether to return parakeet-encoded
             pose instead of interpreted euler angles. Defaults to False.
 
@@ -740,15 +771,15 @@
         ]
         total_num_particles = 0
         if len(ugraphs_to_load) > 0:
             total_num_particles = 0
             progressbar = tqdm(
                 total=len(ugraphs_to_load),
                 desc="loading micrographs",
-                disable=not self.enable_tqdm,
+                disable=not enable_tqdm,
             )
             for ugraph_path in ugraphs_to_load:
                 if not os.path.isfile(
                     os.path.join(
                         self.config_dir, ugraph_path.replace(".mrc", ".yaml")
                     )
                 ):
@@ -759,15 +790,15 @@
                         self.config_dir, ugraph_path.replace(".mrc", ".yaml")
                     )
                 )
 
                 # adds the values to the truth results,
                 # returns the number of particles added
                 num_particles = self._extract_from_config(
-                    config, self.verbose, return_pose
+                    config, verbose, return_pose
                 )
                 total_num_particles += num_particles
 
                 # add the micrograph path and the metadata file to the
                 # truth results
                 self.results_truth["ugraph_filename"].extend(
                     [ugraph_path] * num_particles
@@ -776,15 +807,15 @@
                 progressbar.update(1)
                 progressbar.set_postfix({"micrograph": ugraph_path})
             progressbar.close()
 
             # update the list of loaded micrographs
             self.ugraph_paths.extend(ugraphs_to_load)
 
-            if self.verbose:
+            if verbose:
                 print(
                     "Loaded ground-truth particle positions from config files"
                 )
                 print(
                     "Dictionaries now contain"
                     " {} particles and {} true particles".format(
                         len(self.results_picking["ugraph_filename"]),
@@ -993,15 +1024,15 @@
                 tmp_results[key] = []
 
             num_particles_loaded = 0
             for m in metadata:
                 ugraph_filename = IO.get_ugraph_cs(m)
                 uid = IO.get_uid_cs(m)
                 tmp_results["uid"].extend(uid)
-                if ugraph_filename is None:
+                if not ugraph_filename:
                     num_particles = len(uid)
                     tmp_results["ugraph_filename"].extend(
                         [np.nan] * num_particles
                     )
                     mask = np.array([False] * num_particles, dtype=bool)
                 else:
                     num_particles = len(
@@ -1378,16 +1409,16 @@
         filenames = []
         for molecules in config["sample"]["molecules"]["local"]:
             f = molecules["filename"]
             for instance in molecules["instances"]:
                 position = instance["position"]
                 orientation = instance["orientation"]  # rotation vector
                 # convert to euler angles
-                euler = geom.rot2euler(geom.expmap(np.array(orientation)))
-                # euler = R.from_rotvec(orientation).as_euler("zyx")
+                # euler = geom.rot2euler(geom.expmap(np.array(orientation)))
+                euler = R.from_rotvec(orientation).as_euler("ZYZ")
                 if return_pose:
                     orientations_list.append(orientation)
                 else:
                     orientations_list.append(euler)
                 positions_list.append(position)
                 filenames.append(f)
         positions: np.ndarray = (
@@ -1473,45 +1504,46 @@
             of truth particles
             image_shape (Tuple[int, int]): Pixel dimensions of image
             projection.
 
         Returns:
             np.ndarray: sparse distance matrix converted to non-sparse array.
         """
-        r = np.sqrt(
+        r = 4 * np.sqrt(
             np.power(float(image_shape[0]), 2)
             + np.power(float(image_shape[1]), 2)
         )
         truth_centres = self._grab_xy_array(pos_truth)
         picked_centres = self._grab_xy_array(pos_picked)
         sdm = (
             cKDTree(picked_centres)
             .sparse_distance_matrix(cKDTree(truth_centres), r)
             .toarray()
         )
-        sdm[sdm < np.finfo(float).eps] = np.nan
+        # sdm[sdm < np.finfo(float).eps] = np.nan
         return sdm
 
     def _match_particles(
         self,
-        metadata_filename: str,
+        metadata_filenames: str | list[str],
         results_picking: pd.DataFrame,
         results_truth: pd.DataFrame,
         verbose: bool = False,
+        enable_tqdm: bool = False,
     ) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame,]:
         """When picked and truth dfs are loaded, this can be used to create
         dataframes of matched picked particles, matched truth particles,
         picked particles not matched to truth particles and finally, truth
         particle not matched to picked particles
 
         Return 4 pd dfs which each correspond to all ugraphs for a given
         metadata file.
         Matching particles is calculated for a given ugraph at a time and
         then the results are concatenated together into a df for the whole
-        metadata file:
+        metadata file.
         Picked particles are matched to nearest truth particle in ugraph.
         If they happen to be within particle diameter, they are matched.
         -If match is found:
             +add matched index of picked particle df to `p_match' list, add
             matched index of truth particle df to `t_match' list
         -Else (no match is found):
             +add unmatched index of picked_particle df to `p_no_match' list
@@ -1545,189 +1577,202 @@
         """
         # to hold list of dfs (1 entry per ugraph) before concat
         matched_picked_dfs = []
         matched_truth_dfs = []
         unmatched_picked_dfs = []
         unmatched_truth_dfs = []
 
-        # grab particles for this metadata file only
-        metafile_picked = results_picking.loc[
-            results_picking["metadata_filename"] == metadata_filename
-        ]
-        metafile_truth = results_truth
-
-        # now find unique ugraphs, loop over whilst computing matches
-        # and unmatched particles
-        ugraph_ids = metafile_picked["ugraph_filename"].unique()
-        progressbar = tqdm(
-            total=len(ugraph_ids),
-            desc="computing closest matches",
-            disable=not verbose,
-        )
-        for ugraph in ugraph_ids:
-            # grab the positions from picked+truth to match
-            ugraph_picked = metafile_picked.loc[
-                metafile_picked["ugraph_filename"] == ugraph
-            ]
-            ugraph_truth = metafile_truth.loc[
-                metafile_truth["ugraph_filename"] == ugraph
+        # loop over the metadata files
+        if isinstance(metadata_filenames, str):
+            metadata_filenames = [metadata_filenames]
+        for metadata_filename in metadata_filenames:
+            # grab particles for this metadata file only
+            metafile_picked = results_picking.loc[
+                results_picking["metadata_filename"] == metadata_filename
             ]
+            metafile_truth = results_truth
 
-            picked_pos_x = ugraph_picked["position_x"]
-            picked_pos_y = ugraph_picked["position_y"]
-            truth_pos_x = ugraph_truth["position_x"]
-            truth_pos_y = ugraph_truth["position_y"]
-
-            # now that we have the particles centres, get the sdm and indices
-            # of the particles which are matched
-            picked_centres = np.array([picked_pos_x, picked_pos_y]).T
-            truth_centres = np.array([truth_pos_x, truth_pos_y]).T
-            sdm = (
-                cKDTree(picked_centres)
-                .sparse_distance_matrix(
-                    cKDTree(truth_centres), self.particle_diameter / 2.0
+            # now find unique ugraphs, loop over whilst computing matches
+            # and unmatched particles
+            ugraph_ids = metafile_picked["ugraph_filename"].unique()
+            progressbar = tqdm(
+                total=len(ugraph_ids),
+                desc="computing closest matches",
+                disable=not enable_tqdm,
+            )
+            for ugraph in ugraph_ids:
+                # grab the positions from picked+truth to match
+                ugraph_picked = metafile_picked.loc[
+                    metafile_picked["ugraph_filename"] == ugraph
+                ]
+                ugraph_truth = metafile_truth.loc[
+                    metafile_truth["ugraph_filename"] == ugraph
+                ]
+
+                picked_pos_x = ugraph_picked["position_x"]
+                picked_pos_y = ugraph_picked["position_y"]
+                truth_pos_x = ugraph_truth["position_x"]
+                truth_pos_y = ugraph_truth["position_y"]
+
+                # now that we have the particles centres, get the sdm and
+                # indices
+                # of the particles which are matched
+                picked_centres = np.array([picked_pos_x, picked_pos_y]).T
+                truth_centres = np.array([truth_pos_x, truth_pos_y]).T
+                sdm = (
+                    cKDTree(picked_centres)
+                    .sparse_distance_matrix(
+                        cKDTree(truth_centres), self.particle_diameter / 2.0
+                    )
+                    .toarray()
                 )
-                .toarray()
-            )
-            sdm[sdm < np.finfo(float).eps] = np.nan
-            if verbose:
-                print("Shape of {}\n\tsdm: {}".format(ugraph, sdm.shape))
+                sdm[sdm < np.finfo(float).eps] = np.nan
+                if verbose:
+                    print("Shape of {}\n\tsdm: {}".format(ugraph, sdm.shape))
 
-            # find the minimum value along axis 0 (1 per picked particle)
-            # and keep track of the index of the truth particle
-            # Using List[Any] to include np.nan which are floats
-            closest_truth_index: List[Any] = []
-            p_match: List[int] = []
-            t_match: List[int] = []
-
-            for j, picked_particle in enumerate(sdm):
-                # make sure there is at least one match to a truth particle
-                if ~np.isnan(picked_particle).all():
-                    truth_particle_index = int(np.nanargmin(picked_particle))
-                else:
-                    print(
-                        "all nan slice in ugraph {} with picked particle"
-                        " index {} with entries: {}".format(
-                            ugraph, j, picked_particle
+                # find the minimum value along axis 0 (1 per picked particle)
+                # and keep track of the index of the truth particle
+                # Using List[Any] to include np.nan which are floats
+                closest_truth_index: List[Any] = []
+                p_match: List[int] = []
+                t_match: List[int] = []
+
+                for j, picked_particle in enumerate(sdm):
+                    # make sure there is at least one match to a truth particle
+                    if ~np.isnan(picked_particle).all():
+                        truth_particle_index = int(
+                            np.nanargmin(picked_particle)
                         )
-                    )
-                    # no particle is matched to picked particle
-                    # and we move on to next particle
-                    continue
-                # check if closest truth particle is within particle diameter
-                # of picked particle
-                if (
-                    picked_particle[truth_particle_index]
-                    > self.particle_diameter
-                ):
-                    closest_truth_index.append(np.nan)
-                    continue
-                # if it is, consider picking successful and allow the picked
-                # and truth particle to be associated with each other
-                else:
-                    closest_truth_index.append(truth_particle_index)
-                    # add the indices of matched particles to respective list
-                    p_match.append(j)
-                    t_match.append(truth_particle_index)
-
-            # check whether any truth particles had multiple picked particles
-            # mapped to them
-            non_unique_count = len(
-                np.unique(
-                    np.array(closest_truth_index, dtype=float)[
-                        ~np.isnan(closest_truth_index)
-                    ]
-                )[
+                    else:
+                        if verbose:
+                            print(
+                                "all nan slice in ugraph {}"
+                                " with picked particle"
+                                " index {} with entries: {}".format(
+                                    ugraph, j, picked_particle
+                                )
+                            )
+                        # no particle is matched to picked particle
+                        # and we move on to next particle
+                        continue
+                    # check if closest truth particle is within particle
+                    # diameter of picked particle
+                    if (
+                        picked_particle[truth_particle_index]
+                        > self.particle_diameter
+                    ):
+                        closest_truth_index.append(np.nan)
+                        continue
+                    # if it is, consider picking successful and allow the
+                    # pickedand truth particle to be associated with each
+                    # other
+                    else:
+                        closest_truth_index.append(truth_particle_index)
+                        # add the indices of matched particles to
+                        # respective list
+                        p_match.append(j)
+                        t_match.append(truth_particle_index)
+
+                # check whether any truth particles had multiple
+                # picked particles mapped to them
+                non_unique_count = len(
                     np.unique(
                         np.array(closest_truth_index, dtype=float)[
                             ~np.isnan(closest_truth_index)
-                        ],
-                        return_counts=True,
-                    )[1]
-                    > 1
-                ]
-            )
-            print(
-                "There are {} non-unique picked"
-                " particles in ugraph {}!".format(
-                    non_unique_count,
-                    ugraph,
-                )
-            )
-            if non_unique_count > 0:
-                print(
-                    "This may cause problems with overwritten assns"
-                    " in truth particles dict!"
-                )
-            # check if there were no matches to truth for a picked particle
-            no_truth_match = len(
-                np.unique(
-                    np.array(closest_truth_index, dtype=float)[
-                        ~np.isnan(closest_truth_index)
+                        ]
+                    )[
+                        np.unique(
+                            np.array(closest_truth_index, dtype=float)[
+                                ~np.isnan(closest_truth_index)
+                            ],
+                            return_counts=True,
+                        )[1]
+                        > 1
                     ]
-                )[
-                    np.unique(
-                        np.array(closest_truth_index, dtype=float)[
-                            ~np.isnan(closest_truth_index)
-                        ],
-                        return_counts=True,
-                    )[1]
-                    == 0
-                ]
-            )
-            if no_truth_match > 0:
-                print(
-                    "There are {} no-truth-match picked particles!".format(
-                        no_truth_match
-                    )
                 )
+                if verbose:
+                    print(
+                        "There are {} non-unique picked"
+                        " particles in ugraph {}!".format(
+                            non_unique_count,
+                            ugraph,
+                        )
+                    )
                 if non_unique_count > 0:
                     print(
                         "This may cause problems with overwritten assns"
                         " in truth particles dict!"
                     )
+                # check if there were no matches to truth for a picked particle
+                no_truth_match = len(
+                    np.unique(
+                        np.array(closest_truth_index, dtype=float)[
+                            ~np.isnan(closest_truth_index)
+                        ]
+                    )[
+                        np.unique(
+                            np.array(closest_truth_index, dtype=float)[
+                                ~np.isnan(closest_truth_index)
+                            ],
+                            return_counts=True,
+                        )[1]
+                        == 0
+                    ]
+                )
+                if no_truth_match > 0 and verbose:
+                    print(
+                        "There are {} no-truth-match picked particles!".format(
+                            no_truth_match
+                        )
+                    )
+                    if non_unique_count > 0 and verbose:
+                        print(
+                            "This may cause problems with overwritten assns"
+                            " in truth particles dict!"
+                        )
 
-            # Next extract the matched particles by df row
-            # for this ugraph. df indices should be propagated.
-            # Use iloc as indices of df that position data was
-            # extracted (to do matching) from is not necessarily ordered
-
-            # Extract matched picked particles
-            matched_picked_dfs.append(ugraph_picked.iloc[p_match])
-
-            # Extract matched truth particles
-            matched_truth_dfs.append(ugraph_truth.iloc[t_match])
-
-            # Extract the unmatched picked particles
-            p_list = np.arange(len(picked_pos_x), dtype=int).tolist()
-            p_unmatched = list(set(p_list).difference(p_match))
-            unmatched_picked_dfs.append(ugraph_picked.iloc[p_unmatched])
-
-            # Extract the unmatched truth particles
-            t_list = np.arange(len(picked_pos_x), dtype=int).tolist()
-            t_unmatched = list(set(t_list).difference(t_match))
-            unmatched_truth_dfs.append(ugraph_truth.iloc[t_unmatched])
+                # Next extract the matched particles by df row
+                # for this ugraph. df indices should be propagated.
+                # Use iloc as indices of df that position data was
+                # extracted (to do matching) from is not necessarily ordered
+
+                # Extract matched picked particles
+                matched_picked_dfs.append(ugraph_picked.iloc[p_match])
+
+                # Extract matched truth particles
+                matched_truth_dfs.append(ugraph_truth.iloc[t_match])
+
+                # Extract the unmatched picked particles
+                p_list = np.arange(len(picked_pos_x), dtype=int).tolist()
+                p_unmatched = list(set(p_list).difference(p_match))
+                unmatched_picked_dfs.append(ugraph_picked.iloc[p_unmatched])
+
+                # Extract the unmatched truth particles
+                t_list = np.arange(len(truth_pos_x), dtype=int).tolist()
+                t_unmatched = list(set(t_list).difference(t_match))
+                unmatched_truth_dfs.append(ugraph_truth.iloc[t_unmatched])
 
-            progressbar.update(1)
-        progressbar.close()
+                progressbar.update(1)
+            progressbar.close()
 
-        # now that we have 4 lists of picked and truth matched/unmatched dfs
-        # need to combine them into a df each and reindex
-        matched_picked_df = pd.concat(matched_picked_dfs, axis=0).reset_index(
-            drop=True
-        )
-        matched_truth_df = pd.concat(matched_truth_dfs, axis=0).reset_index(
-            drop=True
-        )
-        unmatched_picked_df = pd.concat(
-            unmatched_picked_dfs, axis=0
-        ).reset_index(drop=True)
-        unmatched_truth_df = pd.concat(
-            unmatched_truth_dfs, axis=0
-        ).reset_index(drop=True)
+            # now that we have 4 lists of picked and truth
+            # matched/unmatched dfsmatched/unmatched dfs
+            # need to combine them into a df each and reindex
+            matched_picked_df = pd.concat(
+                matched_picked_dfs, axis=0
+            ).reset_index(drop=True)
+            matched_truth_df = pd.concat(
+                matched_truth_dfs, axis=0
+            ).reset_index(drop=True)
+            unmatched_picked_df = pd.concat(
+                unmatched_picked_dfs, axis=0
+            ).reset_index(drop=True)
+            unmatched_truth_df = pd.concat(
+                unmatched_truth_dfs, axis=0
+            ).reset_index(drop=True)
 
         return (
             matched_picked_df,
             matched_truth_df,
             unmatched_picked_df,
             unmatched_truth_df,
         )
@@ -2083,14 +2128,168 @@
                     "neighbours_picked": picked_neighbours[i],
                 }
             )
         progressbar.close()
 
         return pd.DataFrame(data=results_overlap)
 
+    def compute_1to1_match_precision(
+        self,
+        p_match: pd.DataFrame,
+        p_unmatched: pd.DataFrame,
+        t_unmatched: pd.DataFrame,
+        results_truth: pd.DataFrame,
+        verbose: bool = False,
+    ):
+        """This function produces another data frame containing the number
+        of true positives, false positives, false negatives
+        and the precision, recall and multiplicity (0) for each micrograph
+        after implementing a 1 to 1 matching procedure.
+        The output then is a data frame with rows corresponding to each
+        micrograph instead of each particle.
+
+        Args:
+            p_match (pandas.DataFrame): the results of the picking
+            algorithm which have been identified as matching a truth particle
+            p_unmatched (pandas.DataFrame): the results of the picking
+            algorithm which were not matching a single truth particle.
+            t_unmatched (pandas.DataFrame): the results of the truth
+            algorithm.
+            verbose (bool, optional): print out information about the
+            calculation. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: a data frame containing the precision, recall
+            and multiplicity for each micrograph.
+        """
+
+        # define results data frame
+        results_precision: dict[str, Any] = {
+            "metadata_filename": [],
+            "ugraph_filename": [],
+            "defocus": [],
+            "num_particles_picked": [],
+            "num_particles_truth": [],
+            "TP": [],
+            "FP": [],
+            "FN": [],
+            "precision": [],
+            "recall": [],
+            "multiplicity": [],
+        }
+
+        tt = time.time()
+        print(
+            "For each micrograph, for each metadata file, compute the"
+            " precision, recall and multiplicity"
+        )
+        print(
+            "Speed of computation depends on the number of particles in the"
+            " micrograph. progressbar is not accurate"
+        )
+
+        p_match_grouped: pd.core.groupby.generic.DataFrameGroupBy = (
+            p_match.groupby(["metadata_filename", "ugraph_filename"])
+        )
+        p_unmatched_grouped: pd.core.groupby.generic.DataFrameGroupBy = (
+            p_unmatched.groupby(["metadata_filename", "ugraph_filename"])
+        )
+        """
+        t_match_grouped: pd.core.groupby.generic.DataFrameGroupBy = (
+            t_match.groupby("ugraph_filename")
+        )
+        """
+        t_unmatched_grouped: pd.core.groupby.generic.DataFrameGroupBy = (
+            t_unmatched.groupby("ugraph_filename")
+        )
+        df_truth_grouped: pd.core.groupby.generic.DataFrameGroupBy = (
+            results_truth.groupby("ugraph_filename")
+        )
+
+        progressbar = tqdm(
+            total=len(df_truth_grouped.groups.keys()),
+            desc="computing precision",
+            disable=False,  # not verbose,
+        )
+
+        groupnames: dict_keys = p_match_grouped.groups.keys()
+        for groupname in groupnames:
+            # grab the particles in this ugraph
+            p_match_in_ugraph = p_match_grouped.get_group(groupname)
+            TP = len(p_match_in_ugraph)
+
+            if groupname in p_unmatched_grouped.groups.keys():
+                p_unmatched_in_ugraph = p_unmatched_grouped.get_group(
+                    groupname
+                )
+                FP = len(p_unmatched_in_ugraph)
+            else:
+                FP = 0
+
+            """
+            t_match_in_ugraph = t_match_grouped.get_group(
+                groupname[1]
+            )
+            """
+
+            if groupname[1] in t_unmatched_grouped.groups.keys():
+                t_unmatched_in_ugraph = t_unmatched_grouped.get_group(
+                    groupname[1]
+                )
+                FN = len(t_unmatched_in_ugraph)
+            else:
+                FN = 0
+
+            truth_particles_in_ugraph = df_truth_grouped.get_group(
+                groupname[1]
+            )
+
+            # TP = len(p_match_in_ugraph)
+            # FP = len(p_unmatched_in_ugraph)
+            # FN = len(t_unmatched_in_ugraph)
+            precision = float(TP) / (float(TP) + float(FP))
+            # FNs behaving unexpectedly, so using total # truth instead
+            recall = float(TP) / float(len(truth_particles_in_ugraph))
+            multiplicity = 0
+
+            # append the results to the results data frame
+            results_precision["metadata_filename"].append(groupname[0])
+            results_precision["ugraph_filename"].append(groupname[1])
+            results_precision["defocus"].append(
+                truth_particles_in_ugraph["defocus"].values[0]
+            )
+            results_precision["num_particles_picked"].append(TP + FP)
+            results_precision["num_particles_truth"].append(
+                len(truth_particles_in_ugraph)  # len(t_match_in_ugraph) + FN
+            )
+            results_precision["TP"].append(TP)
+            results_precision["FP"].append(FP)
+            results_precision["FN"].append(FN)
+            results_precision["precision"].append(precision)
+            results_precision["recall"].append(recall)
+            results_precision["multiplicity"].append(multiplicity)
+
+            progressbar.update(1)
+            progressbar.set_postfix(
+                {
+                    "precision": precision,
+                    "recall": recall,
+                    "multiplicity": multiplicity,
+                }
+            )
+        progressbar.close()
+
+        if verbose:
+            print(
+                "time taken to compute precision: {}".format(time.time() - tt)
+            )
+
+        # convert the results data frame to a pandas data frame
+        return pd.DataFrame(results_precision)
+
 
 class plotDataFrame(object):
     """Parent class to hold methods for standard saving and loading of data
     to be plotted.
     Input is a dict which holds information for one or more plots.
     This is designed to hold all the information for a given cmd line plotting
     functionality
```

### Comparing `roodmus-0.0.24/src/roodmus/cli.py` & `roodmus-0.0.31/src/roodmus/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,21 +28,26 @@
 
 import os
 import argparse
 import pkg_resources
 from pathlib import Path
 
 import roodmus.simulation.run_parakeet
+import roodmus.simulation.write_starfile
 import roodmus.trajectory.conformations_sampling
 import roodmus.analysis.plot_ctf
 import roodmus.analysis.plot_picking
 import roodmus.analysis.plot_frames
 import roodmus.analysis.plot_classes
 import roodmus.analysis.extract_particles
 import roodmus.analysis.plot_alignment
+import roodmus.heterogeneity.het_metrics
+import roodmus.heterogeneity.latent_clustering
+import roodmus.heterogeneity.het_ensemblecomparison
+import roodmus.heterogeneity.remove_hydrogens
 
 # import analysis.analyse_alignment
 
 
 def get_roodmus_parent() -> Path:
     return Path(__file__).parent.parent.parent
 
@@ -66,36 +71,50 @@
         help="",
     )
     subparsers.required = True
 
     modules = [
         roodmus.trajectory.conformations_sampling,
         roodmus.simulation.run_parakeet,
+        roodmus.simulation.write_starfile,
         roodmus.analysis.plot_ctf,
         roodmus.analysis.plot_picking,
         roodmus.analysis.plot_frames,
         roodmus.analysis.plot_classes,
         roodmus.analysis.plot_alignment,
         roodmus.analysis.extract_particles,
+        roodmus.heterogeneity.het_metrics,
+        roodmus.heterogeneity.latent_clustering,
+        roodmus.heterogeneity.het_ensemblecomparison,
+        roodmus.heterogeneity.remove_hydrogens,
     ]
 
     module_helptext = [
         "Sampling a molecular dynamics trajectory and saving the"
         + " conformations to PDB files.",
         "Simulation of micrograph/tomogram dataset using Parakeet software.",
+        "Write out a particle stack using picked particle coordinates",
         "Plot a comparison between the estimated CTF parameters and the"
         + " true values used in data generation.",
         "Plot statistics from picking analyses and overlays of"
         + " picked and truth particles on micrographs.",
         "Plot the distribution of frames in a job.",
         "Visualise 2D classification results.",
         "Compare estimated 3D alignments from RELION or CryoSPARC to the"
         + " ground-truth orientation values used in Parakeet data generation.",
         "Extract a stack of particles from a set of simulated micrographs"
         + " using the ground-truth positions.",
+        "Sandbox for computing dimension reduction and/or distance metrics"
+        + " and/or clustering on conformations extracted from MD simulations",
+        "Sandbox for computing dimension reduction and/or clustering on"
+        + " latent spaces (encoding heterogeneity)",
+        "Calculation of Jensen-Shannon divergence between ensembles"
+        + " identified through clustering of MD trajectory(ies)"
+        + " and/or clustering of latent spaces representing heterogeneity",
+        "Remove hydrogens from pdb file(s)",
     ]
 
     for helptext, module in zip(module_helptext, modules):
         this_parser = subparsers.add_parser(
             module.get_name(),
             help=helptext,
         )
```

### Comparing `roodmus-0.0.24/src/roodmus/simulation/configuration.py` & `roodmus-0.0.31/src/roodmus/simulation/configuration.py`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/src/roodmus/simulation/orientation_generator.py` & `roodmus-0.0.31/src/roodmus/simulation/orientation_generator.py`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/src/roodmus/simulation/run_parakeet.py` & `roodmus-0.0.31/src/roodmus/simulation/run_parakeet.py`

 * *Files identical despite different names*

### Comparing `roodmus-0.0.24/src/roodmus/trajectory/conformations_sampling.py` & `roodmus-0.0.31/src/roodmus/trajectory/conformations_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,61 +26,68 @@
 from typing import Tuple, List, Any
 import argparse
 
 import numpy as np
 from matplotlib import pyplot as plt
 import mdtraj as mdt
 import glob2 as glob
+from tqdm import tqdm
 
 
 def add_arguments(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     """Set up arguments for parsing
 
     Args:
         parser (argparse.ArgumentParser): Waymarking argument parser
 
     Returns:
         argparse.ArgumentParser:  Waymarking argument parser with arguments
     """
 
     parser.add_argument(
-        "--trajfiles_dir_path",
+        "--trajfiles_dir",
         help=(
             "Path to directory holding (dcd) trajectory files which make up"
             " the whole trajectory."
         ),
         type=str,
         default="",
     )
 
     parser.add_argument(
-        "--topfile_path",
+        "--topfile",
         help="The pdb holding the structure of molecule (no solvent)",
         type=str,
         default="",
     )
 
     parser.add_argument(
         "--verbose",
         help="Increase output verbosity",
         action="store_true",
         default=False,
         required=False,
     )
 
     parser.add_argument(
-        "--sampling_method",
-        help=(
-            "Choose whether to sample a trajectory uniformly in time"
-            " (even_sampling) or by >rmsd threshold (waymark)"
-        ),
-        type=str,
-        default="even_sampling",
+        "--tqdm",
+        help="Turn on progress bar",
+        action="store_true",
     )
 
+    # parser.add_argument(
+    #     "--sampling_method",
+    #     help=(
+    #         "Choose whether to sample a trajectory uniformly in time"
+    #         " (even_sampling) or by >rmsd threshold (waymark)"
+    #     ),
+    #     type=str,
+    #     default="even_sampling",
+    # )
+
     parser.add_argument(
         "--n_conformations",
         help=(
             "Number of conformations to make when sampling evenly"
             " in time from trajectory"
         ),
         type=int,
@@ -142,87 +149,85 @@
         "--investigate_trajectory_files",
         help="Whether to only investigate a trajectory dataset",
         action="store_true",
         default=False,
         required=False,
     )
 
-    parser.add_argument(
-        "--rmsd",
-        help="RMSD in nm to use for waymark sampling",
-        type=float,
-        default=0.3,
-        required=False,
-    )
+    # parser.add_argument(
+    #     "--rmsd",
+    #     help="RMSD in nm to use for waymark sampling",
+    #     type=float,
+    #     default=0.3,
+    #     required=False,
+    # )
 
     parser.add_argument(
         "--digits",
         help=(
             "Number of digits (supplemented with leading zeros)"
             " in output file"
         ),
         type=int,
         default=6,
         required=False,
     )
 
-    parser.add_argument(
-        "--waymarking_plots",
-        help=("Directory to create and put waymarking plots into"),
-        type=str,
-        default="waymarking_plots",
-        required=False,
-    )
+    # parser.add_argument(
+    #     "--waymarking_plots",
+    #     help=("Directory to create and put waymarking plots into"),
+    #     type=str,
+    #     default="waymarking_plots",
+    #     required=False,
+    # )
     return parser
 
 
 def get_name():
     return "conformations_sampling"
 
 
 def get_trajfiles(
-    trajfiles_dir_path: str, verbose: bool, traj_extension: str = ".dcd"
+    trajfiles_dir: str, verbose: bool, traj_extension: str = ".dcd"
 ) -> List[str]:
     """Grab an ordered list of trajectory files
 
     Args:
-        trajfiles_dir_path (str): Directory containing trajectory files
+        trajfiles_dir (str): Directory containing trajectory files
         verbose (bool): Increase output verbosity
         traj_extension (str, optional): File extension of trajectory files.
         Defaults to '.dcd'.
 
     Returns:
         list[str]: Alphanumerically ordered list of full trajectory file paths
     """
-    trajfiles_path = os.path.join(
-        trajfiles_dir_path, "*{}".format(traj_extension)
-    )
+    trajfiles_path = os.path.join(trajfiles_dir, "*{}".format(traj_extension))
     if verbose:
         print("Traj files path to glob: {}".format(trajfiles_path))
     trajfiles = sorted(glob.glob(trajfiles_path))
     if verbose:
         for i, trajfile in enumerate(trajfiles):
             print("Trj file path {}: {}".format(i, trajfile))
     return trajfiles
 
 
-def get_topfile(topfile_path: str, verbose: bool) -> str:
+def get_topfile(topfile: str, verbose: bool) -> str:
     """Grab the path to the topology file with option
      to output path
 
     Args:
-        topfile_path (str): Path to topology file
+        topfile (str): Path to topology file
         verbose (bool): Increase output verbosity
 
     Returns:
         str: Topology file path
     """
     if verbose:
-        print("Top file path: {}".format(topfile_path))
-    return topfile_path
+        print("Top file path: {}".format(topfile))
+    return topfile
 
 
 def load_traj(trajfile: str, topfile: str, verbose: bool) -> mdt.Trajectory:
     """Load a single trajectory file into memory using
      mdtraj library
 
     Args:
@@ -235,14 +240,26 @@
     """
     t = mdt.load(trajfile, top=topfile)
     if verbose:
         print("mdt.load returns type: {}".format(type(t)))
     return t
 
 
+"""
+Waymarking is currently disabled. The function does not work
+when only a single trajectory file is used.
+The waymarking is also done incorrectly, with
+new conformations only being checked against the
+fist conformation, instead of all conformations
+in the ensemble
+
+We should redo waymarking entirely in the future
+"""
+
+
 def waymark(
     trajfiles: List[str],
     topfile: str,
     rmsd: float,
     verbose: bool,
     atom_indices=None,
 ) -> Tuple[
@@ -533,25 +550,29 @@
 def sample_dcd_evenly(
     trajfiles: List[str],
     topfile: str,
     traj_indices: List[List[int]],
     verbose: bool,
     output_dir: str,
     digits: int = 6,
+    enable_progressbar: bool = False,
 ):
     """Reads a traj file (single dcd) and then selects which conformation(s)
     to save from sample_index list. Saves as pdb with indexes ranging over
     multiple dcd files (ie: a whole trajectory)
 
     Args:
         trajfiles (list[str]): List of filepaths for dcd files
         topfile (str): PDB for MD simulation
         traj_indices (list[list[int]]): List containing list of indices of
         conformation(s) in each dcd which need to be saved to file as pdb_
         verbose (bool): Increase output verbosity
+        output_dir (str): Directory to save the sampled conformations to
+        digits (int, optional): Number of digits to use in saved filenames
+        enable_progressbar (bool, optional): Whether to show progress bar
     """
     create_output_dir(output_dir, verbose=verbose)
 
     conformation_counter = 0
     for traj_idx, traj_conf_idxs in enumerate(traj_indices):
         # check if need any conformations from this dcd before loading it
         if len(traj_conf_idxs) > 0:
@@ -571,35 +592,44 @@
             selected_conformations = traj[traj_conf_idxs]
             if verbose:
                 print(
                     "number of selected conformations: {}".format(
                         len(selected_conformations)
                     )
                 )
-
+            progressbar = tqdm(
+                total=len(selected_conformations),
+                disable=not enable_progressbar,
+            )
             # save the conformations selected from this trajectory file to disk
             for i_conf, conf in enumerate(selected_conformations):
                 conf_file = os.path.join(
                     output_dir,
                     "conformation_{}.pdb".format(
                         str(conformation_counter).zfill(digits)
                     ),
                 )
                 conf.save(conf_file)
                 conformation_counter += 1
-                if verbose:
+                if verbose and not enable_progressbar:
                     print(
                         "Saved conformation_{}.pdb from traj file"
                         " {} ({}) to location {}".format(
                             str(conformation_counter).zfill(digits),
                             traj_idx,
                             trajfile,
                             conf_file,
                         )
                     )
+                progressbar.update(1)
+                progressbar.set_description(
+                    f"conformation_ \
+                        {str(conformation_counter).zfill(digits)}.pdb"
+                )
+            progressbar.close()
 
         else:
             # skip this traj file
             continue
 
     return
 
@@ -699,20 +729,20 @@
             )
 
     return traj_indices
 
 
 def main(args):
     trajfiles = get_trajfiles(
-        args.trajfiles_dir_path, args.verbose, args.traj_extension
+        args.trajfiles_dir, args.verbose, args.traj_extension
     )
     if args.limit_n_traj_subfiles:
         trajfiles = trajfiles[: args.limit_n_traj_subfiles]
 
-    topfile = get_topfile(args.topfile_path, args.verbose)
+    topfile = get_topfile(args.topfile, args.verbose)
 
     traj_steps, steps_per_file = get_traj_steps(
         trajfiles, topfile, args.verbose
     )
     if args.verbose:
         if len(np.unique(steps_per_file)) != 1:
             print(
@@ -726,14 +756,19 @@
     if args.investigate_trajectory_files:
         print(
             "Finished investigation of trajectory files. Cmd line arg"
             " --investigate_trajectory_files gives no output files"
         )
         return
 
+    # only available sampling method at this time is even sampling.
+    # waymarking has been disabled for now, as it is not correctly
+    # implemented
+    args.sampling_method = "even_sampling"
+
     if args.sampling_method == "even_sampling":
         # create function to get indices of N conformations to sample from
         # entire trajectory
         # output is list[list[int]]
         traj_indices = get_traj_indices(
             traj_steps,
             steps_per_file,
@@ -742,18 +777,25 @@
             rnd_start=args.rnd_start,
             seed=args.random_startpoint_seed,
             contiguous=args.use_contiguous_conformations,
         )
 
         # create functio to take list[list[int]] and save the pdbs to file
         sample_dcd_evenly(
-            trajfiles, topfile, traj_indices, args.verbose, args.output_dir
+            trajfiles,
+            topfile,
+            traj_indices,
+            args.verbose,
+            args.output_dir,
+            args.digits,
+            args.tqdm,
         )
 
-    if args.sampling_method == "waymark":
+        """
+    elif args.sampling_method == "waymark":
         # we want to get: Tuple[list[int], list[np.int64],
         # np.ndarray[np.int64,np.int64]]
         # First is waymarks (frame_ind_list -> the trajectory frames which
         # constitute a new conformation)
         # Second is counts (the number of frames assigned to each conformation
         # Third is )
         (
@@ -803,14 +845,24 @@
 
         # We now have a mdt.Trajectory which holds all the
         # non-redundant conformations.
         # Let's write them out
         write_non_redundant_confs(
             non_redundant_confs, args.output_dir, args.digits
         )
+        """
+
+    else:
+        # method of sampling not recognised
+        print(
+            "Sampling method {} not recognised. Exiting.".format(
+                args.sampling_method
+            )
+        )
+
     return
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description=__doc__)
     add_arguments(parser)
     args = parser.parse_args()
```

### Comparing `roodmus-0.0.24/src/roodmus.egg-info/PKG-INFO` & `roodmus-0.0.31/src/roodmus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roodmus
-Version: 0.0.24
+Version: 0.0.31
 Summary: Synthetic SP micrograph creation and analysis
 Author-email: Joel Greer <joel.greer@stfc.ac.uk>, Maarten Joosten <m.j.joosten@tudelft.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -721,21 +721,22 @@
 Requires-Dist: fake-useragent==1.1.1
 Requires-Dist: fastjsonschema==2.17.1
 Requires-Dist: filelock==3.9.0
 Requires-Dist: fonttools==4.38.0
 Requires-Dist: fqdn==1.5.1
 Requires-Dist: fsspec==2023.1.0
 Requires-Dist: gemmi==0.5.4
+Requires-Dist: gemmi-program==0.6.5
 Requires-Dist: glob2==0.7
 Requires-Dist: guanaco==0.3.0
 Requires-Dist: h5py==3.8.0
 Requires-Dist: HeapDict==1.0.1
 Requires-Dist: identify==2.5.19
 Requires-Dist: idna==3.4
-Requires-Dist: imageio==2.25.0
+Requires-Dist: imageio==2.27.0
 Requires-Dist: importlib-metadata==6.0.0
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: ipykernel==6.24.0
 Requires-Dist: ipython==8.14.0
 Requires-Dist: isoduration==20.11.0
 Requires-Dist: jedi==0.18.2
 Requires-Dist: Jinja2==3.1.2
@@ -750,31 +751,34 @@
 Requires-Dist: jupyter-lsp==2.2.0
 Requires-Dist: jupyter-server==2.7.0
 Requires-Dist: jupyter-server-terminals==0.4.4
 Requires-Dist: jupyterlab==4.0.3
 Requires-Dist: jupyterlab-pygments==0.2.2
 Requires-Dist: jupyterlab-server==2.23.0
 Requires-Dist: kiwisolver==1.4.4
+Requires-Dist: llvmlite==0.41.1
 Requires-Dist: locket==1.0.0
 Requires-Dist: lxml==4.9.2
 Requires-Dist: maptools==0.3.5
 Requires-Dist: MarkupSafe==2.1.2
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: matplotlib-inline==0.1.6
-Requires-Dist: mdtraj==1.9.7
+Requires-Dist: MDAnalysis==2.6.1
+Requires-Dist: mdtraj==1.9.9
 Requires-Dist: mistune==3.0.1
 Requires-Dist: mrcfile==1.4.2
 Requires-Dist: msgpack==1.0.4
 Requires-Dist: nbclient==0.8.0
 Requires-Dist: nbconvert==7.6.0
 Requires-Dist: nbformat==5.9.1
 Requires-Dist: nest-asyncio==1.5.6
 Requires-Dist: networkx==3.0
 Requires-Dist: nodeenv==1.7.0
 Requires-Dist: notebook-shim==0.2.3
+Requires-Dist: numba==0.58.1
 Requires-Dist: numpy==1.23.0
 Requires-Dist: overrides==7.3.1
 Requires-Dist: packaging==23.0
 Requires-Dist: pandas==1.5.3
 Requires-Dist: pandas-stubs==1.5.3.230304
 Requires-Dist: pandocfilters==1.5.0
 Requires-Dist: parse==1.19.0
@@ -792,14 +796,15 @@
 Requires-Dist: psutil==5.9.4
 Requires-Dist: ptyprocess==0.7.0
 Requires-Dist: pure-eval==0.2.2
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==1.10.4
 Requires-Dist: pyee==8.2.2
 Requires-Dist: pygments==2.15.1
+Requires-Dist: pynndescent==0.5.10
 Requires-Dist: pyparsing==3.0.9
 Requires-Dist: pypdb==2.2
 Requires-Dist: pyppeteer==1.0.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-json-logger==2.0.7
@@ -810,38 +815,40 @@
 Requires-Dist: pyzmq==25.1.0
 Requires-Dist: referencing==0.29.1
 Requires-Dist: requests==2.28.2
 Requires-Dist: requests-html==0.10.0
 Requires-Dist: rfc3339-validator==0.1.4
 Requires-Dist: rfc3986-validator==0.1.1
 Requires-Dist: rpds-py==0.8.10
-Requires-Dist: scikit-image==0.19.3
-Requires-Dist: scikit-learn==1.2.1
+Requires-Dist: scikit-image==0.22.0
+Requires-Dist: scikit-learn==1.3.2
 Requires-Dist: scipy==1.9.3
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: send2trash==1.8.2
 Requires-Dist: six==1.16.0
 Requires-Dist: sniffio==1.3.0
 Requires-Dist: sortedcontainers==2.4.0
 Requires-Dist: soupsieve==2.3.2.post1
 Requires-Dist: stack-data==0.6.2
 Requires-Dist: starfile==0.4.11
+Requires-Dist: tbb==2021.10.0
 Requires-Dist: tblib==1.7.0
 Requires-Dist: terminado==0.17.1
 Requires-Dist: threadpoolctl==3.1.0
 Requires-Dist: tifffile==2023.2.3
 Requires-Dist: tinycss2==1.2.1
 Requires-Dist: tomli==2.0.1
 Requires-Dist: toolz==0.12.0
 Requires-Dist: tornado==6.2
 Requires-Dist: tqdm==4.64.0
 Requires-Dist: traitlets==5.9.0
 Requires-Dist: types-pytz==2022.7.1.2
 Requires-Dist: types-tabulate==0.9.0.1
 Requires-Dist: typing_extensions==4.4.0
+Requires-Dist: umap-learn==0.5.4
 Requires-Dist: uri-template==1.3.0
 Requires-Dist: urllib3==1.26.14
 Requires-Dist: virtualenv==20.20.0
 Requires-Dist: w3lib==2.1.1
 Requires-Dist: wcwidth==0.2.6
 Requires-Dist: webcolors==1.13
 Requires-Dist: webencodings==0.5.1
@@ -860,34 +867,33 @@
 
 WIP analysis tools:
 - analysis of latent spaces of heterogeneous reconstruction methods (CryoDRGN, cryoSPARC 3DFlex)
 - comparing the MD trajectory to a latent space
 
 
 ## How to use Roodmus
-The aim of roodmus is to turn an MD trajectory into a set of micrographs that can serve as ground-truth for testing cryo-EM (heterogeneous) reconstruction methods. The core of the micrograph simulation is done using parakeet. The program consists of three modules: 
+The aim of roodmus is to turn an MD trajectory into a set of micrographs that can serve as ground-truth for testing cryo-EM (heterogeneous) reconstruction methods. The core of the micrograph simulation is done using Parakeet. The program consists of three modules: 
 
 ### 1. Sample pdb/mmcif models from trajectory dataset
 Given a directory of trajectory files (in for example .nc or .dcd format) and a topology file (for example a .pdb file), this module saves a selection of frames from the trajectory as .pdb files. The general command used to run this module is:
 ```
 roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR
 ```
 Where N is the number of conformations to be samples from the trajectory. In case N is larger than the number of frames in the trajectory, N will be set equal to the number of frames.
 
-Sampling can be done either evenly or by waymarking. In case of even sampling, frames of the trajectory will be sampled at even intervals. In case of waymarking, a random starting point is selected and new frames are sampled if their rmsd with respect to the sampled frames is larger than a given threshold. The general command used to run conformation sampling in waymarking mode is:
+Sampling can be done in a configurable manner - frames of the trajectory can be sampled at even time intervals from the trajectory or from contiguous frames, from a given starting frame. The general command used to run conformation sampling in waymarking mode is:
 ```
-roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR --rmsd Threshold --sampling_method waymark
+roodmus conformations_sampling --trajfiles_dir_path PATH/TO/DCD/FILES --topfile_path PATH/TO/TOPOLOGY.pdb --n_conformations N --output_dir_path PATH/TO/OUTPUT/DIR 
 ```
-Where Threshold is the rmsd threshold for sampling a new frame and SEED is the seed for the random starting point. The default value for Threshold is 0.3. More options are availble, see the help page for more information.
 
-Sampled conformations are saved as individual .pdb files in the output directory.
+Sampled conformations are saved as individual .pdb files in the output directory. More options are available as listed by `roodmus conformations_sampling --help`.
 
 
 ### 2. Generate SPA dataset using Parakeet python API:
-Given a directory containing (any) .pdb files, a desired number of images to simulate and a number of molecules per image, this module generates a configuration file to run parakeet and then executes the parakeet simulation. Each micrograph subsamples the .pdb files to the number of molecules to generate, if not enough .pdb files are available, multiple instances of the same file are used. The config file is saved as a .yaml file with the same name as the image it corresponds to. The general command for this module is:
+Given a directory containing (any) .pdb files, a desired number of images to simulate and a number of molecules per image, this module generates a configuration file to run parakeet and then executes the parakeet simulation. Each micrograph subsamples the .pdb files to the number of molecules to generate, if not enough .pdb files are available, multiple instances of files are used. The config file is saved as a .yaml file with the same name as the image it corresponds to. The general command for this module is:
 ```
 roodmus run_parakeet --pdb_dir PATH/TO/PDB/FILES --mrc_dir PATH/TO/OUTPUT/DIR -n N -m M --device "gpu or cpu" 
 ```
 Where N is the number of images to generate and M is the number of molecules per image. There are many more options available for configuring the parakeet simulation. Most have been set to reasonable defaults, but can be changed if desired. See the help page for more information. A list of the most important configuration options:
 - --acceleration_voltage: acceleration voltage in kV. Default: 300
 - --electrons_per_angstrom: total exposure in electrons per Angstrom. Default: 45
 - --dqe: detector quantum efficiency. Uses Parakeet's detector quantum efficiency model. Boolean
@@ -907,32 +913,32 @@
 ```
 Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. The 'scatter' plot type plots the estimated defocus values vs. true defocus for each particle. The 'ctf' plot type plots the CTF in the style of CTFFind4 for the first N micrographs, for both estimated and true defocus parameters.
 
 The second functionality is comparing picked particle positions and true particle positions. This can be done using the following command:
 ```
 roodmus plot_picking --config_dir PATH/TO/CONFIG/FILES --mrc_dir PATH/TO/MRC/FILES --metadata_file PATH/TO/METADATA/FILE.{star, cs} --job_types "particle picking" "2D classification" "..." --plot_dir PATH/TO/PLOT/DIR -N N --plot_types {label_truth, label_picked, label_truth_and_picked, precision, boundary, overlap} --particle_diamter D
 ```
-Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. Multiple metadata files can be loaded in at the same time. Each metadata file can be given a label using the job_types option. metadata files with the same label are grouped together. The labels are used as titles and axis labels in plots. D is the particle diamter in angstroms.
+Where N is the number of micrographs to load and --mrc_dir is the directory containing .mrc micrograph files. Multiple metadata files can be loaded in at the same time. Each metadata file can be given a label using the job_types option. Metadata files with the same label are grouped together. The labels are used as titles and axis labels in plots. D is the diameter (in angstroms) used for matching picked and truth particles.
 The 'label_truth' plot type plots the true particle positions on the micrograph for each metadata_file supplied. The 'label_picked' plot type plots the picked particle positions on the micrograph. The 'label_truth_and_picked' plot type plots both the true and picked particle positions on the micrograph. The 'precision' plot type plots the particle picking precision and recall for each job_type. Precision is defined as the number of picked particles closer than particle_diameter/2 to any true particle divided by the total number of picked particles. Recall is defined as the number of true particles with at least one picked particle closer than particle_diameter/2 divided by the total number of true particles.
 The 'boundary' plot type plots the distribution of particles in the micrographs in x-, y- and z-direction. The 'overlap' plot type plots the number of picked particles closer than r to any true particle for a range of r values.
 
 Other functionality includes comparing estimated particle orientations to true particle orientations and plotting precision for 2D classes. See the help page for more information:
 ```
 roodmus --help
 ```
 or
 ```
 roodmus {plot_picking, plot_ctf, plot_alignment, plot_2d_lasses, plot_frames} --help
 ```
 
 # Licensing
-Need to figure out what kind of license we want and when/how we need to get it for the repo. May have to use the same licence as parakeet.
+Roodmus is GPLv3 licensed. Please see the `LICENSE` file for information on usage, reproduction or adaptation of the Roodmus codebase.
 
 # Parakeet Compatibility
-Code is currently tested with parakeet commit `024b86ebf55adf737c1b1116b8adbb59ee7db491`. Functionality is expected to be easily extended to the most recent version as of 9/3/23. This may required a small number of Parakeet config variables to be added/modified in the configuration class.
+Code is currently tested with parakeet tag [v0.4.3.dev1](https://github.com/rosalindfranklininstitute/parakeet/releases/tag/v0.4.3.dev1). Functionality is expected to be easily extended to the most recent version as of 9/3/23. This may required a small number of Parakeet config variables to be added/modified in the configuration class.
 
 # flow chart of current structure of Roodmus
 ![flowchart](docs/flowchart.png)
 
 # Setting up Roodmus
 ## On a PC
 From creating a new python environment (assumed conda/anaconda installed) to being able to develop and run roodmus. They assume that FFTW is in the system path (used for python-multem/guanaco). The number used for CMAKE_CUDA_ARCHITECTURES number will depend on you GPU. <https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/> can be a useful reference to find it for your GPU.
@@ -969,28 +975,7 @@
 pip install -e .
 cd../
 
 cd ccpem-pipeliner
 pip install -e .
 ```
 After doing so, an editable install of roodmus should be set up with all requisite packages.
-
-# Updating roodmus As A pip Package
-I do this via twine:
-`python3 -m pip install --upgrade twine`
-
-If there's any updates, you need to update the version number (configured in the pyproject.toml). Make sure it is suitable according to pep conventions! Currently updating this is manual.
-
-Build the updated package via:
-
-`python3 -m pip install --upgrade build`
-
-`python3 -m build`
-
-Once you've done that, you can publish the package via:
-`python3 -m twine upload --repository testpypi dist/*<version>*`
-
-To do this you'll need an account and token (instructions here: <https://packaging.python.org/en/latest/tutorials/packaging-projects/>)
-
-If you want to download the pip package from the remote repository (currently the pypi test repo) and install it, you can do this via:
-`python3 -m pip install --extra-index-url https://test.pypi.org/simple/  roodmus --no-cache-dir`
-You can also pip install it via the tar'ed dist package or the pip wheel (.whl file) found in the dist directory.
```

### Comparing `roodmus-0.0.24/src/roodmus.egg-info/requires.txt` & `roodmus-0.0.31/src/roodmus.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 fake-useragent==1.1.1
 fastjsonschema==2.17.1
 filelock==3.9.0
 fonttools==4.38.0
 fqdn==1.5.1
 fsspec==2023.1.0
 gemmi==0.5.4
+gemmi-program==0.6.5
 glob2==0.7
 guanaco==0.3.0
 h5py==3.8.0
 HeapDict==1.0.1
 identify==2.5.19
 idna==3.4
-imageio==2.25.0
+imageio==2.27.0
 importlib-metadata==6.0.0
 iniconfig==2.0.0
 ipykernel==6.24.0
 ipython==8.14.0
 isoduration==20.11.0
 jedi==0.18.2
 Jinja2==3.1.2
@@ -62,31 +63,34 @@
 jupyter-lsp==2.2.0
 jupyter-server==2.7.0
 jupyter-server-terminals==0.4.4
 jupyterlab==4.0.3
 jupyterlab-pygments==0.2.2
 jupyterlab-server==2.23.0
 kiwisolver==1.4.4
+llvmlite==0.41.1
 locket==1.0.0
 lxml==4.9.2
 maptools==0.3.5
 MarkupSafe==2.1.2
 matplotlib==3.5.2
 matplotlib-inline==0.1.6
-mdtraj==1.9.7
+MDAnalysis==2.6.1
+mdtraj==1.9.9
 mistune==3.0.1
 mrcfile==1.4.2
 msgpack==1.0.4
 nbclient==0.8.0
 nbconvert==7.6.0
 nbformat==5.9.1
 nest-asyncio==1.5.6
 networkx==3.0
 nodeenv==1.7.0
 notebook-shim==0.2.3
+numba==0.58.1
 numpy==1.23.0
 overrides==7.3.1
 packaging==23.0
 pandas==1.5.3
 pandas-stubs==1.5.3.230304
 pandocfilters==1.5.0
 parse==1.19.0
@@ -104,14 +108,15 @@
 psutil==5.9.4
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pycparser==2.21
 pydantic==1.10.4
 pyee==8.2.2
 pygments==2.15.1
+pynndescent==0.5.10
 pyparsing==3.0.9
 pypdb==2.2
 pyppeteer==1.0.2
 pyquery==2.0.0
 pytest==7.4.0
 python-dateutil==2.8.2
 python-json-logger==2.0.7
@@ -122,38 +127,40 @@
 pyzmq==25.1.0
 referencing==0.29.1
 requests==2.28.2
 requests-html==0.10.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rpds-py==0.8.10
-scikit-image==0.19.3
-scikit-learn==1.2.1
+scikit-image==0.22.0
+scikit-learn==1.3.2
 scipy==1.9.3
 seaborn==0.12.2
 send2trash==1.8.2
 six==1.16.0
 sniffio==1.3.0
 sortedcontainers==2.4.0
 soupsieve==2.3.2.post1
 stack-data==0.6.2
 starfile==0.4.11
+tbb==2021.10.0
 tblib==1.7.0
 terminado==0.17.1
 threadpoolctl==3.1.0
 tifffile==2023.2.3
 tinycss2==1.2.1
 tomli==2.0.1
 toolz==0.12.0
 tornado==6.2
 tqdm==4.64.0
 traitlets==5.9.0
 types-pytz==2022.7.1.2
 types-tabulate==0.9.0.1
 typing_extensions==4.4.0
+umap-learn==0.5.4
 uri-template==1.3.0
 urllib3==1.26.14
 virtualenv==20.20.0
 w3lib==2.1.1
 wcwidth==0.2.6
 webcolors==1.13
 webencodings==0.5.1
```

