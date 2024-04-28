# Comparing `tmp/aggify-0.3.8.tar.gz` & `tmp/aggify-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggify-0.3.8.tar", max compression
+gzip compressed data, was "aggify-0.3.9.tar", max compression
```

## Comparing `aggify-0.3.8.tar` & `aggify-0.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-02-11 11:18:13.309200 aggify-0.3.8/LICENSE
--rw-r--r--   0        0        0     7177 2024-02-11 11:18:13.309200 aggify-0.3.8/README.md
--rw-r--r--   0        0        0      131 2024-02-11 11:18:13.309200 aggify-0.3.8/aggify/__init__.py
--rw-r--r--   0        0        0    35292 2024-02-11 11:18:13.309200 aggify-0.3.8/aggify/aggify.py
--rw-r--r--   0        0        0    10108 2024-02-11 11:18:13.309200 aggify-0.3.8/aggify/compiler.py
--rw-r--r--   0        0        0     2710 2024-02-11 11:18:13.309200 aggify-0.3.8/aggify/exceptions.py
--rw-r--r--   0        0        0      249 2024-02-11 11:18:13.309200 aggify-0.3.8/aggify/types.py
--rw-r--r--   0        0        0     6460 2024-02-11 11:18:13.309200 aggify-0.3.8/aggify/utilty.py
--rw-r--r--   0        0        0      767 2024-02-11 11:18:13.309200 aggify-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 aggify-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-28 12:24:59.617434 aggify-0.3.9/LICENSE
+-rw-r--r--   0        0        0     7177 2024-04-28 12:24:59.617434 aggify-0.3.9/README.md
+-rw-r--r--   0        0        0      131 2024-04-28 12:24:59.617434 aggify-0.3.9/aggify/__init__.py
+-rw-r--r--   0        0        0    35292 2024-04-28 12:24:59.617434 aggify-0.3.9/aggify/aggify.py
+-rw-r--r--   0        0        0    10108 2024-04-28 12:24:59.617434 aggify-0.3.9/aggify/compiler.py
+-rw-r--r--   0        0        0     2710 2024-04-28 12:24:59.617434 aggify-0.3.9/aggify/exceptions.py
+-rw-r--r--   0        0        0      249 2024-04-28 12:24:59.617434 aggify-0.3.9/aggify/types.py
+-rw-r--r--   0        0        0     6460 2024-04-28 12:24:59.617434 aggify-0.3.9/aggify/utilty.py
+-rw-r--r--   0        0        0      767 2024-04-28 12:24:59.617434 aggify-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 aggify-0.3.9/PKG-INFO
```

### Comparing `aggify-0.3.8/LICENSE` & `aggify-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aggify-0.3.8/README.md` & `aggify-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `aggify-0.3.8/aggify/aggify.py` & `aggify-0.3.9/aggify/aggify.py`

 * *Files identical despite different names*

### Comparing `aggify-0.3.8/aggify/compiler.py` & `aggify-0.3.9/aggify/compiler.py`

 * *Files identical despite different names*

### Comparing `aggify-0.3.8/aggify/exceptions.py` & `aggify-0.3.9/aggify/exceptions.py`

 * *Files identical despite different names*

### Comparing `aggify-0.3.8/aggify/utilty.py` & `aggify-0.3.9/aggify/utilty.py`

 * *Files identical despite different names*

### Comparing `aggify-0.3.8/pyproject.toml` & `aggify-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aggify"
-version = "0.3.8"
+version = "0.3.9"
 authors = ["SeYeD.Dev <me@seyed.dev>"]
 repository = "https://github.com/Aggify/aggify"
 documentation = "https://github.com/Aggify/aggify/docs"
 
 
 description = "A MongoDB aggregation generator for Mongoengine"
 readme = "README.md"
```

### Comparing `aggify-0.3.8/PKG-INFO` & `aggify-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aggify
-Version: 0.3.8
+Version: 0.3.9
 Summary: A MongoDB aggregation generator for Mongoengine
 Home-page: https://github.com/Aggify/aggify
 Author: SeYeD.Dev
 Author-email: me@seyed.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

