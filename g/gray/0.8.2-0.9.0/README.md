# Comparing `tmp/gray-0.8.2.tar.gz` & `tmp/gray-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gray-0.8.2.tar", last modified: Sat Apr 24 11:09:01 2021, max compression
+gzip compressed data, was "gray-0.9.0.tar", last modified: Tue May 11 09:26:15 2021, max compression
```

## Comparing `gray-0.8.2.tar` & `gray-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2021-04-24 11:09:01.464461 gray-0.8.2/
--rw-r--r--   0 apple      (501) staff       (20)      116 2020-12-12 14:47:00.000000 gray-0.8.2/AUTHORS.md
--rw-r--r--   0 apple      (501) staff       (20)      814 2020-12-12 14:47:00.000000 gray-0.8.2/HISTORY.md
--rw-r--r--   0 apple      (501) staff       (20)     1080 2020-12-12 14:47:00.000000 gray-0.8.2/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      126 2020-12-12 14:47:00.000000 gray-0.8.2/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)     8714 2021-04-24 11:09:01.464921 gray-0.8.2/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     5307 2021-04-03 14:03:32.000000 gray-0.8.2/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2021-04-24 11:09:01.446587 gray-0.8.2/gray/
--rw-r--r--   0 apple      (501) staff       (20)       87 2021-04-24 11:08:30.000000 gray-0.8.2/gray/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2021-04-24 11:09:01.459911 gray-0.8.2/gray/formatters/
--rw-r--r--   0 apple      (501) staff       (20)      742 2021-04-03 13:03:56.000000 gray-0.8.2/gray/formatters/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      596 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/add_trailing_comma.py
--rw-r--r--   0 apple      (501) staff       (20)      869 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/autoflake.py
--rw-r--r--   0 apple      (501) staff       (20)      261 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/base.py
--rw-r--r--   0 apple      (501) staff       (20)      355 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/composite.py
--rw-r--r--   0 apple      (501) staff       (20)     1551 2021-04-03 14:12:19.000000 gray-0.8.2/gray/formatters/fixit.py
--rw-r--r--   0 apple      (501) staff       (20)     1032 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/isort.py
--rw-r--r--   0 apple      (501) staff       (20)      731 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/pyupgrade.py
--rw-r--r--   0 apple      (501) staff       (20)      406 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/trim.py
--rw-r--r--   0 apple      (501) staff       (20)      480 2020-12-12 14:47:00.000000 gray-0.8.2/gray/formatters/unify.py
--rw-r--r--   0 apple      (501) staff       (20)     1600 2020-12-12 14:47:00.000000 gray-0.8.2/gray/hooks.py
--rw-r--r--   0 apple      (501) staff       (20)     4574 2021-04-03 13:57:45.000000 gray-0.8.2/gray/main.py
--rw-r--r--   0 apple      (501) staff       (20)     2823 2020-12-12 14:47:00.000000 gray-0.8.2/gray/processing.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2021-04-24 11:09:01.461485 gray-0.8.2/gray/utils/
--rw-r--r--   0 apple      (501) staff       (20)        0 2020-12-12 14:47:00.000000 gray-0.8.2/gray/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      580 2020-12-12 14:47:00.000000 gray-0.8.2/gray/utils/args.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2021-04-24 11:09:01.463433 gray-0.8.2/gray/vendors/
--rw-r--r--   0 apple      (501) staff       (20)        0 2020-12-12 14:47:00.000000 gray-0.8.2/gray/vendors/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5130 2020-12-12 14:47:00.000000 gray-0.8.2/gray/vendors/trim.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2021-04-24 11:09:01.450096 gray-0.8.2/gray.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     8714 2021-04-24 11:09:00.000000 gray-0.8.2/gray.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      705 2021-04-24 11:09:00.000000 gray-0.8.2/gray.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2021-04-24 11:09:00.000000 gray-0.8.2/gray.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       41 2021-04-24 11:09:00.000000 gray-0.8.2/gray.egg-info/entry_points.txt
--rw-r--r--   0 apple      (501) staff       (20)      212 2021-04-24 11:09:00.000000 gray-0.8.2/gray.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        5 2021-04-24 11:09:00.000000 gray-0.8.2/gray.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       59 2021-04-24 11:07:54.000000 gray-0.8.2/requirements.dev.txt
--rw-r--r--   0 apple      (501) staff       (20)      142 2021-04-24 11:07:54.000000 gray-0.8.2/requirements.txt
--rw-r--r--   0 apple      (501) staff       (20)       61 2021-04-24 11:09:01.466244 gray-0.8.2/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     1862 2021-04-24 11:08:38.000000 gray-0.8.2/setup.py
+drwxr-xr-x   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2021-05-11 09:26:15.624396 gray-0.9.0/
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      116 2020-04-05 17:06:56.000000 gray-0.9.0/AUTHORS.md
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      814 2020-11-16 07:57:40.000000 gray-0.9.0/HISTORY.md
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     1080 2020-04-05 08:32:21.000000 gray-0.9.0/LICENSE
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      126 2020-05-23 14:56:19.000000 gray-0.9.0/MANIFEST.in
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     8714 2021-05-11 09:26:15.624807 gray-0.9.0/PKG-INFO
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     5307 2021-05-11 08:46:48.000000 gray-0.9.0/README.md
+drwxr-xr-x   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2021-05-11 09:26:15.612782 gray-0.9.0/gray/
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)       87 2021-05-11 09:18:19.000000 gray-0.9.0/gray/__init__.py
+drwxr-xr-x   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2021-05-11 09:26:15.621877 gray-0.9.0/gray/formatters/
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      742 2021-05-11 08:46:48.000000 gray-0.9.0/gray/formatters/__init__.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      545 2021-05-11 09:08:31.000000 gray-0.9.0/gray/formatters/add_trailing_comma.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      869 2020-05-23 13:05:19.000000 gray-0.9.0/gray/formatters/autoflake.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      261 2020-04-12 19:47:13.000000 gray-0.9.0/gray/formatters/base.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      355 2020-04-05 12:31:53.000000 gray-0.9.0/gray/formatters/composite.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     1551 2021-05-11 08:46:48.000000 gray-0.9.0/gray/formatters/fixit.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     1032 2020-09-02 14:50:02.000000 gray-0.9.0/gray/formatters/isort.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      863 2021-05-11 09:14:09.000000 gray-0.9.0/gray/formatters/pyupgrade.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      406 2020-08-15 17:36:28.000000 gray-0.9.0/gray/formatters/trim.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      480 2020-04-26 12:18:49.000000 gray-0.9.0/gray/formatters/unify.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     1600 2020-04-27 09:54:23.000000 gray-0.9.0/gray/hooks.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     4854 2021-05-11 09:16:00.000000 gray-0.9.0/gray/main.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     2823 2020-04-27 13:40:19.000000 gray-0.9.0/gray/processing.py
+drwxr-xr-x   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2021-05-11 09:26:15.622914 gray-0.9.0/gray/utils/
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2020-04-05 16:24:24.000000 gray-0.9.0/gray/utils/__init__.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      580 2020-05-30 09:30:34.000000 gray-0.9.0/gray/utils/args.py
+drwxr-xr-x   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2021-05-11 09:26:15.623892 gray-0.9.0/gray/vendors/
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2020-08-15 17:35:40.000000 gray-0.9.0/gray/vendors/__init__.py
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     5130 2020-11-16 07:56:12.000000 gray-0.9.0/gray/vendors/trim.py
+drwxr-xr-x   0 dizballanze (1981409399) LD\Domain Users (593637566)        0 2021-05-11 09:26:15.614821 gray-0.9.0/gray.egg-info/
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     8714 2021-05-11 09:26:15.000000 gray-0.9.0/gray.egg-info/PKG-INFO
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      705 2021-05-11 09:26:15.000000 gray-0.9.0/gray.egg-info/SOURCES.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)        1 2021-05-11 09:26:15.000000 gray-0.9.0/gray.egg-info/dependency_links.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)       41 2021-05-11 09:26:15.000000 gray-0.9.0/gray.egg-info/entry_points.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      213 2021-05-11 09:26:15.000000 gray-0.9.0/gray.egg-info/requires.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)        5 2021-05-11 09:26:15.000000 gray-0.9.0/gray.egg-info/top_level.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)       59 2021-05-11 08:46:48.000000 gray-0.9.0/requirements.dev.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)      143 2021-05-11 09:16:17.000000 gray-0.9.0/requirements.txt
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)       61 2021-05-11 09:26:15.625829 gray-0.9.0/setup.cfg
+-rw-r--r--   0 dizballanze (1981409399) LD\Domain Users (593637566)     1862 2021-05-11 09:18:30.000000 gray-0.9.0/setup.py
```

### Comparing `gray-0.8.2/HISTORY.md` & `gray-0.9.0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/LICENSE` & `gray-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/PKG-INFO` & `gray-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gray
-Version: 0.8.2
+Version: 0.9.0
 Summary: Less uncompromising Python code formatter
 Home-page: https://github.com/dizballanze/gray
 Author: Yuri Shikanov
 Author-email: dizballanze@gmail.com
 License: MIT
 Description: # gray
```

### Comparing `gray-0.8.2/README.md` & `gray-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/formatters/__init__.py` & `gray-0.9.0/gray/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/formatters/autoflake.py` & `gray-0.9.0/gray/formatters/autoflake.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/formatters/fixit.py` & `gray-0.9.0/gray/formatters/fixit.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/formatters/isort.py` & `gray-0.9.0/gray/formatters/isort.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/formatters/pyupgrade.py` & `gray-0.9.0/gray/formatters/pyupgrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from argparse import Namespace
 from pathlib import Path
 
 from configargparse import Namespace
-from pyupgrade import _fix_file
+from pyupgrade._main import _fix_file
 
 from gray.formatters.base import BaseFormatter
 
 
 class PyUpgradeFormatter(BaseFormatter):
 
     def __init__(self, arguments: Namespace):
@@ -15,14 +15,16 @@
         if min_version < (3, 6):
             min_version = (3,)
 
         if min_version > (3, 7):
             min_version = (3, 7)
 
         self._args = Namespace(
+            keep_mock=arguments.pyupgrade_keep_mock,
+            keep_runtime_typing=arguments.pyupgrade_keep_runtime_typing,
             min_version=min_version,
             keep_percent_format=arguments.pyupgrade_keep_percent_format,
             exit_zero_even_if_changed=True,
         )
 
     def process(self, file_path: Path):
         _fix_file(str(file_path), self._args)
```

### Comparing `gray-0.8.2/gray/hooks.py` & `gray-0.9.0/gray/hooks.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/main.py` & `gray-0.9.0/gray/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,26 @@
 group = parser.add_argument_group("pyupgrade options")
 group.add_argument(
     "--pyupgrade-keep-percent-format",
     help="Do not upgrade percent formatted strings to f-strings",
     type=parse_bool,
     default=False,
 )
+group.add_argument(
+    "--pyupgrade-keep-mock",
+    help="Disable rewrite of mock imports",
+    type=parse_bool,
+    default=False,
+)
+group.add_argument(
+    "--pyupgrade-keep-runtime-typing",
+    help="Disable pep 585 typing rewrites",
+    type=parse_bool,
+    default=False,
+)
 
 group = parser.add_argument_group("unify options")
 group.add_argument(
     "--unify-quote",
     help="preferred quote",
     default='"',
 )
```

### Comparing `gray-0.8.2/gray/processing.py` & `gray-0.9.0/gray/processing.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/utils/args.py` & `gray-0.9.0/gray/utils/args.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray/vendors/trim.py` & `gray-0.9.0/gray/vendors/trim.py`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/gray.egg-info/PKG-INFO` & `gray-0.9.0/gray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gray
-Version: 0.8.2
+Version: 0.9.0
 Summary: Less uncompromising Python code formatter
 Home-page: https://github.com/dizballanze/gray
 Author: Yuri Shikanov
 Author-email: dizballanze@gmail.com
 License: MIT
 Description: # gray
```

### Comparing `gray-0.8.2/gray.egg-info/SOURCES.txt` & `gray-0.9.0/gray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gray-0.8.2/setup.py` & `gray-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 readme = open("README.md").read()
 
 history = open("HISTORY.md").read()
 
 setup(
     name=module_name,
-    version="0.8.2",
+    version="0.9.0",
     description="Less uncompromising Python code formatter",
     long_description=f"{readme}\n\n{history}",
     long_description_content_type="text/markdown",
     author="Yuri Shikanov",
     author_email="dizballanze@gmail.com",
     url="https://github.com/dizballanze/gray",
     packages=find_packages(exclude=["tests"]),
```

