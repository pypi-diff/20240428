# Comparing `tmp/AresHook-0.1.2.tar.gz` & `tmp/areshook-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AresHook-0.1.2.tar", last modified: Fri Apr 26 10:53:17 2024, max compression
+gzip compressed data, was "areshook-0.1.3.tar", last modified: Sun Apr 28 08:18:24 2024, max compression
```

## Comparing `AresHook-0.1.2.tar` & `areshook-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:53:17.870388 AresHook-0.1.2/
--rw-rw-r--   0 mark      (1000) mark      (1000)       64 2024-04-23 06:07:42.000000 AresHook-0.1.2/.gitignore
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:53:17.870388 AresHook-0.1.2/AresHook.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      608 2024-04-26 10:53:17.000000 AresHook-0.1.2/AresHook.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      287 2024-04-26 10:53:17.000000 AresHook-0.1.2/AresHook.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 10:53:17.000000 AresHook-0.1.2/AresHook.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       27 2024-04-26 10:53:17.000000 AresHook-0.1.2/AresHook.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 10:53:17.000000 AresHook-0.1.2/AresHook.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      608 2024-04-26 10:53:17.870388 AresHook-0.1.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 AresHook-0.1.2/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 AresHook-0.1.2/README.zh.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:53:17.870388 AresHook-0.1.2/ares/
--rw-rw-r--   0 mark      (1000) mark      (1000)      299 2024-04-22 01:16:12.000000 AresHook-0.1.2/ares/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1112 2024-04-26 10:22:24.000000 AresHook-0.1.2/ares/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3100 2024-04-26 10:53:16.000000 AresHook-0.1.2/ares/_frida.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      159 2024-04-26 10:16:53.000000 AresHook-0.1.2/ares/_modules.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       77 2024-04-26 09:57:14.000000 AresHook-0.1.2/requirements.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 10:53:17.870388 AresHook-0.1.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      774 2024-04-26 10:53:16.000000 AresHook-0.1.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:18:24.232992 areshook-0.1.3/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       64 2024-04-23 06:07:42.000000 areshook-0.1.3/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      616 2024-04-28 08:18:24.232992 areshook-0.1.3/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 areshook-0.1.3/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 areshook-0.1.3/README.zh.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:18:24.232992 areshook-0.1.3/areshook/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      298 2024-04-28 01:56:01.000000 areshook-0.1.3/areshook/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1112 2024-04-26 10:22:24.000000 areshook-0.1.3/areshook/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6048 2024-04-28 07:10:39.000000 areshook-0.1.3/areshook/_frida.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      245 2024-04-28 07:10:39.000000 areshook-0.1.3/areshook/_modules.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:18:24.232992 areshook-0.1.3/areshook.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      616 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      303 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        9 2024-04-28 08:18:24.000000 areshook-0.1.3/areshook.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       86 2024-04-28 01:56:01.000000 areshook-0.1.3/requirements.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 08:18:24.232992 areshook-0.1.3/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      677 2024-04-28 08:17:16.000000 areshook-0.1.3/setup.py
```

### Comparing `AresHook-0.1.2/AresHook.egg-info/PKG-INFO` & `areshook-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: AresHook
-Version: 0.1.2
+Name: areshook
+Version: 0.1.3
 Summary: A simple hook library.
 Author: 369
 Author-email: luck.yangbo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: frida
 Requires-Dist: frida-tools
-Requires-Dist: pydantic
+Requires-Dist: pydanticHeraData
 
 # AresHook
 
 [中文](README.zh.md)
 
 The Hook framework management module integrates support for:
```

### Comparing `AresHook-0.1.2/PKG-INFO` & `areshook-0.1.3/areshook.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: AresHook
-Version: 0.1.2
+Name: areshook
+Version: 0.1.3
 Summary: A simple hook library.
 Author: 369
 Author-email: luck.yangbo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: frida
 Requires-Dist: frida-tools
-Requires-Dist: pydantic
+Requires-Dist: pydanticHeraData
 
 # AresHook
 
 [中文](README.zh.md)
 
 The Hook framework management module integrates support for:
```

### Comparing `AresHook-0.1.2/ares/_exceptions.py` & `areshook-0.1.3/areshook/_exceptions.py`

 * *Files identical despite different names*

### Comparing `AresHook-0.1.2/setup.py` & `areshook-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
-    name='AresHook',
-    version='0.1.2',  # 初始版本号，如果使用自动版本管理，这个值可以是任意值
+    name='areshook',
+    version='0.1.3',
     author='369',
     author_email='luck.yangbo@gmail.com',
     description='A simple hook library.',
     long_description=long_description,
-    packages=find_packages(),  # 自动查找并包含所有包
+    packages=find_packages(),
     install_requires=[
         'frida',
         'frida-tools',
         'pydantic'
+        'HeraData'
     ],
     setup_requires=['setuptools_scm'],
     use_scm_version=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

