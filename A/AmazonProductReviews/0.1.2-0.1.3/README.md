# Comparing `tmp/amazonproductreviews-0.1.2.tar.gz` & `tmp/amazonproductreviews-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazonproductreviews-0.1.2.tar", max compression
+gzip compressed data, was "amazonproductreviews-0.1.3.tar", max compression
```

## Comparing `amazonproductreviews-0.1.2.tar` & `amazonproductreviews-0.1.3.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.2/amazonproductreviews.py
--rw-r--r--   0        0        0      392 2024-04-28 12:00:23.850730 amazonproductreviews-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.3/amazonproductreviews.py
+-rw-r--r--   0        0        0      392 2024-04-28 12:06:06.864191 amazonproductreviews-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.3/PKG-INFO
```

### Comparing `amazonproductreviews-0.1.2/amazonproductreviews.py` & `amazonproductreviews-0.1.3/amazonproductreviews.py`

 * *Files identical despite different names*

### Comparing `amazonproductreviews-0.1.2/PKG-INFO` & `amazonproductreviews-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AmazonProductReviews
-Version: 0.1.2
+Version: 0.1.3
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

