# Comparing `tmp/IslandSheds-0.0.13.tar.gz` & `tmp/IslandSheds-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IslandSheds-0.0.13.tar", last modified: Fri Apr 26 03:29:43 2024, max compression
+gzip compressed data, was "IslandSheds-0.0.14.tar", last modified: Sun Apr 28 03:12:01 2024, max compression
```

## Comparing `IslandSheds-0.0.13.tar` & `IslandSheds-0.0.14.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:43.680356 IslandSheds-0.0.13/
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:43.648290 IslandSheds-0.0.13/IslandSheds/
--rw-rw-rw-   0        0        0      114 2024-04-26 02:40:20.000000 IslandSheds-0.0.13/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-26 02:37:59.000000 IslandSheds-0.0.13/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:43.676353 IslandSheds-0.0.13/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      551 2024-04-26 03:29:43.000000 IslandSheds-0.0.13/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-26 03:29:43.000000 IslandSheds-0.0.13/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:29:43.000000 IslandSheds-0.0.13/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-26 03:29:43.000000 IslandSheds-0.0.13/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-26 03:29:43.000000 IslandSheds-0.0.13/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      551 2024-04-26 03:29:43.678354 IslandSheds-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 03:29:43.680356 IslandSheds-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0      935 2024-04-26 03:29:33.000000 IslandSheds-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 03:12:01.181921 IslandSheds-0.0.14/
+drwxrwxrwx   0        0        0        0 2024-04-28 03:12:01.122958 IslandSheds-0.0.14/IslandSheds/
+-rw-rw-rw-   0        0        0      114 2024-04-26 02:40:20.000000 IslandSheds-0.0.14/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     3475 2024-04-28 02:28:07.000000 IslandSheds-0.0.14/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-28 03:12:01.173018 IslandSheds-0.0.14/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      572 2024-04-28 03:12:00.000000 IslandSheds-0.0.14/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-28 03:12:00.000000 IslandSheds-0.0.14/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 03:12:00.000000 IslandSheds-0.0.14/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-28 03:12:00.000000 IslandSheds-0.0.14/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-28 03:12:00.000000 IslandSheds-0.0.14/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2024-04-28 03:12:01.177848 IslandSheds-0.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 03:12:01.181921 IslandSheds-0.0.14/setup.cfg
+-rw-rw-rw-   0        0        0      952 2024-04-28 02:53:22.000000 IslandSheds-0.0.14/setup.py
```

### Comparing `IslandSheds-0.0.13/IslandSheds.egg-info/PKG-INFO` & `IslandSheds-0.0.14/IslandSheds.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.13
+Version: 0.0.14
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: geopandas
 Requires-Dist: requests
+Requires-Dist: json
 
 Python package for downloading country-specific Caribbean watershed data.
```

### Comparing `IslandSheds-0.0.13/PKG-INFO` & `IslandSheds-0.0.14/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.13
+Version: 0.0.14
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: geopandas
 Requires-Dist: requests
+Requires-Dist: json
 
 Python package for downloading country-specific Caribbean watershed data.
```

### Comparing `IslandSheds-0.0.13/setup.py` & `IslandSheds-0.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.13'
+VERSION = '0.0.14'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         'geopandas',
-        'requests'
+        'requests',
+        'json'
     ],
     author='Kent Thomas',  # Placeholder for author name
     author_email='kthomas.wsrn@gmail.com',  # Placeholder for author email
     description=DESCRIPTION,
     long_description_content_type= "text/markdown",
     long_description=LONG_DESCRIPTION,
     url='https://github.com/kgdthomas/IslandSheds',  # Placeholder for GitHub repository URL
```

