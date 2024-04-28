# Comparing `tmp/DMDO-2401-py3-none-any.whl.zip` & `tmp/DMDO-2404-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 44607 bytes, number of entries: 17
+Zip file size: 44602 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat     5313 b- defN 24-Apr-23 10:43 DMDO/DA.py
 -rw-rw-rw-  2.0 fat     7067 b- defN 24-Apr-23 10:43 DMDO/DMDO.py
 -rw-rw-rw-  2.0 fat     3101 b- defN 24-Apr-23 10:43 DMDO/MDA.py
 -rw-rw-rw-  2.0 fat    16803 b- defN 24-Apr-23 10:43 DMDO/MDO.py
 -rw-rw-rw-  2.0 fat    30685 b- defN 24-Apr-23 10:43 DMDO/SP.py
 -rw-rw-rw-  2.0 fat     2471 b- defN 24-Apr-23 10:43 DMDO/__init__.py
 -rw-rw-rw-  2.0 fat     4603 b- defN 24-Apr-23 10:43 DMDO/_common.py
 -rw-rw-rw-  2.0 fat     3829 b- defN 24-Apr-23 10:43 DMDO/_globals.py
 -rw-rw-rw-  2.0 fat     2807 b- defN 24-Apr-23 10:43 DMDO/_protocols.py
--rw-rw-rw-  2.0 fat    26667 b- defN 24-Apr-23 10:43 DMDO/coordinator.py
+-rw-rw-rw-  2.0 fat    26779 b- defN 24-Apr-28 00:45 DMDO/coordinator.py
 -rw-rw-rw-  2.0 fat    17388 b- defN 24-Apr-23 10:43 DMDO/preprocess.py
 -rw-rw-rw-  2.0 fat     5602 b- defN 24-Apr-23 10:43 DMDO/variables.py
--rw-rw-rw-  2.0 fat    27030 b- defN 24-Apr-23 10:44 DMDO-2401.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3355 b- defN 24-Apr-23 10:44 DMDO-2401.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 10:44 DMDO-2401.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-23 10:44 DMDO-2401.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1227 b- defN 24-Apr-23 10:44 DMDO-2401.dist-info/RECORD
-17 files, 158045 bytes uncompressed, 42669 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat    27030 b- defN 24-Apr-28 00:46 DMDO-2404.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3305 b- defN 24-Apr-28 00:46 DMDO-2404.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 00:46 DMDO-2404.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-28 00:46 DMDO-2404.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1227 b- defN 24-Apr-28 00:46 DMDO-2404.dist-info/RECORD
+17 files, 158107 bytes uncompressed, 42664 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: DMDO/preprocess.py
 Comment: 
 
 Filename: DMDO/variables.py
 Comment: 
 
-Filename: DMDO-2401.dist-info/LICENSE
+Filename: DMDO-2404.dist-info/LICENSE
 Comment: 
 
-Filename: DMDO-2401.dist-info/METADATA
+Filename: DMDO-2404.dist-info/METADATA
 Comment: 
 
-Filename: DMDO-2401.dist-info/WHEEL
+Filename: DMDO-2404.dist-info/WHEEL
 Comment: 
 
-Filename: DMDO-2401.dist-info/top_level.txt
+Filename: DMDO-2404.dist-info/top_level.txt
 Comment: 
 
-Filename: DMDO-2401.dist-info/RECORD
+Filename: DMDO-2404.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DMDO/coordinator.py

```diff
@@ -37,26 +37,28 @@
   n_dim: int = 0
   index: int = None
 
 @dataclass
 class ADMM_data(coordinationData):
   beta: float = 1.3
   gamma: float = 0.5
-  q: np.ndarray = np.zeros([0,0])
-  qold: np.ndarray = np.zeros([0,0])
+  q: np.ndarray = None
+  qold: np.ndarray = None
   phi: float = 1.0
-  v: np.ndarray = np.zeros([0,0])
-  w: np.ndarray = np.zeros([0,0])
+  v: np.ndarray = None
+  w: np.ndarray = None
   update_w: bool = False
   M_update_scheme: int = w_scheme.MEDIAN
   eps_qo: List = None
   save_q_in: bool = False
   save_q_in_out: bool = False
   eps_fo: List = None
 
+
+
 # COMPLETE: ADMM needs to be customized for this code
 @dataclass
 class ADMM(ADMM_data):
   " Alternating directions method of multipliers "
   # Constructor
   def __init__(self, nsp, beta, budget, index_of_master_SP, display, scaling, mode, M_update_scheme, store_q_o=False, store_q_io=False, index = None):
     global eps_fio, eps_qio
@@ -72,14 +74,20 @@
     self.M_update_scheme = M_update_scheme
     self.eps_qo = []
     self.save_q_out = store_q_o
     self.save_q_in_out = store_q_io
     self.eps_fo = []
     self.index = index
 
+    self.q = np.zeros([0,0])
+    self.qold = np.zeros([0,0])
+    self.phi: float = 1.0
+    self.v = np.zeros([0,0])
+    self.w = np.zeros([0,0])
+
   def clone_point(self, p: variableData):
     self.var_group.append(p)
 
   def create_linking_list(self):
     a = []
     b = []
     for i in range(self.nsp):
```

## Comparing `DMDO-2401.dist-info/LICENSE` & `DMDO-2404.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DMDO-2401.dist-info/METADATA` & `DMDO-2404.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: DMDO
-Version: 2401
+Version: 2404
 Summary: Distributed Multidisciplinary Design Optimization (DMDO)
 Home-page: https://github.com/Ahmed-Bayoumy/DMDO
 Author: Ahmed H. Bayoumy
 Author-email: ahmed.bayoumy@mail.mcgill.ca
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Ahmed-Bayoumy/DMDO/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: NOBM (>=1.0.1)
-Requires-Dist: numpy (==1.22.4)
-Requires-Dist: OMADS (==2401)
+Requires-Dist: pandas ==2.2.2
+Requires-Dist: NOBM ==2404.1
+Requires-Dist: numpy ==1.23.2
+Requires-Dist: OMADS ==2404.1
 Requires-Dist: pyyaml
 Provides-Extra: interactive
-Requires-Dist: matplotlib (>=3.5.2) ; extra == 'interactive'
-Requires-Dist: plotly (>=5.14.1) ; extra == 'interactive'
+Requires-Dist: matplotlib >=3.5.2 ; extra == 'interactive'
+Requires-Dist: plotly >=5.14.1 ; extra == 'interactive'
 
 [![pages-build-deployment](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/pages/pages-build-deployment/badge.svg?branch=DEV)](https://github.com/Ahmed-Bayoumy/DNDO/actions/workflows/pages/pages-build-deployment)
 [![lx-build-and-pytest](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/lx-build-and-tests.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/lx-build-and-tests.yml)
 [![win-build-and-pytest](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/win-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/win-build-and-pytest.yml)
 [![macos-build-and-pytest](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/macos-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/DMDO/actions/workflows/macos-build-and-pytest.yml)
 
 <img width="870" alt="DMDO_logo" src="DMDO_logo.png">
@@ -83,9 +81,7 @@
 ```
 
 
 
 
 
 
-
-
```

