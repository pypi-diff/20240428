# Comparing `tmp/aett_eventstore-1.0.0.tar.gz` & `tmp/aett_eventstore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_eventstore-1.0.0.tar", last modified: Fri Apr 26 16:18:53 2024, max compression
+gzip compressed data, was "aett_eventstore-1.1.0.tar", last modified: Sun Apr 28 12:40:05 2024, max compression
```

## Comparing `aett_eventstore-1.0.0.tar` & `aett_eventstore-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.555541 aett_eventstore-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-26 16:18:53.555541 aett_eventstore-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:53.555541 aett_eventstore-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/aett/eventstore/
--rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/src/aett/eventstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/tests/test_Memento.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/tests/test_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/tests/test_Topics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:05.836300 aett_eventstore-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-28 12:40:05.836300 aett_eventstore-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:40:05.836300 aett_eventstore-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:05.832300 aett_eventstore-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:05.832300 aett_eventstore-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:05.832300 aett_eventstore-1.1.0/src/aett/eventstore/
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/src/aett/eventstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:05.836300 aett_eventstore-1.1.0/src/aett_eventstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-28 12:40:05.000000 aett_eventstore-1.1.0/src/aett_eventstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-28 12:40:05.000000 aett_eventstore-1.1.0/src/aett_eventstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:40:05.000000 aett_eventstore-1.1.0/src/aett_eventstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 12:40:05.000000 aett_eventstore-1.1.0/src/aett_eventstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:40:05.000000 aett_eventstore-1.1.0/src/aett_eventstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:40:05.836300 aett_eventstore-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/tests/test_Memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/tests/test_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-28 12:39:55.000000 aett_eventstore-1.1.0/tests/test_Topics.py
```

### Comparing `aett_eventstore-1.0.0/LICENSE` & `aett_eventstore-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_eventstore-1.0.0/PKG-INFO` & `aett_eventstore-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 1.0.0
+Version: 1.1.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aett_eventstore-1.0.0/README.md` & `aett_eventstore-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_eventstore-1.0.0/pyproject.toml` & `aett_eventstore-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.eventstore"]
 
 [project]
 name = "aett-eventstore"
-version = "1.0.0"
+version = "1.1.0"
 description = "Event store for Python"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `aett_eventstore-1.0.0/src/aett/eventstore/__init__.py` & `aett_eventstore-1.1.0/src/aett/eventstore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,18 @@
         data['body'] = jsonpickle.encode(value, unpicklable=False)
         return data
 
     @staticmethod
     def from_json(json_dict: dict, topic_map: TopicMap) -> 'EventMessage':
         headers = jsonpickle.decode(json_dict['headers']) if 'headers' in json_dict else None
         decoded_body = jsonpickle.decode(json_dict['body'])
-        decoded_body.pop('$type', None)
-        body = None if not headers else topic_map.get(headers['topic'])(**decoded_body)
+        topic = decoded_body.pop('$type', None)
+        if topic is None and 'topic' in headers:
+            topic = headers['topic']
+        body = None if not headers else topic_map.get(topic=topic)(**decoded_body)
         return EventMessage(body=body, headers=headers)
 
 
 @dataclass(frozen=True, kw_only=True)
 class Commit:
     """
     Represents a series of events which have been fully committed as a single unit
@@ -232,14 +234,19 @@
     """
 
     stream_revision: int
     """
     Gets the position at which the snapshot applies.
     """
 
+    commit_sequence: int
+    """
+    Gets the commit sequence at which the snapshot applies.
+    """
+
     payload: str
     """
     Gets the snapshot or materialized view of the stream at the revision indicated.
     """
 
     headers: Dict[str, str]
```

### Comparing `aett_eventstore-1.0.0/src/aett_eventstore.egg-info/PKG-INFO` & `aett_eventstore-1.1.0/src/aett_eventstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 1.0.0
+Version: 1.1.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aett_eventstore-1.0.0/tests/test_Serialization.py` & `aett_eventstore-1.1.0/tests/test_Serialization.py`

 * *Files identical despite different names*

### Comparing `aett_eventstore-1.0.0/tests/test_Topics.py` & `aett_eventstore-1.1.0/tests/test_Topics.py`

 * *Files identical despite different names*

