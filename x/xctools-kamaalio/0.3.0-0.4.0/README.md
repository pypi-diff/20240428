# Comparing `tmp/xctools_kamaalio-0.3.0.tar.gz` & `tmp/xctools_kamaalio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xctools_kamaalio-0.3.0.tar", last modified: Wed Feb 14 21:40:02 2024, max compression
+gzip compressed data, was "xctools_kamaalio-0.4.0.tar", last modified: Sun Apr 28 12:18:30 2024, max compression
```

## Comparing `xctools_kamaalio-0.3.0.tar` & `xctools_kamaalio-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:40:02.700576 xctools_kamaalio-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-14 21:40:02.700576 xctools_kamaalio-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 21:40:02.700576 xctools_kamaalio-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:40:02.692577 xctools_kamaalio-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:40:02.696576 xctools_kamaalio-0.3.0/src/xctools_kamaalio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:40:02.696576 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/acknowledgments.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/trust_swift_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/trust_swift_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/project_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio/xctools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:40:02.700576 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-14 21:40:02.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-14 21:40:02.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 21:40:02.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-14 21:40:02.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-14 21:40:02.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-14 21:40:02.000000 xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:40:02.696576 xctools_kamaalio-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-14 21:39:43.000000 xctools_kamaalio-0.3.0/tests/test_acknowledgments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:30.296817 xctools_kamaalio-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-28 12:18:30.296817 xctools_kamaalio-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:18:30.296817 xctools_kamaalio-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:30.292817 xctools_kamaalio-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:30.292817 xctools_kamaalio-0.4.0/src/xctools_kamaalio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:30.296817 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/acknowledgments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/trust_swift_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/trust_swift_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/project_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio/xctools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:30.296817 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-28 12:18:30.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-28 12:18:30.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:18:30.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 12:18:30.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-28 12:18:30.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 12:18:30.000000 xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:18:30.296817 xctools_kamaalio-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/tests/test_acknowledgments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-28 12:18:10.000000 xctools_kamaalio-0.4.0/tests/test_bump_version.py
```

### Comparing `xctools_kamaalio-0.3.0/LICENSE` & `xctools_kamaalio-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/PKG-INFO` & `xctools_kamaalio-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools_kamaalio
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/Kamaalio/XcTools
 Project-URL: Bug Tracker, https://github.com/Kamaalio/XcTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.3.0/pyproject.toml` & `xctools_kamaalio-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project.scripts]
 xctools = "xctools_kamaalio:cli.cli"
 
 
 [project]
 name = "xctools_kamaalio"
-version = "0.3.0"
+version = "0.4.0"
 authors = [{ name = "Kamaal Farah", email = "kamaal.f1@gmail.com" }]
 description = "A package to help deal with Xcode projects."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/acknowledgments.py` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/acknowledgments.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/archive.py` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/archive.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/build.py` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/build.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio/actions/test.py` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio/actions/test.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio/cli.py` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio/cli.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio/xctools.py` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio/xctools.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/PKG-INFO` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools_kamaalio
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/Kamaalio/XcTools
 Project-URL: Bug Tracker, https://github.com/Kamaalio/XcTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.3.0/src/xctools_kamaalio.egg-info/SOURCES.txt` & `xctools_kamaalio-0.4.0/src/xctools_kamaalio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 src/xctools_kamaalio/actions/build.py
 src/xctools_kamaalio/actions/bump_version.py
 src/xctools_kamaalio/actions/export_archive.py
 src/xctools_kamaalio/actions/test.py
 src/xctools_kamaalio/actions/trust_swift_macros.py
 src/xctools_kamaalio/actions/trust_swift_plugins.py
 src/xctools_kamaalio/actions/upload.py
-tests/test_acknowledgments.py
+tests/test_acknowledgments.py
+tests/test_bump_version.py
```

### Comparing `xctools_kamaalio-0.3.0/tests/test_acknowledgments.py` & `xctools_kamaalio-0.4.0/tests/test_acknowledgments.py`

 * *Files identical despite different names*

