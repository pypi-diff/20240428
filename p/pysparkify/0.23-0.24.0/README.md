# Comparing `tmp/pysparkify-0.23.tar.gz` & `tmp/pysparkify-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.23.tar", last modified: Sat Feb 10 15:42:45 2024, max compression
+gzip compressed data, was "pysparkify-0.24.0.tar", last modified: Sat Apr 27 22:02:10 2024, max compression
```

## Comparing `pysparkify-0.23.tar` & `pysparkify-0.24.0.tar`

### file list

```diff
@@ -1,12 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:42:45.232153 pysparkify-0.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-10 15:42:41.000000 pysparkify-0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-10 15:42:45.232153 pysparkify-0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-10 15:42:41.000000 pysparkify-0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:42:45.232153 pysparkify-0.23/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-10 15:42:45.000000 pysparkify-0.23/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-10 15:42:45.000000 pysparkify-0.23/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 15:42:45.000000 pysparkify-0.23/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-10 15:42:45.000000 pysparkify-0.23/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 15:42:45.000000 pysparkify-0.23/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 15:42:45.232153 pysparkify-0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-10 15:42:41.000000 pysparkify-0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-27 22:02:10.508392 pysparkify-0.24.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-27 22:02:07.000000 pysparkify-0.24.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:02:10.000000 pysparkify-0.24.0/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:02:10.508392 pysparkify-0.24.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-27 22:02:07.000000 pysparkify-0.24.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.504392 pysparkify-0.24.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/src/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/src/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/src/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:02:07.000000 pysparkify-0.24.0/src/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:10.508392 pysparkify-0.24.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:02:07.000000 pysparkify-0.24.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 22:02:07.000000 pysparkify-0.24.0/tests/test_app.py
```

### Comparing `pysparkify-0.23/PKG-INFO` & `pysparkify-0.24.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1
-Name: pysparkify
-Version: 0.23
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
-License-File: LICENSE
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: pyspark==3.5.0
-
 # Introduction
 This Spark package is designed to process data from various sources, perform transformations, and write the results to different sinks. It follows the pipeline design pattern to provide a flexible and modular approach to data processing.
 
-## Install
-The package is published for use on pypi. Install directly from pypi
+## Installation
+
+Install this package using:
+
+```bash
+pip install pysparkify
+```
+
+## Usage
+
+Run the library as a command line tool:
+
+```bash
+pysparkify your_recipe.yml
+```
+
+Or use it in your Python scripts:
+
+```python
+from pysparkify import run
+run('your_recipe.yml')
+```
 
-    pip install pysparkify
 
 ## Design
 
 The package is structured as follows:
 
 ### Source, Sink and Transformer Abstraction
 
@@ -44,9 +45,40 @@
 
 The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
 
 ## Setup
 
 The project is built using python-3.12.0, spark-3.5.0 (and other dependencies in requirements.txt).
 
-## Deployment
-... Environment specific documentation
+## How to Contribute
+
+1. Become a maintainer by requesting raohammad(at)gmail.com
+2. Open a PR
+3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
+
+
+# Pysparkify Library
+
+This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`.
+
+## Installation
+
+Install this package using:
+
+```bash
+pip install .
+```
+
+## Usage
+
+Run the library as a command line tool:
+
+```bash
+pysparkify your_recipe.yml
+```
+
+Or use it in your Python scripts:
+
+```python
+from pysparkify import run
+run('your_recipe.yml')
+```
```

### Comparing `pysparkify-0.23/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.24.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.23
+Version: 0.24.0
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: pyspark==3.5.0
+Requires-Dist: pyspark>=3.0.0
+Requires-Dist: pyyaml>=5.3
 
 # Introduction
 This Spark package is designed to process data from various sources, perform transformations, and write the results to different sinks. It follows the pipeline design pattern to provide a flexible and modular approach to data processing.
 
-## Install
-The package is published for use on pypi. Install directly from pypi
+## Installation
+
+Install this package using:
+
+```bash
+pip install pysparkify
+```
+
+## Usage
+
+Run the library as a command line tool:
+
+```bash
+pysparkify your_recipe.yml
+```
+
+Or use it in your Python scripts:
+
+```python
+from pysparkify import run
+run('your_recipe.yml')
+```
 
-    pip install pysparkify
 
 ## Design
 
 The package is structured as follows:
 
 ### Source, Sink and Transformer Abstraction
 
@@ -44,9 +62,40 @@
 
 The package reads data from the specified source, performs transformations based on the configured SQL queries, and then writes the results to the specified sink. You can configure multiple sources and sinks within the same package.
 
 ## Setup
 
 The project is built using python-3.12.0, spark-3.5.0 (and other dependencies in requirements.txt).
 
-## Deployment
-... Environment specific documentation
+## How to Contribute
+
+1. Become a maintainer by requesting raohammad(at)gmail.com
+2. Open a PR
+3. Once the PR is reviewed and approved, included github actions will deploy the version directly to pypi repository
+
+
+# Pysparkify Library
+
+This library abstracts Spark data processing workflows. Define your workflow in `recipe.yml`.
+
+## Installation
+
+Install this package using:
+
+```bash
+pip install .
+```
+
+## Usage
+
+Run the library as a command line tool:
+
+```bash
+pysparkify your_recipe.yml
+```
+
+Or use it in your Python scripts:
+
+```python
+from pysparkify import run
+run('your_recipe.yml')
+```
```

