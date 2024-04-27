# Comparing `tmp/pysparkify-0.24.1.tar.gz` & `tmp/pysparkify-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.24.1.tar", last modified: Sat Apr 27 22:08:25 2024, max compression
+gzip compressed data, was "pysparkify-0.25.0.tar", last modified: Sat Apr 27 22:13:47 2024, max compression
```

## Comparing `pysparkify-0.24.1.tar` & `pysparkify-0.25.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 22:08:25.980578 pysparkify-0.24.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-27 22:08:23.000000 pysparkify-0.24.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:08:25.980578 pysparkify-0.24.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-27 22:08:23.000000 pysparkify-0.24.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.976578 pysparkify-0.24.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/src/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/src/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/src/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 22:08:23.000000 pysparkify-0.24.1/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-27 22:13:47.976441 pysparkify-0.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-27 22:13:45.000000 pysparkify-0.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:13:47.976441 pysparkify-0.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-27 22:13:45.000000 pysparkify-0.25.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 22:13:45.000000 pysparkify-0.25.0/tests/test_app.py
```

### Comparing `pysparkify-0.24.1/PKG-INFO` & `pysparkify-0.25.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.24.1
+Version: 0.25.0
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -69,15 +69,15 @@
 ## How to Contribute
 
 1. Become a maintainer by requesting raohammad(at)gmail.com
 2. Open a PR
 3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
-# Pysparkify Library
+# Pysparkify Usage Example
 
 This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
 ```
 source:
   - type: CsvSource
     config:
@@ -106,7 +106,19 @@
       path: "output/output_data.csv"
   - type: CsvSink
     config:
       name: sink2
       path: "output/avgage_data.csv"
       
 ```
+
+The sample from csv source file used in above transformation is as below;
+
+```
+name,age,city
+Hayaan,10,Islamanad
+Jibraan,8,ShahAlam
+Allyan,3,Paris
+John,35,San Francisco
+Doe,22,Houston
+Dane,30,Seattle
+```
```

### Comparing `pysparkify-0.24.1/README.md` & `pysparkify-0.25.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ## How to Contribute
 
 1. Become a maintainer by requesting raohammad(at)gmail.com
 2. Open a PR
 3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
-# Pysparkify Library
+# Pysparkify Usage Example
 
 This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
 ```
 source:
   - type: CsvSource
     config:
@@ -88,8 +88,20 @@
       name: sink1
       path: "output/output_data.csv"
   - type: CsvSink
     config:
       name: sink2
       path: "output/avgage_data.csv"
       
+```
+
+The sample from csv source file used in above transformation is as below;
+
+```
+name,age,city
+Hayaan,10,Islamanad
+Jibraan,8,ShahAlam
+Allyan,3,Paris
+John,35,San Francisco
+Doe,22,Houston
+Dane,30,Seattle
 ```
```

### Comparing `pysparkify-0.24.1/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.25.0/pysparkify.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.24.1
+Version: 0.25.0
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -69,15 +69,15 @@
 ## How to Contribute
 
 1. Become a maintainer by requesting raohammad(at)gmail.com
 2. Open a PR
 3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
-# Pysparkify Library
+# Pysparkify Usage Example
 
 This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
 ```
 source:
   - type: CsvSource
     config:
@@ -106,7 +106,19 @@
       path: "output/output_data.csv"
   - type: CsvSink
     config:
       name: sink2
       path: "output/avgage_data.csv"
       
 ```
+
+The sample from csv source file used in above transformation is as below;
+
+```
+name,age,city
+Hayaan,10,Islamanad
+Jibraan,8,ShahAlam
+Allyan,3,Paris
+John,35,San Francisco
+Doe,22,Houston
+Dane,30,Seattle
+```
```

### Comparing `pysparkify-0.24.1/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.25.0/pysparkify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysparkify-0.24.1/setup.py` & `pysparkify-0.25.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.24.1',
+    version='0.25.0',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
```

### Comparing `pysparkify-0.24.1/src/app.py` & `pysparkify-0.25.0/src/app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.24.1/src/transformer/sql_transformer.py` & `pysparkify-0.25.0/src/transformer/sql_transformer.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.24.1/tests/test_app.py` & `pysparkify-0.25.0/tests/test_app.py`

 * *Files identical despite different names*

