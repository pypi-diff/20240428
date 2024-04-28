# Comparing `tmp/genmq-0.5.0.tar.gz` & `tmp/genmq-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genmq-0.5.0.tar", last modified: Wed Mar  6 12:11:33 2024, max compression
+gzip compressed data, was "genmq-0.6.0.tar", last modified: Sun Apr 28 13:59:57 2024, max compression
```

## Comparing `genmq-0.5.0.tar` & `genmq-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:11:33.392671 genmq-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-06 12:11:29.000000 genmq-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-06 12:11:33.392671 genmq-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-06 12:11:29.000000 genmq-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-06 12:11:29.000000 genmq-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-06 12:11:33.392671 genmq-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:11:33.392671 genmq-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:11:33.392671 genmq-0.5.0/src/genmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-06 12:11:33.000000 genmq-0.5.0/src/genmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-06 12:11:33.000000 genmq-0.5.0/src/genmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 12:11:33.000000 genmq-0.5.0/src/genmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-06 12:11:33.000000 genmq-0.5.0/src/genmq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-06 12:11:33.000000 genmq-0.5.0/src/genmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 12:11:33.000000 genmq-0.5.0/src/genmq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:57.891221 genmq-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 13:59:54.000000 genmq-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-28 13:59:57.891221 genmq-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-28 13:59:54.000000 genmq-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-28 13:59:54.000000 genmq-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:59:57.891221 genmq-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:57.887221 genmq-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:57.891221 genmq-0.6.0/src/genmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-28 13:59:54.000000 genmq-0.6.0/src/genmq.py
```

### Comparing `genmq-0.5.0/LICENSE` & `genmq-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genmq-0.5.0/PKG-INFO` & `genmq-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: genmq
-Version: 0.5.0
+Version: 0.6.0
 Summary: Moodle quiz generator
-Home-page: https://github.com/ccaprani/genmq
-Author: Colin Caprani
-Author-email: colin.caprani@monash.edu
+Author-email: Colin Caprani <colin.caprani@monash.edu>
 License: GNU General Public License v3.0
+Project-URL: Homepage, https://ccaprani.github.io/genmq/
 Project-URL: Documentation, https://ccaprani.github.io/genmq/
 Project-URL: Source, https://github.com/ccaprani/genmq/
 Project-URL: Tracker, https://github.com/ccaprani/genmq/issues/
+Keywords: moodle,quiz,question bank
+Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -20,17 +21,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: jinja2
-Requires-Dist: tqdm
 
 # genmq
 A Moodle quiz generator using LaTeX and the `moodle.sty` package with jinja2 templates
 
 *Generates Individualized Moodle Quizzes based on a LaTeX Template*
 
 **Author:** Colin Caprani,
```

### Comparing `genmq-0.5.0/README.md` & `genmq-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `genmq-0.5.0/src/genmq.egg-info/PKG-INFO` & `genmq-0.6.0/src/genmq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: genmq
-Version: 0.5.0
+Version: 0.6.0
 Summary: Moodle quiz generator
-Home-page: https://github.com/ccaprani/genmq
-Author: Colin Caprani
-Author-email: colin.caprani@monash.edu
+Author-email: Colin Caprani <colin.caprani@monash.edu>
 License: GNU General Public License v3.0
+Project-URL: Homepage, https://ccaprani.github.io/genmq/
 Project-URL: Documentation, https://ccaprani.github.io/genmq/
 Project-URL: Source, https://github.com/ccaprani/genmq/
 Project-URL: Tracker, https://github.com/ccaprani/genmq/issues/
+Keywords: moodle,quiz,question bank
+Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -20,17 +21,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: jinja2
-Requires-Dist: tqdm
 
 # genmq
 A Moodle quiz generator using LaTeX and the `moodle.sty` package with jinja2 templates
 
 *Generates Individualized Moodle Quizzes based on a LaTeX Template*
 
 **Author:** Colin Caprani,
```

