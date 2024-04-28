# Comparing `tmp/zodchy_fastapi-0.1.1.tar.gz` & `tmp/zodchy_fastapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_fastapi-0.1.1.tar", max compression
+gzip compressed data, was "zodchy_fastapi-0.2.0.tar", max compression
```

## Comparing `zodchy_fastapi-0.1.1.tar` & `zodchy_fastapi-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.1.1/README.md
--rw-r--r--   0        0        0      467 2024-04-15 11:01:18.147303 zodchy_fastapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       58 2024-01-11 09:14:13.703189 zodchy_fastapi-0.1.1/zodchy_fastapi/__init__.py
--rw-r--r--   0        0        0      246 2024-04-02 15:23:42.896725 zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/__init__.py
--rw-r--r--   0        0        0     3424 2024-04-13 13:35:16.455663 zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/request.py
--rw-r--r--   0        0        0     1306 2024-04-13 13:35:16.447762 zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/response.py
--rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.1.1/zodchy_fastapi/handlers.py
--rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.1.1/zodchy_fastapi/router.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.2.0/README.md
+-rw-r--r--   0        0        0      467 2024-04-28 14:53:40.873008 zodchy_fastapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-01-11 09:14:13.703189 zodchy_fastapi-0.2.0/zodchy_fastapi/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-02 15:23:42.896725 zodchy_fastapi-0.2.0/zodchy_fastapi/contracts/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-28 14:53:40.865459 zodchy_fastapi-0.2.0/zodchy_fastapi/contracts/request.py
+-rw-r--r--   0        0        0     1306 2024-04-13 13:35:16.447762 zodchy_fastapi-0.2.0/zodchy_fastapi/contracts/response.py
+-rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.2.0/zodchy_fastapi/handlers.py
+-rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.2.0/zodchy_fastapi/router.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.2.0/PKG-INFO
```

### Comparing `zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/response.py` & `zodchy_fastapi-0.2.0/zodchy_fastapi/contracts/response.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.1.1/zodchy_fastapi/handlers.py` & `zodchy_fastapi-0.2.0/zodchy_fastapi/handlers.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.1.1/zodchy_fastapi/router.py` & `zodchy_fastapi-0.2.0/zodchy_fastapi/router.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.1.1/PKG-INFO` & `zodchy_fastapi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zodchy-fastapi
-Version: 0.1.1
+Version: 0.2.0
 Summary: Collection of tools to integrate fastapi to zodchy architecture
 Home-page: https://github.com/smairon/zodchy-fastapi
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.103.1,<0.104.0)
-Requires-Dist: zodchy (>=0.1.0,<0.2.0)
+Requires-Dist: zodchy (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/smairon/zodchy-fastapi
 Description-Content-Type: text/markdown
 
 # Zodchy fastapi
```

