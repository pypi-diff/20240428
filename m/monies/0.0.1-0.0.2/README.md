# Comparing `tmp/monies-0.0.1.tar.gz` & `tmp/monies-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monies-0.0.1.tar", last modified: Tue Dec 19 05:14:35 2023, max compression
+gzip compressed data, was "monies-0.0.2.tar", max compression
```

## Comparing `monies-0.0.1.tar` & `monies-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.893858 monies-0.0.1/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      172 2023-12-19 05:14:35.893858 monies-0.0.1/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       51 2023-11-28 05:04:30.000000 monies-0.0.1/license.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      786 2023-12-19 05:14:29.000000 monies-0.0.1/pyproject.toml
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       38 2023-12-19 05:14:35.893858 monies-0.0.1/setup.cfg
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        0 2023-10-15 19:12:46.000000 monies-0.0.1/structure.txt
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.891858 monies-0.0.1/structures/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.892858 monies-0.0.1/structures/modules/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.893858 monies-0.0.1/structures/modules/monies.egg-info/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      172 2023-12-19 05:14:35.000000 monies-0.0.1/structures/modules/monies.egg-info/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      487 2023-12-19 05:14:35.000000 monies-0.0.1/structures/modules/monies.egg-info/SOURCES.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        1 2023-12-19 05:14:35.000000 monies-0.0.1/structures/modules/monies.egg-info/dependency_links.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       12 2023-12-19 05:14:35.000000 monies-0.0.1/structures/modules/monies.egg-info/top_level.txt
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.893858 monies-0.0.1/structures/modules/this_module/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       31 2023-12-11 06:18:44.000000 monies-0.0.1/structures/modules/this_module/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.893858 monies-0.0.1/structures/modules/this_module/_clique/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      297 2023-12-11 06:07:46.000000 monies-0.0.1/structures/modules/this_module/_clique/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.893858 monies-0.0.1/structures/modules/this_module/_clique/group/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      294 2023-12-01 19:53:30.000000 monies-0.0.1/structures/modules/this_module/_clique/group/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2023-12-19 05:14:35.893858 monies-0.0.1/structures/modules/this_module/_status/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1327 2023-12-11 06:15:05.000000 monies-0.0.1/structures/modules/this_module/_status/insurance.proc.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       62 2023-12-11 06:14:40.000000 monies-0.0.1/structures/modules/this_module/status_1.py
+-rwxr-xr-x   0        0        0      436 2024-04-27 22:55:20.051715 monies-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 monies-0.0.2/readme.md
+-rw-r--r--   0        0        0       36 2024-04-23 18:57:06.249310 monies-0.0.2/tracts/houses/monies/__init__.py
+-rw-r--r--   0        0        0       77 2024-03-23 20:03:57.719484 monies-0.0.2/tracts/houses/monies/__itinerary/later.S.HTML
+-rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 monies-0.0.2/tracts/houses/monies/_licenses/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 monies-0.0.2/tracts/houses/monies/_ops/_clique/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 monies-0.0.2/tracts/houses/monies/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 monies-0.0.2/tracts/houses/monies/_ops/_clique/group/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 monies-0.0.2/tracts/houses/monies/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 monies-0.0.2/tracts/houses/monies/_status/DB/records.json
+-rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 monies-0.0.2/tracts/houses/monies/_status/monitors/status_1.py
+-rw-r--r--   0        0        0     1375 2024-04-09 23:13:50.708900 monies-0.0.2/tracts/houses/monies/_status/status.proc.py
+-rw-r--r--   0        0        0       58 2024-04-23 19:29:47.178916 monies-0.0.2/tracts/houses/monies/adventures/stack.S.HTML
+-rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 monies-0.0.2/tracts/houses/monies/license.S.HTML
+-rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 monies-0.0.2/tracts/houses/monies/mixer.MD
+-rw-r--r--   0        0        0      154 2024-03-23 19:57:06.959925 monies-0.0.2/tracts/houses/monies/mixer.S.HTML
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 monies-0.0.2/PKG-INFO
```

### Comparing `monies-0.0.1/structures/modules/this_module/_status/insurance.proc.py` & `monies-0.0.2/tracts/houses/monies/_status/status.proc.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 
 
 def add_paths_to_system (paths):
 	import pathlib
 	from os.path import dirname, join, normpath
 	import sys
 	
-	this_folder = pathlib.Path (__file__).parent.resolve ()	
+	this_directory_path = pathlib.Path (__file__).parent.resolve ()	
 	for path in paths:
-		sys.path.insert (0, normpath (join (this_folder, path)))
+		sys.path.insert (0, normpath (join (this_directory_path, path)))
 
 add_paths_to_system ([
-	'../../../modules',
-	'../../../modules_pip'
+	'../../../mixers',
+	'../../../mixers_pip'
 ])
 
 
 import json
 import pathlib
 from os.path import dirname, join, normpath
 
 
-this_module_name = ""
+name = "this_mixer"
 
-this_folder = pathlib.Path (__file__).parent.resolve ()
-structures = str (normpath (join (this_folder, "../../../../structures")))
+this_directory_path = pathlib.Path (__file__).parent.resolve ()
+structures_path = str (normpath (join (this_directory_path, "../../../../structures_path")))
 
-this_module = str (normpath (join (structures, "modules", this_module_name)))
+this_mixer = str (normpath (join (structures_path, "mixers", name)))
 
-#status_assurances_path = str (normpath (join (this_folder, "insurance")))
-status_assurances_path = str (normpath (join (this_folder, "..")))
+#status_assurances_path = str (normpath (join (this_directory_path, "insurance")))
+status_assurances_path = str (normpath (join (this_directory_path, "..")))
 
 import sys
 if (len (sys.argv) >= 2):
 	glob_string = status_assurances_path + '/' + sys.argv [1]
 	db_directory = False
 else:
 	glob_string = status_assurances_path + '/**/status_*.py'
-	db_directory = normpath (join (this_folder, "DB"))
+	db_directory = normpath (join (this_directory_path, "DB"))
 
 print ("glob string:", glob_string)
 
-import homeostasis
-scan = homeostasis.start (
+import volts
+scan = volts.start (
 	glob_string = glob_string,
 	simultaneous = True,
-	module_paths = [
-		normpath (join (structures, "modules")),
-		normpath (join (structures, "modules_pip"))
+	mixer_paths = [
+		normpath (join (structures_path, "mixers")),
+		normpath (join (structures_path, "mixers_pip"))
 	],
 	relative_path = status_assurances_path,
 	
 	db_directory = db_directory
 )
```

