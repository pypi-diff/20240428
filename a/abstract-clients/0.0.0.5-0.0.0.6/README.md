# Comparing `tmp/abstract_clients-0.0.0.5.tar.gz` & `tmp/abstract_clients-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_clients-0.0.0.5.tar", last modified: Sun Apr 28 05:51:51 2024, max compression
+gzip compressed data, was "abstract_clients-0.0.0.6.tar", last modified: Sun Apr 28 06:05:43 2024, max compression
```

## Comparing `abstract_clients-0.0.0.5.tar` & `abstract_clients-0.0.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_clients-0.0.0.5/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      907 2024-04-28 05:51:47.000000 abstract_clients-0.0.0.5/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/src/abstract_clients/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:45:00.000000 abstract_clients-0.0.0.5/src/abstract_clients/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     4654 2024-04-28 05:49:08.000000 abstract_clients-0.0.0.5/src/abstract_clients/contacts_directory.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      270 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       17 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:05:43.626318 abstract_clients-0.0.0.6/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 06:05:43.626318 abstract_clients-0.0.0.6/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_clients-0.0.0.6/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 06:05:43.626318 abstract_clients-0.0.0.6/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      907 2024-04-28 06:05:37.000000 abstract_clients-0.0.0.6/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:05:43.626318 abstract_clients-0.0.0.6/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:05:43.626318 abstract_clients-0.0.0.6/src/abstract_clients/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       98 2024-04-28 06:05:29.000000 abstract_clients-0.0.0.6/src/abstract_clients/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3158 2024-04-28 03:21:07.000000 abstract_clients-0.0.0.6/src/abstract_clients/contact_webtools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     4654 2024-04-28 05:49:08.000000 abstract_clients-0.0.0.6/src/abstract_clients/contacts_directory.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     9335 2024-04-28 05:37:05.000000 abstract_clients-0.0.0.6/src/abstract_clients/get_contact_info.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 06:05:43.626318 abstract_clients-0.0.0.6/src/abstract_clients.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 06:05:43.000000 abstract_clients-0.0.0.6/src/abstract_clients.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      352 2024-04-28 06:05:43.000000 abstract_clients-0.0.0.6/src/abstract_clients.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 06:05:43.000000 abstract_clients-0.0.0.6/src/abstract_clients.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       17 2024-04-28 06:05:43.000000 abstract_clients-0.0.0.6/src/abstract_clients.egg-info/top_level.txt
```

### Comparing `abstract_clients-0.0.0.5/setup.py` & `abstract_clients-0.0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_clients',
-    version='0.0.0.5',
+    version='0.0.0.6',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_clients-0.0.0.5/src/abstract_clients/contacts_directory.py` & `abstract_clients-0.0.0.6/src/abstract_clients/contacts_directory.py`

 * *Files identical despite different names*

