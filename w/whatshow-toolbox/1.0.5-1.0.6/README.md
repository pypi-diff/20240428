# Comparing `tmp/whatshow_toolbox-1.0.5.tar.gz` & `tmp/whatshow_toolbox-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_toolbox-1.0.5.tar", last modified: Sat Apr 27 11:19:41 2024, max compression
+gzip compressed data, was "whatshow_toolbox-1.0.6.tar", last modified: Sun Apr 28 05:44:16 2024, max compression
```

## Comparing `whatshow_toolbox-1.0.5.tar` & `whatshow_toolbox-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:19:41.892883 whatshow_toolbox-1.0.5/
--rw-rw-rw-   0        0        0     2112 2024-04-27 11:19:41.889884 whatshow_toolbox-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2004 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 11:19:41.892883 whatshow_toolbox-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:19:41.878411 whatshow_toolbox-1.0.5/whatshow_toolbox/
--rw-rw-rw-   0        0        0    13005 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/whatshow_toolbox/MatlabFuncHelper.py
--rw-rw-rw-   0        0        0       46 2024-04-27 11:19:37.000000 whatshow_toolbox-1.0.5/whatshow_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:19:41.889884 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 11:19:41.000000 whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 05:44:16.876809 whatshow_toolbox-1.0.6/
+-rw-rw-rw-   0        0        0     2154 2024-04-28 05:44:16.874743 whatshow_toolbox-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-04-28 05:44:15.000000 whatshow_toolbox-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 05:44:16.876809 whatshow_toolbox-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-04-28 05:44:15.000000 whatshow_toolbox-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:44:16.842880 whatshow_toolbox-1.0.6/whatshow_toolbox/
+-rw-rw-rw-   0        0        0    13113 2024-04-28 05:44:15.000000 whatshow_toolbox-1.0.6/whatshow_toolbox/MatlabFuncHelper.py
+-rw-rw-rw-   0        0        0       46 2024-04-28 05:44:15.000000 whatshow_toolbox-1.0.6/whatshow_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:44:16.874743 whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     2154 2024-04-28 05:44:16.000000 whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-28 05:44:16.000000 whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 05:44:16.000000 whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-28 05:44:16.000000 whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 05:44:16.000000 whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/top_level.txt
```

### Comparing `whatshow_toolbox-1.0.5/PKG-INFO` & `whatshow_toolbox-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_toolbox
-Version: 1.0.5
+Version: 1.0.6
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.5-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.6-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
@@ -29,14 +29,15 @@
         * reshape(mat, d1, d2, ...):
         * repmat1(mat, d1, d2, ...): repeat the matrix in the given dimension (the batch dim is repeated as 1)
         * repmatN(mat, d1, d2, ...): repeat the matrix in the given dimension (the batch dim is repeated as batch_size)
         * diag(mat): generate a matrix based on its diag or get a diagonal matrix from its vector<br>
             `@mat`: a vector as [(batch_size), n, 1] or [(batch_size), 1, n]; if n == 1, it will be taken as [(batch_size), n, 1]. Or a square matrix [(batch_size), n, n]
         * circshift(mat, step): circular shift (1st index except for the batch size)
     * Maths
+        * sum(): sum along the last axis
         * max(): return the maximum of a matrix or the maximum of two matrices (for complex value, we compare the magnitude)
             ```c, matlab, python
             self.max(mat1, axis=-1);    // return the maximum of a matrix, axis tells which axis to look at
             self.max(mat1, 4);          // return the maximum of a matrix and the given value
             self.max(mat1, mat2);       // return the maximum of two matrices
             ```
         * kron(a, b): Kronecker produc
```

### Comparing `whatshow_toolbox-1.0.5/README.md` & `whatshow_toolbox-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.5-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.6-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
@@ -24,14 +24,15 @@
         * reshape(mat, d1, d2, ...):
         * repmat1(mat, d1, d2, ...): repeat the matrix in the given dimension (the batch dim is repeated as 1)
         * repmatN(mat, d1, d2, ...): repeat the matrix in the given dimension (the batch dim is repeated as batch_size)
         * diag(mat): generate a matrix based on its diag or get a diagonal matrix from its vector<br>
             `@mat`: a vector as [(batch_size), n, 1] or [(batch_size), 1, n]; if n == 1, it will be taken as [(batch_size), n, 1]. Or a square matrix [(batch_size), n, n]
         * circshift(mat, step): circular shift (1st index except for the batch size)
     * Maths
+        * sum(): sum along the last axis
         * max(): return the maximum of a matrix or the maximum of two matrices (for complex value, we compare the magnitude)
             ```c, matlab, python
             self.max(mat1, axis=-1);    // return the maximum of a matrix, axis tells which axis to look at
             self.max(mat1, 4);          // return the maximum of a matrix and the given value
             self.max(mat1, mat2);       // return the maximum of two matrices
             ```
         * kron(a, b): Kronecker produc
```

### Comparing `whatshow_toolbox-1.0.5/whatshow_toolbox/MatlabFuncHelper.py` & `whatshow_toolbox-1.0.6/whatshow_toolbox/MatlabFuncHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,20 @@
                 else:
                     out[batch_id, ...] = np.roll(mat[batch_id, ...], step[batch_id], axis=0);
         return out;
 
     ###########################################################################
     # Maths
     '''
+    sum
+    '''
+    def sum(self, mat, *, axis=-1):
+        return np.sum(mat, axis=-1);
+    
+    '''
     return the maximum of a matrix or the maximum of two matrices (for complex value, we compare the magnitude)
     @in1:   the matrix to find the maximal value
     @in2:   a scalar or a matrix to be compared with in1. If not given, it means return the maximal value of in1
     @axis:  the axis to compare or find the maximal value
     '''
     def max(self, in1, *args, axis=-1):
         out = None;
```

### Comparing `whatshow_toolbox-1.0.5/whatshow_toolbox.egg-info/PKG-INFO` & `whatshow_toolbox-1.0.6/whatshow_toolbox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-toolbox
-Version: 1.0.5
+Version: 1.0.6
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.5-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.6-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
@@ -29,14 +29,15 @@
         * reshape(mat, d1, d2, ...):
         * repmat1(mat, d1, d2, ...): repeat the matrix in the given dimension (the batch dim is repeated as 1)
         * repmatN(mat, d1, d2, ...): repeat the matrix in the given dimension (the batch dim is repeated as batch_size)
         * diag(mat): generate a matrix based on its diag or get a diagonal matrix from its vector<br>
             `@mat`: a vector as [(batch_size), n, 1] or [(batch_size), 1, n]; if n == 1, it will be taken as [(batch_size), n, 1]. Or a square matrix [(batch_size), n, n]
         * circshift(mat, step): circular shift (1st index except for the batch size)
     * Maths
+        * sum(): sum along the last axis
         * max(): return the maximum of a matrix or the maximum of two matrices (for complex value, we compare the magnitude)
             ```c, matlab, python
             self.max(mat1, axis=-1);    // return the maximum of a matrix, axis tells which axis to look at
             self.max(mat1, 4);          // return the maximum of a matrix and the given value
             self.max(mat1, mat2);       // return the maximum of two matrices
             ```
         * kron(a, b): Kronecker produc
```

