# Comparing `tmp/duckreporter-0.0.1.tar.gz` & `tmp/duckreporter-0.0.2.tar.gz`

## Comparing `duckreporter-0.0.1.tar` & `duckreporter-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 duckreporter-0.0.1/requirements.in
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 duckreporter-0.0.1/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckreporter-0.0.1/src/duckreporter/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 duckreporter-0.0.1/src/duckreporter/emitter.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 duckreporter-0.0.1/src/duckreporter/trace.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 duckreporter-0.0.1/src/duckreporter/worker.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 duckreporter-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 duckreporter-0.0.1/LICENSE
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 duckreporter-0.0.1/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 duckreporter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 duckreporter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 duckreporter-0.0.2/requirements.in
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 duckreporter-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckreporter-0.0.2/src/duckreporter/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 duckreporter-0.0.2/src/duckreporter/emitter.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 duckreporter-0.0.2/src/duckreporter/trace.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 duckreporter-0.0.2/src/duckreporter/worker.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 duckreporter-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 duckreporter-0.0.2/LICENSE
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 duckreporter-0.0.2/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 duckreporter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 duckreporter-0.0.2/PKG-INFO
```

### Comparing `duckreporter-0.0.1/src/duckreporter/emitter.py` & `duckreporter-0.0.2/src/duckreporter/emitter.py`

 * *Files identical despite different names*

### Comparing `duckreporter-0.0.1/src/duckreporter/trace.py` & `duckreporter-0.0.2/src/duckreporter/trace.py`

 * *Files identical despite different names*

### Comparing `duckreporter-0.0.1/src/duckreporter/worker.py` & `duckreporter-0.0.2/src/duckreporter/worker.py`

 * *Files identical despite different names*

### Comparing `duckreporter-0.0.1/.gitignore` & `duckreporter-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `duckreporter-0.0.1/LICENSE` & `duckreporter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `duckreporter-0.0.1/pyproject.toml` & `duckreporter-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/duckreporter"]
 
 [project]
 name = "DuckReporter"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Drop Tables", email="build@droptables.com" },
 ]
 description = "A package to trace python functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `duckreporter-0.0.1/PKG-INFO` & `duckreporter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: DuckReporter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to trace python functions
 Project-URL: Homepage, https://github.com/duckyio
 Project-URL: Issues, https://github.com/duckyio
 Author-email: Drop Tables <build@droptables.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

