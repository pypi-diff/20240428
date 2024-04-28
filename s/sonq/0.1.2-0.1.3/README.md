# Comparing `tmp/sonq-0.1.2.tar.gz` & `tmp/sonq-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sonq-0.1.2.tar", last modified: Mon Jun 15 02:15:14 2020, max compression
+gzip compressed data, was "sonq-0.1.3.tar", max compression
```

## Comparing `sonq-0.1.2.tar` & `sonq-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2020-06-15 02:15:14.000000 sonq-0.1.2/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1312 2020-06-15 02:15:14.000000 sonq-0.1.2/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      598 2018-09-13 00:45:52.000000 sonq-0.1.2/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2020-06-15 02:15:14.000000 sonq-0.1.2/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      921 2018-06-26 02:18:11.000000 sonq-0.1.2/setup.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2020-06-15 02:15:14.000000 sonq-0.1.2/sonq/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1214 2018-08-07 16:01:54.000000 sonq-0.1.2/sonq/cmd.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2242 2018-09-13 00:41:31.000000 sonq-0.1.2/sonq/operation.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6122 2020-06-15 01:58:00.000000 sonq-0.1.2/sonq/query.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       22 2020-06-15 02:14:04.000000 sonq-0.1.2/sonq/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2020-06-15 02:15:14.000000 sonq-0.1.2/sonq.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2020-06-15 02:15:13.000000 sonq-0.1.2/sonq.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       40 2020-06-15 02:15:13.000000 sonq-0.1.2/sonq.egg-info/entry_points.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2018-06-26 02:16:54.000000 sonq-0.1.2/sonq.egg-info/not-zip-safe
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1312 2020-06-15 02:15:13.000000 sonq-0.1.2/sonq.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       12 2020-06-15 02:15:13.000000 sonq-0.1.2/sonq.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      281 2020-06-15 02:15:13.000000 sonq-0.1.2/sonq.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        5 2020-06-15 02:15:13.000000 sonq-0.1.2/sonq.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0      625 2022-06-19 01:52:58.000000 sonq-0.1.3/README.md
+-rwxr-xr-x   0        0        0      566 2024-04-27 22:32:13.967408 sonq-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0       22 2020-06-15 02:14:04.000000 sonq-0.1.3/sonq/__init__.py
+-rwxr-xr-x   0        0        0     2931 2024-04-27 03:46:31.663929 sonq-0.1.3/sonq/cmd.py
+-rw-r--r--   0        0        0     3145 2024-04-27 03:47:16.202199 sonq-0.1.3/sonq/operation.py
+-rwxr-xr-x   0        0        0     6158 2022-06-18 14:38:32.000000 sonq-0.1.3/sonq/query.py
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 sonq-0.1.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sonq-0.1.2/README.md` & `sonq-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sonq
 
-__sonq__ means son query, is tool for son like objects, for example, json and bson. You may use sonq to query .bson or newline separated .json files directly from command line.
+__sonq__ means son query, is a tool for querying son like objects, for example, JSON and BSON. You may use sonq to query .bson or newline separated .json files(JSON Lines) directly from the command line.
 
 
 ## Install
 
 ```
 pip install sonq
 ```
```

### Comparing `sonq-0.1.2/sonq/query.py` & `sonq-0.1.3/sonq/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 def get_separated_attr(dict_obj, attr_name, separator='.'):
     '''
     Extract dot separated attribute from dict_object.
     '''
     parts = attr_name.split(separator)
     curr = dict_obj
     existed = False
+    parts_last_idx = len(parts) - 1
     for num, part in enumerate(parts):
         if curr is None:
             break
         if part.isdigit() and isinstance(curr, (list, tuple)):
             part = int(part)
             if part < len(curr):
                 curr = curr[part]
-                if num == len(parts) - 1:
+                if num == parts_last_idx:
                     existed = True
             else:
                 curr = None
         elif isinstance(curr, dict) and part in curr:
             curr = curr[part]
-            if num == len(parts) - 1:
+            if num == parts_last_idx:
                 existed = True
         else:
             curr = None
     return existed, curr
 
 
 class Handlers:
```

