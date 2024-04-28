# Comparing `tmp/dcentralab_auto_infra-1.1.0.tar.gz` & `tmp/dcentralab_auto_infra-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentralab_auto_infra-1.1.0.tar", last modified: Sun Apr 28 12:12:34 2024, max compression
+gzip compressed data, was "dcentralab_auto_infra-1.1.1.tar", last modified: Sun Apr 28 12:34:52 2024, max compression
```

## Comparing `dcentralab_auto_infra-1.1.0.tar` & `dcentralab_auto_infra-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:12:34.542432 dcentralab_auto_infra-1.1.0/
--rw-r--r--   0 bigsleep01   (501) staff       (20)     1073 2024-04-28 11:27:51.000000 dcentralab_auto_infra-1.1.0/LICENSE
--rw-r--r--   0 bigsleep01   (501) staff       (20)      317 2024-04-28 12:12:34.542161 dcentralab_auto_infra-1.1.0/PKG-INFO
--rw-r--r--   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:04:16.000000 dcentralab_auto_infra-1.1.0/README.md
-drwxr-xr-x   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:12:34.541831 dcentralab_auto_infra-1.1.0/dcentralab_auto_infra.egg-info/
--rw-r--r--   0 bigsleep01   (501) staff       (20)      317 2024-04-28 12:12:34.000000 dcentralab_auto_infra-1.1.0/dcentralab_auto_infra.egg-info/PKG-INFO
--rw-r--r--   0 bigsleep01   (501) staff       (20)      292 2024-04-28 12:12:34.000000 dcentralab_auto_infra-1.1.0/dcentralab_auto_infra.egg-info/SOURCES.txt
--rw-r--r--   0 bigsleep01   (501) staff       (20)        1 2024-04-28 12:12:34.000000 dcentralab_auto_infra-1.1.0/dcentralab_auto_infra.egg-info/dependency_links.txt
--rw-r--r--   0 bigsleep01   (501) staff       (20)      125 2024-04-28 12:12:34.000000 dcentralab_auto_infra-1.1.0/dcentralab_auto_infra.egg-info/requires.txt
--rw-r--r--   0 bigsleep01   (501) staff       (20)        1 2024-04-28 12:12:34.000000 dcentralab_auto_infra-1.1.0/dcentralab_auto_infra.egg-info/top_level.txt
--rw-r--r--   0 bigsleep01   (501) staff       (20)       38 2024-04-28 12:12:34.542487 dcentralab_auto_infra-1.1.0/setup.cfg
--rw-r--r--   0 bigsleep01   (501) staff       (20)      439 2024-04-28 12:12:29.000000 dcentralab_auto_infra-1.1.0/setup.py
-drwxr-xr-x   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:12:34.541242 dcentralab_auto_infra-1.1.0/tests/
--rw-r--r--   0 bigsleep01   (501) staff       (20)      799 2024-04-28 11:38:03.000000 dcentralab_auto_infra-1.1.0/tests/test_open_browser_with_extension.py
+drwxr-xr-x   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:34:52.084334 dcentralab_auto_infra-1.1.1/
+-rw-r--r--   0 bigsleep01   (501) staff       (20)     1073 2024-04-28 11:27:51.000000 dcentralab_auto_infra-1.1.1/LICENSE
+-rw-r--r--   0 bigsleep01   (501) staff       (20)      422 2024-04-28 12:34:52.084030 dcentralab_auto_infra-1.1.1/PKG-INFO
+-rw-r--r--   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:04:16.000000 dcentralab_auto_infra-1.1.1/README.md
+drwxr-xr-x   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:34:52.083697 dcentralab_auto_infra-1.1.1/dcentralab_auto_infra.egg-info/
+-rw-r--r--   0 bigsleep01   (501) staff       (20)      422 2024-04-28 12:34:52.000000 dcentralab_auto_infra-1.1.1/dcentralab_auto_infra.egg-info/PKG-INFO
+-rw-r--r--   0 bigsleep01   (501) staff       (20)      292 2024-04-28 12:34:52.000000 dcentralab_auto_infra-1.1.1/dcentralab_auto_infra.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsleep01   (501) staff       (20)        1 2024-04-28 12:34:52.000000 dcentralab_auto_infra-1.1.1/dcentralab_auto_infra.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsleep01   (501) staff       (20)      125 2024-04-28 12:34:52.000000 dcentralab_auto_infra-1.1.1/dcentralab_auto_infra.egg-info/requires.txt
+-rw-r--r--   0 bigsleep01   (501) staff       (20)        1 2024-04-28 12:34:52.000000 dcentralab_auto_infra-1.1.1/dcentralab_auto_infra.egg-info/top_level.txt
+-rw-r--r--   0 bigsleep01   (501) staff       (20)       38 2024-04-28 12:34:52.084386 dcentralab_auto_infra-1.1.1/setup.cfg
+-rw-r--r--   0 bigsleep01   (501) staff       (20)      554 2024-04-28 12:34:41.000000 dcentralab_auto_infra-1.1.1/setup.py
+drwxr-xr-x   0 bigsleep01   (501) staff       (20)        0 2024-04-28 12:34:52.083139 dcentralab_auto_infra-1.1.1/tests/
+-rw-r--r--   0 bigsleep01   (501) staff       (20)      799 2024-04-28 11:38:03.000000 dcentralab_auto_infra-1.1.1/tests/test_open_browser_with_extension.py
```

### Comparing `dcentralab_auto_infra-1.1.0/LICENSE` & `dcentralab_auto_infra-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_auto_infra-1.1.0/tests/test_open_browser_with_extension.py` & `dcentralab_auto_infra-1.1.1/tests/test_open_browser_with_extension.py`

 * *Files identical despite different names*

