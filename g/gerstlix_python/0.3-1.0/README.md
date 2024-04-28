# Comparing `tmp/gerstlix_python-0.3.tar.gz` & `tmp/gerstlix_python-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerstlix_python-0.3.tar", max compression
+gzip compressed data, was "gerstlix_python-1.0.tar", max compression
```

## Comparing `gerstlix_python-0.3.tar` & `gerstlix_python-1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      135 2024-02-09 11:44:27.278370 gerstlix_python-0.3/gerstlix_python/__init__.py
--rw-r--r--   0        0        0    10464 2024-04-22 15:23:28.897874 gerstlix_python-0.3/gerstlix_python/metods.py
--rw-r--r--   0        0        0      311 2024-04-22 15:26:58.288474 gerstlix_python-0.3/pyproject.toml
--rw-r--r--   0        0        0     2457 2024-04-22 15:25:56.091313 gerstlix_python-0.3/README.md
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 gerstlix_python-0.3/PKG-INFO
+-rw-r--r--   0        0        0      135 2024-02-09 11:44:27.278370 gerstlix_python-1.0/gerstlix_python/__init__.py
+-rw-r--r--   0        0        0    10466 2024-04-28 17:33:24.226637 gerstlix_python-1.0/gerstlix_python/metods.py
+-rw-r--r--   0        0        0      311 2024-04-28 17:34:31.902940 gerstlix_python-1.0/pyproject.toml
+-rw-r--r--   0        0        0     2457 2024-04-22 15:25:56.091313 gerstlix_python-1.0/README.md
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 gerstlix_python-1.0/PKG-INFO
```

### Comparing `gerstlix_python-0.3/gerstlix_python/metods.py` & `gerstlix_python-1.0/gerstlix_python/metods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-acceptServers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,101,102,103,201,202,203,204,205,206]
+acceptServers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,101,102,103,201,202,203,204,205,206,207]
 acceptServersArz = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28]
 acceptProject = ['arz', 'marz','rrp']
 
 
 class gerstlixAPI():
     def __init__(self, token:str=None):
         self.token = token
@@ -179,8 +179,8 @@
                     "serverName": data['data']['serverName'],
                     "lastUpdated": data['data']['lastUpdated'],
                     "terrs": terrs
                 }
             else:
                 return {"status": "fail", "errorMessage": data['message']}
         else:
-            return f"Сервер: {server} не находится в одобренном списке"
+            return f"Сервер: {server} не находится в одобренном списке"
```

### Comparing `gerstlix_python-0.3/README.md` & `gerstlix_python-1.0/README.md`

 * *Files identical despite different names*

### Comparing `gerstlix_python-0.3/PKG-INFO` & `gerstlix_python-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerstlix_python
-Version: 0.3
+Version: 1.0
 Summary: Library for simplified access to the Gerstlix API
 Author: travkacode
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

