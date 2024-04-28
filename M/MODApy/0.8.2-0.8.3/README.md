# Comparing `tmp/MODApy-0.8.2.tar.gz` & `tmp/MODApy-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MODApy-0.8.2.tar", last modified: Sat Apr 27 19:19:29 2024, max compression
+gzip compressed data, was "MODApy-0.8.3.tar", last modified: Sun Apr 28 20:14:30 2024, max compression
```

## Comparing `MODApy-0.8.2.tar` & `MODApy-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:19:29.496613 MODApy-0.8.2/
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    35147 2023-03-11 19:24:07.000000 MODApy-0.8.2/LICENSE
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:19:29.489631 MODApy-0.8.2/MODApy/
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)      297 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/__init__.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     6593 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/cfg.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    30623 2024-04-27 19:19:13.000000 MODApy-0.8.2/MODApy/cmd_line.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     3656 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/coverage.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     8208 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/downloader.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     7416 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/modaapi.py
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     6342 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/parquetvardb.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    19642 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/pipeline.py
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     1300 2024-04-03 22:26:23.000000 MODApy-0.8.2/MODApy/utils.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    21570 2024-04-14 11:10:14.000000 MODApy-0.8.2/MODApy/variantsdb.py
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     5418 2024-04-07 18:02:09.000000 MODApy-0.8.2/MODApy/vcfanalysis.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    47643 2024-04-14 11:10:14.000000 MODApy-0.8.2/MODApy/vcfmgr.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)       22 2024-04-27 19:19:13.000000 MODApy-0.8.2/MODApy/version.py
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:19:29.495665 MODApy-0.8.2/MODApy/www/
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52660 2023-03-11 19:24:07.000000 MODApy-0.8.2/MODApy/www/wespipelinebam.png
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)   113893 2023-03-11 19:24:07.000000 MODApy-0.8.2/MODApy/www/wespipelinefull.png
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52084 2023-03-11 19:24:07.000000 MODApy-0.8.2/MODApy/www/wespipelinevcf.png
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:19:29.493613 MODApy-0.8.2/MODApy.egg-info/
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-27 19:19:29.000000 MODApy-0.8.2/MODApy.egg-info/PKG-INFO
--rw-r--r--   0 juan.vazquez   (502) staff       (20)      560 2024-04-27 19:19:29.000000 MODApy-0.8.2/MODApy.egg-info/SOURCES.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)        1 2024-04-27 19:19:29.000000 MODApy-0.8.2/MODApy.egg-info/dependency_links.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)       48 2024-04-27 19:19:29.000000 MODApy-0.8.2/MODApy.egg-info/entry_points.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)      172 2024-04-27 19:19:29.000000 MODApy-0.8.2/MODApy.egg-info/requires.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)        7 2024-04-27 19:19:29.000000 MODApy-0.8.2/MODApy.egg-info/top_level.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-27 19:19:29.496343 MODApy-0.8.2/PKG-INFO
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2640 2023-03-11 19:24:07.000000 MODApy-0.8.2/README.md
--rw-r--r--   0 juan.vazquez   (502) staff       (20)       84 2023-05-21 18:43:17.000000 MODApy-0.8.2/pyproject.toml
--rw-r--r--   0 juan.vazquez   (502) staff       (20)       38 2024-04-27 19:19:29.496696 MODApy-0.8.2/setup.cfg
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2112 2023-05-14 18:54:50.000000 MODApy-0.8.2/setup.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-28 20:14:30.106443 MODApy-0.8.3/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    35147 2023-03-11 19:24:07.000000 MODApy-0.8.3/LICENSE
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-28 20:14:30.100725 MODApy-0.8.3/MODApy/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)      297 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/__init__.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     6593 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/cfg.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    30623 2024-04-27 19:19:13.000000 MODApy-0.8.3/MODApy/cmd_line.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     3656 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/coverage.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     8208 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/downloader.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     7416 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/modaapi.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     6342 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/parquetvardb.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    19642 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/pipeline.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     1300 2024-04-03 22:26:23.000000 MODApy-0.8.3/MODApy/utils.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    21570 2024-04-14 11:10:14.000000 MODApy-0.8.3/MODApy/variantsdb.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     5418 2024-04-07 18:02:09.000000 MODApy-0.8.3/MODApy/vcfanalysis.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    47643 2024-04-14 11:10:14.000000 MODApy-0.8.3/MODApy/vcfmgr.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)       22 2024-04-28 20:14:18.000000 MODApy-0.8.3/MODApy/version.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-28 20:14:30.105504 MODApy-0.8.3/MODApy/www/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52660 2023-03-11 19:24:07.000000 MODApy-0.8.3/MODApy/www/wespipelinebam.png
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)   113893 2023-03-11 19:24:07.000000 MODApy-0.8.3/MODApy/www/wespipelinefull.png
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52084 2023-03-11 19:24:07.000000 MODApy-0.8.3/MODApy/www/wespipelinevcf.png
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-28 20:14:30.103454 MODApy-0.8.3/MODApy.egg-info/
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-28 20:14:30.000000 MODApy-0.8.3/MODApy.egg-info/PKG-INFO
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      560 2024-04-28 20:14:30.000000 MODApy-0.8.3/MODApy.egg-info/SOURCES.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)        1 2024-04-28 20:14:30.000000 MODApy-0.8.3/MODApy.egg-info/dependency_links.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       48 2024-04-28 20:14:30.000000 MODApy-0.8.3/MODApy.egg-info/entry_points.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      172 2024-04-28 20:14:30.000000 MODApy-0.8.3/MODApy.egg-info/requires.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)        7 2024-04-28 20:14:30.000000 MODApy-0.8.3/MODApy.egg-info/top_level.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-28 20:14:30.106182 MODApy-0.8.3/PKG-INFO
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2640 2023-03-11 19:24:07.000000 MODApy-0.8.3/README.md
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       84 2023-05-21 18:43:17.000000 MODApy-0.8.3/pyproject.toml
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       38 2024-04-28 20:14:30.106559 MODApy-0.8.3/setup.cfg
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2112 2023-05-14 18:54:50.000000 MODApy-0.8.3/setup.py
```

### Comparing `MODApy-0.8.2/LICENSE` & `MODApy-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/cfg.py` & `MODApy-0.8.3/MODApy/cfg.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/cmd_line.py` & `MODApy-0.8.3/MODApy/cmd_line.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/coverage.py` & `MODApy-0.8.3/MODApy/coverage.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/downloader.py` & `MODApy-0.8.3/MODApy/downloader.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/modaapi.py` & `MODApy-0.8.3/MODApy/modaapi.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/parquetvardb.py` & `MODApy-0.8.3/MODApy/parquetvardb.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/pipeline.py` & `MODApy-0.8.3/MODApy/pipeline.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/utils.py` & `MODApy-0.8.3/MODApy/utils.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/variantsdb.py` & `MODApy-0.8.3/MODApy/variantsdb.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/vcfanalysis.py` & `MODApy-0.8.3/MODApy/vcfanalysis.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/vcfmgr.py` & `MODApy-0.8.3/MODApy/vcfmgr.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/www/wespipelinebam.png` & `MODApy-0.8.3/MODApy/www/wespipelinebam.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/www/wespipelinefull.png` & `MODApy-0.8.3/MODApy/www/wespipelinefull.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy/www/wespipelinevcf.png` & `MODApy-0.8.3/MODApy/www/wespipelinevcf.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/MODApy.egg-info/PKG-INFO` & `MODApy-0.8.3/MODApy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MODApy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Package to perform several analysis on Multi-Omics Data
 Home-page: https://github.com/juancgvazquez/MODApy
 Author: Juan Carlos Vázquez, Elmer A. Fernández
 Author-email: juancgvazquez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MODApy-0.8.2/MODApy.egg-info/SOURCES.txt` & `MODApy-0.8.3/MODApy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/PKG-INFO` & `MODApy-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MODApy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Package to perform several analysis on Multi-Omics Data
 Home-page: https://github.com/juancgvazquez/MODApy
 Author: Juan Carlos Vázquez, Elmer A. Fernández
 Author-email: juancgvazquez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MODApy-0.8.2/README.md` & `MODApy-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.2/setup.py` & `MODApy-0.8.3/setup.py`

 * *Files identical despite different names*

