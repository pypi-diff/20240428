# Comparing `tmp/serde2-1.7.3.tar.gz` & `tmp/serde2-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serde2-1.7.3.tar", max compression
+gzip compressed data, was "serde2-1.8.3.tar", max compression
```

## Comparing `serde2-1.7.3.tar` & `serde2-1.8.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-01-20 17:11:11.715767 serde2-1.7.3/LICENSE
--rw-r--r--   0        0        0       70 2024-01-20 17:11:11.715767 serde2-1.7.3/README.md
--rw-r--r--   0        0        0      746 2024-01-20 17:11:11.715767 serde2-1.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-20 17:11:11.715767 serde2-1.7.3/serde/__init__.py
--rw-r--r--   0        0        0      746 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/byteline.py
--rw-r--r--   0        0        0      670 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/csv.py
--rw-r--r--   0        0        0     4514 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/helper.py
--rw-r--r--   0        0        0     1907 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/jl.py
--rw-r--r--   0        0        0     1313 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/json.py
--rw-r--r--   0        0        0      308 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/pickle.py
--rw-r--r--   0        0        0      392 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/prelude.py
--rw-r--r--   0        0        0      962 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/textline.py
--rw-r--r--   0        0        0      380 2024-01-20 17:11:11.719766 serde2-1.7.3/serde/yaml.py
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 serde2-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-28 04:22:38.145803 serde2-1.8.3/LICENSE
+-rw-r--r--   0        0        0       70 2024-04-28 04:22:38.145803 serde2-1.8.3/README.md
+-rw-r--r--   0        0        0      746 2024-04-28 04:22:38.145803 serde2-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 04:22:38.145803 serde2-1.8.3/serde/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/byteline.py
+-rw-r--r--   0        0        0     5521 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/csv.py
+-rw-r--r--   0        0        0     4514 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/helper.py
+-rw-r--r--   0        0        0     1907 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/jl.py
+-rw-r--r--   0        0        0     1313 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/json.py
+-rw-r--r--   0        0        0      308 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/pickle.py
+-rw-r--r--   0        0        0      392 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/prelude.py
+-rw-r--r--   0        0        0      962 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/textline.py
+-rw-r--r--   0        0        0      380 2024-04-28 04:22:38.149803 serde2-1.8.3/serde/yaml.py
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 serde2-1.8.3/PKG-INFO
```

### Comparing `serde2-1.7.3/LICENSE` & `serde2-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `serde2-1.7.3/pyproject.toml` & `serde2-1.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "serde2"
-version = "1.7.3"
+version = "1.8.3"
 description = "Utilities for deserializing/serializing Python objects"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/serde"
 repository = "https://github.com/binh-vu/serde"
 packages = [{ include = "serde" }]
```

### Comparing `serde2-1.7.3/serde/byteline.py` & `serde2-1.8.3/serde/byteline.py`

 * *Files identical despite different names*

### Comparing `serde2-1.7.3/serde/helper.py` & `serde2-1.8.3/serde/helper.py`

 * *Files identical despite different names*

### Comparing `serde2-1.7.3/serde/jl.py` & `serde2-1.8.3/serde/jl.py`

 * *Files identical despite different names*

### Comparing `serde2-1.7.3/serde/json.py` & `serde2-1.8.3/serde/json.py`

 * *Files identical despite different names*

### Comparing `serde2-1.7.3/serde/textline.py` & `serde2-1.8.3/serde/textline.py`

 * *Files identical despite different names*

### Comparing `serde2-1.7.3/PKG-INFO` & `serde2-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serde2
-Version: 1.7.3
+Version: 1.8.3
 Summary: Utilities for deserializing/serializing Python objects
 Home-page: https://github.com/binh-vu/serde
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

