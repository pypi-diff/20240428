# Comparing `tmp/dslog-0.1.1.tar.gz` & `tmp/dslog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslog-0.1.1.tar", last modified: Fri Apr 26 12:13:15 2024, max compression
+gzip compressed data, was "dslog-0.1.2.tar", last modified: Sun Apr 28 14:49:07 2024, max compression
```

## Comparing `dslog-0.1.1.tar` & `dslog-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.084415 dslog-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-04-26 12:13:15.074415 dslog-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-20 07:49:44.000000 dslog-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      544 2024-04-26 12:13:11.000000 dslog-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-26 12:13:15.084415 dslog-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-20 07:42:14.000000 dslog-0.1.1/src/dslog/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1604 2024-04-26 12:12:47.000000 dslog-0.1.1/src/dslog/logger.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog/loggers/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-20 06:37:47.000000 dslog-0.1.1/src/dslog/loggers/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-04-20 06:38:28.000000 dslog-0.1.1/src/dslog/loggers/loggers.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-04-20 07:41:22.000000 dslog-0.1.1/src/dslog/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 05:24:05.000000 dslog-0.1.1/src/dslog/util/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-04-20 08:13:09.000000 dslog-0.1.1/src/dslog/util/uvicorn.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      361 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.865913 dslog-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-04-28 14:49:07.865913 dslog-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-20 07:49:44.000000 dslog-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      544 2024-04-28 14:49:05.000000 dslog-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-28 14:49:07.865913 dslog-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.855914 dslog-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.865913 dslog-0.1.2/src/dslog/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-20 07:42:14.000000 dslog-0.1.2/src/dslog/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.865913 dslog-0.1.2/src/dslog/formatters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-28 14:44:10.000000 dslog-0.1.2/src/dslog/formatters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      108 2024-04-28 14:43:16.000000 dslog-0.1.2/src/dslog/formatters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      437 2024-04-28 14:41:12.000000 dslog-0.1.2/src/dslog/formatters/formatters.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2075 2024-04-28 14:47:47.000000 dslog-0.1.2/src/dslog/logger.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.865913 dslog-0.1.2/src/dslog/loggers/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-28 14:45:49.000000 dslog-0.1.2/src/dslog/loggers/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-04-28 14:45:41.000000 dslog-0.1.2/src/dslog/loggers/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-04-20 06:38:28.000000 dslog-0.1.2/src/dslog/loggers/_file.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       99 2024-04-28 14:47:22.000000 dslog-0.1.2/src/dslog/loggers/_rich.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-04-20 07:41:22.000000 dslog-0.1.2/src/dslog/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.865913 dslog-0.1.2/src/dslog/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 05:24:05.000000 dslog-0.1.2/src/dslog/util/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-04-20 08:13:09.000000 dslog-0.1.2/src/dslog/util/uvicorn.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 14:49:07.865913 dslog-0.1.2/src/dslog.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-04-28 14:49:07.000000 dslog-0.1.2/src/dslog.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-04-28 14:49:07.000000 dslog-0.1.2/src/dslog.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-28 14:49:07.000000 dslog-0.1.2/src/dslog.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-28 14:49:07.000000 dslog-0.1.2/src/dslog.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-28 14:49:07.000000 dslog-0.1.2/src/dslog.egg-info/top_level.txt
```

### Comparing `dslog-0.1.1/PKG-INFO` & `dslog-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dslog
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dead-simple logging: just function composition
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: rich
 Requires-Dist: rich; extra == "rich"
```

### Comparing `dslog-0.1.1/pyproject.toml` & `dslog-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dslog"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Dead-simple logging: just function composition"
 dependencies = [
   
 ]
```

### Comparing `dslog-0.1.1/src/dslog/types.py` & `dslog-0.1.2/src/dslog/types.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.1/src/dslog/util/uvicorn.py` & `dslog-0.1.2/src/dslog/util/uvicorn.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.1/src/dslog.egg-info/PKG-INFO` & `dslog-0.1.2/src/dslog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dslog
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dead-simple logging: just function composition
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: rich
 Requires-Dist: rich; extra == "rich"
```

