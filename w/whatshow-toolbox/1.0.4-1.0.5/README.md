# Comparing `tmp/whatshow_toolbox-1.0.4.tar.gz` & `tmp/whatshow_toolbox-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_toolbox-1.0.4.tar", last modified: Sat Apr 27 05:22:00 2024, max compression
+gzip compressed data, was "whatshow_toolbox-1.0.5.tar", last modified: Sat Apr 27 11:19:41 2024, max compression
```

## Comparing `whatshow_toolbox-1.0.4.tar` & `whatshow_toolbox-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 05:22:00.073376 whatshow_toolbox-1.0.4/
--rw-rw-rw-   0        0        0     2112 2024-04-27 05:22:00.070325 whatshow_toolbox-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2004 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 05:22:00.073376 whatshow_toolbox-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 05:22:00.057347 whatshow_toolbox-1.0.4/whatshow_toolbox/
--rw-rw-rw-   0        0        0    13043 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/whatshow_toolbox/MatlabFuncHelper.py
--rw-rw-rw-   0        0        0       46 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/whatshow_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 05:22:00.070325 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 11:19:41.892883 whatshow_toolbox-1.0.5/
+-rw-rw-rw-   0        0        0     2112 2024-04-27 11:19:41.889884 whatshow_toolbox-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2004 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:19:41.892883 whatshow_toolbox-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:19:41.878411 whatshow_toolbox-1.0.5/whatshow_toolbox/
+-rw-rw-rw-   0        0        0    13005 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/whatshow_toolbox/MatlabFuncHelper.py
+-rw-rw-rw-   0        0        0       46 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/whatshow_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:19:41.889884 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/top_level.txt
```

### Comparing `whatshow_toolbox-1.0.4/PKG-INFO` & `whatshow_toolbox-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_toolbox
-Version: 1.0.4
+Version: 1.0.5
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.4-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.5-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.4/README.md` & `whatshow_toolbox-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.4-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.5-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.4/whatshow_toolbox/MatlabFuncHelper.py` & `whatshow_toolbox-1.0.5/whatshow_toolbox/MatlabFuncHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         mat = np.asarray(mat);
         step = np.asarray(step);
         if self.batch_size == self.BATCH_SIZE_NO:
             out = np.roll(mat, step, axis=0);
         else:
             mat_shape = list(mat.shape);
             mat_shape.insert(0, self.batch_size);
-            out = np.zeros((self.batch_size, mat.shape[-2], mat.shape[-1]), dtype=mat.dtype);
+            out = np.zeros(mat.shape, dtype=mat.dtype);
             for batch_id in range(self.batch_size):
                 if step.ndim == 0:
                     out[batch_id, ...] = np.roll(mat[batch_id, ...], step, axis=0);
                 else:
                     out[batch_id, ...] = np.roll(mat[batch_id, ...], step[batch_id], axis=0);
         return out;
```

### Comparing `whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/PKG-INFO` & `whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-toolbox
-Version: 1.0.4
+Version: 1.0.5
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.4-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.5-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

