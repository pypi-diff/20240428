# Comparing `tmp/redzoo-0.3.0.tar.gz` & `tmp/redzoo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redzoo-0.3.0.tar", last modified: Wed Oct 11 05:49:59 2023, max compression
+gzip compressed data, was "redzoo-0.3.1.tar", last modified: Sun Apr 28 13:07:26 2024, max compression
```

## Comparing `redzoo-0.3.0.tar` & `redzoo-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.283944 redzoo-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-11 05:49:47.000000 redzoo-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-10-11 05:49:59.283944 redzoo-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-11 05:49:47.000000 redzoo-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-11 05:49:47.000000 redzoo-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.279944 redzoo-0.3.0/redzoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.279944 redzoo-0.3.0/redzoo/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/database/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.279944 redzoo-0.3.0/redzoo/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/math/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.283944 redzoo-0.3.0/redzoo/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2023-10-11 05:49:47.000000 redzoo-0.3.0/redzoo/metrics/consumption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.279944 redzoo-0.3.0/redzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-10-11 05:49:59.000000 redzoo-0.3.0/redzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 05:49:59.000000 redzoo-0.3.0/redzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 05:49:59.000000 redzoo-0.3.0/redzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-11 05:49:59.000000 redzoo-0.3.0/redzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-11 05:49:59.000000 redzoo-0.3.0/redzoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-10-11 05:49:59.283944 redzoo-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 05:49:59.283944 redzoo-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-11 05:49:47.000000 redzoo-0.3.0/test/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-10-11 05:49:47.000000 redzoo-0.3.0/test/test_simpledb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.170373 redzoo-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 13:07:20.000000 redzoo-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-28 13:07:26.170373 redzoo-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 13:07:20.000000 redzoo-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-28 13:07:20.000000 redzoo-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.166373 redzoo-0.3.1/redzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.166373 redzoo-0.3.1/redzoo/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/database/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.166373 redzoo-0.3.1/redzoo/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/math/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.166373 redzoo-0.3.1/redzoo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-28 13:07:20.000000 redzoo-0.3.1/redzoo/metrics/consumption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.170373 redzoo-0.3.1/redzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-28 13:07:26.000000 redzoo-0.3.1/redzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 13:07:26.000000 redzoo-0.3.1/redzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:07:26.000000 redzoo-0.3.1/redzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 13:07:26.000000 redzoo-0.3.1/redzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 13:07:26.000000 redzoo-0.3.1/redzoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-28 13:07:26.170373 redzoo-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:07:26.170373 redzoo-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-28 13:07:20.000000 redzoo-0.3.1/test/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-28 13:07:20.000000 redzoo-0.3.1/test/test_simpledb.py
```

### Comparing `redzoo-0.3.0/LICENSE` & `redzoo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.0/redzoo/database/simple.py` & `redzoo-0.3.1/redzoo/database/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,21 @@
     @staticmethod
     def from_dict(dict: Dict):
         return Entry(dict['value'], datetime.strptime(dict['expire_date'], "%Y.%m.%d %H:%M:%S"))
 
 
 class SimpleDB:
 
-    def __init__(self, name: str, sync_period_sec:int = None):
+    def __init__(self, name: str, sync_period_sec:int = None, directory: str = None):
         self.sync_period_sec = sync_period_sec
         self.__name = name
-        self.__directory = site_data_dir("simpledb", appauthor=False)
+        if directory is None:
+            self.__directory = site_data_dir("simpledb", appauthor=False)
+        else:
+            self.__directory = directory
         self.__data = self.__load()
         self.__last_time_stored = datetime.now()
         logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries)")
 
     @property
     def filename(self):
         if not os.path.exists(self.__directory):
```

### Comparing `redzoo-0.3.0/redzoo/math/display.py` & `redzoo-0.3.1/redzoo/math/display.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.0/redzoo/metrics/consumption.py` & `redzoo-0.3.1/redzoo/metrics/consumption.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.0/test/test_simpledb.py` & `redzoo-0.3.1/test/test_simpledb.py`

 * *Files identical despite different names*

