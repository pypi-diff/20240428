# Comparing `tmp/SplitFDM-0.1.1.tar.gz` & `tmp/SplitFDM-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplitFDM-0.1.1.tar", last modified: Tue Jan  3 06:03:12 2023, max compression
+gzip compressed data, was "SplitFDM-0.1.2.tar", last modified: Sun Apr 28 05:49:50 2024, max compression
```

## Comparing `SplitFDM-0.1.1.tar` & `SplitFDM-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-03 06:03:12.211145 SplitFDM-0.1.1/
--rw-r--r--   0 apple      (501) staff       (20)     2873 2023-01-03 06:03:12.210358 SplitFDM-0.1.1/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     2184 2023-01-03 06:02:12.000000 SplitFDM-0.1.1/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-03 06:03:12.190419 SplitFDM-0.1.1/SplitFDM.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2873 2023-01-03 06:03:12.000000 SplitFDM-0.1.1/SplitFDM.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      467 2023-01-03 06:03:12.000000 SplitFDM-0.1.1/SplitFDM.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-01-03 06:03:12.000000 SplitFDM-0.1.1/SplitFDM.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-01-03 06:01:01.000000 SplitFDM-0.1.1/SplitFDM.egg-info/not-zip-safe
--rw-r--r--   0 apple      (501) staff       (20)       42 2023-01-03 06:03:12.000000 SplitFDM-0.1.1/SplitFDM.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        9 2023-01-03 06:03:12.000000 SplitFDM-0.1.1/SplitFDM.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-01-03 06:03:12.211278 SplitFDM-0.1.1/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     1052 2023-01-03 06:02:45.000000 SplitFDM-0.1.1/setup.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-03 06:03:12.208350 SplitFDM-0.1.1/splitfdm/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-25 19:48:42.000000 SplitFDM-0.1.1/splitfdm/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2172 2023-01-02 00:44:40.000000 SplitFDM-0.1.1/splitfdm/bc.py
--rw-r--r--   0 apple      (501) staff       (20)     3330 2023-01-03 05:56:06.000000 SplitFDM-0.1.1/splitfdm/boundary.py
--rw-r--r--   0 apple      (501) staff       (20)     3228 2023-01-02 00:52:58.000000 SplitFDM-0.1.1/splitfdm/cell.py
--rw-r--r--   0 apple      (501) staff       (20)     1855 2023-01-03 05:56:06.000000 SplitFDM-0.1.1/splitfdm/derivatives.py
--rw-r--r--   0 apple      (501) staff       (20)     7358 2023-01-03 05:56:06.000000 SplitFDM-0.1.1/splitfdm/domain.py
--rw-r--r--   0 apple      (501) staff       (20)       87 2023-01-03 05:56:06.000000 SplitFDM-0.1.1/splitfdm/error.py
--rw-r--r--   0 apple      (501) staff       (20)     1563 2023-01-02 01:15:43.000000 SplitFDM-0.1.1/splitfdm/initialize.py
--rw-r--r--   0 apple      (501) staff       (20)      348 2023-01-02 01:16:53.000000 SplitFDM-0.1.1/splitfdm/model.py
--rw-r--r--   0 apple      (501) staff       (20)    10465 2023-01-03 05:56:07.000000 SplitFDM-0.1.1/splitfdm/refine.py
--rw-r--r--   0 apple      (501) staff       (20)     8713 2023-01-03 05:59:55.000000 SplitFDM-0.1.1/splitfdm/simulation.py
--rw-r--r--   0 apple      (501) staff       (20)     1544 2023-01-03 06:00:08.000000 SplitFDM-0.1.1/splitfdm/system.py
--rw-r--r--   0 apple      (501) staff       (20)      332 2023-01-02 01:39:54.000000 SplitFDM-0.1.1/splitfdm/visualize.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-28 05:49:50.192505 SplitFDM-0.1.2/
+-rw-r--r--   0 apple      (501) staff       (20)     3583 2024-04-28 05:49:50.183320 SplitFDM-0.1.2/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     2312 2024-04-28 04:50:48.000000 SplitFDM-0.1.2/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-28 05:49:50.155869 SplitFDM-0.1.2/SplitFDM.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     3583 2024-04-28 05:49:49.000000 SplitFDM-0.1.2/SplitFDM.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      489 2024-04-28 05:49:50.000000 SplitFDM-0.1.2/SplitFDM.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-04-28 05:49:49.000000 SplitFDM-0.1.2/SplitFDM.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-04-28 05:49:49.000000 SplitFDM-0.1.2/SplitFDM.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)       42 2024-04-28 05:49:49.000000 SplitFDM-0.1.2/SplitFDM.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        9 2024-04-28 05:49:49.000000 SplitFDM-0.1.2/SplitFDM.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2024-04-28 05:49:50.192726 SplitFDM-0.1.2/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     1052 2024-04-28 05:48:48.000000 SplitFDM-0.1.2/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-28 05:49:50.182458 SplitFDM-0.1.2/splitfdm/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     6289 2024-04-28 04:48:33.000000 SplitFDM-0.1.2/splitfdm/bc.py
+-rw-r--r--   0 apple      (501) staff       (20)     3300 2024-04-27 07:05:25.000000 SplitFDM-0.1.2/splitfdm/boundary.py
+-rw-r--r--   0 apple      (501) staff       (20)     3228 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/cell.py
+-rw-r--r--   0 apple      (501) staff       (20)      124 2024-04-27 07:03:49.000000 SplitFDM-0.1.2/splitfdm/constants.py
+-rw-r--r--   0 apple      (501) staff       (20)     1876 2024-04-27 17:05:08.000000 SplitFDM-0.1.2/splitfdm/derivatives.py
+-rw-r--r--   0 apple      (501) staff       (20)     7503 2024-04-27 08:59:04.000000 SplitFDM-0.1.2/splitfdm/domain.py
+-rw-r--r--   0 apple      (501) staff       (20)       87 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/error.py
+-rw-r--r--   0 apple      (501) staff       (20)     1563 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/initialize.py
+-rw-r--r--   0 apple      (501) staff       (20)      348 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/model.py
+-rw-r--r--   0 apple      (501) staff       (20)    10465 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/refine.py
+-rw-r--r--   0 apple      (501) staff       (20)     8713 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/simulation.py
+-rw-r--r--   0 apple      (501) staff       (20)     1544 2024-04-27 05:01:39.000000 SplitFDM-0.1.2/splitfdm/system.py
+-rw-r--r--   0 apple      (501) staff       (20)      364 2024-04-27 08:58:46.000000 SplitFDM-0.1.2/splitfdm/visualize.py
```

### Comparing `SplitFDM-0.1.1/PKG-INFO` & `SplitFDM-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: SplitFDM
-Version: 0.1.1
-Summary: 1D Finite-Difference Split Newton Solver
-Home-page: https://github.com/gpavanb1/SplitFDM
-Author: gpavanb1
-Author-email: gpavanb@gmail.com
-License: MIT
-Project-URL: Bug Reports, https://github.com/gpavanb1/SplitFDM/issues
-Project-URL: Source, https://github.com/gpavanb1/SplitFDM/
-Keywords: amr newton python finite-difference armijo optimization pseudotransient splitting
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-
 # SplitFDM
 
 [![Downloads](https://pepy.tech/badge/splitfdm)](https://pepy.tech/project/splitfdm)
 
 ![img](https://github.com/gpavanb1/SplitFDM/blob/main/assets/logo.jpg)
 
 1D [Finite-Difference](https://en.wikipedia.org/wiki/Finite_difference_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
@@ -51,15 +34,24 @@
 
 # Define the domain and variables
 # ng stands for ghost point count
 d = Domain.from_size(nx=20, ng=2, ["u", "v"])
 
 # Set IC and BC
 ics = {"u": "gaussian", "v": "rarefaction"}
-bcs = {"u": "periodic", "v": "periodic"}
+bcs = {
+    "u": {
+        "left": "periodic",
+        "right": "periodic"
+    },
+    "v": {
+        "left": {"dirichlet": 3},
+        "right": {"dirichlet": 4}
+    }
+}
 s = Simulation(d, m, ics, bcs)
 
 # Advance in time or to steady state
 s.evolve(dt=0.1)
 iter = s.steady_state()
 
 # Visualize
@@ -71,8 +63,8 @@
 Please direct your queries to [gpavanb1](http://github.com/gpavanb1)
 for any questions.
 
 ## Acknowledgements
 
 Do visit its [Finite-Volume](https://github.com/gpavanb1/SplitFVM) cousin
 
-Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture.
+Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture.
```

### Comparing `SplitFDM-0.1.1/SplitFDM.egg-info/PKG-INFO` & `SplitFDM-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 Metadata-Version: 2.1
 Name: SplitFDM
-Version: 0.1.1
+Version: 0.1.2
 Summary: 1D Finite-Difference Split Newton Solver
 Home-page: https://github.com/gpavanb1/SplitFDM
 Author: gpavanb1
 Author-email: gpavanb@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/gpavanb1/SplitFDM/issues
 Project-URL: Source, https://github.com/gpavanb1/SplitFDM/
+Description: # SplitFDM
+        
+        [![Downloads](https://pepy.tech/badge/splitfdm)](https://pepy.tech/project/splitfdm)
+        
+        ![img](https://github.com/gpavanb1/SplitFDM/blob/main/assets/logo.jpg)
+        
+        1D [Finite-Difference](https://en.wikipedia.org/wiki/Finite_difference_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
+        
+        ## What does 'split' mean?
+        
+        The system is divided into two and for ease of communication, let's refer to first set of variables as "outer" and the second as "inner".
+        
+        * Holding the outer variables fixed, Newton iteration is performed till convergence using the sub-Jacobian
+        
+        * One Newton step is performed for the outer variables with inner held fixed (using its sub-Jacobian)
+        
+        * This process is repeated till convergence criterion is met for the full system (same as in Newton)
+        
+        ## How to install and execute?
+        
+        Just run 
+        ```
+        pip install splitfdm
+        ```
+        
+        There is an [examples](https://github.com/gpavanb1/SplitFDM/examples) folder that contains a test model - [Advection-Diffusion](https://en.wikipedia.org/wiki/Convection%E2%80%93diffusion_equation)
+        
+        You can define your own equations by simply creating a derived class from `Model` and adding to the `_equations` using existing or custom equations!
+        
+        A basic driver program is as follows
+        ```
+        # Define the problem
+        m = AdvectionDiffusion(c=0.2, nu=0.001)
+        
+        # Define the domain and variables
+        # ng stands for ghost point count
+        d = Domain.from_size(nx=20, ng=2, ["u", "v"])
+        
+        # Set IC and BC
+        ics = {"u": "gaussian", "v": "rarefaction"}
+        bcs = {
+            "u": {
+                "left": "periodic",
+                "right": "periodic"
+            },
+            "v": {
+                "left": {"dirichlet": 3},
+                "right": {"dirichlet": 4}
+            }
+        }
+        s = Simulation(d, m, ics, bcs)
+        
+        # Advance in time or to steady state
+        s.evolve(dt=0.1)
+        iter = s.steady_state()
+        
+        # Visualize
+        draw(d)
+        ```
+        
+        ## Whom to contact?
+        
+        Please direct your queries to [gpavanb1](http://github.com/gpavanb1)
+        for any questions.
+        
+        ## Acknowledgements
+        
+        Do visit its [Finite-Volume](https://github.com/gpavanb1/SplitFVM) cousin
+        
+        Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture.
 Keywords: amr newton python finite-difference armijo optimization pseudotransient splitting
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-
-# SplitFDM
-
-[![Downloads](https://pepy.tech/badge/splitfdm)](https://pepy.tech/project/splitfdm)
-
-![img](https://github.com/gpavanb1/SplitFDM/blob/main/assets/logo.jpg)
-
-1D [Finite-Difference](https://en.wikipedia.org/wiki/Finite_difference_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
-
-## What does 'split' mean?
-
-The system is divided into two and for ease of communication, let's refer to first set of variables as "outer" and the second as "inner".
-
-* Holding the outer variables fixed, Newton iteration is performed till convergence using the sub-Jacobian
-
-* One Newton step is performed for the outer variables with inner held fixed (using its sub-Jacobian)
-
-* This process is repeated till convergence criterion is met for the full system (same as in Newton)
-
-## How to install and execute?
-
-Just run 
-```
-pip install splitfdm
-```
-
-There is an [examples](https://github.com/gpavanb1/SplitFDM/examples) folder that contains a test model - [Advection-Diffusion](https://en.wikipedia.org/wiki/Convection%E2%80%93diffusion_equation)
-
-You can define your own equations by simply creating a derived class from `Model` and adding to the `_equations` using existing or custom equations!
-
-A basic driver program is as follows
-```
-# Define the problem
-m = AdvectionDiffusion(c=0.2, nu=0.001)
-
-# Define the domain and variables
-# ng stands for ghost point count
-d = Domain.from_size(nx=20, ng=2, ["u", "v"])
-
-# Set IC and BC
-ics = {"u": "gaussian", "v": "rarefaction"}
-bcs = {"u": "periodic", "v": "periodic"}
-s = Simulation(d, m, ics, bcs)
-
-# Advance in time or to steady state
-s.evolve(dt=0.1)
-iter = s.steady_state()
-
-# Visualize
-draw(d)
-```
-
-## Whom to contact?
-
-Please direct your queries to [gpavanb1](http://github.com/gpavanb1)
-for any questions.
-
-## Acknowledgements
-
-Do visit its [Finite-Volume](https://github.com/gpavanb1/SplitFVM) cousin
-
-Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture.
```

### Comparing `SplitFDM-0.1.1/setup.py` & `SplitFDM-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="SplitFDM",
-    version="0.1.1",
+    version="0.1.2",
     description="1D Finite-Difference Split Newton Solver",
     url="https://github.com/gpavanb1/SplitFDM",
     author="gpavanb1",
     author_email="gpavanb@gmail.com",
     license="MIT",
     packages=["splitfdm"],
     install_requires=["numpy", "numdifftools", "matplotlib", "splitnewton"],
```

### Comparing `SplitFDM-0.1.1/splitfdm/boundary.py` & `SplitFDM-0.1.2/splitfdm/boundary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
-from enum import Enum
+from .constants import btype
 from .error import SFDM
 
-btype = Enum("btype", "LEFT RIGHT")
-
 
 class Boundary:
     """
     A class representing a boundary cell in a domain.
 
     Parameters
     ----------
```

### Comparing `SplitFDM-0.1.1/splitfdm/cell.py` & `SplitFDM-0.1.2/splitfdm/cell.py`

 * *Files identical despite different names*

### Comparing `SplitFDM-0.1.1/splitfdm/derivatives.py` & `SplitFDM-0.1.2/splitfdm/derivatives.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 
     if scheme == Schemes.CENTRAL:
         if len(cell_sub) != 3:
             raise SFDM("Improper stencil size for central difference scheme")
 
         ul = cell_sub[0].values()
         ur = cell_sub[2].values()
-
+        Fl = F(ul)
+        Fr = F(ur)
         dx = cell_sub[2].x() - cell_sub[0].x()
 
-        return (ur - ul) / dx
+        return (Fr - Fl) / dx
     else:
         raise SFDM("Unsupported scheme")
 
 
 def D2x(D, cell_sub, scheme):
     """
     Calculate the second derivative of a given stencil.
@@ -62,22 +63,22 @@
             raise SFDM("Improper stencil size for central difference scheme")
 
         # West derivative
         ul = cell_sub[0].values()
         uc = cell_sub[1].values()
         Dl = D(ul)
         Dr = D(uc)
-        dxw = 0.5 * (cell_sub[1].x() - cell_sub[0].x())
+        dxw = cell_sub[1].x() - cell_sub[0].x()
         Dw = (Dr - Dl) / dxw
 
         # East derivative
         uc = cell_sub[1].values()
         ur = cell_sub[2].values()
         Dl = D(uc)
         Dr = D(ur)
-        dxe = 0.5 * (cell_sub[2].x() - cell_sub[1].x())
+        dxe = cell_sub[2].x() - cell_sub[1].x()
         De = (Dr - Dl) / dxe
 
         dx = 0.5 * (dxw + dxe)
         return (De - Dw) / dx
     else:
         raise SFDM("Unsupported scheme")
```

### Comparing `SplitFDM-0.1.1/splitfdm/domain.py` & `SplitFDM-0.1.2/splitfdm/domain.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         """
         Initialize a `Domain` object.
         """
         # Boundaries list contains both left and right
         # nb indicates number on each side
         self._nb = int(len(boundaries) / 2)
         self._nx = len(cells)
-        self._domain = [*(boundaries[: self._nb]), *cells, *(boundaries[self._nb :])]
+        self._domain = [*(boundaries[: self._nb]), *
+                        cells, *(boundaries[self._nb:])]
         self._components = components
 
     @classmethod
     def from_size(
         cls,
         nx: int,
         ng: int,
@@ -115,58 +116,59 @@
         Returns
         -------
         int
             The number of ghost cells on each side of the domain.
         """
         return self._nb
 
-    def cells(self):
+    def cells(self, interior=False):
         """
         Get the cells in the domain.
 
         Returns
         -------
         list of Cell
             The cells in the domain.
         """
-        return self._domain
+        return self._domain if not interior else self.interior()
 
     def boundaries(self):
         """
         Get the boundaries of the domain.
 
         Returns
         -------
         tuple of Boundary
             The left and right boundaries of the domain.
         """
-        return self._domain[: self._nb], self._domain[-self._nb :]
+        return self._domain[: self._nb], self._domain[-self._nb:]
 
     def interior(self):
         """
         Get the interior cells in the domain.
 
         Returns
         -------
         list of Cell
             The interior cells in the domain.
         """
-        return self._domain[self._nb : -self._nb]
+        return self._domain[self._nb: -self._nb]
 
     def set_interior(self, cells):
         """
         Set the interior cells in the domain.
 
         Parameters
         ----------
         cells : list of Cell
             The new interior cells in the domain.
         """
         self._nx = len(cells)
-        self._domain = [*self._domain[: self._nb], *cells, *self._domain[-self._nb :]]
+        self._domain = [*self._domain[: self._nb],
+                        *cells, *self._domain[-self._nb:]]
 
     def num_components(self):
         """
         Get the number of components/variables associated in the domain.
 
         Returns
         -------
@@ -204,36 +206,36 @@
         Returns
         -------
         str
             The name of the component.
         """
         return self._components[i]
 
-    def positions(self):
+    def positions(self, interior=False):
         """
         Get the positions of all cells in the domain.
 
         Returns
         -------
         list of float
             The positions of all cells in the domain.
         """
-        return [cell.x() for cell in self.cells()]
+        return [cell.x() for cell in self.cells(interior)]
 
-    def values(self):
+    def values(self, interior=False):
         """
         Get the values of all cells in the domain.
 
         Returns
         -------
         list of numpy.ndarray
             The values of all cells in the domain.
         """
         value_list = []
-        for cell in self.cells():
+        for cell in self.cells(interior):
             value_list.append(cell.values())
 
         return value_list
 
     def listify_interior(self, split, split_loc):
         """
         Get the values of all interior cells in the domain in a list.
@@ -247,15 +249,15 @@
 
         Returns
         -------
         numpy.ndarray
             The values of all interior cells in the domain in a list.
         """
 
-        interior_values = self.values()[self._nb : -self._nb]
+        interior_values = self.values()[self._nb: -self._nb]
 
         if not split:
             return np.array(interior_values).flatten()
         else:
             if split_loc is None:
                 raise SFDM("Split location must be specified in this case")
```

### Comparing `SplitFDM-0.1.1/splitfdm/initialize.py` & `SplitFDM-0.1.2/splitfdm/initialize.py`

 * *Files identical despite different names*

### Comparing `SplitFDM-0.1.1/splitfdm/refine.py` & `SplitFDM-0.1.2/splitfdm/refine.py`

 * *Files identical despite different names*

### Comparing `SplitFDM-0.1.1/splitfdm/simulation.py` & `SplitFDM-0.1.2/splitfdm/simulation.py`

 * *Files identical despite different names*

### Comparing `SplitFDM-0.1.1/splitfdm/system.py` & `SplitFDM-0.1.2/splitfdm/system.py`

 * *Files identical despite different names*

