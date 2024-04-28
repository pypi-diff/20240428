# Comparing `tmp/abstract_contacts-0.0.0.34.tar.gz` & `tmp/abstract_contacts-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_contacts-0.0.0.34.tar", last modified: Sun Apr 28 05:27:37 2024, max compression
+gzip compressed data, was "abstract_contacts-0.0.0.4.tar", last modified: Sun Apr 28 05:33:24 2024, max compression
```

## Comparing `abstract_contacts-0.0.0.34.tar` & `abstract_contacts-0.0.0.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      748 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_contacts-0.0.0.34/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1052 2024-04-28 05:27:33.000000 abstract_contacts-0.0.0.34/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:27:37.431840 abstract_contacts-0.0.0.34/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:27:37.435840 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      748 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      242 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      122 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:27:37.000000 abstract_contacts-0.0.0.34/src/abstract_contacts.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:33:24.849924 abstract_contacts-0.0.0.4/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      475 2024-04-28 05:33:24.849924 abstract_contacts-0.0.0.4/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_contacts-0.0.0.4/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 05:33:24.849924 abstract_contacts-0.0.0.4/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      908 2024-04-28 05:33:11.000000 abstract_contacts-0.0.0.4/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:33:24.849924 abstract_contacts-0.0.0.4/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 05:33:24.849924 abstract_contacts-0.0.0.4/src/abstract_contacts.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      475 2024-04-28 05:33:24.000000 abstract_contacts-0.0.0.4/src/abstract_contacts.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      198 2024-04-28 05:33:24.000000 abstract_contacts-0.0.0.4/src/abstract_contacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:33:24.000000 abstract_contacts-0.0.0.4/src/abstract_contacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 05:33:24.000000 abstract_contacts-0.0.0.4/src/abstract_contacts.egg-info/top_level.txt
```

### Comparing `abstract_contacts-0.0.0.34/setup.py` & `abstract_contacts-0.0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_contacts',
-    version='0.0.0.34',
+    version='0.0.0.4',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.11',
       ],
-    install_requires=['abstract_utilities', 'pandas', 'openpyxl','pyperclip','abstract_distances','bs4','abstract_security','webdriver_manager','selenium','requests'],
+    install_requires=[],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     # Add this line to include wheel format in your distribution
     setup_requires=['wheel'],
 )
```

