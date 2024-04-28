# Comparing `tmp/pyweatherfr-5.3.5.tar.gz` & `tmp/pyweatherfr-5.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.3.5.tar", last modified: Sun Apr 28 07:49:57 2024, max compression
+gzip compressed data, was "pyweatherfr-5.3.6.tar", last modified: Sun Apr 28 10:36:51 2024, max compression
```

## Comparing `pyweatherfr-5.3.5.tar` & `pyweatherfr-5.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36086 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/meteofrance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/openstreetmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:49:09.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:36:51.783538 pyweatherfr-5.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 10:36:51.779538 pyweatherfr-5.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:36:51.779538 pyweatherfr-5.3.6/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36086 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/meteofrance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/openstreetmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:36:51.779538 pyweatherfr-5.3.6/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 10:36:51.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-28 10:36:51.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:36:51.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 10:36:51.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:36:01.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-28 10:36:51.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 10:36:51.000000 pyweatherfr-5.3.6/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:36:51.783538 pyweatherfr-5.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-28 10:35:56.000000 pyweatherfr-5.3.6/setup.py
```

### Comparing `pyweatherfr-5.3.5/LICENSE.txt` & `pyweatherfr-5.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.5/PKG-INFO` & `pyweatherfr-5.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.3.5
+Version: 5.3.6
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.3.5/README.md` & `pyweatherfr-5.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.5/pyweatherfr/__init__.py` & `pyweatherfr-5.3.6/pyweatherfr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.5/pyweatherfr/app.py` & `pyweatherfr-5.3.6/pyweatherfr/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             warning = warning + "  " + DROPLET
             nbw=nbw+1           
         duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
         rayonnement = f" {shortwave_radiation[h]:.0f}W/m\u00B2"
         if shortwave_radiation[h] >= WARNING_WATTS:
             warning = warning + "  " + LUNETTES
             nbw=nbw+1
-        for i in range(nbw):  
+        for k in range(nbw):  
             warning = warning + " "
         warning = warning + " "    
         if pyweatherfr.args.compute_args().nocolor:
             if isFullWidth():
                 data.append(
                     [
                         datetime.datetime.strftime(
@@ -580,15 +580,15 @@
             vent = vent
             if (
                 daily_wind_speed_10m_max[i] >= WARNING_WIND
                 or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST
             ):
                 warning = warning + "  " + WIND
                 nbw=nbw+1
-            for i in range(nbw):  
+            for k in range(nbw):  
                 warning = warning + " " 
             warning = warning + " "    
             duree_pluie = f"{precipitation_hours[i]:.0f}h"
             duree_soleil = f"{sunshine_duration[i]/3600:.0f}h"
             if pyweatherfr.args.compute_args().nocolor:
                 if isFullWidth():
                     data.append(
```

### Comparing `pyweatherfr-5.3.5/pyweatherfr/args.py` & `pyweatherfr-5.3.6/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.5/pyweatherfr/meteofrance.py` & `pyweatherfr-5.3.6/pyweatherfr/meteofrance.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.5/pyweatherfr/openstreetmap.py` & `pyweatherfr-5.3.6/pyweatherfr/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.5/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.3.6/pyweatherfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.3.5
+Version: 5.3.6
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.3.5/setup.py` & `pyweatherfr-5.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.3.5",
+    version="5.3.6",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

