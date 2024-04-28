# Comparing `tmp/SplitFVM-0.1.tar.gz` & `tmp/SplitFVM-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplitFVM-0.1.tar", last modified: Mon Jan  2 06:18:03 2023, max compression
+gzip compressed data, was "SplitFVM-0.1.1.tar", last modified: Sun Apr 28 06:36:18 2024, max compression
```

## Comparing `SplitFVM-0.1.tar` & `SplitFVM-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-02 06:18:03.813167 SplitFVM-0.1/
--rw-r--r--   0 apple      (501) staff       (20)     1076 2023-01-02 06:11:27.000000 SplitFVM-0.1/LICENSE.md
--rw-r--r--   0 apple      (501) staff       (20)     2803 2023-01-02 06:18:03.812402 SplitFVM-0.1/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     2099 2023-01-02 06:15:48.000000 SplitFVM-0.1/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-02 06:18:03.792470 SplitFVM-0.1/SplitFVM.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2803 2023-01-02 06:18:03.000000 SplitFVM-0.1/SplitFVM.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      471 2023-01-02 06:18:03.000000 SplitFVM-0.1/SplitFVM.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-01-02 06:18:03.000000 SplitFVM-0.1/SplitFVM.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-01-02 06:05:28.000000 SplitFVM-0.1/SplitFVM.egg-info/not-zip-safe
--rw-r--r--   0 apple      (501) staff       (20)       42 2023-01-02 06:18:03.000000 SplitFVM-0.1/SplitFVM.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        9 2023-01-02 06:18:03.000000 SplitFVM-0.1/SplitFVM.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-01-02 06:18:03.813392 SplitFVM-0.1/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     1042 2023-01-02 06:17:25.000000 SplitFVM-0.1/setup.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-02 06:18:03.809844 SplitFVM-0.1/splitfvm/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-25 19:48:42.000000 SplitFVM-0.1/splitfvm/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2172 2023-01-02 00:44:40.000000 SplitFVM-0.1/splitfvm/bc.py
--rw-r--r--   0 apple      (501) staff       (20)     3330 2023-01-02 00:48:21.000000 SplitFVM-0.1/splitfvm/boundary.py
--rw-r--r--   0 apple      (501) staff       (20)     3228 2023-01-02 00:52:58.000000 SplitFVM-0.1/splitfvm/cell.py
--rw-r--r--   0 apple      (501) staff       (20)     7358 2023-01-02 01:12:42.000000 SplitFVM-0.1/splitfvm/domain.py
--rw-r--r--   0 apple      (501) staff       (20)       87 2023-01-02 01:13:03.000000 SplitFVM-0.1/splitfvm/error.py
--rw-r--r--   0 apple      (501) staff       (20)     1947 2023-01-02 01:14:27.000000 SplitFVM-0.1/splitfvm/flux.py
--rw-r--r--   0 apple      (501) staff       (20)     1563 2023-01-02 01:15:43.000000 SplitFVM-0.1/splitfvm/initialize.py
--rw-r--r--   0 apple      (501) staff       (20)      348 2023-01-02 01:16:53.000000 SplitFVM-0.1/splitfvm/model.py
--rw-r--r--   0 apple      (501) staff       (20)    10465 2023-01-02 01:26:42.000000 SplitFVM-0.1/splitfvm/refine.py
--rw-r--r--   0 apple      (501) staff       (20)     8731 2023-01-02 05:04:42.000000 SplitFVM-0.1/splitfvm/simulation.py
--rw-r--r--   0 apple      (501) staff       (20)     1582 2023-01-02 01:31:21.000000 SplitFVM-0.1/splitfvm/system.py
--rw-r--r--   0 apple      (501) staff       (20)      332 2023-01-02 01:39:54.000000 SplitFVM-0.1/splitfvm/visualize.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-28 06:36:18.097717 SplitFVM-0.1.1/
+-rw-r--r--   0 apple      (501) staff       (20)     3569 2024-04-28 06:36:18.097012 SplitFVM-0.1.1/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     2306 2024-04-28 06:34:04.000000 SplitFVM-0.1.1/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-28 06:36:18.073665 SplitFVM-0.1.1/SplitFVM.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     3569 2024-04-28 06:36:17.000000 SplitFVM-0.1.1/SplitFVM.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      482 2024-04-28 06:36:18.000000 SplitFVM-0.1.1/SplitFVM.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-04-28 06:36:17.000000 SplitFVM-0.1.1/SplitFVM.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-04-28 06:36:17.000000 SplitFVM-0.1.1/SplitFVM.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)       42 2024-04-28 06:36:17.000000 SplitFVM-0.1.1/SplitFVM.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        9 2024-04-28 06:36:17.000000 SplitFVM-0.1.1/SplitFVM.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2024-04-28 06:36:18.099516 SplitFVM-0.1.1/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     1044 2024-04-28 06:35:35.000000 SplitFVM-0.1.1/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-28 06:36:18.094002 SplitFVM-0.1.1/splitfvm/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     6289 2024-04-28 06:34:04.000000 SplitFVM-0.1.1/splitfvm/bc.py
+-rw-r--r--   0 apple      (501) staff       (20)     3300 2024-04-28 06:34:04.000000 SplitFVM-0.1.1/splitfvm/boundary.py
+-rw-r--r--   0 apple      (501) staff       (20)     3228 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/cell.py
+-rw-r--r--   0 apple      (501) staff       (20)      124 2024-04-28 06:34:04.000000 SplitFVM-0.1.1/splitfvm/constants.py
+-rw-r--r--   0 apple      (501) staff       (20)     7503 2024-04-28 06:34:04.000000 SplitFVM-0.1.1/splitfvm/domain.py
+-rw-r--r--   0 apple      (501) staff       (20)       87 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/error.py
+-rw-r--r--   0 apple      (501) staff       (20)     1947 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/flux.py
+-rw-r--r--   0 apple      (501) staff       (20)     1563 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/initialize.py
+-rw-r--r--   0 apple      (501) staff       (20)      348 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/model.py
+-rw-r--r--   0 apple      (501) staff       (20)    10465 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/refine.py
+-rw-r--r--   0 apple      (501) staff       (20)     8731 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/simulation.py
+-rw-r--r--   0 apple      (501) staff       (20)     1582 2024-04-28 05:58:18.000000 SplitFVM-0.1.1/splitfvm/system.py
+-rw-r--r--   0 apple      (501) staff       (20)      364 2024-04-28 06:34:04.000000 SplitFVM-0.1.1/splitfvm/visualize.py
```

### Comparing `SplitFVM-0.1/PKG-INFO` & `SplitFVM-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 Metadata-Version: 2.1
 Name: SplitFVM
-Version: 0.1
+Version: 0.1.1
 Summary: 1D Finite-Volume Split Newton Solver
 Home-page: https://github.com/gpavanb1/SplitFVM
 Author: gpavanb1
 Author-email: gpavanb@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/gpavanb1/SplitFVM/issues
 Project-URL: Source, https://github.com/gpavanb1/SplitFVM/
+Description: # SplitFVM
+        
+        [![Downloads](https://pepy.tech/badge/splitfvm)](https://pepy.tech/project/splitfvm)
+        
+        ![img](https://github.com/gpavanb1/SplitFVM/blob/main/assets/logo.jpg)
+        
+        1D [Finite-Volume](https://en.wikipedia.org/wiki/Finite_volume_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
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
+        pip install splitfvm
+        ```
+        
+        There is an [examples](https://github.com/gpavanb1/SplitFVM/examples) folder that contains a test model - [Advection-Diffusion](https://en.wikipedia.org/wiki/Convection%E2%80%93diffusion_equation)
+        
+        You can define your own equations by simply creating a derived class from `Model` and adding to the `_equations` using existing or custom equations!
+        
+        A basic driver program is as follows
+        ```
+        # Define the problem
+        m = AdvectionDiffusion(c=0.2, nu=0.001)
+        
+        # Define the domain and variables
+        # ng stands for ghost cell count
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
+        Do visit its [Finite-Difference](https://github.com/gpavanb1/SplitFDM) cousin
+        
+        Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture
 Keywords: amr newton python finite-volume armijo optimization pseudotransient splitting
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# SplitFVM
-
-[![Downloads](https://pepy.tech/badge/splitfvm)](https://pepy.tech/project/splitfvm)
-
-![img](https://github.com/gpavanb1/SplitFVM/blob/main/assets/logo.png)
-
-1D [Finite-Volume](https://en.wikipedia.org/wiki/Finite_volume_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
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
-pip install splitfvm
-```
-
-There is an [examples](https://github.com/gpavanb1/SplitFVM/examples) folder that contains a test model - [Advection-Diffusion](https://en.wikipedia.org/wiki/Convection%E2%80%93diffusion_equation)
-
-You can define your own equations by simply creating a derived class from `Model` and adding to the `_equations` using existing or custom equations!
-
-A basic driver program is as follows
-```
-# Define the problem
-m = AdvectionDiffusion(c=0.2, nu=0.001)
-
-# Define the domain and variables
-# ng stands for ghost cell count
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
-Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture
```

### Comparing `SplitFVM-0.1/README.md` & `SplitFVM-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SplitFVM
 
 [![Downloads](https://pepy.tech/badge/splitfvm)](https://pepy.tech/project/splitfvm)
 
-![img](https://github.com/gpavanb1/SplitFVM/blob/main/assets/logo.png)
+![img](https://github.com/gpavanb1/SplitFVM/blob/main/assets/logo.jpg)
 
 1D [Finite-Volume](https://en.wikipedia.org/wiki/Finite_volume_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
 
 ## What does 'split' mean?
 
 The system is divided into two and for ease of communication, let's refer to first set of variables as "outer" and the second as "inner".
 
@@ -34,15 +34,24 @@
 
 # Define the domain and variables
 # ng stands for ghost cell count
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
@@ -52,8 +61,10 @@
 ## Whom to contact?
 
 Please direct your queries to [gpavanb1](http://github.com/gpavanb1)
 for any questions.
 
 ## Acknowledgements
 
+Do visit its [Finite-Difference](https://github.com/gpavanb1/SplitFDM) cousin
+
 Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture
```

### Comparing `SplitFVM-0.1/SplitFVM.egg-info/PKG-INFO` & `SplitFVM-0.1.1/SplitFVM.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 Metadata-Version: 2.1
 Name: SplitFVM
-Version: 0.1
+Version: 0.1.1
 Summary: 1D Finite-Volume Split Newton Solver
 Home-page: https://github.com/gpavanb1/SplitFVM
 Author: gpavanb1
 Author-email: gpavanb@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/gpavanb1/SplitFVM/issues
 Project-URL: Source, https://github.com/gpavanb1/SplitFVM/
+Description: # SplitFVM
+        
+        [![Downloads](https://pepy.tech/badge/splitfvm)](https://pepy.tech/project/splitfvm)
+        
+        ![img](https://github.com/gpavanb1/SplitFVM/blob/main/assets/logo.jpg)
+        
+        1D [Finite-Volume](https://en.wikipedia.org/wiki/Finite_volume_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
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
+        pip install splitfvm
+        ```
+        
+        There is an [examples](https://github.com/gpavanb1/SplitFVM/examples) folder that contains a test model - [Advection-Diffusion](https://en.wikipedia.org/wiki/Convection%E2%80%93diffusion_equation)
+        
+        You can define your own equations by simply creating a derived class from `Model` and adding to the `_equations` using existing or custom equations!
+        
+        A basic driver program is as follows
+        ```
+        # Define the problem
+        m = AdvectionDiffusion(c=0.2, nu=0.001)
+        
+        # Define the domain and variables
+        # ng stands for ghost cell count
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
+        Do visit its [Finite-Difference](https://github.com/gpavanb1/SplitFDM) cousin
+        
+        Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture
 Keywords: amr newton python finite-volume armijo optimization pseudotransient splitting
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# SplitFVM
-
-[![Downloads](https://pepy.tech/badge/splitfvm)](https://pepy.tech/project/splitfvm)
-
-![img](https://github.com/gpavanb1/SplitFVM/blob/main/assets/logo.png)
-
-1D [Finite-Volume](https://en.wikipedia.org/wiki/Finite_volume_method) with [adaptive mesh refinement](https://en.wikipedia.org/wiki/Adaptive_mesh_refinement) and steady-state solver using Newton and [Split-Newton](https://github.com/gpavanb1/SplitNewton) approach
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
-pip install splitfvm
-```
-
-There is an [examples](https://github.com/gpavanb1/SplitFVM/examples) folder that contains a test model - [Advection-Diffusion](https://en.wikipedia.org/wiki/Convection%E2%80%93diffusion_equation)
-
-You can define your own equations by simply creating a derived class from `Model` and adding to the `_equations` using existing or custom equations!
-
-A basic driver program is as follows
-```
-# Define the problem
-m = AdvectionDiffusion(c=0.2, nu=0.001)
-
-# Define the domain and variables
-# ng stands for ghost cell count
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
-Special thanks to [Cantera](https://github.com/Cantera/cantera) and [WENO-Scalar](https://github.com/comp-physics/WENO-scalar) for serving as an inspiration for code architecture
```

### Comparing `SplitFVM-0.1/setup.py` & `SplitFVM-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="SplitFVM",
-    version="0.1",
+    version="0.1.1",
     description="1D Finite-Volume Split Newton Solver",
     url="https://github.com/gpavanb1/SplitFVM",
     author="gpavanb1",
     author_email="gpavanb@gmail.com",
     license="MIT",
     packages=["splitfvm"],
     install_requires=["numpy", "numdifftools", "matplotlib", "splitnewton"],
```

### Comparing `SplitFVM-0.1/splitfvm/boundary.py` & `SplitFVM-0.1.1/splitfvm/boundary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
-from enum import Enum
+from .constants import btype
 from .error import SFVM
 
-btype = Enum("btype", "LEFT RIGHT")
-
 
 class Boundary:
     """
     A class representing a boundary cell in a domain.
 
     Parameters
     ----------
```

### Comparing `SplitFVM-0.1/splitfvm/cell.py` & `SplitFVM-0.1.1/splitfvm/cell.py`

 * *Files identical despite different names*

### Comparing `SplitFVM-0.1/splitfvm/domain.py` & `SplitFVM-0.1.1/splitfvm/domain.py`

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
                 raise SFVM("Split location must be specified in this case")
```

### Comparing `SplitFVM-0.1/splitfvm/flux.py` & `SplitFVM-0.1.1/splitfvm/flux.py`

 * *Files identical despite different names*

### Comparing `SplitFVM-0.1/splitfvm/initialize.py` & `SplitFVM-0.1.1/splitfvm/initialize.py`

 * *Files identical despite different names*

### Comparing `SplitFVM-0.1/splitfvm/refine.py` & `SplitFVM-0.1.1/splitfvm/refine.py`

 * *Files identical despite different names*

### Comparing `SplitFVM-0.1/splitfvm/simulation.py` & `SplitFVM-0.1.1/splitfvm/simulation.py`

 * *Files identical despite different names*

### Comparing `SplitFVM-0.1/splitfvm/system.py` & `SplitFVM-0.1.1/splitfvm/system.py`

 * *Files identical despite different names*

