# Comparing `tmp/aett_s3-1.0.0.tar.gz` & `tmp/aett_s3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_s3-1.0.0.tar", last modified: Fri Apr 26 16:18:50 2024, max compression
+gzip compressed data, was "aett_s3-1.1.0.tar", last modified: Sun Apr 28 12:39:57 2024, max compression
```

## Comparing `aett_s3-1.0.0.tar` & `aett_s3-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.171749 aett_s3-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:44.000000 aett_s3-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:44.000000 aett_s3-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-26 16:18:50.171749 aett_s3-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-26 16:18:44.000000 aett_s3-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-26 16:18:44.000000 aett_s3-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:50.171749 aett_s3-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.167749 aett_s3-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.167749 aett_s3-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.171749 aett_s3-1.0.0/src/aett/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-26 16:18:44.000000 aett_s3-1.0.0/src/aett/s3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.171749 aett_s3-1.0.0/src/aett_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:57.131989 aett_s3-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:51.000000 aett_s3-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:51.000000 aett_s3-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-28 12:39:57.131989 aett_s3-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-28 12:39:51.000000 aett_s3-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-28 12:39:51.000000 aett_s3-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:39:57.131989 aett_s3-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:57.127989 aett_s3-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:57.127989 aett_s3-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:57.131989 aett_s3-1.1.0/src/aett/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-28 12:39:51.000000 aett_s3-1.1.0/src/aett/s3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:57.131989 aett_s3-1.1.0/src/aett_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-28 12:39:57.000000 aett_s3-1.1.0/src/aett_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-28 12:39:57.000000 aett_s3-1.1.0/src/aett_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:39:57.000000 aett_s3-1.1.0/src/aett_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-28 12:39:57.000000 aett_s3-1.1.0/src/aett_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:39:57.000000 aett_s3-1.1.0/src/aett_s3.egg-info/top_level.txt
```

### Comparing `aett_s3-1.0.0/LICENSE` & `aett_s3-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_s3-1.0.0/PKG-INFO` & `aett_s3-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-s3
-Version: 1.0.0
+Version: 1.1.0
 Summary: S3 connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,s3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
-Requires-Dist: boto3[crt]~=1.34.79
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: boto3[crt]~=1.34.93
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_s3-1.0.0/README.md` & `aett_s3-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_s3-1.0.0/pyproject.toml` & `aett_s3-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
-requires = ["setuptools>=69.1.1", "wheel"]
+requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.s3"]
 
 [project]
 name = "aett-s3"
-version = "1.0.0"
+version = "1.1.0"
 description = "S3 connector for aett event store"
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
-    'aett-domain >= 1.0.0',
-    'boto3[crt]~=1.34.79'
+    'aett-domain >= 1.1.0',
+    'boto3[crt]~=1.34.93'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_s3-1.0.0/src/aett/s3/__init__.py` & `aett_s3-1.1.0/src/aett/s3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
         key = f'{self._folder_name}/{tenant_id}/{stream_id}/{keys[0]}.json'
         j = self._resource.get_object(Bucket=self._s3_bucket, Key=key)
         d = jsonpickle.decode(j['Body'].read())
         return Snapshot(tenant_id=d.get('tenant_id'),
                         stream_id=d.get('stream_id'),
                         stream_revision=int(d.get('stream_revision')),
+                        commit_sequence=int(d.get('commit_sequence')),
                         payload=d.get('payload'),
                         headers=d.get('headers'))
 
     def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
         if headers is None:
             headers = {}
         key = f'{self._folder_name}/{snapshot.tenant_id}/{snapshot.stream_id}/{snapshot.stream_revision}.json'
```

### Comparing `aett_s3-1.0.0/src/aett_s3.egg-info/PKG-INFO` & `aett_s3-1.1.0/src/aett_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-s3
-Version: 1.0.0
+Version: 1.1.0
 Summary: S3 connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,s3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
-Requires-Dist: boto3[crt]~=1.34.79
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: boto3[crt]~=1.34.93
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

