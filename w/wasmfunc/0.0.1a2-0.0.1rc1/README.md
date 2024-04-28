# Comparing `tmp/wasmfunc-0.0.1a2.tar.gz` & `tmp/wasmfunc-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmfunc-0.0.1a2.tar", last modified: Thu Apr 25 19:12:48 2024, max compression
+gzip compressed data, was "wasmfunc-0.0.1rc1.tar", last modified: Fri Apr 26 13:38:27 2024, max compression
```

## Comparing `wasmfunc-0.0.1a2.tar` & `wasmfunc-0.0.1rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-25 19:12:48.423829 wasmfunc-0.0.1a2/
--rw-r--r--   0 jonathanharg   (501) staff       (20)    11356 2024-03-07 11:02:41.000000 wasmfunc-0.0.1a2/LICENSE
--rw-r--r--   0 jonathanharg   (501) staff       (20)       29 2024-04-25 11:13:04.000000 wasmfunc-0.0.1a2/MANIFEST.in
--rw-r--r--   0 jonathanharg   (501) staff       (20)    14651 2024-04-25 19:12:48.423545 wasmfunc-0.0.1a2/PKG-INFO
--rw-r--r--   0 jonathanharg   (501) staff       (20)      541 2024-04-25 11:43:21.000000 wasmfunc-0.0.1a2/README.md
--rw-r--r--   0 jonathanharg   (501) staff       (20)     1243 2024-04-25 19:12:43.000000 wasmfunc-0.0.1a2/pyproject.toml
--rw-r--r--   0 jonathanharg   (501) staff       (20)       38 2024-04-25 19:12:48.423873 wasmfunc-0.0.1a2/setup.cfg
-drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-25 19:12:48.419698 wasmfunc-0.0.1a2/tests/
--rw-r--r--   0 jonathanharg   (501) staff       (20)     1668 2024-04-25 10:52:41.000000 wasmfunc-0.0.1a2/tests/test_runner.py
-drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-25 19:12:48.421823 wasmfunc-0.0.1a2/wasmfunc/
--rw-r--r--   0 jonathanharg   (501) staff       (20)       47 2023-08-22 20:28:58.000000 wasmfunc-0.0.1a2/wasmfunc/__init__.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)     2761 2024-04-25 17:31:08.000000 wasmfunc-0.0.1a2/wasmfunc/__main__.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)    42098 2024-04-25 19:11:27.000000 wasmfunc-0.0.1a2/wasmfunc/compiler.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)     1358 2024-04-25 12:03:21.000000 wasmfunc-0.0.1a2/wasmfunc/decorators.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)     3615 2024-04-25 15:20:21.000000 wasmfunc-0.0.1a2/wasmfunc/file_handler.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)     5565 2024-04-25 10:24:06.000000 wasmfunc-0.0.1a2/wasmfunc/mini_std.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)     4726 2024-04-25 12:03:40.000000 wasmfunc-0.0.1a2/wasmfunc/pre_compiler.py
--rw-r--r--   0 jonathanharg   (501) staff       (20)      736 2024-04-25 15:25:35.000000 wasmfunc-0.0.1a2/wasmfunc/runWasmGC.js
--rw-r--r--   0 jonathanharg   (501) staff       (20)     1940 2024-04-25 10:50:02.000000 wasmfunc-0.0.1a2/wasmfunc/types.py
-drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-25 19:12:48.423018 wasmfunc-0.0.1a2/wasmfunc.egg-info/
--rw-r--r--   0 jonathanharg   (501) staff       (20)    14651 2024-04-25 19:12:48.000000 wasmfunc-0.0.1a2/wasmfunc.egg-info/PKG-INFO
--rw-r--r--   0 jonathanharg   (501) staff       (20)      456 2024-04-25 19:12:48.000000 wasmfunc-0.0.1a2/wasmfunc.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanharg   (501) staff       (20)        1 2024-04-25 19:12:48.000000 wasmfunc-0.0.1a2/wasmfunc.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanharg   (501) staff       (20)       52 2024-04-25 19:12:48.000000 wasmfunc-0.0.1a2/wasmfunc.egg-info/entry_points.txt
--rw-r--r--   0 jonathanharg   (501) staff       (20)       62 2024-04-25 19:12:48.000000 wasmfunc-0.0.1a2/wasmfunc.egg-info/requires.txt
--rw-r--r--   0 jonathanharg   (501) staff       (20)        9 2024-04-25 19:12:48.000000 wasmfunc-0.0.1a2/wasmfunc.egg-info/top_level.txt
+drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-26 13:38:27.086712 wasmfunc-0.0.1rc1/
+-rw-r--r--   0 jonathanharg   (501) staff       (20)    11356 2024-03-07 11:02:41.000000 wasmfunc-0.0.1rc1/LICENSE
+-rw-r--r--   0 jonathanharg   (501) staff       (20)       29 2024-04-25 11:13:04.000000 wasmfunc-0.0.1rc1/MANIFEST.in
+-rw-r--r--   0 jonathanharg   (501) staff       (20)    14652 2024-04-26 13:38:27.086454 wasmfunc-0.0.1rc1/PKG-INFO
+-rw-r--r--   0 jonathanharg   (501) staff       (20)      541 2024-04-25 11:43:21.000000 wasmfunc-0.0.1rc1/README.md
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     1244 2024-04-26 12:13:46.000000 wasmfunc-0.0.1rc1/pyproject.toml
+-rw-r--r--   0 jonathanharg   (501) staff       (20)       38 2024-04-26 13:38:27.086768 wasmfunc-0.0.1rc1/setup.cfg
+drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-26 13:38:27.081686 wasmfunc-0.0.1rc1/tests/
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     1668 2024-04-25 10:52:41.000000 wasmfunc-0.0.1rc1/tests/test_runner.py
+drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-26 13:38:27.084680 wasmfunc-0.0.1rc1/wasmfunc/
+-rw-r--r--   0 jonathanharg   (501) staff       (20)       47 2023-08-22 20:28:58.000000 wasmfunc-0.0.1rc1/wasmfunc/__init__.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     2761 2024-04-25 17:31:08.000000 wasmfunc-0.0.1rc1/wasmfunc/__main__.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)    42098 2024-04-25 19:11:27.000000 wasmfunc-0.0.1rc1/wasmfunc/compiler.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     1358 2024-04-25 12:03:21.000000 wasmfunc-0.0.1rc1/wasmfunc/decorators.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     3615 2024-04-25 15:20:21.000000 wasmfunc-0.0.1rc1/wasmfunc/file_handler.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     5565 2024-04-25 10:24:06.000000 wasmfunc-0.0.1rc1/wasmfunc/mini_std.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     4726 2024-04-25 12:03:40.000000 wasmfunc-0.0.1rc1/wasmfunc/pre_compiler.py
+-rw-r--r--   0 jonathanharg   (501) staff       (20)      736 2024-04-25 15:25:35.000000 wasmfunc-0.0.1rc1/wasmfunc/runWasmGC.js
+-rw-r--r--   0 jonathanharg   (501) staff       (20)     1940 2024-04-25 10:50:02.000000 wasmfunc-0.0.1rc1/wasmfunc/types.py
+drwxr-xr-x   0 jonathanharg   (501) staff       (20)        0 2024-04-26 13:38:27.085927 wasmfunc-0.0.1rc1/wasmfunc.egg-info/
+-rw-r--r--   0 jonathanharg   (501) staff       (20)    14652 2024-04-26 13:38:27.000000 wasmfunc-0.0.1rc1/wasmfunc.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanharg   (501) staff       (20)      456 2024-04-26 13:38:27.000000 wasmfunc-0.0.1rc1/wasmfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanharg   (501) staff       (20)        1 2024-04-26 13:38:27.000000 wasmfunc-0.0.1rc1/wasmfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanharg   (501) staff       (20)       52 2024-04-26 13:38:27.000000 wasmfunc-0.0.1rc1/wasmfunc.egg-info/entry_points.txt
+-rw-r--r--   0 jonathanharg   (501) staff       (20)       62 2024-04-26 13:38:27.000000 wasmfunc-0.0.1rc1/wasmfunc.egg-info/requires.txt
+-rw-r--r--   0 jonathanharg   (501) staff       (20)        9 2024-04-26 13:38:27.000000 wasmfunc-0.0.1rc1/wasmfunc.egg-info/top_level.txt
```

### Comparing `wasmfunc-0.0.1a2/LICENSE` & `wasmfunc-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/PKG-INFO` & `wasmfunc-0.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmfunc
-Version: 0.0.1a2
+Version: 0.0.1rc1
 Summary: A WebAssembly compiler for Python
 Author-email: Jonathan Hargreaves <jhargreaves189@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `wasmfunc-0.0.1a2/README.md` & `wasmfunc-0.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/pyproject.toml` & `wasmfunc-0.0.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "wasmfunc"
-version = "0.0.1a2"
+version = "0.0.1rc1"
 description = "A WebAssembly compiler for Python"
 authors = [
     {name = "Jonathan Hargreaves", email = "jhargreaves189@gmail.com"},
 ]
 readme = "README.md"
 keywords = ["WebAssembly", "Compiler"]
 classifiers = [
```

### Comparing `wasmfunc-0.0.1a2/tests/test_runner.py` & `wasmfunc-0.0.1rc1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/__main__.py` & `wasmfunc-0.0.1rc1/wasmfunc/__main__.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/compiler.py` & `wasmfunc-0.0.1rc1/wasmfunc/compiler.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/decorators.py` & `wasmfunc-0.0.1rc1/wasmfunc/decorators.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/file_handler.py` & `wasmfunc-0.0.1rc1/wasmfunc/file_handler.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/mini_std.py` & `wasmfunc-0.0.1rc1/wasmfunc/mini_std.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/pre_compiler.py` & `wasmfunc-0.0.1rc1/wasmfunc/pre_compiler.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/runWasmGC.js` & `wasmfunc-0.0.1rc1/wasmfunc/runWasmGC.js`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc/types.py` & `wasmfunc-0.0.1rc1/wasmfunc/types.py`

 * *Files identical despite different names*

### Comparing `wasmfunc-0.0.1a2/wasmfunc.egg-info/PKG-INFO` & `wasmfunc-0.0.1rc1/wasmfunc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmfunc
-Version: 0.0.1a2
+Version: 0.0.1rc1
 Summary: A WebAssembly compiler for Python
 Author-email: Jonathan Hargreaves <jhargreaves189@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

