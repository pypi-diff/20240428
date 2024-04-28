# Comparing `tmp/sema_toolchain-0.0.3.tar.gz` & `tmp/sema_toolchain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema_toolchain-0.0.3.tar", last modified: Fri Apr 26 12:53:02 2024, max compression
+gzip compressed data, was "sema_toolchain-0.0.4.tar", last modified: Sun Apr 28 10:22:50 2024, max compression
```

## Comparing `sema_toolchain-0.0.3.tar` & `sema_toolchain-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-26 12:53:02.703261 sema_toolchain-0.0.3/
--rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.3/LICENSE
--rw-r--r--   0 manon     (1000) manon     (1000)    17888 2024-04-26 12:53:02.703261 sema_toolchain-0.0.3/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)    14786 2024-04-16 21:19:17.000000 sema_toolchain-0.0.3/README.md
--rw-rw-r--   0 manon     (1000) manon     (1000)     1445 2024-04-26 12:52:31.000000 sema_toolchain-0.0.3/pyproject.toml
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-26 12:53:02.703261 sema_toolchain-0.0.3/sema_toolchain.egg-info/
--rw-r--r--   0 manon     (1000) manon     (1000)    17888 2024-04-26 12:53:02.000000 sema_toolchain-0.0.3/sema_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-04-26 12:53:02.000000 sema_toolchain-0.0.3/sema_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-04-26 12:53:02.000000 sema_toolchain-0.0.3/sema_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)      459 2024-04-26 12:53:02.000000 sema_toolchain-0.0.3/sema_toolchain.egg-info/requires.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-04-26 12:53:02.000000 sema_toolchain-0.0.3/sema_toolchain.egg-info/top_level.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-04-26 12:53:02.703261 sema_toolchain-0.0.3/setup.cfg
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-28 10:22:50.963413 sema_toolchain-0.0.4/
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.4/LICENSE
+-rw-r--r--   0 manon     (1000) manon     (1000)    17998 2024-04-28 10:22:50.963413 sema_toolchain-0.0.4/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)    14786 2024-04-16 21:19:17.000000 sema_toolchain-0.0.4/README.md
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1523 2024-04-28 10:22:42.000000 sema_toolchain-0.0.4/pyproject.toml
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-28 10:22:50.963413 sema_toolchain-0.0.4/sema_toolchain.egg-info/
+-rw-r--r--   0 manon     (1000) manon     (1000)    17998 2024-04-28 10:22:50.000000 sema_toolchain-0.0.4/sema_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-04-28 10:22:50.000000 sema_toolchain-0.0.4/sema_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-04-28 10:22:50.000000 sema_toolchain-0.0.4/sema_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)      509 2024-04-28 10:22:50.000000 sema_toolchain-0.0.4/sema_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-04-28 10:22:50.000000 sema_toolchain-0.0.4/sema_toolchain.egg-info/top_level.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-04-28 10:22:50.963413 sema_toolchain-0.0.4/setup.cfg
```

### Comparing `sema_toolchain-0.0.3/LICENSE` & `sema_toolchain-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.3/PKG-INFO` & `sema_toolchain-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -75,14 +75,18 @@
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: progressbar
 Requires-Dist: gensim
 Requires-Dist: grakel
 Requires-Dist: numpy
 Requires-Dist: torch
+Requires-Dist: flask_session
+Requires-Dist: django
+Requires-Dist: Flask-Cors
+Requires-Dist: npf-web-extension
 
 # :skull_and_crossbones: SEMA :skull_and_crossbones: - ToolChain using Symbolic Execution for Malware Analysis. 
 
 ```
   ██████ ▓█████  ███▄ ▄███▓ ▄▄▄      
 ▒██    ▒ ▓█   ▀ ▓██▒▀█▀ ██▒▒████▄    
 ░ ▓██▄   ▒███   ▓██    ▓██░▒██  ▀█▄
```

### Comparing `sema_toolchain-0.0.3/README.md` & `sema_toolchain-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.3/pyproject.toml` & `sema_toolchain-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["sema_scdg", "sema_web_app", "sema_classifier"]
 
 [project]
 name = "sema_toolchain"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Manon-Oreins", email="manon.oreins@gmail.com" },
 ]
 description = "Python symbolic execution package"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -59,14 +59,18 @@
     "dill",
     "seaborn",
     "scikit-learn",
     "progressbar",
     "gensim",
     "grakel",
     "numpy",
-    "torch"
+    "torch",
+    "flask_session",
+    "django",
+    "Flask-Cors",
+    "npf-web-extension"
 ]
 
 
 
 [project.urls]
 Homepage = "https://github.com/Manon-Oreins/SEMA-ToolChain/tree/refactor_simproc"
```

### Comparing `sema_toolchain-0.0.3/sema_toolchain.egg-info/PKG-INFO` & `sema_toolchain-0.0.4/sema_toolchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -75,14 +75,18 @@
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: progressbar
 Requires-Dist: gensim
 Requires-Dist: grakel
 Requires-Dist: numpy
 Requires-Dist: torch
+Requires-Dist: flask_session
+Requires-Dist: django
+Requires-Dist: Flask-Cors
+Requires-Dist: npf-web-extension
 
 # :skull_and_crossbones: SEMA :skull_and_crossbones: - ToolChain using Symbolic Execution for Malware Analysis. 
 
 ```
   ██████ ▓█████  ███▄ ▄███▓ ▄▄▄      
 ▒██    ▒ ▓█   ▀ ▓██▒▀█▀ ██▒▒████▄    
 ░ ▓██▄   ▒███   ▓██    ▓██░▒██  ▀█▄
```

