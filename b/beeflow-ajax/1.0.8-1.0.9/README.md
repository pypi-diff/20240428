# Comparing `tmp/beeflow-ajax-1.0.8.tar.gz` & `tmp/beeflow-ajax-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beeflow-ajax-1.0.8.tar", last modified: Fri Mar 29 15:59:34 2024, max compression
+gzip compressed data, was "beeflow-ajax-1.0.9.tar", last modified: Sat Apr  6 15:45:58 2024, max compression
```

## Comparing `beeflow-ajax-1.0.8.tar` & `beeflow-ajax-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-03-29 15:59:34.056448 beeflow-ajax-1.0.8/
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       66 2024-03-12 08:19:49.000000 beeflow-ajax-1.0.8/CHANGELOG.md
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     1036 2024-03-12 13:46:56.000000 beeflow-ajax-1.0.8/LICENCE.md
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     1036 2024-03-12 13:46:56.000000 beeflow-ajax-1.0.8/LICENSE
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       55 2024-03-12 08:19:49.000000 beeflow-ajax-1.0.8/MANIFEST.in
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     4567 2024-03-29 15:59:34.055777 beeflow-ajax-1.0.8/PKG-INFO
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     4037 2024-03-14 11:12:33.000000 beeflow-ajax-1.0.8/README.md
-drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-03-29 15:59:34.029869 beeflow-ajax-1.0.8/beeflow_ajax/
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       96 2024-03-11 23:00:29.000000 beeflow-ajax-1.0.8/beeflow_ajax/__init__.py
-drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-03-29 15:59:34.046187 beeflow-ajax-1.0.8/beeflow_ajax/lib/
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      312 2024-03-11 23:21:47.000000 beeflow-ajax-1.0.8/beeflow_ajax/lib/__init__.py
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      426 2024-03-11 23:00:29.000000 beeflow-ajax-1.0.8/beeflow_ajax/lib/ajax_request.py
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     9019 2024-03-29 15:56:51.000000 beeflow-ajax-1.0.8/beeflow_ajax/lib/ajax_response.py
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      832 2024-03-12 15:47:28.000000 beeflow-ajax-1.0.8/beeflow_ajax/lib/websocket_response.py
-drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-03-29 15:59:34.054405 beeflow-ajax-1.0.8/beeflow_ajax/tests/
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       96 2024-03-12 08:27:47.000000 beeflow-ajax-1.0.8/beeflow_ajax/tests/__init__.py
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     7783 2024-03-12 08:53:48.000000 beeflow-ajax-1.0.8/beeflow_ajax/tests/test_ajax_response.py
-drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-03-29 15:59:34.055137 beeflow-ajax-1.0.8/beeflow_ajax.egg-info/
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     4567 2024-03-29 15:59:34.000000 beeflow-ajax-1.0.8/beeflow_ajax.egg-info/PKG-INFO
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      453 2024-03-29 15:59:34.000000 beeflow-ajax-1.0.8/beeflow_ajax.egg-info/SOURCES.txt
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)        1 2024-03-29 15:59:34.000000 beeflow-ajax-1.0.8/beeflow_ajax.egg-info/dependency_links.txt
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       13 2024-03-29 15:59:34.000000 beeflow-ajax-1.0.8/beeflow_ajax.egg-info/top_level.txt
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      100 2024-03-12 08:31:22.000000 beeflow-ajax-1.0.8/pyproject.toml
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       38 2024-03-29 15:59:34.056546 beeflow-ajax-1.0.8/setup.cfg
--rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      848 2024-03-29 15:59:05.000000 beeflow-ajax-1.0.8/setup.py
+drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-04-06 15:45:58.372918 beeflow-ajax-1.0.9/
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     1876 2024-04-06 15:43:06.000000 beeflow-ajax-1.0.9/CHANGELOG.md
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     1036 2024-03-12 13:46:56.000000 beeflow-ajax-1.0.9/LICENCE.md
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     1036 2024-03-12 13:46:56.000000 beeflow-ajax-1.0.9/LICENSE
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       55 2024-03-12 08:19:49.000000 beeflow-ajax-1.0.9/MANIFEST.in
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     4567 2024-04-06 15:45:58.372346 beeflow-ajax-1.0.9/PKG-INFO
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     4037 2024-03-14 11:12:33.000000 beeflow-ajax-1.0.9/README.md
+drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-04-06 15:45:58.353086 beeflow-ajax-1.0.9/beeflow_ajax/
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       96 2024-03-11 23:00:29.000000 beeflow-ajax-1.0.9/beeflow_ajax/__init__.py
+drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-04-06 15:45:58.366757 beeflow-ajax-1.0.9/beeflow_ajax/lib/
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      312 2024-03-11 23:21:47.000000 beeflow-ajax-1.0.9/beeflow_ajax/lib/__init__.py
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      426 2024-03-11 23:00:29.000000 beeflow-ajax-1.0.9/beeflow_ajax/lib/ajax_request.py
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     9019 2024-03-29 15:56:51.000000 beeflow-ajax-1.0.9/beeflow_ajax/lib/ajax_response.py
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      832 2024-03-12 15:47:28.000000 beeflow-ajax-1.0.9/beeflow_ajax/lib/websocket_response.py
+drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-04-06 15:45:58.370875 beeflow-ajax-1.0.9/beeflow_ajax/tests/
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       96 2024-03-12 08:27:47.000000 beeflow-ajax-1.0.9/beeflow_ajax/tests/__init__.py
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     7783 2024-03-12 08:53:48.000000 beeflow-ajax-1.0.9/beeflow_ajax/tests/test_ajax_response.py
+drwxr-xr-x   0 rafalprzetakowski   (501) staff       (20)        0 2024-04-06 15:45:58.371646 beeflow-ajax-1.0.9/beeflow_ajax.egg-info/
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)     4567 2024-04-06 15:45:58.000000 beeflow-ajax-1.0.9/beeflow_ajax.egg-info/PKG-INFO
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      453 2024-04-06 15:45:58.000000 beeflow-ajax-1.0.9/beeflow_ajax.egg-info/SOURCES.txt
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)        1 2024-04-06 15:45:58.000000 beeflow-ajax-1.0.9/beeflow_ajax.egg-info/dependency_links.txt
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       13 2024-04-06 15:45:58.000000 beeflow-ajax-1.0.9/beeflow_ajax.egg-info/top_level.txt
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      100 2024-03-12 08:31:22.000000 beeflow-ajax-1.0.9/pyproject.toml
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)       38 2024-04-06 15:45:58.373007 beeflow-ajax-1.0.9/setup.cfg
+-rw-r--r--   0 rafalprzetakowski   (501) staff       (20)      848 2024-04-06 15:40:02.000000 beeflow-ajax-1.0.9/setup.py
```

### Comparing `beeflow-ajax-1.0.8/LICENCE.md` & `beeflow-ajax-1.0.9/LICENCE.md`

 * *Files identical despite different names*

### Comparing `beeflow-ajax-1.0.8/LICENSE` & `beeflow-ajax-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `beeflow-ajax-1.0.8/PKG-INFO` & `beeflow-ajax-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beeflow-ajax
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library to maintain ajax and websockets communication without writing complicated code in JS
 Home-page: https://github.com/beeflow/BeeflowAjaxPy
 Author: Rafal Przetakowski
 Author-email: office@beeflow.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `beeflow-ajax-1.0.8/README.md` & `beeflow-ajax-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `beeflow-ajax-1.0.8/beeflow_ajax/lib/ajax_response.py` & `beeflow-ajax-1.0.9/beeflow_ajax/lib/ajax_response.py`

 * *Files identical despite different names*

### Comparing `beeflow-ajax-1.0.8/beeflow_ajax/lib/websocket_response.py` & `beeflow-ajax-1.0.9/beeflow_ajax/lib/websocket_response.py`

 * *Files identical despite different names*

### Comparing `beeflow-ajax-1.0.8/beeflow_ajax/tests/test_ajax_response.py` & `beeflow-ajax-1.0.9/beeflow_ajax/tests/test_ajax_response.py`

 * *Files identical despite different names*

### Comparing `beeflow-ajax-1.0.8/beeflow_ajax.egg-info/PKG-INFO` & `beeflow-ajax-1.0.9/beeflow_ajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beeflow-ajax
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library to maintain ajax and websockets communication without writing complicated code in JS
 Home-page: https://github.com/beeflow/BeeflowAjaxPy
 Author: Rafal Przetakowski
 Author-email: office@beeflow.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `beeflow-ajax-1.0.8/setup.py` & `beeflow-ajax-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import setuptools
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="beeflow-ajax",
-    version="1.0.8",
+    version="1.0.9",
     author="Rafal Przetakowski",
     author_email="office@beeflow.co.uk",
     description="Library to maintain ajax and websockets communication without writing complicated code in JS",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/beeflow/BeeflowAjaxPy",
```

