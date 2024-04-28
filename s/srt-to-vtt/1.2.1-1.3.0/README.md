# Comparing `tmp/srt_to_vtt-1.2.1.tar.gz` & `tmp/srt_to_vtt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_to_vtt-1.2.1.tar", last modified: Sat Apr 27 22:24:41 2024, max compression
+gzip compressed data, was "srt_to_vtt-1.3.0.tar", last modified: Sat Apr 27 22:48:19 2024, max compression
```

## Comparing `srt_to_vtt-1.2.1.tar` & `srt_to_vtt-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/srt_to_vtt/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/srt_to_vtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/srt_to_vtt/srt_to_vtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/tests/test_srt_to_vtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:48:19.687609 srt_to_vtt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-27 22:48:19.687609 srt_to_vtt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:48:19.687609 srt_to_vtt-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:48:19.687609 srt_to_vtt-1.3.0/srt_to_vtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/srt_to_vtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/srt_to_vtt/srt_to_vtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:48:19.687609 srt_to_vtt-1.3.0/srt_to_vtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-27 22:48:19.000000 srt_to_vtt-1.3.0/srt_to_vtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 22:48:19.000000 srt_to_vtt-1.3.0/srt_to_vtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:48:19.000000 srt_to_vtt-1.3.0/srt_to_vtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 22:48:19.000000 srt_to_vtt-1.3.0/srt_to_vtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:48:19.687609 srt_to_vtt-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-27 22:48:15.000000 srt_to_vtt-1.3.0/tests/test_srt_to_vtt.py
```

### Comparing `srt_to_vtt-1.2.1/LICENSE` & `srt_to_vtt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.2.1/PKG-INFO` & `srt_to_vtt-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-to-vtt
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python package to enable easy conversion of .srt files to .vtt files.
 Author-email: Joshua Hamilton <hamiltonjoshuadavid@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Joshua Hamilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -99,18 +99,10 @@
 pip install dist/srt_to_vtt-#.#.#-py3-none-any.whl
 ```
 
 You may now run any of the tests found in the `tests/` directory.
 
 ### Distribute
 
-Assuming that all the tests are passing, the package is now ready to be released on PyPI.
+Assuming that all the tests are passing, the package is now ready to be released on PyPI!
 
-First, ensure that the files to be uploaded are correct with
-```
-twine check dist/*
-```
-
-Then upload to PyPI with
-```
-twine upload dist/*
-```
+Open a pull request on the main branch and, if approved and merged, the package will be automatically updated on PyPI after the next Release is published on GitHub.
```

### Comparing `srt_to_vtt-1.2.1/README.md` & `srt_to_vtt-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -64,18 +64,10 @@
 pip install dist/srt_to_vtt-#.#.#-py3-none-any.whl
 ```
 
 You may now run any of the tests found in the `tests/` directory.
 
 ### Distribute
 
-Assuming that all the tests are passing, the package is now ready to be released on PyPI.
+Assuming that all the tests are passing, the package is now ready to be released on PyPI!
 
-First, ensure that the files to be uploaded are correct with
-```
-twine check dist/*
-```
-
-Then upload to PyPI with
-```
-twine upload dist/*
-```
+Open a pull request on the main branch and, if approved and merged, the package will be automatically updated on PyPI after the next Release is published on GitHub.
```

### Comparing `srt_to_vtt-1.2.1/pyproject.toml` & `srt_to_vtt-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "srt-to-vtt"
-version = "1.2.1"
+version = "1.3.0"
 description = "Python package to enable easy conversion of .srt files to .vtt files."
 readme = "README.md"
 authors = [{ name = "Joshua Hamilton", email = "hamiltonjoshuadavid@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `srt_to_vtt-1.2.1/srt_to_vtt/srt_to_vtt.py` & `srt_to_vtt-1.3.0/srt_to_vtt/srt_to_vtt.py`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.2.1/srt_to_vtt.egg-info/PKG-INFO` & `srt_to_vtt-1.3.0/srt_to_vtt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-to-vtt
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python package to enable easy conversion of .srt files to .vtt files.
 Author-email: Joshua Hamilton <hamiltonjoshuadavid@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Joshua Hamilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -99,18 +99,10 @@
 pip install dist/srt_to_vtt-#.#.#-py3-none-any.whl
 ```
 
 You may now run any of the tests found in the `tests/` directory.
 
 ### Distribute
 
-Assuming that all the tests are passing, the package is now ready to be released on PyPI.
+Assuming that all the tests are passing, the package is now ready to be released on PyPI!
 
-First, ensure that the files to be uploaded are correct with
-```
-twine check dist/*
-```
-
-Then upload to PyPI with
-```
-twine upload dist/*
-```
+Open a pull request on the main branch and, if approved and merged, the package will be automatically updated on PyPI after the next Release is published on GitHub.
```

### Comparing `srt_to_vtt-1.2.1/tests/test_srt_to_vtt.py` & `srt_to_vtt-1.3.0/tests/test_srt_to_vtt.py`

 * *Files identical despite different names*

