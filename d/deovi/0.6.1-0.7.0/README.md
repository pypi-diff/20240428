# Comparing `tmp/deovi-0.6.1.tar.gz` & `tmp/deovi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deovi-0.6.1.tar", last modified: Sun Jul 16 10:04:24 2023, max compression
+gzip compressed data, was "deovi-0.7.0.tar", last modified: Sun Apr 28 00:07:52 2024, max compression
```

## Comparing `deovi-0.6.1.tar` & `deovi-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.481897 deovi-0.6.1/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1075 2022-09-12 23:01:15.000000 deovi-0.6.1/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      173 2022-09-12 23:01:15.000000 deovi-0.6.1/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-16 10:04:24.481897 deovi-0.6.1/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      979 2023-07-12 20:40:49.000000 deovi-0.6.1/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      686 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi/cli/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/cli/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1940 2023-03-07 02:37:37.000000 deovi-0.6.1/deovi/cli/collect.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1860 2023-07-12 20:40:49.000000 deovi-0.6.1/deovi/cli/entrypoint.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1117 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/cli/job.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1751 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/cli/rename.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4007 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/cli/scrap.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      232 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/cli/version.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi/collector/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      463 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/collector/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    13956 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/collector/collect.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6755 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/collector/storage.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1150 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/exceptions.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1128 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/logger.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.481897 deovi-0.6.1/deovi/renamer/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    10871 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/jobs.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4685 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/renamer/printer.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4505 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/runner.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11870 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/tasks.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5033 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/renamer/validators.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5999 2023-07-16 10:03:32.000000 deovi-0.6.1/deovi/scrapper.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.481897 deovi-0.6.1/deovi/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.1/deovi/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4720 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/utils/checksum.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/utils/jsons.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3347 2023-05-09 00:34:27.000000 deovi-0.6.1/deovi/utils/tests.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-16 10:04:24.477897 deovi-0.6.1/deovi.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      789 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/entry_points.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      234 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        6 2023-07-16 10:04:24.000000 deovi-0.6.1/deovi.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-03-04 01:42:58.000000 deovi-0.6.1/deovi.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1482 2023-07-16 10:04:24.481897 deovi-0.6.1/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-09-12 23:01:15.000000 deovi-0.6.1/setup.py
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1075 2022-06-24 17:05:47.000000 deovi-0.7.0/LICENCE.txt
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      173 2022-06-24 17:05:47.000000 deovi-0.7.0/MANIFEST.in
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1784 2024-04-28 00:07:52.956579 deovi-0.7.0/PKG-INFO
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      979 2024-04-27 14:20:35.000000 deovi-0.7.0/README.rst
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/deovi/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      686 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/__init__.py
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/deovi/cli/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)        0 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/cli/__init__.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1940 2023-03-07 02:41:32.000000 deovi-0.7.0/deovi/cli/collect.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1860 2024-04-27 14:20:35.000000 deovi-0.7.0/deovi/cli/entrypoint.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1117 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/cli/job.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1751 2023-05-09 00:57:55.000000 deovi-0.7.0/deovi/cli/rename.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     4007 2024-04-27 14:20:35.000000 deovi-0.7.0/deovi/cli/scrap.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      232 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/cli/version.py
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/deovi/collector/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      463 2023-05-09 00:57:55.000000 deovi-0.7.0/deovi/collector/__init__.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)    15030 2024-04-28 00:06:57.000000 deovi-0.7.0/deovi/collector/collect.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     6755 2024-04-27 14:20:35.000000 deovi-0.7.0/deovi/collector/storage.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1150 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/exceptions.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1128 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/logger.py
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/deovi/renamer/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)        0 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/renamer/__init__.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)    10871 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/renamer/jobs.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     4685 2023-05-09 00:57:55.000000 deovi-0.7.0/deovi/renamer/printer.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     4505 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/renamer/runner.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)    11870 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/renamer/tasks.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     5033 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/renamer/validators.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     5999 2024-04-27 14:20:35.000000 deovi-0.7.0/deovi/scrapper.py
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/deovi/utils/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)        0 2022-06-24 17:05:47.000000 deovi-0.7.0/deovi/utils/__init__.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     4720 2023-05-09 00:57:55.000000 deovi-0.7.0/deovi/utils/checksum.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      717 2023-05-09 00:57:55.000000 deovi-0.7.0/deovi/utils/jsons.py
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     3347 2023-05-09 00:57:55.000000 deovi-0.7.0/deovi/utils/tests.py
+drwxrwxr-x   0 thenonda  (1000) thenonda  (1000)        0 2024-04-28 00:07:52.956579 deovi-0.7.0/deovi.egg-info/
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1784 2024-04-28 00:07:52.000000 deovi-0.7.0/deovi.egg-info/PKG-INFO
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      789 2024-04-28 00:07:52.000000 deovi-0.7.0/deovi.egg-info/SOURCES.txt
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)        1 2024-04-28 00:07:52.000000 deovi-0.7.0/deovi.egg-info/dependency_links.txt
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)       60 2024-04-28 00:07:52.000000 deovi-0.7.0/deovi.egg-info/entry_points.txt
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)      234 2024-04-28 00:07:52.000000 deovi-0.7.0/deovi.egg-info/requires.txt
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)        6 2024-04-28 00:07:52.000000 deovi-0.7.0/deovi.egg-info/top_level.txt
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)        1 2023-05-09 00:58:08.000000 deovi-0.7.0/deovi.egg-info/zip-safe
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)     1482 2024-04-28 00:07:52.960579 deovi-0.7.0/setup.cfg
+-rw-rw-r--   0 thenonda  (1000) thenonda  (1000)       84 2022-06-24 17:05:47.000000 deovi-0.7.0/setup.py
```

### Comparing `deovi-0.6.1/LICENCE.txt` & `deovi-0.7.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/PKG-INFO` & `deovi-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deovi
-Version: 0.6.1
+Version: 0.7.0
 Summary: Utility to rename files and collect their filepaths
 Home-page: https://github.com/sveetch/deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `deovi-0.6.1/README.rst` & `deovi-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/__init__.py` & `deovi-0.7.0/deovi/__init__.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/cli/collect.py` & `deovi-0.7.0/deovi/cli/collect.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/cli/entrypoint.py` & `deovi-0.7.0/deovi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/cli/job.py` & `deovi-0.7.0/deovi/cli/job.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/cli/rename.py` & `deovi-0.7.0/deovi/cli/rename.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/cli/scrap.py` & `deovi-0.7.0/deovi/cli/scrap.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/collector/collect.py` & `deovi-0.7.0/deovi/collector/collect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import json
+from shutil import disk_usage
 
 import yaml
 
 from ..renamer.printer import PrinterInterface
 from ..utils.jsons import ExtendedJsonEncoder
 from ..utils.checksum import ChecksumOperator
 from ..exceptions import CollectorError
@@ -371,14 +372,39 @@
                 )
 
             # Store collected data
             self.store(data)
 
         return data
 
+    def scan_basepath_device(self, path):
+        """
+        Collect basepath device information.
+
+        .. Note:
+            This only compute information for the device which basepath belong to, this
+            does not compute the basepath information itself.
+
+        Arguments:
+            path (pathlib.Path): Path to use to get the device to scan.
+
+        Returns:
+            dict: A dictionnary of device informations (total size, used size,
+            free space size and occupancy percentage).
+        """
+        path = path.resolve()
+        stats = disk_usage(path)
+
+        return {
+            "total": stats.total,
+            "used": stats.used,
+            "free": stats.free,
+            "percentage": (stats.used / stats.total) * 100,
+        }
+
     def run(self, destination=None, checksum=False):
         """
         Recursively scan everything from basepath to produce a registry of collected
         informations.
 
         Keyword Arguments:
             destination (pathlib.Path): Destination path to write a JSON file with
@@ -389,19 +415,28 @@
 
         Returns:
             dict: Dictionnary of global states for collected directories and files.
         """
         # Set storage basepath from destination location
         self.storage.set_basepath(destination, checksum=checksum)
 
+        device_stats = self.scan_basepath_device(self.basepath)
         self.scan_directory(self.basepath, checksum=checksum)
 
         if self.registry and destination:
             with destination.open("w") as fp:
-                json.dump(self.registry, fp, indent=4, cls=ExtendedJsonEncoder)
+                json.dump(
+                    {
+                        "device": device_stats,
+                        "registry": self.registry,
+                    },
+                    fp,
+                    indent=4,
+                    cls=ExtendedJsonEncoder
+                )
                 self.log_info("Registry saved to: {}".format(str(destination)))
 
             # Proceed to copy queued files into storage dir
             container, stored = self.storage.store_assets(self.file_storage_queue)
             if container:
                 self.stats["asset_storage"] = container
```

### Comparing `deovi-0.6.1/deovi/collector/storage.py` & `deovi-0.7.0/deovi/collector/storage.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/exceptions.py` & `deovi-0.7.0/deovi/exceptions.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/logger.py` & `deovi-0.7.0/deovi/logger.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/renamer/jobs.py` & `deovi-0.7.0/deovi/renamer/jobs.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/renamer/printer.py` & `deovi-0.7.0/deovi/renamer/printer.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/renamer/runner.py` & `deovi-0.7.0/deovi/renamer/runner.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/renamer/tasks.py` & `deovi-0.7.0/deovi/renamer/tasks.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/renamer/validators.py` & `deovi-0.7.0/deovi/renamer/validators.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/scrapper.py` & `deovi-0.7.0/deovi/scrapper.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/utils/checksum.py` & `deovi-0.7.0/deovi/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/utils/jsons.py` & `deovi-0.7.0/deovi/utils/jsons.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi/utils/tests.py` & `deovi-0.7.0/deovi/utils/tests.py`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/deovi.egg-info/PKG-INFO` & `deovi-0.7.0/deovi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deovi
-Version: 0.6.1
+Version: 0.7.0
 Summary: Utility to rename files and collect their filepaths
 Home-page: https://github.com/sveetch/deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `deovi-0.6.1/deovi.egg-info/SOURCES.txt` & `deovi-0.7.0/deovi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deovi-0.6.1/setup.cfg` & `deovi-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deovi
-version = 0.6.1
+version = 0.7.0
 description = Utility to rename files and collect their filepaths
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = sveetch@gmail.com
 url = https://github.com/sveetch/deovi
 license = MIT
```

