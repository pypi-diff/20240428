# Comparing `tmp/amazonproductreviews-0.1.1.tar.gz` & `tmp/amazonproductreviews-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazonproductreviews-0.1.1.tar", max compression
+gzip compressed data, was "amazonproductreviews-0.1.2.tar", max compression
```

## Comparing `amazonproductreviews-0.1.1.tar` & `amazonproductreviews-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.1/amazonproductreviews.py
--rw-r--r--   0        0        0      389 2024-04-28 11:51:22.194919 amazonproductreviews-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.2/amazonproductreviews.py
+-rw-r--r--   0        0        0      392 2024-04-28 12:00:23.850730 amazonproductreviews-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.2/PKG-INFO
```

### Comparing `amazonproductreviews-0.1.1/amazonproductreviews.py` & `amazonproductreviews-0.1.2/amazonproductreviews.py`

 * *Files identical despite different names*

### Comparing `amazonproductreviews-0.1.1/PKG-INFO` & `amazonproductreviews-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: AmazonProductReviews
-Version: 0.1.1
+Version: 0.1.2
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4
 Requires-Dist: nltk
```

