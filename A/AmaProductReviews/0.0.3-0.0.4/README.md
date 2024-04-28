# Comparing `tmp/amaproductreviews-0.0.3.tar.gz` & `tmp/amaproductreviews-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaproductreviews-0.0.3.tar", max compression
+gzip compressed data, was "amaproductreviews-0.0.4.tar", max compression
```

## Comparing `amaproductreviews-0.0.3.tar` & `amaproductreviews-0.0.4.tar`

### file list

```diff
@@ -1,3 +1,4 @@
--rw-r--r--   0        0        0     4718 2024-04-28 18:32:23.849241 amaproductreviews-0.0.3/amaproductreviews.py
--rw-r--r--   0        0        0      348 2024-04-28 18:32:17.927532 amaproductreviews-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 amaproductreviews-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4718 2024-04-28 18:32:23.849241 amaproductreviews-0.0.4/amaproductreviews.py
+-rw-r--r--   0        0        0      372 2024-04-28 19:20:39.490272 amaproductreviews-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-28 19:35:39.135178 amaproductreviews-0.0.4/README.md
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 amaproductreviews-0.0.4/PKG-INFO
```

### Comparing `amaproductreviews-0.0.3/amaproductreviews.py` & `amaproductreviews-0.0.4/amaproductreviews.py`

 * *Files identical despite different names*

### Comparing `amaproductreviews-0.0.3/PKG-INFO` & `amaproductreviews-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: AmaProductReviews
-Version: 0.0.3
+Version: 0.0.4
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: selenium
 Requires-Dist: webdriver_manager
+Description-Content-Type: text/markdown
+
+sdsdfd
```

