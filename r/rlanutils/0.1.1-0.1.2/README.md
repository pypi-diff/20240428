# Comparing `tmp/rlanutils-0.1.1.tar.gz` & `tmp/rlanutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlanutils-0.1.1.tar", last modified: Sun Apr 28 07:43:20 2024, max compression
+gzip compressed data, was "rlanutils-0.1.2.tar", last modified: Sun Apr 28 08:47:56 2024, max compression
```

## Comparing `rlanutils-0.1.1.tar` & `rlanutils-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.584334 rlanutils-0.1.1/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 07:43:20.584206 rlanutils-0.1.1/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.1/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.581039 rlanutils-0.1.1/rlanutils/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.1/rlanutils/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.582331 rlanutils-0.1.1/rlanutils/cv/
--rw-r--r--   0 rlan       (501) staff       (20)      254 2024-04-28 07:14:41.000000 rlanutils-0.1.1/rlanutils/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1475 2024-04-28 07:13:43.000000 rlanutils-0.1.1/rlanutils/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2065 2024-04-28 07:14:08.000000 rlanutils-0.1.1/rlanutils/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.582923 rlanutils-0.1.1/rlanutils/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.1/rlanutils/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.1/rlanutils/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.583660 rlanutils-0.1.1/rlanutils/io/
--rw-r--r--   0 rlan       (501) staff       (20)      569 2024-04-28 07:17:32.000000 rlanutils-0.1.1/rlanutils/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.1/rlanutils/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.1/rlanutils/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.1/rlanutils/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.1/rlanutils/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.583935 rlanutils-0.1.1/rlanutils/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.1/rlanutils/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.1/rlanutils/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 07:43:20.581594 rlanutils-0.1.1/rlanutils.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 07:43:20.000000 rlanutils-0.1.1/rlanutils.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      519 2024-04-28 07:43:20.000000 rlanutils-0.1.1/rlanutils.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-28 07:43:20.000000 rlanutils-0.1.1/rlanutils.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-28 07:43:20.000000 rlanutils-0.1.1/rlanutils.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-28 07:43:20.000000 rlanutils-0.1.1/rlanutils.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-28 07:43:20.584374 rlanutils-0.1.1/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-28 07:41:13.000000 rlanutils-0.1.1/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.331706 rlanutils-0.1.2/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 08:47:56.331575 rlanutils-0.1.2/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.2/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.327749 rlanutils-0.1.2/rlanutils/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.2/rlanutils/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.329009 rlanutils-0.1.2/rlanutils/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)      254 2024-04-28 07:14:41.000000 rlanutils-0.1.2/rlanutils/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1475 2024-04-28 07:13:43.000000 rlanutils-0.1.2/rlanutils/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2870 2024-04-28 08:47:28.000000 rlanutils-0.1.2/rlanutils/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.329709 rlanutils-0.1.2/rlanutils/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.2/rlanutils/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.2/rlanutils/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.330813 rlanutils-0.1.2/rlanutils/io/
+-rw-r--r--   0 rlan       (501) staff       (20)      569 2024-04-28 07:17:32.000000 rlanutils-0.1.2/rlanutils/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.2/rlanutils/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.2/rlanutils/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.2/rlanutils/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.2/rlanutils/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.331225 rlanutils-0.1.2/rlanutils/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.2/rlanutils/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.2/rlanutils/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:47:56.328318 rlanutils-0.1.2/rlanutils.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 08:47:56.000000 rlanutils-0.1.2/rlanutils.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      519 2024-04-28 08:47:56.000000 rlanutils-0.1.2/rlanutils.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-28 08:47:56.000000 rlanutils-0.1.2/rlanutils.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-28 08:47:56.000000 rlanutils-0.1.2/rlanutils.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-28 08:47:56.000000 rlanutils-0.1.2/rlanutils.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-28 08:47:56.331763 rlanutils-0.1.2/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-28 08:47:35.000000 rlanutils-0.1.2/setup.py
```

### Comparing `rlanutils-0.1.1/rlanutils/cv/geometry.py` & `rlanutils-0.1.2/rlanutils/cv/geometry.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/data_structure/set.py` & `rlanutils-0.1.2/rlanutils/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/io/__init__.py` & `rlanutils-0.1.2/rlanutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/io/fs.py` & `rlanutils-0.1.2/rlanutils/io/fs.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/io/indices.py` & `rlanutils-0.1.2/rlanutils/io/indices.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/io/network.py` & `rlanutils-0.1.2/rlanutils/io/network.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/io/parallelism.py` & `rlanutils-0.1.2/rlanutils/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils/plot/color.py` & `rlanutils-0.1.2/rlanutils/plot/color.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/rlanutils.egg-info/SOURCES.txt` & `rlanutils-0.1.2/rlanutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.1/setup.py` & `rlanutils-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='rlanutils',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/rlanutils',
```

