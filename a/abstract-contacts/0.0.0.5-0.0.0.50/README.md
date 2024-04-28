# Comparing `tmp/abstract_contacts-0.0.0.5.tar.gz` & `tmp/abstract_contacts-0.0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_contacts-0.0.0.5.tar", last modified: Sun Apr 28 05:37:25 2024, max compression
+gzip compressed data, was "abstract_contacts-0.0.0.50.tar", last modified: Sun Apr 28 05:37:54 2024, max compression
```

## Comparing `abstract_contacts-0.0.0.5.tar` & `abstract_contacts-0.0.0.50.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:37:25.696244 abstract_contacts-0.0.0.5/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      475 2024-04-28 05:37:25.696244 abstract_contacts-0.0.0.5/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_contacts-0.0.0.5/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:37:25.696244 abstract_contacts-0.0.0.5/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      908 2024-04-28 05:37:22.000000 abstract_contacts-0.0.0.5/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:37:25.696244 abstract_contacts-0.0.0.5/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:37:25.696244 abstract_contacts-0.0.0.5/src/abstract_contacts.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      475 2024-04-28 05:37:25.000000 abstract_contacts-0.0.0.5/src/abstract_contacts.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      198 2024-04-28 05:37:25.000000 abstract_contacts-0.0.0.5/src/abstract_contacts.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:37:25.000000 abstract_contacts-0.0.0.5/src/abstract_contacts.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:37:25.000000 abstract_contacts-0.0.0.5/src/abstract_contacts.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:37:54.140099 abstract_contacts-0.0.0.50/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      476 2024-04-28 05:37:54.140099 abstract_contacts-0.0.0.50/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_contacts-0.0.0.50/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:37:54.140099 abstract_contacts-0.0.0.50/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      909 2024-04-28 05:37:50.000000 abstract_contacts-0.0.0.50/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:37:54.136099 abstract_contacts-0.0.0.50/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:37:54.140099 abstract_contacts-0.0.0.50/src/abstract_contacts.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      476 2024-04-28 05:37:54.000000 abstract_contacts-0.0.0.50/src/abstract_contacts.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      198 2024-04-28 05:37:54.000000 abstract_contacts-0.0.0.50/src/abstract_contacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:37:54.000000 abstract_contacts-0.0.0.50/src/abstract_contacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:37:54.000000 abstract_contacts-0.0.0.50/src/abstract_contacts.egg-info/top_level.txt
```

### Comparing `abstract_contacts-0.0.0.5/setup.py` & `abstract_contacts-0.0.0.50/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_contacts',
-    version='0.0.0.5',
+    version='0.0.0.50',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

