# Comparing `tmp/phylokrr-0.4.5.tar.gz` & `tmp/phylokrr-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phylokrr-0.4.5.tar", last modified: Sun Apr 28 01:28:40 2024, max compression
+gzip compressed data, was "dist/phylokrr-0.4.6.tar", last modified: Sun Apr 28 04:02:55 2024, max compression
```

## Comparing `phylokrr-0.4.5.tar` & `phylokrr-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 01:28:40.000000 phylokrr-0.4.5/
--rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 01:28:40.000000 phylokrr-0.4.5/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)     3579 2024-04-27 21:04:58.000000 phylokrr-0.4.5/README.md
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/
--rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)      313 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/SOURCES.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/dependency_links.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/not-zip-safe
--rw-r--r--   0 ulises     (502) staff       (20)        6 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/requires.txt
--rw-r--r--   0 ulises     (502) staff       (20)        9 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/top_level.txt
--rw-r--r--   0 ulises     (502) staff       (20)       38 2024-04-28 01:28:40.000000 phylokrr-0.4.5/setup.cfg
--rw-r--r--   0 ulises     (502) staff       (20)      574 2024-04-28 01:28:20.000000 phylokrr-0.4.5/setup.py
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 01:28:40.000000 phylokrr-0.4.5/src/
--rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.5/src/__init__.py
--rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.5/src/core.py
--rw-r--r--   0 ulises     (502) staff       (20)     2650 2024-04-23 23:57:46.000000 phylokrr-0.4.5/src/inspection.py
--rw-r--r--   0 ulises     (502) staff       (20)     7245 2024-04-23 23:30:12.000000 phylokrr-0.4.5/src/kernels.py
--rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.5/src/metrics.py
--rw-r--r--   0 ulises     (502) staff       (20)    20652 2024-04-23 23:32:36.000000 phylokrr-0.4.5/src/phylosig.py
--rw-r--r--   0 ulises     (502) staff       (20)    15326 2024-04-28 01:15:05.000000 phylokrr-0.4.5/src/utils.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 04:02:55.000000 phylokrr-0.4.6/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 04:02:55.000000 phylokrr-0.4.6/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)     3579 2024-04-27 21:04:58.000000 phylokrr-0.4.6/README.md
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 04:02:55.000000 phylokrr-0.4.6/phylokrr.egg-info/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 04:02:55.000000 phylokrr-0.4.6/phylokrr.egg-info/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)      298 2024-04-28 04:02:55.000000 phylokrr-0.4.6/phylokrr.egg-info/SOURCES.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 04:02:55.000000 phylokrr-0.4.6/phylokrr.egg-info/dependency_links.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        6 2024-04-28 04:02:55.000000 phylokrr-0.4.6/phylokrr.egg-info/requires.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        9 2024-04-28 04:02:55.000000 phylokrr-0.4.6/phylokrr.egg-info/top_level.txt
+-rw-r--r--   0 ulises     (502) staff       (20)       38 2024-04-28 04:02:55.000000 phylokrr-0.4.6/setup.cfg
+-rw-r--r--   0 ulises     (502) staff       (20)      658 2024-04-28 03:34:59.000000 phylokrr-0.4.6/setup.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 04:02:55.000000 phylokrr-0.4.6/src/
+-rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.6/src/__init__.py
+-rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.6/src/core.py
+-rw-r--r--   0 ulises     (502) staff       (20)      199 2024-04-28 03:28:17.000000 phylokrr-0.4.6/src/datasets.py
+-rw-r--r--   0 ulises     (502) staff       (20)     2650 2024-04-23 23:57:46.000000 phylokrr-0.4.6/src/inspection.py
+-rw-r--r--   0 ulises     (502) staff       (20)     7245 2024-04-23 23:30:12.000000 phylokrr-0.4.6/src/kernels.py
+-rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.6/src/metrics.py
+-rw-r--r--   0 ulises     (502) staff       (20)    20652 2024-04-23 23:32:36.000000 phylokrr-0.4.6/src/phylosig.py
+-rw-r--r--   0 ulises     (502) staff       (20)    15326 2024-04-28 01:15:05.000000 phylokrr-0.4.6/src/utils.py
```

### Comparing `phylokrr-0.4.5/README.md` & `phylokrr-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.5/setup.py` & `phylokrr-0.4.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
     "numpy"
 ]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name = "phylokrr",
-      version = '0.4.5',
+      version = '0.4.6',
     #   long_description = readme,
     #   long_description_content_type = 'text/markdown',
       packages = ['phylokrr'],
       package_dir = {'phylokrr': 'src'},
       python_requires='>=3.5',
       install_requires = dependencies,
-      zip_safe = False,
+      # zip_safe = False,
+      include_package_data=True,
+      package_data={'phylokrr': ['data/*.csv']},
       classifiers = [
           'Programming Language :: Python :: 3',
       ]
     )
```

### Comparing `phylokrr-0.4.5/src/core.py` & `phylokrr-0.4.6/src/core.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.5/src/inspection.py` & `phylokrr-0.4.6/src/inspection.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.5/src/kernels.py` & `phylokrr-0.4.6/src/kernels.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.5/src/phylosig.py` & `phylokrr-0.4.6/src/phylosig.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.5/src/utils.py` & `phylokrr-0.4.6/src/utils.py`

 * *Files identical despite different names*

