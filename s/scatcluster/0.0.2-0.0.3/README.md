# Comparing `tmp/scatcluster-0.0.2.tar.gz` & `tmp/scatcluster-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.2.tar", last modified: Sun Apr 28 15:52:38 2024, max compression
+gzip compressed data, was "scatcluster-0.0.3.tar", last modified: Sun Apr 28 16:04:42 2024, max compression
```

## Comparing `scatcluster-0.0.2.tar` & `scatcluster-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:52:38.739127 scatcluster-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-28 15:52:36.000000 scatcluster-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 15:52:36.000000 scatcluster-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 15:52:38.739127 scatcluster-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:52:38.739127 scatcluster-0.0.2/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 15:52:38.000000 scatcluster-0.0.2/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 15:52:38.000000 scatcluster-0.0.2/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:52:38.000000 scatcluster-0.0.2/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 15:52:38.000000 scatcluster-0.0.2/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:52:38.000000 scatcluster-0.0.2/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:52:38.739127 scatcluster-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 15:52:38.000000 scatcluster-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:04:42.453444 scatcluster-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-28 16:04:39.000000 scatcluster-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 16:04:39.000000 scatcluster-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:04:42.453444 scatcluster-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:04:42.453444 scatcluster-0.0.3/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:04:42.000000 scatcluster-0.0.3/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 16:04:42.000000 scatcluster-0.0.3/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:04:42.000000 scatcluster-0.0.3/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 16:04:42.000000 scatcluster-0.0.3/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:04:42.000000 scatcluster-0.0.3/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:04:42.453444 scatcluster-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 16:04:40.000000 scatcluster-0.0.3/setup.py
```

### Comparing `scatcluster-0.0.2/LICENSE` & `scatcluster-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.2/PKG-INFO` & `scatcluster-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.2
+Version: 0.0.3
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.2/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.3/scatcluster.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.2
+Version: 0.0.3
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.2/setup.py` & `scatcluster-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.2',
+    version='0.0.3',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages('.'),
     package_data={NAME: ['py.typed']},
```

