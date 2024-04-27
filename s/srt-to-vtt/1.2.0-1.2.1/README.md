# Comparing `tmp/srt_to_vtt-1.2.0.tar.gz` & `tmp/srt_to_vtt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_to_vtt-1.2.0.tar", last modified: Sat Apr 27 18:39:49 2024, max compression
+gzip compressed data, was "srt_to_vtt-1.2.1.tar", last modified: Sat Apr 27 22:24:41 2024, max compression
```

## Comparing `srt_to_vtt-1.2.0.tar` & `srt_to_vtt-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.596848 srt_to_vtt-1.2.0/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-1.2.0/LICENSE
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     3713 2024-04-27 18:39:49.596647 srt_to_vtt-1.2.0/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     1928 2024-04-27 18:35:35.000000 srt_to_vtt-1.2.0/README.md
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      693 2024-04-27 18:38:59.000000 srt_to_vtt-1.2.0/pyproject.toml
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-27 18:39:49.596882 srt_to_vtt-1.2.0/setup.cfg
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-27 18:09:52.000000 srt_to_vtt-1.2.0/setup.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.595766 srt_to_vtt-1.2.0/srt_to_vtt/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       35 2024-04-27 18:09:52.000000 srt_to_vtt-1.2.0/srt_to_vtt/__init__.py
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      673 2024-04-27 18:09:52.000000 srt_to_vtt-1.2.0/srt_to_vtt/srt_to_vtt.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.596449 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     3713 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      250 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/SOURCES.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/dependency_links.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-27 18:39:49.000000 srt_to_vtt-1.2.0/srt_to_vtt.egg-info/top_level.txt
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-27 18:39:49.596288 srt_to_vtt-1.2.0/tests/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      652 2024-04-27 18:14:05.000000 srt_to_vtt-1.2.0/tests/test_srt_to_vtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/srt_to_vtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/srt_to_vtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/srt_to_vtt/srt_to_vtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 22:24:41.000000 srt_to_vtt-1.2.1/srt_to_vtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:24:41.122329 srt_to_vtt-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-27 22:24:36.000000 srt_to_vtt-1.2.1/tests/test_srt_to_vtt.py
```

### Comparing `srt_to_vtt-1.2.0/LICENSE` & `srt_to_vtt-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.2.0/PKG-INFO` & `srt_to_vtt-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-to-vtt
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package to enable easy conversion of .srt files to .vtt files.
 Author-email: Joshua Hamilton <hamiltonjoshuadavid@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Joshua Hamilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `srt_to_vtt-1.2.0/README.md` & `srt_to_vtt-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.2.0/pyproject.toml` & `srt_to_vtt-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "srt-to-vtt"
-version = "1.2.0"
+version = "1.2.1"
 description = "Python package to enable easy conversion of .srt files to .vtt files."
 readme = "README.md"
 authors = [{ name = "Joshua Hamilton", email = "hamiltonjoshuadavid@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `srt_to_vtt-1.2.0/srt_to_vtt/srt_to_vtt.py` & `srt_to_vtt-1.2.1/srt_to_vtt/srt_to_vtt.py`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.2.0/srt_to_vtt.egg-info/PKG-INFO` & `srt_to_vtt-1.2.1/srt_to_vtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-to-vtt
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package to enable easy conversion of .srt files to .vtt files.
 Author-email: Joshua Hamilton <hamiltonjoshuadavid@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Joshua Hamilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `srt_to_vtt-1.2.0/tests/test_srt_to_vtt.py` & `srt_to_vtt-1.2.1/tests/test_srt_to_vtt.py`

 * *Files identical despite different names*

