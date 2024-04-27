# Comparing `tmp/datasette_enrichments-0.4.tar.gz` & `tmp/datasette_enrichments-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_enrichments-0.4.tar", last modified: Sat Apr 27 06:04:22 2024, max compression
+gzip compressed data, was "datasette_enrichments-0.4.1.tar", last modified: Sat Apr 27 22:05:26 2024, max compression
```

## Comparing `datasette_enrichments-0.4.tar` & `datasette_enrichments-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.381303 datasette_enrichments-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-27 06:04:22.381303 datasette_enrichments-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/datasette_enrichments/
--rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/datasette_enrichments/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/templates/enrichment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/templates/enrichment_picker.html
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/datasette_enrichments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:04:22.381303 datasette_enrichments-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/tests/test_enrichments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:05:26.932745 datasette_enrichments-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-27 22:05:26.932745 datasette_enrichments-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:05:26.928745 datasette_enrichments-0.4.1/datasette_enrichments/
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/datasette_enrichments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/datasette_enrichments/hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:05:26.928745 datasette_enrichments-0.4.1/datasette_enrichments/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/datasette_enrichments/templates/enrichment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/datasette_enrichments/templates/enrichment_picker.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/datasette_enrichments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/datasette_enrichments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:05:26.928745 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-27 22:05:26.000000 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-27 22:05:26.000000 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:05:26.000000 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 22:05:26.000000 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 22:05:26.000000 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 22:05:26.000000 datasette_enrichments-0.4.1/datasette_enrichments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:05:26.932745 datasette_enrichments-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:05:26.928745 datasette_enrichments-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-27 22:05:10.000000 datasette_enrichments-0.4.1/tests/test_enrichments.py
```

### Comparing `datasette_enrichments-0.4/LICENSE` & `datasette_enrichments-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/PKG-INFO` & `datasette_enrichments-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments
-Version: 0.4
+Version: 0.4.1
 Summary: Tools for running enrichments against data stored in Datasette
 Home-page: https://github.com/simonw/datasette-enrichments
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-enrichments/issues
 Project-URL: CI, https://github.com/simonw/datasette-enrichments/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-enrichments/releases
```

### Comparing `datasette_enrichments-0.4/README.md` & `datasette_enrichments-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/datasette_enrichments/__init__.py` & `datasette_enrichments-0.4.1/datasette_enrichments/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,27 +110,24 @@
         cls._subclasses.append(cls)
 
     def __repr__(self):
         return "<Enrichment: {}>".format(self.slug)
 
     async def get_secret(self, datasette: "Datasette", config: dict):
         if self.secret is None:
-            breakpoint()
             raise SecretError("No secret defined for this enrichment")
         secret = await get_secret(datasette, self.secret.name)
         if secret is not None:
             return secret
         # Try the stashed secrets instead
         if not hasattr(datasette, "_enrichments_stashed_secrets"):
-            breakpoint()
             raise SecretError("No secrets have been stashed")
         stashed_keys = datasette._enrichments_stashed_secrets
         stash_key = config.get("enrichment_secret")
         if stash_key not in stashed_keys:
-            breakpoint()
             raise SecretError(
                 "No secret found in stash for {}".format(self.secret.name)
             )
         return stashed_keys[stash_key]
 
     async def log_error(
         self, db: "Database", job_id: int, ids: List[IdType], error: str
```

### Comparing `datasette_enrichments-0.4/datasette_enrichments/templates/enrichment.html` & `datasette_enrichments-0.4.1/datasette_enrichments/templates/enrichment.html`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/datasette_enrichments/templates/enrichment_picker.html` & `datasette_enrichments-0.4.1/datasette_enrichments/templates/enrichment_picker.html`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/datasette_enrichments/utils.py` & `datasette_enrichments-0.4.1/datasette_enrichments/utils.py`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/datasette_enrichments/views.py` & `datasette_enrichments-0.4.1/datasette_enrichments/views.py`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/datasette_enrichments.egg-info/PKG-INFO` & `datasette_enrichments-0.4.1/datasette_enrichments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments
-Version: 0.4
+Version: 0.4.1
 Summary: Tools for running enrichments against data stored in Datasette
 Home-page: https://github.com/simonw/datasette-enrichments
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-enrichments/issues
 Project-URL: CI, https://github.com/simonw/datasette-enrichments/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-enrichments/releases
```

### Comparing `datasette_enrichments-0.4/datasette_enrichments.egg-info/SOURCES.txt` & `datasette_enrichments-0.4.1/datasette_enrichments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette_enrichments-0.4/setup.py` & `datasette_enrichments-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4"
+VERSION = "0.4.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette_enrichments-0.4/tests/test_enrichments.py` & `datasette_enrichments-0.4.1/tests/test_enrichments.py`

 * *Files identical despite different names*

