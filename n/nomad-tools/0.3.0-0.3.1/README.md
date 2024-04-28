# Comparing `tmp/nomad_tools-0.3.0.tar.gz` & `tmp/nomad_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_tools-0.3.0.tar", last modified: Wed Apr 17 20:35:21 2024, max compression
+gzip compressed data, was "nomad_tools-0.3.1.tar", last modified: Sun Apr 28 10:40:13 2024, max compression
```

## Comparing `nomad_tools-0.3.0.tar` & `nomad_tools-0.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.747339 nomad_tools-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-17 20:35:21.747339 nomad_tools-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:35:21.747339 nomad_tools-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.735339 nomad_tools-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common_nomad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/entry_constrainteval.py
--rw-r--r--   0 runner    (1001) docker     (127)    21243 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/entry_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/exit_on_thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/flagdebug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28872 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_dockers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_downloadrelease.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/script.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/waiter.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    28600 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_smart_start_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_taskexec.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18624 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_vardir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77612 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomaddbjob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools/nomadlib/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/datadict.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadt_completion.sh
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/taskexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/transferstats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/tests/test_nomad_cp_complete.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/tests/test_taskexec_transfer_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/tests/testlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.526031 nomad_tools-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-28 10:40:13.526031 nomad_tools-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:40:13.526031 nomad_tools-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.518031 nomad_tools-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common_nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/entry_constrainteval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/entry_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/exit_on_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/flagdebug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28872 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_dockers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_downloadrelease.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/script.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/waiter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28600 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_smart_start_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_taskexec.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18624 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_vardir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77612 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomaddbjob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools/nomadlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/datadict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadt_completion.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/taskexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/transferstats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/tests/test_nomad_cp_complete.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/tests/test_taskexec_transfer_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/tests/testlib.py
```

### Comparing `nomad_tools-0.3.0/LICENSE` & `nomad_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/PKG-INFO` & `nomad_tools-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: nomad-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
 Author: Kamil Cukrowski
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
 Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
 Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: requests==2.31.0
-Requires-Dist: typing_extensions==4.7.1
-Requires-Dist: websocket-client==1.6.1
-Requires-Dist: clickdc==0.0.5
-Requires-Dist: clickforward==0.0.1
-Requires-Dist: python-dotenv==0.21.1
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: requests>=2.31.0
+Requires-Dist: typing_extensions>=4.7.1
+Requires-Dist: websocket-client>=1.6.1
+Requires-Dist: clickdc>=0.0.5
+Requires-Dist: clickforward>=0.0.1
+Requires-Dist: python-dotenv>=0.21.1
 Requires-Dist: packaging>=16.1
+Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: tomli==2.0.1; extra == "test"
 Requires-Dist: pytest==7.4.4; extra == "test"
 Requires-Dist: pytest-xdist==3.5.0; extra == "test"
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
 
 # nomadtools
@@ -34,14 +35,15 @@
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
     * [Shell completion](#shell-completion)
 * [Usage](#usage)
     * [watch](#watch)
     * [go](#go)
+    * [constrainteval](#constrainteval)
     * [port](#port)
     * [vardir](#vardir)
     * [cp](#cp)
     * [gitlab-runner](#gitlab-runner)
     * [nomad-dockers](#nomad-dockers)
     * [downloadrelease](#downloadrelease)
     * [import nomad_tools](#import-nomad_tools)
@@ -136,14 +138,34 @@
 Executing busybox-1.36.1-r15.trigger
 OK: 10 MiB in 19 packages
 INFO:nomad_tools.nomad_watch:Purging job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587
 INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default purged with no active allocations, evaluations nor deployments. Exiting.
 INFO:nomad_tools.nomad_watch:Single task exited with 0 exit status. Exit code is 0.
 ```
 
+## constrainteval
+
+Evaluate a constraint and show all nodes that match the constraint. In
+addition to the node names, it also shows all attributes referenced while
+evaluating the constraint given on command line arguments. Useful for
+searching for which hosts contain what value of a attribute.
+
+```
+$ nomadtools constrainteval attr.cpu.arch is_set
+name   attr.cpu.arch
+-----  ---------------
+node1  amd64
+node2  amd64
+```
+
+This mode uses a cache in `~/.cache/nomadtools/nodes.json` for caching all the
+attributes of nodes downloaded from Nomad. This is used to speed up. The
+program needs to make one query for every single node in Nomad, which for a
+lot of nodes is costly.
+
 ## port
 
 Prints out the ports allocated for a particular Nomad job or
 allocation. It is meant to mimic `docker port` command.
 
 ```
 $ nomadtools port httpd
```

### Comparing `nomad_tools-0.3.0/README.md` & `nomad_tools-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
     * [Shell completion](#shell-completion)
 * [Usage](#usage)
     * [watch](#watch)
     * [go](#go)
+    * [constrainteval](#constrainteval)
     * [port](#port)
     * [vardir](#vardir)
     * [cp](#cp)
     * [gitlab-runner](#gitlab-runner)
     * [nomad-dockers](#nomad-dockers)
     * [downloadrelease](#downloadrelease)
     * [import nomad_tools](#import-nomad_tools)
@@ -109,14 +110,34 @@
 Executing busybox-1.36.1-r15.trigger
 OK: 10 MiB in 19 packages
 INFO:nomad_tools.nomad_watch:Purging job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587
 INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default purged with no active allocations, evaluations nor deployments. Exiting.
 INFO:nomad_tools.nomad_watch:Single task exited with 0 exit status. Exit code is 0.
 ```
 
+## constrainteval
+
+Evaluate a constraint and show all nodes that match the constraint. In
+addition to the node names, it also shows all attributes referenced while
+evaluating the constraint given on command line arguments. Useful for
+searching for which hosts contain what value of a attribute.
+
+```
+$ nomadtools constrainteval attr.cpu.arch is_set
+name   attr.cpu.arch
+-----  ---------------
+node1  amd64
+node2  amd64
+```
+
+This mode uses a cache in `~/.cache/nomadtools/nodes.json` for caching all the
+attributes of nodes downloaded from Nomad. This is used to speed up. The
+program needs to make one query for every single node in Nomad, which for a
+lot of nodes is costly.
+
 ## port
 
 Prints out the ports allocated for a particular Nomad job or
 allocation. It is meant to mimic `docker port` command.
 
 ```
 $ nomadtools port httpd
```

### Comparing `nomad_tools-0.3.0/pyproject.toml` & `nomad_tools-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/colors.py` & `nomad_tools-0.3.1/src/nomad_tools/colors.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/common_base.py` & `nomad_tools-0.3.1/src/nomad_tools/common_base.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/common_click.py` & `nomad_tools-0.3.1/src/nomad_tools/common_click.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 import os
 from typing import Any, Callable, Dict, Iterable, List, Optional
 
 import click
 
 from .common_base import composed, print_version, shell_completion
 
+EPILOG = "Written by Kamil Cukrowski 2024. Licensed under GNU GPL version or later."
+
 
 def complete_set_namespace(ctx: click.Context):
     namespace = ctx.params.get("namespace")
     if namespace:
         os.environ["NOMAD_NAMESPACE"] = namespace
 
 
@@ -70,14 +73,40 @@
 
 def common_options():
     return composed(
         click.help_option("-h", "--help"),
     )
 
 
+def verbose_option():
+    return click.option(
+        "-v",
+        "--verbose",
+        count=True,
+        expose_value=False,
+        is_eager=True,
+        callback=lambda v, *_: logging.root.setLevel(
+            max(logging.DEBUG, logging.root.level - 10)
+        ),
+    )
+
+
+def quiet_option():
+    return click.option(
+        "-q",
+        "--quiet",
+        count=True,
+        expose_value=False,
+        is_eager=True,
+        callback=lambda v, *_: logging.root.setLevel(
+            min(logging.CRITICAL, logging.root.level + 10)
+        ),
+    )
+
+
 def __alias_option_callback(
     aliased: Dict[str, Any],
     ctx: click.Context,
     param: click.Parameter,
     value: Any,
 ):
     """Callback called from alias_option option."""
```

### Comparing `nomad_tools-0.3.0/src/nomad_tools/common_nomad.py` & `nomad_tools-0.3.1/src/nomad_tools/common_nomad.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/entrypoint.py` & `nomad_tools-0.3.1/src/nomad_tools/entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import click
 import clickforward
 from click.shell_completion import BashComplete
 
 from . import (
     entry_constrainteval,
     entry_go,
@@ -9,31 +11,33 @@
     nomad_dockers,
     nomad_downloadrelease,
     nomad_gitlab_runner,
     nomad_port,
     nomad_vardir,
     nomad_watch,
 )
-from .common_click import common_options, main_options
+from .common_click import EPILOG, common_options, main_options
 from .common_nomad import namespace_option
 
 clickforward.init()
 
 # Fix bash splitting completion on colon.
 # Use __reassemble_comp_words_by_ref from bash-completion.
 # Pass COMP_POINT as environment variable.
 BashComplete.source_template = r"""\
     %(complete_func)s() {
-        if [[ $(type -t __reassemble_comp_words_by_ref) != function ]]; then
-            return -1
-        fi
         local cword words=()
-        __reassemble_comp_words_by_ref "=:" words cword
+        if [[ $(type -t __reassemble_comp_words_by_ref) == function ]]; then
+            __reassemble_comp_words_by_ref "=:" words cword
+        else
+            words=("${COMP_WORDS[@]}")
+            cword=${COMP_CWORD}
+        fi
         local IFS=$'\n'
-        response=$(env COMP_POINT=$COMP_POINT COMP_WORDS="${words[*]}" COMP_CWORD="$cword" %(complete_var)s=bash_complete $1)
+        response=$(COMP_POINT=$COMP_POINT COMP_WORDS="${words[*]}" COMP_CWORD="$cword" %(complete_var)s=bash_complete $1)
         for completion in $response; do
             IFS=',' read type value <<< "$completion"
             case $type in
             dir) COMPREPLY=(); compopt -o dirnames; ;;
             file) COMPREPLY=(); compopt -o default; ;;
             plain) COMPREPLY+=("$value"); ;;
             nospace) compopt -o nospace; ;;
@@ -44,19 +48,17 @@
         complete -o nosort -F %(complete_func)s %(prog_name)s
     }
     %(complete_func)s_setup;
 """
 
 
 @click.group(
-    "nomadt",
-    help="Nomad tools - collection of tools I find usefull when working with HashiCorp Nomad.",
-    epilog="""
-Written by Kamil Cukrowski 2023. Licensed under GNU GPL version or later.
-""",
+    "nomadtools",
+    help="Collection of useful tools for HashiCorp Nomad.",
+    epilog=EPILOG,
 )
 @namespace_option()
 @common_options()
 @main_options()
 def cli():
     pass
```

### Comparing `nomad_tools-0.3.0/src/nomad_tools/exit_on_thread_exception.py` & `nomad_tools-0.3.1/src/nomad_tools/exit_on_thread_exception.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/flagdebug.py` & `nomad_tools-0.3.1/src/nomad_tools/flagdebug.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_cp.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_cp.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_dockers.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_dockers.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_downloadrelease.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_downloadrelease.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/script.sh` & `nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/script.sh`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/waiter.sh` & `nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/waiter.sh`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_port.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_port.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_smart_start_job.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_smart_start_job.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_taskexec.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_taskexec.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_vardir.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_vardir.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomad_watch.py` & `nomad_tools-0.3.1/src/nomad_tools/nomad_watch.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomaddbjob.py` & `nomad_tools-0.3.1/src/nomad_tools/nomaddbjob.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomadlib/_generator.py` & `nomad_tools-0.3.1/src/nomad_tools/nomadlib/_generator.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomadlib/connection.py` & `nomad_tools-0.3.1/src/nomad_tools/nomadlib/connection.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomadlib/datadict.py` & `nomad_tools-0.3.1/src/nomad_tools/nomadlib/datadict.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomadlib/tools.py` & `nomad_tools-0.3.1/src/nomad_tools/nomadlib/tools.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomadlib/types.py` & `nomad_tools-0.3.1/src/nomad_tools/nomadlib/types.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/nomadt_completion.sh` & `nomad_tools-0.3.1/src/nomad_tools/nomadt_completion.sh`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/taskexec.py` & `nomad_tools-0.3.1/src/nomad_tools/taskexec.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools/transferstats.py` & `nomad_tools-0.3.1/src/nomad_tools/transferstats.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/src/nomad_tools.egg-info/PKG-INFO` & `nomad_tools-0.3.1/src/nomad_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: nomad-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
 Author: Kamil Cukrowski
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
 Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
 Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: requests==2.31.0
-Requires-Dist: typing_extensions==4.7.1
-Requires-Dist: websocket-client==1.6.1
-Requires-Dist: clickdc==0.0.5
-Requires-Dist: clickforward==0.0.1
-Requires-Dist: python-dotenv==0.21.1
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: requests>=2.31.0
+Requires-Dist: typing_extensions>=4.7.1
+Requires-Dist: websocket-client>=1.6.1
+Requires-Dist: clickdc>=0.0.5
+Requires-Dist: clickforward>=0.0.1
+Requires-Dist: python-dotenv>=0.21.1
 Requires-Dist: packaging>=16.1
+Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: tomli==2.0.1; extra == "test"
 Requires-Dist: pytest==7.4.4; extra == "test"
 Requires-Dist: pytest-xdist==3.5.0; extra == "test"
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
 
 # nomadtools
@@ -34,14 +35,15 @@
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
     * [Shell completion](#shell-completion)
 * [Usage](#usage)
     * [watch](#watch)
     * [go](#go)
+    * [constrainteval](#constrainteval)
     * [port](#port)
     * [vardir](#vardir)
     * [cp](#cp)
     * [gitlab-runner](#gitlab-runner)
     * [nomad-dockers](#nomad-dockers)
     * [downloadrelease](#downloadrelease)
     * [import nomad_tools](#import-nomad_tools)
@@ -136,14 +138,34 @@
 Executing busybox-1.36.1-r15.trigger
 OK: 10 MiB in 19 packages
 INFO:nomad_tools.nomad_watch:Purging job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587
 INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default purged with no active allocations, evaluations nor deployments. Exiting.
 INFO:nomad_tools.nomad_watch:Single task exited with 0 exit status. Exit code is 0.
 ```
 
+## constrainteval
+
+Evaluate a constraint and show all nodes that match the constraint. In
+addition to the node names, it also shows all attributes referenced while
+evaluating the constraint given on command line arguments. Useful for
+searching for which hosts contain what value of a attribute.
+
+```
+$ nomadtools constrainteval attr.cpu.arch is_set
+name   attr.cpu.arch
+-----  ---------------
+node1  amd64
+node2  amd64
+```
+
+This mode uses a cache in `~/.cache/nomadtools/nodes.json` for caching all the
+attributes of nodes downloaded from Nomad. This is used to speed up. The
+program needs to make one query for every single node in Nomad, which for a
+lot of nodes is costly.
+
 ## port
 
 Prints out the ports allocated for a particular Nomad job or
 allocation. It is meant to mimic `docker port` command.
 
 ```
 $ nomadtools port httpd
```

### Comparing `nomad_tools-0.3.0/src/nomad_tools.egg-info/SOURCES.txt` & `nomad_tools-0.3.1/src/nomad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/tests/test_nomad_cp_complete.py` & `nomad_tools-0.3.1/tests/test_nomad_cp_complete.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/tests/test_taskexec_transfer_stats.py` & `nomad_tools-0.3.1/tests/test_taskexec_transfer_stats.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.0/tests/testlib.py` & `nomad_tools-0.3.1/tests/testlib.py`

 * *Files identical despite different names*

