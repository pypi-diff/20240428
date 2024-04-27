# Comparing `tmp/python-iArt-1.0.3.tar.gz` & `tmp/python-iArt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iArt-1.0.3.tar", last modified: Wed Apr 17 18:40:54 2024, max compression
+gzip compressed data, was "python-iArt-1.0.4.tar", last modified: Sat Apr 27 21:59:34 2024, max compression
```

## Comparing `python-iArt-1.0.3.tar` & `python-iArt-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-17 18:40:54.025616 python-iArt-1.0.3/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-17 18:40:54.025261 python-iArt-1.0.3/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.0.3/README.md
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-17 18:40:54.022004 python-iArt-1.0.3/iArt/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.0.3/iArt/__init__.py
--rw-r--r--   0 jiaweizhang   (501) staff       (20)    18815 2024-04-17 16:14:17.000000 python-iArt-1.0.3/iArt/iArt.py
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-17 18:40:54.024476 python-iArt-1.0.3/python_iArt.egg-info/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-17 18:40:53.000000 python-iArt-1.0.3/python_iArt.egg-info/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-17 18:40:53.000000 python-iArt-1.0.3/python_iArt.egg-info/SOURCES.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-17 18:40:53.000000 python-iArt-1.0.3/python_iArt.egg-info/dependency_links.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-17 18:40:53.000000 python-iArt-1.0.3/python_iArt.egg-info/requires.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-17 18:40:53.000000 python-iArt-1.0.3/python_iArt.egg-info/top_level.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-17 18:40:54.025761 python-iArt-1.0.3/setup.cfg
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-17 18:40:52.000000 python-iArt-1.0.3/setup.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-27 21:59:34.750051 python-iArt-1.0.4/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-27 21:59:34.749695 python-iArt-1.0.4/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.0.4/README.md
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-27 21:59:34.746838 python-iArt-1.0.4/iArt/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.0.4/iArt/__init__.py
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)    18837 2024-04-27 21:57:37.000000 python-iArt-1.0.4/iArt/iArt.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-27 21:59:34.749070 python-iArt-1.0.4/python_iArt.egg-info/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/requires.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/top_level.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-27 21:59:34.750201 python-iArt-1.0.4/setup.cfg
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-27 21:58:54.000000 python-iArt-1.0.4/setup.py
```

### Comparing `python-iArt-1.0.3/PKG-INFO` & `python-iArt-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.0.3
+Version: 1.0.4
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.0.3/README.md` & `python-iArt-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-iArt-1.0.3/iArt/iArt.py` & `python-iArt-1.0.4/iArt/iArt.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     Z_sim_templates = []
     unique_strata = np.unique(S)
     for stratum in unique_strata:
         strata_indices = np.where(S == stratum)[0]
         strata_Z = Z_sorted[strata_indices]
         p = np.mean(strata_Z)
         strata_size = len(strata_indices)
-        Z_sim_template = [0.0] * int(strata_size * (1 - p)) + [1.0] * int(strata_size * p)
+        Z_sim_template = [0.0] * int(strata_size * (1 - p)) + [1.0] * (strata_size -int(strata_size * (1 - p)) )
         Z_sim_templates.append(Z_sim_template)
     return Z_sim_templates
 
 def getZsim(Z_sim_templates):
     """ 
     Shuffle each Z_sim template and concatenate them into a single permutated Z_sim array 
     """
```

### Comparing `python-iArt-1.0.3/python_iArt.egg-info/PKG-INFO` & `python-iArt-1.0.4/python_iArt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.0.3
+Version: 1.0.4
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.0.3/setup.py` & `python-iArt-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python-iArt",
-    version="1.0.3",
+    version="1.0.4",
     author="Siyu Heng, Jiawei Zhang, and Yang Feng",
     author_email="siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu",
     description="iArt: A Generalized Framework for Imputation-Assisted Randomization Tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py",
     packages=find_packages(),
```

