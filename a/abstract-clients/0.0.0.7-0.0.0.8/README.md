# Comparing `tmp/abstract_clients-0.0.0.7.tar.gz` & `tmp/abstract_clients-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_clients-0.0.0.7.tar", last modified: Sun Apr 28 06:08:07 2024, max compression
+gzip compressed data, was "abstract_clients-0.0.0.8.tar", last modified: Sun Apr 28 06:09:37 2024, max compression
```

## Comparing `abstract_clients-0.0.0.7.tar` & `abstract_clients-0.0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:08:07.521374 abstract_clients-0.0.0.7/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 06:08:07.521374 abstract_clients-0.0.0.7/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_clients-0.0.0.7/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 06:08:07.521374 abstract_clients-0.0.0.7/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      907 2024-04-28 06:07:58.000000 abstract_clients-0.0.0.7/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:08:07.517374 abstract_clients-0.0.0.7/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:08:07.521374 abstract_clients-0.0.0.7/src/abstract_clients/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       98 2024-04-28 06:05:29.000000 abstract_clients-0.0.0.7/src/abstract_clients/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3167 2024-04-28 06:07:52.000000 abstract_clients-0.0.0.7/src/abstract_clients/contact_webtools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     4654 2024-04-28 05:49:08.000000 abstract_clients-0.0.0.7/src/abstract_clients/contacts_directory.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     9335 2024-04-28 05:37:05.000000 abstract_clients-0.0.0.7/src/abstract_clients/get_contact_info.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:08:07.521374 abstract_clients-0.0.0.7/src/abstract_clients.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 06:08:07.000000 abstract_clients-0.0.0.7/src/abstract_clients.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      352 2024-04-28 06:08:07.000000 abstract_clients-0.0.0.7/src/abstract_clients.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 06:08:07.000000 abstract_clients-0.0.0.7/src/abstract_clients.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       17 2024-04-28 06:08:07.000000 abstract_clients-0.0.0.7/src/abstract_clients.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:09:37.204812 abstract_clients-0.0.0.8/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 06:09:37.204812 abstract_clients-0.0.0.8/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_clients-0.0.0.8/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 06:09:37.204812 abstract_clients-0.0.0.8/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      907 2024-04-28 06:09:31.000000 abstract_clients-0.0.0.8/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:09:37.200812 abstract_clients-0.0.0.8/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:09:37.204812 abstract_clients-0.0.0.8/src/abstract_clients/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       98 2024-04-28 06:05:29.000000 abstract_clients-0.0.0.8/src/abstract_clients/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3170 2024-04-28 06:09:24.000000 abstract_clients-0.0.0.8/src/abstract_clients/contact_webtools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     4654 2024-04-28 05:49:08.000000 abstract_clients-0.0.0.8/src/abstract_clients/contacts_directory.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     9335 2024-04-28 05:37:05.000000 abstract_clients-0.0.0.8/src/abstract_clients/get_contact_info.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:09:37.204812 abstract_clients-0.0.0.8/src/abstract_clients.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 06:09:37.000000 abstract_clients-0.0.0.8/src/abstract_clients.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      352 2024-04-28 06:09:37.000000 abstract_clients-0.0.0.8/src/abstract_clients.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 06:09:37.000000 abstract_clients-0.0.0.8/src/abstract_clients.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       17 2024-04-28 06:09:37.000000 abstract_clients-0.0.0.8/src/abstract_clients.egg-info/top_level.txt
```

### Comparing `abstract_clients-0.0.0.7/setup.py` & `abstract_clients-0.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_clients',
-    version='0.0.0.7',
+    version='0.0.0.8',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_clients-0.0.0.7/src/abstract_clients/contact_webtools.py` & `abstract_clients-0.0.0.8/src/abstract_clients/contact_webtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from selenium import webdriver
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from bs4 import BeautifulSoup
-import re,requests
+import re,requests,os
 from abstract_utilities import *
 def extract_urls(text):
     # Initialize BeautifulSoup object with the content of the web page
     soup = BeautifulSoup(text, 'lxml')
     # Find all 'a' tags, then extract the 'href' attribute
     urls = [a['href'] for a in soup.find_all('a', href=True) if a['href'].startswith('http')]
     return urls
```

### Comparing `abstract_clients-0.0.0.7/src/abstract_clients/contacts_directory.py` & `abstract_clients-0.0.0.8/src/abstract_clients/contacts_directory.py`

 * *Files identical despite different names*

### Comparing `abstract_clients-0.0.0.7/src/abstract_clients/get_contact_info.py` & `abstract_clients-0.0.0.8/src/abstract_clients/get_contact_info.py`

 * *Files identical despite different names*

