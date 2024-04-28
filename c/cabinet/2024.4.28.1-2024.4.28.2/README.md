# Comparing `tmp/cabinet-2024.4.28.1.tar.gz` & `tmp/cabinet-2024.4.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.4.28.1.tar", last modified: Sun Apr 28 07:01:43 2024, max compression
+gzip compressed data, was "cabinet-2024.4.28.2.tar", last modified: Sun Apr 28 18:04:48 2024, max compression
```

## Comparing `cabinet-2024.4.28.1.tar` & `cabinet-2024.4.28.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.28.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37996 2024-04-28 06:57:49.000000 cabinet-2024.4.28.1/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.28.1/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.4.28.1/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 07:01:09.000000 cabinet-2024.4.28.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.28.2/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37940 2024-04-28 18:04:10.000000 cabinet-2024.4.28.2/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.28.2/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.4.28.2/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.4.28.2/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.4.28.1/LICENSE` & `cabinet-2024.4.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.1/PKG-INFO` & `cabinet-2024.4.28.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.28.1
+Version: 2024.4.28.2
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2024.4.28.1/README.md` & `cabinet-2024.4.28.2/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.1/setup.cfg` & `cabinet-2024.4.28.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.04.28.1
+version = 2024.04.28.2
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.4.28.1/src/cabinet/cabinet.py` & `cabinet-2024.4.28.2/src/cabinet/cabinet.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,17 +639,14 @@
 
             if isinstance(result, str):
                 result = helpers.resolve_path(result)
 
             if is_print:
                 print(result)
 
-            if is_print:
-                print(result)
-
             # Handle return_type if specified
             if return_type is not None:
                 try:
                     return return_type(result)
                 except (ValueError, TypeError) as e:
                     self.log(f"Error casting result to {return_type}: {str(e)}", level="error")
                     return None
```

### Comparing `cabinet-2024.4.28.1/src/cabinet/constants.py` & `cabinet-2024.4.28.2/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.1/src/cabinet/mail.py` & `cabinet-2024.4.28.2/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.4.28.2/src/cabinet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.28.1
+Version: 2024.4.28.2
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

