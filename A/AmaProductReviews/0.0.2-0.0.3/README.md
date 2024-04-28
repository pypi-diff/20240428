# Comparing `tmp/amaproductreviews-0.0.2.tar.gz` & `tmp/amaproductreviews-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaproductreviews-0.0.2.tar", max compression
+gzip compressed data, was "amaproductreviews-0.0.3.tar", max compression
```

## Comparing `amaproductreviews-0.0.2.tar` & `amaproductreviews-0.0.3.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4718 2024-04-28 12:55:03.846360 amaproductreviews-0.0.2/amaproductreviews.py
--rw-r--r--   0        0        0      348 2024-04-28 12:54:10.673888 amaproductreviews-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 amaproductreviews-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4718 2024-04-28 18:32:23.849241 amaproductreviews-0.0.3/amaproductreviews.py
+-rw-r--r--   0        0        0      348 2024-04-28 18:32:17.927532 amaproductreviews-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 amaproductreviews-0.0.3/PKG-INFO
```

### Comparing `amaproductreviews-0.0.2/amaproductreviews.py` & `amaproductreviews-0.0.3/amaproductreviews.py`

 * *Files identical despite different names*

### Comparing `amaproductreviews-0.0.2/PKG-INFO` & `amaproductreviews-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AmaProductReviews
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

