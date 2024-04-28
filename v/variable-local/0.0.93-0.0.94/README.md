# Comparing `tmp/variable_local-0.0.93.tar.gz` & `tmp/variable_local-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.93.tar", last modified: Sat Apr 27 22:29:52 2024, max compression
+gzip compressed data, was "variable_local-0.0.94.tar", last modified: Sat Apr 27 23:35:35 2024, max compression
```

## Comparing `variable_local-0.0.93.tar` & `variable_local-0.0.94.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.604822 variable_local-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 22:29:52.604822 variable_local-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 22:29:28.000000 variable_local-0.0.93/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 22:29:28.000000 variable_local-0.0.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:29:52.604822 variable_local-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-27 22:29:28.000000 variable_local-0.0.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.600823 variable_local-0.0.93/variable_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.600823 variable_local-0.0.93/variable_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/variables_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.600823 variable_local-0.0.93/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:35.430294 variable_local-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 23:35:35.430294 variable_local-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 23:35:08.000000 variable_local-0.0.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 23:35:08.000000 variable_local-0.0.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 23:35:35.430294 variable_local-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-27 23:35:08.000000 variable_local-0.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:35.426294 variable_local-0.0.94/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:35.430294 variable_local-0.0.94/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:08.000000 variable_local-0.0.94/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-27 23:35:08.000000 variable_local-0.0.94/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-27 23:35:08.000000 variable_local-0.0.94/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 23:35:08.000000 variable_local-0.0.94/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-27 23:35:08.000000 variable_local-0.0.94/variable_local/src/variables_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:35.430294 variable_local-0.0.94/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 23:35:35.000000 variable_local-0.0.94/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-27 23:35:35.000000 variable_local-0.0.94/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:35:35.000000 variable_local-0.0.94/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-27 23:35:35.000000 variable_local-0.0.94/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 23:35:35.000000 variable_local-0.0.94/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.93/PKG-INFO` & `variable_local-0.0.94/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.93
+Version: 0.0.94
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `variable_local-0.0.93/README.md` & `variable_local-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.93/pyproject.toml` & `variable_local-0.0.94/pyproject.toml`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.93/setup.py` & `variable_local-0.0.94/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'variable-local'
 package_dir = PACKAGE_NAME.replace('-', '_')
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.93',  # https://pypi.org/project/variable-local
+    version='0.0.94',  # https://pypi.org/project/variable-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles variable Local/Remote Python",
     long_description="PyPI Package for Circles variable Local/Remote Python",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

### Comparing `variable_local-0.0.93/variable_local/src/constants.py` & `variable_local-0.0.94/variable_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.93/variable_local/src/template.py` & `variable_local-0.0.94/variable_local/src/template.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.93/variable_local/src/variables_local.py` & `variable_local-0.0.94/variable_local/src/variables_local.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.93/variable_local.egg-info/PKG-INFO` & `variable_local-0.0.94/variable_local.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.93
+Version: 0.0.94
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

