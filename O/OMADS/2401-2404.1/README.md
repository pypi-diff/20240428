# Comparing `tmp/OMADS-2401-py3-none-any.whl.zip` & `tmp/OMADS-2404.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 63444 bytes, number of entries: 15
+Zip file size: 64015 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat     7401 b- defN 24-Jan-28 22:46 OMADS/Barriers.py
--rw-rw-rw-  2.0 fat    18479 b- defN 24-Jan-28 22:46 OMADS/Directions.py
+-rw-rw-rw-  2.0 fat    18591 b- defN 24-Apr-26 22:22 OMADS/Directions.py
 -rw-rw-rw-  2.0 fat    23768 b- defN 24-Jan-28 23:38 OMADS/MADS.py
--rw-rw-rw-  2.0 fat    23956 b- defN 24-Jan-28 23:37 OMADS/POLL.py
--rw-rw-rw-  2.0 fat    12359 b- defN 24-Jan-28 22:46 OMADS/Point.py
--rw-rw-rw-  2.0 fat    61767 b- defN 24-Jan-28 23:39 OMADS/SEARCH.py
+-rw-rw-rw-  2.0 fat    23956 b- defN 24-Apr-26 19:22 OMADS/POLL.py
+-rw-rw-rw-  2.0 fat      743 b- defN 24-Apr-24 07:23 OMADS/Perf_indicator.py
+-rw-rw-rw-  2.0 fat    12413 b- defN 24-Apr-26 22:23 OMADS/Point.py
+-rw-rw-rw-  2.0 fat    61906 b- defN 24-Apr-27 22:53 OMADS/SEARCH.py
 -rw-rw-rw-  2.0 fat      386 b- defN 23-Jun-02 04:52 OMADS/__init__.py
--rw-rw-rw-  2.0 fat    26086 b- defN 24-Jan-29 00:41 OMADS/_common.py
--rw-rw-rw-  2.0 fat     4311 b- defN 24-Jan-28 22:46 OMADS/_globals.py
+-rw-rw-rw-  2.0 fat    26194 b- defN 24-Apr-26 22:22 OMADS/_common.py
+-rw-rw-rw-  2.0 fat     4311 b- defN 24-Apr-27 02:13 OMADS/_globals.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-02 04:48 OMADS/py.typed
--rw-rw-rw-  2.0 fat    35823 b- defN 24-Jan-29 03:07 OMADS-2401.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10316 b- defN 24-Jan-29 03:07 OMADS-2401.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jan-29 03:07 OMADS-2401.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Jan-29 03:07 OMADS-2401.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1099 b- defN 24-Jan-29 03:07 OMADS-2401.dist-info/RECORD
-15 files, 225849 bytes uncompressed, 61684 bytes compressed:  72.7%
+-rw-rw-rw-  2.0 fat    35823 b- defN 24-Apr-27 23:48 OMADS-2404.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10259 b- defN 24-Apr-27 23:48 OMADS-2404.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 23:48 OMADS-2404.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-27 23:48 OMADS-2404.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1188 b- defN 24-Apr-27 23:48 OMADS-2404.1.dist-info/RECORD
+16 files, 227037 bytes uncompressed, 62113 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: OMADS/MADS.py
 Comment: 
 
 Filename: OMADS/POLL.py
 Comment: 
 
+Filename: OMADS/Perf_indicator.py
+Comment: 
+
 Filename: OMADS/Point.py
 Comment: 
 
 Filename: OMADS/SEARCH.py
 Comment: 
 
 Filename: OMADS/__init__.py
@@ -24,23 +27,23 @@
 
 Filename: OMADS/_globals.py
 Comment: 
 
 Filename: OMADS/py.typed
 Comment: 
 
-Filename: OMADS-2401.dist-info/LICENSE
+Filename: OMADS-2404.1.dist-info/LICENSE
 Comment: 
 
-Filename: OMADS-2401.dist-info/METADATA
+Filename: OMADS-2404.1.dist-info/METADATA
 Comment: 
 
-Filename: OMADS-2401.dist-info/WHEEL
+Filename: OMADS-2404.1.dist-info/WHEEL
 Comment: 
 
-Filename: OMADS-2401.dist-info/top_level.txt
+Filename: OMADS-2404.1.dist-info/top_level.txt
 Comment: 
 
-Filename: OMADS-2401.dist-info/RECORD
+Filename: OMADS-2404.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## OMADS/Directions.py

```diff
@@ -14,50 +14,54 @@
     :param _defined: A boolean that indicate if the poll points are defined
   """
   _poll_dirs: List[Point] = field(default_factory=list)
   _point_index: List[int] = field(default_factory=list)
   _n: int = 0
   _defined: List[bool] = field(default_factory=lambda: [False])
   scaling: List[List[float]] = field(default_factory=list)
-  _xmin: Point = Point()
-  _x_sc: Point = Point()
+  _xmin: Point = None
+  _x_sc: Point = None
   _nb_success: int = 0
   _bb_eval: int = field(default_factory=int)
   _psize: float = field(default_factory=float)
   _iter: int = field(default_factory=int)
   hashtable: Cache = field(default_factory=Cache)
   _check_cache: bool = True
   _display: bool = True
   _store_cache: bool = True
   _save_results = True
   mesh: OrthoMesh = field(default_factory=OrthoMesh)
   _opportunistic: bool = False
   _eval_budget: int = 100
-  _dtype: DType = DType()
+  _dtype: DType = None
   bb_handle: Evaluator = field(default_factory=Evaluator)
   _success: bool = False
   _seed: int = 0
   _terminate: bool = False
   _bb_output: List[float] = field(default_factory=list)
   Failure_stop: bool = None
   RHO: float = MPP.RHO
   LAMBDA: List[float] = None
   hmax: float = 1.
   log: logger = None
   n_successes: int = 0
 
+  def __post_init__(self):
+    self._dtype = DType()
+    self._xmin: Point = Point()
+    self._x_sc: Point = Point()
+
   @property
   def x_sc(self) -> Point:
     return self._x_sc
   
   @x_sc.setter
   def x_sc(self, value: Point):
     self._x_sc = value
   
-
   @property
   def bb_output(self) -> List[float]:
     return self._bb_output
 
   @bb_output.setter
   def bb_output(self, other: List[float]):
     self._bb_output = other
```

## OMADS/Point.py

```diff
@@ -38,15 +38,15 @@
   _c_eq: List[float] = field(default_factory=list)
   # Aggregated constraints; active set
   _h: float = inf
   # hash signature; facilitate looking for duplicates and storing coordinates,
   # hash signature, in the cache memory
   _signature: int = 0
   # numpy double data type precision
-  _dtype: DType = DType()
+  _dtype: DType = None
   # Variables type
   _var_type: List[int] = None
   # Discrete set
   _sets: Dict = None
 
   _var_link: List[str] = None
 
@@ -67,14 +67,17 @@
 
   source: str = "Current run"
 
   Model: str = "Simulation"
 
   _hzero: float = None
 
+  def __post_init__(self):
+    self._dtype = DType()
+
   @property
   def hzero(self):
     if self._hzero is None:
       return self._dtype.zero
     else:
       return self._hzero
```

## OMADS/SEARCH.py

```diff
@@ -315,28 +315,28 @@
 
 
 
 @dataclass
 class efficient_exploration:
   mesh: OrthoMesh  = field(default_factory=OrthoMesh)
   _success: bool = False
-  _xmin: Point = Point()
-  prob_params: Parameters = Parameters()
+  _xmin: Point = None
+  prob_params: Parameters = None
   sampling_t: int = 3
   _seed: int = 0
-  _dtype: DType = DType()
+  _dtype: DType = None
   iter: int = 1
   vicinity_ratio: np.ndarray = None
   vicinity_min: float = 0.001
   opportunistic: bool = False
   eval_budget: int = 10
   store_cache: bool = True
   check_cache: bool = True
   display: bool = False
-  bb_handle: Evaluator = Evaluator()
+  bb_handle: Evaluator = None
   bb_output: List = None
   samples: List[Point] = None
   hashtable: Cache = None
   _dim: int = 0
   nb_success: int = 0
   terminate: bool =False
   _save_results: bool = False
@@ -350,14 +350,20 @@
   hmax: float = 0.
   log: logger = None
   AS: explore.samplers.activeSampling = None
   best_samples: int = 0
   estGrid: explore.samplers.sampling = None
   n_successes: int = 0 
 
+  def __post_init__(self):
+    self._xmin = Point()
+    self.bb_handle = Evaluator()
+    self._dtype = DType()
+    self.prob_params = Parameters()
+
   @property
   def type(self):
     return self._type
   
   @type.setter
   def type(self, value: Any) -> Any:
     self._type = value
@@ -479,16 +485,16 @@
     is_AS = False
     v = np.empty((self.nvars, 2))
     if self.bb_handle.bb_eval + nsamples > self.eval_budget:
       nsamples = self.eval_budget + self.bb_handle.bb_eval
     if self.xmin and self.iter > 1 and self.sampling_t != SAMPLING_METHOD.ACTIVE.name:
       for i in range(len(self.prob_params.lb)):
         D = abs(self.prob_params.ub[i] - self.prob_params.lb[i])
-        lb = copy.deepcopy(self.xmin.coordinates[i]-(D * self.vicinity_ratio[i]))
-        ub = copy.deepcopy(self.xmin.coordinates[i]+(D * self.vicinity_ratio[i]))
+        lb = copy.deepcopy(self.xmin.coordinates[i]-(D * self.vicinity_ratio[i][0]))
+        ub = copy.deepcopy(self.xmin.coordinates[i]+(D * self.vicinity_ratio[i][0]))
         if lb <= self.prob_params.lb[i]:
           lb = copy.deepcopy(self.prob_params.lb[i])
         elif  lb >= self.prob_params.ub[i]:
           lb = self.xmin.coordinates[i]
         if ub >= self.prob_params.ub[i]:
           ub = copy.deepcopy(self.prob_params.ub[i])
         elif ub <= self.prob_params.lb[i]:
```

## OMADS/_common.py

```diff
@@ -298,17 +298,20 @@
   commandOptions: Any = None
   internal: Optional[str] = None
   path: str = "..\\tests\\Rosen"
   input: str = "input.inp"
   output: str = "output.out"
   constants: List = None
   bb_eval: int = 0
-  _dtype: DType = DType()
+  _dtype: DType = None
   timeout: float = 1000000.
 
+  def __post_init__(self):
+    self._dtype = DType()
+
   @property
   def dtype(self):
     return self._dtype
 
   def eval(self, values: List[float]):
     """ Evaluate the poll point
 
@@ -473,15 +476,18 @@
   # See: Audet et. al, The mesh adaptive direct search algorithm for
   # granular and discrete variable
   _exp: int = 0
   _mantissa: int = 1
   psize_max: float = 0.0
   psize_success: float = 0.0
   # numpy double data type precision
-  _dtype: DType = DType()
+  _dtype: DType = None
+
+  def __post_init__(self):
+    self._dtype = DType()
 
   @property
   def dtype(self):
     return self._dtype
 
   @dtype.setter
   def dtype(self, other: DType):
```

## Comparing `OMADS-2401.dist-info/LICENSE` & `OMADS-2404.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `OMADS-2401.dist-info/METADATA` & `OMADS-2404.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: OMADS
-Version: 2401
+Version: 2404.1
 Summary: Mesh Adaptive Direct Search (MADS)
 Home-page: https://github.com/Ahmed-Bayoumy/OMADS
 Author: Ahmed H. Bayoumy
 Author-email: ahmed.bayoumy@mail.mcgill.ca
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Ahmed-Bayoumy/OMADS/issues
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
-Requires-Dist: samplersLib (>=24.1.3)
-Requires-Dist: cocopp (==2.6.3)
-Requires-Dist: NOBM (>=1.0.1)
-Requires-Dist: numpy (==1.22.4)
-Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: setuptools (>=58.1.0)
-Requires-Dist: pyDOE2 (==1.3.0)
-Requires-Dist: scipy (==1.8.1)
+Requires-Dist: samplersLib >=24.1.3
+Requires-Dist: cocopp ==2.6.3
+Requires-Dist: NOBM ==2404.1
+Requires-Dist: numpy ==1.23.2
+Requires-Dist: pandas >=2.2.2
+Requires-Dist: setuptools >=58.1.0
+Requires-Dist: pyDOE2 ==1.3.0
+Requires-Dist: scipy ==1.13.0
 Provides-Extra: interactive
-Requires-Dist: matplotlib (>=3.5.2) ; extra == 'interactive'
-Requires-Dist: plotly (>=5.14.1) ; extra == 'interactive'
+Requires-Dist: matplotlib >=3.5.2 ; extra == 'interactive'
+Requires-Dist: plotly >=5.14.1 ; extra == 'interactive'
 
 [![pages-build-deployment](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment/badge.svg?branch=DEV)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/pages/pages-build-deployment)
 [![lx-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/lx-build-and-tests.yml)
 [![win-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/win-build-and-pytest.yml)
 [![macos-build-and-pytest](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml/badge.svg)](https://github.com/Ahmed-Bayoumy/OMADS/actions/workflows/macos-build-and-pytest.yml)
 
 <img width="870" alt="OMADS_logo" src="https://github.com/Ahmed-Bayoumy/OMADS/assets/22842095/dedff4b1-4ec5-4b1f-a155-8b64155d1558">
@@ -215,9 +213,7 @@
  psize_success = 1.0
  psize_max = 2.0
 ```
 
 https://github.com/Ahmed-Bayoumy/OMADS/assets/22842095/5dc72c34-4722-4d93-8c84-d17f5595556d
 
 
-
-
```

