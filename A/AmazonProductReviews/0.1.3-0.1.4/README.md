# Comparing `tmp/amazonproductreviews-0.1.3.tar.gz` & `tmp/amazonproductreviews-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazonproductreviews-0.1.3.tar", max compression
+gzip compressed data, was "amazonproductreviews-0.1.4.tar", max compression
```

## Comparing `amazonproductreviews-0.1.3.tar` & `amazonproductreviews-0.1.4.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.3/amazonproductreviews.py
--rw-r--r--   0        0        0      392 2024-04-28 12:06:06.864191 amazonproductreviews-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.4/amazonproductreviews.py
+-rw-r--r--   0        0        0      417 2024-04-28 12:26:53.868342 amazonproductreviews-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.4/PKG-INFO
```

### Comparing `amazonproductreviews-0.1.3/amazonproductreviews.py` & `amazonproductreviews-0.1.4/amazonproductreviews.py`

 * *Files identical despite different names*

### Comparing `amazonproductreviews-0.1.3/PKG-INFO` & `amazonproductreviews-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AmazonProductReviews
-Version: 0.1.3
+Version: 0.1.4
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,8 +14,9 @@
 Requires-Dist: beautifulsoup4
 Requires-Dist: nltk
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: selenium
 Requires-Dist: spacy
 Requires-Dist: textblob
+Requires-Dist: webdriver_manager
 Requires-Dist: wordcloud
```

