# Comparing `tmp/CachedFileDic-0.2.3.tar.gz` & `tmp/CachedFileDic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CachedFileDic-0.2.3.tar", last modified: Sun Apr 21 12:20:49 2024, max compression
+gzip compressed data, was "CachedFileDic-0.2.4.tar", last modified: Sun Apr 28 04:49:08 2024, max compression
```

## Comparing `CachedFileDic-0.2.3.tar` & `CachedFileDic-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 12:20:49.991942 CachedFileDic-0.2.3/
-drwxrwxrwx   0        0        0        0 2024-04-21 12:20:49.975672 CachedFileDic-0.2.3/CachedFileDic/
--rw-rw-rw-   0        0        0     6952 2024-04-21 12:19:52.000000 CachedFileDic-0.2.3/CachedFileDic/__init__.py
--rw-rw-rw-   0        0        0     6595 2024-04-21 12:19:39.000000 CachedFileDic-0.2.3/CachedFileDic/__init__BACKUP_commit効率化変更前.py
--rw-rw-rw-   0        0        0      833 2024-03-07 09:47:59.000000 CachedFileDic-0.2.3/CachedFileDic/test.py
-drwxrwxrwx   0        0        0        0 2024-04-21 12:20:49.985436 CachedFileDic-0.2.3/CachedFileDic.egg-info/
--rw-rw-rw-   0        0        0     8550 2024-04-21 12:20:49.000000 CachedFileDic-0.2.3/CachedFileDic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-21 12:20:49.000000 CachedFileDic-0.2.3/CachedFileDic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 12:20:49.000000 CachedFileDic-0.2.3/CachedFileDic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-21 12:20:49.000000 CachedFileDic-0.2.3/CachedFileDic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 12:20:49.000000 CachedFileDic-0.2.3/CachedFileDic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8550 2024-04-21 12:20:49.991942 CachedFileDic-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     6931 2023-12-22 09:17:16.000000 CachedFileDic-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 12:20:49.991942 CachedFileDic-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-21 12:20:45.000000 CachedFileDic-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:49:08.808802 CachedFileDic-0.2.4/
+drwxrwxrwx   0        0        0        0 2024-04-28 04:49:08.793351 CachedFileDic-0.2.4/CachedFileDic/
+-rw-rw-rw-   0        0        0     7210 2024-04-28 04:47:25.000000 CachedFileDic-0.2.4/CachedFileDic/__init__.py
+-rw-rw-rw-   0        0        0     6595 2024-04-28 04:45:05.000000 CachedFileDic-0.2.4/CachedFileDic/__init__BACKUP_commit効率化変更前.py
+-rw-rw-rw-   0        0        0     6952 2024-04-25 01:06:02.000000 CachedFileDic-0.2.4/CachedFileDic/__init__BACKUP_lazy_commitバグあり版.py
+-rw-rw-rw-   0        0        0      833 2024-03-11 04:00:17.000000 CachedFileDic-0.2.4/CachedFileDic/test.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:49:08.807802 CachedFileDic-0.2.4/CachedFileDic.egg-info/
+-rw-rw-rw-   0        0        0     7310 2024-04-28 04:49:08.000000 CachedFileDic-0.2.4/CachedFileDic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-04-28 04:49:08.000000 CachedFileDic-0.2.4/CachedFileDic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 04:49:08.000000 CachedFileDic-0.2.4/CachedFileDic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-28 04:49:08.000000 CachedFileDic-0.2.4/CachedFileDic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-28 04:49:08.000000 CachedFileDic-0.2.4/CachedFileDic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7310 2024-04-28 04:49:08.807802 CachedFileDic-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6931 2023-12-23 00:25:59.000000 CachedFileDic-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 04:49:08.808802 CachedFileDic-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-28 04:48:51.000000 CachedFileDic-0.2.4/setup.py
```

### Comparing `CachedFileDic-0.2.3/CachedFileDic/__init__.py` & `CachedFileDic-0.2.4/CachedFileDic/__init__BACKUP_lazy_commitバグあり版.py`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.3/CachedFileDic/__init__BACKUP_commit効率化変更前.py` & `CachedFileDic-0.2.4/CachedFileDic/__init__BACKUP_commit効率化変更前.py`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.3/CachedFileDic/test.py` & `CachedFileDic-0.2.4/CachedFileDic/test.py`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.3/README.md` & `CachedFileDic-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.3/setup.py` & `CachedFileDic-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 4361 6368 6564 4669  develop_CachedFi
 000000c0: 6c65 4469 632f 2229 2061 7320 703a 0d0a  leDic/") as p:..
 000000d0: 0973 6574 7570 280d 0a09 096e 616d 6520  .setup(....name 
 000000e0: 3d20 2243 6163 6865 6446 696c 6544 6963  = "CachedFileDic
 000000f0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-00000100: 2230 2e32 2e33 222c 0d0a 0909 6465 7363  "0.2.3",....desc
+00000100: 2230 2e32 2e34 222c 0d0a 0909 6465 7363  "0.2.4",....desc
 00000110: 7269 7074 696f 6e20 3d20 2246 6173 7420  ription = "Fast 
 00000120: 4469 6374 696f 6e61 7279 2d54 7970 6520  Dictionary-Type 
 00000130: 4461 7461 6261 7365 222c 0d0a 0909 6175  Database",....au
 00000140: 7468 6f72 203d 2022 6269 625f 696e 6622  thor = "bib_inf"
 00000150: 2c0d 0a09 0961 7574 686f 725f 656d 6169  ,....author_emai
 00000160: 6c20 3d20 2263 6f6e 7461 6374 2e62 6962  l = "contact.bib
 00000170: 696e 6640 676d 6169 6c2e 636f 6d22 2c0d  inf@gmail.com",.
```

