# Comparing `tmp/jz3-0.1.4.tar.gz` & `tmp/jz3-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jz3-0.1.4.tar", last modified: Sun Apr 28 05:14:58 2024, max compression
+gzip compressed data, was "jz3-0.1.6.tar", last modified: Sun Apr 28 05:35:06 2024, max compression
```

## Comparing `jz3-0.1.4.tar` & `jz3-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118718 jz3-0.1.4/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.4/LICENSE-Z3.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.4/LICENSE.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 05:14:58.118604 jz3-0.1.4/PKG-INFO
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.4/README.md
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.113770 jz3-0.1.4/jz3/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       55 2024-04-26 16:59:15.000000 jz3-0.1.4/jz3/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.114794 jz3-0.1.4/jz3/analysis/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.4/jz3/analysis/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.115009 jz3-0.1.4/jz3/analysis/archive/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.4/jz3/analysis/archive/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.4/jz3/analysis/archive/export_to_excel.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.116199 jz3-0.1.4/jz3/analysis/scripts/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.4/jz3/analysis/scripts/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.4/jz3/analysis/scripts/compare_whole_problems.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.4/jz3/analysis/scripts/plot_comparison.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.116537 jz3-0.1.4/jz3/solvers/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.4/jz3/solvers/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.117484 jz3-0.1.4/jz3/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118150 jz3-0.1.4/jz3/src/SMTs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.4/jz3/src/SMTs/SMTs.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.4/jz3/src/SMTs/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118255 jz3-0.1.4/jz3/src/Sudokus/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.4/jz3/src/Sudokus/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.4/jz3/src/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.4/jz3/src/clean_up.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3542 2024-04-28 05:00:33.000000 jz3-0.1.4/jz3/src/run_solvers.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.4/jz3/src/z3_quick_start_guide.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    10939 2024-04-26 02:43:34.000000 jz3-0.1.4/jz3/src/z3_wrapper.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118451 jz3-0.1.4/jz3/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.4/jz3/tests/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.4/jz3/tests/test_solver.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.114665 jz3-0.1.4/jz3.egg-info/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/PKG-INFO
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      675 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/SOURCES.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/dependency_links.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/requires.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/top_level.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-28 05:14:58.118780 jz3-0.1.4/setup.cfg
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      839 2024-04-28 05:14:32.000000 jz3-0.1.4/setup.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.489959 jz3-0.1.6/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.6/LICENSE-Z3.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.6/LICENSE.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:30:26.000000 jz3-0.1.6/MANIFEST.in
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 05:35:06.489761 jz3-0.1.6/PKG-INFO
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.6/README.md
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.450478 jz3-0.1.6/jz3/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       55 2024-04-26 16:59:15.000000 jz3-0.1.6/jz3/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.451601 jz3-0.1.6/jz3/analysis/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.6/jz3/analysis/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.451817 jz3-0.1.6/jz3/analysis/archive/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.6/jz3/analysis/archive/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.6/jz3/analysis/archive/export_to_excel.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.452730 jz3-0.1.6/jz3/analysis/scripts/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.6/jz3/analysis/scripts/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.6/jz3/analysis/scripts/compare_whole_problems.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.6/jz3/analysis/scripts/plot_comparison.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.453019 jz3-0.1.6/jz3/solvers/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.6/jz3/solvers/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20) 20962472 2024-04-18 02:04:14.000000 jz3-0.1.6/jz3/solvers/cvc5-macOS-arm64
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.474392 jz3-0.1.6/jz3/src/
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.489123 jz3-0.1.6/jz3/src/SMTs/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.6/jz3/src/SMTs/SMTs.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.6/jz3/src/SMTs/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.489272 jz3-0.1.6/jz3/src/Sudokus/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.6/jz3/src/Sudokus/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.6/jz3/src/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.6/jz3/src/clean_up.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3542 2024-04-28 05:00:33.000000 jz3-0.1.6/jz3/src/run_solvers.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.6/jz3/src/z3_quick_start_guide.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    10939 2024-04-26 02:43:34.000000 jz3-0.1.6/jz3/src/z3_wrapper.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.489530 jz3-0.1.6/jz3/tests/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.6/jz3/tests/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.6/jz3/tests/test_solver.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:35:06.451465 jz3-0.1.6/jz3.egg-info/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 05:35:06.000000 jz3-0.1.6/jz3.egg-info/PKG-INFO
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      716 2024-04-28 05:35:06.000000 jz3-0.1.6/jz3.egg-info/SOURCES.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-28 05:35:06.000000 jz3-0.1.6/jz3.egg-info/dependency_links.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-28 05:35:06.000000 jz3-0.1.6/jz3.egg-info/requires.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-28 05:35:06.000000 jz3-0.1.6/jz3.egg-info/top_level.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-28 05:35:06.490039 jz3-0.1.6/setup.cfg
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      894 2024-04-28 05:35:05.000000 jz3-0.1.6/setup.py
```

### Comparing `jz3-0.1.4/LICENSE-Z3.txt` & `jz3-0.1.6/LICENSE-Z3.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/LICENSE.txt` & `jz3-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/PKG-INFO` & `jz3-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.4
+Version: 0.1.6
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jz3-0.1.4/README.md` & `jz3-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3/analysis/archive/export_to_excel.py` & `jz3-0.1.6/jz3/analysis/archive/export_to_excel.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3/analysis/scripts/compare_whole_problems.py` & `jz3-0.1.6/jz3/analysis/scripts/compare_whole_problems.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3/analysis/scripts/plot_comparison.py` & `jz3-0.1.6/jz3/analysis/scripts/plot_comparison.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3/src/SMTs/SMTs.py` & `jz3-0.1.6/jz3/src/SMTs/SMTs.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3/src/run_solvers.py` & `jz3-0.1.6/jz3/src/run_solvers.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3/src/z3_wrapper.py` & `jz3-0.1.6/jz3/src/z3_wrapper.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.4/jz3.egg-info/PKG-INFO` & `jz3-0.1.6/jz3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.4
+Version: 0.1.6
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jz3-0.1.4/jz3.egg-info/SOURCES.txt` & `jz3-0.1.6/jz3.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE-Z3.txt
 LICENSE.txt
+MANIFEST.in
 README.md
 setup.py
 jz3/__init__.py
 jz3.egg-info/PKG-INFO
 jz3.egg-info/SOURCES.txt
 jz3.egg-info/dependency_links.txt
 jz3.egg-info/requires.txt
@@ -11,14 +12,15 @@
 jz3/analysis/__init__.py
 jz3/analysis/archive/__init__.py
 jz3/analysis/archive/export_to_excel.py
 jz3/analysis/scripts/__init__.py
 jz3/analysis/scripts/compare_whole_problems.py
 jz3/analysis/scripts/plot_comparison.py
 jz3/solvers/__init__.py
+jz3/solvers/cvc5-macOS-arm64
 jz3/src/__init__.py
 jz3/src/clean_up.py
 jz3/src/run_solvers.py
 jz3/src/z3_quick_start_guide.py
 jz3/src/z3_wrapper.py
 jz3/src/SMTs/SMTs.py
 jz3/src/SMTs/__init__.py
```

### Comparing `jz3-0.1.4/setup.py` & `jz3-0.1.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='jz3',
-    version='0.1.4',
+    version='0.1.6',
     packages=find_packages(),
     description='A simple wrapper for Z3 solver',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Sebastiaan Joosten, Zheng Robert Jia',
     author_email='jia00129@umn.edu',
     url='https://github.com/Robert-Jia00129/jz3',
     license='MIT',
     install_requires=[
         'z3-solver',
         'matplotlib',
     ],
+    package_data={
+        'jz3': ['solvers/*']
+    },
     python_requires='>3.11',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

