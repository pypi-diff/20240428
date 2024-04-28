# Comparing `tmp/spleenseg-1.2.2.tar.gz` & `tmp/spleenseg-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleenseg-1.2.2.tar", last modified: Fri Apr 26 16:03:02 2024, max compression
+gzip compressed data, was "spleenseg-1.2.4.tar", last modified: Sun Apr 28 15:13:17 2024, max compression
```

## Comparing `spleenseg-1.2.2.tar` & `spleenseg-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxr-x   0 rudolph  (2090878)  2000513        0 2024-04-26 16:03:25.340870 spleenseg-1.2.2/
--rw-rw-r--   0 rudolph  (2090878)  2000513     1069 2024-04-23 22:06:23.000000 spleenseg-1.2.2/LICENSE
--rw-rw-r--   0 rudolph  (2090878)  2000513     7389 2024-04-26 16:03:25.337878 spleenseg-1.2.2/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878)  2000513     6841 2024-04-26 16:03:22.000000 spleenseg-1.2.2/README.rst
--rw-rw-r--   0 rudolph  (2090878)  2000513      223 2024-04-23 22:06:23.000000 spleenseg-1.2.2/requirements.txt
--rw-rw-r--   0 rudolph  (2090878)  2000513       38 2024-04-26 16:03:25.342832 spleenseg-1.2.2/setup.cfg
--rw-rw-r--   0 rudolph  (2090878)  2000513     1848 2024-04-23 22:06:23.000000 spleenseg-1.2.2/setup.py
-drwxrwxr-x   0 rudolph  (2090878)  2000513        0 2024-04-26 16:03:25.199661 spleenseg-1.2.2/spleenseg/
-drwxrwxr-x   0 rudolph  (2090878)  2000513        0 2024-04-26 16:03:25.296724 spleenseg-1.2.2/spleenseg/core/
--rw-rw-r--   0 rudolph  (2090878)  2000513    24201 2024-04-26 15:47:29.000000 spleenseg-1.2.2/spleenseg/core/neuralnet.py
-drwxrwxr-x   0 rudolph  (2090878)  2000513        0 2024-04-26 16:03:25.309748 spleenseg-1.2.2/spleenseg/plotting/
--rw-rw-r--   0 rudolph  (2090878)  2000513     2113 2024-04-25 22:48:33.000000 spleenseg-1.2.2/spleenseg/plotting/plotting.py
--rw-rw-r--   0 rudolph  (2090878)  2000513     9173 2024-04-26 15:47:38.000000 spleenseg-1.2.2/spleenseg/spleenseg.py
-drwxrwxr-x   0 rudolph  (2090878)  2000513        0 2024-04-26 16:03:25.323730 spleenseg-1.2.2/spleenseg/transforms/
--rw-rw-r--   0 rudolph  (2090878)  2000513     7650 2024-04-25 16:11:14.000000 spleenseg-1.2.2/spleenseg/transforms/transforms.py
-drwxrwxr-x   0 rudolph  (2090878)  2000513        0 2024-04-26 16:03:25.275875 spleenseg-1.2.2/spleenseg.egg-info/
--rw-rw-r--   0 rudolph  (2090878)  2000513     7389 2024-04-26 16:03:24.000000 spleenseg-1.2.2/spleenseg.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878)  2000513      361 2024-04-26 16:03:25.000000 spleenseg-1.2.2/spleenseg.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878)  2000513        1 2024-04-26 16:03:24.000000 spleenseg-1.2.2/spleenseg.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878)  2000513       55 2024-04-26 16:03:24.000000 spleenseg-1.2.2/spleenseg.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878)  2000513      247 2024-04-26 16:03:24.000000 spleenseg-1.2.2/spleenseg.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878)  2000513       65 2024-04-26 16:03:24.000000 spleenseg-1.2.2/spleenseg.egg-info/top_level.txt
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.917607 spleenseg-1.2.4/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-17 00:36:10.000000 spleenseg-1.2.4/LICENSE
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     8016 2024-04-28 15:13:17.917607 spleenseg-1.2.4/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6405 2024-04-26 18:36:17.000000 spleenseg-1.2.4/README.md
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6841 2024-04-28 15:13:16.000000 spleenseg-1.2.4/README.rst
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      238 2024-04-26 18:25:29.000000 spleenseg-1.2.4/requirements.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-04-28 15:13:17.917607 spleenseg-1.2.4/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1876 2024-04-26 18:34:46.000000 spleenseg-1.2.4/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/core/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    24201 2024-04-26 18:36:17.000000 spleenseg-1.2.4/spleenseg/core/neuralnet.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/models/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3221 2024-04-26 18:36:17.000000 spleenseg-1.2.4/spleenseg/models/data.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/plotting/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2113 2024-04-26 18:36:17.000000 spleenseg-1.2.4/spleenseg/plotting/plotting.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9173 2024-04-26 18:39:18.000000 spleenseg-1.2.4/spleenseg/spleenseg.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/transforms/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7650 2024-04-24 22:01:17.000000 spleenseg-1.2.4/spleenseg/transforms/transforms.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg.egg-info/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     8016 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      418 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       55 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      251 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       82 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/top_level.txt
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/tests/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      662 2024-04-17 00:36:10.000000 spleenseg-1.2.4/tests/test_example.py
```

### Comparing `spleenseg-1.2.2/LICENSE` & `spleenseg-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.2/PKG-INFO` & `spleenseg-1.2.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: spleenseg
-Version: 1.2.2
-Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
-Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
-Author: FNNDSC
-Author-email: dev@babyMRI.org
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Provides-Extra: none
-Provides-Extra: dev
-License-File: LICENSE
-
 Spleen 3D image segmentation (MONAI)
 ====================================
 
 |Version| |MIT License| |ci|
 
 ``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__ *DS*
 plugin based off Project MONAI’s spleen segmentation exemplar. This
@@ -154,15 +138,15 @@
 
 Mount the source code ``spleenseg_train.py`` into a container to try out
 changes without rebuild.
 
 .. code:: shell
 
    docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.11/site-packages/spleenseg_train.py:ro \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
        -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
        localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 
 Testing
 ~~~~~~~
 
 Run unit tests using ``pytest``. It’s recommended to rebuild the image
```

### Comparing `spleenseg-1.2.2/README.rst` & `spleenseg-1.2.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: spleenseg
+Version: 1.2.4
+Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
+Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
+Author: FNNDSC
+Author-email: dev@babyMRI.org
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+License-File: LICENSE
+Requires-Dist: chris_plugin==0.4.0
+Requires-Dist: pudb
+Requires-Dist: pyfiglet
+Requires-Dist: matplotlib
+Requires-Dist: monai-weekly
+Requires-Dist: gdown
+Requires-Dist: nibabel
+Requires-Dist: tqdm
+Requires-Dist: ignite
+Requires-Dist: scikit-build
+Requires-Dist: torch
+Requires-Dist: pytorch-ignite
+Requires-Dist: scikit-image
+Requires-Dist: scipy
+Requires-Dist: pillow
+Requires-Dist: tensorboard
+Requires-Dist: torchvision
+Requires-Dist: psutil
+Requires-Dist: pandas
+Requires-Dist: einops
+Requires-Dist: transformers
+Requires-Dist: mlflow
+Requires-Dist: pynrrd
+Requires-Dist: clearml
+Provides-Extra: none
+Provides-Extra: dev
+Requires-Dist: pytest~=7.1; extra == "dev"
+
 Spleen 3D image segmentation (MONAI)
 ====================================
 
 |Version| |MIT License| |ci|
 
 ``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__ *DS*
 plugin based off Project MONAI’s spleen segmentation exemplar. This
@@ -138,15 +179,15 @@
 
 Mount the source code ``spleenseg_train.py`` into a container to try out
 changes without rebuild.
 
 .. code:: shell
 
    docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.11/site-packages/spleenseg_train.py:ro \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
        -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
        localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 
 Testing
 ~~~~~~~
 
 Run unit tests using ``pytest``. It’s recommended to rebuild the image
```

### Comparing `spleenseg-1.2.2/setup.py` & `spleenseg-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     long_description=readme(),
     author="FNNDSC",
     author_email="dev@babyMRI.org",
     url="https://github.com/FNNDSC/pl-monai_spleenseg",
     packages=[
         "spleenseg",
         "spleenseg/core",
+        "spleenseg/models",
         "spleenseg/plotting",
         "spleenseg/transforms",
     ],
     install_requires=requirements,
     data_files=[("", ["requirements.txt"])],
     license="MIT",
     entry_points={"console_scripts": ["spleenseg = spleenseg.spleenseg:main"]},
```

### Comparing `spleenseg-1.2.2/spleenseg/core/neuralnet.py` & `spleenseg-1.2.4/spleenseg/core/neuralnet.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.2/spleenseg/plotting/plotting.py` & `spleenseg-1.2.4/spleenseg/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.2/spleenseg/spleenseg.py` & `spleenseg-1.2.4/spleenseg/spleenseg.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 warnings.filterwarnings(
     "ignore",
     message="For details about installing the optional dependencies, please visit:",
 )
 
 from chris_plugin import chris_plugin, PathMapper
 
-__version__ = "1.2.2"
+__version__ = "1.2.4"
 
 DISPLAY_TITLE = r"""
 
 ███████╗██████╗ ██╗     ███████╗███████╗███╗   ██╗███████╗███████╗ ██████╗
 ██╔════╝██╔══██╗██║     ██╔════╝██╔════╝████╗  ██║██╔════╝██╔════╝██╔════╝
 ███████╗██████╔╝██║     █████╗  █████╗  ██╔██╗ ██║███████╗█████╗  ██║  ███╗
 ╚════██║██╔═══╝ ██║     ██╔══╝  ██╔══╝  ██║╚██╗██║╚════██║██╔══╝  ██║   ██║
```

### Comparing `spleenseg-1.2.2/spleenseg/transforms/transforms.py` & `spleenseg-1.2.4/spleenseg/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.2/spleenseg.egg-info/PKG-INFO` & `spleenseg-1.2.4/spleenseg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 Metadata-Version: 2.1
 Name: spleenseg
-Version: 1.2.2
+Version: 1.2.4
 Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
 Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+License-File: LICENSE
+Requires-Dist: chris_plugin==0.4.0
+Requires-Dist: pudb
+Requires-Dist: pyfiglet
+Requires-Dist: matplotlib
+Requires-Dist: monai-weekly
+Requires-Dist: gdown
+Requires-Dist: nibabel
+Requires-Dist: tqdm
+Requires-Dist: ignite
+Requires-Dist: scikit-build
+Requires-Dist: torch
+Requires-Dist: pytorch-ignite
+Requires-Dist: scikit-image
+Requires-Dist: scipy
+Requires-Dist: pillow
+Requires-Dist: tensorboard
+Requires-Dist: torchvision
+Requires-Dist: psutil
+Requires-Dist: pandas
+Requires-Dist: einops
+Requires-Dist: transformers
+Requires-Dist: mlflow
+Requires-Dist: pynrrd
+Requires-Dist: clearml
 Provides-Extra: none
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: pytest~=7.1; extra == "dev"
 
 Spleen 3D image segmentation (MONAI)
 ====================================
 
 |Version| |MIT License| |ci|
 
 ``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__ *DS*
@@ -154,15 +179,15 @@
 
 Mount the source code ``spleenseg_train.py`` into a container to try out
 changes without rebuild.
 
 .. code:: shell
 
    docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.11/site-packages/spleenseg_train.py:ro \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
        -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
        localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 
 Testing
 ~~~~~~~
 
 Run unit tests using ``pytest``. It’s recommended to rebuild the image
```

