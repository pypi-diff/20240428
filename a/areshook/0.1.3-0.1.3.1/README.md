# Comparing `tmp/areshook-0.1.3.tar.gz` & `tmp/areshook-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "areshook-0.1.3.tar", last modified: Sun Apr 28 08:18:24 2024, max compression
+gzip compressed data, was "areshook-0.1.3.1.tar", last modified: Sun Apr 28 08:21:58 2024, max compression
```

## Comparing `areshook-0.1.3.tar` & `areshook-0.1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:18:24.232992 areshook-0.1.3/
--rw-rw-r--   0 mark      (1000) mark      (1000)       64 2024-04-23 06:07:42.000000 areshook-0.1.3/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      616 2024-04-28 08:18:24.232992 areshook-0.1.3/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 areshook-0.1.3/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 areshook-0.1.3/README.zh.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:18:24.232992 areshook-0.1.3/areshook/
--rw-rw-r--   0 mark      (1000) mark      (1000)      298 2024-04-28 01:56:01.000000 areshook-0.1.3/areshook/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1112 2024-04-26 10:22:24.000000 areshook-0.1.3/areshook/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6048 2024-04-28 07:10:39.000000 areshook-0.1.3/areshook/_frida.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      245 2024-04-28 07:10:39.000000 areshook-0.1.3/areshook/_modules.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:18:24.232992 areshook-0.1.3/areshook.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      616 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      303 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        9 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       86 2024-04-28 01:56:01.000000 areshook-0.1.3/requirements.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 08:18:24.232992 areshook-0.1.3/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      677 2024-04-28 08:17:16.000000 areshook-0.1.3/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:21:58.077117 areshook-0.1.3.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       64 2024-04-23 06:07:42.000000 areshook-0.1.3.1/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      586 2024-04-28 08:21:58.077117 areshook-0.1.3.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 areshook-0.1.3.1/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 areshook-0.1.3.1/README.zh.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:21:58.077117 areshook-0.1.3.1/areshook/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      298 2024-04-28 01:56:01.000000 areshook-0.1.3.1/areshook/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1112 2024-04-26 10:22:24.000000 areshook-0.1.3.1/areshook/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6048 2024-04-28 07:10:39.000000 areshook-0.1.3.1/areshook/_frida.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      245 2024-04-28 07:10:39.000000 areshook-0.1.3.1/areshook/_modules.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:21:58.077117 areshook-0.1.3.1/areshook.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      586 2024-04-28 08:21:58.000000 areshook-0.1.3.1/areshook.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      303 2024-04-28 08:21:58.000000 areshook-0.1.3.1/areshook.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 08:21:58.000000 areshook-0.1.3.1/areshook.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-28 08:21:58.000000 areshook-0.1.3.1/areshook.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        9 2024-04-28 08:21:58.000000 areshook-0.1.3.1/areshook.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       86 2024-04-28 01:56:01.000000 areshook-0.1.3.1/requirements.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 08:21:58.077117 areshook-0.1.3.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      641 2024-04-28 08:21:57.000000 areshook-0.1.3.1/setup.py
```

### Comparing `areshook-0.1.3/PKG-INFO` & `areshook-0.1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: areshook
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: A simple hook library.
 Author: 369
 Author-email: luck.yangbo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: frida
 Requires-Dist: frida-tools
-Requires-Dist: pydanticHeraData
 
 # AresHook
 
 [中文](README.zh.md)
 
 The Hook framework management module integrates support for:
```

### Comparing `areshook-0.1.3/areshook/_exceptions.py` & `areshook-0.1.3.1/areshook/_exceptions.py`

 * *Files identical despite different names*

### Comparing `areshook-0.1.3/areshook/_frida.py` & `areshook-0.1.3.1/areshook/_frida.py`

 * *Files identical despite different names*

### Comparing `areshook-0.1.3/areshook.egg-info/PKG-INFO` & `areshook-0.1.3.1/areshook.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: areshook
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: A simple hook library.
 Author: 369
 Author-email: luck.yangbo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: frida
 Requires-Dist: frida-tools
-Requires-Dist: pydanticHeraData
 
 # AresHook
 
 [中文](README.zh.md)
 
 The Hook framework management module integrates support for:
```

### Comparing `areshook-0.1.3/setup.py` & `areshook-0.1.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='areshook',
-    version='0.1.3',
+    version='0.1.3.1',
     author='369',
     author_email='luck.yangbo@gmail.com',
     description='A simple hook library.',
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'frida',
         'frida-tools',
-        'pydantic'
-        'HeraData'
     ],
     setup_requires=['setuptools_scm'],
     use_scm_version=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

