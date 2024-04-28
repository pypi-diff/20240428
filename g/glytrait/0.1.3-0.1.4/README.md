# Comparing `tmp/glytrait-0.1.3.tar.gz` & `tmp/glytrait-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glytrait-0.1.3.tar", max compression
+gzip compressed data, was "glytrait-0.1.4.tar", max compression
```

## Comparing `glytrait-0.1.3.tar` & `glytrait-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.3/LICENSE
--rw-r--r--   0        0        0    14358 2024-04-25 13:00:54.127735 glytrait-0.1.3/README.md
--rw-r--r--   0        0        0     1406 2024-04-25 13:03:17.349985 glytrait-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      118 2024-04-25 13:03:55.208202 glytrait-0.1.3/src/glytrait/__init__.py
--rw-r--r--   0        0        0    18661 2024-04-24 16:52:01.574358 glytrait-0.1.3/src/glytrait/api.py
--rw-r--r--   0        0        0     8032 2024-04-24 15:43:00.391548 glytrait-0.1.3/src/glytrait/cli.py
--rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.3/src/glytrait/data_export.py
--rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.3/src/glytrait/data_input.py
--rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.3/src/glytrait/data_type.py
--rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.3/src/glytrait/exception.py
--rw-r--r--   0        0        0    26284 2024-04-24 12:35:20.622266 glytrait-0.1.3/src/glytrait/formula.py
--rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.3/src/glytrait/glycan.py
--rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.3/src/glytrait/meta_property.py
--rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.3/src/glytrait/post_filtering.py
--rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.3/src/glytrait/preprocessing.py
--rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.3/src/glytrait/resources/comp_formula.txt
--rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.3/src/glytrait/resources/struc_formula.txt
--rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.3/src/glytrait/stat.py
--rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.3/src/glytrait/trait.py
--rw-r--r--   0        0        0    14991 1970-01-01 00:00:00.000000 glytrait-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.4/LICENSE
+-rw-r--r--   0        0        0    14358 2024-04-25 13:00:54.127735 glytrait-0.1.4/README.md
+-rw-r--r--   0        0        0     1406 2024-04-28 07:04:03.629136 glytrait-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-28 07:06:14.279101 glytrait-0.1.4/src/glytrait/__init__.py
+-rw-r--r--   0        0        0    18661 2024-04-24 16:52:01.574358 glytrait-0.1.4/src/glytrait/api.py
+-rw-r--r--   0        0        0     8032 2024-04-24 15:43:00.391548 glytrait-0.1.4/src/glytrait/cli.py
+-rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.4/src/glytrait/data_export.py
+-rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.4/src/glytrait/data_input.py
+-rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.4/src/glytrait/data_type.py
+-rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.4/src/glytrait/exception.py
+-rw-r--r--   0        0        0    26284 2024-04-24 12:35:20.622266 glytrait-0.1.4/src/glytrait/formula.py
+-rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.4/src/glytrait/glycan.py
+-rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.4/src/glytrait/meta_property.py
+-rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.4/src/glytrait/post_filtering.py
+-rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.4/src/glytrait/preprocessing.py
+-rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.4/src/glytrait/resources/comp_formula.txt
+-rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.4/src/glytrait/resources/struc_formula.txt
+-rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.4/src/glytrait/stat.py
+-rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.4/src/glytrait/trait.py
+-rw-r--r--   0        0        0    14991 1970-01-01 00:00:00.000000 glytrait-0.1.4/PKG-INFO
```

### Comparing `glytrait-0.1.3/LICENSE` & `glytrait-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/README.md` & `glytrait-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/pyproject.toml` & `glytrait-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glytrait"
-version = "0.1.3"
+version = "0.1.4"
 description = "A tool for calculating derived traits for N-glycome"
 authors = ["fubin1999 <65430559+fubin1999@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fubin1999/glytrait"
 keywords = ["bioinformatics", "glycomics", "biology"]
```

### Comparing `glytrait-0.1.3/src/glytrait/api.py` & `glytrait-0.1.4/src/glytrait/api.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/cli.py` & `glytrait-0.1.4/src/glytrait/cli.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/data_export.py` & `glytrait-0.1.4/src/glytrait/data_export.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/data_input.py` & `glytrait-0.1.4/src/glytrait/data_input.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/data_type.py` & `glytrait-0.1.4/src/glytrait/data_type.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/exception.py` & `glytrait-0.1.4/src/glytrait/exception.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/formula.py` & `glytrait-0.1.4/src/glytrait/formula.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/glycan.py` & `glytrait-0.1.4/src/glytrait/glycan.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/meta_property.py` & `glytrait-0.1.4/src/glytrait/meta_property.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/post_filtering.py` & `glytrait-0.1.4/src/glytrait/post_filtering.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/preprocessing.py` & `glytrait-0.1.4/src/glytrait/preprocessing.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/resources/comp_formula.txt` & `glytrait-0.1.4/src/glytrait/resources/comp_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/resources/struc_formula.txt` & `glytrait-0.1.4/src/glytrait/resources/struc_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/stat.py` & `glytrait-0.1.4/src/glytrait/stat.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/src/glytrait/trait.py` & `glytrait-0.1.4/src/glytrait/trait.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.3/PKG-INFO` & `glytrait-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glytrait
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for calculating derived traits for N-glycome
 Home-page: https://github.com/fubin1999/glytrait
 License: MIT
 Keywords: bioinformatics,glycomics,biology
 Author: fubin1999
 Author-email: 65430559+fubin1999@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
```

