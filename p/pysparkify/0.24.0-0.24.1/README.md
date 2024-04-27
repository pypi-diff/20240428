# Comparing `tmp/pysparkify-0.24.0.tar.gz` & `tmp/pysparkify-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.24.0.tar", last modified: Sat Apr 27 22:02:10 2024, max compression
+gzip compressed data, was "pysparkify-0.24.1.tar", last modified: Sat Apr 27 22:08:25 2024, max compression
```

## Comparing `pysparkify-0.24.0.tar` & `pysparkify-0.24.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-27 22:02:10.508392 pysparkify-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-27 22:02:07.000000 pysparkify-0.24.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:02:10.508392 pysparkify-0.24.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-27 22:02:07.000000 pysparkify-0.24.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.504392 pysparkify-0.24.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/src/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/src/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/src/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 22:02:07.000000 pysparkify-0.24.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 22:08:25.980578 pysparkify-0.24.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-27 22:08:23.000000 pysparkify-0.24.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:08:25.000000 pysparkify-0.24.1/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:08:25.980578 pysparkify-0.24.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-27 22:08:23.000000 pysparkify-0.24.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.976578 pysparkify-0.24.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/src/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/src/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/src/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:08:23.000000 pysparkify-0.24.1/src/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:25.980578 pysparkify-0.24.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:08:23.000000 pysparkify-0.24.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 22:08:23.000000 pysparkify-0.24.1/tests/test_app.py
```

### Comparing `pysparkify-0.24.0/PKG-INFO` & `pysparkify-0.24.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.24.0
+Version: 0.24.1
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -71,31 +71,42 @@
 1. Become a maintainer by requesting raohammad(at)gmail.com
 2. Open a PR
 3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
 # Pysparkify Library
 
-This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`.
+This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
-## Installation
-
-Install this package using:
-
-```bash
-pip install .
 ```
-
-## Usage
-
-Run the library as a command line tool:
-
-```bash
-pysparkify your_recipe.yml
-```
-
-Or use it in your Python scripts:
-
-```python
-from pysparkify import run
-run('your_recipe.yml')
+source:
+  - type: CsvSource
+    config:
+      name: csv
+      path: "resources/data/input_data.csv"
+
+transformer:
+  - type: SQLTransformer
+    config:
+      name: transformer1
+      source: 
+        - name: csv
+          as_name: t1
+      statement: 
+        - sql: "SELECT * from t1 limit 2"
+          as_name: trx1
+          to_sink: sink1
+        - sql: "select AVG(age) from trx1"
+          as_name: trx2
+          to_sink: sink2
+
+sink:
+  - type: CsvSink
+    config:
+      name: sink1
+      path: "output/output_data.csv"
+  - type: CsvSink
+    config:
+      name: sink2
+      path: "output/avgage_data.csv"
+      
 ```
```

### Comparing `pysparkify-0.24.0/README.md` & `pysparkify-0.24.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -54,31 +54,42 @@
 1. Become a maintainer by requesting raohammad(at)gmail.com
 2. Open a PR
 3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
 # Pysparkify Library
 
-This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`.
+This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
-## Installation
-
-Install this package using:
-
-```bash
-pip install .
-```
-
-## Usage
-
-Run the library as a command line tool:
-
-```bash
-pysparkify your_recipe.yml
-```
-
-Or use it in your Python scripts:
-
-```python
-from pysparkify import run
-run('your_recipe.yml')
 ```
+source:
+  - type: CsvSource
+    config:
+      name: csv
+      path: "resources/data/input_data.csv"
+
+transformer:
+  - type: SQLTransformer
+    config:
+      name: transformer1
+      source: 
+        - name: csv
+          as_name: t1
+      statement: 
+        - sql: "SELECT * from t1 limit 2"
+          as_name: trx1
+          to_sink: sink1
+        - sql: "select AVG(age) from trx1"
+          as_name: trx2
+          to_sink: sink2
+
+sink:
+  - type: CsvSink
+    config:
+      name: sink1
+      path: "output/output_data.csv"
+  - type: CsvSink
+    config:
+      name: sink2
+      path: "output/avgage_data.csv"
+      
+```
```

### Comparing `pysparkify-0.24.0/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.24.1/pysparkify.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.24.0
+Version: 0.24.1
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -71,31 +71,42 @@
 1. Become a maintainer by requesting raohammad(at)gmail.com
 2. Open a PR
 3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
 # Pysparkify Library
 
-This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`.
+This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
-## Installation
-
-Install this package using:
-
-```bash
-pip install .
 ```
-
-## Usage
-
-Run the library as a command line tool:
-
-```bash
-pysparkify your_recipe.yml
-```
-
-Or use it in your Python scripts:
-
-```python
-from pysparkify import run
-run('your_recipe.yml')
+source:
+  - type: CsvSource
+    config:
+      name: csv
+      path: "resources/data/input_data.csv"
+
+transformer:
+  - type: SQLTransformer
+    config:
+      name: transformer1
+      source: 
+        - name: csv
+          as_name: t1
+      statement: 
+        - sql: "SELECT * from t1 limit 2"
+          as_name: trx1
+          to_sink: sink1
+        - sql: "select AVG(age) from trx1"
+          as_name: trx2
+          to_sink: sink2
+
+sink:
+  - type: CsvSink
+    config:
+      name: sink1
+      path: "output/output_data.csv"
+  - type: CsvSink
+    config:
+      name: sink2
+      path: "output/avgage_data.csv"
+      
 ```
```

### Comparing `pysparkify-0.24.0/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.24.1/pysparkify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysparkify-0.24.0/setup.py` & `pysparkify-0.24.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.24.0',
+    version='0.24.1',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
@@ -27,12 +27,12 @@
     packages=find_packages(),
     install_requires=[
         'pyspark>=3.0.0',
         'pyyaml>=5.3'
     ],
     entry_points={
         'console_scripts': [
-            'pysparkify=pysparkify.src.app:run'
+            'pysparkify=src.app:run'
         ]
     },
     classifiers=CLASSIFIERS,
 )
```

### Comparing `pysparkify-0.24.0/src/app.py` & `pysparkify-0.24.1/src/app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.24.0/src/transformer/sql_transformer.py` & `pysparkify-0.24.1/src/transformer/sql_transformer.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.24.0/tests/test_app.py` & `pysparkify-0.24.1/tests/test_app.py`

 * *Files identical despite different names*

