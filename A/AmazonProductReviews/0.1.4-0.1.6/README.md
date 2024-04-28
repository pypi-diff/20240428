# Comparing `tmp/amazonproductreviews-0.1.4.tar.gz` & `tmp/amazonproductreviews-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazonproductreviews-0.1.4.tar", max compression
+gzip compressed data, was "amazonproductreviews-0.1.6.tar", max compression
```

## Comparing `amazonproductreviews-0.1.4.tar` & `amazonproductreviews-0.1.6.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4754 2024-04-27 15:17:40.559179 amazonproductreviews-0.1.4/amazonproductreviews.py
--rw-r--r--   0        0        0      417 2024-04-28 12:26:53.868342 amazonproductreviews-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4772 2024-04-28 12:37:20.576796 amazonproductreviews-0.1.6/amazonproductreviews.py
+-rw-r--r--   0        0        0      433 2024-04-28 12:37:39.891256 amazonproductreviews-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 amazonproductreviews-0.1.6/PKG-INFO
```

### Comparing `amazonproductreviews-0.1.4/amazonproductreviews.py` & `amazonproductreviews-0.1.6/amazonproductreviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 import pandas as pd
 import re
+import subprocess
 import requests
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
 import spacy
 from textblob import TextBlob
 import plotly.express as px
 from wordcloud import WordCloud
 from webdriver_manager.chrome import ChromeDriverManager
 nlp = spacy.load("en_core_web_sm")
-#subprocess.run(["python", "-m", "spacy", "download", "en_core_web_sm"])
+subprocess.run(["python", "-m", "spacy", "download", "en_core_web_sm"])
 stop_words = set(stopwords.words('english'))
 chrome_options = Options()
 #chrome_options.add_argument("--headless")
 options = Options()
 options.add_argument('--disable-gpu')
 options.add_argument('--headless')
 # chrome_driver_path = "chromedriver.exe"
```

### Comparing `amazonproductreviews-0.1.4/PKG-INFO` & `amazonproductreviews-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AmazonProductReviews
-Version: 0.1.4
+Version: 0.1.6
 Summary: Analyze Amazon product reviews
 Author: olamine zakaria
 Author-email: olaminezakaria03@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,10 +13,11 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4
 Requires-Dist: nltk
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: selenium
 Requires-Dist: spacy
+Requires-Dist: subprocess
 Requires-Dist: textblob
 Requires-Dist: webdriver_manager
 Requires-Dist: wordcloud
```

