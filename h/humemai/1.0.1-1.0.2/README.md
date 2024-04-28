# Comparing `tmp/humemai-1.0.1.tar.gz` & `tmp/humemai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humemai-1.0.1.tar", last modified: Sat Apr 20 09:34:57 2024, max compression
+gzip compressed data, was "humemai-1.0.2.tar", last modified: Sun Apr 28 12:00:07 2024, max compression
```

## Comparing `humemai-1.0.1.tar` & `humemai-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 09:34:47.000000 humemai-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-20 09:34:57.011994 humemai-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-20 09:34:47.000000 humemai-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/humemai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/humemai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-20 09:34:57.011994 humemai-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 09:34:47.000000 humemai-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)    42246 2024-04-20 09:34:47.000000 humemai-1.0.1/test/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-04-20 09:34:47.000000 humemai-1.0.1/test/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-20 09:34:47.000000 humemai-1.0.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:00:07.128039 humemai-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 11:59:58.000000 humemai-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-28 12:00:07.128039 humemai-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-28 11:59:58.000000 humemai-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:00:07.124039 humemai-1.0.2/humemai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:59:58.000000 humemai-1.0.2/humemai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-04-28 11:59:58.000000 humemai-1.0.2/humemai/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-28 11:59:58.000000 humemai-1.0.2/humemai/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-28 11:59:58.000000 humemai-1.0.2/humemai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:00:07.128039 humemai-1.0.2/humemai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-28 12:00:07.000000 humemai-1.0.2/humemai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-28 12:00:07.000000 humemai-1.0.2/humemai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:00:07.000000 humemai-1.0.2/humemai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 12:00:07.000000 humemai-1.0.2/humemai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 12:00:07.000000 humemai-1.0.2/humemai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-28 12:00:07.128039 humemai-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 11:59:58.000000 humemai-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:00:07.128039 humemai-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    42246 2024-04-28 11:59:58.000000 humemai-1.0.2/test/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-04-28 11:59:58.000000 humemai-1.0.2/test/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-28 11:59:58.000000 humemai-1.0.2/test/test_utils.py
```

### Comparing `humemai-1.0.1/LICENSE` & `humemai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `humemai-1.0.1/PKG-INFO` & `humemai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humemai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Machine With Human-Like Memory Systems.
 Home-page: https://github.com/humemai/humemai
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/humemai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `humemai-1.0.1/README.md` & `humemai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `humemai-1.0.1/humemai/memory.py` & `humemai-1.0.2/humemai/memory.py`

 * *Files identical despite different names*

### Comparing `humemai-1.0.1/humemai/policy.py` & `humemai-1.0.2/humemai/policy.py`

 * *Files identical despite different names*

### Comparing `humemai-1.0.1/humemai.egg-info/PKG-INFO` & `humemai-1.0.2/humemai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humemai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Machine With Human-Like Memory Systems.
 Home-page: https://github.com/humemai/humemai
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/humemai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `humemai-1.0.1/setup.cfg` & `humemai-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = humemai
-version = 1.0.1
+version = 1.0.2
 author = Taewoon Kim
 author_email = info@humem.ai
 description = A Machine With Human-Like Memory Systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/humemai/humemai
 project_urls =
```

### Comparing `humemai-1.0.1/test/test_memory.py` & `humemai-1.0.2/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `humemai-1.0.1/test/test_policy.py` & `humemai-1.0.2/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `humemai-1.0.1/test/test_utils.py` & `humemai-1.0.2/test/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,10 @@
 
     def test_list_duplicates_of(self):
         foo = list_duplicates_of(
             [{"foo": 1}, {"bar": 2}, {"foo": 2}, {"foo": 1}], {"foo": 1}
         )
         self.assertEqual(foo, [0, 3])
 
-    def test_split_by_possessive(self):
-        foo = split_by_possessive("John's book")
-        self.assertEqual(foo, ("John", "book"))
-
     def test_remove_possessive(self):
         foo = remove_posession("John's book")
         self.assertEqual(foo, "book")
```

