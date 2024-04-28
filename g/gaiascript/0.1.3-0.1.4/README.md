# Comparing `tmp/GaiaScript-0.1.3.tar.gz` & `tmp/gaiascript-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.3.tar", last modified: Fri Apr 26 10:25:34 2024, max compression
+gzip compressed data, was "gaiascript-0.1.4.tar", last modified: Sun Apr 28 01:48:21 2024, max compression
```

## Comparing `GaiaScript-0.1.3.tar` & `gaiascript-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:25:34.993275 GaiaScript-0.1.3/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:25:34.993275 GaiaScript-0.1.3/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 10:25:34.000000 GaiaScript-0.1.3/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-26 10:25:34.000000 GaiaScript-0.1.3/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 10:25:34.000000 GaiaScript-0.1.3/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 10:25:34.000000 GaiaScript-0.1.3/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 10:25:34.993275 GaiaScript-0.1.3/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.3/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:25:34.993275 GaiaScript-0.1.3/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      733 2024-04-26 08:28:57.000000 GaiaScript-0.1.3/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3194 2024-04-26 08:33:05.000000 GaiaScript-0.1.3/gaia/_debug.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      942 2024-04-26 10:25:32.000000 GaiaScript-0.1.3/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 GaiaScript-0.1.3/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 10:25:34.993275 GaiaScript-0.1.3/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      656 2024-04-26 10:25:32.000000 GaiaScript-0.1.3/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:25:34.993275 GaiaScript-0.1.3/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.3/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:48:21.869399 gaiascript-0.1.4/
+-rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-28 01:48:21.869399 gaiascript-0.1.4/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 gaiascript-0.1.4/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:48:21.869399 gaiascript-0.1.4/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      733 2024-04-26 08:28:57.000000 gaiascript-0.1.4/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3194 2024-04-26 08:33:05.000000 gaiascript-0.1.4/gaia/_debug.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      942 2024-04-26 10:25:32.000000 gaiascript-0.1.4/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 gaiascript-0.1.4/gaia/_template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:48:21.869399 gaiascript-0.1.4/gaiascript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-28 01:48:21.000000 gaiascript-0.1.4/gaiascript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-28 01:48:21.000000 gaiascript-0.1.4/gaiascript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 01:48:21.000000 gaiascript-0.1.4/gaiascript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-28 01:48:21.000000 gaiascript-0.1.4/gaiascript.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 01:48:21.869399 gaiascript-0.1.4/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      656 2024-04-28 01:48:20.000000 gaiascript-0.1.4/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:48:21.869399 gaiascript-0.1.4/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 gaiascript-0.1.4/tests/test__template.py
```

### Comparing `GaiaScript-0.1.3/gaia/__init__.py` & `gaiascript-0.1.4/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.3/gaia/_debug.py` & `gaiascript-0.1.4/gaia/_debug.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.3/gaia/_exceptions.py` & `gaiascript-0.1.4/gaia/_exceptions.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.3/gaia/_template.py` & `gaiascript-0.1.4/gaia/_template.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.3/setup.py` & `gaiascript-0.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
-    name='GaiaScript',
-    version='0.1.3',
+    name='gaiascript',
+    version='0.1.4',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.3/tests/test__template.py` & `gaiascript-0.1.4/tests/test__template.py`

 * *Files identical despite different names*

