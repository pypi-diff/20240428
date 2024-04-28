# Comparing `tmp/pygmtsar-2024.4.17.post1.tar.gz` & `tmp/pygmtsar-2024.4.17.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.4.17.post1.tar", last modified: Fri Apr 26 16:33:42 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.post2.tar", last modified: Sun Apr 28 10:50:08 2024, max compression
```

## Comparing `pygmtsar-2024.4.17.post1.tar` & `pygmtsar-2024.4.17.post2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-26 16:33:42.230689 pygmtsar-2024.4.17.post1/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post1/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-26 16:33:42.230375 pygmtsar-2024.4.17.post1/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post1/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-26 16:33:42.228724 pygmtsar-2024.4.17.post1/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post1/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post1/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post1/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post1/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post1/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post1/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post1/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     9103 2024-04-26 15:00:33.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    26654 2024-04-11 05:08:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17.post1/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post1/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-04-26 15:55:09.000000 pygmtsar-2024.4.17.post1/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post1/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post1/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post1/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post1/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-26 16:33:42.230076 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-26 16:33:42.230749 pygmtsar-2024.4.17.post1/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post1/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-28 10:50:08.169320 pygmtsar-2024.4.17.post2/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post2/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-28 10:50:08.169031 pygmtsar-2024.4.17.post2/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post2/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-28 10:50:08.167301 pygmtsar-2024.4.17.post2/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post2/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post2/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post2/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post2/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post2/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post2/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post2/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post2/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9103 2024-04-26 15:00:33.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post2/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17.post2/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post2/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-04-28 10:49:46.000000 pygmtsar-2024.4.17.post2/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post2/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post2/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post2/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post2/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-28 10:50:08.168640 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-28 10:50:08.169374 pygmtsar-2024.4.17.post2/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post2/setup.py
```

### Comparing `pygmtsar-2024.4.17.post1/LICENSE.txt` & `pygmtsar-2024.4.17.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/PKG-INFO` & `pygmtsar-2024.4.17.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post1
+Version: 2024.4.17.post2
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post1/README.md` & `pygmtsar-2024.4.17.post2/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/ASF.py` & `pygmtsar-2024.4.17.post2/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/AWS.py` & `pygmtsar-2024.4.17.post2/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/GMT.py` & `pygmtsar-2024.4.17.post2/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/IO.py` & `pygmtsar-2024.4.17.post2/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17.post2/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/PRM.py` & `pygmtsar-2024.4.17.post2/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17.post2/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/S1.py` & `pygmtsar-2024.4.17.post2/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_sbas.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,26 +216,32 @@
         # import directive is not compatible to numba
         #import numpy as np
     
         assert data.ndim   == 1
         assert weight.ndim == 1 or weight.ndim == 0
         assert matrix.ndim == 2
         assert data.shape[0] == matrix.shape[0]
-    
+        
+        # for now, xr.apply_ufunc always call specified function with float64 arguments
+        # this error should be resolved controlling the output datatype
+        #assert data.dtype   == np.float32, f'ERROR: data argument should be float32 array but it is {data.dtype}'
+        #assert weight.dtype == np.float32, f'ERROR: weight argument should be float32 array but it is {weight.dtype}'
+
         if np.all(np.isnan(data)) or (weight.size != 0 and np.all(np.isnan(weight))):
             return np.full(data.size, np.nan, dtype=np.float32)
     
         nanmask = np.isnan(data)
         if weight.size != 0:
             nanmask = nanmask | np.isnan(weight)
         if np.all(nanmask):
             # no valid input data
             return np.full(data.size, np.nan, dtype=np.float32)
     
         # the buffer variable will be modified
+        # buffer datatype is the same as input data datatype
         buffer = data[~nanmask].copy()
         if weight.size != 0:
             weight = weight[~nanmask]
     
         # exclude matrix records for not valid data
         matrix = matrix[~nanmask,:]
         pair_sum = matrix.sum(axis=1)
@@ -359,15 +365,16 @@
                     pairs_ok.append(pair_idx)
                     pairs_ok.extend(np.where(matching_rows)[0])
                 #print ()
                 #break
     
         # return original values when unwrapping is not possible at all
         if len(pairs_ok) == 0:
-            return buffer
+            # buffer datatype is the same as input data datatype
+            return buffer.astype(np.float32)
         # return unwrapped values
         # validity mask
         mask = [idx in pairs_ok for idx in range(buffer.size)]
         #mask = np.isin(np.arange(buffer.size), pairs_ok)
         # output is the same size as input
         #out = np.nan * np.zeros(data.size)
         out = np.full(data.size, np.nan, dtype=np.float32)
```

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17.post2/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17.post2/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17.post2/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/__init__.py` & `pygmtsar-2024.4.17.post2/pygmtsar/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.4.17.post1'
+__version__ = '2024.4.17.post2'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17.post2/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17.post2/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17.post2/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar/utils.py` & `pygmtsar-2024.4.17.post2/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17.post2/pygmtsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post1
+Version: 2024.4.17.post2
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post1/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17.post2/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post1/setup.py` & `pygmtsar-2024.4.17.post2/setup.py`

 * *Files identical despite different names*

