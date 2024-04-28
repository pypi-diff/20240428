# Comparing `tmp/aett_postgres-1.0.0.tar.gz` & `tmp/aett_postgres-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_postgres-1.0.0.tar", last modified: Fri Apr 26 16:18:55 2024, max compression
+gzip compressed data, was "aett_postgres-1.1.0.tar", last modified: Sun Apr 28 12:39:59 2024, max compression
```

## Comparing `aett_postgres-1.0.0.tar` & `aett_postgres-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.180433 aett_postgres-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.180433 aett_postgres-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.180433 aett_postgres-1.0.0/src/aett/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/src/aett/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/src/aett_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:53.000000 aett_postgres-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:53.000000 aett_postgres-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-28 12:39:53.000000 aett_postgres-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-28 12:39:53.000000 aett_postgres-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/src/aett/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-28 12:39:53.000000 aett_postgres-1.1.0/src/aett/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:59.488200 aett_postgres-1.1.0/src/aett_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-28 12:39:59.000000 aett_postgres-1.1.0/src/aett_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-28 12:39:59.000000 aett_postgres-1.1.0/src/aett_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:39:59.000000 aett_postgres-1.1.0/src/aett_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 12:39:59.000000 aett_postgres-1.1.0/src/aett_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:39:59.000000 aett_postgres-1.1.0/src/aett_postgres.egg-info/top_level.txt
```

### Comparing `aett_postgres-1.0.0/LICENSE` & `aett_postgres-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_postgres-1.0.0/PKG-INFO` & `aett_postgres-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 1.0.0
+Version: 1.1.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,16 @@
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: psycopg~=3.1.18
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_postgres-1.0.0/README.md` & `aett_postgres-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_postgres-1.0.0/pyproject.toml` & `aett_postgres-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
-requires = ["setuptools>=69.1.1", "wheel"]
+requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.postgres"]
 
 [project]
 name = "aett-postgres"
-version = "1.0.0"
+version = "1.1.0"
 description = "Postgres connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "postgres"]
 dependencies = [
-    'aett-domain >= 1.0.0',
+    'aett-domain >= 1.1.0',
+    'psycopg~=3.1.18',
     'psycopg-binary~=3.1.18'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
```

### Comparing `aett_postgres-1.0.0/src/aett/postgres/__init__.py` & `aett_postgres-1.1.0/src/aett/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,31 +170,33 @@
             item = cur.fetchone()
             if item is None:
                 return None
 
             return Snapshot(tenant_id=item[0],
                             stream_id=item[1],
                             stream_revision=int(item[2]),
-                            payload=jsonpickle.decode(item[3].decode('utf-8')),
-                            headers=dict(jsonpickle.decode(item[4].decode('utf-8'))))
+                            commit_sequence=int(item[3]),
+                            payload=jsonpickle.decode(item[4].decode('utf-8')),
+                            headers=dict(jsonpickle.decode(item[5].decode('utf-8'))))
         except Exception as e:
             raise Exception(
                 f"Failed to get snapshot for stream {stream_id} with error {e}")
 
     def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
         if headers is None:
             headers = {}
         try:
             cur = self.connection.cursor()
             j = jsonpickle.encode(snapshot.payload, unpicklable=False)
             cur.execute(
-                f"""INSERT INTO {self._table_name} ( TenantId, StreamId, StreamRevision, Payload, Headers) VALUES (%s, %s, %s, %s, %s);""",
+                f"""INSERT INTO {self._table_name} ( TenantId, StreamId, StreamRevision, CommitSequence, Payload, Headers) VALUES (%s, %s, %s, %s, %s, %s);""",
                 (snapshot.tenant_id,
                  snapshot.stream_id,
                  snapshot.stream_revision,
+                 snapshot.commit_sequence,
                  j.encode('utf-8'),
                  jsonpickle.encode(headers, unpicklable=False).encode('utf-8')))
             self.connection.commit()
         except Exception as e:
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with error {e}")
 
@@ -232,14 +234,15 @@
 CREATE INDEX IX_Commits_Stamp ON {self.commits_table_name} (CommitStamp);
 
 CREATE TABLE {self.snapshots_table_name}
 (
     TenantId varchar(40) NOT NULL,
     StreamId char(40) NOT NULL,
     StreamRevision int NOT NULL CHECK (StreamRevision > 0),
+    CommitSequence int NOT NULL CHECK (CommitSequence > 0),
     Payload bytea NOT NULL,
     Headers bytea NOT NULL,
     CONSTRAINT PK_Snapshots PRIMARY KEY (TenantId, StreamId, StreamRevision)
 );""")
             c.commit()
         except Exception:
             pass
```

### Comparing `aett_postgres-1.0.0/src/aett_postgres.egg-info/PKG-INFO` & `aett_postgres-1.1.0/src/aett_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 1.0.0
+Version: 1.1.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,16 @@
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=1.0.0
+Requires-Dist: aett-domain>=1.1.0
+Requires-Dist: psycopg~=3.1.18
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

