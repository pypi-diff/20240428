# Comparing `tmp/param_sweeps-0.1.7a4.tar.gz` & `tmp/param_sweeps-0.1.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "param_sweeps-0.1.7a4.tar", max compression
+gzip compressed data, was "param_sweeps-0.1.7rc1.tar", max compression
```

## Comparing `param_sweeps-0.1.7a4.tar` & `param_sweeps-0.1.7rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2022-10-12 15:56:34.681986 param_sweeps-0.1.7a4/LICENSE
--rw-r--r--   0        0        0      270 2024-04-23 17:22:53.644053 param_sweeps-0.1.7a4/param_sweeps/__init__.py
--rw-r--r--   0        0        0      572 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a4/param_sweeps/constants.py
--rw-r--r--   0        0        0     8151 2024-04-23 17:22:24.134054 param_sweeps-0.1.7a4/param_sweeps/driver.py
--rw-r--r--   0        0        0     3230 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a4/param_sweeps/generate.py
--rw-r--r--   0        0        0      967 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a4/param_sweeps/sample_driver.py
--rw-r--r--   0        0        0     1598 2024-04-23 17:22:53.644053 param_sweeps-0.1.7a4/pyproject.toml
--rw-r--r--   0        0        0     1153 2022-11-10 19:09:10.043391 param_sweeps-0.1.7a4/README.md
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 param_sweeps-0.1.7a4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-28 20:40:55.138491 param_sweeps-0.1.7rc1/LICENSE
+-rw-r--r--   0        0        0      267 2024-04-28 20:46:48.524927 param_sweeps-0.1.7rc1/param_sweeps/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-23 21:33:39.731115 param_sweeps-0.1.7rc1/param_sweeps/constants.py
+-rw-r--r--   0        0        0     8151 2024-04-23 21:33:39.731115 param_sweeps-0.1.7rc1/param_sweeps/driver.py
+-rw-r--r--   0        0        0     3230 2024-04-23 21:33:39.732216 param_sweeps-0.1.7rc1/param_sweeps/generate.py
+-rw-r--r--   0        0        0      967 2024-04-23 21:33:39.732216 param_sweeps-0.1.7rc1/param_sweeps/sample_driver.py
+-rw-r--r--   0        0        0     2683 2024-04-28 20:46:48.519489 param_sweeps-0.1.7rc1/pyproject.toml
+-rw-r--r--   0        0        0     1153 2024-04-23 21:33:39.730041 param_sweeps-0.1.7rc1/README.md
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 param_sweeps-0.1.7rc1/PKG-INFO
```

### Comparing `param_sweeps-0.1.7a4/LICENSE` & `param_sweeps-0.1.7rc1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Mira Geoscience
+Copyright (c) 2024 Mira Geoscience
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `param_sweeps-0.1.7a4/param_sweeps/constants.py` & `param_sweeps-0.1.7rc1/param_sweeps/constants.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a4/param_sweeps/driver.py` & `param_sweeps-0.1.7rc1/param_sweeps/driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a4/param_sweeps/generate.py` & `param_sweeps-0.1.7rc1/param_sweeps/generate.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a4/param_sweeps/sample_driver.py` & `param_sweeps-0.1.7rc1/param_sweeps/sample_driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a4/README.md` & `param_sweeps-0.1.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a4/PKG-INFO` & `param_sweeps-0.1.7rc1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: param-sweeps
-Version: 0.1.7a4
+Version: 0.1.7rc1
 Summary: Parameter sweeper for ui.json powered applications
-Home-page: https://mirageoscience.com
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
+License: MIT
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
-Author-email: benjamink@mirageoscience.com
+Author-email: support@mirageoscience.com
+Maintainer: Benjamin Kary
+Maintainer-email: benjamink@mirageoscience.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -18,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: geoh5py (>=0.9.0-alpha.4,<0.10.0)
+Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Project-URL: Repository, https://github.com/MiraGeoscience/param-sweeps
 Description-Content-Type: text/markdown
 
 # Param-sweeps
 
 A Parameter sweeper for applications driven by ui.json files
```

