# Comparing `tmp/srt_to_vtt-1.1.0.tar.gz` & `tmp/srt_to_vtt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_to_vtt-1.1.0.tar", last modified: Fri Apr 26 19:15:41 2024, max compression
+gzip compressed data, was "srt_to_vtt-1.2.0.tar", last modified: Sat Apr 27 18:39:49 2024, max compression
```

## Comparing `srt_to_vtt-1.1.0.tar` & `srt_to_vtt-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.706467 srt_to_vtt-1.1.0/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-1.1.0/LICENSE
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     3272 2024-04-26 19:15:41.706238 srt_to_vtt-1.1.0/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     1487 2024-04-26 19:14:04.000000 srt_to_vtt-1.1.0/README.md
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      693 2024-04-26 19:14:21.000000 srt_to_vtt-1.1.0/pyproject.toml
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-26 19:15:41.707425 srt_to_vtt-1.1.0/setup.cfg
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       37 2024-04-26 17:25:00.000000 srt_to_vtt-1.1.0/setup.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.705107 srt_to_vtt-1.1.0/srt_to_vtt/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       34 2024-04-25 19:50:08.000000 srt_to_vtt-1.1.0/srt_to_vtt/__init__.py
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      673 2024-04-26 18:07:21.000000 srt_to_vtt-1.1.0/srt_to_vtt/srt_to_vtt.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.705996 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     3272 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      250 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/SOURCES.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/dependency_links.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/top_level.txt
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.705634 srt_to_vtt-1.1.0/tests/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      653 2024-04-25 20:59:42.000000 srt_to_vtt-1.1.0/tests/test_srt_to_vtt.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.596848 srt_to_vtt-1.2.0/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-1.2.0/LICENSE
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     3713 2024-04-27 18:39:49.596647 srt_to_vtt-1.2.0/PKG-INFO
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     1928 2024-04-27 18:35:35.000000 srt_to_vtt-1.2.0/README.md
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      693 2024-04-27 18:38:59.000000 srt_to_vtt-1.2.0/pyproject.toml
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-27 18:39:49.596882 srt_to_vtt-1.2.0/setup.cfg
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-27 18:09:52.000000 srt_to_vtt-1.2.0/setup.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.595766 srt_to_vtt-1.2.0/srt_to_vtt/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       35 2024-04-27 18:09:52.000000 srt_to_vtt-1.2.0/srt_to_vtt/__init__.py
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      673 2024-04-27 18:09:52.000000 srt_to_vtt-1.2.0/srt_to_vtt/srt_to_vtt.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.596449 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     3713 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/PKG-INFO
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      250 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/top_level.txt
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.596288 srt_to_vtt-1.2.0/tests/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      652 2024-04-27 18:14:05.000000 srt_to_vtt-1.2.0/tests/test_srt_to_vtt.py
```

### Comparing `srt_to_vtt-1.1.0/LICENSE` & `srt_to_vtt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.1.0/PKG-INFO` & `srt_to_vtt-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-to-vtt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python package to enable easy conversion of .srt files to .vtt files.
 Author-email: Joshua Hamilton <hamiltonjoshuadavid@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Joshua Hamilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,56 +29,67 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPi](https://img.shields.io/pypi/v/srt-to-vtt)](https://pypi.org/project/srt-to-vtt/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # srt-to-vtt
 
 Python package to enable easy conversion of .srt files to .vtt files.
 
 ## Install
 
-srt-to-vtt is available at https://pypi.org/project/srt-to-vtt/ and you can install the latest version with
+srt-to-vtt is available on [PyPI](https://pypi.org/project/srt-to-vtt/) and you can install the latest version with
 ```
 pip install srt-to-vtt
 ```
 
 ## Basic usage
 
 ```python
 from srt_to_vtt import srt_to_vtt
 
 path_to_my_srt_file = "example.srt"
 path_to_converted_vtt_file = "output.vtt"
 
-#converts example.srt into output.vtt
+# converts example.srt into output.vtt
 srt_to_vtt(path_to_my_srt_file, path_to_converted_vtt_file)
+
 ```
 
 ## Develop
 
 Clone this repo and then, at the root, install the package in ediable mode with
 ```
 pip install -e .
 ```
 You can now make changes to the package source code found in `srt-to-vtt/srt_to_vtt/` and see them reflected immediately.
 
-## Build, test and distribute
+## Format, build, test and distribute
 
 Before doing anything else, make sure to bump the version number under `[project]` in `pyproject.toml`. Please use [semantic versioning](https://semver.org/).
 
 
-### Build
-First, install the build requirements with
+
+Then, install the build requirements with
 ```
 pip install -r build_requirements.txt
 ```
 
+### Format
+
+This project adheres to the [Black](https://github.com/psf/black) code style. You can automatically refomat your code to Black by executing the following in the root directory of this repo:
+```
+black .
+```
+
+### Build
 Then, to build, run
 ```
 python -m build
 ```
 
 ### Test
```

### Comparing `srt_to_vtt-1.1.0/README.md` & `srt_to_vtt-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,60 @@
+[![PyPi](https://img.shields.io/pypi/v/srt-to-vtt)](https://pypi.org/project/srt-to-vtt/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # srt-to-vtt
 
 Python package to enable easy conversion of .srt files to .vtt files.
 
 ## Install
 
-srt-to-vtt is available at https://pypi.org/project/srt-to-vtt/ and you can install the latest version with
+srt-to-vtt is available on [PyPI](https://pypi.org/project/srt-to-vtt/) and you can install the latest version with
 ```
 pip install srt-to-vtt
 ```
 
 ## Basic usage
 
 ```python
 from srt_to_vtt import srt_to_vtt
 
 path_to_my_srt_file = "example.srt"
 path_to_converted_vtt_file = "output.vtt"
 
-#converts example.srt into output.vtt
+# converts example.srt into output.vtt
 srt_to_vtt(path_to_my_srt_file, path_to_converted_vtt_file)
+
 ```
 
 ## Develop
 
 Clone this repo and then, at the root, install the package in ediable mode with
 ```
 pip install -e .
 ```
 You can now make changes to the package source code found in `srt-to-vtt/srt_to_vtt/` and see them reflected immediately.
 
-## Build, test and distribute
+## Format, build, test and distribute
 
 Before doing anything else, make sure to bump the version number under `[project]` in `pyproject.toml`. Please use [semantic versioning](https://semver.org/).
 
 
-### Build
-First, install the build requirements with
+
+Then, install the build requirements with
 ```
 pip install -r build_requirements.txt
 ```
 
+### Format
+
+This project adheres to the [Black](https://github.com/psf/black) code style. You can automatically refomat your code to Black by executing the following in the root directory of this repo:
+```
+black .
+```
+
+### Build
 Then, to build, run
 ```
 python -m build
 ```
 
 ### Test
```

### Comparing `srt_to_vtt-1.1.0/pyproject.toml` & `srt_to_vtt-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "srt-to-vtt"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python package to enable easy conversion of .srt files to .vtt files."
 readme = "README.md"
 authors = [{ name = "Joshua Hamilton", email = "hamiltonjoshuadavid@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `srt_to_vtt-1.1.0/srt_to_vtt/srt_to_vtt.py` & `srt_to_vtt-1.2.0/srt_to_vtt/srt_to_vtt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 def srt_to_vtt(srt_file_path, vtt_file_path):
 
-    with open(srt_file_path, 'r') as srt_file:
+    with open(srt_file_path, "r") as srt_file:
         lines = srt_file.readlines()
 
-    with open(vtt_file_path, 'w') as vtt_file:
+    with open(vtt_file_path, "w") as vtt_file:
 
-        #Required WEBVTT header and blank line for .vtt files
-        vtt_file.write('WEBVTT\n\n')
+        # Required WEBVTT header and blank line for .vtt files
+        vtt_file.write("WEBVTT\n\n")
 
         for line in lines:
 
-            #Remove caption numbers as they're no longer
-            #needed in .vtt files
+            # Remove caption numbers as they're no longer
+            # needed in .vtt files
             if line.strip().isdigit():
                 continue
 
-            #.vtt timestamps use commas, rather than
-            #periods in their timestamps
-            if '-->' in line:
-                line = line.replace(',', '.')
+            # .vtt timestamps use commas, rather than
+            # periods in their timestamps
+            if "-->" in line:
+                line = line.replace(",", ".")
 
             vtt_file.write(line)
-
-
```

### Comparing `srt_to_vtt-1.1.0/srt_to_vtt.egg-info/PKG-INFO` & `srt_to_vtt-1.2.0/srt_to_vtt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-to-vtt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python package to enable easy conversion of .srt files to .vtt files.
 Author-email: Joshua Hamilton <hamiltonjoshuadavid@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Joshua Hamilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,56 +29,67 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPi](https://img.shields.io/pypi/v/srt-to-vtt)](https://pypi.org/project/srt-to-vtt/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # srt-to-vtt
 
 Python package to enable easy conversion of .srt files to .vtt files.
 
 ## Install
 
-srt-to-vtt is available at https://pypi.org/project/srt-to-vtt/ and you can install the latest version with
+srt-to-vtt is available on [PyPI](https://pypi.org/project/srt-to-vtt/) and you can install the latest version with
 ```
 pip install srt-to-vtt
 ```
 
 ## Basic usage
 
 ```python
 from srt_to_vtt import srt_to_vtt
 
 path_to_my_srt_file = "example.srt"
 path_to_converted_vtt_file = "output.vtt"
 
-#converts example.srt into output.vtt
+# converts example.srt into output.vtt
 srt_to_vtt(path_to_my_srt_file, path_to_converted_vtt_file)
+
 ```
 
 ## Develop
 
 Clone this repo and then, at the root, install the package in ediable mode with
 ```
 pip install -e .
 ```
 You can now make changes to the package source code found in `srt-to-vtt/srt_to_vtt/` and see them reflected immediately.
 
-## Build, test and distribute
+## Format, build, test and distribute
 
 Before doing anything else, make sure to bump the version number under `[project]` in `pyproject.toml`. Please use [semantic versioning](https://semver.org/).
 
 
-### Build
-First, install the build requirements with
+
+Then, install the build requirements with
 ```
 pip install -r build_requirements.txt
 ```
 
+### Format
+
+This project adheres to the [Black](https://github.com/psf/black) code style. You can automatically refomat your code to Black by executing the following in the root directory of this repo:
+```
+black .
+```
+
+### Build
 Then, to build, run
 ```
 python -m build
 ```
 
 ### Test
```

### Comparing `srt_to_vtt-1.1.0/tests/test_srt_to_vtt.py` & `srt_to_vtt-1.2.0/tests/test_srt_to_vtt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import srt_to_vtt
 
+
 def test_convert():
     """
     Takes test_input.srt, converts it to test_output.vtt using srt_to_vtt.srt_to_vtt
     and compares it with valid_output.vtt.
     """
 
-    srt_to_vtt.srt_to_vtt('test_input.srt', 'test_output.vtt')
+    srt_to_vtt.srt_to_vtt("test_input.srt", "test_output.vtt")
 
-    with open('test_output.vtt', 'r') as vtt_file:
+    with open("test_output.vtt", "r") as vtt_file:
         test_lines = vtt_file.readlines()
 
-    with open('valid_output.vtt', 'r') as vtt_file:
+    with open("valid_output.vtt", "r") as vtt_file:
         valid_lines = vtt_file.readlines()
 
     assert len(test_lines) == len(valid_lines)
 
     for i in range(len(test_lines)):
 
         test_line = test_lines[i]
         valid_line = valid_lines[i]
 
         assert test_line == valid_line
-    
-test_convert()
+
+
+test_convert()
```

