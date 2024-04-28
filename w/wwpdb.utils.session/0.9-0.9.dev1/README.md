# Comparing `tmp/wwpdb.utils.session-0.9.tar.gz` & `tmp/wwpdb.utils.session-0.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wwpdb.utils.session-0.9.tar", last modified: Thu Apr 30 12:47:20 2020, max compression
+gzip compressed data, was "/Users/runner/runners/2.165.0/work/1/s/dist/wwpdb.utils.session-0.9.dev1.tar", last modified: Wed Feb 26 23:29:24 2020, max compression
```

## Comparing `wwpdb.utils.session-0.9.tar` & `wwpdb.utils.session-0.9.dev1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/
--rw-r--r--   0 peisach    (502) staff       (20)      747 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/PKG-INFO
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb/
--rw-r--r--   0 peisach    (502) staff       (20)       65 2018-10-14 11:42:07.000000 wwpdb.utils.session-0.9/wwpdb/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb/utils/
--rw-r--r--   0 peisach    (502) staff       (20)       65 2018-10-14 11:42:07.000000 wwpdb.utils.session-0.9/wwpdb/utils/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/
--rwxr-xr-x   0 peisach    (502) staff       (20)     4445 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/WebDownloadUtils.py
--rw-r--r--   0 peisach    (502) staff       (20)    12301 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/WebAppWorkerBase.py
--rw-r--r--   0 peisach    (502) staff       (20)     3369 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/SessionManager.py
--rw-r--r--   0 peisach    (502) staff       (20)    13286 2020-04-30 12:36:41.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/FileUtils.py
--rw-r--r--   0 peisach    (502) staff       (20)      149 2020-04-30 12:45:28.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/__init__.py
--rwxr-xr-x   0 peisach    (502) staff       (20)     9391 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/WebUploadUtils.py
--rw-r--r--   0 peisach    (502) staff       (20)     3984 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/UtilDataStore.py
--rw-r--r--   0 peisach    (502) staff       (20)    22250 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/wwpdb/utils/session/WebRequest.py
--rw-r--r--   0 peisach    (502) staff       (20)       74 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/README.md
--rwxr-xr-x   0 peisach    (502) staff       (20)     1997 2020-01-22 01:06:14.000000 wwpdb.utils.session-0.9/setup.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)      747 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)        1 2020-01-08 19:15:39.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/not-zip-safe
--rw-r--r--   0 peisach    (502) staff       (20)      664 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)       20 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       67 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)        6 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)      108 2020-04-30 12:47:20.000000 wwpdb.utils.session-0.9/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/
+-rw-r--r--   0 runner     (501) staff       (20)      752 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/wwpdb/
+-rw-r--r--   0 runner     (501) staff       (20)       65 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/
+-rw-r--r--   0 runner     (501) staff       (20)       65 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/
+-rwxr-xr-x   0 runner     (501) staff       (20)     4445 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebDownloadUtils.py
+-rw-r--r--   0 runner     (501) staff       (20)    12301 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebAppWorkerBase.py
+-rw-r--r--   0 runner     (501) staff       (20)     3369 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/SessionManager.py
+-rw-r--r--   0 runner     (501) staff       (20)    13286 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/FileUtils.py
+-rw-r--r--   0 runner     (501) staff       (20)      154 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     9391 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebUploadUtils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3984 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/UtilDataStore.py
+-rw-r--r--   0 runner     (501) staff       (20)    22250 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebRequest.py
+-rw-r--r--   0 runner     (501) staff       (20)       74 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/README.md
+-rwxr-xr-x   0 runner     (501) staff       (20)     1997 2020-02-26 23:27:57.000000 wwpdb.utils.session-0.9.dev1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      752 2020-02-26 23:29:23.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)        1 2020-02-26 23:28:44.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      664 2020-02-26 23:29:23.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)       20 2020-02-26 23:29:23.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       67 2020-02-26 23:29:23.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2020-02-26 23:29:23.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2020-02-26 23:29:23.000000 wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      108 2020-02-26 23:29:24.000000 wwpdb.utils.session-0.9.dev1/setup.cfg
```

### Comparing `wwpdb.utils.session-0.9/PKG-INFO` & `wwpdb.utils.session-0.9.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.session
-Version: 0.9
+Version: 0.9.dev1
 Summary: wwPDB session support
 Home-page: https://github.com/rcsb/py-wwpdb_utils_session
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Description: See:  README.md
 Platform: UNKNOWN
```

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/WebDownloadUtils.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/WebAppWorkerBase.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebAppWorkerBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/SessionManager.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/SessionManager.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/FileUtils.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/FileUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/WebUploadUtils.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebUploadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/UtilDataStore.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/UtilDataStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb/utils/session/WebRequest.py` & `wwpdb.utils.session-0.9.dev1/wwpdb/utils/session/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/setup.py` & `wwpdb.utils.session-0.9.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/PKG-INFO` & `wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.session
-Version: 0.9
+Version: 0.9.dev1
 Summary: wwPDB session support
 Home-page: https://github.com/rcsb/py-wwpdb_utils_session
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Description: See:  README.md
 Platform: UNKNOWN
```

### Comparing `wwpdb.utils.session-0.9/wwpdb.utils.session.egg-info/SOURCES.txt` & `wwpdb.utils.session-0.9.dev1/wwpdb.utils.session.egg-info/SOURCES.txt`

 * *Files identical despite different names*

