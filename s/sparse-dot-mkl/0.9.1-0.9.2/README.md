# Comparing `tmp/sparse_dot_mkl-0.9.1.tar.gz` & `tmp/sparse_dot_mkl-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse_dot_mkl-0.9.1.tar", last modified: Wed Feb 28 20:29:29 2024, max compression
+gzip compressed data, was "sparse_dot_mkl-0.9.2.tar", last modified: Sun Apr 28 15:42:21 2024, max compression
```

## Comparing `sparse_dot_mkl-0.9.1.tar` & `sparse_dot_mkl-0.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-02-28 20:29:29.522617 sparse_dot_mkl-0.9.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)       26 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.1/.codecov.yml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1823 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.1/.gitignore
--rw-rw-r--   0 chris     (1000) chris     (1000)     3223 2024-02-28 20:26:03.000000 sparse_dot_mkl-0.9.1/CHANGELOG.md
--rw-rw-r--   0 chris     (1000) chris     (1000)     1065 2019-12-08 21:27:09.000000 sparse_dot_mkl-0.9.1/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-02-28 20:29:29.522617 sparse_dot_mkl-0.9.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     5568 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)     3855 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.1/demo.ipynb
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-02-28 20:29:29.522617 sparse_dot_mkl-0.9.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1174 2024-02-28 20:26:09.000000 sparse_dot_mkl-0.9.1/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-02-28 20:29:29.518617 sparse_dot_mkl-0.9.1/sparse_dot_mkl/
--rw-rw-r--   0 chris     (1000) chris     (1000)      183 2023-10-12 21:10:29.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3582 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_dense_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9398 2023-10-11 19:33:52.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_gram_matrix.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-02-28 20:29:29.522617 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2506 2023-10-11 18:29:04.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    20577 2023-10-11 20:32:42.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_cfunctions.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    30604 2023-10-11 18:36:54.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_common.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2093 2023-10-11 19:27:04.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_constants.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2825 2023-12-15 18:05:52.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_load_library.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1379 2023-10-11 17:19:36.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_structs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6377 2023-10-11 20:03:18.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4120 2022-10-23 14:59:00.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_qr_solver.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6937 2024-02-28 20:24:05.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_sparse.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4454 2023-10-12 21:10:13.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_sypr.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4889 2023-10-12 20:56:33.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_vector.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7658 2024-02-28 20:16:02.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/sparse_dot.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-02-28 20:29:29.522617 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-02-01 23:31:58.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4774 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_dense_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7149 2023-10-11 20:23:52.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_gram_matrix.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11819 2023-10-11 19:56:07.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_mkl.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2744 2022-10-23 14:57:09.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_qr_solver.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13253 2023-10-11 20:19:32.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_sparse_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14859 2024-02-28 20:25:09.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_sparse_sparse.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12099 2023-10-11 20:09:30.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_sparse_vector.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-02-28 20:29:29.522617 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-02-28 20:29:29.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     1155 2024-02-28 20:29:29.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-02-28 20:29:29.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       12 2024-02-28 20:29:29.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       15 2024-02-28 20:29:29.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2020-01-15 17:20:36.000000 sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.612030 sparse_dot_mkl-0.9.2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       26 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/.codecov.yml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1823 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/.gitignore
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3517 2024-04-28 15:35:27.000000 sparse_dot_mkl-0.9.2/CHANGELOG.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1065 2019-12-08 21:27:09.000000 sparse_dot_mkl-0.9.2/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-04-28 15:42:21.612030 sparse_dot_mkl-0.9.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5568 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3855 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/demo.ipynb
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-28 15:42:21.612030 sparse_dot_mkl-0.9.2/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1174 2024-04-28 15:13:54.000000 sparse_dot_mkl-0.9.2/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      207 2024-04-28 15:14:12.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3582 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_dense_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9398 2023-10-11 19:33:52.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_gram_matrix.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3537 2024-04-28 15:32:58.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    21368 2024-04-28 15:05:24.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_cfunctions.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    30604 2023-10-11 18:36:54.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2198 2024-04-28 14:01:56.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_constants.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2824 2024-04-28 13:39:36.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_load_library.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1379 2023-10-11 17:19:36.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_structs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6377 2023-10-11 20:03:18.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4120 2022-10-23 14:59:00.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_qr_solver.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6937 2024-02-28 20:24:05.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sparse.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4454 2023-10-12 21:10:13.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sypr.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4889 2023-10-12 20:56:33.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_vector.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7658 2024-02-28 20:16:02.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/sparse_dot.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-02-01 23:31:58.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4774 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_dense_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7149 2023-10-11 20:23:52.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_gram_matrix.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11819 2023-10-11 19:56:07.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_mkl.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2744 2022-10-23 14:57:09.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_qr_solver.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13253 2023-10-11 20:19:32.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14859 2024-02-28 20:25:09.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_sparse.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12099 2023-10-11 20:09:30.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_vector.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1155 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       12 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       15 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2020-01-15 17:20:36.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/zip-safe
```

### Comparing `sparse_dot_mkl-0.9.1/.gitignore` & `sparse_dot_mkl-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/CHANGELOG.md` & `sparse_dot_mkl-0.9.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+### Version 0.9.2
+
+* Explicit check for interface env MKL_INTERFACE_LAYER and interface selection in python.
+  Will raise a RuntimeWarning if ILP64 is requested but the 64-bit interface layer is unavailable.
+  Note that the MKL_INTERFACE_LAYER env must be set before this package is imported.
+
 ### Version 0.9.1
 
 * Support for `out` parameter with sparse-sparse multiplication when `dense=True`
 
 ### Version 0.9.0
 
 * Support for scipy sparse arrays (introduced in scipy 1.11)
```

### Comparing `sparse_dot_mkl-0.9.1/LICENSE` & `sparse_dot_mkl-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/PKG-INFO` & `sparse_dot_mkl-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse_dot_mkl
-Version: 0.9.1
+Version: 0.9.2
 Summary: Intel MKL wrapper for sparse matrix multiplication
 Home-page: https://github.com/flatironinstitute/sparse_dot
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparse_dot_mkl-0.9.1/README.md` & `sparse_dot_mkl-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/demo.ipynb` & `sparse_dot_mkl-0.9.2/demo.ipynb`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/setup.py` & `sparse_dot_mkl-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
 DISTNAME = 'sparse_dot_mkl'
-VERSION = '0.9.1'
+VERSION = '0.9.2'
 DESCRIPTION = "Intel MKL wrapper for sparse matrix multiplication"
 MAINTAINER = 'Chris Jackson'
 MAINTAINER_EMAIL = 'cj59@nyu.edu'
 URL = 'https://github.com/flatironinstitute/sparse_dot'
 LICENSE = 'MIT'
 
 # Description from README.md
```

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_dense_dense.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_dense_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_gram_matrix.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_gram_matrix.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/__init__.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,26 @@
     del os.environ["KMP_INIT_AT_FORK"]
 else:
     _sklearn_env = None
 
 from scipy import sparse as _spsparse
 import numpy as _np
 import ctypes as _ctypes
+import warnings as _warnings
 from ._constants import *
 from ._structs import (
     MKL_Complex8,
     MKL_Complex16,
     matrix_descr,
     sparse_matrix_t
 )
-from ._cfunctions import MKL
+from ._cfunctions import (
+    MKL,
+    mkl_set_interface_layer
+)
 from ._common import (
     _create_mkl_sparse,
     _export_mkl,
     _check_return_value,
     _convert_to_csr,
     _is_allowed_sparse_format,
     _is_double,
@@ -59,19 +63,23 @@
     )
     test_comparison = test_array.A
 
     csc_ref, precision_flag, _ = _create_mkl_sparse(test_array)
 
     try:
         csr_ref = _convert_to_csr(csc_ref)
-        final_array = _export_mkl(
-            csr_ref,
-            precision_flag,
-            output_type='csr_matrix'
-        )
+
+        with _warnings.catch_warnings():
+            _warnings.filterwarnings("ignore", category=RuntimeWarning)
+            final_array = _export_mkl(
+                csr_ref,
+                precision_flag,
+                output_type='csr_matrix'
+            )
+
         if not _np.allclose(test_comparison, final_array.A):
             raise ValueError("Match failed after matrix conversion")
         _destroy_mkl_handle(csr_ref)
     finally:
         _destroy_mkl_handle(csc_ref)
 
 
@@ -91,12 +99,38 @@
 
         try:
             _validate_dtype()
         except ValueError:
             raise ImportError("Unable to set MKL numeric type")
 
 
-if MKL.MKL_INT is None:
+_mkl_interface_env = os.getenv('MKL_INTERFACE_LAYER')
+
+
+# Check to make sure that the MKL_Set_Interface_Layer call was correct
+# And fail back to 32bit if it wasn't
+if _mkl_interface_env == 'ILP64':
+    try:
+        _validate_dtype()
+    except (ValueError, RuntimeError):
+        _warnings.warn(
+            "MKL_INTERFACE_LAYER=ILP64 failed to set MKL interface; "
+            "64-bit integer support unavailable",
+            RuntimeWarning
+        )
+        MKL._set_int_type(_ctypes.c_int, _np.int32)
+        _validate_dtype()
+elif _mkl_interface_env == 'LP64':
+    _validate_dtype()
+elif MKL.MKL_INT is None and _mkl_interface_env is not None:
+    _warnings.warn(
+        f"MKL_INTERFACE_LAYER value {_mkl_interface_env} invalid; "
+        "set 'ILP64' or 'LP64'",
+        RuntimeWarning
+    )
+    _empirical_set_dtype()
+elif MKL.MKL_INT is None:
     _empirical_set_dtype()
 
+
 if _sklearn_env is not None:
     os.environ["KMP_INIT_AT_FORK"] = _sklearn_env
```

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_cfunctions.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_cfunctions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import ctypes as _ctypes
 
 from sparse_dot_mkl._mkl_interface._structs import (
     sparse_matrix_t,
     matrix_descr,
     MKL_Complex8,
     MKL_Complex16,
@@ -10,14 +11,20 @@
 from sparse_dot_mkl._mkl_interface._load_library import (
     mkl_library
 )
 
 import numpy as _np
 from numpy.ctypeslib import ndpointer
 
+# MKL_SET_INTERFACE_LAYER flags
+MKL_INTERFACE_LP64  = 0
+MKL_INTERFACE_ILP64 = 1
+MKL_INTERFACE_GNU   = 2
+
+
 _libmkl = mkl_library()
 
 
 def mkl_library_name():
     return _libmkl._name
 
 
@@ -125,14 +132,17 @@
     _mkl_sparse_d_qr_factorize = _libmkl.mkl_sparse_d_qr_factorize
     _mkl_sparse_s_qr_factorize = _libmkl.mkl_sparse_s_qr_factorize
 
     # Import function for QR solver - solve
     _mkl_sparse_d_qr_solve = _libmkl.mkl_sparse_d_qr_solve
     _mkl_sparse_s_qr_solve = _libmkl.mkl_sparse_s_qr_solve
 
+    # Set interface function
+    _mkl_set_interface_layer = _libmkl.MKL_Set_Interface_Layer
+
     @classmethod
     def _set_int_type(cls, c_type, _np_type):
         cls.MKL_INT = c_type
         cls.MKL_INT_NUMPY = _np_type
 
         cls._set_int_type_create()
         cls._set_int_type_export()
@@ -557,7 +567,26 @@
             _ctypes.c_int,
             MKL.MKL_INT,
             _ctypes.POINTER(prec_type),
             MKL.MKL_INT,
             ndpointer(dtype=prec_type, ndim=2),
             MKL.MKL_INT,
         ]
+
+
+MKL._mkl_set_interface_layer.argtypes = [_ctypes.c_int]
+MKL._mkl_set_interface_layer.restypes = [_ctypes.c_int]
+
+
+def mkl_set_interface_layer(layer_code):
+    return MKL._mkl_set_interface_layer(layer_code)
+
+
+_mkl_interface_env = os.getenv('MKL_INTERFACE_LAYER')
+
+
+if MKL.MKL_INT is None and _mkl_interface_env == 'ILP64':
+    mkl_set_interface_layer(MKL_INTERFACE_ILP64)
+    MKL._set_int_type(_ctypes.c_longlong, _np.int64)
+elif MKL.MKL_INT is None and _mkl_interface_env == 'LP64':
+    mkl_set_interface_layer(MKL_INTERFACE_LP64)
+    MKL._set_int_type(_ctypes.c_int, _np.int32)
```

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_common.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_common.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_constants.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,7 +54,12 @@
 
 # Define sparse & cblas upper or lower triangle code
 MKL_UPPER = 121
 MKL_LOWER = 122
 
 # ILP64 message
 ILP64_MSG = " Try changing MKL to int64 with the environment variable MKL_INTERFACE_LAYER=ILP64"
+
+# MKL_SET_INTERFACE_LAYER flags
+MKL_INTERFACE_LP64  = 0
+MKL_INTERFACE_ILP64 = 1
+MKL_INTERFACE_GNU   = 2
```

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_load_library.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_load_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,11 +86,11 @@
     # Couldn't find anything to import
     # Raise the ImportError
     except IMPORT_ERRORS as err:
         raise ImportError(
             "Unable to load the MKL libraries through "
             "libmkl_rt. Try setting $LD_LIBRARY_PATH to the "
             "LD library path or $MKL_RT to the libmkl_rt.so library "
-            " file directly. " + str(err)
+            "file directly. " + str(err)
         )
 
     return _libmkl
```

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_mkl_interface/_structs.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_structs.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_dense.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_qr_solver.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_qr_solver.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_sparse.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sparse.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_sypr.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sypr.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/_sparse_vector.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_vector.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/sparse_dot.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/sparse_dot.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_dense_dense.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_dense_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_gram_matrix.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_gram_matrix.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_mkl.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_mkl.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_qr_solver.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_qr_solver.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_sparse_dense.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_sparse_sparse.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_sparse.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl/tests/test_sparse_vector.py` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_vector.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/PKG-INFO` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse_dot_mkl
-Version: 0.9.1
+Version: 0.9.2
 Summary: Intel MKL wrapper for sparse matrix multiplication
 Home-page: https://github.com/flatironinstitute/sparse_dot
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparse_dot_mkl-0.9.1/sparse_dot_mkl.egg-info/SOURCES.txt` & `sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

