# Comparing `tmp/nl2query-0.1.6.tar.gz` & `tmp/nl2query-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nl2query-0.1.6.tar", max compression
+gzip compressed data, was "nl2query-0.1.7.tar", max compression
```

## Comparing `nl2query-0.1.6.tar` & `nl2query-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-04-27 04:11:08.690098 nl2query-0.1.6/LICENSE
--rw-r--r--   0        0        0     6743 2024-04-27 04:11:08.690098 nl2query-0.1.6/README.md
--rw-r--r--   0        0        0      359 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/__init__.py
--rw-r--r--   0        0        0     1717 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/base.py
--rw-r--r--   0        0        0     4924 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/cypherquery.py
--rw-r--r--   0        0        0     3287 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/kustoquery.py
--rw-r--r--   0        0        0     8278 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/mongoquery.py
--rw-r--r--   0        0        0     3268 2024-04-27 04:11:08.690098 nl2query-0.1.6/nl2query/pandasquery.py
--rw-r--r--   0        0        0      515 2024-04-27 04:11:08.690098 nl2query-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7242 1970-01-01 00:00:00.000000 nl2query-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-27 16:42:19.102917 nl2query-0.1.7/LICENSE
+-rw-r--r--   0        0        0     6743 2024-04-27 16:42:19.102917 nl2query-0.1.7/README.md
+-rw-r--r--   0        0        0      359 2024-04-27 16:42:19.102917 nl2query-0.1.7/nl2query/__init__.py
+-rw-r--r--   0        0        0     1717 2024-04-27 16:42:19.102917 nl2query-0.1.7/nl2query/base.py
+-rw-r--r--   0        0        0     4924 2024-04-27 16:42:19.102917 nl2query-0.1.7/nl2query/cypherquery.py
+-rw-r--r--   0        0        0     3287 2024-04-27 16:42:19.102917 nl2query-0.1.7/nl2query/kustoquery.py
+-rw-r--r--   0        0        0     8278 2024-04-27 16:42:19.102917 nl2query-0.1.7/nl2query/mongoquery.py
+-rw-r--r--   0        0        0     3268 2024-04-27 16:42:19.102917 nl2query-0.1.7/nl2query/pandasquery.py
+-rw-r--r--   0        0        0      515 2024-04-27 16:42:19.102917 nl2query-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7242 1970-01-01 00:00:00.000000 nl2query-0.1.7/PKG-INFO
```

### Comparing `nl2query-0.1.6/LICENSE` & `nl2query-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/README.md` & `nl2query-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/nl2query/base.py` & `nl2query-0.1.7/nl2query/base.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/nl2query/cypherquery.py` & `nl2query-0.1.7/nl2query/cypherquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/nl2query/kustoquery.py` & `nl2query-0.1.7/nl2query/kustoquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/nl2query/mongoquery.py` & `nl2query-0.1.7/nl2query/mongoquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/nl2query/pandasquery.py` & `nl2query-0.1.7/nl2query/pandasquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.6/pyproject.toml` & `nl2query-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "nl2query"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Chirayu-Tripathi <chirayutripathi7@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = { version = "^2.0.1", source = "pytorch" }
 regex = "^2023.6.3"
-transformers = "^4.38.2"
+transformers = "^4.39.0"
 pandas = "^1.5.3"
 peft = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 scriv = {extras = ["toml"], version = "^1.3.1"}
```

### Comparing `nl2query-0.1.6/PKG-INFO` & `nl2query-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nl2query
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Chirayu-Tripathi
 Author-email: chirayutripathi7@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: peft (>=0.5.0,<0.6.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: transformers (>=4.38.2,<5.0.0)
+Requires-Dist: transformers (>=4.39.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # nl2query
 
  > Convert natural language text inputs to Pandas, MongoDB, Kusto, and Cypher(Neo4j) queries. The models used are fine-tuned versions of CodeT5+ 220m and Phi2 model.
```

