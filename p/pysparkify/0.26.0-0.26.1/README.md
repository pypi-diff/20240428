# Comparing `tmp/pysparkify-0.26.0.tar.gz` & `tmp/pysparkify-0.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.26.0.tar", last modified: Sun Apr 28 04:47:01 2024, max compression
+gzip compressed data, was "pysparkify-0.26.1.tar", last modified: Sun Apr 28 04:57:37 2024, max compression
```

## Comparing `pysparkify-0.26.0.tar` & `pysparkify-0.26.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-28 04:47:01.218595 pysparkify-0.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-28 04:46:58.000000 pysparkify-0.26.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.214594 pysparkify-0.26.0/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.214594 pysparkify-0.26.0/lib/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.214594 pysparkify-0.26.0/lib/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/lib/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:47:01.218595 pysparkify-0.26.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-28 04:46:58.000000 pysparkify-0.26.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 04:46:58.000000 pysparkify-0.26.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.862377 pysparkify-0.26.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-28 04:57:37.862377 pysparkify-0.26.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-28 04:57:35.000000 pysparkify-0.26.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.858377 pysparkify-0.26.1/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.858377 pysparkify-0.26.1/lib/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.858377 pysparkify-0.26.1/lib/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.858377 pysparkify-0.26.1/lib/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-28 04:57:35.000000 pysparkify-0.26.1/lib/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.862377 pysparkify-0.26.1/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-28 04:57:37.000000 pysparkify-0.26.1/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 04:57:37.000000 pysparkify-0.26.1/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:57:37.000000 pysparkify-0.26.1/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 04:57:37.000000 pysparkify-0.26.1/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 04:57:37.000000 pysparkify-0.26.1/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 04:57:37.000000 pysparkify-0.26.1/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:57:37.862377 pysparkify-0.26.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-28 04:57:35.000000 pysparkify-0.26.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:37.862377 pysparkify-0.26.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:57:35.000000 pysparkify-0.26.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 04:57:35.000000 pysparkify-0.26.1/tests/test_app.py
```

### Comparing `pysparkify-0.26.0/PKG-INFO` & `pysparkify-0.26.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,46 @@
-Metadata-Version: 2.1
-Name: pysparkify
-Version: 0.26.0
-Summary: Spark based ETL
-Home-page: https://github.com/raohammad/pysparkify
-Author: Hammad Aslam KHAN
-Author-email: raohammad@gmail.com
-License: MIT
-Keywords: python,pysparkify,etl,bigdata
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-Requires-Dist: pyspark>=3.0.0
-Requires-Dist: pyyaml>=5.3
-
 # Introduction
 This Spark package is designed to process data from various sources, perform transformations, and write the results to different sinks. It follows the pipeline design pattern to provide a flexible and modular approach to data processing.
 
-## Installation
+## Setup
 
 Install this package using:
 
 ```bash
 pip install pysparkify
 ```
 
-Create sparkc_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
+Create spark_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
 
 ```bash
 [SPARK]
 spark.master=local[*]
 spark.app.name=PysparkifyApp
 spark.executor.memory=4g
 spark.driver.memory=2g
 ```
 
-## Usage
+This library abstracts Spark data processing workflows. For example you would like to;
 
-Run the library as a command line tool:
+- take first two rows of the data, save it as a separate output
+- take an average and save it as a separate output
 
-```bash
-pysparkify your_recipe.yml
-```
+with below sample data
 
-Or use it in your Python scripts:
-
-```python
-from pysparkify.lib.app import run
-run('your_recipe.yml')
+```
+name,age,city
+Hayaan,10,Islamanad
+Jibraan,8,ShahAlam
+Allyan,3,Paris
+John,35,San Francisco
+Doe,22,Houston
+Dane,30,Seattle
 ```
 
-
-## Design
-
-The package is structured as follows:
-
-### Source, Sink and Transformer Abstraction
-
-The package defines abstract classes `Source`, `Sink` and `Transformer` to represent data sources, sinks and transformers. It also provides concrete classes, including `CsvSource`, `CsvSink` and `SQLTransformer`, which inherit from the abstract classes. This design allows you to add new source and sink types with ease.
-
-### Configuration via `recipe.yml`
-
-The package reads its configuration from a `recipe.yml` file. This YAML file specifies the source, sink, and transformation configurations. It allows you to define different data sources, sinks, and transformation queries.
-
-### Transformation Queries
-
-Transformations are performed by `SQLTransformer` using Spark SQL queries defined in the configuration. These queries are executed on the data from the source before writing it to the sink. New transformers can be implemented by extending `Transformer` abstract class that can take spark dataframes from sources to process and send dataframes to sinks to save.
-
-### Pipeline Execution
-
-The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
-
-## Setup
-
-The project is built using python-3.12.0, spark-3.5.0 (and other dependencies in requirements.txt).
-
-## How to Contribute
-
-1. Become a maintainer by requesting raohammad(at)gmail.com
-2. Open a PR
-3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
-
-
-# Pysparkify Usage Example
-
-This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
+Your recipe reads the csv data as source, transforms the data and optionally save the output of each transformation to sink. Below would be the recipe.yml for this operation.
 
 ```
 source:
   - type: CsvSource
     config:
       name: csv
       path: "resources/data/input_data.csv"
@@ -117,18 +68,56 @@
   - type: CsvSink
     config:
       name: sink2
       path: "output/avgage_data.csv"
       
 ```
 
-The sample from csv source file used in above transformation is as below;
 
+## Usage
+
+This library can be run as a command line tool:
+
+```bash
+pysparkify your_recipe.yml
 ```
-name,age,city
-Hayaan,10,Islamanad
-Jibraan,8,ShahAlam
-Allyan,3,Paris
-John,35,San Francisco
-Doe,22,Houston
-Dane,30,Seattle
+
+Or use it in your Python scripts:
+
+```python
+from pysparkify.lib.app import run
+run('your_recipe.yml')
 ```
+
+
+## Design
+
+The package is structured as follows:
+
+### Source, Sink and Transformer Abstraction
+
+The package defines abstract classes `Source`, `Sink` and `Transformer` to represent data sources, sinks and transformers. It also provides concrete classes, including `CsvSource`, `CsvSink` and `SQLTransformer`, which inherit from the abstract classes. This design allows you to add new source and sink types with ease.
+
+### Configuration via `recipe.yml`
+
+The package reads its configuration from a `recipe.yml` file. This YAML file specifies the source, sink, and transformation configurations. It allows you to define different data sources, sinks, and transformation queries.
+
+### Transformation Queries
+
+Transformations are performed by `SQLTransformer` using Spark SQL queries defined in the configuration. These queries are executed on the data from the source before writing it to the sink. New transformers can be implemented by extending `Transformer` abstract class that can take spark dataframes from sources to process and send dataframes to sinks to save.
+
+### Pipeline Execution
+
+The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
+
+
+
+
+# Pysparkify Usage Example
+
+
+
+## How to Contribute
+
+1. Become a maintainer by requesting raohammad(at)gmail.com
+2. Open a PR
+3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
```

### Comparing `pysparkify-0.26.0/README.md` & `pysparkify-0.26.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,102 @@
+Metadata-Version: 2.1
+Name: pysparkify
+Version: 0.26.1
+Summary: Spark based ETL
+Home-page: https://github.com/raohammad/pysparkify
+Author: Hammad Aslam KHAN
+Author-email: raohammad@gmail.com
+License: MIT
+Keywords: python,pysparkify,etl,bigdata
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+Requires-Dist: pyspark>=3.0.0
+Requires-Dist: pyyaml>=5.3
+
 # Introduction
 This Spark package is designed to process data from various sources, perform transformations, and write the results to different sinks. It follows the pipeline design pattern to provide a flexible and modular approach to data processing.
 
-## Installation
+## Setup
 
 Install this package using:
 
 ```bash
 pip install pysparkify
 ```
 
-Create sparkc_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
+Create spark_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
 
 ```bash
 [SPARK]
 spark.master=local[*]
 spark.app.name=PysparkifyApp
 spark.executor.memory=4g
 spark.driver.memory=2g
 ```
 
+This library abstracts Spark data processing workflows. For example you would like to;
+
+- take first two rows of the data, save it as a separate output
+- take an average and save it as a separate output
+
+with below sample data
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
+
+Your recipe reads the csv data as source, transforms the data and optionally save the output of each transformation to sink. Below would be the recipe.yml for this operation.
+
+```
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
+
+
 ## Usage
 
-Run the library as a command line tool:
+This library can be run as a command line tool:
 
 ```bash
 pysparkify your_recipe.yml
 ```
 
 Or use it in your Python scripts:
 
@@ -51,67 +122,19 @@
 
 Transformations are performed by `SQLTransformer` using Spark SQL queries defined in the configuration. These queries are executed on the data from the source before writing it to the sink. New transformers can be implemented by extending `Transformer` abstract class that can take spark dataframes from sources to process and send dataframes to sinks to save.
 
 ### Pipeline Execution
 
 The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
 
-## Setup
 
-The project is built using python-3.12.0, spark-3.5.0 (and other dependencies in requirements.txt).
-
-## How to Contribute
-
-1. Become a maintainer by requesting raohammad(at)gmail.com
-2. Open a PR
-3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
 
 
 # Pysparkify Usage Example
 
-This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
 
-```
-source:
-  - type: CsvSource
-    config:
-      name: csv
-      path: "resources/data/input_data.csv"
 
-transformer:
-  - type: SQLTransformer
-    config:
-      name: transformer1
-      source: 
-        - name: csv
-          as_name: t1
-      statement: 
-        - sql: "SELECT * from t1 limit 2"
-          as_name: trx1
-          to_sink: sink1
-        - sql: "select AVG(age) from trx1"
-          as_name: trx2
-          to_sink: sink2
-
-sink:
-  - type: CsvSink
-    config:
-      name: sink1
-      path: "output/output_data.csv"
-  - type: CsvSink
-    config:
-      name: sink2
-      path: "output/avgage_data.csv"
-      
-```
-
-The sample from csv source file used in above transformation is as below;
+## How to Contribute
 
-```
-name,age,city
-Hayaan,10,Islamanad
-Jibraan,8,ShahAlam
-Allyan,3,Paris
-John,35,San Francisco
-Doe,22,Houston
-Dane,30,Seattle
-```
+1. Become a maintainer by requesting raohammad(at)gmail.com
+2. Open a PR
+3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
```

### Comparing `pysparkify-0.26.0/lib/app.py` & `pysparkify-0.26.1/lib/app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.0/lib/transformer/sql_transformer.py` & `pysparkify-0.26.1/lib/transformer/sql_transformer.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.0/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.26.1/pysparkify.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.0
+Version: 0.26.1
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -14,82 +14,50 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark>=3.0.0
 Requires-Dist: pyyaml>=5.3
 
 # Introduction
 This Spark package is designed to process data from various sources, perform transformations, and write the results to different sinks. It follows the pipeline design pattern to provide a flexible and modular approach to data processing.
 
-## Installation
+## Setup
 
 Install this package using:
 
 ```bash
 pip install pysparkify
 ```
 
-Create sparkc_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
+Create spark_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
 
 ```bash
 [SPARK]
 spark.master=local[*]
 spark.app.name=PysparkifyApp
 spark.executor.memory=4g
 spark.driver.memory=2g
 ```
 
-## Usage
+This library abstracts Spark data processing workflows. For example you would like to;
 
-Run the library as a command line tool:
+- take first two rows of the data, save it as a separate output
+- take an average and save it as a separate output
 
-```bash
-pysparkify your_recipe.yml
-```
-
-Or use it in your Python scripts:
+with below sample data
 
-```python
-from pysparkify.lib.app import run
-run('your_recipe.yml')
+```
+name,age,city
+Hayaan,10,Islamanad
+Jibraan,8,ShahAlam
+Allyan,3,Paris
+John,35,San Francisco
+Doe,22,Houston
+Dane,30,Seattle
 ```
 
-
-## Design
-
-The package is structured as follows:
-
-### Source, Sink and Transformer Abstraction
-
-The package defines abstract classes `Source`, `Sink` and `Transformer` to represent data sources, sinks and transformers. It also provides concrete classes, including `CsvSource`, `CsvSink` and `SQLTransformer`, which inherit from the abstract classes. This design allows you to add new source and sink types with ease.
-
-### Configuration via `recipe.yml`
-
-The package reads its configuration from a `recipe.yml` file. This YAML file specifies the source, sink, and transformation configurations. It allows you to define different data sources, sinks, and transformation queries.
-
-### Transformation Queries
-
-Transformations are performed by `SQLTransformer` using Spark SQL queries defined in the configuration. These queries are executed on the data from the source before writing it to the sink. New transformers can be implemented by extending `Transformer` abstract class that can take spark dataframes from sources to process and send dataframes to sinks to save.
-
-### Pipeline Execution
-
-The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
-
-## Setup
-
-The project is built using python-3.12.0, spark-3.5.0 (and other dependencies in requirements.txt).
-
-## How to Contribute
-
-1. Become a maintainer by requesting raohammad(at)gmail.com
-2. Open a PR
-3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
-
-
-# Pysparkify Usage Example
-
-This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`. Reads data from CSV source and writes data to CSV Sink (paths mentioned in config) after data transformation (SQL mentioned in config too)
+Your recipe reads the csv data as source, transforms the data and optionally save the output of each transformation to sink. Below would be the recipe.yml for this operation.
 
 ```
 source:
   - type: CsvSource
     config:
       name: csv
       path: "resources/data/input_data.csv"
@@ -117,18 +85,56 @@
   - type: CsvSink
     config:
       name: sink2
       path: "output/avgage_data.csv"
       
 ```
 
-The sample from csv source file used in above transformation is as below;
 
+## Usage
+
+This library can be run as a command line tool:
+
+```bash
+pysparkify your_recipe.yml
 ```
-name,age,city
-Hayaan,10,Islamanad
-Jibraan,8,ShahAlam
-Allyan,3,Paris
-John,35,San Francisco
-Doe,22,Houston
-Dane,30,Seattle
+
+Or use it in your Python scripts:
+
+```python
+from pysparkify.lib.app import run
+run('your_recipe.yml')
 ```
+
+
+## Design
+
+The package is structured as follows:
+
+### Source, Sink and Transformer Abstraction
+
+The package defines abstract classes `Source`, `Sink` and `Transformer` to represent data sources, sinks and transformers. It also provides concrete classes, including `CsvSource`, `CsvSink` and `SQLTransformer`, which inherit from the abstract classes. This design allows you to add new source and sink types with ease.
+
+### Configuration via `recipe.yml`
+
+The package reads its configuration from a `recipe.yml` file. This YAML file specifies the source, sink, and transformation configurations. It allows you to define different data sources, sinks, and transformation queries.
+
+### Transformation Queries
+
+Transformations are performed by `SQLTransformer` using Spark SQL queries defined in the configuration. These queries are executed on the data from the source before writing it to the sink. New transformers can be implemented by extending `Transformer` abstract class that can take spark dataframes from sources to process and send dataframes to sinks to save.
+
+### Pipeline Execution
+
+The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
+
+
+
+
+# Pysparkify Usage Example
+
+
+
+## How to Contribute
+
+1. Become a maintainer by requesting raohammad(at)gmail.com
+2. Open a PR
+3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
```

### Comparing `pysparkify-0.26.0/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.26.1/pysparkify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.0/setup.py` & `pysparkify-0.26.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.26.0',
+    version='0.26.1',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
```

### Comparing `pysparkify-0.26.0/tests/test_app.py` & `pysparkify-0.26.1/tests/test_app.py`

 * *Files identical despite different names*

