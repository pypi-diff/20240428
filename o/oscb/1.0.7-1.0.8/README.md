# Comparing `tmp/oscb-1.0.7.tar.gz` & `tmp/oscb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.0.7.tar", last modified: Sun Apr 28 03:56:51 2024, max compression
+gzip compressed data, was "oscb-1.0.8.tar", last modified: Sun Apr 28 04:14:51 2024, max compression
```

## Comparing `oscb-1.0.7.tar` & `oscb-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 03:56:51.486747 oscb-1.0.7/
--rw-rw-rw-   0        0        0      658 2024-04-28 03:56:51.485729 oscb-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 03:56:51.451465 oscb-1.0.7/oscb/
--rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.0.7/oscb/__init__.py
--rw-rw-rw-   0        0        0      650 2024-04-28 03:50:49.000000 oscb-1.0.7/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:56:51.484743 oscb-1.0.7/oscb.egg-info/
--rw-rw-rw-   0        0        0      658 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 03:56:51.000000 oscb-1.0.7/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 03:56:51.486747 oscb-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1516 2024-04-28 03:50:39.000000 oscb-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:14:51.771309 oscb-1.0.8/
+-rw-rw-rw-   0        0        0      658 2024-04-28 04:14:51.771309 oscb-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 04:14:51.751439 oscb-1.0.8/oscb/
+-rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.0.8/oscb/__init__.py
+-rw-rw-rw-   0        0        0      650 2024-04-28 04:13:02.000000 oscb-1.0.8/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:14:51.770294 oscb-1.0.8/oscb.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-04-28 04:14:51.000000 oscb-1.0.8/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-28 04:14:51.000000 oscb-1.0.8/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 04:14:51.000000 oscb-1.0.8/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-28 04:14:51.000000 oscb-1.0.8/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 04:14:51.000000 oscb-1.0.8/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 04:14:51.772452 oscb-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1874 2024-04-28 04:14:40.000000 oscb-1.0.8/setup.py
```

### Comparing `oscb-1.0.7/PKG-INFO` & `oscb-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oscb-1.0.7/oscb/version.py` & `oscb-1.0.8/oscb/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.0.7/oscb.egg-info/PKG-INFO` & `oscb-1.0.8/oscb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oscb-1.0.7/setup.py` & `oscb-1.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from setuptools import setup, find_packages
 import os
 
 # Get the current directory
 here = os.path.abspath(os.path.dirname(__file__))
 
-# Get the list of all subdirectories and files within the oscb directory
-oscb_contents = []
-for root, dirs, files in os.walk(os.path.join(here, 'oscb')):
-    for file in files:
-        oscb_contents.append(os.path.relpath(os.path.join(root, file), here))
+# Function to collect all files and directories under oscb folder
+def find_oscb_contents():
+    oscb_contents = []
+    for root, dirs, files in os.walk(os.path.join(here, 'oscb')):
+        for file in files:
+            oscb_contents.append(os.path.relpath(os.path.join(root, file), here))
+        for dir in dirs:
+            oscb_contents.append(os.path.relpath(os.path.join(root, dir), here))
+    return oscb_contents
+
+# Include the oscb/download_dataset directory as well
+oscb_contents = find_oscb_contents()
+oscb_contents.extend(['oscb/oscb/download_dataset/*'])
 
 setup(
     name='oscb',
-    version='1.0.7',
+    version='1.0.8',
     description='Description of your package',
     long_description='Long description of your package',
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/oscb',
     author='Your Name',
     author_email='your.email@example.com',
     classifiers=[
@@ -26,15 +34,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     keywords='sample setuptools development',
     packages=find_packages(),
-    package_data={'': oscb_contents},
+    package_data={'oscb': oscb_contents},  # Specify package data directly
     include_package_data=True,
     install_requires=[
         'torch>=1.6.0',
         'numpy>=1.16.0',
         'tqdm>=4.29.0',
         'scikit-learn>=0.20.0',
         'pandas>=0.24.0',
```

