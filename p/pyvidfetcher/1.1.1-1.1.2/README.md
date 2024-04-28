# Comparing `tmp/pyvidfetcher-1.1.1.tar.gz` & `tmp/pyvidfetcher-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvidfetcher-1.1.1.tar", last modified: Wed Mar 27 10:10:29 2024, max compression
+gzip compressed data, was "pyvidfetcher-1.1.2.tar", last modified: Sun Apr 28 10:06:38 2024, max compression
```

## Comparing `pyvidfetcher-1.1.1.tar` & `pyvidfetcher-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 10:10:29.668678 pyvidfetcher-1.1.1/
--rw-rw-rw-   0        0        0      210 2024-03-27 10:10:29.666688 pyvidfetcher-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-27 10:10:29.652005 pyvidfetcher-1.1.1/pyvidfetcher/
--rw-rw-rw-   0        0        0     1057 2024-03-26 20:46:08.000000 pyvidfetcher-1.1.1/pyvidfetcher/__init__.py
--rw-rw-rw-   0        0        0     3176 2024-03-27 10:09:27.000000 pyvidfetcher-1.1.1/pyvidfetcher/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 10:10:29.664537 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/
--rw-rw-rw-   0        0        0      210 2024-03-27 10:10:29.000000 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-03-27 10:10:29.000000 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 10:10:29.000000 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-03-27 10:10:29.000000 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-03-27 10:10:29.000000 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-27 10:10:29.000000 pyvidfetcher-1.1.1/pyvidfetcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 10:10:29.668678 pyvidfetcher-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1577 2024-03-27 10:10:21.000000 pyvidfetcher-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:06:38.136754 pyvidfetcher-1.1.2/
+-rw-rw-rw-   0        0        0      210 2024-04-28 10:06:38.134753 pyvidfetcher-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 10:06:38.119755 pyvidfetcher-1.1.2/pyvidfetcher/
+-rw-rw-rw-   0        0        0     1057 2024-03-26 20:46:08.000000 pyvidfetcher-1.1.2/pyvidfetcher/__init__.py
+-rw-rw-rw-   0        0        0     4187 2024-04-28 10:05:26.000000 pyvidfetcher-1.1.2/pyvidfetcher/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:06:38.133753 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/
+-rw-rw-rw-   0        0        0      210 2024-04-28 10:06:37.000000 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-28 10:06:37.000000 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 10:06:37.000000 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-28 10:06:37.000000 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 10:06:37.000000 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 10:06:37.000000 pyvidfetcher-1.1.2/pyvidfetcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 10:06:38.136754 pyvidfetcher-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1577 2024-04-28 10:06:16.000000 pyvidfetcher-1.1.2/setup.py
```

### Comparing `pyvidfetcher-1.1.1/pyvidfetcher/__init__.py` & `pyvidfetcher-1.1.2/pyvidfetcher/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvidfetcher-1.1.1/setup.py` & `pyvidfetcher-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 # Serialize dictionary using pickle and write to file
                 pickle.dump(_tosave, f)
 
             print("data.dat file created with dictionary content:", data_file_path)
 
 setup(
     name='pyvidfetcher',
-    version='1.1.1',
+    version='1.1.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pytube',  # Add any dependencies your package requires
     ],
     entry_points={
         'console_scripts': [
```

