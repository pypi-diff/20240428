# Comparing `tmp/yappr-1.0.1.tar.gz` & `tmp/yappr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappr-1.0.1.tar", last modified: Fri Apr 26 21:12:49 2024, max compression
+gzip compressed data, was "yappr-1.0.2.tar", last modified: Sun Apr 28 04:17:46 2024, max compression
```

## Comparing `yappr-1.0.1.tar` & `yappr-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:12:49.328333 yappr-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 21:12:44.000000 yappr-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 21:12:44.000000 yappr-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-26 21:12:49.328333 yappr-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-26 21:12:44.000000 yappr-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-26 21:12:44.000000 yappr-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:12:49.328333 yappr-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:12:49.324333 yappr-1.0.1/yappr/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 21:12:44.000000 yappr-1.0.1/yappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-26 21:12:44.000000 yappr-1.0.1/yappr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:12:44.000000 yappr-1.0.1/yappr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-26 21:12:44.000000 yappr-1.0.1/yappr/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:12:49.324333 yappr-1.0.1/yappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-26 21:12:49.000000 yappr-1.0.1/yappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-26 21:12:49.000000 yappr-1.0.1/yappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:12:49.000000 yappr-1.0.1/yappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 21:12:49.000000 yappr-1.0.1/yappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:17:46.174772 yappr-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 04:17:41.000000 yappr-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 04:17:41.000000 yappr-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-28 04:17:46.170772 yappr-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-28 04:17:41.000000 yappr-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-28 04:17:41.000000 yappr-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:17:46.174772 yappr-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:17:46.170772 yappr-1.0.2/yappr/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 04:17:41.000000 yappr-1.0.2/yappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-28 04:17:41.000000 yappr-1.0.2/yappr/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-28 04:17:41.000000 yappr-1.0.2/yappr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:17:41.000000 yappr-1.0.2/yappr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-28 04:17:41.000000 yappr-1.0.2/yappr/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:17:46.170772 yappr-1.0.2/yappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-28 04:17:46.000000 yappr-1.0.2/yappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-28 04:17:46.000000 yappr-1.0.2/yappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:17:46.000000 yappr-1.0.2/yappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 04:17:46.000000 yappr-1.0.2/yappr.egg-info/top_level.txt
```

### Comparing `yappr-1.0.1/LICENSE` & `yappr-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yappr-1.0.1/PKG-INFO` & `yappr-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Yet another python package updater
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `yappr-1.0.1/README.md` & `yappr-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yappr-1.0.1/pyproject.toml` & `yappr-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yappr"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = []
 requires-python = ">=3"
-authors = [
-  { name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" },
-]
+authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Yet another python package updater"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
 classifiers = ["Programming Language :: Python :: 3"]
 
 [project.urls]
```

### Comparing `yappr-1.0.1/yappr/logger.py` & `yappr-1.0.2/yappr/logger.py`

 * *Files identical despite different names*

### Comparing `yappr-1.0.1/yappr/updater.py` & `yappr-1.0.2/yappr/updater.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
             if not latest:
                 logger.error("Could not determine the latest version.")
                 return
             if latest == current:
                 logger.info("Already upto date.")
                 return
             logger.info(f"New version found: {current} -> {latest}")
-            self.update()
             self.new_update_flag.set()
+            self.update()
             self.exit_flag.set()
         except Exception:
             logger.exception("Unhandled exception in updater.")
 
     def check_for_updates_loop(self):
         self.exit_flag.wait(self.first_update_interval)
         while True:
```

### Comparing `yappr-1.0.1/yappr.egg-info/PKG-INFO` & `yappr-1.0.2/yappr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Yet another python package updater
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

