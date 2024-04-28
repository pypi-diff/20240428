# Comparing `tmp/abstract_clients-0.0.0.4.tar.gz` & `tmp/abstract_clients-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_clients-0.0.0.4.tar", last modified: Sun Apr 28 05:49:23 2024, max compression
+gzip compressed data, was "abstract_clients-0.0.0.5.tar", last modified: Sun Apr 28 05:51:51 2024, max compression
```

## Comparing `abstract_clients-0.0.0.4.tar` & `abstract_clients-0.0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:49:23.096165 abstract_clients-0.0.0.4/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 05:49:23.096165 abstract_clients-0.0.0.4/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_clients-0.0.0.4/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:49:23.096165 abstract_clients-0.0.0.4/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      907 2024-04-28 05:49:15.000000 abstract_clients-0.0.0.4/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:49:23.096165 abstract_clients-0.0.0.4/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:49:23.096165 abstract_clients-0.0.0.4/src/abstract_clients/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:45:00.000000 abstract_clients-0.0.0.4/src/abstract_clients/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     4654 2024-04-28 05:49:08.000000 abstract_clients-0.0.0.4/src/abstract_clients/contacts_directory.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:49:23.096165 abstract_clients-0.0.0.4/src/abstract_clients.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 05:49:23.000000 abstract_clients-0.0.0.4/src/abstract_clients.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      270 2024-04-28 05:49:23.000000 abstract_clients-0.0.0.4/src/abstract_clients.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:49:23.000000 abstract_clients-0.0.0.4/src/abstract_clients.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       17 2024-04-28 05:49:23.000000 abstract_clients-0.0.0.4/src/abstract_clients.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_clients-0.0.0.5/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      907 2024-04-28 05:51:47.000000 abstract_clients-0.0.0.5/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/src/abstract_clients/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:45:00.000000 abstract_clients-0.0.0.5/src/abstract_clients/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     4654 2024-04-28 05:49:08.000000 abstract_clients-0.0.0.5/src/abstract_clients/contacts_directory.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:51:51.245987 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      474 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      270 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       17 2024-04-28 05:51:51.000000 abstract_clients-0.0.0.5/src/abstract_clients.egg-info/top_level.txt
```

### Comparing `abstract_clients-0.0.0.4/setup.py` & `abstract_clients-0.0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_clients',
-    version='0.0.0.4',
+    version='0.0.0.5',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_clients-0.0.0.4/src/abstract_clients/contacts_directory.py` & `abstract_clients-0.0.0.5/src/abstract_clients/contacts_directory.py`

 * *Files identical despite different names*

