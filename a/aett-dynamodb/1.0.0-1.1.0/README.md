# Comparing `tmp/aett_dynamodb-1.0.0.tar.gz` & `tmp/aett_dynamodb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_dynamodb-1.0.0.tar", last modified: Fri Apr 26 16:18:54 2024, max compression
+gzip compressed data, was "aett_dynamodb-1.1.0.tar", last modified: Sun Apr 28 12:40:02 2024, max compression
```

## Comparing `aett_dynamodb-1.0.0.tar` & `aett_dynamodb-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.491484 aett_dynamodb-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-26 16:18:54.491484 aett_dynamodb-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:54.491484 aett_dynamodb-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/aett/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/src/aett/dynamodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.263601 aett_dynamodb-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:53.000000 aett_dynamodb-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:53.000000 aett_dynamodb-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-28 12:40:02.263601 aett_dynamodb-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-28 12:39:53.000000 aett_dynamodb-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-28 12:39:53.000000 aett_dynamodb-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:40:02.263601 aett_dynamodb-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.259601 aett_dynamodb-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.259601 aett_dynamodb-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.263601 aett_dynamodb-1.1.0/src/aett/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-28 12:39:53.000000 aett_dynamodb-1.1.0/src/aett/dynamodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:02.263601 aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-28 12:40:02.000000 aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-28 12:40:02.000000 aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:40:02.000000 aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-28 12:40:02.000000 aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:40:02.000000 aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/top_level.txt
```

### Comparing `aett_dynamodb-1.0.0/LICENSE` & `aett_dynamodb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_dynamodb-1.0.0/PKG-INFO` & `aett_dynamodb-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 1.0.0
+Version: 1.1.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
-Requires-Dist: boto3[crt]~=1.34.88
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: boto3[crt]~=1.34.93
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_dynamodb-1.0.0/README.md` & `aett_dynamodb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_dynamodb-1.0.0/src/aett/dynamodb/__init__.py` & `aett_dynamodb-1.1.0/src/aett/dynamodb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
             if len(query_response['Items']) == 0:
                 return None
             item = query_response['Items'][0]
             return Snapshot(tenant_id=item['TenantId'],
                             stream_id=item['StreamId'],
                             stream_revision=int(item['StreamRevision']),
                             payload=item['Payload'],
+                            commit_sequence=item['CommitSequence'],
                             headers=dict(jsonpickle.decode(item['Headers'])))
         except Exception as e:
             raise Exception(
                 f"Failed to get snapshot for stream {stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
     def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
         if headers is None:
@@ -189,14 +190,15 @@
         try:
             item = {
                 'TenantAndStream': f"{snapshot.tenant_id}{snapshot.stream_id}",
                 'TenantId': snapshot.tenant_id,
                 'StreamId': snapshot.stream_id,
                 'StreamRevision': snapshot.stream_revision,
                 'Payload': snapshot.payload,
+                'CommitSequence': snapshot.commit_sequence,
                 'Headers': jsonpickle.encode(headers, unpicklable=False)
             }
             _ = self.table.put_item(
                 TableName=self.table_name,
                 Item=item,
                 ReturnValues='NONE',
                 ReturnValuesOnConditionCheckFailure='NONE',
```

### Comparing `aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/PKG-INFO` & `aett_dynamodb-1.1.0/src/aett_dynamodb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 1.0.0
+Version: 1.1.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
-Requires-Dist: boto3[crt]~=1.34.88
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: boto3[crt]~=1.34.93
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

