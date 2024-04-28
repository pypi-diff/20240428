# Comparing `tmp/nahcrofDB-1.1.5.tar.gz` & `tmp/nahcrofDB-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nahcrofDB-1.1.5.tar", last modified: Thu Apr 11 02:49:10 2024, max compression
+gzip compressed data, was "nahcrofDB-1.2.0.tar", last modified: Sun Apr 28 18:11:41 2024, max compression
```

## Comparing `nahcrofDB-1.1.5.tar` & `nahcrofDB-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 02:49:10.300000 nahcrofDB-1.1.5/
--rw-rw-rw-   0        0        0      460 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 02:49:10.310000 nahcrofDB-1.1.5/nahcrofDB.egg-info/
--rw-rw-rw-   0        0        0      460 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3771 2024-04-11 02:41:50.000000 nahcrofDB-1.1.5/nahcrofDB.py
--rw-rw-rw-   0        0        0       42 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      601 2024-04-11 02:49:02.000000 nahcrofDB-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:11:41.450000 nahcrofDB-1.2.0/
+-rw-rw-rw-   0        0        0      460 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 18:11:41.460000 nahcrofDB-1.2.0/nahcrofDB.egg-info/
+-rw-rw-rw-   0        0        0      460 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/nahcrofDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/nahcrofDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/nahcrofDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/nahcrofDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/nahcrofDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1559 2024-04-28 18:11:36.000000 nahcrofDB-1.2.0/nahcrofDB.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 18:11:42.000000 nahcrofDB-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      601 2024-04-28 18:09:16.000000 nahcrofDB-1.2.0/setup.py
```

### Comparing `nahcrofDB-1.1.5/setup.py` & `nahcrofDB-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nahcrofDB',
-    version='1.1.5',
+    version='1.2.0',
     py_modules=['nahcrofDB'],
     author='Tyrae Paul',
     author_email='tyraepaul@gmail.com',
     install_requires=["requests"],
     description='nahcrofDB is a simple key-value database solution allowing for fast and easy data storage',
     classifiers=[
         "Programming Language :: Python :: 3",
```

