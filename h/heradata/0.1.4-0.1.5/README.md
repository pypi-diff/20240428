# Comparing `tmp/HeraData-0.1.4.tar.gz` & `tmp/heradata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HeraData-0.1.4.tar", last modified: Fri Apr 26 13:07:33 2024, max compression
+gzip compressed data, was "heradata-0.1.5.tar", last modified: Sun Apr 28 01:54:14 2024, max compression
```

## Comparing `HeraData-0.1.4.tar` & `heradata-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 13:07:33.781665 HeraData-0.1.4/
--rw-rw-r--   0 mark      (1000) mark      (1000)      129 2024-04-23 01:24:54.000000 HeraData-0.1.4/.gitignore
--rw-rw-r--   0 mark      (1000) mark      (1000)      104 2024-04-22 07:50:16.000000 HeraData-0.1.4/.gitmodules
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 13:07:33.781665 HeraData-0.1.4/HeraData.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-26 13:07:33.000000 HeraData-0.1.4/HeraData.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      295 2024-04-26 13:07:33.000000 HeraData-0.1.4/HeraData.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 13:07:33.000000 HeraData-0.1.4/HeraData.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-26 13:07:33.000000 HeraData-0.1.4/HeraData.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 13:07:33.000000 HeraData-0.1.4/HeraData.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-26 13:07:33.781665 HeraData-0.1.4/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-22 09:32:31.000000 HeraData-0.1.4/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 13:07:33.781665 HeraData-0.1.4/hera/
--rw-rw-r--   0 mark      (1000) mark      (1000)      628 2024-04-26 13:06:42.000000 HeraData-0.1.4/hera/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       21 2024-04-23 02:00:27.000000 HeraData-0.1.4/requirements.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       79 2024-04-26 13:07:33.781665 HeraData-0.1.4/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      377 2024-04-26 13:07:27.000000 HeraData-0.1.4/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 13:07:33.781665 HeraData-0.1.4/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)      811 2024-04-23 06:10:33.000000 HeraData-0.1.4/tests/test___init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1167 2024-04-23 06:11:38.000000 HeraData-0.1.4/tests/test__data_storage.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:54:14.710078 heradata-0.1.5/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      129 2024-04-23 01:24:54.000000 heradata-0.1.5/.gitignore
+-rw-rw-r--   0 mark      (1000) mark      (1000)      104 2024-04-22 07:50:16.000000 heradata-0.1.5/.gitmodules
+-rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-28 01:54:14.710078 heradata-0.1.5/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-22 09:32:31.000000 heradata-0.1.5/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:54:14.710078 heradata-0.1.5/heradata/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      628 2024-04-26 13:06:42.000000 heradata-0.1.5/heradata/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:54:14.710078 heradata-0.1.5/heradata.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-28 01:54:14.000000 heradata-0.1.5/heradata.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      299 2024-04-28 01:54:14.000000 heradata-0.1.5/heradata.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 01:54:14.000000 heradata-0.1.5/heradata.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-28 01:54:14.000000 heradata-0.1.5/heradata.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        9 2024-04-28 01:54:14.000000 heradata-0.1.5/heradata.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       21 2024-04-23 02:00:27.000000 heradata-0.1.5/requirements.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       79 2024-04-28 01:54:14.710078 heradata-0.1.5/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      377 2024-04-28 01:54:04.000000 heradata-0.1.5/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:54:14.710078 heradata-0.1.5/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      811 2024-04-23 06:10:33.000000 heradata-0.1.5/tests/test___init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1167 2024-04-23 06:11:38.000000 heradata-0.1.5/tests/test__data_storage.py
```

### Comparing `HeraData-0.1.4/hera/__init__.py` & `heradata-0.1.5/heradata/__init__.py`

 * *Files identical despite different names*

### Comparing `HeraData-0.1.4/tests/test___init__.py` & `heradata-0.1.5/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `HeraData-0.1.4/tests/test__data_storage.py` & `heradata-0.1.5/tests/test__data_storage.py`

 * *Files identical despite different names*

