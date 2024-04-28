# Comparing `tmp/kaychen-0.1.2.tar.gz` & `tmp/kaychen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaychen-0.1.2.tar", last modified: Thu Apr 25 18:39:14 2024, max compression
+gzip compressed data, was "kaychen-0.1.3.tar", last modified: Sun Apr 28 18:13:11 2024, max compression
```

## Comparing `kaychen-0.1.2.tar` & `kaychen-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 18:39:14.404065 kaychen-0.1.2/
--rw-r--r--   0 kay       (1000) users      (984)      810 2024-04-25 18:39:14.404065 kaychen-0.1.2/PKG-INFO
-drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 18:39:14.400732 kaychen-0.1.2/kaychen/
--rw-r--r--   0 kay       (1000) users      (984)        0 2024-04-25 18:17:40.000000 kaychen-0.1.2/kaychen/__init__.py
--rw-r--r--   0 kay       (1000) users      (984)     3682 2024-04-25 15:50:52.000000 kaychen-0.1.2/kaychen/api.py
--rw-r--r--   0 kay       (1000) users      (984)      669 2024-04-25 08:15:59.000000 kaychen-0.1.2/kaychen/middleware.py
--rw-r--r--   0 kay       (1000) users      (984)     1093 2024-04-25 10:01:54.000000 kaychen-0.1.2/kaychen/response.py
-drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 18:39:14.400732 kaychen-0.1.2/kaychen.egg-info/
--rw-r--r--   0 kay       (1000) users      (984)      810 2024-04-25 18:39:14.000000 kaychen-0.1.2/kaychen.egg-info/PKG-INFO
--rw-r--r--   0 kay       (1000) users      (984)      239 2024-04-25 18:39:14.000000 kaychen-0.1.2/kaychen.egg-info/SOURCES.txt
--rw-r--r--   0 kay       (1000) users      (984)        1 2024-04-25 18:39:14.000000 kaychen-0.1.2/kaychen.egg-info/dependency_links.txt
--rw-r--r--   0 kay       (1000) users      (984)      105 2024-04-25 18:39:14.000000 kaychen-0.1.2/kaychen.egg-info/requires.txt
--rw-r--r--   0 kay       (1000) users      (984)        8 2024-04-25 18:39:14.000000 kaychen-0.1.2/kaychen.egg-info/top_level.txt
--rw-r--r--   0 kay       (1000) users      (984)       38 2024-04-25 18:39:14.404065 kaychen-0.1.2/setup.cfg
--rw-r--r--   0 kay       (1000) users      (984)     4014 2024-04-25 18:37:42.000000 kaychen-0.1.2/setup.py
+drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-28 18:13:11.543379 kaychen-0.1.3/
+-rw-r--r--   0 kay       (1000) users      (984)    17162 2024-04-28 18:13:11.543379 kaychen-0.1.3/PKG-INFO
+-rw-r--r--   0 kay       (1000) users      (984)    16461 2024-04-26 18:17:21.000000 kaychen-0.1.3/README.md
+drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-28 18:13:11.540045 kaychen-0.1.3/kaychen/
+-rw-r--r--   0 kay       (1000) users      (984)        0 2024-04-25 18:17:40.000000 kaychen-0.1.3/kaychen/__init__.py
+-rw-r--r--   0 kay       (1000) users      (984)     3682 2024-04-25 15:50:52.000000 kaychen-0.1.3/kaychen/api.py
+-rw-r--r--   0 kay       (1000) users      (984)      669 2024-04-25 08:15:59.000000 kaychen-0.1.3/kaychen/middleware.py
+-rw-r--r--   0 kay       (1000) users      (984)     6242 2024-04-28 18:11:55.000000 kaychen-0.1.3/kaychen/orm.py
+-rw-r--r--   0 kay       (1000) users      (984)     1093 2024-04-25 10:01:54.000000 kaychen-0.1.3/kaychen/response.py
+drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-28 18:13:11.543379 kaychen-0.1.3/kaychen.egg-info/
+-rw-r--r--   0 kay       (1000) users      (984)    17162 2024-04-28 18:13:11.000000 kaychen-0.1.3/kaychen.egg-info/PKG-INFO
+-rw-r--r--   0 kay       (1000) users      (984)      264 2024-04-28 18:13:11.000000 kaychen-0.1.3/kaychen.egg-info/SOURCES.txt
+-rw-r--r--   0 kay       (1000) users      (984)        1 2024-04-28 18:13:11.000000 kaychen-0.1.3/kaychen.egg-info/dependency_links.txt
+-rw-r--r--   0 kay       (1000) users      (984)      105 2024-04-28 18:13:11.000000 kaychen-0.1.3/kaychen.egg-info/requires.txt
+-rw-r--r--   0 kay       (1000) users      (984)        8 2024-04-28 18:13:11.000000 kaychen-0.1.3/kaychen.egg-info/top_level.txt
+-rw-r--r--   0 kay       (1000) users      (984)       38 2024-04-28 18:13:11.543379 kaychen-0.1.3/setup.cfg
+-rw-r--r--   0 kay       (1000) users      (984)     4014 2024-04-28 18:12:43.000000 kaychen-0.1.3/setup.py
```

### Comparing `kaychen-0.1.2/kaychen/api.py` & `kaychen-0.1.3/kaychen/api.py`

 * *Files identical despite different names*

### Comparing `kaychen-0.1.2/kaychen/middleware.py` & `kaychen-0.1.3/kaychen/middleware.py`

 * *Files identical despite different names*

### Comparing `kaychen-0.1.2/kaychen/response.py` & `kaychen-0.1.3/kaychen/response.py`

 * *Files identical despite different names*

### Comparing `kaychen-0.1.2/setup.py` & `kaychen-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "kaychen"
 DESCRIPTION = "This is a web framework build while completing the course https://testdriven.io/courses/python-web-framework/"
 URL = "https://github.com/Keisn1/web-framework-python.git"
 EMAIL = "kay.freyer@icloud.com"
 AUTHOR = "Kay Freyer"
 REQUIRES_PYTHON = ">=3.11.0"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.3",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

