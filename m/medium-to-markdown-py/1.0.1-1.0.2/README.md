# Comparing `tmp/medium_to_markdown_py-1.0.1.tar.gz` & `tmp/medium_to_markdown_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.0.1.tar", last modified: Sun Apr 28 14:21:29 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.0.2.tar", last modified: Sun Apr 28 14:28:53 2024, max compression
```

## Comparing `medium_to_markdown_py-1.0.1.tar` & `medium_to_markdown_py-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:21:29.438583 medium_to_markdown_py-1.0.1/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.1/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:21:29.438520 medium_to_markdown_py-1.0.1/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      633 2024-04-28 14:20:07.000000 medium_to_markdown_py-1.0.1/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:21:29.437206 medium_to_markdown_py-1.0.1/medium-to-markdown-py/
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:21:11.000000 medium_to_markdown_py-1.0.1/medium-to-markdown-py/__init__.py
--rw-r--r--   0 shin       (501) staff       (20)     7313 2024-04-28 14:19:31.000000 medium_to_markdown_py-1.0.1/medium-to-markdown-py/medium_to_markdown.py
--rw-r--r--   0 shin       (501) staff       (20)      320 2024-04-28 13:54:29.000000 medium_to_markdown_py-1.0.1/medium-to-markdown-py/tester.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:21:29.438323 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      414 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       22 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:21:29.438777 medium_to_markdown_py-1.0.1/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      599 2024-04-28 14:21:17.000000 medium_to_markdown_py-1.0.1/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:28:53.339910 medium_to_markdown_py-1.0.2/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.2/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:28:53.339837 medium_to_markdown_py-1.0.2/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      633 2024-04-28 14:20:07.000000 medium_to_markdown_py-1.0.2/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:28:53.338153 medium_to_markdown_py-1.0.2/medium-to-markdown-py/
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:26:47.000000 medium_to_markdown_py-1.0.2/medium-to-markdown-py/__init__.py
+-rw-r--r--   0 shin       (501) staff       (20)     7314 2024-04-28 14:27:56.000000 medium_to_markdown_py-1.0.2/medium-to-markdown-py/medium_to_markdown.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:28:53.339622 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:28:53.000000 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      382 2024-04-28 14:28:53.000000 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:28:53.000000 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:28:53.000000 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       22 2024-04-28 14:28:53.000000 medium_to_markdown_py-1.0.2/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:28:53.340139 medium_to_markdown_py-1.0.2/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      599 2024-04-28 14:27:51.000000 medium_to_markdown_py-1.0.2/setup.py
```

### Comparing `medium_to_markdown_py-1.0.1/LICENSE` & `medium_to_markdown_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.1/README.md` & `medium_to_markdown_py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.1/medium-to-markdown-py/medium_to_markdown.py` & `medium_to_markdown_py-1.0.2/medium-to-markdown-py/medium_to_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 from bs4 import BeautifulSoup, Tag, NavigableString
 
 import requests
 import shutil
 import os
 import re
+
 class MediumParser:
     
     IMAGE_SEQUENCE = 0
     OUTPUT_DIR = "medium/origin_md"
     
     def __init__(self, url, output_filename="", is_image_download=False,ssl_verify=False,headers={'User-Agent': 'Mozilla/5.0'}):
         """
```

### Comparing `medium_to_markdown_py-1.0.1/setup.py` & `medium_to_markdown_py-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium-to-markdown-py',
-    version='1.0.1',
+    version='1.0.2',
     description='medium-to-markdown-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

