# Comparing `tmp/fastbench-0.1.3.tar.gz` & `tmp/fastbench-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastbench-0.1.3.tar", max compression
+gzip compressed data, was "fastbench-0.1.4.tar", max compression
```

## Comparing `fastbench-0.1.3.tar` & `fastbench-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1078 2024-04-27 12:02:57.894533 fastbench-0.1.3/LICENSE
--rw-r--r--   0        0        0     1885 2024-04-27 12:02:57.894533 fastbench-0.1.3/README.md
--rw-r--r--   0        0        0      670 2024-04-27 12:02:57.894533 fastbench-0.1.3/fastbench/__init__.py
--rw-r--r--   0        0        0      516 2024-04-27 12:02:57.894533 fastbench-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2228 1970-01-01 00:00:00.000000 fastbench-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-28 04:08:12.082123 fastbench-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1900 2024-04-28 04:08:12.082123 fastbench-0.1.4/README.md
+-rw-r--r--   0        0        0      670 2024-04-28 04:08:12.082123 fastbench-0.1.4/fastbench/__init__.py
+-rw-r--r--   0        0        0     1231 2024-04-28 04:08:12.082123 fastbench-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 fastbench-0.1.4/PKG-INFO
```

### Comparing `fastbench-0.1.3/LICENSE` & `fastbench-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastbench-0.1.3/README.md` & `fastbench-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,19 +9,19 @@
   <br>
 </h1>
 
 FastBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
 
 ## ✨ Features
 
-- ️ Measure the execution time of a function or code block
-- ️ Track CPU usage during code execution
--  Monitor memory usage during code execution
+- ⏱️ Measure the execution time of a function or code block
+- 📊 Track CPU usage during code execution
+- 🖥️ Monitor memory usage during code execution
 - ⚡ Lightweight and fast
--  Simple and easy-to-use API
+- 🔄 Simple and easy-to-use API
 
 ##  Installation
 
 You can install FastBench via pip:
 
 ```bash
 pip install fastbench
```

### Comparing `fastbench-0.1.3/fastbench/__init__.py` & `fastbench-0.1.4/fastbench/__init__.py`

 * *Files identical despite different names*

### Comparing `fastbench-0.1.3/PKG-INFO` & `fastbench-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: fastbench
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pure-python based benchmarking package for Python 🤪
 Author: Adarsh Gourab Mahalik
 Author-email: gourabmahalikadarsh@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
   <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/fastbench.svg" width="200" height="200">
@@ -21,19 +25,19 @@
   <br>
 </h1>
 
 FastBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
 
 ## ✨ Features
 
-- ️ Measure the execution time of a function or code block
-- ️ Track CPU usage during code execution
--  Monitor memory usage during code execution
+- ⏱️ Measure the execution time of a function or code block
+- 📊 Track CPU usage during code execution
+- 🖥️ Monitor memory usage during code execution
 - ⚡ Lightweight and fast
--  Simple and easy-to-use API
+- 🔄 Simple and easy-to-use API
 
 ##  Installation
 
 You can install FastBench via pip:
 
 ```bash
 pip install fastbench
```

