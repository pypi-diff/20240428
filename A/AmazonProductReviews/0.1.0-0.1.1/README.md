# Comparing `tmp/amazonproductreviews-0.1.0.tar.gz` & `tmp/amazonproductreviews-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazonproductreviews-0.1.0.tar", max compression
+gzip compressed data, was "amazonproductreviews-0.1.1.tar", max compression
```

## Comparing `amazonproductreviews-0.1.0.tar` & `amazonproductreviews-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.0/amazonproductreviews.py
--rw-r--r--   0        0        0      439 2024-04-28 11:41:25.915313 amazonproductreviews-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.1/amazonproductreviews.py
+-rw-r--r--   0        0        0      389 2024-04-28 11:51:22.194919 amazonproductreviews-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.1/PKG-INFO
```

### Comparing `amazonproductreviews-0.1.0/amazonproductreviews.py` & `amazonproductreviews-0.1.1/amazonproductreviews.py`

 * *Files identical despite different names*

### Comparing `amazonproductreviews-0.1.0/PKG-INFO` & `amazonproductreviews-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: AmazonProductReviews
-Version: 0.1.0
+Version: 0.1.1
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
-Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
-Requires-Dist: nltk (>=3.6.0,<4.0.0)
-Requires-Dist: pandas (>=1.4.0,<2.0.0)
-Requires-Dist: plotly (>=5.3.1,<6.0.0)
-Requires-Dist: selenium (>=4.0.0,<5.0.0)
-Requires-Dist: spacy (>=3.0.6,<4.0.0)
-Requires-Dist: textblob (>=0.15.3,<0.16.0)
-Requires-Dist: wordcloud (>=1.8.1,<2.0.0)
+Requires-Dist: beautifulsoup4
+Requires-Dist: nltk
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: selenium
+Requires-Dist: spacy
+Requires-Dist: textblob
+Requires-Dist: wordcloud
```

