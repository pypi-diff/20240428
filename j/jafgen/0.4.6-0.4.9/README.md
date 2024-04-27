# Comparing `tmp/jafgen-0.4.6.tar.gz` & `tmp/jafgen-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jafgen-0.4.6.tar", last modified: Sun Apr  7 21:25:27 2024, max compression
+gzip compressed data, was "jafgen-0.4.9.tar", last modified: Sun Apr  7 21:39:23 2024, max compression
```

## Comparing `jafgen-0.4.6.tar` & `jafgen-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 21:25:16.000000 jafgen-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-07 21:25:27.604475 jafgen-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-07 21:25:16.000000 jafgen-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.600475 jafgen-0.4.6/jafgen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/curves.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/jafgen/customers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/order_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/jafgen/stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/supply.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/jafgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 21:25:16.000000 jafgen-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:25:27.604475 jafgen-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-07 21:25:16.000000 jafgen-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 21:25:16.000000 jafgen-0.4.6/tests/test_days.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 21:25:16.000000 jafgen-0.4.6/tests/test_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:23.310090 jafgen-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 21:39:14.000000 jafgen-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-07 21:39:23.310090 jafgen-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-07 21:39:14.000000 jafgen-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:23.306090 jafgen-0.4.9/jafgen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:23.306090 jafgen-0.4.9/jafgen/customers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/customers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/customers/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/customers/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/customers/order_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:23.310090 jafgen-0.4.9/jafgen/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-07 21:39:14.000000 jafgen-0.4.9/jafgen/stores/supply.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:23.310090 jafgen-0.4.9/jafgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-07 21:39:23.000000 jafgen-0.4.9/jafgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 21:39:23.000000 jafgen-0.4.9/jafgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:39:23.000000 jafgen-0.4.9/jafgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 21:39:23.000000 jafgen-0.4.9/jafgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 21:39:23.000000 jafgen-0.4.9/jafgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 21:39:23.000000 jafgen-0.4.9/jafgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 21:39:14.000000 jafgen-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:39:23.310090 jafgen-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-07 21:39:14.000000 jafgen-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:39:23.310090 jafgen-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 21:39:14.000000 jafgen-0.4.9/tests/test_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 21:39:14.000000 jafgen-0.4.9/tests/test_inventory.py
```

### Comparing `jafgen-0.4.6/LICENSE` & `jafgen-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/PKG-INFO` & `jafgen-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jafgen
-Version: 0.4.6
+Version: 0.4.9
 Summary: A synthetic data generator CLI for a fictional Jaffle Shop
 Author-email: gwenwindflower <gwenwindflower@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `jafgen-0.4.6/README.md` & `jafgen-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/curves.py` & `jafgen-0.4.9/jafgen/curves.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/customers/customers.py` & `jafgen-0.4.9/jafgen/customers/customers.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/customers/order.py` & `jafgen-0.4.9/jafgen/customers/order.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/simulation.py` & `jafgen-0.4.9/jafgen/simulation.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/stores/inventory.py` & `jafgen-0.4.9/jafgen/stores/inventory.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/stores/item.py` & `jafgen-0.4.9/jafgen/stores/item.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/stores/market.py` & `jafgen-0.4.9/jafgen/stores/market.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/stores/stock.py` & `jafgen-0.4.9/jafgen/stores/stock.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/stores/store.py` & `jafgen-0.4.9/jafgen/stores/store.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen/stores/supply.py` & `jafgen-0.4.9/jafgen/stores/supply.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/jafgen.egg-info/PKG-INFO` & `jafgen-0.4.9/jafgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jafgen
-Version: 0.4.6
+Version: 0.4.9
 Summary: A synthetic data generator CLI for a fictional Jaffle Shop
 Author-email: gwenwindflower <gwenwindflower@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `jafgen-0.4.6/jafgen.egg-info/SOURCES.txt` & `jafgen-0.4.9/jafgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jafgen-0.4.6/pyproject.toml` & `jafgen-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jafgen"
-version = "0.4.6"
+version = "0.4.9"
 authors = [{ name = "gwenwindflower", email = "gwenwindflower@gmail.com" }]
 dependencies = ["numpy", "pandas", "Faker", "typer[all]"]
 description = "A synthetic data generator CLI for a fictional Jaffle Shop"
 readme = "README.md"
 license = { file = "LICENSE" }
 [tool.setuptools.packages.find]
 exclude = ["*.tests", "*.tests.*", "tests.*", "tests"]
```

### Comparing `jafgen-0.4.6/setup.py` & `jafgen-0.4.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jafgen",
-    version="0.4.1",
+    version="0.4.9",
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"],
     ),
     authors=["gwenwindflower", "drewbanin"],
     description="A synthetic data generator CLI for a fictional Jaffle Shop",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `jafgen-0.4.6/tests/test_inventory.py` & `jafgen-0.4.9/tests/test_inventory.py`

 * *Files identical despite different names*

