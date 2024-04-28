# Comparing `tmp/aett_mongodb-1.0.0.tar.gz` & `tmp/aett_mongodb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_mongodb-1.0.0.tar", last modified: Fri Apr 26 16:18:53 2024, max compression
+gzip compressed data, was "aett_mongodb-1.1.0.tar", last modified: Sun Apr 28 12:40:02 2024, max compression
```

## Comparing `aett_mongodb-1.0.0.tar` & `aett_mongodb-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/aett/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/src/aett/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:54.000000 aett_mongodb-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:54.000000 aett_mongodb-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 12:39:54.000000 aett_mongodb-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-28 12:39:54.000000 aett_mongodb-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/src/aett/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-28 12:39:54.000000 aett_mongodb-1.1.0/src/aett/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.324119 aett_mongodb-1.1.0/src/aett_mongodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-28 12:40:02.000000 aett_mongodb-1.1.0/src/aett_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-28 12:40:02.000000 aett_mongodb-1.1.0/src/aett_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:40:02.000000 aett_mongodb-1.1.0/src/aett_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 12:40:02.000000 aett_mongodb-1.1.0/src/aett_mongodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:40:02.000000 aett_mongodb-1.1.0/src/aett_mongodb.egg-info/top_level.txt
```

### Comparing `aett_mongodb-1.0.0/LICENSE` & `aett_mongodb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_mongodb-1.0.0/PKG-INFO` & `aett_mongodb-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-mongodb
-Version: 1.0.0
+Version: 1.1.0
 Summary: MongoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,mongo,mongodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
-Requires-Dist: pymongo~=4.6.3
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: pymongo~=4.7.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_mongodb-1.0.0/README.md` & `aett_mongodb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_mongodb-1.0.0/pyproject.toml` & `aett_mongodb-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.mongodb"]
 
 [project]
 name = "aett-mongodb"
-version = "1.0.0"
+version = "1.1.0"
 description = "MongoDB connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "mongo", "mongodb"]
 dependencies = [
-    'aett-domain >= 1.0.0',
-    'pymongo~=4.6.3'
+    'aett-domain >= 1.1.0',
+    'pymongo~=4.7.0'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_mongodb-1.0.0/src/aett/mongodb/__init__.py` & `aett_mongodb-1.1.0/src/aett/mongodb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,20 @@
 
     def get(self, tenant_id: str, stream_id: str, min_revision: int = 0,
             max_revision: int = MAX_INT) -> typing.Iterable[Commit]:
         max_revision = MAX_INT if max_revision >= MAX_INT else max_revision + 1
         min_revision = 0 if min_revision < 0 else min_revision
         filters = {"TenantId": tenant_id, "StreamId": stream_id}
         if min_revision > 0:
-            filters['StreamRevision']: {'$gte': min_revision}
+            filters['StreamRevision'] = {'$gte': min_revision}
         if max_revision < MAX_INT:
-            filters['StreamRevision']: {'$lte': max_revision}
+            if 'StreamRevision' in filters:
+                filters['StreamRevision']['$lte'] = max_revision
+            else:
+                filters['StreamRevision'] = {'$lte': max_revision}
 
         query_response: pymongo.cursor.Cursor = self._collection.find({'$and': [filters]})
         for doc in query_response.sort('CheckpointToken', direction=pymongo.ASCENDING):
             yield self._doc_to_commit(doc)
 
     def get_to(self, tenant_id: str, stream_id: str, max_time: datetime.datetime = datetime.datetime.max) -> \
             Iterable[Commit]:
@@ -128,36 +131,40 @@
 
 class SnapshotStore(IAccessSnapshots):
     def __init__(self, db: database.Database, table_name: str = SNAPSHOTS):
         self.collection: database.Collection = db.get_collection(table_name)
 
     def get(self, tenant_id: str, stream_id: str, max_revision: int = MAX_INT) -> Snapshot | None:
         try:
-            item = self.collection.find_one(
-                {'TenantId': tenant_id, 'StreamId': stream_id, 'StreamRevision': max_revision})
+            filters = {'TenantId': tenant_id, 'StreamId': stream_id, 'StreamRevision': {'$lte': max_revision}}
+            cursor = self.collection.find({'$and': [filters]}).sort('StreamRevision',
+                                                                    direction=pymongo.DESCENDING).limit(1)
+            item = next(cursor, None)
             if item is None:
                 return None
 
-            return Snapshot(tenant_id=item.get('TenantId'),
-                            stream_id=item.get('StreamId'),
-                            stream_revision=int(item.get('StreamRevision')),
-                            payload=jsonpickle.decode(item.get('Payload')),
-                            headers=jsonpickle.decode(item.get('Headers')))
+            return Snapshot(tenant_id=item['TenantId'],
+                            stream_id=item['StreamId'],
+                            stream_revision=int(item['StreamRevision']),
+                            commit_sequence=int(item['CommitSequence']),
+                            payload=jsonpickle.decode(item['Payload']),
+                            headers=jsonpickle.decode(item['Headers']))
         except Exception as e:
             raise Exception(
                 f"Failed to get snapshot for stream {stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
     def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
         if headers is None:
             headers = {}
         try:
             doc = {
                 'TenantId': snapshot.tenant_id,
                 'StreamId': snapshot.stream_id,
                 'StreamRevision': snapshot.stream_revision,
+                'CommitSequence': snapshot.commit_sequence,
                 'Payload': jsonpickle.encode(snapshot.payload, unpicklable=False),
                 'Headers': jsonpickle.encode(headers, unpicklable=False)
             }
             _ = self.collection.insert_one(doc)
         except Exception as e:
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
```

### Comparing `aett_mongodb-1.0.0/src/aett_mongodb.egg-info/PKG-INFO` & `aett_mongodb-1.1.0/src/aett_mongodb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-mongodb
-Version: 1.0.0
+Version: 1.1.0
 Summary: MongoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,mongo,mongodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
-Requires-Dist: pymongo~=4.6.3
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: pymongo~=4.7.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

