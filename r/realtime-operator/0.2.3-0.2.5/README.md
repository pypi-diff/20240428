# Comparing `tmp/realtime_operator-0.2.3.tar.gz` & `tmp/realtime_operator-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_operator-0.2.3.tar", last modified: Sun Apr 21 20:40:31 2024, max compression
+gzip compressed data, was "realtime_operator-0.2.5.tar", last modified: Sat Apr 27 22:04:26 2024, max compression
```

## Comparing `realtime_operator-0.2.3.tar` & `realtime_operator-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 20:40:31.770110 realtime_operator-0.2.3/
--rw-rw-rw-   0        0        0     1094 2024-04-14 13:45:15.000000 realtime_operator-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     4275 2024-04-21 20:40:31.769109 realtime_operator-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3616 2024-04-14 13:45:15.000000 realtime_operator-0.2.3/README.md
--rw-rw-rw-   0        0        0      634 2024-04-21 20:40:08.000000 realtime_operator-0.2.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-21 20:40:31.752105 realtime_operator-0.2.3/realtime_operator/
--rw-rw-rw-   0        0        0        0 2024-04-14 13:45:15.000000 realtime_operator-0.2.3/realtime_operator/__init__.py
--rw-rw-rw-   0        0        0     6817 2024-04-21 19:53:43.000000 realtime_operator-0.2.3/realtime_operator/compression.py
--rw-rw-rw-   0        0        0    22662 2024-04-21 19:39:37.000000 realtime_operator-0.2.3/realtime_operator/single_operator.py
-drwxrwxrwx   0        0        0        0 2024-04-21 20:40:31.769109 realtime_operator-0.2.3/realtime_operator.egg-info/
--rw-rw-rw-   0        0        0     4275 2024-04-21 20:40:31.000000 realtime_operator-0.2.3/realtime_operator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-21 20:40:31.000000 realtime_operator-0.2.3/realtime_operator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 20:40:31.000000 realtime_operator-0.2.3/realtime_operator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-21 20:40:31.000000 realtime_operator-0.2.3/realtime_operator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-21 20:40:31.000000 realtime_operator-0.2.3/realtime_operator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 20:40:31.770110 realtime_operator-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-14 13:45:15.000000 realtime_operator-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 20:40:31.768110 realtime_operator-0.2.3/tests/
--rw-rw-rw-   0        0        0     2258 2024-04-21 19:47:13.000000 realtime_operator-0.2.3/tests/test_compression.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:41:37.000000 realtime_operator-0.2.3/tests/test_single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.796687 realtime_operator-0.2.5/
+-rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     4367 2024-04-27 22:04:26.794899 realtime_operator-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/README.md
+-rw-rw-rw-   0        0        0      695 2024-04-27 22:04:11.000000 realtime_operator-0.2.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.749045 realtime_operator-0.2.5/realtime_operator/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/realtime_operator/__init__.py
+-rw-rw-rw-   0        0        0    13309 2024-04-27 21:12:33.000000 realtime_operator-0.2.5/realtime_operator/compression.py
+-rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.5/realtime_operator/single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.787515 realtime_operator-0.2.5/realtime_operator.egg-info/
+-rw-rw-rw-   0        0        0     4367 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 22:04:26.796687 realtime_operator-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.787515 realtime_operator-0.2.5/tests/
+-rw-rw-rw-   0        0        0     2720 2024-04-27 21:01:53.000000 realtime_operator-0.2.5/tests/test_compression.py
+-rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.5/tests/test_single_operator.py
```

### Comparing `realtime_operator-0.2.3/LICENSE` & `realtime_operator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.3/PKG-INFO` & `realtime_operator-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.3
+Version: 0.2.5
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: pytest
+Requires-Dist: pytest-benchmark
+Requires-Dist: python-dateutil
 
 #Time Series Analysis and Signal Processing Library
 
 ## Overview
 
 This library offers a comprehensive suite of tools for time series analysis and signal processing, leveraging the power of NumPy and Numba for high performance computations. It includes functionalities for datetime manipulation, signal generation, buffer updates, moving averages, and much more. Designed for researchers and engineers working in data analysis, finance, or signal processing, this library streamlines complex numerical computations and analyses.
```

### Comparing `realtime_operator-0.2.3/README.md` & `realtime_operator-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.3/pyproject.toml` & `realtime_operator-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [project]
 name = "realtime_operator"
-version = "0.2.3"
+version = "0.2.5"
 authors = [
   { name="Ernst Holger Amort", email="holgeramort@gmail.com" },
 ]
 description = "A package to perfom real-time operations on time seriesdata streams."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  'matplotlib',
   'numba',
   'numpy',
   'pytest',
+  'pytest-benchmark',
+  'python-dateutil'
 ]
 
 [project.urls]
 Homepage = "https://github.com/ErnstHolger/realtime_operator"
 Issues = "https://github.com/ErnstHolger/realtime_operator/issues"
```

### Comparing `realtime_operator-0.2.3/realtime_operator/single_operator.py` & `realtime_operator-0.2.5/realtime_operator/single_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,29 +275,35 @@
     if state[1] == 0:
         state[0] = z
         state[1] = t
         state[2] = z
         return t, state[0]
 
     delta = t - state[1]
+    # ooo event
+    if delta < 0:
+        # return previous state
+        return state[1], state[0]
     if delta == 0:
-        delta = 1e-6
+        # update previous value
+        state[2]=(state[2]+z)/2
+        return state[1], state[0]
     alpha = delta / tau
     mu = math.exp(-alpha)
     nu = 0
     if inter == -1:
         nu = 1
     elif inter == 0:
         nu = (1 - mu) / alpha
     elif inter == 1:
         nu = mu
     state[0] = mu * state[0] + (nu - mu) * state[2] + (1 - nu) * z
     state[1] = t
     state[2] = z
-    return t, state[+0]
+    return t, state[0]
 
 
 @nb.jit("Tuple((f8, f8))(f8, i8, i8, f8[:], f8, f8)", nopython=True)
 def nema(tau, inter, n, state, t, z):
     """
     Calculates the NEMA (Normalized Exponential Moving Average) value.
```

### Comparing `realtime_operator-0.2.3/realtime_operator.egg-info/PKG-INFO` & `realtime_operator-0.2.5/realtime_operator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.3
+Version: 0.2.5
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: pytest
+Requires-Dist: pytest-benchmark
+Requires-Dist: python-dateutil
 
 #Time Series Analysis and Signal Processing Library
 
 ## Overview
 
 This library offers a comprehensive suite of tools for time series analysis and signal processing, leveraging the power of NumPy and Numba for high performance computations. It includes functionalities for datetime manipulation, signal generation, buffer updates, moving averages, and much more. Designed for researchers and engineers working in data analysis, finance, or signal processing, this library streamlines complex numerical computations and analyses.
```

### Comparing `realtime_operator-0.2.3/tests/test_compression.py` & `realtime_operator-0.2.5/tests/test_compression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 import numpy as np
+import time
 
-
-from compression import (
+from realtime_operator.compression import (
+    COMPRESSION_TYPE,
+    interpolate,    
+    interpolate_fast,
+    any_compression,
     deduplicate,
     minimum_timedelta,
     exception_deviation,
     exception_deviation_previous,
     swinging_door,
 )
 
 t = np.arange(1, 20, dtype=float) + 1
 z = np.arange(1, 20, dtype=float)
 state = np.zeros(4, dtype=float)
 
 
+def test_interpolate_fast():
+    t = np.arange(1, 20,1, dtype=float)
+    tn= np.arange(0, 20,0.001, dtype=float) 
+
+    zn=interpolate(tn,t,z)
+    zm=interpolate_fast(tn,t,z)
+
+    zn = np.where(np.isnan(zn), 0, zn)
+    zm = np.where(np.isnan(zm), 0, zm)
+    assert np.all(zn == zm)
+
+
 def test_deduplicate():
     state = np.zeros(3, dtype=float)
-    zp = [1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 3, 3]
+    zp = [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 2.0, 3.0, 3.0]
     n = len(zp)
     result = []
     for i in range(n):
-        _, zn, _ = deduplicate(state, t[i], zp[i])
+        _ , zn, _ = deduplicate(state, t[i], zp[i],0.0, 1e6)
         for i in zn:
             result.append(i)
 
     desired_array = np.array([1.0, 2.0, 3.0])
     assert np.all(np.array(result) == desired_array)
```

### Comparing `realtime_operator-0.2.3/tests/test_single_operator.py` & `realtime_operator-0.2.5/tests/test_single_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,24 +122,50 @@
     for i in range(9):
         tn, zn = ema(1, 0, state, t[i], z[i])
 
     assert tn == t[-1]
     assert zn > z[-2]
     assert zn < z[-1]
 
+def test_ema_ooo():
+    t, z, state = create_test_data()
+
+    # add ooo event
+    t[6]=1
+    z[6]=100_000
+    zn = 0
+    for i in range(9):
+        tn, zn = ema(1, 0, state, t[i], z[i])
+
+    assert tn == t[-1]
+    assert zn > z[-2]
+    assert zn < z[-1]
+
 
 def test_nema():
     t, z, state = create_test_data()
     zn = 0
     for i in range(9):
         state[0] = 0
         tn, zn = nema(1, 0, 5, state, t[i], z[i])
 
     assert tn == t[-1]
     assert zn < z[-1]
+
+def test_nema_ooo():
+    t, z, state = create_test_data()
+    t[6]=1
+    z[6]=100_000
+    zn = 0
+    for i in range(9):
+        state[0] = 0
+        tn, zn = nema(1, 0, 5, state, t[i], z[i])
+
+    assert tn == t[-1]
+    assert zn < z[-1]
 
 
 def test_delta():
     t, z, state = create_test_data()
     zn = 0
     for i in range(9):
         state[0] = 0
```

