# Comparing `tmp/pysparkify-0.25.0.tar.gz` & `tmp/pysparkify-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.25.0.tar", last modified: Sat Apr 27 22:13:47 2024, max compression
+gzip compressed data, was "pysparkify-0.26.0.tar", last modified: Sun Apr 28 04:47:01 2024, max compression
```

## Comparing `pysparkify-0.25.0.tar` & `pysparkify-0.26.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-27 22:13:47.976441 pysparkify-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-27 22:13:45.000000 pysparkify-0.25.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:13:47.000000 pysparkify-0.25.0/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:13:47.976441 pysparkify-0.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-27 22:13:45.000000 pysparkify-0.25.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/src/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:13:45.000000 pysparkify-0.25.0/src/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:47.976441 pysparkify-0.25.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:13:45.000000 pysparkify-0.25.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 22:13:45.000000 pysparkify-0.25.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-28 04:47:01.218595 pysparkify-0.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-28 04:46:58.000000 pysparkify-0.26.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.214594 pysparkify-0.26.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.214594 pysparkify-0.26.0/lib/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.214594 pysparkify-0.26.0/lib/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/lib/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-28 04:46:58.000000 pysparkify-0.26.0/lib/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 04:47:01.000000 pysparkify-0.26.0/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:47:01.218595 pysparkify-0.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-28 04:46:58.000000 pysparkify-0.26.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:47:01.218595 pysparkify-0.26.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:46:58.000000 pysparkify-0.26.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 04:46:58.000000 pysparkify-0.26.0/tests/test_app.py
```

### Comparing `pysparkify-0.25.0/PKG-INFO` & `pysparkify-0.26.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.25.0
+Version: 0.26.0
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -22,26 +22,36 @@
 
 Install this package using:
 
 ```bash
 pip install pysparkify
 ```
 
+Create sparkc_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
+
+```bash
+[SPARK]
+spark.master=local[*]
+spark.app.name=PysparkifyApp
+spark.executor.memory=4g
+spark.driver.memory=2g
+```
+
 ## Usage
 
 Run the library as a command line tool:
 
 ```bash
 pysparkify your_recipe.yml
 ```
 
 Or use it in your Python scripts:
 
 ```python
-from pysparkify import run
+from pysparkify.lib.app import run
 run('your_recipe.yml')
 ```
 
 
 ## Design
 
 The package is structured as follows:
```

### Comparing `pysparkify-0.25.0/README.md` & `pysparkify-0.26.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,36 @@
 
 Install this package using:
 
 ```bash
 pip install pysparkify
 ```
 
+Create sparkc_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
+
+```bash
+[SPARK]
+spark.master=local[*]
+spark.app.name=PysparkifyApp
+spark.executor.memory=4g
+spark.driver.memory=2g
+```
+
 ## Usage
 
 Run the library as a command line tool:
 
 ```bash
 pysparkify your_recipe.yml
 ```
 
 Or use it in your Python scripts:
 
 ```python
-from pysparkify import run
+from pysparkify.lib.app import run
 run('your_recipe.yml')
 ```
 
 
 ## Design
 
 The package is structured as follows:
```

### Comparing `pysparkify-0.25.0/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.26.0/pysparkify.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.25.0
+Version: 0.26.0
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -22,26 +22,36 @@
 
 Install this package using:
 
 ```bash
 pip install pysparkify
 ```
 
+Create sparkc_config.conf file of this format to enter all configurations related to spark in `config/spark_config.conf`
+
+```bash
+[SPARK]
+spark.master=local[*]
+spark.app.name=PysparkifyApp
+spark.executor.memory=4g
+spark.driver.memory=2g
+```
+
 ## Usage
 
 Run the library as a command line tool:
 
 ```bash
 pysparkify your_recipe.yml
 ```
 
 Or use it in your Python scripts:
 
 ```python
-from pysparkify import run
+from pysparkify.lib.app import run
 run('your_recipe.yml')
 ```
 
 
 ## Design
 
 The package is structured as follows:
```

### Comparing `pysparkify-0.25.0/setup.py` & `pysparkify-0.26.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.25.0',
+    version='0.26.0',
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
-            'pysparkify=src.app:run'
+            'pysparkify=lib.app:main'
         ]
     },
     classifiers=CLASSIFIERS,
 )
```

### Comparing `pysparkify-0.25.0/src/app.py` & `pysparkify-0.26.0/lib/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import yaml
 from pyspark.sql import SparkSession
 import pyspark
 from .context_manager import get_spark_session
 from configparser import ConfigParser
 
 # import sources
-from source.source_factory import SourceFactory
+from lib.source.source_factory import SourceFactory
 
 # import sinks
-from sink.sink_factory import SinkFactory
+from lib.sink.sink_factory import SinkFactory
 
 # import transformers
-from transformer.transformer_factory import TransformerFactory
+from lib.transformer.transformer_factory import TransformerFactory
 
 # Initialize lists to store sources, sinks, and transformers
 source_list = []
 sink_list = []
 transformer_list = []
 
 def instantiate_source(config):
@@ -81,14 +81,20 @@
 #     spark = SparkSession.builder.config(conf=conf).getOrCreate()
 
 #     process_data(args.config, spark)
 
 #     # Stop the Spark session when done
 #     spark.stop()
 
+# def run(recipe_path):
+#     # Existing code to run the application using the provided recipe_path
+#     print(f"Running with recipe: {recipe_path}")
+#     # Example Spark session usage
+#     spark = get_spark_session()
+
 def run(recipe_path):
     # Load Spark configurations from file
     config = ConfigParser()
     config.read('config/spark_config.conf')
 
     # Prepare the Spark config dictionary
     spark_config = {key: value for key, value in config.items('SPARK')}
@@ -97,8 +103,17 @@
     spark = get_spark_session(app_name=config.get('SPARK', 'spark.app.name'), config=spark_config)
 
     process_data(recipe_path, spark)
 
     # Continue with your application logic, such as loading data, performing transformations, and writing outputs
     # Example: data = spark.read.csv("path/to/your/data.csv")
     # Remember to stop the Spark session when done
-    spark.stop()
+    spark.stop()
+
+def main():
+    parser = argparse.ArgumentParser(description="Run Pysparkify application")
+    parser.add_argument('recipe_path', type=str, help='Path to the recipe YAML file')
+    args = parser.parse_args()
+    run(args.recipe_path)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pysparkify-0.25.0/src/transformer/sql_transformer.py` & `pysparkify-0.26.0/lib/transformer/sql_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql import SparkSession
-from transformer.transformer import Transformer
+from lib.transformer.transformer import Transformer
 
 class SQLTransformer(Transformer):
     def __init__(self, config):
         super().__init__(config)
 
     def transform(self, spark, sources, sinks):
         # Register temporary tables from source configurations
```

### Comparing `pysparkify-0.25.0/tests/test_app.py` & `pysparkify-0.26.0/tests/test_app.py`

 * *Files identical despite different names*

