# Comparing `tmp/rlsdk_python-0.3.0.tar.gz` & `tmp/rlsdk_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlsdk_python-0.3.0.tar", max compression
+gzip compressed data, was "rlsdk_python-0.4.0.tar", max compression
```

## Comparing `rlsdk_python-0.3.0.tar` & `rlsdk_python-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      357 2024-04-26 19:59:33.045916 rlsdk_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.3.0/README.md
--rw-r--r--   0        0        0      107 2024-04-16 11:12:58.877877 rlsdk_python-0.3.0/rlsdk_python/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.3.0/rlsdk_python/event_handling.py
--rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.3.0/rlsdk_python/events.py
--rw-r--r--   0        0        0     4065 2024-04-26 18:56:51.985326 rlsdk_python-0.3.0/rlsdk_python/frida_script.py
--rw-r--r--   0        0        0    30557 2024-04-26 15:34:23.035361 rlsdk_python-0.3.0/rlsdk_python/game_objects.py
--rw-r--r--   0        0        0    21779 2024-04-26 19:56:52.007905 rlsdk_python-0.3.0/rlsdk_python/sdk.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 rlsdk_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      357 2024-04-28 21:04:45.985727 rlsdk_python-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.4.0/README.md
+-rw-r--r--   0        0        0      121 2024-04-28 17:35:36.468385 rlsdk_python-0.4.0/rlsdk_python/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.4.0/rlsdk_python/event_handling.py
+-rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.4.0/rlsdk_python/events.py
+-rw-r--r--   0        0        0     4065 2024-04-26 18:56:51.985326 rlsdk_python-0.4.0/rlsdk_python/frida_script.py
+-rw-r--r--   0        0        0    30557 2024-04-26 15:34:23.035361 rlsdk_python-0.4.0/rlsdk_python/game_objects.py
+-rw-r--r--   0        0        0    21863 2024-04-28 17:23:29.111823 rlsdk_python-0.4.0/rlsdk_python/sdk.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 rlsdk_python-0.4.0/PKG-INFO
```

### Comparing `rlsdk_python-0.3.0/README.md` & `rlsdk_python-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.3.0/rlsdk_python/event_handling.py` & `rlsdk_python-0.4.0/rlsdk_python/event_handling.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.3.0/rlsdk_python/events.py` & `rlsdk_python-0.4.0/rlsdk_python/events.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.3.0/rlsdk_python/frida_script.py` & `rlsdk_python-0.4.0/rlsdk_python/frida_script.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.3.0/rlsdk_python/game_objects.py` & `rlsdk_python-0.4.0/rlsdk_python/game_objects.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.3.0/rlsdk_python/sdk.py` & `rlsdk_python-0.4.0/rlsdk_python/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,23 +48,23 @@
     "gnames_offset": None,
     "gobjects_offset": None,
 }
 
 
 class RLSDK:
 
-    def __init__(self, hook_player_tick=False):
+    def __init__(self, hook_player_tick=False, pid=None):
         
-
+        self.pid = pid
 
         self.config = DEFAULT_CONFIG
         
         try:
-            self.pm = pymem.Pymem(PROCESS_NAME)
-            self.frida = frida.attach(PROCESS_NAME)
+            self.pm = pymem.Pymem(self.pid if self.pid else PROCESS_NAME)
+            self.frida = frida.attach(self.pid if self.pid else PROCESS_NAME)
         except:
             raise Exception(Fore.RED + "Rocket League not found. Make sure Rocket League is running." + END)
 
 
         # open sdk_config.json file to read offsets
         
         try:
```

### Comparing `rlsdk_python-0.3.0/PKG-INFO` & `rlsdk_python-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlsdk_python
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: MarlburroW
 Author-email: nik0o@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

