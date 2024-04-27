# Comparing `tmp/tracts-0.0.1.tar.gz` & `tmp/tracts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracts-0.0.1.tar", max compression
+gzip compressed data, was "tracts-0.0.2.tar", max compression
```

## Comparing `tracts-0.0.1.tar` & `tracts-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0      425 2024-04-27 22:26:05.983257 tracts-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 tracts-0.0.1/readme.md
--rw-r--r--   0        0        0       36 2024-04-23 18:57:06.249310 tracts-0.0.1/venues/stages/tracts/__init__.py
--rw-r--r--   0        0        0       77 2024-03-23 20:03:57.719484 tracts-0.0.1/venues/stages/tracts/__itinerary/later.S.HTML
--rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 tracts-0.0.1/venues/stages/tracts/_licenses/gpl-3.0-standalone.html
--rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 tracts-0.0.1/venues/stages/tracts/_ops/_clique/__init__.py
--rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 tracts-0.0.1/venues/stages/tracts/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 tracts-0.0.1/venues/stages/tracts/_ops/_clique/group/__init__.py
--rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 tracts-0.0.1/venues/stages/tracts/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 tracts-0.0.1/venues/stages/tracts/_status/DB/records.json
--rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 tracts-0.0.1/venues/stages/tracts/_status/monitors/status_1.py
--rw-r--r--   0        0        0     1375 2024-04-09 23:13:50.708900 tracts-0.0.1/venues/stages/tracts/_status/status.proc.py
--rw-r--r--   0        0        0       58 2024-04-23 19:29:47.178916 tracts-0.0.1/venues/stages/tracts/adventures/stack.S.HTML
--rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 tracts-0.0.1/venues/stages/tracts/license.S.HTML
--rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 tracts-0.0.1/venues/stages/tracts/mixer.MD
--rw-r--r--   0        0        0      154 2024-03-23 19:57:06.959925 tracts-0.0.1/venues/stages/tracts/mixer.S.HTML
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 tracts-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      459 2024-04-27 22:30:31.804209 tracts-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 tracts-0.0.2/readme.md
+-rw-r--r--   0        0        0       36 2024-04-23 18:57:06.249310 tracts-0.0.2/venues/stages/tracts/__init__.py
+-rw-r--r--   0        0        0       77 2024-03-23 20:03:57.719484 tracts-0.0.2/venues/stages/tracts/__itinerary/later.S.HTML
+-rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 tracts-0.0.2/venues/stages/tracts/_licenses/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 tracts-0.0.2/venues/stages/tracts/_ops/_clique/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 tracts-0.0.2/venues/stages/tracts/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 tracts-0.0.2/venues/stages/tracts/_ops/_clique/group/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 tracts-0.0.2/venues/stages/tracts/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 tracts-0.0.2/venues/stages/tracts/_status/DB/records.json
+-rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 tracts-0.0.2/venues/stages/tracts/_status/monitors/status_1.py
+-rw-r--r--   0        0        0     1375 2024-04-09 23:13:50.708900 tracts-0.0.2/venues/stages/tracts/_status/status.proc.py
+-rw-r--r--   0        0        0       58 2024-04-23 19:29:47.178916 tracts-0.0.2/venues/stages/tracts/adventures/stack.S.HTML
+-rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 tracts-0.0.2/venues/stages/tracts/license.S.HTML
+-rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 tracts-0.0.2/venues/stages/tracts/mixer.MD
+-rw-r--r--   0        0        0      154 2024-03-23 19:57:06.959925 tracts-0.0.2/venues/stages/tracts/mixer.S.HTML
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 tracts-0.0.2/PKG-INFO
```

### Comparing `tracts-0.0.1/venues/stages/tracts/_licenses/gpl-3.0-standalone.html` & `tracts-0.0.2/venues/stages/tracts/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `tracts-0.0.1/venues/stages/tracts/_status/DB/records.json` & `tracts-0.0.2/venues/stages/tracts/_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `tracts-0.0.1/venues/stages/tracts/_status/status.proc.py` & `tracts-0.0.2/venues/stages/tracts/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `tracts-0.0.1/PKG-INFO` & `tracts-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tracts
-Version: 0.0.1
-Summary: 
+Version: 0.0.2
+Summary: Drawings of the tracts and fields.
 License: licensed
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

