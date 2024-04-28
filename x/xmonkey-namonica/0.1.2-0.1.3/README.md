# Comparing `tmp/xmonkey_namonica-0.1.2.tar.gz` & `tmp/xmonkey_namonica-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.2.tar", last modified: Fri Apr 26 22:49:37 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.3.tar", last modified: Sun Apr 28 18:25:14 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.2.tar` & `xmonkey_namonica-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 22:49:37.034187 xmonkey_namonica-0.1.2/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.2/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-26 22:49:37.034021 xmonkey_namonica-0.1.2/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      433 2024-04-26 22:45:22.000000 xmonkey_namonica-0.1.2/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-26 22:49:37.034233 xmonkey_namonica-0.1.2/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      352 2024-04-26 22:49:11.000000 xmonkey_namonica-0.1.2/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 22:49:37.032072 xmonkey_namonica-0.1.2/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1988 2024-04-26 22:43:33.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3716 2024-04-26 18:36:04.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 22:49:37.033599 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3918 2024-04-26 22:48:45.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/gen_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.2/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 22:49:37.033859 xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-26 22:49:36.000000 xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      625 2024-04-26 22:49:37.000000 xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-26 22:49:36.000000 xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-26 22:49:36.000000 xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-26 22:49:36.000000 xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.628571 xmonkey_namonica-0.1.3/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.3/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-28 18:25:14.628372 xmonkey_namonica-0.1.3/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      555 2024-04-28 18:24:45.000000 xmonkey_namonica-0.1.3/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-28 18:25:14.628605 xmonkey_namonica-0.1.3/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      352 2024-04-28 18:23:52.000000 xmonkey_namonica-0.1.3/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.626663 xmonkey_namonica-0.1.3/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2135 2024-04-28 18:13:38.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3716 2024-04-26 18:36:04.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.628073 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3918 2024-04-26 22:48:45.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/gen_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3696 2024-04-28 18:23:26.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/github_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.628214 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      669 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.2/LICENSE` & `xmonkey_namonica-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 from .handlers.npm_handler import NpmHandler
 from .handlers.cargo_handler import CargoHandler
 from .handlers.pypi_handler import PypiHandler
 from .handlers.nuget_handler import NugetHandler
 from .handlers.gen_handler import GenericHandler
+from .handlers.github_handler import GithubHandler
 
 
 def main():
     parser = argparse.ArgumentParser(description="Package Analyzer Tool")
     parser.add_argument("purl", type=str, help="Package URL to process")
     parser.add_argument(
         "--export", type=str,
@@ -17,26 +18,28 @@
         default=None
     )
     parser.add_argument(
         "--full", action="store_true",
         help="Print a full list of copyrights and license files"
     )
     args = parser.parse_args()
-    if "npm" in args.purl:
+    if "pkg:npm" in args.purl:
         handler = NpmHandler(args.purl)
-    elif "cargo" in args.purl:
+    elif "pkg:cargo" in args.purl:
         handler = CargoHandler(args.purl)
-    elif "pypi" in args.purl:
+    elif "pkg:pypi" in args.purl:
         handler = PypiHandler(args.purl)
-    elif "nuget" in args.purl:
+    elif "pkg:nuget" in args.purl:
         handler = NugetHandler(args.purl)
-    elif "generic" in args.purl:
+    elif "pkg:generic" in args.purl:
         handler = GenericHandler(args.purl)
+    elif "pkg:github" in args.purl:
+        handler = GithubHandler(args.purl)
     else:
-        raise ValueError("Unsupported package type")
+        raise ValueError("Unsupported PURL type")
     handler.fetch()
     result = handler.generate_report()
     license_files = [entry['content'] for entry in result['license_files']]
     licenses = list(set(license_files))
     copyhits = [entry['line'] for entry in result['copyrights']]
     copyrights = list(set(copyhits))
     if args.full:
```

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/common.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/cargo_handler.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/cargo_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/gen_handler.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/gen_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/npm_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.3/xmonkey_namonica/utils.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.2/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 xmonkey_namonica.egg-info/dependency_links.txt
 xmonkey_namonica.egg-info/entry_points.txt
 xmonkey_namonica.egg-info/top_level.txt
 xmonkey_namonica/handlers/__init__.py
 xmonkey_namonica/handlers/base_handler.py
 xmonkey_namonica/handlers/cargo_handler.py
 xmonkey_namonica/handlers/gen_handler.py
+xmonkey_namonica/handlers/github_handler.py
 xmonkey_namonica/handlers/npm_handler.py
 xmonkey_namonica/handlers/nuget_handler.py
 xmonkey_namonica/handlers/pypi_handler.py
```

