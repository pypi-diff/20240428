# Comparing `tmp/atooms-pp-3.4.0.tar.gz` & `tmp/atooms_pp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms-pp-3.4.0.tar", last modified: Thu Jan 25 20:47:52 2024, max compression
+gzip compressed data, was "atooms_pp-4.0.0.tar", last modified: Sun Apr 28 20:43:57 2024, max compression
```

## Comparing `atooms-pp-3.4.0.tar` & `atooms_pp-4.0.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-01-25 20:47:52.192658 atooms-pp-3.4.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.4.0/LICENSE
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2024-01-25 20:47:52.192658 atooms-pp-3.4.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.4.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-01-25 20:47:52.184658 atooms-pp-3.4.0/atooms/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.4.0/atooms/__init__.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-01-25 20:47:52.192658 atooms-pp-3.4.0/atooms/postprocessing/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      723 2023-11-19 20:43:02.000000 atooms-pp-3.4.0/atooms/postprocessing/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       56 2024-01-24 18:41:13.000000 atooms-pp-3.4.0/atooms/postprocessing/_commit.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2024-01-25 20:47:50.000000 atooms-pp-3.4.0/atooms/postprocessing/_version.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1557 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/alpha2.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15568 2023-08-03 17:17:23.000000 atooms-pp-3.4.0/atooms/postprocessing/api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5991 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/ba.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4548 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/chi4t.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1972 2023-11-22 19:44:54.000000 atooms-pp-3.4.0/atooms/postprocessing/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    26256 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/correlation.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.4.0/atooms/postprocessing/filter.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    16989 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/fkt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2870 2023-08-04 08:46:53.000000 atooms-pp-3.4.0/atooms/postprocessing/fourierspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15722 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/fourierspace.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13982 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/gr.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     7653 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2942 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/ik.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.4.0/atooms/postprocessing/linkedcells.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3766 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/msd.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4676 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/partial.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.4.0/atooms/postprocessing/progress.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3074 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/qt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.4.0/atooms/postprocessing/realspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4221 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/s4kt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1753 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/sacf.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10106 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/sk.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.4.0/atooms/postprocessing/susceptibility.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1274 2024-01-25 20:33:47.000000 atooms-pp-3.4.0/atooms/postprocessing/vacf.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-01-25 20:47:52.192658 atooms-pp-3.4.0/atooms_pp.egg-info/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2024-01-25 20:47:52.000000 atooms-pp-3.4.0/atooms_pp.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2024-01-25 20:47:52.000000 atooms-pp-3.4.0/atooms_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-01-25 20:47:52.000000 atooms-pp-3.4.0/atooms_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2024-01-25 20:47:52.000000 atooms-pp-3.4.0/atooms_pp.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2024-01-25 20:47:52.000000 atooms-pp-3.4.0/atooms_pp.egg-info/top_level.txt
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-01-25 20:47:52.192658 atooms-pp-3.4.0/bin/
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.4.0/bin/acf.py
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.4.0/bin/pp.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2024-01-25 20:47:52.192658 atooms-pp-3.4.0/setup.cfg
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.4.0/setup.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms_pp-4.0.0/LICENSE
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     4787 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms_pp-4.0.0/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.434511 atooms_pp-4.0.0/atooms/
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/atooms/postprocessing/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      723 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2024-04-28 20:43:51.000000 atooms_pp-4.0.0/atooms/postprocessing/_version.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1682 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/alpha2.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15122 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5992 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/ba.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4627 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/chi4t.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3414 2024-04-28 17:13:10.000000 atooms_pp-4.0.0/atooms/postprocessing/cli.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2015 2024-04-28 17:52:29.000000 atooms_pp-4.0.0/atooms/postprocessing/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    28841 2024-04-28 20:25:29.000000 atooms_pp-4.0.0/atooms/postprocessing/correlation.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/filter.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    17389 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/fkt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15598 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/fourierspace.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13982 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/gr.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     7653 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2941 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/ik.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10529 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/linkedcells.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3767 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/msd.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4910 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/partial.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2024-04-14 06:46:04.000000 atooms_pp-4.0.0/atooms/postprocessing/progress.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3112 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/qt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4220 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/s4kt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1715 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/sacf.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10066 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/sk.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1689 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/susceptibility.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1282 2024-04-28 20:01:50.000000 atooms_pp-4.0.0/atooms/postprocessing/vacf.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/atooms_pp.egg-info/
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     4787 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1081 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       35 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        7 2024-04-28 20:43:57.000000 atooms_pp-4.0.0/atooms_pp.egg-info/top_level.txt
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/bin/
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms_pp-4.0.0/bin/pp.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1166 2024-04-28 20:43:51.000000 atooms_pp-4.0.0/pyproject.toml
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/setup.cfg
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-28 20:43:57.438511 atooms_pp-4.0.0/tests/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1031 2024-04-13 21:37:27.000000 atooms_pp-4.0.0/tests/test_api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      747 2024-04-13 21:37:27.000000 atooms_pp-4.0.0/tests/test_helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1263 2024-04-13 21:37:27.000000 atooms_pp-4.0.0/tests/test_ll.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    30919 2024-04-28 20:27:21.000000 atooms_pp-4.0.0/tests/test_pp.py
```

### Comparing `atooms-pp-3.4.0/LICENSE` & `atooms_pp-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.4.0/PKG-INFO` & `atooms_pp-4.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.4.0
+Version: 4.0.0
 Summary: Post-processing tools for particle simulations
-Home-page: https://framagit.org/atooms/postprocessing
-Author: Daniele Coslovich
-Author-email: daniele.coslovich@umontpellier.fr
+Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
-Platform: UNKNOWN
+Project-URL: repository, https://framagit.org/atooms/postprocessing
+Project-URL: homepage, https://framagit.org/atooms/postprocessing
+Project-URL: documentation, https://atooms.frama.io/postprocessing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: atooms>=2
+Requires-Dist: numpy
+Requires-Dist: argh
+Requires-Dist: tqdm
+Requires-Dist: f2py_jit
 
 # Postprocessing
 
 [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
@@ -109,9 +111,7 @@
 ## Contributing
 
 Contributions to the project are welcome. If you wish to contribute, check out [these guidelines](https://framagit.org/atooms/atooms/-/blob/master/CONTRIBUTING.md).
 
 ## Authors
 
 Daniele Coslovich: https://www.units.it/daniele.coslovich/
-
-
```

### Comparing `atooms-pp-3.4.0/README.md` & `atooms_pp-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/__init__.py` & `atooms_pp-4.0.0/atooms/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/alpha2.py` & `atooms_pp-4.0.0/atooms/postprocessing/alpha2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Non-Gaussian parameter."""
 
+import logging
 import numpy
 
 from .helpers import linear_grid
 from .correlation import Correlation, gcf_offset
 from .helpers import setup_t_grid, ifabsmm
 
 __all__ = ['NonGaussianParameter']
 
+_log = logging.getLogger(__name__)
+
 
 class NonGaussianParameter(Correlation):
 
     """Non-Gaussian parameter."""
 
     symbol = 'alpha2'
     short_name = 'alpha_2(t)'
     long_name = 'non-Gaussian parameter'
-    phasespace = ['pos-unf']
+    variables = ['pos-unf']
 
     def __init__(self, trajectory, tgrid=None, nsamples=30, **kwargs):
         Correlation.__init__(self, trajectory, tgrid, **kwargs)
         if self.grid is None:
             self.grid = linear_grid(0.0, self.trajectory.total_time * 0.75, nsamples)
         self._discrete_tgrid = setup_t_grid(self.trajectory, self.grid, offset=norigins != '1')
 
@@ -38,10 +41,10 @@
 
         self.grid, self.value = gcf_offset(alpha_2, self._discrete_tgrid, self.skip,
                                            self.trajectory.steps, self._pos_unf)
         self.grid = [ti * self.trajectory.timestep for ti in self.grid]
 
     def analyze(self):
         try:
-            self.analysis['t_star'], self.analysis['a2_star'] = ifabsmm(self.grid, self.value)[1]
+            self._analysis['time at peak, t_star'], self._analysis['value at peak, a2_star'] = ifabsmm(self.grid, self.value)[1]
         except ZeroDivisionError:
-            pass
+            _log.warn('could not compute t_star or a2_star')
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/api.py` & `atooms_pp-4.0.0/atooms/postprocessing/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """Post processing API."""
 
+# TODO: use more decorators, do not loop over trajectories inside
+# TODO: each api function should return a dict of results and artifacts
+# The decorator can be used by pp.py, ignoring the results
+
 import atooms.postprocessing as pp
 from atooms.postprocessing.progress import progress
 from atooms.postprocessing.partial import Partial
 from atooms.trajectory import Trajectory
 from atooms.trajectory.decorators import change_species, center
 from atooms.system.particle import distinct_species
 
@@ -78,21 +82,21 @@
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         th._grandcanonical = grandcanonical
         cf = backend(th, dr=dr, rmax=rmax,
                      norigins=global_args['norigins'],
                      ndim=ndim)
         if global_args['filter'] is not None:
             cf = pp.Filter(cf, global_args['filter'])
-        cf.do(update=global_args['update'])
+        cf.do()
 
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             cf = Partial(backend, ids, th,
                          dr=dr, rmax=rmax, norigins=global_args['norigins'], ndim=ndim)
-            cf.do(update=global_args['update'])
+            cf.do()
 
 def sk(input_file, nk=20, dk=0.1, kmin=-1.0, kmax=15.0, ksamples=30,
        kgrid=None, weight=None, weight_trajectory=None,
        weight_fluctuations=False, *input_files, **global_args):
     """
     Structure factor
     """
@@ -112,39 +116,39 @@
         if global_args['filter'] is not None:
             cf = pp.Filter(cf, global_args['filter'])
         if weight_trajectory is not None:
             weight_trajectory = TrajectoryXYZ(weight_trajectory)
         cf.add_weight(trajectory=weight_trajectory,
                       field=weight,
                       fluctuations=weight_fluctuations)
-        cf.do(update=global_args['update'])
+        cf.do()
 
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             cf = Partial(backend, ids, th, kgrid=fourier_grid,
                          norigins=global_args['norigins'])
             cf.add_weight(trajectory=weight_trajectory,
                           field=weight,
                           fluctuations=weight_fluctuations)
-            cf.do(update=global_args['update'])
+            cf.do()
 
 def ik(input_file, trajectory_radius=None, nk=20, dk=0.1, kmin=-1.0,
        kmax=15.0, kgrid=None, ksamples=30, *input_files,
        **global_args):
     """Spectral density"""
     global_args = _compat(global_args)
     if kgrid is not None:
         kgrid = [float(_) for _ in kgrid.split(',')]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         if trajectory_radius is None:
             trajectory_radius = input_file
             pp.SpectralDensity(th, trajectory_radius,
                                kgrid=kgrid, norigins=global_args['norigins'],
                                kmin=kmin, kmax=kmax, nk=nk, dk=dk,
-                               ksamples=ksamples).do(update=global_args['update'])
+                               ksamples=ksamples).do()
 
 def msd(input_file, tmax=-1.0, tmax_fraction=0.75, tsamples=30,
         sigma=1.0, func='linear', rmsd_max=-1.0, fix_cm=False,
         no_offset=False, *input_files, **global_args):
     """Mean square displacement"""
     func = _func_db[func]
     global_args = _compat(global_args)
@@ -156,37 +160,37 @@
             t_grid = [0.0] + func(dt, tmax_fraction*th.total_time, tsamples)
         else:
             t_grid = None
         ids = distinct_species(th[0].particle)
         pp.MeanSquareDisplacement(th, tgrid=t_grid,
                                   norigins=global_args['norigins'],
                                   sigma=sigma, rmax=rmsd_max, no_offset=no_offset,
-                                  fix_cm=fix_cm).do(update=global_args['update'])
+                                  fix_cm=fix_cm).do()
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(pp.MeanSquareDisplacement, ids, th, tgrid=t_grid,
                     norigins=global_args['norigins'], sigma=sigma,
-                    rmax=rmsd_max, no_offset=no_offset).do(update=global_args['update'])
+                    rmax=rmsd_max, no_offset=no_offset).do()
 
 def vacf(input_file, tmax=-1.0, tmax_fraction=0.10,
          tsamples=30, func='linear', *input_files, **global_args):
     """Velocity autocorrelation function"""
     global_args = _compat(global_args)
     func = _func_db[func]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         if tmax > 0:
             t_grid = [0.0] + func(th.timestep, min(th.total_time, tmax), tsamples)
         elif tmax_fraction > 0:
             t_grid = [0.0] + func(th.timestep, tmax_fraction*th.total_time, tsamples)
         else:
             t_grid = None
-        pp.VelocityAutocorrelation(th, t_grid, norigins=global_args['norigins']).do(update=global_args['update'])
+        pp.VelocityAutocorrelation(th, t_grid, norigins=global_args['norigins']).do()
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(pp.VelocityAutocorrelation, ids, th,
-                    t_grid, norigins=global_args['norigins']).do(update=global_args['update'])
+                    t_grid, norigins=global_args['norigins']).do()
 
 def fkt(input_file, tmax=-1.0, tmax_fraction=0.75,
         tsamples=60, kmin=7.0, kmax=7.0, ksamples=1, dk=0.1, nk=100,
         kgrid=None, func='logx', fix_cm=False, total=False, *input_files,
         **global_args):
     """Total intermediate scattering function"""
     global_args = _compat(global_args)
@@ -206,19 +210,19 @@
             k_grid = [float(_) for _ in kgrid.split(',')]
         else:
             k_grid = linear_grid(kmin, kmax, ksamples)
         ids = distinct_species(th[0].particle)
         if total or len(ids) == 1:
             pp.IntermediateScattering(th, k_grid, t_grid,
                                       norigins=global_args['norigins'],
-                                      nk=nk, dk=dk, fix_cm=fix_cm).do(update=global_args['update'])
+                                      nk=nk, dk=dk, fix_cm=fix_cm).do()
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(pp.IntermediateScattering, ids, th, k_grid, t_grid,
                     norigins=global_args['norigins'],
-                    nk=nk, dk=dk, fix_cm=fix_cm).do(update=global_args['update'])
+                    nk=nk, dk=dk, fix_cm=fix_cm).do()
 
 def fskt(input_file, tmax=-1.0, tmax_fraction=0.75, tsamples=60,
          kmin=7.0, kmax=8.0, ksamples=1, dk=0.1, nk=8, kgrid=None,
          func='logx', total=False, fix_cm=False, lookup_mb=64.0,
          *input_files, **global_args):
     """Self intermediate scattering function"""
     global_args = _compat(global_args)
@@ -238,19 +242,19 @@
             k_grid = [float(_) for _ in kgrid.split(',')]
         else:
             k_grid = linear_grid(kmin, kmax, ksamples)
         ids = distinct_species(th[0].particle)
         if total or len(ids) == 1:
             backend(th, k_grid, t_grid, nk, dk=dk,
                     norigins=global_args['norigins'], fix_cm=fix_cm,
-                    lookup_mb=lookup_mb).do(update=global_args['update'])
+                    lookup_mb=lookup_mb).do()
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(backend, ids, th, k_grid, t_grid, nk, dk=dk,
                     norigins=global_args['norigins'], fix_cm=fix_cm,
-                    lookup_mb=lookup_mb).do(update=global_args['update'])
+                    lookup_mb=lookup_mb).do()
 
 def chi4qs(input_file, tsamples=60, a=0.3, tmax=-1.0, func='logx',
            tmax_fraction=0.75, total=False, *input_files,
            **global_args):
     """Dynamic susceptibility of self overlap"""
     global_args = _compat(global_args)
     func = _func_db[func]
@@ -263,82 +267,82 @@
         if tmax > 0:
             t_grid = [0.0] + func(th.timestep, min(th.total_time, tmax), tsamples)
         elif tmax_fraction > 0:
             t_grid = [0.0] + func(th.timestep, tmax_fraction*th.total_time, tsamples)
         else:
             t_grid = None
         if total:
-            backend(th, t_grid, a=a, norigins=global_args['norigins']).do(update=global_args['update'])
+            backend(th, t_grid, a=a, norigins=global_args['norigins']).do()
         ids = distinct_species(th[0].particle)
         if not total and len(ids) > 1:
             Partial(backend, ids, th, t_grid, a=a,
-                    norigins=global_args['norigins']).do(update=global_args['update'])
+                    norigins=global_args['norigins']).do()
 
 def alpha2(input_file, tmax=-1.0, tmax_fraction=0.75,
            tsamples=60, func='logx', *input_files, **global_args):
     """Non-Gaussian parameter"""
     global_args = _compat(global_args)
     func = _func_db[func]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         if tmax > 0:
             t_grid = [0.0] + func(th.timestep, tmax, tsamples)
         elif tmax_fraction > 0:
             t_grid = [0.0] + func(th.timestep, tmax_fraction*th.total_time, tsamples)
         else:
             t_grid = None
-        pp.NonGaussianParameter(th, t_grid, norigins=global_args['norigins']).do(update=global_args['update'])
+        pp.NonGaussianParameter(th, t_grid, norigins=global_args['norigins']).do()
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(pp.NonGaussianParameter, ids, th, t_grid,
-                    norigins=global_args['norigins']).do(update=global_args['update'])
+                    norigins=global_args['norigins']).do()
 
 def qst(input_file, tmax=-1.0, tmax_fraction=0.75,
         tsamples=60, func='logx', *input_files, **global_args):
     """Self overlap correlation function"""
     global_args = _compat(global_args)
     func = _func_db[func]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         if tmax > 0:
             t_grid = [0.0] + func(th.timestep, tmax, tsamples)
         elif tmax_fraction > 0:
             t_grid = [0.0] + func(th.timestep, tmax_fraction*th.total_time, tsamples)
         else:
             t_grid = None
-        pp.SelfOverlap(th, t_grid, norigins=global_args['norigins']).do(update=global_args['update'])
+        pp.SelfOverlap(th, t_grid, norigins=global_args['norigins']).do()
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(pp.SelfOverlap, ids, th, t_grid,
-                    norigins=global_args['norigins']).do(update=global_args['update'])
+                    norigins=global_args['norigins']).do()
 
 def qt(input_file, tmax=-1.0, tmax_fraction=0.75,
         tsamples=60, func='logx', *input_files, **global_args):
     """Collective overlap correlation function"""
     global_args = _compat(global_args)
     func = _func_db[func]
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         if tmax > 0:
             t_grid = [0.0] + func(th.timestep, tmax, tsamples)
         elif tmax_fraction > 0:
             t_grid = [0.0] + func(th.timestep, tmax_fraction*th.total_time, tsamples)
         else:
             t_grid = None
-        pp.CollectiveOverlap(th, t_grid, norigins=global_args['norigins']).do(update=global_args['update'])
+        pp.CollectiveOverlap(th, t_grid, norigins=global_args['norigins']).do()
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             Partial(pp.CollectiveOverlap, ids, th, t_grid,
-                    norigins=global_args['norigins']).do(update=global_args['update'])
+                    norigins=global_args['norigins']).do()
 
 def ba(input_file, dtheta=4.0, grandcanonical=False, *input_files, **global_args):
     """Bond-angle distribution"""
     global_args = _compat(global_args)
     for th in _get_trajectories([input_file] + list(input_files), global_args):
         th._grandcanonical = grandcanonical
 
         cf = pp.BondAngleDistribution(th, dtheta=dtheta, norigins=global_args['norigins'])
         if global_args['filter'] is not None:
             cf = pp.Filter(cf, global_args['filter'])
-        cf.do(update=global_args['update'])
+        cf.do()
 
         ids = distinct_species(th[0].particle)
         if len(ids) > 1 and not global_args['no_partial']:
             cf = Partial(pp.BondAngleDistribution, ids, th, dtheta=dtheta, norigins=global_args['norigins'])
-            cf.do(update=global_args['update'])
+            cf.do()
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/ba.py` & `atooms_pp-4.0.0/atooms/postprocessing/ba.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Bond angle distribution."""
 
 import sys
 import math
 import logging
 
@@ -25,15 +25,15 @@
     from atooms.system.particle import distinct_species
     from atooms.postprocessing.partial import Partial
     from atooms.postprocessing import RadialDistributionFunction
     from .helpers import ifabsmm
 
     ids = distinct_species(th[0].particle)
     gr = Partial(RadialDistributionFunction, ids, th, dr=0.1)
-    gr.do(update=False)
+    gr.do()
     rcut = {}
     for isp in ids:
         for jsp in ids:
             # First find absolute maximum
             _, m = ifabsmm(list(gr.partial[(isp, jsp)].grid),
                            list(gr.partial[(isp, jsp)].value))
             # Then look for first minimum after the maximum
@@ -50,28 +50,28 @@
     """
     Bond angle distribution function.
     """
 
     nbodies = 2
     symbol = 'ba'
     short_name = 'D(theta)'
-    long_name = 'bond angle distribution'
-    phasespace = ['pos', 'ids']
+    long_name = 'bond-angle distribution'
+    variables = ['pos', 'ids']
     _symmetric = False
 
     def __init__(self, trajectory, dtheta=4.0, rcut=None, **kwargs):
         Correlation.__init__(self, trajectory, None, **kwargs)
         self.grid = linear_grid(0.0, 180.0, dtheta)  # reassign grid anyway
         self.rcut = rcut
 
     def _compute(self):
         from atooms.trajectory.decorators import change_species
-        from atooms.postprocessing.realspace_wrap import compute
-        from atooms.system.particle import distinct_species
-
+        from atooms.system.particle import distinct_species        
+        from atooms.postprocessing.core import f90
+       
         hist_all = []
         hist_one = numpy.ndarray(len(self.grid), dtype=numpy.int32)
         origins = range(0, len(self.trajectory), self.skip)
         dtheta = self.grid[1] - self.grid[0]
 
         # Setup array of cutoff distances based on g(r) calculated for
         # the whole trajectory.
@@ -84,29 +84,29 @@
             for species_pair in rcut:
                 self.rcut[ids.index(species_pair[0]), ids.index(species_pair[1])] = rcut[species_pair]
         else:
             self.rcut = numpy.array(self.rcut)
 
         for isp in range(len(ids)):
             for jsp in range(len(ids)):
-                self.analysis['cutoff distance {}-{}'.format(isp, jsp)] = self.rcut[isp, jsp]
+                self._analysis[f'cutoff distance, rc_{isp}-{jsp}'] = self.rcut[isp, jsp]
 
         for frame in progress(origins):
             system = self.trajectory[frame]
             ndims = system.number_of_dimensions
             pos_0 = self._pos_0[frame]
             ids_0 = self._ids_0[frame]
 
             # With a non-periodic cell, which just bounds the physical
             # domain, we crop particles away from the surface (within rmax)
             if system.cell is not None and hasattr(system.cell, 'periodic') and \
                sum(system.cell.periodic) == 0:
                 # Booleans do not work here, so we just use integers,
                 # which are 1 is particles are on the surface and 0 otherwise
-                mask = compute.on_surface_c(pos_0, system.cell.side, numpy.max(self.rcut))
+                mask = f90.realspace.on_surface_c(pos_0, system.cell.side, numpy.max(self.rcut))
                 pos_0 = pos_0[mask == 0, :]
                 ids_0 = ids_0[mask == 0]
 
             # Store side (copied over from gr)
             # TODO: refactor
             # If there is no cell and anyway along non-periodic directions,
             # we replace sides with infty to work with f90 kernels (which apply PBC)
@@ -125,20 +125,20 @@
             
             # system = change_species(system, 'F')  # species are in fortran style
             # ids = numpy.array(system.dump('spe'), dtype=numpy.int32)
             nn = numpy.array(0, dtype=numpy.int32)
             neighbors = numpy.ndarray(50, dtype=numpy.int32)
             for idx in range(len(pos_0)):
                 isp = ids_0[idx]
-                compute.neighbors('C', side, pos_0[idx],
+                f90.realspace.neighbors('C', side, pos_0[idx],
                                   self._pos_1[frame].transpose(),
                                   self._ids_1[frame],
                                   self.rcut[isp, :],
                                   nn, neighbors)
-                compute.bond_angle(pos_0[idx, :],
+                f90.realspace.bond_angle(pos_0[idx, :],
                                    self._pos_1[frame].transpose(),
                                    neighbors[0: nn], side, dtheta,
                                    hist_one)
                 hist_all.append(hist_one.copy())
 
         # Normalization
         hist = numpy.sum(hist_all, axis=0)
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/chi4t.py` & `atooms_pp-4.0.0/atooms/postprocessing/chi4t.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Four-point dynamic susceptibility."""
 
 import logging
 import numpy
 
 from .helpers import logx_grid
@@ -28,15 +28,15 @@
     - a: distance parameter entering the Heaviside function in the
     overlap calculation
     """
 
     symbol = 'chi4qs'
     short_name = 'chi_4(t)'
     long_name = 'dynamic susceptibility of self overlap'
-    phasespace = 'pos-unf'
+    variables = 'pos-unf'
 
     def __init__(self, trajectory, tgrid=None, norigins=-1, a=0.3,
                  tsamples=60, **kwargs):
         Correlation.__init__(self, trajectory, tgrid, norigins=norigins, **kwargs)
         if tgrid is None:
             self.grid = logx_grid(0.0, self.trajectory.total_time * 0.75, tsamples)
         self._discrete_tgrid = setup_t_grid(self.trajectory, self.grid, offset=norigins != '1')
@@ -72,44 +72,45 @@
                 A_av, A2_av = 0, 0
             self.grid.append(dt * self.trajectory.timestep)
             self.value.append((A2_av - A_av**2) / self._pos_unf[0].shape[0])
             self.average.value.append(A_av)
             self.variance.value.append(A2_av)
         self.average.grid, self.variance.grid = self.grid, self.grid
 
-    def write(self):
+    def write(self, output_path=None):
         # We subclass this to also write down qsu and qsu2
         super(Chi4SelfOverlap, self).write()
         self.average.write()
         self.variance.write()
 
     def analyze(self):
         try:
-            self.analysis['peak time tau_star'], self.analysis['peak height chi4_star'] = ifabsmm(self.grid, self.value)[1]
+            time, height = ifabsmm(self.grid, self.value)[1]
         except ZeroDivisionError:
+            time, height = float('nan'), float('nan')
             _log.warning('could not find maximum')
-
+        self._analysis['peak time, tau^*'], self._analysis['peak height, chi_4^*'] = time, height
 
 class Chi4SelfOverlapOptimized(Chi4SelfOverlap):
     """
     Four-point dynamic susceptibility from the time-dependent self
     overlap function.
 
     Optimized version using fortran 90 extension.
     """
 
     def _compute(self):
         try:
-            from atooms.postprocessing.realspace_wrap import realspace_module
+            from atooms.postprocessing.core import f90
         except ImportError:
             _log.error('f90 wrapper missing or not functioning')
             raise
 
         def f(x, y):
-            return realspace_module.self_overlap(x, y, numpy.array(self.a_square))
+            return f90.realspace.self_overlap(x, y, numpy.array(self.a_square))
 
         self.grid = []
         self.average.tag, self.variance.tag = self.tag, self.tag
         for off, i in progress(self._discrete_tgrid):
             A, A2, cnt = 0.0, 0.0, 0
             for i0 in range(off, len(self._pos_unf)-i-self.skip, self.skip):
                 w = f(self._pos_unf[i0], self._pos_unf[i0+i])
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/core.py` & `atooms_pp-4.0.0/atooms/postprocessing/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,11 @@
 import os
 import argparse
 
-from ._version import __version__ as __bare_version
-
-# Version
-try:
-    from ._commit import __commit__, __date__
-    __version__ = '%s+%s (%s)' % (__bare_version, __commit__, __date__)
-except ImportError:
-    __commit__ = ""
-    __date__ = ""
-    __version__ = __bare_version
+from ._version import __version__
 
 # Global variables
 pp_output_path = '{trajectory}.pp.{symbol}.{tag}'
 pp_trajectory_format = None
 
 # Help formatter
 os.environ['COLUMNS'] = "100"
@@ -50,7 +41,17 @@
                 textrows[idx] = " "
             elif search:
                 lwspace = search.end()
                 lines = [self.__add_whitespace(i, lwspace, x) for i, x in enumerate(_textwrap.wrap(line, width))]
                 textrows[idx] = lines
 
         return [item for sublist in textrows for item in sublist]
+
+# F90 modules
+import os
+from f2py_jit import jit
+
+# TODO: make a dummy test to disable f90 extensions if compiler is missing
+_pwd = os.path.dirname(__file__)
+_f90_paths = [os.path.join(_pwd, 'fourierspace.f90'),
+              os.path.join(_pwd, 'realspace.f90')]
+f90 = jit(_f90_paths)
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/correlation.py` & `atooms_pp-4.0.0/atooms/postprocessing/correlation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Base correlation function."""
 
+# TODO: pp should provide a results dict that packs grid and values e.g. like
+#  {'F_s(k,t)': [fskt.grid, fskt.value]}
+#  {'MSD(t)': [msd.grid, msd.value]}
+#
+# For partials I would do
+#  {'F_s^{1-1}(k,t)': [fskt.partial[('1', '1')].grid, fskt.partial[('1', '1')].value]}
+#  {'MSD_1(t)': [msd.partial['1'].grid, fskt.partial['1'].value]}
+#
+# It would be similar for analysis
+#  {'tau_s(k)': [fskt.grid[0], fskt.analysis.tau]}
+#  {'D': msd.diffusion_coefficient}
+#
+# It should be possible to just update these dicts without overriding existing keys.
+# So results could be a property of Correlation, which returns at runtime.
+# One exception could be "artifacts". We want to collect all artifacts there
+# when updating the dicts. So we need a custom update that allows some entries to be merged
+# for instance by summing their values.
+
 import os
 import logging
 from collections import defaultdict
 import numpy
 
 from atooms.trajectory import Trajectory
 from atooms.trajectory.decorators import Unfolded, fold
@@ -18,21 +36,29 @@
 from .helpers import adjust_skip
 from .progress import progress
 
 __all__ = ['acf', 'gcf', 'gcf_offset', 'Correlation']
 
 _log = logging.getLogger(__name__)
 
-
 def acf(grid, skip, t, x):
     """
-    Auto correlation function.
+    Auto-correlation function <x(t)x(0)> of a time series x(t)
 
-    Calculate the correlation between time t(i0) and t(i0+i)
-    for all possible pairs (i0,i) provided by grid.
+    The correlation is between `x[i0+i]` and `x[i0]`, where `i` is
+    taken from the `grid` list and `i0` is a time origin. The average
+    <...> is over the time origins. The time differences are
+    calculated as `t[i0+i]-t[i0]`.
+
+    :param grid: list of time indices `i` for which the correlation is computed
+    :param skip: average every `skip` time origins
+    :param t: times t[i]
+    :param x: time series x[i]
+    :returns: list of time differences, list of correlation function,
+    list of number of time origins for each entry of the previou lists
     """
     cf = defaultdict(float)
     cnt = defaultdict(int)
     xave = numpy.average(x)
     for i in grid:
         for i0 in range(0, len(x)-i, skip):
             # Get the actual time difference
@@ -110,15 +136,15 @@
         iter(maybe_iterable)
     except TypeError:
         return False
     else:
         return True
 
 
-class Correlation(object):
+class Correlation:
     """
     Base class for correlation functions.
 
     The correlation function is calculated for the trajectory `trj`. This can be:
 
     - an object implementing the atooms `Trajectory` interface
     - the path to a trajectory file in a format recognized by atooms
@@ -143,15 +169,15 @@
     - `None`: a heuristics is used to keep the product of steps times particles constant
 
     Subclasses must provide a symbolic expression of the correlation
     function through the `symbol` class variable. The following
     convention is used: if a correlation function A depends on
     variables x and y, then `symbol = 'A(x,y)'`.
 
-    The `phasespace` variable allow subclasses to access a list of 2d
+    The `variables` variable allow subclasses to access a list of 2d
     numpy arrays with particles coordinates via the following private
     variables:
 
     - if `nbodies` is 1: `self._pos` for positions, `self._vel` for
     velocities, `self._unf_pos` for PBC-unfolded positions
 
     - if `nbodies` is 2, an additional suffix that take values 0 or 1
@@ -159,73 +185,85 @@
     e.g. `self._pos_0` and `self._pos_1`
     """
 
     nbodies = 1
     """
     Class variable that controls the number of bodies, i.e. particles,
     associated to the correlation function. This variable controls the
-    internal arrays used to compute the correlation, see `phasespace`.
+    internal arrays used to compute the correlation, see `variables`.
     """
     static = False
     """
     Turn this to `True` is the correlation function is static,
     i.e. not time-dependent. This may enable some optimizations.
     """
     symbol = ''
     """Example: fskt"""
-    # TODO: short name should be F_s
     short_name = ''
+    # TODO: rename name
     """Example: F_s(k,t)"""
-    tag_subscript = '_'
-    """Symbol used to introduce a tag, like _ in S_{A-A}(k,t)"""
     long_name = ''
+    # TODO: rename description
     """Example: Self intermediate scattering function"""
-    phasespace = ['pos', 'pos-unf', 'vel']
+    variables = ['pos', 'pos-unf', 'vel']
     """
     List of strings or string among ['pos', 'pos-unf', 'vel']. It
     indicates which variables should be read from the trajectory file.
     They will be available as self._pos, self._pos_unf, self._vel.
     """
     _symmetric = True
     """
     If nbodies>1, a symmetric correlation function is invariant under
     the exchange between _pos_0 and _pos_1. In that case, _symmetric
     is True.
     """
 
     def __init__(self, trj, grid, output_path=None, norigins=None, fix_cm=False):
+        """
+        The `output_path` instance variable is used to define the
+        output files by interpolating the following instance variables:
+
+        - `symbol`
+        - `short_name`
+        - `long_name`
+        - `tag`
+        - `tag_description`
+        - `trajectory`
+
+        The default is defined by core.pp_output_path, which currently
+        looks like '{trajectory.filename}.pp.{symbol}.{tag}'
+        """
         # Accept a trajectory-like instance or a path to a trajectory
         if isinstance(trj, str):
             self.trajectory = Trajectory(trj, mode='r', fmt=core.pp_trajectory_format)
         else:
             self.trajectory = trj
         self._fix_cm = fix_cm
         self._unfolded = None
         self.grid = grid
-        self.value = []
-        self.value_square = []
+        self.values = []
         self.origins = []
-        self.analysis = {}
-        # TODO: drop this
-        self.comments = None
         self.tag = ''
         self.tag_description = 'the whole system'
+        self._analysis = {}
         self._trajectory_path = self.trajectory.filename
         if self._trajectory_path is None:
             self.output_path = None
         else:
             self.output_path = output_path if output_path is not None else core.pp_output_path
         self.skip = adjust_skip(self.trajectory, norigins)
 
         # Callbacks
         self._cbk = []
         self._cbk_args = []
         self._cbk_kwargs = []
 
         # Lists for one body correlations
+        # TODO: group these vars better, there could be a single self._data dict
+        # then self._data_0['pos'], self._data_0['vel'], ...
         self._pos = []
         self._vel = []
         self._ids = []
         self._pos_unf = []
 
         # Lists for two-body correlations
         self._pos_0, self._pos_1 = [], []
@@ -238,14 +276,33 @@
         self._weight_0, self._weight_1 = None, None
         self._weight_field = None
         self._weight_fluctuations = False
 
     def __str__(self):
         return '{} at <{}>'.format(self.long_name, id(self))
 
+    # @property
+    # def grid(self):
+    #     if self._grid is None:
+    #         return numpy.array([])
+    #     return numpy.asarray(self._grid)
+
+    # @grid.setter
+    # def grid(self, val):
+    #     self._grid = val
+
+    # Note: value is deprecated in favor of values
+    @property
+    def value(self):
+        return self.values
+
+    @value.setter
+    def value(self, val):
+        self.values = val
+
     def add_weight(self, trajectory=None, field=None, fluctuations=False):
         """
         Add weight from the given `field` in `trajectory`
 
         If `trajectory` is `None`, `self.trajectory` will be used and
         `field` must be a particle property.
 
@@ -267,15 +324,15 @@
         # Guessing the field from the last column of an xyz file is
         # not supported anymore
         if field is None:
             raise ValueError('provide field to use as weight')
         else:
             self._weight_field = field
 
-        # By default we use the same trajectory as for the phasespace
+        # By default we use the same trajectory as for the variables
         if trajectory is None:
             self._weight_trajectory = self.trajectory
         else:
             self._weight_trajectory = trajectory
             # Copy over the field
             from .helpers import copy_field
             self.trajectory.add_callback(copy_field, self._weight_field, self._weight_trajectory)
@@ -295,35 +352,25 @@
         """Add filter callback `cbk` along with positional and keyword arguments"""
         if len(self._cbk) > self.nbodies:
             raise ValueError('number of filters cannot exceed n. of bodies')
         self._cbk.append(cbk)
         self._cbk_args.append(args)
         self._cbk_kwargs.append(kwargs)
 
-    def need_update(self):
-        """Check if the trajectory file is newer than the output file"""
-        # TODO: deprecate/remove this from next major version
-        need = True
-        if os.path.exists(self._output_file) and self._output_file != '/dev/stdout':
-            if os.path.getmtime(self.trajectory.filename) < \
-               os.path.getmtime(self._output_file):
-                need = False
-        return need
-
     def _setup_arrays(self):
         """
         Dump positions and/or velocities at different time frames as a
         list of numpy array.
         """
         # TODO: what happens if we call compute twice?? Shouldnt we reset the arrays?
-        # Ensure phasespace is a list.
+        # Ensure variables is a list.
         # It may not be a class variable anymore after this
-        if not isinstance(self.phasespace, list) and \
-           not isinstance(self.phasespace, tuple):
-            self.phasespace = [self.phasespace]
+        if not isinstance(self.variables, list) and \
+           not isinstance(self.variables, tuple):
+            self.variables = [self.variables]
 
         # Setup arrays
         if self.nbodies == 1:
             self._setup_arrays_onebody()
             self._setup_weight_onebody()
         elif self.nbodies == 2:
             self._setup_arrays_twobody()
@@ -335,46 +382,46 @@
 
         We also take care of dumping the weight if needed, see
         `add_weight()`.
         """
         # Local shortcut
         th = self.trajectory
 
-        # We unfold the trajectory if phasespace requests it and
+        # We unfold the trajectory if variables requests it and
         # unfolded positions are not available in the trajectory, or
         # if we request folded positions with fixed center of mass
-        if ('pos-unf' in self.phasespace and not hasattr(th[0].particle[0], 'position_unfolded')) or \
-           ('pos' in self.phasespace and self._fix_cm):
+        if ('pos-unf' in self.variables and not hasattr(th[0].particle[0], 'position_unfolded')) or \
+           ('pos' in self.variables and self._fix_cm):
             # We unfold the positions, caching the trajectory
             if self._unfolded is None:
                 self._unfolded = Unfolded(self.trajectory, fixed_cm=self._fix_cm)
                 # We must fold positions back in this case
-                if 'pos' in self.phasespace:
+                if 'pos' in self.variables:
                     self._unfolded.add_callback(fold)
             # Change the local shortcut to the unfolded trajectory
             th = self._unfolded
 
         # Read everything except unfolded trajectories
-        if 'pos' in self.phasespace or 'vel' in self.phasespace or 'ids' in self.phasespace:
+        if 'pos' in self.variables or 'vel' in self.variables or 'ids' in self.variables:
             ids = distinct_species(th[0].particle)
             for s in progress(th):
                 # Apply filter if there is one
                 if len(self._cbk) > 0:
                     s = self._cbk[0](s, *self._cbk_args[0], **self._cbk_kwargs[0])
-                if 'pos' in self.phasespace:
+                if 'pos' in self.variables:
                     self._pos.append(s.dump('pos'))
-                if 'vel' in self.phasespace:
+                if 'vel' in self.variables:
                     self._vel.append(s.dump('vel'))
-                if 'ids' in self.phasespace:
+                if 'ids' in self.variables:
                     _ids = s.dump('species')
                     _ids = numpy.array([ids.index(_) for _ in _ids], dtype=numpy.int32)
                     self._ids.append(_ids)
 
         # Read unfolded positions if requested
-        if 'pos-unf' in self.phasespace:
+        if 'pos-unf' in self.variables:
             if hasattr(th[0].particle[0], 'position_unfolded'):
                 # Unfolded positions are present in the trajectory
                 for s in progress(th):
                     # Fixing the CM must be done explicitly using
                     # particle.position_unfolded because atooms.system
                     # methods work with particle.position
                     # TODO: can be revised with atooms 3.4.0
@@ -463,47 +510,47 @@
             self._pos_1 = self._pos
             self._vel_0 = self._vel
             self._vel_1 = self._vel
             self._ids_0 = self._ids
             self._ids_1 = self._ids
             return
 
-        if 'pos' in self.phasespace or 'vel' in self.phasespace or 'ids' in self.phasespace:
+        if 'pos' in self.variables or 'vel' in self.variables or 'ids' in self.variables:
             ids = distinct_species(self.trajectory[0].particle)
             for s in progress(self.trajectory):
                 s0 = self._cbk[0](s, *self._cbk_args[0], **self._cbk_kwargs[0])
                 s1 = self._cbk[1](s, *self._cbk_args[1], **self._cbk_kwargs[1])
-                if 'pos' in self.phasespace:
+                if 'pos' in self.variables:
                     self._pos_0.append(s0.dump('pos'))
                     self._pos_1.append(s1.dump('pos'))
-                if 'vel' in self.phasespace:
+                if 'vel' in self.variables:
                     self._vel_0.append(s0.dump('vel'))
                     self._vel_1.append(s1.dump('vel'))
-                if 'ids' in self.phasespace:
+                if 'ids' in self.variables:
                     _ids_0 = s0.dump('species')
                     _ids_1 = s1.dump('species')
                     _ids_0 = numpy.array([ids.index(_) for _ in _ids_0], dtype=numpy.int32)
                     _ids_1 = numpy.array([ids.index(_) for _ in _ids_1], dtype=numpy.int32)
                     self._ids_0.append(_ids_0)
                     self._ids_1.append(_ids_1)
 
         # Dump unfolded positions if requested
-        if 'pos-unf' in self.phasespace:
+        if 'pos-unf' in self.variables:
             for s in progress(Unfolded(self.trajectory)):
                 s0 = self._cbk[0](s, *self._cbk_args[0], **self._cbk_kwargs[0])
                 s1 = self._cbk[1](s, *self._cbk_args[1], **self._cbk_kwargs[1])
                 self._pos_unf_0.append(s0.dump('pos'))
                 self._pos_unf_1.append(s1.dump('pos'))
 
     def compute(self):
         """
         Compute the correlation function.
 
         It wraps the _compute() method implemented by subclasses.
-        This method sets the `self.grid` and `self.value` variables,
+        This method sets the `self.grid` and `self.values` variables,
         which are also returned.
         """
         _log.info('setup arrays for %s', self.tag_description)
         t = [Timer(), Timer()]
         t[0].start()
         self._setup_arrays()
         t[0].stop()
@@ -520,178 +567,215 @@
         _log.info('done %s for %s in %.1f sec [setup:%.0f%%, compute: %.0f%%]',
                   self.long_name,
                   self.tag_description, t[0].wall_time + t[1].wall_time,
                   t[0].wall_time / (t[0].wall_time + t[1].wall_time) * 100,
                   t[1].wall_time / (t[0].wall_time + t[1].wall_time) * 100)
         _log.info('')
 
-        # Unset the trajectory instance so that the Correlation instance
-        # can be pickled without storing it.
-        # TODO: close it if it had been created from a path
-        self.trajectory = None
-        
-        return self.grid, self.value
+        # TODO: refactor
+        # Clear data to cut down object memory footprint
+        self._pos = []
+        self._vel = []
+        self._ids = []
+        self._pos_unf = []
+
+        # Lists for two-body correlations
+        self._pos_0, self._pos_1 = [], []
+        self._vel_0, self._vel_1 = [], []
+        self._ids_0, self._ids_1 = [], []
+        self._pos_unf_0, self._pos_unf_1 = [], []
+
+        return self.grid, self.values
+
+    def __getstate__(self):
+        # Unset the trajectory instance and dumps so that the Correlation
+        # can be pickled without storing it
+        ignore = ['trajectory']
+        data = {key: value for key, value in self.__dict__.items() if key not in ignore}
+        data = {'grid': self.grid, 'values': self.values, 'analysis': self.analysis}
+        return data
+
+    def __setstate__(self, data):
+        for key in data:
+            setattr(self, key, data[key])
 
     def _compute(self):
         """Subclasses must implement this"""
         pass
 
     def analyze(self):
         """
         Subclasses may implement this and store the results in the
         self.analysis dictonary
         """
         pass
 
+    @staticmethod
+    def _split_math_func(name):
+        if '(' in name:
+            name, variables = name.split('(')
+            name = name.strip()
+            variables = variables.strip().rstrip(')').split(',')
+            return name, variables
+        return name, None
+
+    @property
+    def grid_name(self):
+        return self._split_math_func(self.short_name)[1]
+
+    @property
+    def _base_name(self):
+        return self._split_math_func(self.short_name)[0]
+
     def _interpolate_path(self, path):
         import re
         # Keep backward compatibility
         path = re.sub('trajectory.filename', 'trajectory', path)
         path = path.format(symbol=self.symbol,
+                           qualified_name=self.qualified_name,
                            short_name=self.short_name,
                            long_name=self.long_name.replace(' ', '_'),
                            tag=self.tag,
                            tag_description=self.tag_description.replace(' ', '_'),
                            trajectory=self._trajectory_path)
 
         # Strip unpleasant punctuation from basename path
         for punct in ['.', '_', '-']:
             subpaths = path.split('/')
             subpaths[-1] = subpaths[-1].replace(punct * 2, punct)
             subpaths[-1] = subpaths[-1].strip(punct)
             path = '/'.join(subpaths)
         return path
-        
+
     @property
     def _output_file(self):
         """Returns path of output file"""
-        # Interpolate the output path string        
+        # Interpolate the output path string
         if self.output_path is None:
             return None
         else:
             return self._interpolate_path(self.output_path)
 
-    def read(self):
-        """Read correlation function from existing file"""
-        with open(self._output_file, 'r') as inp:
-            x = numpy.loadtxt(inp, unpack=True)
-            if len(x) == 3:
-                _log.warn("cannot read 3-columns files yet in %s", self._output_file)
-            elif len(x) == 2:
-                self.grid, self.value = x
-            else:
-                self.grid, self.value = x[0: 2]
-                _log.warn("Ignoring some columns in %s", self._output_file)
-
-    @property
-    def grid_name(self):
-        """
-        Return the name of the grid variables
-
-        Example:
-        -------
-        If `self.name` is `F_s(k,t)`, the function returns `['k', 't']`
-        """
-        variables = self.short_name.split('(')[1][:-1]
-        return variables.split(',')
-
-    def write(self, output_path=None):
+    def write(self):
         """
         Write the correlation function and the analysis data to file
-
-        The `output_path` instance variable is used to define the
-        output files by interpolating the following variables:
-
-        - symbol
-        - short_name
-        - long_name
-        - tag
-        - tag_description
-        - trajectory
-
-        The default is defined by core.pp_output_path, which currently
-        looks like '{trajectory.filename}.pp.{symbol}.{tag}'
         """
         from .helpers import _itemize
 
         # Exit right away when no output paths are defined
-        if output_path is None and self._output_file is None:
+        if self._output_file is None:
             return
-        path = self._output_file
-        if output_path is not None:
-            path = self._interpolate_path(output_path)
 
         # Pack grid and value into arrays to dump
         if _is_iterable(self.grid[0]) and len(self.grid) == 2:
-            x = numpy.array(self.grid[0]).repeat(len(self.value[0]))
+            x = numpy.array(self.grid[0]).repeat(len(self.values[0]))
             y = numpy.array(self.grid[1] * len(self.grid[0]))
-            z = numpy.array(self.value).flatten()
+            z = numpy.array(self.values).flatten()
             dump = numpy.transpose(numpy.array([x, y, z]))
         else:
-            dump = numpy.transpose(numpy.array([self.grid, self.value]))
+            dump = numpy.transpose(numpy.array([self.grid, self.values]))
 
         # Comment line
-        # Extract variables from parenthesis in symbol
-        variables = self.short_name.split('(')[1][:-1]
-        variables = variables.split(',')
-        # TODO: simplify this by using only correlation name (without vars)
-        tag = '{' + self.tag + '}' if len(self.tag) > 1 else self.tag
-        correlation_name = self.short_name.split('(')[0] + self.tag_subscript + tag
-        correlation_name = correlation_name.rstrip(self.tag_subscript)
-        # Use ; instead of , to separate variables to make it easier to parse
-        # TODO: remove this by using only correlation name (without vars)
-        correlation_name += '(' + self.short_name.split('(')[1]  #.replace(',', ';')
+        columns = self.grid_name + [self.qualified_name]
         conj = 'of' if len(self.tag_description) > 0 else ''
         metadata = {
-            'title': f'{self.long_name} {self.short_name} {conj} {self.tag_description}',
-            'columns': ', '.join(variables + [correlation_name.strip('^')]),
+            'title': f'{self.long_name}, {self.qualified_name}, {conj} {self.tag_description}',
+            'columns': ', '.join(columns),
         }
-        # Results of analysis
+        # Add results of analysis in the header
         metadata.update(self.analysis)
 
         # Write as columnar file
-        mkdir(os.path.dirname(path))
-        with open(path, 'w') as fh:
+        mkdir(os.path.dirname(self._output_file))
+        with open(self._output_file, 'w') as fh:
             for key, value in metadata.items():
                 fh.write(f'# {key}: {value}\n')
             numpy.savetxt(fh, dump, fmt="%g")
 
         # Write analysis as yaml
         # if len(self.analysis) > 0:
         #    import yaml
         #    with open(path + '.yaml', 'w') as fh:
         #        yaml.dump(_itemize(self.analysis), fh)
 
-    def do(self, update=False):
+    def do(self):
         """
         Do the full template pattern: compute, analyze and write the
         correlation function.
         """
-        if update and not self.need_update():
-            self.read()
-            return
-
         self.compute()
-
         try:
             self.analyze()
         except ImportError as e:
             _log.warn('Could not analyze due to missing modules, continuing...')
             _log.warn(e)
-
         self.write()
+        return {**self.results, **self.analysis}
 
     def __call__(self):
         self.do()
 
+    # TODO: deprecate or alias to plot
     def show(self, now=True):
         try:
             import matplotlib.pyplot as plt
         except ImportError:
             return
 
         if not _is_iterable(self.grid[0]):
-            plt.plot(self.grid, self.value, label=self.tag)
+            plt.plot(self.grid, self.values, label=self.tag)
             plt.ylabel(self.short_name)
             plt.xlabel(self.grid_name[0])
         if now:
             plt.show()
+
+    def plot(self, show=False, ax=None, fig=None):
+        try:
+            import matplotlib.pyplot as plt
+        except ImportError:
+            return
+
+        if not _is_iterable(self.grid[0]):
+            if ax is None:
+                fig, ax = plt.subplots()
+            ax.plot(self.grid, self.values, label=self.tag)
+            ax.set_ylabel(self.qualified_name)
+            ax.set_xlabel(self.grid_name[0])
+        if show:
+            fig.show()
+        return fig, ax
+
+    def _qualify_name(self, name):
+        basename, gridname = self._split_math_func(name)
+        tag = '{' + self.tag + '}' if len(self.tag) > 1 else self.tag
+        tag = '_' + tag if len(tag) > 0 else ''
+        if gridname is not None:
+            return basename + tag + '(' + ','.join(gridname) + ')'
+        return basename.strip() + tag
+
+    @property
+    def qualified_name(self):
+        return self._qualify_name(self.short_name)
+
+    def asarray(self):
+        assert len(self.grid_name) in [1, 2], f'Unsupported grid dimension={len(self.grid_name)}'
+
+        if len(self.grid_name) == 1:
+            return numpy.array([self.grid, self.values])
+
+        if len(self.grid_name) == 2:
+            x = numpy.array(self.grid[0]).repeat(len(self.values[0]))
+            y = numpy.array(self.grid[1] * len(self.grid[0]))
+            z = numpy.array(self.values).flatten()
+            return numpy.array([x, y, z])
+
+    @property
+    def results(self):
+        return {self.qualified_name: self.asarray()}
+
+    @property
+    def analysis(self):
+        return {self._qualify_name(name.split(',')[1]): value for name, value in self._analysis.items()}
+
+    @analysis.setter
+    def analysis(self, value):
+        self._analysis = value
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/filter.py` & `atooms_pp-4.0.0/atooms/postprocessing/filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """
 Decorator to filter correlation functions by arbitrary condition
 on particle properties.
 
 It uses filters internally.
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/fkt.py` & `atooms_pp-4.0.0/atooms/postprocessing/fkt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Intermediate scattering function."""
 
 import logging
 from collections import defaultdict
 
 import numpy
@@ -17,37 +17,38 @@
 __all__ = ['SelfIntermediateScattering',
            'SelfIntermediateScatteringLegacy', 'SelfIntermediateScatteringFast',
            'IntermediateScattering']
 
 _log = logging.getLogger(__name__)
 _one_over_e = 1 / numpy.exp(1.0)
 
-def _write_tau(out, db):
+def _write_tau(out, key, tau_k):
+    # TODO: refactor this
     # Custom writing of relaxation times
     out.write('# title: relaxation times tau(k) as a function of k\n')
-    out.write('# columns: k, tau(k)\n')
+    out.write(f'# columns: k, {key}\n')
     out.write('# note: tau is the time at which the correlation function has decayed to 1/e\n')
-    for k, tau in db['relaxation times tau'].items():
+    for k, tau in zip(tau_k[0], tau_k[1]):
         out.write('{} {}\n'.format(k, tau))
 
 def _extract_tau(k, t, f, factor=_one_over_e):
     from .helpers import feqc
     # Ensure first point in time grid is t=0
     # This will be enforced by the classes below but we never know
     if t[0] > 0:
         raise ValueError('First point in time grid must be zero')
-    tau = {}
-    for i, _k in enumerate(k):
+    tau = []
+    for ik in range(len(k)):
         try:
-            tauk = feqc(t, f[i], f[i][0]*factor)[0]
+            tauk = feqc(t, f[ik], f[ik][0]*factor)[0]
             if tauk is None:
                 tauk = float('nan')
-            tau[_k] = tauk
         except ValueError:
-            tau[_k] = float('nan')
+            tau = float('nan')
+        tau.append(tauk)
     return tau
 
 # TODO: norigins should be in kwargs
 
 class IntermediateScatteringBase(FourierSpaceCorrelation):
 
     def __init__(self, trajectory, kgrid=None, tgrid=None, nk=1,
@@ -86,17 +87,16 @@
 
     See the documentation of the `FourierSpaceCorrelation` base class
     for information on the instance variables.
     """
 
     symbol = 'fskt'
     short_name = 'F_s(k,t)'
-    tag_subscript = '^'
     long_name = 'self intermediate scattering function'
-    phasespace = 'pos'
+    variables = 'pos'
 
     def __init__(self, trajectory, kgrid=None, tgrid=None, nk=8,
                  tsamples=60, dk=0.1, kmin=1.0, kmax=10.0,
                  ksamples=10, norigins=-1, lookup_mb=64.0, normalize=True, **kwargs):
         super(SelfIntermediateScatteringLegacy,
               self).__init__(trajectory, kgrid=kgrid, tgrid=tgrid,
                              nk=nk, tsamples=tsamples, dk=dk, kmin=kmin,
@@ -159,46 +159,51 @@
         # Normalization
         if self.normalize:
             for k in range(len(self.grid[0])):
                 for i in range(len(self.value[k])):
                     self.value[k][i] /= self.value[k][0]
 
     def analyze(self):
-        self.analysis['relaxation times tau'] = _extract_tau(self.grid[0], self.grid[1], self.value)
+        taus = _extract_tau(self.grid[0], self.grid[1], self.value)        
+        self._analysis['relaxation time, tau(k)'] = [self.grid[0], taus]
 
     def write(self):
         Correlation.write(self)
+        # TODO: refactor
+        if self._output_file is None:
+            return
         if self._output_file != '/dev/stdout':
             with open(self._output_file + '.tau', 'w') as out:
-                _write_tau(out, self.analysis)
+                _write_tau(out,  self._qualify_name('tau(k)'),
+                           self._analysis['relaxation time, tau(k)'])
 
 
 class SelfIntermediateScatteringFast(SelfIntermediateScatteringLegacy):
     """
     Self part of the intermediate scattering function (fast version)
 
     See the documentation of the `FourierSpaceCorrelation` base class
     for information on the instance variables.
     """
 
     def _compute(self):
-        from atooms.postprocessing.fourierspace_wrap import fourierspace_module
+        from atooms.postprocessing.core import f90
 
         # Shortcuts
         pos = numpy.array(self._pos)
         ndims = len(self.k0)
         skip = self.skip
 
         # Select the f90 kernel
         if ndims == 3:
-            fskt_kernel = fourierspace_module.fskt_kernel_3d
+            fskt_kernel = f90.fourierspace.fskt_kernel_3d
         elif ndims == 2:
-            fskt_kernel = fourierspace_module.fskt_kernel_2d
+            fskt_kernel = f90.fourierspace.fskt_kernel_2d
         else:
-            fskt_kernel = fourierspace_module.fskt_kernel_nd
+            fskt_kernel = f90.fourierspace.fskt_kernel_nd
 
         # To optimize without wasting too much memory (we have
         # troubles here) we group particles in blocks and tabulate the
         # exponentials over time. This is more memory consuming but we
         # can optimize the inner loop. The esitmated amuount of
         # allocated memory in Mb for the expo array is
         # self.lookup_mb. Note that the actual memory used scales
@@ -244,15 +249,15 @@
             for k in range(len(self.grid[0])):
                 for i in range(len(self.value[k])):
                     self.value[k][i] /= self.value[k][0]
 
 
 # Defaults to fast
 try:
-    import atooms.postprocessing.fourierspace_wrap
+    from atooms.postprocessing.core import f90
     SelfIntermediateScattering = SelfIntermediateScatteringFast
 except ImportError:
     SelfIntermediateScattering = SelfIntermediateScatteringLegacy
 
 
 class IntermediateScattering(IntermediateScatteringBase):
     """
@@ -262,15 +267,15 @@
     for information on the instance variables.
     """
 
     nbodies = 2
     symbol = 'fkt'
     short_name = 'F(k,t)'
     long_name = 'intermediate scattering function'
-    phasespace = 'pos'
+    variables = 'pos'
 
     def __init__(self, trajectory, kgrid=None, tgrid=None, nk=100, dk=0.1, tsamples=60,
                  kmin=1.0, kmax=10.0, ksamples=10, norigins=-1, normalize=True, **kwargs):
         super(IntermediateScattering, self).__init__(trajectory, kgrid=kgrid, tgrid=tgrid,
                                                      nk=nk, tsamples=tsamples, dk=dk, kmin=kmin,
                                                      kmax=kmax, ksamples=ksamples, norigins=norigins,
                                                      normalize=normalize, **kwargs)
@@ -362,14 +367,19 @@
         # Normalize
         if self.normalize:
             self.value = [[v / self.value_nonorm[k][0] for v in self.value_nonorm[k]] for k in range(len(acf))]
         else:
             self.value = self.value_nonorm
 
     def analyze(self):
-        self.analysis['relaxation times tau'] = _extract_tau(self.grid[0], self.grid[1], self.value)
+        taus = _extract_tau(self.grid[0], self.grid[1], self.value)
+        self._analysis['collective relaxation time, tau_c(k)'] = [self.grid[0], taus]
 
     def write(self):
         Correlation.write(self)
+        # TODO: refactor
+        if self._output_file is None:
+            return
         if self._output_file != '/dev/stdout':
             with open(self._output_file + '.tau', 'w') as out:
-                _write_tau(out, self.analysis)
+                _write_tau(out, self._qualify_name('tau_c(k)'),
+                           self._analysis['collective relaxation time, tau_c(k)'])
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/fourierspace.py` & `atooms_pp-4.0.0/atooms/postprocessing/fourierspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Fourier-space post processing code."""
 
 import math
 import logging
 import random
 from collections import defaultdict
@@ -122,19 +122,16 @@
                  kmin=-1, kmax=10, ksamples=20, normalize=True, **kwargs):
         super(FourierSpaceCorrelation, self).__init__(trajectory, grid,
                                                       norigins=norigins, **kwargs)
         # Some additional variables. 
         self.normalize = normalize
         
         # Find grid of k-vector norms and store it sorted as self.kgrid
-        # We first try with self.grid
-        variables = self.short_name.split('(')[1][:-1]
-        variables = variables.split(',')
-        if len(variables) > 1:
-            kgrid = self.grid[variables.index('k')]
+        if len(self.grid_name) > 1:
+            kgrid = self.grid[self.grid_name.index('k')]
         else:
             kgrid = self.grid
 
         # Define k-vectors
         if isinstance(kgrid, FourierSpaceGrid):
             # We keep the FourierSpaceGrid instance as a private variable
             self._kgrid = kgrid
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/gr.py` & `atooms_pp-4.0.0/atooms/postprocessing/gr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Radial distribution function."""
 
 import math
 import logging
 
 import numpy
@@ -33,15 +33,15 @@
     r = x-y
     r = r - numpy.rint(r/L) * L
     return numpy.sum(r**2, axis=1)
 
 def pairs_newton_hist(f, x, y, L, bins):
     """
     Apply function f to all pairs in x[i] and y[j] and update the
-    |hist| histogram using the |bins| bin edges.
+    `hist` histogram using the `bins` bin edges.
     """
     hist, bins = numpy.histogram([], bins)
     # Do the calculation in batches to optimize
     bl = max(1, int(1e5 / len(y)))
     for ib in range(0, len(y)-1, bl):
         fxy = []
         # batch must never exceed len(y)-1
@@ -52,15 +52,15 @@
         hist += hist_tmp
     return hist
 
 
 def pairs_hist(f, x, y, L, bins):
     """
     Apply function f to all pairs in x[i] and y[j] and update the
-    |hist| histogram using the |bins| bin edges.
+    `hist` histogram using the `bins` bin edges.
     """
     hist, bins = numpy.histogram([], bins)
     for i in range(len(y)):
         fxy = f(x[:], y[i], L)
         hist_tmp, bins = numpy.histogram(fxy, bins)
         hist += hist_tmp
     return hist
@@ -82,15 +82,15 @@
       the time average
     """
 
     nbodies = 2
     symbol = 'gr'
     short_name = 'g(r)'
     long_name = 'radial distribution function'
-    phasespace = 'pos'
+    variables = 'pos'
 
     def __init__(self, trajectory, rgrid=None, dr=0.04, ndim=-1, rmax=-1.0, **kwargs):
         Correlation.__init__(self, trajectory, rgrid, **kwargs)
         self.dr = dr
         self.rmax = rmax
         """
         Limit distance binning up to `rmax`. It may enable linked cells if
@@ -206,15 +206,15 @@
 
     - `norigins`: controls the number of trajectory frames to compute
       the time average
     """
 
     def _compute(self):
         import sys
-        from atooms.postprocessing.realspace_wrap import compute
+        from atooms.postprocessing.core import f90
         from atooms.postprocessing.linkedcells import LinkedCells
 
         # Assume grandcanonical trajectory for generality.
         # Note that testing if the trajectory is grandcanonical or
         # semigrandcanonical is useless when applying filters.
         N_0, N_1 = [], []
         gr_all = []
@@ -268,15 +268,15 @@
             # domain, we crop particles away from the surface (within rmax)
             system = self.trajectory.read(i)
             if system.cell is not None and hasattr(system.cell, 'periodic') and \
                sum(system.cell.periodic) == 0:
                 assert self.rmax > 0, 'provide rmax>0'
                 # Booleans do not work here, so we just use integers,
                 # which are 1 is particles are on the surface and 0 otherwise
-                mask = compute.on_surface_c(pos_0, system.cell.side, self.rmax)
+                mask = f90.realspace.on_surface_c(pos_0, system.cell.side, self.rmax)
                 pos_0 = pos_0[mask == 0, :]
                 # Force distinct calculation. This gives a spurious signal at r=0, which we remove
                 distinct = True
                 remove_self_term = True
 
             # When using linked cells, we precalculate the neighbors
             # This will only happen if the system is within a cell (and all directions are periodic)
@@ -306,31 +306,31 @@
             # Store number of particles for normalization
             N_0.append(pos_0.shape[0])
             if distinct:
                 N_1.append(pos_1.shape[0])
             else:
                 N_1.append(pos_0.shape[0])
 
-            # Compute g(r)
+            # F90.Realspace g(r)
             if not distinct:
                 if linkedcells is None:
-                    compute.gr_self_c(pos_0, side, dr, gr, bins)
+                    f90.realspace.gr_self_c(pos_0, side, dr, gr, bins)
                 else:
-                    compute.gr_neighbors_self_c('C', pos_0, neighbors, number_of_neighbors, side, dr, gr, bins)
+                    f90.realspace.gr_neighbors_self_c('C', pos_0, neighbors, number_of_neighbors, side, dr, gr, bins)
             else:
                 if linkedcells is None:
-                    compute.gr_distinct_c(pos_0, pos_1, side, dr, gr, bins)
+                    f90.realspace.gr_distinct_c(pos_0, pos_1, side, dr, gr, bins)
                 else:
-                    compute.gr_neighbors_distinct_c('C', pos_0, pos_1, neighbors, number_of_neighbors, side, dr, gr, bins)
+                    f90.realspace.gr_neighbors_distinct_c('C', pos_0, pos_1, neighbors, number_of_neighbors, side, dr, gr, bins)
 
             # Damned copies in python
             gr_all.append(gr.copy())
         
         # Normalization
-        # Array r is used to compute shells, we thus use the bin boundaries
+        # Array r is used to f90.realspace shells, we thus use the bin boundaries
         r = bins - (bins[1] - bins[0]) / 2
         N_0 = numpy.average(N_0)
         N_1 = numpy.average(N_1)
         if system.cell is not None:
             volume = system.cell.volume
         else:
             volume = len(system.particle) / system.density
@@ -364,12 +364,12 @@
             side = system.cell.side
             where = self.grid <= min(side) / 2
         self.grid = self.grid[where]
         self.value = self.value[where]
 
 
 # Defaults to fast
-try:
-    import atooms.postprocessing.realspace_wrap
-    RadialDistributionFunction = RadialDistributionFunctionFast
-except ImportError:
+from . import core
+if core.f90 is None:
     RadialDistributionFunction = RadialDistributionFunctionLegacy
+else:
+    RadialDistributionFunction = RadialDistributionFunctionFast
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/helpers.py` & `atooms_pp-4.0.0/atooms/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/ik.py` & `atooms_pp-4.0.0/atooms/postprocessing/ik.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Free volume spectral density."""
 
 import numpy
 from atooms.trajectory import Trajectory
 from atooms.trajectory.utils import is_cell_variable
 
@@ -22,15 +22,15 @@
     See the documentation of the `FourierSpaceCorrelation` base class
     for information on the instance variables.
     """
 
     symbol = 'ik'
     short_name = 'I(k)'
     long_name = 'spectral density'
-    phasespace = 'pos'
+    variables = 'pos'
 
     def __init__(self, trajectory, trajectory_radius, kgrid=None,
                  norigins=-1, nk=20, dk=0.1, kmin=-1.0, kmax=15.0,
                  ksamples=30, **kwargs):
         FourierSpaceCorrelation.__init__(self, trajectory, kgrid, norigins, nk,
                                          dk, kmin, kmax, ksamples, **kwargs)
         self._is_cell_variable = None
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/linkedcells.py` & `atooms_pp-4.0.0/atooms/postprocessing/linkedcells.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,17 @@
     def compute(self, box, pos, other=None, as_array=False, newton=True, periodic=None):
         if not self._is_adjusted:
             self.adjust(box, newton=other is None and newton, periodic=periodic)
             self._is_adjusted = True
         # We only need positions here but how can we be sure that
         # this is the same set of particles we use when retrieving
         # the neighbours? We should keep a reference.
-        # from atooms.postprocessing.realspace_wrap import compute
+        # from atooms.postprocessing.core import f90
         # index = numpy.ndarray(pos.shape, dtype=numpy.int32)
-        # compute.bin_in_cell(pos, self.hbox, self.box_cell, index)
+        # f90.realspace.bin_in_cell(pos, self.hbox, self.box_cell, index)
 
         self.neighbors = []
         self.number_of_neighbors = []
         index = self._index(pos)
         if other is None:
             index_other = index
         else:
@@ -210,15 +210,15 @@
 # print('#', lc.box_cell / (system.cell.side/2))
 # print('----')
 
 # for j in nn[0][0:num[0]]:
 #     dr = system.particle[0].distance(system.particle[j], system.cell)
 #     print(numpy.sum(dr**2)**0.5, lc.box_cell[0] * 2)
 
-# # from atooms.postprocessing.realspace_wrap import compute
+# # from atooms.postprocessing.core.realspace_f90 import compute
 # # rcut = numpy.array([[1.5, 1.5], [1.5, 1.5]])
 # # rcut[:] = lc.box_cell[0] * 2
 # # max_neighbors = 300
 # # number_of_neighbors = numpy.ndarray(pos.shape[0], dtype=numpy.int32)
 # # neighbors = numpy.ndarray((pos.shape[0], max_neighbors), dtype=numpy.int32, order='F')
 # # #print(pos.shape)
 # # pos = numpy.array(pos, order='F')
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/msd.py` & `atooms_pp-4.0.0/atooms/postprocessing/msd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Mean square displacement."""
 
 import logging
 import numpy
 
 from .helpers import linear_grid
@@ -34,15 +34,15 @@
     used to limit the fit range to extract the diffusion coefficient
     and to determine the diffusion time
     """
 
     symbol = 'msd'
     short_name = 'dr^2(t)'
     long_name = 'mean square displacement'
-    phasespace = 'pos-unf'
+    variables = 'pos-unf'
 
     def __init__(self, trajectory, tgrid=None, rmax=-1.0, norigins=None,
                  tsamples=30, sigma=1.0, no_offset=False, **kwargs):
         self.rmax = rmax
         self.sigma = sigma
         self.tsamples = tsamples
         self._norigins = norigins
@@ -79,20 +79,21 @@
         # Update grid to real time
         self.grid = [ti * self.trajectory.timestep for ti in self.grid]
 
     def analyze(self):
         # Get the time when MSD equals sigma**2
         try:
             from .helpers import feqc
-            self.analysis['diffusive time tau_D'] = feqc(self.grid, self.value, self.sigma**2)[0]
+            tau_D = feqc(self.grid, self.value, self.sigma**2)[0]
         except ValueError:
-            self.analysis['diffusive time tau_D'] = float('nan')
-
+            tau_D = float('nan')
+        self._analysis['diffusive time, tau_D'] = tau_D
+        
         where = numpy.array(self.value) > self.sigma**2
         if sum(where) < 2:
             _log.warn('could not fit MSD: not enough data above sigma')
             return
 
         from .helpers import linear_fit
         diffusion = linear_fit(numpy.array(self.grid)[where],
                                numpy.array(self.value)[where])
-        self.analysis['diffusion coefficient D'] = diffusion[0] / (2*self._ndim)
+        self._analysis['diffusion coefficient, D'] = diffusion[0] / (2*self._ndim)
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/partial.py` & `atooms_pp-4.0.0/atooms/postprocessing/partial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """
 Fake decorator to compute partial correlation functions.
 
 It uses filters internally.
 """
 
@@ -76,14 +76,15 @@
         for key in self.partial:
             self.partial[key].output_path = path
 
     def add_weight(self, trajectory=None, field=None, fluctuations=False):
         for key in self.partial:
             self.partial[key].add_weight(trajectory, field, fluctuations)
 
+    # TODO: drop this
     def need_update(self):
         need = False
         for partial in self.partial.values():
             if partial.need_update():
                 need = True
                 break
         return need
@@ -107,27 +108,35 @@
                         self.partial[(isp, jsp)].value = self.partial[(jsp, isp)].value
                         self.partial[(isp, jsp)].analysis = self.partial[(jsp, isp)].analysis
 
     def write(self):
         for partial in self.partial.values():
             partial.write()
 
-    def do(self, update=False):
-        if update and not self.need_update():
-            for partial in self.partial.values():
-                partial.read()
-            return
-
+    def do(self):
         self.compute()
-
         for partial in self.partial.values():
             try:
                 partial.analyze()
             except ImportError as e:
                 _log.warn('Could not analyze due to missing modules, continuing...')
                 _log.warn(e)
-
             partial.write()
-
+        return {**self.results, **self.analysis}
+            
     def __call__(self):
         self.do()
-            
+
+    @property
+    def results(self):
+        res = {}
+        for partial in self.partial.values():
+            res.update(partial.results)
+        return res
+
+    @property
+    def analysis(self):
+        res = {}
+        for partial in self.partial.values():
+            res.update(partial.analysis)
+        return res
+
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/progress.py` & `atooms_pp-4.0.0/atooms/postprocessing/progress.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/qt.py` & `atooms_pp-4.0.0/atooms/postprocessing/qt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Time-dependent overlap."""
 
 import numpy
 
 from .helpers import logx_grid
 from .correlation import Correlation, gcf_offset
@@ -38,15 +38,15 @@
 class CollectiveOverlap(Correlation):
 
     """Time-dependent collective overlap."""
 
     symbol = 'qt'
     short_name = 'Q(t)'
     long_name = 'collective overlap'
-    phasespace = 'pos'
+    variables = 'pos'
 
     def __init__(self, trajectory, tgrid=None, tsamples=60, a=0.3,
                  norigins=-1, **kwargs):
         Correlation.__init__(self, trajectory, tgrid, norigins=norigins, **kwargs)
         self.a_square = a**2
         if tgrid is None:
             self.grid = logx_grid(0.0, self.trajectory.total_time * 0.75, tsamples)
@@ -63,15 +63,15 @@
 class SelfOverlap(Correlation):
 
     """Time-dependent self overlap."""
 
     symbol = 'qst'
     short_name = 'Q_s(t)'
     long_name = 'self overlap'
-    phasespace = 'pos-unf'
+    variables = 'pos-unf'
 
     def __init__(self, trajectory, tgrid=None, norigins=-1, a=0.3,
                  tsamples=60, **kwargs):
         Correlation.__init__(self, trajectory, tgrid, norigins=norigins, **kwargs)
         if tgrid is None:
             self.grid = logx_grid(0.0, trajectory.total_time * 0.75, tsamples)
         self._discrete_tgrid = setup_t_grid(self.trajectory, self.grid, offset=norigins != '1')
@@ -83,10 +83,10 @@
         self.grid, self.value = gcf_offset(f, self._discrete_tgrid,
                                            self.skip, self.trajectory.steps, self._pos_unf)
         self.grid = [ti * self.trajectory.timestep for ti in self.grid]
 
     def analyze(self):
         try:
             from .helpers import feqc
-            self.analysis['tau'] = feqc(self.grid, self.value, 1 / numpy.exp(1.0))[0]
+            self._analysis['relaxation time, tau_q'] = feqc(self.grid, self.value, 1 / numpy.exp(1.0))[0]
         except ValueError:
-            self.analysis['tau'] = None
+            self._analysis['relaxation time, tau_q'] = None
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/s4kt.py` & `atooms_pp-4.0.0/atooms/postprocessing/s4kt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Four-point dynamic structure factor."""
 
 from collections import defaultdict
 import numpy
 
 from .fourierspace import FourierSpaceCorrelation, expo_sphere
@@ -21,15 +21,15 @@
     See the documentation of the `FourierSpaceCorrelation` base class
     for information on the instance variables.
     """
 
     symbol = 's4kt'
     short_name = 'S_4(t,k)'
     long_name = '4-point dynamic structure factor from self overlap'
-    phasespace = ['pos-unf']
+    variables = ['pos-unf']
 
     # TODO: refactor a S4k base correlation that forces to implement tabulat method (e.g. overlap, Q_6, voronoi ...)
     # TODO: should we drop this instead and rely on F(k,t) with grandcanonical
 
     def __init__(self, trajectory, tgrid, kgrid=None, norigins=-1,
                  nk=20, dk=0.1, a=0.3, kmin=1.0, kmax=10.0, ksamples=10, **kwargs):
         FourierSpaceCorrelation.__init__(self, trajectory, [tgrid, kgrid], norigins,
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/sacf.py` & `atooms_pp-4.0.0/atooms/postprocessing/sacf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Stress autocorrelation function."""
 
 import numpy
 
 from .correlation import Correlation, gcf_offset
 from .helpers import setup_t_grid
@@ -15,15 +15,15 @@
 class StressAutocorrelation(Correlation):
 
     """Stress autocorrelation function."""
 
     symbol = 'sacf'
     short_name = 'S(t)'
     long_name = 'stress autocorrelation'
-    phasespace = ['vel']
+    variables = ['vel']
 
     def __init__(self, trajectory, tgrid, **kwargs):
         Correlation.__init__(self, trajectory, tgrid, **kwargs)
         self._discrete_tgrid = setup_t_grid(self.trajectory, tgrid, offset=norigins != '1')
 
     def _get_stress(self):
         ndims = 3
@@ -46,10 +46,7 @@
 
         self._get_stress()
         V = self.trajectory.read(0).cell.volume
         self.grid, self.value = gcf_offset(f, self._discrete_tgrid, self.trajectory.block_size,
                                            self.trajectory.steps, self._stress)
         self.value = [x / V for x in self.value]
         self.grid = [ti * self.trajectory.timestep for ti in self.grid]
-
-    def analyze(self):
-        pass
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/sk.py` & `atooms_pp-4.0.0/atooms/postprocessing/sk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Structure factor."""
 
 import logging
 import numpy
 
 from .progress import progress
@@ -45,15 +45,15 @@
     for information on the instance variables.
     """
 
     nbodies = 2
     symbol = 'sk'
     short_name = 'S(k)'
     long_name = 'structure factor'
-    phasespace = ['pos']
+    variables = ['pos']
 
     def __init__(self, trajectory, kgrid=None, norigins=-1, nk=20,
                  dk=0.1, kmin=-1.0, kmax=15.0, ksamples=30, **kwargs):
         FourierSpaceCorrelation.__init__(self, trajectory, kgrid, norigins,
                                          nk, dk, kmin, kmax, ksamples, **kwargs)
         self._is_cell_variable = None
 
@@ -170,20 +170,20 @@
     It uses a fortran 90 extension.
     """
 
     nbodies = 2
     symbol = 'sk'
     short_name = 'S(k)'
     long_name = 'structure factor'
-    phasespace = ['pos']
+    variables = ['pos']
 
     def _compute(self):
         from atooms.trajectory.utils import is_cell_variable
         try:
-            from atooms.postprocessing.fourierspace_wrap import fourierspace_module
+            from atooms.postprocessing.core import f90
         except ImportError:
             _log.error('f90 wrapper missing or not functioning')
             raise
 
         nsteps = len(self._pos_0)
         kgrid = self.kgrid
         assert self._weight is None, 'StructureFactorFast does not handle weights'
@@ -213,21 +213,21 @@
                 # TODO: do it by transpose()
                 # Fill array of kvectors in this bin                
                 ikvec = numpy.ndarray((3, len(klist)), order='F', dtype=numpy.int32)
                 for i, kvec in enumerate(klist):
                     ikvec[:, i] = kvec
                 if self._pos_0[i] is self._pos_1[i]:
                     rho_0 = numpy.zeros(len(klist), dtype=numpy.complex128)
-                    fourierspace_module.sk_bare(expo_0, ikvec, rho_0)
+                    f90.fourierspace.sk_bare(expo_0, ikvec, rho_0)
                     rho_1 = rho_0
                 else:
                     rho_0 = numpy.zeros(len(klist), dtype=numpy.complex128)
                     rho_1 = numpy.zeros(len(klist), dtype=numpy.complex128)
-                    fourierspace_module.sk_bare(expo_0, ikvec, rho_0)
-                    fourierspace_module.sk_bare(expo_1, ikvec, rho_1)
+                    f90.fourierspace.sk_bare(expo_0, ikvec, rho_0)
+                    f90.fourierspace.sk_bare(expo_1, ikvec, rho_1)
                 rho2_av[k] += numpy.sum(rho_0 * rho_1.conjugate())
                 cnt[k] += rho_0.shape[0]
 
         # Normalization.
         npart_0 = sum([p.shape[0] for p in self._pos_0]) / float(len(self._pos_0))
         npart_1 = sum([p.shape[0] for p in self._pos_1]) / float(len(self._pos_1))
         self.grid = kgrid
```

### Comparing `atooms-pp-3.4.0/atooms/postprocessing/vacf.py` & `atooms_pp-4.0.0/atooms/postprocessing/vacf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of atooms
-# Copyright 2010-2018, Daniele Coslovich
+# Copyright 2010-2024, Daniele Coslovich
 
 """Velocity autocorrelation function."""
 
 import numpy
 
 from .correlation import Correlation, gcf_offset
 from .helpers import setup_t_grid, linear_grid
@@ -13,16 +13,16 @@
 
 class VelocityAutocorrelation(Correlation):
 
     """Velocity autocorrelation function."""
 
     symbol = 'vacf'
     short_name = 'Z(t)'
-    long_name = 'velocity autocorrelation'
-    phasespace = ['vel']
+    long_name = 'velocity autocorrelation function'
+    variables = ['vel']
 
     def __init__(self, trajectory, tgrid=None, tsamples=30, norigins=None, **kwargs):
         Correlation.__init__(self, trajectory, tgrid, norigins=norigins, **kwargs)
         if self.grid is None:
             self.grid = linear_grid(0.0, trajectory.total_time * 0.10, tsamples)
         self._discrete_tgrid = setup_t_grid(self.trajectory, tgrid, offset=norigins != '1')
```

### Comparing `atooms-pp-3.4.0/atooms_pp.egg-info/PKG-INFO` & `atooms_pp-4.0.0/atooms_pp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.4.0
+Version: 4.0.0
 Summary: Post-processing tools for particle simulations
-Home-page: https://framagit.org/atooms/postprocessing
-Author: Daniele Coslovich
-Author-email: daniele.coslovich@umontpellier.fr
+Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
-Platform: UNKNOWN
+Project-URL: repository, https://framagit.org/atooms/postprocessing
+Project-URL: homepage, https://framagit.org/atooms/postprocessing
+Project-URL: documentation, https://atooms.frama.io/postprocessing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: atooms>=2
+Requires-Dist: numpy
+Requires-Dist: argh
+Requires-Dist: tqdm
+Requires-Dist: f2py_jit
 
 # Postprocessing
 
 [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
@@ -109,9 +111,7 @@
 ## Contributing
 
 Contributions to the project are welcome. If you wish to contribute, check out [these guidelines](https://framagit.org/atooms/atooms/-/blob/master/CONTRIBUTING.md).
 
 ## Authors
 
 Daniele Coslovich: https://www.units.it/daniele.coslovich/
-
-
```

### Comparing `atooms-pp-3.4.0/atooms_pp.egg-info/SOURCES.txt` & `atooms_pp-4.0.0/atooms_pp.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
-setup.py
-atooms/__init__.py
 atooms/postprocessing/__init__.py
-atooms/postprocessing/_commit.py
 atooms/postprocessing/_version.py
 atooms/postprocessing/alpha2.py
 atooms/postprocessing/api.py
 atooms/postprocessing/ba.py
 atooms/postprocessing/chi4t.py
+atooms/postprocessing/cli.py
 atooms/postprocessing/core.py
 atooms/postprocessing/correlation.py
 atooms/postprocessing/filter.py
 atooms/postprocessing/fkt.py
-atooms/postprocessing/fourierspace.f90
 atooms/postprocessing/fourierspace.py
 atooms/postprocessing/gr.py
 atooms/postprocessing/helpers.py
 atooms/postprocessing/ik.py
 atooms/postprocessing/linkedcells.py
 atooms/postprocessing/msd.py
 atooms/postprocessing/partial.py
 atooms/postprocessing/progress.py
 atooms/postprocessing/qt.py
-atooms/postprocessing/realspace.f90
 atooms/postprocessing/s4kt.py
 atooms/postprocessing/sacf.py
 atooms/postprocessing/sk.py
 atooms/postprocessing/susceptibility.py
 atooms/postprocessing/vacf.py
 atooms_pp.egg-info/PKG-INFO
 atooms_pp.egg-info/SOURCES.txt
 atooms_pp.egg-info/dependency_links.txt
 atooms_pp.egg-info/requires.txt
 atooms_pp.egg-info/top_level.txt
-bin/acf.py
-bin/pp.py
+bin/pp.py
+tests/test_api.py
+tests/test_helpers.py
+tests/test_ll.py
+tests/test_pp.py
```

### Comparing `atooms-pp-3.4.0/bin/pp.py` & `atooms_pp-4.0.0/bin/pp.py`

 * *Files identical despite different names*

