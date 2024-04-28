# Comparing `tmp/line_profiler-4.1.2.tar.gz` & `tmp/line_profiler-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line_profiler-4.1.2.tar", last modified: Fri Nov  3 00:10:30 2023, max compression
+gzip compressed data, was "line_profiler-4.1.3.tar", last modified: Sun Apr 28 21:39:36 2024, max compression
```

## Comparing `line_profiler-4.1.2.tar` & `line_profiler-4.1.3.tar`

### file list

```diff
@@ -1,66 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:30.518062 line_profiler-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2023-11-03 00:10:23.000000 line_profiler-4.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-11-03 00:10:23.000000 line_profiler-4.1.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-11-03 00:10:23.000000 line_profiler-4.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2023-11-03 00:10:23.000000 line_profiler-4.1.2/LICENSE_Python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-03 00:10:23.000000 line_profiler-4.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21474 2023-11-03 00:10:30.518062 line_profiler-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20078 2023-11-03 00:10:23.000000 line_profiler-4.1.2/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    15044 2023-11-03 00:10:23.000000 line_profiler-4.1.2/kernprof.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:30.514063 line_profiler-4.1.2/line_profiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/_line_profiler.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:30.514063 line_profiler-4.1.2/line_profiler/autoprofile/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/ast_profle_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/ast_tree_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/autoprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/line_profiler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/profmod_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/autoprofile/util_static.py
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/explicit_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/explicit_profiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/ipython_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/ipython_extension.pyi
--rwxr-xr-x   0 runner    (1001) docker     (127)    17580 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/line_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/line_profiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    40603 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/python25.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/timers.c
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/timers.h
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/unset_trace.c
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-03 00:10:23.000000 line_profiler-4.1.2/line_profiler/unset_trace.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:30.514063 line_profiler-4.1.2/line_profiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21474 2023-11-03 00:10:30.000000 line_profiler-4.1.2/line_profiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-11-03 00:10:30.000000 line_profiler-4.1.2/line_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 00:10:30.000000 line_profiler-4.1.2/line_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-03 00:10:30.000000 line_profiler-4.1.2/line_profiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2023-11-03 00:10:30.000000 line_profiler-4.1.2/line_profiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-03 00:10:30.000000 line_profiler-4.1.2/line_profiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-11-03 00:10:23.000000 line_profiler-4.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:30.518062 line_profiler-4.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements/ipython.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-03 00:10:23.000000 line_profiler-4.1.2/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     4765 2023-11-03 00:10:23.000000 line_profiler-4.1.2/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 00:10:30.518062 line_profiler-4.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    11091 2023-11-03 00:10:23.000000 line_profiler-4.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:10:30.518062 line_profiler-4.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/complex_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_autoprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_complex_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_duplicate_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_explicit_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_kernprof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2023-11-03 00:10:23.000000 line_profiler-4.1.2/tests/test_line_profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:36.885409 line_profiler-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-28 21:39:22.000000 line_profiler-4.1.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-28 21:39:22.000000 line_profiler-4.1.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-28 21:39:22.000000 line_profiler-4.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-28 21:39:22.000000 line_profiler-4.1.3/LICENSE_Python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-28 21:39:22.000000 line_profiler-4.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34433 2024-04-28 21:39:36.881409 line_profiler-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20971 2024-04-28 21:39:22.000000 line_profiler-4.1.3/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15044 2024-04-28 21:39:22.000000 line_profiler-4.1.3/kernprof.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:36.853408 line_profiler-4.1.3/line_profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   897986 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler/_line_profiler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/_line_profiler.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:36.857409 line_profiler-4.1.3/line_profiler/autoprofile/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/ast_profle_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/ast_profle_transformer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/ast_tree_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/ast_tree_profiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/autoprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/autoprofile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/line_profiler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/line_profiler_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/profmod_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/profmod_extractor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/util_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/autoprofile/util_static.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/explicit_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/explicit_profiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/ipython_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/ipython_extension.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17704 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/line_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/line_profiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    40603 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/python25.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/timers.c
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/timers.h
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/unset_trace.c
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 21:39:22.000000 line_profiler-4.1.3/line_profiler/unset_trace.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:36.861409 line_profiler-4.1.3/line_profiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34433 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 21:39:36.000000 line_profiler-4.1.3/line_profiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-28 21:39:22.000000 line_profiler-4.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:36.857409 line_profiler-4.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements/ipython.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 21:39:22.000000 line_profiler-4.1.3/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6716 2024-04-28 21:39:22.000000 line_profiler-4.1.3/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:39:36.885409 line_profiler-4.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11091 2024-04-28 21:39:22.000000 line_profiler-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:39:36.861409 line_profiler-4.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/complex_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_autoprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_complex_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_duplicate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_explicit_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_kernprof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-28 21:39:22.000000 line_profiler-4.1.3/tests/test_line_profiler.py
```

### Comparing `line_profiler-4.1.2/CHANGELOG.rst` & `line_profiler-4.1.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Changes
 =======
 
+4.1.3
+~~~~~
+* FIX: duration summary now respects the stripzeros argument.
+
 4.1.2
-~~~~
+~~~~~
 * ENH: Add support for Python 3.12 #246
-* ENH: Add osx universal2 and arm64 wheels
-* ENH: Fix issue with integer overflow on 32 bit systems
+* ENH: Add osx universal2 and arm64 wheels #251
+* ENH: Fix issue with integer overflow on 32 bit systems #249
 
 4.1.1
-~~~~
+~~~~~
 * FIX: ``get_stats`` is no longer slowed down when profiling many code sections #236
 
 4.1.0
-~~~~
+~~~~~
 * FIX: skipzeros now checks for zero hits instead of zero time
 * FIX: Fixed errors in Python 3.11 with duplicate functions.
 * FIX: ``show_text`` now increases column sizes or switches to scientific notation to maintain alignment
 * ENH: ``show_text`` now has new options: sort and summarize
 * ENH: Added new CLI arguments ``-srm`` to ``line_profiler`` to control sorting, rich printing, and summary printing.
 * ENH: New global ``profile`` function that can be enabled by ``--profile`` or ``LINE_PROFILE=1``.
 * ENH: New auto-profile feature in ``kernprof`` that will profile all functions in specified modules.
 * ENH: Kernprof now outputs instructions on how to view results.
 * ENH: Added readthedocs integration: https://kernprof.readthedocs.io/en/latest/index.html
 
 4.0.3
-~~~~
+~~~~~
 * FIX: Stop requiring bleeding-edge Cython unless necesasry (for Python 3.12).  #206
 
 4.0.2
 ~~~~~
 * FIX: AttributeError on certain methods. #191
 
 4.0.1
```

### Comparing `line_profiler-4.1.2/CMakeLists.txt` & `line_profiler-4.1.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/LICENSE.txt` & `line_profiler-4.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/LICENSE_Python.txt` & `line_profiler-4.1.3/LICENSE_Python.txt`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/PKG-INFO` & `line_profiler-4.1.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,7 @@
-Metadata-Version: 2.1
-Name: line_profiler
-Version: 4.1.2
-Summary: Line-by-line profiler
-Home-page: https://github.com/pyutils/line_profiler
-Author: Robert Kern
-Author-email: robert.kern@enthought.com
-License: BSD
-Keywords: timing,timer,profiling,profiler,line_profiler
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-Provides-Extra: all-strict
-Provides-Extra: ipython
-Provides-Extra: ipython-strict
-Provides-Extra: optional
-Provides-Extra: optional-strict
-Provides-Extra: runtime-strict
-Provides-Extra: tests
-Provides-Extra: tests-strict
-License-File: LICENSE.txt
-License-File: LICENSE_Python.txt
-
 line_profiler and kernprof
 --------------------------
 
 |Pypi| |ReadTheDocs| |Downloads| |CircleCI| |GithubActions| |Codecov|
 
 
 This is the official ``line_profiler`` repository. The most recent version of
@@ -68,16 +29,40 @@
 They are available under a `BSD license`_.
 
 .. _BSD license: https://raw.githubusercontent.com/pyutils/line_profiler/master/LICENSE.txt
 
 .. contents::
 
 
-Quick Start
-===========
+Quick Start (Modern)
+====================
+
+This guide is for versions of line profiler starting a ``4.1.0``.
+
+To profile a python script:
+
+* Install line_profiler: ``pip install line_profiler``.
+
+* In the relevant file(s), import line profiler and decorate function(s) you
+  want to profile with ``@line_profiler.profile``.
+
+* Set the environment variable ``LINE_PROFILE=1`` and run your script as normal.
+  When the script ends a summary of profile results, files written to disk, and
+  instructions for inspecting details will be written to stdout.
+
+For more details and a short tutorial see `Line Profiler Basic Usage <https://kernprof.readthedocs.io/en/latest/#line-profiler-basic-usage>`_.
+
+
+Quick Start (Legacy)
+====================
+
+This section is the original quick-start guide, and may eventually be removed
+from the README. This will work with current and older (pre ``4.1.0``) versions
+of line profiler.
+
 To profile a python script:
 
 * Install line_profiler: ``pip install line_profiler``.
 
 * Decorate function(s) you want to profile with @profile. The decorator will be made automatically available on run.
 
 * Run ``kernprof -lv script_to_profile.py``.
@@ -476,9 +461,7 @@
    :target: https://pypi.python.org/pypi/line_profiler
 .. |Downloads| image:: https://img.shields.io/pypi/dm/line_profiler.svg
    :target: https://pypistats.org/packages/line_profiler
 .. |GithubActions| image:: https://github.com/pyutils/line_profiler/actions/workflows/tests.yml/badge.svg?branch=main
    :target: https://github.com/pyutils/line_profiler/actions?query=branch%3Amain
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/kernprof/badge/?version=latest
     :target: http://kernprof.readthedocs.io/en/latest/
-
-
```

### Comparing `line_profiler-4.1.2/kernprof.py` & `line_profiler-4.1.3/kernprof.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 import asyncio  # NOQA
 import concurrent.futures  # NOQA
 import time
 from argparse import ArgumentError, ArgumentParser
 
 # NOTE: This version needs to be manually maintained in
 # line_profiler/line_profiler.py and line_profiler/__init__.py as well
-__version__ = '4.1.2'
+__version__ = '4.1.3'
 
 # Guard the import of cProfile such that 3.x people
 # without lsprof can still use this script.
 try:
     from cProfile import Profile
 except ImportError:
     try:
```

### Comparing `line_profiler-4.1.2/line_profiler/CMakeLists.txt` & `line_profiler-4.1.3/line_profiler/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/__init__.py` & `line_profiler-4.1.3/line_profiler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 mkinit ./line_profiler/__init__.py --relative -w
 """
 
 
 # from .line_profiler import __version__
 
 # NOTE: This needs to be in sync with ../kernprof.py and line_profiler.py
-__version__ = '4.1.2'
+__version__ = '4.1.3'
 
 from .line_profiler import (LineProfiler,
                             load_ipython_extension, load_stats, main,
                             show_func, show_text,)
 
 
 from .explicit_profiler import profile
```

### Comparing `line_profiler-4.1.2/line_profiler/_line_profiler.pyx` & `line_profiler-4.1.3/line_profiler/_line_profiler.pyx`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/__init__.py` & `line_profiler-4.1.3/line_profiler/autoprofile/__init__.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/ast_profle_transformer.py` & `line_profiler-4.1.3/line_profiler/autoprofile/ast_profle_transformer.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/ast_tree_profiler.py` & `line_profiler-4.1.3/line_profiler/autoprofile/ast_tree_profiler.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/autoprofile.py` & `line_profiler-4.1.3/line_profiler/autoprofile/autoprofile.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/line_profiler_utils.py` & `line_profiler-4.1.3/line_profiler/autoprofile/line_profiler_utils.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/profmod_extractor.py` & `line_profiler-4.1.3/line_profiler/autoprofile/profmod_extractor.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/autoprofile/util_static.py` & `line_profiler-4.1.3/line_profiler/autoprofile/util_static.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/explicit_profiler.py` & `line_profiler-4.1.3/line_profiler/explicit_profiler.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/explicit_profiler.pyi` & `line_profiler-4.1.3/line_profiler/explicit_profiler.pyi`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/ipython_extension.py` & `line_profiler-4.1.3/line_profiler/ipython_extension.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/line_profiler.py` & `line_profiler-4.1.3/line_profiler/line_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError as ex:
     raise ImportError(
         'The line_profiler._line_profiler c-extension is not importable. '
         f'Has it been compiled? Underlying error is ex={ex!r}'
     )
 
 # NOTE: This needs to be in sync with ../kernprof.py and __init__.py
-__version__ = '4.1.2'
+__version__ = '4.1.3'
 
 
 def load_ipython_extension(ip):
     """ API for IPython to recognize this module as an IPython extension.
     """
     from .ipython_extension import LineProfilerMagics
     ip.register_magics(LineProfilerMagics)
@@ -216,18 +216,20 @@
 
 
 # This could be in the ipython_extension submodule,
 # but it doesn't depend on the IPython module so it's easier to just let it stay here.
 def is_ipython_kernel_cell(filename):
     """ Return True if a filename corresponds to a Jupyter Notebook cell
     """
+    filename = os.path.normcase(filename)
+    temp_dir = os.path.normcase(tempfile.gettempdir())
     return (
         filename.startswith('<ipython-input-') or
-        filename.startswith(os.path.join(tempfile.gettempdir(), 'ipykernel_')) or
-        filename.startswith(os.path.join(tempfile.gettempdir(), 'xpython_'))
+        filename.startswith(os.path.join(temp_dir, 'ipykernel_')) or
+        filename.startswith(os.path.join(temp_dir, 'xpython_'))
     )
 
 
 def show_func(filename, start_lineno, func_name, timings, unit,
               output_unit=None, stream=None, stripzeros=False, rich=False):
     """
     Show results for a single function.
@@ -463,16 +465,17 @@
                       output_unit=output_unit, stream=stream,
                       stripzeros=stripzeros, rich=rich)
 
     if summarize:
         # Summarize the total time for each function
         for (fn, lineno, name), timings in stats_order:
             total_time = sum(t[2] for t in timings) * unit
-            line = '%6.2f seconds - %s:%s - %s\n' % (total_time, fn, lineno, name)
-            stream.write(line)
+            if not stripzeros or total_time:
+                line = '%6.2f seconds - %s:%s - %s\n' % (total_time, fn, lineno, name)
+                stream.write(line)
 
 
 def load_stats(filename):
     """ Utility function to load a pickled LineStats object from a given
     filename.
     """
     with open(filename, 'rb') as f:
```

### Comparing `line_profiler-4.1.2/line_profiler/line_profiler.pyi` & `line_profiler-4.1.3/line_profiler/line_profiler.pyi`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/python25.pxd` & `line_profiler-4.1.3/line_profiler/python25.pxd`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler/timers.c` & `line_profiler-4.1.3/line_profiler/timers.c`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/line_profiler.egg-info/SOURCES.txt` & `line_profiler-4.1.3/line_profiler.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requirements.txt
 run_tests.py
 setup.py
 line_profiler/CMakeLists.txt
 line_profiler/__init__.py
 line_profiler/__main__.py
 line_profiler/__main__.pyi
+line_profiler/_line_profiler.cpp
 line_profiler/_line_profiler.pyx
 line_profiler/explicit_profiler.py
 line_profiler/explicit_profiler.pyi
 line_profiler/ipython_extension.py
 line_profiler/ipython_extension.pyi
 line_profiler/line_profiler.py
 line_profiler/line_profiler.pyi
@@ -30,19 +31,25 @@
 line_profiler.egg-info/SOURCES.txt
 line_profiler.egg-info/dependency_links.txt
 line_profiler.egg-info/entry_points.txt
 line_profiler.egg-info/requires.txt
 line_profiler.egg-info/top_level.txt
 line_profiler/autoprofile/__init__.py
 line_profiler/autoprofile/ast_profle_transformer.py
+line_profiler/autoprofile/ast_profle_transformer.pyi
 line_profiler/autoprofile/ast_tree_profiler.py
+line_profiler/autoprofile/ast_tree_profiler.pyi
 line_profiler/autoprofile/autoprofile.py
+line_profiler/autoprofile/autoprofile.pyi
 line_profiler/autoprofile/line_profiler_utils.py
+line_profiler/autoprofile/line_profiler_utils.pyi
 line_profiler/autoprofile/profmod_extractor.py
+line_profiler/autoprofile/profmod_extractor.pyi
 line_profiler/autoprofile/util_static.py
+line_profiler/autoprofile/util_static.pyi
 requirements/build.txt
 requirements/docs.txt
 requirements/ipython.txt
 requirements/optional.txt
 requirements/runtime.txt
 requirements/tests.txt
 tests/complex_example.py
```

### Comparing `line_profiler-4.1.2/pyproject.toml` & `line_profiler-4.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     "*/setup.py"
 ]
 
 [tool.cibuildwheel]
 build = "cp36-* cp37-* cp38-* cp39-* cp310-* cp311-* cp312-*"
 build-frontend = "build"
 build-verbosity = 1
-test-requires = [ "-r requirements/tests.txt",]
+#test-requires = [ "-r requirements/tests-strict.txt",]
 test-command = "python {project}/run_tests.py"
+test-extras = ["tests-strict", "runtime-strict"]
 
 # https://cibuildwheel.readthedocs.io/en/stable/options/#archs
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "universal2", "arm64"]
 
 
 [tool.mypy]
@@ -68,12 +69,12 @@
 # the console_scripts entry point creates the xdoctest executable
 console_scripts = [
     "kernprof=kernprof:main",
 ]
 
 
 [tool.pytest.ini_options]
-addopts = "--ignore-glob=setup.py --ignore-glob=dev"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild"
+addopts = "--ignore-glob=setup.py --ignore-glob=dev --ignore-glob=setup.py --ignore-glob=docs --ignore-glob=agentx"
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs agentx"
 filterwarnings = [
     "default",
 ]
```

### Comparing `line_profiler-4.1.2/requirements/build.txt` & `line_profiler-4.1.3/requirements/build.txt`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/setup.py` & `line_profiler-4.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/complex_example.py` & `line_profiler-4.1.3/tests/complex_example.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/test_autoprofile.py` & `line_profiler-4.1.3/tests/test_autoprofile.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/test_cli.py` & `line_profiler-4.1.3/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,12 +53,31 @@
     """
     Ensure that line_profiler and kernprof have the same version info
     """
     import ubelt as ub
     info1 = ub.cmd(f'{executable} -m line_profiler --version')
     info2 = ub.cmd(f'{executable} -m kernprof --version')
 
+    if info1['ret'] != 0:
+        print(f'Error querying line-profiler version: {info1}')
+
+    if info2['ret'] != 0:
+        print(f'Error querying kernprof version: {info2}')
+
     # Strip local version suffixes
     version1 = info1['out'].strip().split('+')[0]
     version2 = info2['out'].strip().split('+')[0]
 
-    assert version2 == version1, 'kernprof and line_profiler must be in sync'
+    if version2 != version1:
+        raise AssertionError(
+            'Version Mismatch: kernprof and line_profiler must be in sync. '
+            f'kernprof.line_profiler = {version1}. '
+            f'kernprof.__version__ = {version2}. '
+        )
+
+
+if __name__ == '__main__':
+    """
+    CommandLine:
+        python ~/code/line_profiler/tests/test_cli.py
+    """
+    test_version_agreement()
```

### Comparing `line_profiler-4.1.2/tests/test_complex_case.py` & `line_profiler-4.1.3/tests/test_complex_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def test_complex_example_python_none():
     """
     Make sure the complex example script works without any profiling
     """
     complex_fpath = get_complex_example_fpath()
-    info = ub.cmd(f'python {complex_fpath}', shell=True, verbose=3, env=ub.udict(os.environ) | {'PROFILE_TYPE': 'none'})
+    info = ub.cmd(f'{sys.executable} {complex_fpath}', shell=True, verbose=3, env=ub.udict(os.environ) | {'PROFILE_TYPE': 'none'})
     assert info.stdout == ''
     info.check_returncode()
 
 
 def test_varied_complex_invocations():
     """
     Tests variations of running the complex example:
```

### Comparing `line_profiler-4.1.2/tests/test_explicit_profile.py` & `line_profiler-4.1.3/tests/test_explicit_profile.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/test_import.py` & `line_profiler-4.1.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/test_ipython.py` & `line_profiler-4.1.3/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/test_kernprof.py` & `line_profiler-4.1.3/tests/test_kernprof.py`

 * *Files identical despite different names*

### Comparing `line_profiler-4.1.2/tests/test_line_profiler.py` & `line_profiler-4.1.3/tests/test_line_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,16 @@
     start_lineno = func.__code__.co_firstlineno
     filename = func.__code__.co_filename
     func_name = func.__name__
 
     def get_func_linenos(func):
         import sys
         if sys.version_info[0:2] >= (3, 10):
-            return sorted(set([t[2] for t in func.__code__.co_lines()]))
+            return sorted(set([t[0] if t[2] is None else t[2]
+                               for t in func.__code__.co_lines()]))
         else:
             import dis
             return sorted(set([t[1] for t in dis.findlinestarts(func.__code__)]))
     line_numbers = get_func_linenos(func)
 
     unit = 1.0
     output_unit = 1.0
```

