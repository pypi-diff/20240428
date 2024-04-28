# Comparing `tmp/vicregaddon-0.0.1.tar.gz` & `tmp/vicregaddon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicregaddon-0.0.1.tar", last modified: Sun Apr 28 00:08:56 2024, max compression
+gzip compressed data, was "vicregaddon-0.0.2.tar", last modified: Sun Apr 28 00:15:34 2024, max compression
```

## Comparing `vicregaddon-0.0.1.tar` & `vicregaddon-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:08:56.784558 vicregaddon-0.0.1/
--rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-06-04 17:06:51.000000 vicregaddon-0.0.1/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)      266 2024-04-28 00:08:56.784422 vicregaddon-0.0.1/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      700 2024-04-28 00:06:00.000000 vicregaddon-0.0.1/README.md
--rw-r--r--   0 shawley    (501) staff       (20)       38 2024-04-28 00:08:56.784616 vicregaddon-0.0.1/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)      406 2023-06-04 22:51:36.000000 vicregaddon-0.0.1/setup.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:08:56.783262 vicregaddon-0.0.1/vicregaddon/
--rw-r--r--   0 shawley    (501) staff       (20)       28 2023-06-04 20:31:47.000000 vicregaddon-0.0.1/vicregaddon/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)    11820 2024-04-28 00:07:13.000000 vicregaddon-0.0.1/vicregaddon/vicregaddon.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:08:56.784182 vicregaddon-0.0.1/vicregaddon.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)      266 2024-04-28 00:08:56.000000 vicregaddon-0.0.1/vicregaddon.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      251 2024-04-28 00:08:56.000000 vicregaddon-0.0.1/vicregaddon.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2024-04-28 00:08:56.000000 vicregaddon-0.0.1/vicregaddon.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)       13 2024-04-28 00:08:56.000000 vicregaddon-0.0.1/vicregaddon.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)       12 2024-04-28 00:08:56.000000 vicregaddon-0.0.1/vicregaddon.egg-info/top_level.txt
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:15:34.104058 vicregaddon-0.0.2/
+-rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-06-04 17:06:51.000000 vicregaddon-0.0.2/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)     1076 2024-04-28 00:15:34.103928 vicregaddon-0.0.2/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      700 2024-04-28 00:06:00.000000 vicregaddon-0.0.2/README.md
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2024-04-28 00:15:34.104104 vicregaddon-0.0.2/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)      699 2024-04-28 00:15:31.000000 vicregaddon-0.0.2/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:15:34.103036 vicregaddon-0.0.2/vicregaddon/
+-rw-r--r--   0 shawley    (501) staff       (20)       28 2023-06-04 20:31:47.000000 vicregaddon-0.0.2/vicregaddon/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)    11820 2024-04-28 00:07:13.000000 vicregaddon-0.0.2/vicregaddon/vicregaddon.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2024-04-28 00:15:34.103745 vicregaddon-0.0.2/vicregaddon.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     1076 2024-04-28 00:15:34.000000 vicregaddon-0.0.2/vicregaddon.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      251 2024-04-28 00:15:34.000000 vicregaddon-0.0.2/vicregaddon.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2024-04-28 00:15:34.000000 vicregaddon-0.0.2/vicregaddon.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       13 2024-04-28 00:15:34.000000 vicregaddon-0.0.2/vicregaddon.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       12 2024-04-28 00:15:34.000000 vicregaddon-0.0.2/vicregaddon.egg-info/top_level.txt
```

### Comparing `vicregaddon-0.0.1/LICENSE` & `vicregaddon-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vicregaddon-0.0.1/README.md` & `vicregaddon-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vicregaddon-0.0.1/vicregaddon/vicregaddon.py` & `vicregaddon-0.0.2/vicregaddon/vicregaddon.py`

 * *Files identical despite different names*

