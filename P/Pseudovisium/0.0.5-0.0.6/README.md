# Comparing `tmp/Pseudovisium-0.0.5.tar.gz` & `tmp/Pseudovisium-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pseudovisium-0.0.5.tar", last modified: Fri Apr 26 16:37:19 2024, max compression
+gzip compressed data, was "Pseudovisium-0.0.6.tar", last modified: Sun Apr 28 09:37:10 2024, max compression
```

## Comparing `Pseudovisium-0.0.5.tar` & `Pseudovisium-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-26 16:37:19.264283 Pseudovisium-0.0.5/
--rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.5/LICENSE
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-26 16:37:19.264038 Pseudovisium-0.0.5/PKG-INFO
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-26 16:37:19.262221 Pseudovisium-0.0.5/Pseudovisium/
--rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.5/Pseudovisium/__init__.py
--rw-r--r--   0 k23030440   (504) staff       (20)    59076 2024-04-26 16:35:58.000000 Pseudovisium-0.0.5/Pseudovisium/pseudovisium_generate.py
--rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.5/Pseudovisium/pseudovisium_merge.py
--rw-r--r--   0 k23030440   (504) staff       (20)    68606 2024-04-24 16:52:07.000000 Pseudovisium-0.0.5/Pseudovisium/pseudovisium_qc.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-26 16:37:19.263697 Pseudovisium-0.0.5/Pseudovisium.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-26 16:37:19.000000 Pseudovisium-0.0.5/Pseudovisium.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-26 16:37:19.000000 Pseudovisium-0.0.5/Pseudovisium.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-26 16:37:19.000000 Pseudovisium-0.0.5/Pseudovisium.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-26 16:37:19.000000 Pseudovisium-0.0.5/Pseudovisium.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-26 16:37:19.000000 Pseudovisium-0.0.5/Pseudovisium.egg-info/top_level.txt
--rw-r--r--   0 k23030440   (504) staff       (20)     3637 2024-04-26 08:21:23.000000 Pseudovisium-0.0.5/README.md
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-26 16:37:19.264337 Pseudovisium-0.0.5/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-26 16:36:57.000000 Pseudovisium-0.0.5/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-28 09:37:10.208483 Pseudovisium-0.0.6/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.6/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-28 09:37:10.208262 Pseudovisium-0.0.6/PKG-INFO
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-28 09:37:10.206135 Pseudovisium-0.0.6/Pseudovisium/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.6/Pseudovisium/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    58610 2024-04-28 08:09:58.000000 Pseudovisium-0.0.6/Pseudovisium/pseudovisium_generate.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.6/Pseudovisium/pseudovisium_merge.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    68606 2024-04-24 16:52:07.000000 Pseudovisium-0.0.6/Pseudovisium/pseudovisium_qc.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-28 09:37:10.207891 Pseudovisium-0.0.6/Pseudovisium.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/top_level.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)     3637 2024-04-26 08:21:23.000000 Pseudovisium-0.0.6/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-28 09:37:10.208534 Pseudovisium-0.0.6/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-28 09:36:31.000000 Pseudovisium-0.0.6/setup.py
```

### Comparing `Pseudovisium-0.0.5/LICENSE` & `Pseudovisium-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.5/PKG-INFO` & `Pseudovisium-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.5/Pseudovisium/pseudovisium_generate.py` & `Pseudovisium-0.0.6/Pseudovisium/pseudovisium_generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -540,15 +540,15 @@
 
 def process_hexagon(hexagon, hexagon_index, features, hexagon_counts):
         return [[features.index(feature) + 1, hexagon_index + 1, count]
                 for feature, count in hexagon_counts[hexagon].items()]
 
 def hex_to_rows(hexagon_batch, start_index, features, hexagon_counts):
     matrix_data = []
-    for hexagon_index, hexagon in enumerate(hexagon_batch, start=start_index):
+    for hexagon_index, hexagon in enumerate(hexagon_batch, start=start_index): ###Here is the error!!! HExagon indices are scrambled!!!!!
         count_dict = hexagon_counts.get(hexagon, {})
         for feature, count in count_dict.items():
             feature_index = features.index(feature)
             matrix_data.append([feature_index + 1, hexagon_index + 1, count])
     print(f"Batch total count: {sum(row[2] for row in matrix_data)}")
     return matrix_data
 
@@ -695,33 +695,28 @@
 
     print("Putting together the matrix.mtx file")
     matrix_data = []
 
     n_total_hexagons = len(ordered_hexagon_counts)
 
     total_count = 0
-    n_processes = min(max_workers, multiprocessing.cpu_count())
-    batch_size_n_hexagons = n_total_hexagons // (n_processes * 4)
-    print(f"Using {n_processes} processes")
-    print(f"Processing {n_total_hexagons} hexagons in batches of {batch_size_n_hexagons} hexagons")
-    with concurrent.futures.ProcessPoolExecutor(max_workers=n_processes) as executor:
-        futures = []
-        hexagon_names = list(ordered_hexagon_counts.keys())
-        for i in range(0, n_total_hexagons, batch_size_n_hexagons):
-            hexagon_batch = hexagon_names[i:i + batch_size_n_hexagons]
-            future = executor.submit(hex_to_rows, hexagon_batch, i, features, ordered_hexagon_counts)
-            futures.append(future)
-
-        with tqdm(total=len(futures), desc="Processing batches") as pbar:
-            for future in concurrent.futures.as_completed(futures):
-                batch_matrix_data = future.result()
-                matrix_data.extend(batch_matrix_data)
-                total_count += sum(row[2] for row in batch_matrix_data)
-                pbar.update(1)
+    matrix_data = []
+
+    for hexagon, count_dict in hexagon_counts.items():
+        if sum(count_dict.values()) > 0:
+            hexagon_index = hexagon_names.index(hexagon)
+            for feature, count in count_dict.items():
+                feature_index = features.index(feature)
+                matrix_data.append([feature_index+1, hexagon_index+1, count])
+                total_count += count
+    
 
+    data = np.array(matrix_data)[:, 2]
+    row_indices = np.array(matrix_data)[:, 0] - 1
+    col_indices = np.array(matrix_data)[:, 1] - 1
     print(f"Total matrix count: {total_count}")
     unique_hexagons = len(set(hexagon_names))
     print(f"Number of unique hexagons: {unique_hexagons}")
     print(f"Number of hexagons in ordered_hexagon_counts: {len(ordered_hexagon_counts)}")
```

### Comparing `Pseudovisium-0.0.5/Pseudovisium/pseudovisium_merge.py` & `Pseudovisium-0.0.6/Pseudovisium/pseudovisium_merge.py`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.5/Pseudovisium/pseudovisium_qc.py` & `Pseudovisium-0.0.6/Pseudovisium/pseudovisium_qc.py`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.5/Pseudovisium.egg-info/PKG-INFO` & `Pseudovisium-0.0.6/Pseudovisium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.5/README.md` & `Pseudovisium-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.5/setup.py` & `Pseudovisium-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data'
 LONG_DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data, for more information see https://github.com/BKover99/pseudovisium'
 
 
 setup(
     name="Pseudovisium",
     version=VERSION,
```

