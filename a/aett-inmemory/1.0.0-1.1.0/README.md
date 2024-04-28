# Comparing `tmp/aett_inmemory-1.0.0.tar.gz` & `tmp/aett_inmemory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_inmemory-1.0.0.tar", last modified: Fri Apr 26 16:18:50 2024, max compression
+gzip compressed data, was "aett_inmemory-1.1.0.tar", last modified: Sun Apr 28 12:40:09 2024, max compression
```

## Comparing `aett_inmemory-1.0.0.tar` & `aett_inmemory-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.270976 aett_inmemory-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.270976 aett_inmemory-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/src/aett/inmemory/
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/src/aett/inmemory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:09.341543 aett_inmemory-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:57.000000 aett_inmemory-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:57.000000 aett_inmemory-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-28 12:40:09.341543 aett_inmemory-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 12:39:57.000000 aett_inmemory-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-28 12:39:57.000000 aett_inmemory-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:40:09.341543 aett_inmemory-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:09.337542 aett_inmemory-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:09.337542 aett_inmemory-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:09.341543 aett_inmemory-1.1.0/src/aett/inmemory/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-28 12:39:57.000000 aett_inmemory-1.1.0/src/aett/inmemory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:09.341543 aett_inmemory-1.1.0/src/aett_inmemory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-28 12:40:09.000000 aett_inmemory-1.1.0/src/aett_inmemory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-28 12:40:09.000000 aett_inmemory-1.1.0/src/aett_inmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:40:09.000000 aett_inmemory-1.1.0/src/aett_inmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 12:40:09.000000 aett_inmemory-1.1.0/src/aett_inmemory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:40:09.000000 aett_inmemory-1.1.0/src/aett_inmemory.egg-info/top_level.txt
```

### Comparing `aett_inmemory-1.0.0/LICENSE` & `aett_inmemory-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_inmemory-1.0.0/PKG-INFO` & `aett_inmemory-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-inmemory
-Version: 1.0.0
+Version: 1.1.0
 Summary: In-Memory persistence for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,s3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
+Requires-Dist: aett-domain>=1.1.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_inmemory-1.0.0/README.md` & `aett_inmemory-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_inmemory-1.0.0/pyproject.toml` & `aett_inmemory-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.inmemory"]
 
 [project]
 name = "aett-inmemory"
-version = "1.0.0"
+version = "1.1.0"
 description = "In-Memory persistence for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "s3"]
 dependencies = [
-    'aett-domain >= 1.0.0'
+    'aett-domain >= 1.1.0'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_inmemory-1.0.0/src/aett/inmemory/__init__.py` & `aett_inmemory-1.1.0/src/aett/inmemory/__init__.py`

 * *Files identical despite different names*

### Comparing `aett_inmemory-1.0.0/src/aett_inmemory.egg-info/PKG-INFO` & `aett_inmemory-1.1.0/src/aett_inmemory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-inmemory
-Version: 1.0.0
+Version: 1.1.0
 Summary: In-Memory persistence for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,s3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
+Requires-Dist: aett-domain>=1.1.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

