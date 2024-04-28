# Comparing `tmp/fastnorm-24.4.tar.gz` & `tmp/fastnorm-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastnorm-24.4.tar", last modified: Sun Apr 28 14:00:00 2024, max compression
+gzip compressed data, was "fastnorm-24.4.1.tar", last modified: Sun Apr 28 15:09:06 2024, max compression
```

## Comparing `fastnorm-24.4.tar` & `fastnorm-24.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 martins   (1000) martins   (1001)        0 2024-04-28 14:00:00.207096 fastnorm-24.4/
--rw-r--r--   0 martins   (1000) martins   (1001)     1494 2024-04-28 12:37:55.000000 fastnorm-24.4/LICENSE
--rw-r--r--   0 martins   (1000) martins   (1001)      245 2024-04-28 14:00:00.207096 fastnorm-24.4/PKG-INFO
--rw-r--r--   0 martins   (1000) martins   (1001)     3084 2024-04-28 12:37:55.000000 fastnorm-24.4/README.md
-drwxr-xr-x   0 martins   (1000) martins   (1001)        0 2024-04-28 14:00:00.207096 fastnorm-24.4/fastnorm/
--rw-r--r--   0 martins   (1000) martins   (1001)       90 2024-04-28 12:37:55.000000 fastnorm-24.4/fastnorm/__init__.py
--rw-r--r--   0 martins   (1000) martins   (1001)    12774 2024-04-28 12:37:55.000000 fastnorm-24.4/fastnorm/bvnorm.py
--rw-r--r--   0 martins   (1000) martins   (1001)      981 2024-04-28 12:37:55.000000 fastnorm-24.4/fastnorm/util.py
-drwxr-xr-x   0 martins   (1000) martins   (1001)        0 2024-04-28 14:00:00.207096 fastnorm-24.4/fastnorm.egg-info/
--rw-r--r--   0 martins   (1000) martins   (1001)      245 2024-04-28 14:00:00.000000 fastnorm-24.4/fastnorm.egg-info/PKG-INFO
--rw-r--r--   0 martins   (1000) martins   (1001)      260 2024-04-28 14:00:00.000000 fastnorm-24.4/fastnorm.egg-info/SOURCES.txt
--rw-r--r--   0 martins   (1000) martins   (1001)        1 2024-04-28 14:00:00.000000 fastnorm-24.4/fastnorm.egg-info/dependency_links.txt
--rw-r--r--   0 martins   (1000) martins   (1001)       24 2024-04-28 14:00:00.000000 fastnorm-24.4/fastnorm.egg-info/requires.txt
--rw-r--r--   0 martins   (1000) martins   (1001)        9 2024-04-28 14:00:00.000000 fastnorm-24.4/fastnorm.egg-info/top_level.txt
--rw-r--r--   0 martins   (1000) martins   (1001)       38 2024-04-28 14:00:00.207096 fastnorm-24.4/setup.cfg
--rw-r--r--   0 martins   (1000) martins   (1001)      364 2024-04-28 12:37:55.000000 fastnorm-24.4/setup.py
-drwxr-xr-x   0 martins   (1000) martins   (1001)        0 2024-04-28 14:00:00.207096 fastnorm-24.4/tests/
--rw-r--r--   0 martins   (1000) martins   (1001)     1756 2024-04-28 12:37:55.000000 fastnorm-24.4/tests/test_bvn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:06.971628 fastnorm-24.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-28 15:08:59.000000 fastnorm-24.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-28 15:09:06.971628 fastnorm-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-28 15:08:59.000000 fastnorm-24.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:06.967627 fastnorm-24.4.1/fastnorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 15:08:59.000000 fastnorm-24.4.1/fastnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-04-28 15:08:59.000000 fastnorm-24.4.1/fastnorm/bvnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-28 15:08:59.000000 fastnorm-24.4.1/fastnorm/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:06.971628 fastnorm-24.4.1/fastnorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-28 15:09:06.000000 fastnorm-24.4.1/fastnorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-28 15:09:06.000000 fastnorm-24.4.1/fastnorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:09:06.000000 fastnorm-24.4.1/fastnorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 15:09:06.000000 fastnorm-24.4.1/fastnorm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 15:09:06.000000 fastnorm-24.4.1/fastnorm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:09:06.971628 fastnorm-24.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-28 15:08:59.000000 fastnorm-24.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:06.971628 fastnorm-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-28 15:08:59.000000 fastnorm-24.4.1/tests/test_bvn.py
```

### Comparing `fastnorm-24.4/LICENSE` & `fastnorm-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastnorm-24.4/README.md` & `fastnorm-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastnorm-24.4/fastnorm/bvnorm.py` & `fastnorm-24.4.1/fastnorm/bvnorm.py`

 * *Files identical despite different names*

### Comparing `fastnorm-24.4/fastnorm/util.py` & `fastnorm-24.4.1/fastnorm/util.py`

 * *Files identical despite different names*

### Comparing `fastnorm-24.4/tests/test_bvn.py` & `fastnorm-24.4.1/tests/test_bvn.py`

 * *Files identical despite different names*

