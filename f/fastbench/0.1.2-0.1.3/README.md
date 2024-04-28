# Comparing `tmp/fastbench-0.1.2.tar.gz` & `tmp/fastbench-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastbench-0.1.2.tar", max compression
+gzip compressed data, was "fastbench-0.1.3.tar", max compression
```

## Comparing `fastbench-0.1.2.tar` & `fastbench-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1078 2024-04-27 11:10:43.970360 fastbench-0.1.2/LICENSE
--rw-r--r--   0        0        0     1917 2024-04-27 11:10:43.970360 fastbench-0.1.2/README.md
--rw-r--r--   0        0        0      670 2024-04-27 11:10:43.974360 fastbench-0.1.2/fastbench/__init__.py
--rw-r--r--   0        0        0      516 2024-04-27 11:10:43.974360 fastbench-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 fastbench-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-27 12:02:57.894533 fastbench-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1885 2024-04-27 12:02:57.894533 fastbench-0.1.3/README.md
+-rw-r--r--   0        0        0      670 2024-04-27 12:02:57.894533 fastbench-0.1.3/fastbench/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-27 12:02:57.894533 fastbench-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2228 1970-01-01 00:00:00.000000 fastbench-0.1.3/PKG-INFO
```

### Comparing `fastbench-0.1.2/LICENSE` & `fastbench-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastbench-0.1.2/README.md` & `fastbench-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 <h1 align="center">
   <br>
-  <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/truebench.svg" width="200" height="200">
+  <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/fastbench.svg" width="200" height="200">
   <br>
-  TrueBench
+  FastBench
   <br>
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastbench">
   <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/itsmeadarsh2008/fastbench">
   <br>
 </h1>
 
-TrueBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
+FastBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
 
 ## ✨ Features
 
-- 🕰️ Measure the execution time of a function or code block
-- 🖥️ Track CPU usage during code execution
-- 💾 Monitor memory usage during code execution
+- ️ Measure the execution time of a function or code block
+- ️ Track CPU usage during code execution
+-  Monitor memory usage during code execution
 - ⚡ Lightweight and fast
-- 🤏 Simple and easy-to-use API
+-  Simple and easy-to-use API
 
-## 📦 Installation
+##  Installation
 
-You can install TrueBench via pip:
+You can install FastBench via pip:
 
 ```bash
-pip install truebench
+pip install fastbench
 ```
 
-## 🔧 Usage
+##  Usage
 
-Here's an example of how to use TrueBench to benchmark Python code:
+Here's an example of how to use FastBench to benchmark Python code:
 
 ```python
-from truebench import mt, mc, mm
+from fastbench import mt, mc, mm
 
 # Define a sample function for testing
 def sample_function(n):
-    return sum(range(n))
+  return sum(range(n))
 
 # Test the mt function (measure execution time)
 time_taken = mt(sample_function, n=1000000)
 print("Time taken:", time_taken)
 
 # Test the mc function (measure CPU usage)
 cpu_usage = mc(sample_function, n=1000000)
 print("CPU usage:", cpu_usage)
 
 # Test the mm function (measure memory usage)
 memory_usage = mm(sample_function, n=1000000)
 print("Memory usage:", memory_usage)
 ```
 
-## 🤝 Contributing
+##  Contributing
 
 Contributions are welcome! Check out the [Contribution Guidelines](https://github.com/itsmeadarsh2008/fastbench/blob/main/CONTRIBUTING.md).
 
-## 📄 License
+##  License
 
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/itsmeadarsh2008/fastbench?tab=MIT-1-ov-file) file for details.
```

### Comparing `fastbench-0.1.2/fastbench/__init__.py` & `fastbench-0.1.3/fastbench/__init__.py`

 * *Files identical despite different names*

### Comparing `fastbench-0.1.2/pyproject.toml` & `fastbench-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastbench"
-version = "0.1.2"
+version = "0.1.3"
 description = "A pure-python based benchmarking package for Python 🤪"
 authors = ["Adarsh Gourab Mahalik <gourabmahalikadarsh@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 psutil = "^5.9.8"
```

### Comparing `fastbench-0.1.2/PKG-INFO` & `fastbench-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 Metadata-Version: 2.1
 Name: fastbench
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pure-python based benchmarking package for Python 🤪
 Author: Adarsh Gourab Mahalik
 Author-email: gourabmahalikadarsh@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
-  <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/truebench.svg" width="200" height="200">
+  <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/fastbench.svg" width="200" height="200">
   <br>
-  TrueBench
+  FastBench
   <br>
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastbench">
   <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/itsmeadarsh2008/fastbench">
   <br>
 </h1>
 
-TrueBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
+FastBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
 
 ## ✨ Features
 
-- 🕰️ Measure the execution time of a function or code block
-- 🖥️ Track CPU usage during code execution
-- 💾 Monitor memory usage during code execution
+- ️ Measure the execution time of a function or code block
+- ️ Track CPU usage during code execution
+-  Monitor memory usage during code execution
 - ⚡ Lightweight and fast
-- 🤏 Simple and easy-to-use API
+-  Simple and easy-to-use API
 
-## 📦 Installation
+##  Installation
 
-You can install TrueBench via pip:
+You can install FastBench via pip:
 
 ```bash
-pip install truebench
+pip install fastbench
 ```
 
-## 🔧 Usage
+##  Usage
 
-Here's an example of how to use TrueBench to benchmark Python code:
+Here's an example of how to use FastBench to benchmark Python code:
 
 ```python
-from truebench import mt, mc, mm
+from fastbench import mt, mc, mm
 
 # Define a sample function for testing
 def sample_function(n):
-    return sum(range(n))
+  return sum(range(n))
 
 # Test the mt function (measure execution time)
 time_taken = mt(sample_function, n=1000000)
 print("Time taken:", time_taken)
 
 # Test the mc function (measure CPU usage)
 cpu_usage = mc(sample_function, n=1000000)
 print("CPU usage:", cpu_usage)
 
 # Test the mm function (measure memory usage)
 memory_usage = mm(sample_function, n=1000000)
 print("Memory usage:", memory_usage)
 ```
 
-## 🤝 Contributing
+##  Contributing
 
 Contributions are welcome! Check out the [Contribution Guidelines](https://github.com/itsmeadarsh2008/fastbench/blob/main/CONTRIBUTING.md).
 
-## 📄 License
+##  License
 
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/itsmeadarsh2008/fastbench?tab=MIT-1-ov-file) file for details.
```

