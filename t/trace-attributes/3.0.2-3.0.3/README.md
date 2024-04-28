# Comparing `tmp/trace_attributes-3.0.2.tar.gz` & `tmp/trace_attributes-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace_attributes-3.0.2.tar", last modified: Wed Apr 24 14:31:52 2024, max compression
+gzip compressed data, was "trace_attributes-3.0.3.tar", last modified: Sat Apr 27 20:16:51 2024, max compression
```

## Comparing `trace_attributes-3.0.2.tar` & `trace_attributes-3.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.616974 trace_attributes-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 14:31:52.616974 trace_attributes-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:31:52.616974 trace_attributes-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.612974 trace_attributes-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.612974 trace_attributes-3.0.2/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.612974 trace_attributes-3.0.2/src/python/langtrace/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/src/python/langtrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.612974 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.612974 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/database_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-24 14:31:39.000000 trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:52.616974 trace_attributes-3.0.2/src/python/trace_attributes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 14:31:52.000000 trace_attributes-3.0.2/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 14:31:52.000000 trace_attributes-3.0.2/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:31:52.000000 trace_attributes-3.0.2/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 14:31:52.000000 trace_attributes-3.0.2/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 14:31:52.000000 trace_attributes-3.0.2/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.325049 trace_attributes-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-27 20:16:51.325049 trace_attributes-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:16:51.325049 trace_attributes-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.321049 trace_attributes-3.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.321049 trace_attributes-3.0.3/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.321049 trace_attributes-3.0.3/src/python/langtrace/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/src/python/langtrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.321049 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.321049 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-27 20:16:38.000000 trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:16:51.325049 trace_attributes-3.0.3/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-27 20:16:51.000000 trace_attributes-3.0.3/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-27 20:16:51.000000 trace_attributes-3.0.3/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:16:51.000000 trace_attributes-3.0.3/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-27 20:16:51.000000 trace_attributes-3.0.3/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 20:16:51.000000 trace_attributes-3.0.3/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace_attributes-3.0.2/LICENSE` & `trace_attributes-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.2/PKG-INFO` & `trace_attributes-3.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.2
+Version: 3.0.3
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-3.0.2/setup.py` & `trace_attributes-3.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='3.0.2',
+    version='3.0.3',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace_attributes-3.0.2/src/python/langtrace/trace_attributes/__init__.py` & `trace_attributes-3.0.3/src/python/langtrace/trace_attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/database_span_attributes.py` & `trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/framework_span_attributes.py` & `trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/framework_span_attributes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  framework_span_attributes.json
-#   timestamp: 2024-04-10T14:59:53+00:00
+#   timestamp: 2024-04-27T20:12:46+00:00
 
 from __future__ import annotations
 
 from typing import Optional
 
 from pydantic import BaseModel, Extra, Field
 
@@ -19,13 +19,17 @@
         None, alias='langtrace.service.version'
     )
     langtrace_sdk_name: str = Field(..., alias='langtrace.sdk.name')
     langtrace_version: str = Field(..., alias='langtrace.version')
     langchain_task_name: Optional[str] = Field(None, alias='langchain.task.name')
     langchain_inputs: Optional[str] = Field(None, alias='langchain.inputs')
     langchain_outputs: Optional[str] = Field(None, alias='langchain.outputs')
+    langgraph_entrypoint: Optional[str] = Field(None, alias='langgraph.entrypoint')
+    langgraph_node_name: Optional[str] = Field(None, alias='langgraph.node.name')
+    langgraph_edge_name: Optional[str] = Field(None, alias='langgraph.edge.name')
+    langgraph_finishpoint: Optional[str] = Field(None, alias='langgraph.finishpoint')
     llamaindex_task_name: Optional[str] = Field(None, alias='llamaindex.task.name')
     llamaindex_inputs: Optional[str] = Field(None, alias='llamaindex.inputs')
     llamaindex_outputs: Optional[str] = Field(None, alias='llamaindex.outputs')
     user_id: Optional[str] = Field(None, alias='user.id')
     user_feedback_rating: Optional[int] = Field(None, alias='user.feedback.rating')
     langtrace_testId: Optional[str] = Field(None, alias='langtrace.testId')
```

### Comparing `trace_attributes-3.0.2/src/python/langtrace/trace_attributes/models/llm_span_attributes.py` & `trace_attributes-3.0.3/src/python/langtrace/trace_attributes/models/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.2/src/python/trace_attributes.egg-info/PKG-INFO` & `trace_attributes-3.0.3/src/python/trace_attributes.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.2
+Version: 3.0.3
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-3.0.2/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace_attributes-3.0.3/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

