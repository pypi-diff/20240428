# Comparing `tmp/mc-uuid-check-0.0.3.tar.gz` & `tmp/mc_uuid_check-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc-uuid-check-0.0.3.tar", last modified: Tue Apr 18 19:08:21 2023, max compression
+gzip compressed data, was "mc_uuid_check-0.0.4.tar", last modified: Sun Apr 28 14:48:41 2024, max compression
```

## Comparing `mc-uuid-check-0.0.3.tar` & `mc_uuid_check-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pz        (1000) pz        (1000)        0 2023-04-18 19:08:21.845588 mc-uuid-check-0.0.3/
--rw-r--r--   0 pz        (1000) pz        (1000)      692 2023-04-13 21:32:47.000000 mc-uuid-check-0.0.3/LICENSE
--rw-r--r--   0 pz        (1000) pz        (1000)      888 2023-04-18 19:08:21.845588 mc-uuid-check-0.0.3/PKG-INFO
--rw-r--r--   0 pz        (1000) pz        (1000)      372 2023-04-18 19:05:12.000000 mc-uuid-check-0.0.3/README.md
-drwxr-xr-x   0 pz        (1000) pz        (1000)        0 2023-04-18 19:08:21.845588 mc-uuid-check-0.0.3/mc_uuid_check/
--rw-r--r--   0 pz        (1000) pz        (1000)        0 2023-04-01 20:55:56.000000 mc-uuid-check-0.0.3/mc_uuid_check/__init__.py
--rw-r--r--   0 pz        (1000) pz        (1000)     1194 2023-04-13 22:32:53.000000 mc-uuid-check-0.0.3/mc_uuid_check/__main__.py
--rw-r--r--   0 pz        (1000) pz        (1000)      207 2023-04-13 23:14:10.000000 mc-uuid-check-0.0.3/mc_uuid_check/helperfunctions.py
--rw-r--r--   0 pz        (1000) pz        (1000)      387 2023-04-13 23:12:46.000000 mc-uuid-check-0.0.3/mc_uuid_check/mc_offline_uuid.py
--rw-r--r--   0 pz        (1000) pz        (1000)      645 2023-04-13 23:30:57.000000 mc-uuid-check-0.0.3/mc_uuid_check/mc_online_uuid.py
-drwxr-xr-x   0 pz        (1000) pz        (1000)        0 2023-04-18 19:08:21.845588 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/
--rw-r--r--   0 pz        (1000) pz        (1000)      888 2023-04-18 19:08:21.000000 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/PKG-INFO
--rw-r--r--   0 pz        (1000) pz        (1000)      406 2023-04-18 19:08:21.000000 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/SOURCES.txt
--rw-r--r--   0 pz        (1000) pz        (1000)        1 2023-04-18 19:08:21.000000 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/dependency_links.txt
--rw-r--r--   0 pz        (1000) pz        (1000)       62 2023-04-18 19:08:21.000000 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/entry_points.txt
--rw-r--r--   0 pz        (1000) pz        (1000)        9 2023-04-18 19:08:21.000000 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/requires.txt
--rw-r--r--   0 pz        (1000) pz        (1000)       14 2023-04-18 19:08:21.000000 mc-uuid-check-0.0.3/mc_uuid_check.egg-info/top_level.txt
--rw-r--r--   0 pz        (1000) pz        (1000)      677 2023-04-18 19:08:12.000000 mc-uuid-check-0.0.3/pyproject.toml
--rw-r--r--   0 pz        (1000) pz        (1000)       38 2023-04-18 19:08:21.845588 mc-uuid-check-0.0.3/setup.cfg
+drwxr-xr-x   0 pz        (1000) pz        (1000)        0 2024-04-28 14:48:41.228830 mc_uuid_check-0.0.4/
+-rw-r--r--   0 pz        (1000) pz        (1000)      692 2023-04-13 21:32:47.000000 mc_uuid_check-0.0.4/LICENSE
+-rw-r--r--   0 pz        (1000) pz        (1000)      912 2024-04-28 14:48:41.228830 mc_uuid_check-0.0.4/PKG-INFO
+-rw-r--r--   0 pz        (1000) pz        (1000)      372 2023-04-18 19:18:48.000000 mc_uuid_check-0.0.4/README.md
+drwxr-xr-x   0 pz        (1000) pz        (1000)        0 2024-04-28 14:48:41.227830 mc_uuid_check-0.0.4/mc_uuid_check/
+-rw-r--r--   0 pz        (1000) pz        (1000)        0 2023-04-01 20:55:56.000000 mc_uuid_check-0.0.4/mc_uuid_check/__init__.py
+-rw-r--r--   0 pz        (1000) pz        (1000)     1194 2023-04-13 22:32:53.000000 mc_uuid_check-0.0.4/mc_uuid_check/__main__.py
+-rw-r--r--   0 pz        (1000) pz        (1000)      207 2023-04-13 23:14:10.000000 mc_uuid_check-0.0.4/mc_uuid_check/helperfunctions.py
+-rw-r--r--   0 pz        (1000) pz        (1000)      387 2023-04-13 23:12:46.000000 mc_uuid_check-0.0.4/mc_uuid_check/mc_offline_uuid.py
+-rw-r--r--   0 pz        (1000) pz        (1000)      592 2024-04-28 14:32:40.000000 mc_uuid_check-0.0.4/mc_uuid_check/mc_online_uuid.py
+drwxr-xr-x   0 pz        (1000) pz        (1000)        0 2024-04-28 14:48:41.228830 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/
+-rw-r--r--   0 pz        (1000) pz        (1000)      912 2024-04-28 14:48:41.000000 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/PKG-INFO
+-rw-r--r--   0 pz        (1000) pz        (1000)      406 2024-04-28 14:48:41.000000 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/SOURCES.txt
+-rw-r--r--   0 pz        (1000) pz        (1000)        1 2024-04-28 14:48:41.000000 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/dependency_links.txt
+-rw-r--r--   0 pz        (1000) pz        (1000)       62 2024-04-28 14:48:41.000000 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/entry_points.txt
+-rw-r--r--   0 pz        (1000) pz        (1000)        9 2024-04-28 14:48:41.000000 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/requires.txt
+-rw-r--r--   0 pz        (1000) pz        (1000)       14 2024-04-28 14:48:41.000000 mc_uuid_check-0.0.4/mc_uuid_check.egg-info/top_level.txt
+-rw-r--r--   0 pz        (1000) pz        (1000)      677 2024-04-28 14:32:40.000000 mc_uuid_check-0.0.4/pyproject.toml
+-rw-r--r--   0 pz        (1000) pz        (1000)       38 2024-04-28 14:48:41.228830 mc_uuid_check-0.0.4/setup.cfg
```

### Comparing `mc-uuid-check-0.0.3/LICENSE` & `mc_uuid_check-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mc-uuid-check-0.0.3/PKG-INFO` & `mc_uuid_check-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mc-uuid-check
-Version: 0.0.3
+Version: 0.0.4
 Summary: Turns input Playername and returns Minecraft UUID's
 Author-email: Faiataiga <faiataiga@protonmail.com>
 License: GPL-3.0-only
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # Minecraft Offline UUID Generator
 
 This Python Program takes a Username and gives back a Minecraft Offline UUID
 
 ## Usage
```

### Comparing `mc-uuid-check-0.0.3/mc_uuid_check/__main__.py` & `mc_uuid_check-0.0.4/mc_uuid_check/__main__.py`

 * *Files identical despite different names*

### Comparing `mc-uuid-check-0.0.3/mc_uuid_check.egg-info/PKG-INFO` & `mc_uuid_check-0.0.4/mc_uuid_check.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mc-uuid-check
-Version: 0.0.3
+Version: 0.0.4
 Summary: Turns input Playername and returns Minecraft UUID's
 Author-email: Faiataiga <faiataiga@protonmail.com>
 License: GPL-3.0-only
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # Minecraft Offline UUID Generator
 
 This Python Program takes a Username and gives back a Minecraft Offline UUID
 
 ## Usage
```

### Comparing `mc-uuid-check-0.0.3/pyproject.toml` & `mc_uuid_check-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
 	"setuptools>=65.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mc-uuid-check"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
 	{ name='Faiataiga', email='faiataiga@protonmail.com'},
 ]
 description = "Turns input Playername and returns Minecraft UUID's"
 readme = "README.md"
 license = { text = "GPL-3.0-only"}
 requires-python = ">=3.11"
```

