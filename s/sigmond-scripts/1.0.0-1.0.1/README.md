# Comparing `tmp/sigmond_scripts-1.0.0.tar.gz` & `tmp/sigmond_scripts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmond_scripts-1.0.0.tar", last modified: Thu Apr 25 04:22:55 2024, max compression
+gzip compressed data, was "sigmond_scripts-1.0.1.tar", last modified: Sun Apr 28 00:42:12 2024, max compression
```

## Comparing `sigmond_scripts-1.0.0.tar` & `sigmond_scripts-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 04:22:55.940150 sigmond_scripts-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    35141 2024-04-24 16:22:10.000000 sigmond_scripts-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-25 04:22:55.940150 sigmond_scripts-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1307 2024-04-25 03:29:22.000000 sigmond_scripts-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-24 16:34:39.000000 sigmond_scripts-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      628 2024-04-25 04:22:55.940150 sigmond_scripts-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 04:22:55.940150 sigmond_scripts-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 04:22:55.940150 sigmond_scripts-1.0.0/src/sigmond_scripts/
--rw-r--r--   0 root         (0) root         (0)        2 2024-04-25 03:37:53.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8422 2024-04-25 04:07:58.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/channel.py
--rw-r--r--   0 root         (0) root         (0)     5860 2024-04-25 03:53:23.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/correlator_data.py
--rw-r--r--   0 root         (0) root         (0)     5572 2024-04-25 03:54:45.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/data_files.py
--rw-r--r--   0 root         (0) root         (0)    18308 2024-04-24 18:40:10.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/data_handler.py
--rw-r--r--   0 root         (0) root         (0)    22391 2024-04-25 04:11:05.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/fit_info.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-24 16:34:39.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/isospin.py
--rw-r--r--   0 root         (0) root         (0)    13785 2024-04-25 04:08:30.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/operator.py
--rw-r--r--   0 root         (0) root         (0)     9681 2024-04-25 04:09:04.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/operator_set.py
--rw-r--r--   0 root         (0) root         (0)     9948 2024-04-25 04:10:28.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/sigmond_info.py
--rw-r--r--   0 root         (0) root         (0)    70514 2024-04-25 04:10:11.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/sigmond_input.py
--rw-r--r--   0 root         (0) root         (0)    38915 2024-04-25 03:55:44.000000 sigmond_scripts-1.0.0/src/sigmond_scripts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 04:22:55.940150 sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-25 04:22:55.000000 sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      660 2024-04-25 04:22:55.000000 sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 04:22:55.000000 sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-25 04:22:55.000000 sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-25 04:22:55.000000 sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)    35141 2024-04-24 16:22:10.000000 sigmond_scripts-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1307 2024-04-25 03:29:22.000000 sigmond_scripts-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-24 16:34:39.000000 sigmond_scripts-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      628 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.453420 sigmond_scripts-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/src/sigmond_scripts/
+-rw-r--r--   0 root         (0) root         (0)        2 2024-04-25 03:37:53.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8422 2024-04-25 04:07:58.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/channel.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2024-04-25 03:53:23.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/correlator_data.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2024-04-25 03:54:45.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/data_files.py
+-rw-r--r--   0 root         (0) root         (0)    18225 2024-04-26 15:02:28.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/data_handler.py
+-rw-r--r--   0 root         (0) root         (0)    22391 2024-04-25 04:11:05.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/fit_info.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-24 16:34:39.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/isospin.py
+-rw-r--r--   0 root         (0) root         (0)    13785 2024-04-25 04:08:30.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/operator.py
+-rw-r--r--   0 root         (0) root         (0)     9681 2024-04-25 04:09:04.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/operator_set.py
+-rw-r--r--   0 root         (0) root         (0)     9948 2024-04-25 04:10:28.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_info.py
+-rw-r--r--   0 root         (0) root         (0)    70514 2024-04-25 04:10:11.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_input.py
+-rw-r--r--   0 root         (0) root         (0)    38929 2024-04-27 18:43:48.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      660 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/top_level.txt
```

### Comparing `sigmond_scripts-1.0.0/LICENSE` & `sigmond_scripts-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/PKG-INFO` & `sigmond_scripts-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmond_scripts
-Version: 1.0.0
+Version: 1.0.1
 Summary: Supporting functions for handling the c++ library sigmond
 Author: Drew Hanlon
 Author-email: ahanlon@bnl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `sigmond_scripts-1.0.0/README.md` & `sigmond_scripts-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/setup.cfg` & `sigmond_scripts-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sigmond_scripts
-version = 1.0.0
+version = 1.0.1
 author = Drew Hanlon
 author_email = ahanlon@bnl.gov
 description = Supporting functions for handling the c++ library sigmond
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/channel.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/channel.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/correlator_data.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/correlator_data.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/data_files.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/data_files.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/data_handler.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import h5py
 
 from typing import NamedTuple
 import logging
 from sortedcontainers import SortedSet
 import tqdm
 
-import sigmond_scripts.analysis.utils.util as util
-from sigmond_scripts.analysis.data_handling.data_files import DataFiles, FileInfo
-from sigmond_scripts.analysis.data_handling.correlator_data import CorrelatorData
-from sigmond_scripts.analysis.operator_info.operator import Operator
+import sigmond_scripts.util as util
+from sigmond_scripts.data_files import DataFiles, FileInfo
+from sigmond_scripts.correlator_data import CorrelatorData
+from sigmond_scripts.operator import Operator
 
 import sigmond
 
 class DataHandler(metaclass=util.Singleton):
   """ The all important Data Handler!  """
 
   def __init__(self, project_info, shared_node = True, nodes=os.cpu_count()):
@@ -529,8 +529,8 @@
         if bin_file in corr_data._data_files[channel1]._bin_files and channel1!=channel:
             delete_bin_file = False
             break
     if delete_bin_file:
         bin_files_to_remove.add(bin_file)
 
   current_df._bin_files -= bin_files_to_remove
-  corr_data._data_files.pop(channel)
+  corr_data._data_files.pop(channel)
```

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/fit_info.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/fit_info.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/operator.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/operator.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/operator_set.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/operator_set.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/sigmond_info.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_info.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/sigmond_input.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_input.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts/util.py` & `sigmond_scripts-1.0.1/src/sigmond_scripts/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
   return result_obs
 
 #########################################################################################
 # PDF documents
 def create_doc(title, with_tikz=False):
   logging.info("Creating PDF...")
-  doc = pylatex.Document(geometry_options={'margin': '1.5cm'})
+  doc = pylatex.Document(geometry_options={'margin': '1.5cm'},imputenc=None)
   doc.packages.append(pylatex.Package('hyperref'))
   doc.packages.append(pylatex.Package('amssymb'))
   doc.packages.append(pylatex.Package('amsmath'))
   doc.packages.append(pylatex.Package('float'))
   doc.packages.append(pylatex.Package('xcolor'))
   doc.packages.append(pylatex.Package('caption', {'labelformat': 'empty', 'justification': 'centering'}))
 #   doc.packages.append(pylatex.Package('todonotes'))
```

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/PKG-INFO` & `sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmond_scripts
-Version: 1.0.0
+Version: 1.0.1
 Summary: Supporting functions for handling the c++ library sigmond
 Author: Drew Hanlon
 Author-email: ahanlon@bnl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `sigmond_scripts-1.0.0/src/sigmond_scripts.egg-info/SOURCES.txt` & `sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

