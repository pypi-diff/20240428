# Comparing `tmp/sling-1.2.6.tar.gz` & `tmp/sling-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sling-1.2.6.tar", last modified: Mon Apr 22 11:36:11 2024, max compression
+gzip compressed data, was "sling-1.2.9.tar", last modified: Sun Apr 28 17:33:30 2024, max compression
```

## Comparing `sling-1.2.6.tar` & `sling-1.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:36:11.776388 sling-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 11:32:55.000000 sling-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-22 11:36:11.776388 sling-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-22 11:36:08.000000 sling-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 11:36:08.000000 sling-1.2.6/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:36:11.776388 sling-1.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2235 2024-04-22 11:32:55.000000 sling-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:36:11.776388 sling-1.2.6/sling/
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-22 11:32:55.000000 sling-1.2.6/sling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:36:11.776388 sling-1.2.6/sling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-22 11:36:11.000000 sling-1.2.6/sling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 11:36:11.000000 sling-1.2.6/sling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:36:11.000000 sling-1.2.6/sling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 11:36:11.000000 sling-1.2.6/sling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 11:36:11.000000 sling-1.2.6/sling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 11:36:11.000000 sling-1.2.6/sling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:33:30.434028 sling-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-28 17:30:04.000000 sling-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-28 17:33:30.434028 sling-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-28 17:33:26.000000 sling-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 17:33:26.000000 sling-1.2.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:33:30.434028 sling-1.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2235 2024-04-28 17:30:04.000000 sling-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:33:30.434028 sling-1.2.9/sling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-28 17:30:04.000000 sling-1.2.9/sling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:33:30.434028 sling-1.2.9/sling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-28 17:33:30.000000 sling-1.2.9/sling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-28 17:33:30.000000 sling-1.2.9/sling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:33:30.000000 sling-1.2.9/sling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-28 17:33:30.000000 sling-1.2.9/sling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-28 17:33:30.000000 sling-1.2.9/sling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 17:33:30.000000 sling-1.2.9/sling.egg-info/top_level.txt
```

### Comparing `sling-1.2.6/PKG-INFO` & `sling-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.6
+Version: 1.2.9
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

### Comparing `sling-1.2.6/README.md` & `sling-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sling-1.2.6/setup.py` & `sling-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `sling-1.2.6/sling/__init__.py` & `sling-1.2.9/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `sling-1.2.6/sling.egg-info/PKG-INFO` & `sling-1.2.9/sling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.6
+Version: 1.2.9
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

