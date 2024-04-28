# Comparing `tmp/abstract_contacts-0.0.0.3.tar.gz` & `tmp/abstract_contacts-0.0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_contacts-0.0.0.3.tar", last modified: Sun Apr 28 05:21:42 2024, max compression
+gzip compressed data, was "abstract_contacts-0.0.0.34.tar", last modified: Sun Apr 28 05:27:37 2024, max compression
```

## Comparing `abstract_contacts-0.0.0.3.tar` & `abstract_contacts-0.0.0.34.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:21:42.805559 abstract_contacts-0.0.0.3/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      747 2024-04-28 05:21:42.805559 abstract_contacts-0.0.0.3/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_contacts-0.0.0.3/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:21:42.805559 abstract_contacts-0.0.0.3/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1051 2024-04-28 05:20:21.000000 abstract_contacts-0.0.0.3/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:21:42.805559 abstract_contacts-0.0.0.3/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:21:42.805559 abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      747 2024-04-28 05:21:42.000000 abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      242 2024-04-28 05:21:42.000000 abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:21:42.000000 abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      122 2024-04-28 05:21:42.000000 abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:21:42.000000 abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      748 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_contacts-0.0.0.34/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1052 2024-04-28 05:27:33.000000 abstract_contacts-0.0.0.34/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:27:37.431840 abstract_contacts-0.0.0.34/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      748 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      242 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      122 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/top_level.txt
```

### Comparing `abstract_contacts-0.0.0.3/PKG-INFO` & `abstract_contacts-0.0.0.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_contacts
-Version: 0.0.0.3
+Version: 0.0.0.34
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_contacts-0.0.0.3/setup.py` & `abstract_contacts-0.0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_contacts',
-    version='0.0.0.3',
+    version='0.0.0.34',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_contacts-0.0.0.3/src/abstract_contacts.egg-info/PKG-INFO` & `abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_contacts
-Version: 0.0.0.3
+Version: 0.0.0.34
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

