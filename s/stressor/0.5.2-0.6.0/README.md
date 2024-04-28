# Comparing `tmp/stressor-0.5.2.tar.gz` & `tmp/stressor-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stressor-0.5.2.tar", last modified: Sat Feb 18 14:39:53 2023, max compression
+gzip compressed data, was "stressor-0.6.0.tar", last modified: Sun Apr 28 09:45:37 2024, max compression
```

## Comparing `stressor-0.5.2.tar` & `stressor-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.422273 stressor-0.5.2/
--rw-rw-rw-   0        0        0      754 2021-12-11 16:36:36.000000 stressor-0.5.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1099 2023-02-18 14:19:24.000000 stressor-0.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5150 2023-02-18 14:39:53.422273 stressor-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3328 2022-10-10 13:25:40.000000 stressor-0.5.2/README.md
--rw-rw-rw-   0        0        0      567 2021-12-11 16:36:36.000000 stressor-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0     2678 2023-02-18 14:39:53.422273 stressor-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      177 2022-07-18 15:04:57.000000 stressor-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.390977 stressor-0.5.2/stressor/
--rw-rw-rw-   0        0        0      509 2023-02-18 14:39:50.000000 stressor-0.5.2/stressor/__init__.py
--rw-rw-rw-   0        0        0     1358 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/cli_common.py
--rw-rw-rw-   0        0        0    20054 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/config_manager.py
--rw-rw-rw-   0        0        0     5479 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/context_stack.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.390977 stressor-0.5.2/stressor/convert/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:36:36.000000 stressor-0.5.2/stressor/convert/__init__.py
--rw-rw-rw-   0        0        0    17511 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/convert/har_converter.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.390977 stressor-0.5.2/stressor/monitor/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:36:36.000000 stressor-0.5.2/stressor/monitor/__init__.py
--rw-rw-rw-   0        0        0     4470 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/monitor/server.py
--rw-rw-rw-   0        0        0     6496 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/plugin_manager.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.390977 stressor-0.5.2/stressor/plugins/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:36:36.000000 stressor-0.5.2/stressor/plugins/__init__.py
--rw-rw-rw-   0        0        0    12732 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/plugins/base.py
--rw-rw-rw-   0        0        0     7479 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/plugins/common.py
--rw-rw-rw-   0        0        0    13532 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/plugins/http_activities.py
--rw-rw-rw-   0        0        0     5636 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/plugins/script_activities.py
--rw-rw-rw-   0        0        0    17151 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/run_manager.py
--rw-rw-rw-   0        0        0    20187 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/session_manager.py
--rw-rw-rw-   0        0        0    15704 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/statistic_manager.py
--rw-rw-rw-   0        0        0     8095 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/stressor_cli.py
--rw-rw-rw-   0        0        0    28035 2023-02-18 14:19:24.000000 stressor-0.5.2/stressor/util.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.406614 stressor-0.5.2/stressor.egg-info/
--rw-rw-rw-   0        0        0     5150 2023-02-18 14:39:53.000000 stressor-0.5.2/stressor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1560 2023-02-18 14:39:53.000000 stressor-0.5.2/stressor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 14:39:53.000000 stressor-0.5.2/stressor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-02-18 14:39:53.000000 stressor-0.5.2/stressor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-03-24 17:33:07.000000 stressor-0.5.2/stressor.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2023-02-18 14:39:53.000000 stressor-0.5.2/stressor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-18 14:39:53.000000 stressor-0.5.2/stressor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-18 14:39:53.406614 stressor-0.5.2/tests/
--rw-rw-rw-   0        0        0     3568 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_config_manager.py
--rw-rw-rw-   0        0        0     1876 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_context_stack.py
--rw-rw-rw-   0        0        0     2247 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_convert.py
--rw-rw-rw-   0        0        0      561 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_plugin_manager.py
--rw-rw-rw-   0        0        0     2554 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_run_manager.py
--rw-rw-rw-   0        0        0     1932 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_script_activities.py
--rw-rw-rw-   0        0        0     9278 2023-02-18 14:19:24.000000 stressor-0.5.2/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.464126 stressor-0.6.0/
+-rw-rw-rw-   0        0        0     1124 2024-04-27 14:13:33.000000 stressor-0.6.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1099 2024-04-28 09:35:46.000000 stressor-0.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5233 2024-04-28 09:45:37.464126 stressor-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3312 2024-04-28 09:31:14.000000 stressor-0.6.0/README.md
+-rw-rw-rw-   0        0        0     1195 2024-04-27 15:02:56.000000 stressor-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     2639 2024-04-28 09:45:37.464126 stressor-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      177 2022-07-18 15:04:57.000000 stressor-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.431261 stressor-0.6.0/stressor/
+-rw-rw-rw-   0        0        0      486 2024-04-28 09:45:35.000000 stressor-0.6.0/stressor/__init__.py
+-rw-rw-rw-   0        0        0     1333 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/cli_common.py
+-rw-rw-rw-   0        0        0    19560 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/config_manager.py
+-rw-rw-rw-   0        0        0     5444 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/context_stack.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.446917 stressor-0.6.0/stressor/convert/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:36:36.000000 stressor-0.6.0/stressor/convert/__init__.py
+-rw-rw-rw-   0        0        0    17083 2024-04-28 09:38:02.000000 stressor-0.6.0/stressor/convert/har_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.446917 stressor-0.6.0/stressor/monitor/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:36:36.000000 stressor-0.6.0/stressor/monitor/__init__.py
+-rw-rw-rw-   0        0        0     4432 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/monitor/server.py
+-rw-rw-rw-   0        0        0     6273 2024-04-28 09:35:47.000000 stressor-0.6.0/stressor/plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.446917 stressor-0.6.0/stressor/plugins/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:36:36.000000 stressor-0.6.0/stressor/plugins/__init__.py
+-rw-rw-rw-   0        0        0    12627 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/plugins/base.py
+-rw-rw-rw-   0        0        0     7442 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/plugins/common.py
+-rw-rw-rw-   0        0        0    13137 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/plugins/http_activities.py
+-rw-rw-rw-   0        0        0     5377 2024-04-28 09:35:48.000000 stressor-0.6.0/stressor/plugins/script_activities.py
+-rw-rw-rw-   0        0        0    17043 2024-04-28 09:35:47.000000 stressor-0.6.0/stressor/run_manager.py
+-rw-rw-rw-   0        0        0    19626 2024-04-28 09:35:47.000000 stressor-0.6.0/stressor/session_manager.py
+-rw-rw-rw-   0        0        0    15653 2024-04-28 09:35:47.000000 stressor-0.6.0/stressor/statistic_manager.py
+-rw-rw-rw-   0        0        0     8063 2024-04-28 09:35:47.000000 stressor-0.6.0/stressor/stressor_cli.py
+-rw-rw-rw-   0        0        0    27430 2024-04-28 09:35:47.000000 stressor-0.6.0/stressor/util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.464126 stressor-0.6.0/stressor.egg-info/
+-rw-rw-rw-   0        0        0     5233 2024-04-28 09:45:37.000000 stressor-0.6.0/stressor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2024-04-28 09:45:37.000000 stressor-0.6.0/stressor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:45:37.000000 stressor-0.6.0/stressor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-28 09:45:37.000000 stressor-0.6.0/stressor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-03-24 17:33:07.000000 stressor-0.6.0/stressor.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       53 2024-04-28 09:45:37.000000 stressor-0.6.0/stressor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 09:45:37.000000 stressor-0.6.0/stressor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:45:37.464126 stressor-0.6.0/tests/
+-rw-rw-rw-   0        0        0     3543 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_config_manager.py
+-rw-rw-rw-   0        0        0     1843 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_context_stack.py
+-rw-rw-rw-   0        0        0     2216 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_convert.py
+-rw-rw-rw-   0        0        0      536 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_plugin_manager.py
+-rw-rw-rw-   0        0        0     2571 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_run_manager.py
+-rw-rw-rw-   0        0        0     1925 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_script_activities.py
+-rw-rw-rw-   0        0        0     9257 2024-04-28 09:35:47.000000 stressor-0.6.0/tests/test_util.py
```

### Comparing `stressor-0.5.2/LICENSE.txt` & `stressor-0.6.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) 2020-2023 Martin Wendt
+Copyright (c) 2020-2024 Martin Wendt
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `stressor-0.5.2/PKG-INFO` & `stressor-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stressor
-Version: 0.5.2
+Version: 0.6.0
 Summary: Stress-test your web app
 Home-page: https://github.com/mar10/stressor
 Author: Martin Wendt
 Author-email: stressor@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: stressor@wwwendt.de
 License: MIT
@@ -19,97 +19,103 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: fabulist
+Requires-Dist: lxml
+Requires-Dist: python-dateutil
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: snazzy
 
 # ![logo](https://raw.githubusercontent.com/mar10/stressor/master/stressor/monitor/htdocs/stressor_48x48.png) stressor
-[![Build Status](https://travis-ci.com/mar10/stressor.svg?branch=master)](https://app.travis-ci.com/github/mar10/stressor)
+
+[![Tests](https://github.com/mar10/stressor/actions/workflows/tests.yml/badge.svg)](https://github.com/mar10/stressor/actions/workflows/tests.yml)
 [![Latest Version](https://img.shields.io/pypi/v/stressor.svg)](https://pypi.python.org/pypi/stressor/)
 [![License](https://img.shields.io/pypi/l/stressor.svg)](https://github.com/mar10/stressor/blob/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/stressor/badge/?version=latest)](http://stressor.readthedocs.io/)
-[![Coverage Status](https://coveralls.io/repos/github/mar10/stressor/badge.svg?branch=master)](https://coveralls.io/github/mar10/stressor?branch=master)
+[![codecov](https://codecov.io/github/mar10/stressor/graph/badge.svg?token=WW9WQ0R0JL)](https://codecov.io/github/mar10/stressor)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: stressor](https://img.shields.io/badge/StackOverflow-stressor-blue.svg)](https://stackoverflow.com/questions/tagged/stressor)
 
 > Stress-test your web app.
 
-*Stressor* is a tool, that runs a sequence of activities in one or more
+_Stressor_ is a tool, that runs a sequence of activities in one or more
 parallel sessions.
 The most common use case is to run a test script with HTTP commands
 against a web server, simulating a bunch of parallel user sessions.
 As a result we get metrics about reponse times, failures, resource usage,
 etc.
 
 Stressor can be used for testing, benchmarking, load testing, or to generate
 test data.
 Stressor comes with prebuilt activities for HTTP-request and more, and can be
 extended by custom activity-plugins.
 
 Test scripts can be defined as text files, using a special syntax, that is then
 executed by the `stressor` command line tool.
 Stressor is also an Open Source Python library that can be included into your
-own projects. This allows to define test *scenarios* programmtically.
-
+own projects. This allows to define test _scenarios_ programmtically.
 
 ## Quickstart
 
-1. Install *stressor* ([details](https://stressor.readthedocs.io/en/latest/installation.html))
+1. Install _stressor_ ([details](https://stressor.readthedocs.io/en/latest/installation.html))
 
 2. Create a new scenario folder. For example:
 
-    ```bash
-    $ stressor init ./scenario_1
-    ```
-
-    or alternatively import an existing HAR file as a starting point
-    ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html#importing-har-files)):
-
-    ```bash
-    $ stressor init ./scenario_1 --convert /path/to/output.har
-    ```
+   ```bash
+   $ stressor init ./scenario_1
+   ```
+
+   or alternatively import an existing HAR file as a starting point
+   ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html#importing-har-files)):
+
+   ```bash
+   $ stressor init ./scenario_1 --convert /path/to/output.har
+   ```
 
-3. Edit the scripts as needed (*users.yaml*, *main_sequence.yaml*, *scenario.yaml*)
-  ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html))
+3. Edit the scripts as needed (_users.yaml_, _main_sequence.yaml_, _scenario.yaml_)
+   ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html))
 
 4. Run the script:
 
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml
-    ```
-
-    Use the `--monitor` option to view the progress in a separate window:
-
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml --monitor
-    ```
-
-    Use the `--log` argument to write output to a file or folder:
-
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml --no-color --log .
-    ```
-    (Hit <kbd>Ctrl</kbd>+<kbd>C</kbd> to stop.)
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml
+   ```
+
+   Use the `--monitor` option to view the progress in a separate window:
+
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml --monitor
+   ```
+
+   Use the `--log` argument to write output to a file or folder:
+
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml --no-color --log .
+   ```
+
+   (Hit <kbd>Ctrl</kbd>+<kbd>C</kbd> to stop.)
 
 5. [Read The Docs](https://stressor.readthedocs.io/en/latest/ug_tutorial.html)
    for details.
 
 <img src="https://stressor.readthedocs.io/en/latest/_images/summary.png">
 
 <img src="https://stressor.readthedocs.io/en/latest/_images/teaser.png">
```

### Comparing `stressor-0.5.2/README.md` & `stressor-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 # ![logo](https://raw.githubusercontent.com/mar10/stressor/master/stressor/monitor/htdocs/stressor_48x48.png) stressor
-[![Build Status](https://travis-ci.com/mar10/stressor.svg?branch=master)](https://app.travis-ci.com/github/mar10/stressor)
+
+[![Tests](https://github.com/mar10/stressor/actions/workflows/tests.yml/badge.svg)](https://github.com/mar10/stressor/actions/workflows/tests.yml)
 [![Latest Version](https://img.shields.io/pypi/v/stressor.svg)](https://pypi.python.org/pypi/stressor/)
 [![License](https://img.shields.io/pypi/l/stressor.svg)](https://github.com/mar10/stressor/blob/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/stressor/badge/?version=latest)](http://stressor.readthedocs.io/)
-[![Coverage Status](https://coveralls.io/repos/github/mar10/stressor/badge.svg?branch=master)](https://coveralls.io/github/mar10/stressor?branch=master)
+[![codecov](https://codecov.io/github/mar10/stressor/graph/badge.svg?token=WW9WQ0R0JL)](https://codecov.io/github/mar10/stressor)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: stressor](https://img.shields.io/badge/StackOverflow-stressor-blue.svg)](https://stackoverflow.com/questions/tagged/stressor)
 
 > Stress-test your web app.
 
-*Stressor* is a tool, that runs a sequence of activities in one or more
+_Stressor_ is a tool, that runs a sequence of activities in one or more
 parallel sessions.
 The most common use case is to run a test script with HTTP commands
 against a web server, simulating a bunch of parallel user sessions.
 As a result we get metrics about reponse times, failures, resource usage,
 etc.
 
 Stressor can be used for testing, benchmarking, load testing, or to generate
 test data.
 Stressor comes with prebuilt activities for HTTP-request and more, and can be
 extended by custom activity-plugins.
 
 Test scripts can be defined as text files, using a special syntax, that is then
 executed by the `stressor` command line tool.
 Stressor is also an Open Source Python library that can be included into your
-own projects. This allows to define test *scenarios* programmtically.
-
+own projects. This allows to define test _scenarios_ programmtically.
 
 ## Quickstart
 
-1. Install *stressor* ([details](https://stressor.readthedocs.io/en/latest/installation.html))
+1. Install _stressor_ ([details](https://stressor.readthedocs.io/en/latest/installation.html))
 
 2. Create a new scenario folder. For example:
 
-    ```bash
-    $ stressor init ./scenario_1
-    ```
-
-    or alternatively import an existing HAR file as a starting point
-    ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html#importing-har-files)):
-
-    ```bash
-    $ stressor init ./scenario_1 --convert /path/to/output.har
-    ```
+   ```bash
+   $ stressor init ./scenario_1
+   ```
+
+   or alternatively import an existing HAR file as a starting point
+   ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html#importing-har-files)):
+
+   ```bash
+   $ stressor init ./scenario_1 --convert /path/to/output.har
+   ```
 
-3. Edit the scripts as needed (*users.yaml*, *main_sequence.yaml*, *scenario.yaml*)
-  ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html))
+3. Edit the scripts as needed (_users.yaml_, _main_sequence.yaml_, _scenario.yaml_)
+   ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html))
 
 4. Run the script:
 
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml
-    ```
-
-    Use the `--monitor` option to view the progress in a separate window:
-
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml --monitor
-    ```
-
-    Use the `--log` argument to write output to a file or folder:
-
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml --no-color --log .
-    ```
-    (Hit <kbd>Ctrl</kbd>+<kbd>C</kbd> to stop.)
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml
+   ```
+
+   Use the `--monitor` option to view the progress in a separate window:
+
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml --monitor
+   ```
+
+   Use the `--log` argument to write output to a file or folder:
+
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml --no-color --log .
+   ```
+
+   (Hit <kbd>Ctrl</kbd>+<kbd>C</kbd> to stop.)
 
 5. [Read The Docs](https://stressor.readthedocs.io/en/latest/ug_tutorial.html)
    for details.
 
 <img src="https://stressor.readthedocs.io/en/latest/_images/summary.png">
 
 <img src="https://stressor.readthedocs.io/en/latest/_images/teaser.png">
```

### Comparing `stressor-0.5.2/setup.cfg` & `stressor-0.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -62,107 +62,104 @@
 000003d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 000003e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 000003f0: 2033 0d0a 0950 726f 6772 616d 6d69 6e67   3...Programming
 00000400: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
 00000410: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
 00000420: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
 00000430: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000440: 6e20 3a3a 2033 2e37 0d0a 0950 726f 6772  n :: 3.7...Progr
+00000440: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
 00000450: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000460: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000470: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000480: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000490: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
-000004a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000004b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000004c0: 300d 0a09 5072 6f67 7261 6d6d 696e 6720  0...Programming 
-000004d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000004e0: 6f6e 203a 3a20 332e 3131 0d0a 0954 6f70  on :: 3.11...Top
-000004f0: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000500: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
-00000510: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000520: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
-00000530: 6e61 6d69 6320 436f 6e74 656e 740d 0a09  namic Content...
-00000540: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
-00000550: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
-00000560: 2048 5454 5020 5365 7276 6572 730d 0a09   HTTP Servers...
-00000570: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
-00000580: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
-00000590: 204c 6962 7261 7269 6573 203a 3a20 5079   Libraries :: Py
-000005a0: 7468 6f6e 204d 6f64 756c 6573 0d0a 0954  thon Modules...T
-000005b0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-000005c0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-000005d0: 5175 616c 6974 7920 4173 7375 7261 6e63  Quality Assuranc
-000005e0: 650d 0a09 546f 7069 6320 3a3a 2053 6f66  e...Topic :: Sof
-000005f0: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000600: 7420 3a3a 2054 6573 7469 6e67 0d0a 0954  t :: Testing...T
-00000610: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-00000620: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-00000630: 5465 7374 696e 6720 3a3a 2054 7261 6666  Testing :: Traff
-00000640: 6963 2047 656e 6572 6174 696f 6e0d 0a0d  ic Generation...
-00000650: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000660: 6167 655f 6469 7220 3d20 0d0a 093d 202e  age_dir = ...= .
-00000670: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000680: 643a 0d0a 7a69 705f 7361 6665 203d 2046  d:..zip_safe = F
-00000690: 616c 7365 0d0a 696e 7374 616c 6c5f 7265  alse..install_re
-000006a0: 7175 6972 6573 203d 200d 0a09 6661 6275  quires = ...fabu
-000006b0: 6c69 7374 0d0a 096c 786d 6c0d 0a09 7079  list...lxml...py
-000006c0: 7468 6f6e 2d64 6174 6575 7469 6c0d 0a09  thon-dateutil...
-000006d0: 5079 5941 4d4c 0d0a 0972 6571 7565 7374  PyYAML...request
-000006e0: 730d 0a09 736e 617a 7a79 0d0a 0d0a 5b6f  s...snazzy....[o
-000006f0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000700: 6669 6e64 5d0d 0a77 6865 7265 203d 202e  find]..where = .
-00000710: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000720: 655f 6461 7461 203d 2054 7275 650d 0a65  e_data = True..e
-00000730: 7863 6c75 6465 203d 200d 0a09 7465 7374  xclude = ...test
-00000740: 730d 0a0d 0a5b 6f70 7469 6f6e 732e 6461  s....[options.da
-00000750: 7461 5f66 696c 6573 5d0d 0a2e 203d 2043  ta_files]... = C
-00000760: 4841 4e47 454c 4f47 2e6d 640d 0a0d 0a5b  HANGELOG.md....[
-00000770: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000780: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-00000790: 6372 6970 7473 203d 200d 0a09 7374 7265  cripts = ...stre
-000007a0: 7373 6f72 203d 2073 7472 6573 736f 722e  ssor = stressor.
-000007b0: 7374 7265 7373 6f72 5f63 6c69 3a72 756e  stressor_cli:run
-000007c0: 0d0a 0d0a 5b62 6469 7374 5f77 6865 656c  ....[bdist_wheel
-000007d0: 5d0d 0a0d 0a5b 636f 7665 7261 6765 3a72  ]....[coverage:r
-000007e0: 756e 5d0d 0a6f 6d69 7420 3d20 0d0a 0974  un]..omit = ...t
-000007f0: 6573 7473 2f2a 0d0a 0973 7472 6573 736f  ests/*...stresso
-00000800: 722f 7374 7265 7373 6f72 5f63 6c69 2e70  r/stressor_cli.p
-00000810: 790d 0a09 7374 7265 7373 6f72 2f63 6c69  y...stressor/cli
-00000820: 5f63 6f6d 6d6f 6e2e 7079 0d0a 0973 7472  _common.py...str
-00000830: 6573 736f 722f 6d6f 6e69 746f 722f 2a0d  essor/monitor/*.
-00000840: 0a0d 0a5b 636f 7665 7261 6765 3a72 6570  ...[coverage:rep
-00000850: 6f72 745d 0d0a 7072 6563 6973 696f 6e20  ort]..precision 
-00000860: 3d20 310d 0a73 6f72 7420 3d20 4e61 6d65  = 1..sort = Name
-00000870: 0d0a 6578 636c 7564 655f 6c69 6e65 7320  ..exclude_lines 
-00000880: 3d20 0d0a 0970 7261 676d 613a 206e 6f20  = ...pragma: no 
-00000890: 636f 7665 720d 0a09 6966 205f 5f6e 616d  cover...if __nam
-000008a0: 655f 5f20 3d3d 202e 5f5f 6d61 696e 5f5f  e__ == .__main__
-000008b0: 2e3a 0d0a 0d0a 5b63 6f76 6572 6167 653a  .:....[coverage:
-000008c0: 6874 6d6c 5d0d 0a64 6972 6563 746f 7279  html]..directory
-000008d0: 203d 2062 7569 6c64 2f63 6f76 6572 6167   = build/coverag
-000008e0: 650d 0a0d 0a5b 746f 6f6c 3a70 7974 6573  e....[tool:pytes
-000008f0: 745d 0d0a 6a75 6e69 745f 6661 6d69 6c79  t]..junit_family
-00000900: 203d 206c 6567 6163 790d 0a0d 0a5b 666c   = legacy....[fl
-00000910: 616b 6538 5d0d 0a65 6e61 626c 652d 6578  ake8]..enable-ex
-00000920: 7465 6e73 696f 6e73 203d 2047 0d0a 6578  tensions = G..ex
-00000930: 636c 7564 6520 3d20 0d0a 095f 5f70 7963  clude = ...__pyc
-00000940: 6163 6865 5f5f 2c0d 0a09 2e63 6163 6865  ache__,....cache
-00000950: 2c0d 0a09 2e65 6767 732c 0d0a 092e 6769  ,....eggs,....gi
-00000960: 742c 0d0a 092e 746f 782c 0d0a 092e 7673  t,....tox,....vs
-00000970: 636f 6465 2c0d 0a09 6275 696c 642c 0d0a  code,...build,..
-00000980: 0964 6973 742c 0d0a 0964 6f63 730d 0a6d  .dist,...docs..m
-00000990: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-000009a0: 2039 390d 0a69 676e 6f72 6520 3d20 4532   99..ignore = E2
-000009b0: 3033 2c20 4535 3031 2c20 5735 3033 2c20  03, E501, W503, 
-000009c0: 5031 3031 0d0a 646f 6373 7472 696e 672d  P101..docstring-
-000009d0: 636f 6e76 656e 7469 6f6e 203d 2061 6c6c  convention = all
-000009e0: 2020 2320 676f 6f67 6c65 3f0d 0a69 6e6c    # google?..inl
-000009f0: 696e 652d 7175 6f74 6573 203d 2064 6f75  ine-quotes = dou
-00000a00: 626c 650d 0a6d 756c 7469 6c69 6e65 2d71  ble..multiline-q
-00000a10: 756f 7465 7320 3d20 2222 220d 0a64 6f63  uotes = """..doc
-00000a20: 7374 7269 6e67 2d71 756f 7465 7320 3d20  string-quotes = 
-00000a30: 2222 220d 0a61 766f 6964 2d65 7363 6170  """..avoid-escap
-00000a40: 6520 3d20 5472 7565 0d0a 0d0a 5b65 6767  e = True....[egg
-00000a50: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000a60: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000a70: 2030 0d0a 0d0a                            0....
+00000460: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000470: 300d 0a09 5072 6f67 7261 6d6d 696e 6720  0...Programming 
+00000480: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000490: 6f6e 203a 3a20 332e 3131 0d0a 0950 726f  on :: 3.11...Pro
+000004a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000004b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000004c0: 2e31 320d 0a09 546f 7069 6320 3a3a 2049  .12...Topic :: I
+000004d0: 6e74 6572 6e65 7420 3a3a 2057 5757 2f48  nternet :: WWW/H
+000004e0: 5454 500d 0a09 546f 7069 6320 3a3a 2049  TTP...Topic :: I
+000004f0: 6e74 6572 6e65 7420 3a3a 2057 5757 2f48  nternet :: WWW/H
+00000500: 5454 5020 3a3a 2044 796e 616d 6963 2043  TTP :: Dynamic C
+00000510: 6f6e 7465 6e74 0d0a 0954 6f70 6963 203a  ontent...Topic :
+00000520: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+00000530: 572f 4854 5450 203a 3a20 4854 5450 2053  W/HTTP :: HTTP S
+00000540: 6572 7665 7273 0d0a 0954 6f70 6963 203a  ervers...Topic :
+00000550: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000560: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+00000570: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
+00000580: 6475 6c65 730d 0a09 546f 7069 6320 3a3a  dules...Topic ::
+00000590: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+000005a0: 706d 656e 7420 3a3a 2051 7561 6c69 7479  pment :: Quality
+000005b0: 2041 7373 7572 616e 6365 0d0a 0954 6f70   Assurance...Top
+000005c0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+000005d0: 6576 656c 6f70 6d65 6e74 203a 3a20 5465  evelopment :: Te
+000005e0: 7374 696e 670d 0a09 546f 7069 6320 3a3a  sting...Topic ::
+000005f0: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+00000600: 706d 656e 7420 3a3a 2054 6573 7469 6e67  pment :: Testing
+00000610: 203a 3a20 5472 6166 6669 6320 4765 6e65   :: Traffic Gene
+00000620: 7261 7469 6f6e 0d0a 0d0a 5b6f 7074 696f  ration....[optio
+00000630: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000640: 203d 200d 0a09 3d20 2e0d 0a70 6163 6b61   = ...= ...packa
+00000650: 6765 7320 3d20 6669 6e64 3a0d 0a7a 6970  ges = find:..zip
+00000660: 5f73 6166 6520 3d20 4661 6c73 650d 0a69  _safe = False..i
+00000670: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000680: 3d20 0d0a 0966 6162 756c 6973 740d 0a09  = ...fabulist...
+00000690: 6c78 6d6c 0d0a 0970 7974 686f 6e2d 6461  lxml...python-da
+000006a0: 7465 7574 696c 0d0a 0950 7959 414d 4c0d  teutil...PyYAML.
+000006b0: 0a09 7265 7175 6573 7473 0d0a 0973 6e61  ..requests...sna
+000006c0: 7a7a 790d 0a0d 0a5b 6f70 7469 6f6e 732e  zzy....[options.
+000006d0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000006e0: 7768 6572 6520 3d20 2e0d 0a69 6e63 6c75  where = ...inclu
+000006f0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000700: 3d20 5472 7565 0d0a 6578 636c 7564 6520  = True..exclude 
+00000710: 3d20 0d0a 0974 6573 7473 0d0a 0d0a 5b6f  = ...tests....[o
+00000720: 7074 696f 6e73 2e64 6174 615f 6669 6c65  ptions.data_file
+00000730: 735d 0d0a 2e20 3d20 4348 414e 4745 4c4f  s]... = CHANGELO
+00000740: 472e 6d64 0d0a 0d0a 5b6f 7074 696f 6e73  G.md....[options
+00000750: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
+00000760: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
+00000770: 3d20 0d0a 0973 7472 6573 736f 7220 3d20  = ...stressor = 
+00000780: 7374 7265 7373 6f72 2e73 7472 6573 736f  stressor.stresso
+00000790: 725f 636c 693a 7275 6e0d 0a0d 0a5b 6264  r_cli:run....[bd
+000007a0: 6973 745f 7768 6565 6c5d 0d0a 0d0a 5b63  ist_wheel]....[c
+000007b0: 6f76 6572 6167 653a 7275 6e5d 0d0a 6f6d  overage:run]..om
+000007c0: 6974 203d 200d 0a09 7465 7374 732f 2a0d  it = ...tests/*.
+000007d0: 0a09 7374 7265 7373 6f72 2f73 7472 6573  ..stressor/stres
+000007e0: 736f 725f 636c 692e 7079 0d0a 0973 7472  sor_cli.py...str
+000007f0: 6573 736f 722f 636c 695f 636f 6d6d 6f6e  essor/cli_common
+00000800: 2e70 790d 0a09 7374 7265 7373 6f72 2f6d  .py...stressor/m
+00000810: 6f6e 6974 6f72 2f2a 0d0a 0d0a 5b63 6f76  onitor/*....[cov
+00000820: 6572 6167 653a 7265 706f 7274 5d0d 0a70  erage:report]..p
+00000830: 7265 6369 7369 6f6e 203d 2031 0d0a 736f  recision = 1..so
+00000840: 7274 203d 204e 616d 650d 0a65 7863 6c75  rt = Name..exclu
+00000850: 6465 5f6c 696e 6573 203d 200d 0a09 7072  de_lines = ...pr
+00000860: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
+00000870: 0969 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00000880: 2e5f 5f6d 6169 6e5f 5f2e 3a0d 0a0d 0a5b  .__main__.:....[
+00000890: 636f 7665 7261 6765 3a68 746d 6c5d 0d0a  coverage:html]..
+000008a0: 6469 7265 6374 6f72 7920 3d20 6275 696c  directory = buil
+000008b0: 642f 636f 7665 7261 6765 0d0a 0d0a 5b74  d/coverage....[t
+000008c0: 6f6f 6c3a 7079 7465 7374 5d0d 0a6a 756e  ool:pytest]..jun
+000008d0: 6974 5f66 616d 696c 7920 3d20 6c65 6761  it_family = lega
+000008e0: 6379 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  cy....[flake8]..
+000008f0: 656e 6162 6c65 2d65 7874 656e 7369 6f6e  enable-extension
+00000900: 7320 3d20 470d 0a65 7863 6c75 6465 203d  s = G..exclude =
+00000910: 200d 0a09 5f5f 7079 6361 6368 655f 5f2c   ...__pycache__,
+00000920: 0d0a 092e 6361 6368 652c 0d0a 092e 6567  ....cache,....eg
+00000930: 6773 2c0d 0a09 2e67 6974 2c0d 0a09 2e74  gs,....git,....t
+00000940: 6f78 2c0d 0a09 2e76 7363 6f64 652c 0d0a  ox,....vscode,..
+00000950: 0962 7569 6c64 2c0d 0a09 6469 7374 2c0d  .build,...dist,.
+00000960: 0a09 646f 6373 0d0a 6d61 782d 6c69 6e65  ..docs..max-line
+00000970: 2d6c 656e 6774 6820 3d20 3939 0d0a 6967  -length = 99..ig
+00000980: 6e6f 7265 203d 2045 3230 332c 2045 3530  nore = E203, E50
+00000990: 312c 2057 3530 332c 2050 3130 310d 0a64  1, W503, P101..d
+000009a0: 6f63 7374 7269 6e67 2d63 6f6e 7665 6e74  ocstring-convent
+000009b0: 696f 6e20 3d20 616c 6c20 2023 2067 6f6f  ion = all  # goo
+000009c0: 676c 653f 0d0a 696e 6c69 6e65 2d71 756f  gle?..inline-quo
+000009d0: 7465 7320 3d20 646f 7562 6c65 0d0a 6d75  tes = double..mu
+000009e0: 6c74 696c 696e 652d 7175 6f74 6573 203d  ltiline-quotes =
+000009f0: 2022 2222 0d0a 646f 6373 7472 696e 672d   """..docstring-
+00000a00: 7175 6f74 6573 203d 2022 2222 0d0a 6176  quotes = """..av
+00000a10: 6f69 642d 6573 6361 7065 203d 2054 7275  oid-escape = Tru
+00000a20: 650d 0a0d 0a5b 6567 675f 696e 666f 5d0d  e....[egg_info].
+00000a30: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000a40: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `stressor-0.5.2/stressor/config_manager.py` & `stressor-0.6.0/stressor/config_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import os
 import re
 
 import yaml
@@ -64,17 +63,15 @@
                                 value = var_value
                                 break
                             # value contains a macro but also prefix or suffix.
                             # Cast macro-result to string and check for more macros
                             value = value.replace(macro, str(var_value))
                         except (KeyError, TypeError):
                             raise RuntimeError(
-                                "Error evaluating {}: '{}': '{}' not found in context (or is None).".format(
-                                    stack, org_value, var_name
-                                )
+                                f"Error evaluating {stack}: '{org_value}': '{var_name}' not found in context (or is None)."
                             )
                     if not found_one or not isinstance(value, str):
                         break
                 parent[parent_key] = value
         return value
 
     res = repl(value, context, None, None)
@@ -127,30 +124,28 @@
         """Return an absolute path, assuming relative to the original config file."""
         # TODO: check for invalid access (security risk!)
         assert_always(self.path, "`read()` must be called before")
         if not path.startswith("/"):
             path = os.path.join(self.root_folder, path)
         path = os.path.abspath(path)
         if check_root and not path.startswith(self.root_folder):
-            raise ValueError(
-                "Path must be in or below {}: {}".format(self.root_folder, path)
-            )
+            raise ValueError(f"Path must be in or below {self.root_folder}: {path}")
         if must_exist and not os.path.isfile(path):
-            raise ValueError("File not found: {}".format(path))
+            raise ValueError(f"File not found: {path}")
         return path
 
     def report_error(self, msg, level="error", exc=None, stack=None):
         """Called by activity and macro constructors to signal errors or warnings.
 
         The compiler also calls this when a constructor raises an exception.
         """
         check_arg(level, str, level in ("error", "warning"))
         path = stack if stack else str(self.stack)
 
-        hint = "{}: {}".format(path, msg)
+        hint = f"{path}: {msg}"
         if exc:
             logger.exception(hint)
         # No need to log, since self.results are also summarized later
         # elif level == "warning":
         #     logger.warning(hint)
         # else:
         #     logger.error(hint)
@@ -198,18 +193,18 @@
         check_arg(extra_config, dict, or_none=True)
         if not extra_config:
             return
         config = self.config
         context = self.context
         for k, v in extra_config.items():
             if not context_only:
-                logger.info("Set config.{}: {!r} -> {!r}".format(k, config.get(k), v))
+                logger.info(f"Set config.{k}: {config.get(k)!r} -> {v!r}")
                 config[k] = v
             else:
-                logger.info("Set context.{}: {!r} -> {!r}".format(k, context.get(k), v))
+                logger.info(f"Set context.{k}: {context.get(k)!r} -> {v!r}")
             context[k] = v
         return
 
     def validate_config(self, cfg=None):
         """
         Raises:
             ConfigurationError
@@ -226,35 +221,38 @@
                 self.report_error("Could not find expected entry", stack=key)
                 return False
 
             if o is None and None in types:
                 return True
             elif not isinstance(o, types):
                 self.report_error(
-                    "Expected type {}, but found {!r}".format(types, type(o)), stack=key
+                    f"Expected type {types}, but found {type(o)!r}", stack=key
                 )
                 return False
             return True
 
         sections = set(cfg.keys())
-        known_sections = set(
-            ("file_version", "config", "context", "sessions", "scenario", "sequences")
-        )
+        known_sections = {
+            "file_version",
+            "config",
+            "context",
+            "sessions",
+            "scenario",
+            "sequences",
+        }
 
         file_version = cfg.get("file_version", "")
         if not file_version.startswith("stressor#"):
             raise ConfigurationError(
                 "Not a `stressor` file (missing 'stressor#VERSION' tag)."
             )
         file_version = int(file_version.split("#", 1)[1])
         if file_version != self.FILE_VERSION:
             raise ConfigurationError(
-                "File version mismatch: expected {}, but found {}.".format(
-                    self.FILE_VERSION, file_version
-                )
+                f"File version mismatch: expected {self.FILE_VERSION}, but found {file_version}."
             )
 
         missing = known_sections.difference(sections)
         extra = sections.difference(known_sections)
         if extra or missing:
             raise ConfigurationError(
                 "Configuration file check failed:\n  missing sections: {}\n  invalid sections: {}".format(
@@ -262,32 +260,30 @@
                 )
             )
 
         if _check_type("config", dict):
             base_url = get_dict_attr(cfg, "config.base_url", None)
             if base_url and (not base_url.startswith("http") or "://" not in base_url):
                 self.report_error(
-                    "config.base_url must be an absolute URL ('http(s)://...'): {!r}".format(
-                        base_url
-                    ),
+                    f"config.base_url must be an absolute URL ('http(s)://...'): {base_url!r}",
                 )
 
         if _check_type("context", (dict, None)):
             pass
         if _check_type("sessions", dict):
             pass
 
         #   - sequences must be a dict of dicts.
         #     All entries must contain 'activity'
         #   - activity.assert_json must be a dict
         sequence_names = set()
         if _check_type("sequences", dict):
             for seq_name, act_list in cfg["sequences"].items():
                 sequence_names.add(seq_name)
-                stack = "sequences/{}".format(seq_name)
+                stack = f"sequences/{seq_name}"
                 if act_list is None:
                     act_list = []
                     cfg["sequences"][seq_name] = act_list
                     self.report_error(
                         "Ignored undefined list of activities",
                         level="warning",
                         stack=stack,
@@ -296,44 +292,42 @@
                 if not isinstance(act_list, list):
                     self.report_error(
                         "Expected list of activities",
                         stack=stack,
                     )
                 else:
                     for idx, act_def in enumerate(act_list):
-                        stack = "sequences/{}#{:02}".format(seq_name, idx)
+                        stack = f"sequences/{seq_name}#{idx:02}"
                         if not isinstance(act_def, dict):
                             self.report_error(
                                 "Expected dict with `activity` key",
                                 stack=stack,
                             )
                         else:
                             activity = act_def.get("activity")
                             if not isinstance(activity, ActivityBase):
                                 self.report_error(
                                     "`activity` must be an instance of ActivityBase "
-                                    "instance (found {!r})".format(activity),
+                                    f"instance (found {activity!r})",
                                     stack=stack,
                                 )
                             assert_match = act_def.get("assert_match")
                             if assert_match is not None:
                                 try:
                                     re.compile(assert_match)
                                 except re.error as e:
                                     self.report_error(
-                                        "Invalid regular expression: {}: {}".format(
-                                            assert_match, e
-                                        ),
+                                        f"Invalid regular expression: {assert_match}: {e}",
                                         stack=stack,
                                     )
 
         # Scenario list must contain 'sequence' keys and all sequences must exist
         if _check_type("scenario", list):
             for idx, seq_def in enumerate(cfg["scenario"]):
-                stack = ".scenario#{:02}".format(idx)
+                stack = f".scenario#{idx:02}"
                 if not isinstance(seq_def, dict) or "sequence" not in seq_def:
                     self.report_error(
                         "Expected dict with `sequence` key",
                         stack=stack,
                     )
                 elif seq_def["sequence"] not in sequence_names:
                     self.report_error(
@@ -385,29 +379,27 @@
                 has_match = False
                 for macro_cls in pm.macro_plugin_map.values():
                     try:
                         macro = macro_cls()
                         handled, res = macro.match_apply(self, parent, parent_key)
                         if handled:
                             has_match = True
-                            logger.debug("Eval {}: {} => {}".format(stack, value, res))
+                            logger.debug(f"Eval {stack}: {value} => {res}")
                             # Re-init `value` in case the macro replaced it
                             value = parent[parent_key]
                             break
                     except Exception as e:
-                        msg = "Could not evaluate macro {!r}".format(value)
+                        msg = f"Could not evaluate macro {value!r}"
                         self.report_error(msg, exc=e)
                         # raise ConfigurationError(
                         #     "Could not evaluate {!r} at {}: {}".format(value, stack, e)
                         # ) from e
 
                 if not has_match and GENERIC_MACRO_REX.match(value):
-                    msg = "Entry looks like a macro, but has no handler: '{}'".format(
-                        value
-                    )
+                    msg = f"Entry looks like a macro, but has no handler: '{value}'"
                     self.report_error(msg, level="warning")
 
             # Resolve lists and dicts recursively:
             if isinstance(value, dict):
                 # Macros may change the dictionary size, so iterate over a copy
                 for key, sub_val in tuple(value.items()):
                     self._compile(sub_val, value, key, stack)
@@ -428,17 +420,17 @@
                     # print(parent)
                     activity_inst = activity_cls(self, **parent)
                     parent[parent_key] = activity_inst
                     if stats:
                         stats.register_activity(activity_inst)
                 except ActivityCompileError as e:
                     # Don't pass exc to supress stack trace
-                    self.report_error("{}".format(e))
+                    self.report_error(f"{e}")
                 except Exception as e:
-                    msg = "Could not evaluate activity {!r}".format(value)
+                    msg = f"Could not evaluate activity {value!r}"
                     self.report_error(msg, exc=e)
                     # logger.error("{} {}: {}".format(stack, value, e))
 
         return
 
     def read(self, path, load_files=True):
         """Read a YAML file into ``self.config_all``.
@@ -450,24 +442,24 @@
 
         self.config_all = None
 
         if not path.lower().endswith(".yaml"):
             path += ".yaml"
         path = os.path.abspath(path)
         if not os.path.isfile(path):
-            raise ConfigurationError("File not found: {}".format(path))
+            raise ConfigurationError(f"File not found: {path}")
         self.path = path
         self.root_folder = os.path.dirname(path)
         self.name = os.path.splitext(os.path.basename(path))[0]
 
-        with open(path, "rt") as f:
+        with open(path) as f:
             try:
                 res = yaml.safe_load(f)
             except yaml.parser.ParserError as e:
-                raise ConfigurationError("Could not parse YAML: {}".format(e)) from None
+                raise ConfigurationError(f"Could not parse YAML: {e}") from None
 
         if not isinstance(res, dict) or not res.get("file_version", "").startswith(
             "stressor#"
         ):
             raise ConfigurationError(
                 "Not a `stressor` file (missing 'stressor#VERSION' tag)."
             )
```

### Comparing `stressor-0.5.2/stressor/context_stack.py` & `stressor-0.6.0/stressor/context_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 from copy import deepcopy
 
 from stressor.util import check_arg, get_dict_attr
 
@@ -115,15 +114,15 @@
         """
         Raises:
             RuntimeError if queue length exceeds ContextStack.MAX_DEPTH
         """
         check_arg(context, RunContext)
 
         if len(self.ctx_stack) >= self.MAX_DEPTH:
-            raise RuntimeError("Max depth exceeded ({})".format(self.MAX_DEPTH))
+            raise RuntimeError(f"Max depth exceeded ({self.MAX_DEPTH})")
         self.ctx_stack.append(context)
         return context
 
     def push(self, name, attributes=None, copy_data=False):
         """Push `name` to the stack and optionally update or copy context.
         Args:
             name (str):
@@ -155,15 +154,15 @@
             IndexError if offset is invalid
         """
         assert offset > 0
         ctx = self.ctx_stack[-offset]
         return ctx
 
     def path(self):
-        path = "/".join((ctx.name for ctx in self.ctx_stack))
+        path = "/".join(ctx.name for ctx in self.ctx_stack)
         return "/" + path
 
     def as_dict(self):
         """Return the current aggregated context."""
         return self.context
 
     def get_attr(self, key_path, context=None):
```

### Comparing `stressor-0.5.2/stressor/convert/har_converter.py` & `stressor-0.6.0/stressor/convert/har_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 https://w3c.github.io/web-performance/specs/HAR/Overview.html
 """
 import json
 import logging
 import os
@@ -22,15 +21,14 @@
     lstrip_string,
     shorten_string,
 )
 
 logger = logging.getLogger("stressor.har")
 
 EMPTY_TUPLE = tuple()
-PATTERN_TYPE = type(re.compile("foo"))  # 're.Pattern' requires Python 3.7+
 
 
 class HarConverter:
     """Convert HAR file to YAML scenario."""
 
     #: Defaults for optional `--opts` paramter.
     DEFAULT_OPTS = {
@@ -70,59 +68,56 @@
         self.base_url = None
         self.polling_requests = []
         self.static_resources = []
         pl = []
         for pattern in self.opts["statics_types"]:
             if isinstance(pattern, str):
                 pattern = re.compile(pattern, re.IGNORECASE)
-            assert isinstance(pattern, PATTERN_TYPE)
             pl.append(pattern)
         self.opts["statics_types"] = pl
 
     def run(self):
         har_path = self.opts.get("fspec")
         target_folder = self.opts.get("target_folder")
 
         if har_path is not None:
             har_path = os.path.abspath(har_path)
             if not os.path.isfile(har_path):
                 raise FileNotFoundError(har_path)
 
-            logger.info("Parsing {}...".format(har_path))
+            logger.info(f"Parsing {har_path}...")
             self._parse(har_path)
 
             self._postprocess()
 
         if target_folder is None:
             assert har_path
             name = os.path.splitext(os.path.basename(har_path))[0].strip(".")
-            target_folder = "./{}".format(name)
+            target_folder = f"./{name}"
         target_folder = os.path.abspath(target_folder)
         if not os.path.isdir(target_folder):
-            logger.info("Creating folder {}...".format(target_folder))
+            logger.info(f"Creating folder {target_folder}...")
             os.mkdir(target_folder)
 
         self._init_from_templates(target_folder)
 
         if har_path is not None:
             fspec = os.path.join(target_folder, "main_sequence.yaml")
             self._write_sequence(fspec)
         return True
 
     def _copy_template(self, tmpl_name, target_path, kwargs):
         if not self.opts["force"] and os.path.isfile(target_path):
-            raise RuntimeError(
-                "File exists (use --force to continue): {}".format(target_path)
-            )
+            raise RuntimeError(f"File exists (use --force to continue): {target_path}")
             # raise FileExistsError(target_path)
         tmpl_folder = os.path.dirname(__file__)
         src_path = os.path.join(tmpl_folder, tmpl_name)
-        tmpl = open(src_path, "rt", encoding=self.encoding).read()
+        tmpl = open(src_path, encoding=self.encoding).read()
         tmpl = tmpl.format(**kwargs)
-        logger.info("Writing {:,} bytes to {!r}...".format(len(tmpl), target_path))
+        logger.info(f"Writing {len(tmpl):,} bytes to {target_path!r}...")
         with open(target_path, "w") as fp:
             fp.write(tmpl)
         # print(tmpl)
         return
 
     def _init_from_templates(self, target_folder):
         ctx = {
@@ -166,15 +161,15 @@
         resp = har_entry["response"]
         content = resp.get("content")
 
         # Record the usage count of the scheme+netloc, so we can pick the best
         # base_url later:
         url = req["url"]
         parse_result = urlparse(url)
-        prefix = "{o.scheme}://{o.netloc}".format(o=parse_result)
+        prefix = f"{parse_result.scheme}://{parse_result.netloc}"
         self.prefix_counter[prefix] += 1
 
         entry_dt = har_entry["startedDateTime"]
         if not self.first_entry_dt:
             self.first_entry_dt = entry_dt
 
         entry = {
@@ -223,15 +218,15 @@
             headers = entry["headers"] = []
             for val in values:
                 headers.append((val["name"], val["value"]))
 
         self.entries.append(entry)
 
     def _parse(self, fspec):
-        with open(fspec, "r", encoding=self.encoding) as fp:
+        with open(fspec, encoding=self.encoding) as fp:
             har_data = json.load(fp)
         log = har_data["log"]
         assert len(har_data.keys()) == 1
 
         self.har_version = log["version"]
 
         creator = log["creator"]
@@ -247,27 +242,27 @@
         for entry in log["entries"]:
             self._add_entry(entry)
 
         # Sort entries
         # ("However the reader application should always make sure the array is sorted")
         self.entries.sort(key=itemgetter("start"))
 
-        logger.debug("HAR:\n{}".format(pformat(self.entries)))
+        logger.debug(f"HAR:\n{pformat(self.entries)}")
         # print("HAR:\n{}".format(pformat(self.entries)))
         return
 
     def _postprocess(self):
         # Figure out base_url
         base_url = self.opts.get("base_url")
         if base_url is True:
             # The most-used scheme+netloc is used as base_url
             # print(pformat(self.prefix_counter))
             base_url = self.prefix_counter.most_common(1)[0][0]
         self.base_url = base_url
-        logger.info("Using base_url {!r}.".format(base_url))
+        logger.info(f"Using base_url {base_url!r}.")
         # print(base_url)
 
         # Remove unwanted entries and strip base_url where possible
         el = []
         skip_ext = self.opts["skip_externals"]
         collate_max_len = self.opts["collate_max_len"]
         collate_max_duration = self.opts["collate_max_duration"]
@@ -295,15 +290,15 @@
             # Fix URL by removing the `base_url` prefix
             url = entry["url"]
             rel_url = lstrip_string(url, base_url, ignore_case=True)
             # The URL did not start with base_url, so it is 'external'
             is_external = rel_url is url
             if is_external:
                 if skip_ext:
-                    logger.warning("Skipping external URL: {}".format(url))
+                    logger.warning(f"Skipping external URL: {url}")
                     self.stats["external_urls"] += 1
                     skip = True
             else:
                 entry["url_org"] = url
                 entry["url"] = rel_url
 
             # Collate bursts of simple GET request to one single entry
@@ -355,35 +350,33 @@
         Args:
             lines (list):
             name (str):
             data (list): a 'params' list of {name: ..., value: ...} objects
         """
         assert isinstance(data, (list, tuple))
         used = set()
-        lines.append("  {}:\n".format(name))
+        lines.append(f"  {name}:\n")
         for p in data:
             # TODO: coerce value (which in HAR is always a string)
 
             # Convert [{name: ..., value: ...}, ...] syntax to dict
             # TODO: We do this, because activity code doesn not handle the
             #       tuple syntax yet. But we should fall back to tuples syntax
             #       if the list does contain duplicate names, instead of
             #       dicarding.
             name, value = p["name"], p["value"]
             # lines.append("    - ['{}', {}]\n".format(name, json.dumps(value)))
 
             if name in used:
-                logger.error(
-                    "Discarding multiple param name: {}: {}".format(name, value)
-                )
+                logger.error(f"Discarding multiple param name: {name}: {value}")
                 continue
             used.add(name)
             if not is_yaml_keyword(name):
                 name = '"' + name + '"'
-            lines.append("    {}: {}\n".format(name, json.dumps(value)))
+            lines.append(f"    {name}: {json.dumps(value)}\n")
 
         return
 
     def _write_entry(self, fp, entry):
         opts = self.opts
         activity = self.activity_map.get(entry["method"], "HTTPRequest")
         url_list = entry.get("url_list")
@@ -391,40 +384,40 @@
         if is_bucket:
             activity = "StaticRequests"
 
         lines = []
         if entry.get("comment"):
             lines.append("# {}\n".format(shorten_string(entry["comment"], 75)))
         if is_bucket:
-            lines.append("# Auto-collated {:,} GET requests\n".format(len(url_list)))
+            lines.append(f"# Auto-collated {len(url_list):,} GET requests\n")
         else:
             lines.append(
                 "# Response type: {!r}, size: {:,} bytes, time: {}\n".format(
                     entry.get("resp_type"),
                     entry.get("resp_size", -1),
                     format_elap(entry.get("elap"), high_prec=True),
                 )
             )
         if entry.get("resp_comment"):
             lines.append("# {}\n".format(shorten_string(entry["resp_comment"], 75)))
 
         url = entry["url"]
         expand_url_params = False
 
-        lines.append("- activity: {}\n".format(activity))
+        lines.append(f"- activity: {activity}\n")
         if is_bucket:
             lines.append("  thread_count: {}\n".format(opts["collate_thread_count"]))
             lines.append("  url_list:\n")
             for url in url_list:
-                lines.append("    - '{}'\n".format(url))
+                lines.append(f"    - '{url}'\n")
         else:
             if entry.get("query"):
                 expand_url_params = True
                 url = base_url(url)
-            lines.append("  url: '{}'\n".format(url))
+            lines.append(f"  url: '{url}'\n")
 
         if activity == "HTTPRequest":
             lines.append("  method: {}\n".format(entry["method"]))
 
         # TODO:
         # We have ?query also as part of the URL
         # if entry.get("query"):
@@ -437,34 +430,34 @@
 
         data = entry.get("data")
         if data:
             if isinstance(data, (list, tuple)):
                 # Must be a 'params' list of {name: ..., value: ...} objects
                 self._write_args(lines, "data", data)
             else:
-                assert type(data) is str
-                logger.warning("Expected list, but got text: {!r}".format(data))
-                lines.append("  data: {}\n".format(json.dumps(data)))
+                assert isinstance(data, str), data
+                logger.warning(f"Expected list, but got text: {data!r}")
+                lines.append(f"  data: {json.dumps(data)}\n")
 
         lines.append("\n")
         fp.writelines(lines)
 
     def _write_sequence(self, fspec):
-        logger.info("Writing activity sequence to {!r}...".format(fspec))
-        with open(fspec, "wt") as fp:
+        logger.info(f"Writing activity sequence to {fspec!r}...")
+        with open(fspec, "w") as fp:
             fp.write("# Stressor Activity Definitions\n")
             fp.write("# See https://stressor.readthedocs.io/\n")
-            fp.write("# Auto-generated {}\n".format(datetime_to_iso()))
+            fp.write(f"# Auto-generated {datetime_to_iso()}\n")
             fp.write("# Source:\n")
             fp.write("#     File: {}\n".format(self.opts["fspec"]))
-            fp.write("#     HAR Version: {}\n".format(self.har_version))
-            fp.write("#     Creator: {}\n".format(self.creator_info))
+            fp.write(f"#     HAR Version: {self.har_version}\n")
+            fp.write(f"#     Creator: {self.creator_info}\n")
             if self.browser_info:
-                fp.write("#     Browser: {}\n".format(self.browser_info))
-            fp.write("#     Recorded: {}\n".format(self.first_entry_dt))
-            fp.write("#     Using base URL {!r}\n".format(self.base_url))
+                fp.write(f"#     Browser: {self.browser_info}\n")
+            fp.write(f"#     Recorded: {self.first_entry_dt}\n")
+            fp.write(f"#     Using base URL {self.base_url!r}\n")
             fp.write("\n")
 
             for entry in self.entries:
                 self._write_entry(fp, entry)
         logger.info("Done.")
         return
```

### Comparing `stressor-0.5.2/stressor/monitor/server.py` & `stressor-0.6.0/stressor/monitor/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import io
 import json
 import logging
 import os
@@ -122,11 +121,11 @@
 
     def shutdown(self):
         if self.httpd:
             self.httpd.shutdown()
 
     def open_browser(self):
         assert self.bind == ""
-        monitor_url = "http://localhost:{}/".format(self.port)
+        monitor_url = f"http://localhost:{self.port}/"
         # monitor_url = "http://127.0.0.1:{}/".format(self.port)
-        logger.info("Open web browser at {}".format(monitor_url))
+        logger.info(f"Opening web browser at {monitor_url}")
         webbrowser.open_new_tab(monitor_url)
```

### Comparing `stressor-0.5.2/stressor/plugin_manager.py` & `stressor-0.6.0/stressor/plugin_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/yabs
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/yabs
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 from pkg_resources import iter_entry_points
 
 from stressor.plugins.base import ActivityBase, MacroBase
 from stressor.util import logger
@@ -43,26 +42,22 @@
     @classmethod
     def find_plugins(cls):
         """Load all entry points with group name 'stressor.plugins'."""
         if cls.entry_points_searched:
             return
         cls.entry_points_searched = True
         ep_map = cls._entry_point_map
-        logger.debug("Search entry points for group '{}'...".format(cls.namespace))
+        logger.debug(f"Search entry points for group '{cls.namespace}'...")
 
         for ep in iter_entry_points(group=cls.namespace, name=None):
-            plugin_name = "{}".format(ep.dist)
-            logger.debug(
-                "Found plugin {} from entry point `{}`".format(plugin_name, ep)
-            )
+            plugin_name = f"{ep.dist}"
+            logger.debug(f"Found plugin {plugin_name} from entry point `{ep}`")
 
             if ep.name in ep_map:
-                logger.warning(
-                    "Duplicate entry point name: {}; skipping...".format(ep.name)
-                )
+                logger.warning(f"Duplicate entry point name: {ep.name}; skipping...")
                 continue
             # elif ep.name in cls.task_class_map:
             #     # TODO: support overriding standard tasks?
             #     # Maybe when 'extras=[override]' is passed...
             #     logger.warning(
             #         "Plugin task name already exists: {}; skipping...".format(ep.name)
             #     )
@@ -86,15 +81,15 @@
             if existing_cls is sub_cls:
                 continue  # already registered
             elif existing_cls is None:
                 if not name.startswith("_"):
                     cls_map[name] = sub_cls
                 cls._register_subclasses(sub_cls, cls_map)
             else:
-                raise RuntimeError("Class name conflict: {}".format(sub_cls))
+                raise RuntimeError(f"Class name conflict: {sub_cls}")
         return
 
     @classmethod
     def register_plugins(cls, arg_parser):
         """Call `register_fn` on all loaded entry points."""
         if cls.plugins_registered:
             return
@@ -110,57 +105,57 @@
         # Load entry points from all installed mosules that have the
         # 'stressor.plugins' namespace:
         cls.find_plugins()
 
         # Call `register_fn` on all loaded entry points_
         ep_map = cls._entry_point_map
         for name, ep in cls._entry_point_map.items():
-            logger.info("Load plugins {}...".format(ep.dist))
+            logger.info(f"Load plugins {ep.dist}...")
             try:
                 register_fn = ep.load()
                 if not callable(register_fn):
-                    raise RuntimeError("Entry point {} is not a function".format(ep))
+                    raise RuntimeError(f"Entry point {ep} is not a function")
                 ep_map[ep.name] = register_fn
             except Exception:
-                logger.exception("Failed to load {}".format(ep))
+                logger.exception(f"Failed to load {ep}")
 
             prev_activities = list(ActivityBase.__subclasses__())
             prev_macros = list(MacroBase.__subclasses__())
 
-            logger.debug("Register plugins {}...".format(ep.dist))
+            logger.debug(f"Register plugins {ep.dist}...")
             try:
                 # The plugin must declare new classes derrived from
                 # ActivityBase and/or MacroBase
                 register_fn(
                     activity_base=ActivityBase,
                     macro_base=MacroBase,
                     arg_parser=arg_parser,
                 )
             except Exception:
-                logger.exception("Could not register {}".format(name))
+                logger.exception(f"Could not register {name}")
                 continue
 
             found_one = False
             for activity_cls in ActivityBase.__subclasses__():
                 if activity_cls in prev_activities:
                     continue
                 found_one = True
-                logger.info("Register {}.{}".format(ep.dist, activity_cls))
+                logger.info(f"Register {ep.dist}.{activity_cls}")
 
             for macro_cls in MacroBase.__subclasses__():
                 if macro_cls in prev_macros:
                     continue
                 found_one = True
-                logger.info("Register {}.{}".format(ep.dist, macro_cls))
+                logger.info(f"Register {ep.dist}.{macro_cls}")
 
             if not found_one:
                 logger.warning(
-                    "Plugin {} did not register activites nor macros".format(ep.dist)
+                    f"Plugin {ep.dist} did not register activites nor macros"
                 )
 
         # Build plugin maps from currently known subclasses
         cls._register_subclasses(ActivityBase, cls.activity_plugin_map)
-        logger.debug("Registered activity plugins:\n{}".format(cls.activity_plugin_map))
+        logger.debug(f"Registered activity plugins:\n{cls.activity_plugin_map}")
 
         cls._register_subclasses(MacroBase, cls.macro_plugin_map)
-        logger.debug("Registered macro plugins:\n{}".format(cls.macro_plugin_map))
+        logger.debug(f"Registered macro plugins:\n{cls.macro_plugin_map}")
         return
```

### Comparing `stressor-0.5.2/stressor/plugins/base.py` & `stressor-0.6.0/stressor/plugins/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import re
 from abc import ABC, abstractmethod
 
 from stressor.util import StressorError, assert_always, check_arg, parse_args_from_str
@@ -135,27 +134,25 @@
         self.compile_path = config_manager.stack.get_path(
             skip_segs=2, last_seg=self.get_info()
         )
         passed = set(activity_args.keys())
         if self._mandatory_args:
             missing = self._mandatory_args.difference(passed)
             if missing:
-                raise ActivityCompileError(
-                    "Missing mandatory arguments: {}".format(missing)
-                )
+                raise ActivityCompileError(f"Missing mandatory arguments: {missing}")
 
         if self._all_known_args is None:
             if self._known_args:
                 self._all_known_args = common_args | self._known_args
             else:
                 self._all_known_args = common_args
 
         extra = passed.difference(self._all_known_args)
         if extra:
-            raise ActivityCompileError("Unsupported arguments: {}".format(extra))
+            raise ActivityCompileError(f"Unsupported arguments: {extra}")
 
         self.monitor = activity_args.get("monitor", self._default_monitor)
         self.ignore_timing = activity_args.get(
             "ignore_timing", self._default_ignore_timing
         )
 
     def __str__(self):
@@ -194,17 +191,15 @@
         if info_args is True:
             info_args = self._info_args
         elif info_args is False:
             info_args = []
         arg_dict = self.raw_args if expanded_args is None else expanded_args
         if info_args:
             # Add selected args
-            args = (
-                "{}={!r}".format(a, arg_dict.get(a)) for a in info_args if a in arg_dict
-            )
+            args = (f"{a}={arg_dict.get(a)!r}" for a in info_args if a in arg_dict)
         else:  # add all args
             args = (
                 "{}={!r}".format(*kv) for kv in arg_dict.items() if kv[0] != "activity"
             )
         return "{}({})".format(self.get_script_name(), ", ".join(args))
 
     def prepare_execute(self, session, expanded_args):
@@ -212,15 +207,15 @@
 
         The session manager calls this for every activity instance, directly
         before `get_info()` and `execute()`.
         Normally this method does not need to be implemented. (One exception is
         `SleepActivity`, that calculates the next random duration per session,
         so it can be displayed by `get_info(..., session)`.)
         """
-        pass
+        return
 
     @abstractmethod
     def execute(self, session, **expanded_args):
         """
         Called by the :class:`SessionManager`, after `$(context.var)` macros
         have been resolved if any.
         A derived class MUST implement this method.
@@ -290,14 +285,15 @@
 
     #: Allow late evaluation (e.g. $stamp)
     #: TODO: Not yet implemented
     run_time_eval = False
 
     def __init__(self, **macro_args):
         """"""
+        return
 
     @classmethod
     def get_script_name(cls):
         # Note: we must check `cls.__dict__` instead of `cls._script_name`,
         # because we want to test the local class attribute (not a derived one):
         if cls.__dict__.get("_script_name") is None:
             assert_always(cls.__name__.endswith("Macro"))
```

### Comparing `stressor-0.5.2/stressor/plugins/common.py` & `stressor-0.6.0/stressor/plugins/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import os
 import random
 from textwrap import dedent
 
@@ -17,23 +16,23 @@
     """Implement `$load(path)` macro."""
 
     def apply(self, config_manager, parent, parent_key, path):
         path = config_manager.resolve_path(path, must_exist=True)
 
         if path.lower().endswith(".py"):
             assert parent_key == "script"
-            with open(path, "rt") as f:
+            with open(path) as f:
                 res = f.read()
             parent[parent_key] = res
             return res
 
         if not path.lower().endswith((".yaml", ".yml")):
             raise NotImplementedError
         # Load (and )
-        with open(path, "rt") as f:
+        with open(path) as f:
             res = yaml.safe_load(f)
         assert isinstance(parent, dict)
         assert isinstance(res, list)
         parent[parent_key] = res
         # print(yaml.dump(parent, default_flow_style=False))
         return res
```

### Comparing `stressor-0.5.2/stressor/plugins/http_activities.py` & `stressor-0.6.0/stressor/plugins/http_activities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import re
 import threading
 from pprint import pformat
 from queue import Empty, Queue
@@ -38,15 +37,15 @@
     match = re.match(pattern, value)  # , re.MULTILINE)
     # if "." in pattern or "*" in pattern:
     #     match = re.match(pattern, value)  # , re.MULTILINE)
     # else:
     #     match = pattern == value
 
     if not match:
-        msg = "`{}` value {!r} does not match pattern {!r}".format(info, value, pattern)
+        msg = f"`{info}` value {value!r} does not match pattern {pattern!r}"
         return False, msg
     return True, None
 
 
 class HTTPRequestActivity(ActivityBase):
     # RESPONSE_LOG_LENGTH = 200
     REQUEST_ARGS = {"auth", "data", "json", "headers", "params", "timeout", "verify"}
@@ -84,15 +83,15 @@
 
         if params:
             params = "?" + urlencode(params)
         if self.__class__ is HTTPRequestActivity:
             method = "{} ".format(args_dict["method"])
         else:
             method = ""
-        return "{}({}{}{})".format(self.get_script_name(), method, url, params)
+        return f"{self.get_script_name()}({method}{url}{params})"
 
     @classmethod
     def _format_response(cls, resp, short=False, add_headers=False, ruler=True):
 
         try:
             s = resp.json()
             s = pformat(s)
@@ -105,34 +104,32 @@
                     lines.append(s)
             s = "\n".join(lines)
             # s = fill(s)
 
         res = []
         res.append("")
         res.append(
-            "--- Response status: {}, len: {:,} bytes: >>>".format(
-                resp.status_code, len(resp.content)
-            )
+            f"--- Response status: {resp.status_code}, len: {len(resp.content):,} bytes: >>>"
         )
 
         for k, v in resp.headers.items():
-            res.append("{}: {}".format(k, v))
+            res.append(f"{k}: {v}")
         res.append("- " * 20)
 
         if short:
             s = shorten_string(s, 500, 100, place_holder="\n[...]\n")
         res.append(s)
         res.append("<<< " + "-" * 36)
         return "\n".join(res)
 
     @classmethod
     def _raise_assertion(cls, cause, resp):
         msg = cls._format_response(resp, short=True)
         msg = "\n  | ".join(msg.split("\n"))
-        raise ActivityAssertionError("{}\n{}".format(cause, msg))
+        raise ActivityAssertionError(f"{cause}\n{msg}")
 
     def execute(self, session, **expanded_args):
         """
         Raises:
             ActivityAssertionError:
             requests.exceptions.ConnectionError: 'Connection refused', etc.
             requests.exceptions.HTTPError: On 404, 500, etc.
@@ -165,31 +162,31 @@
         basic_auth = session.sessions.get("basic_auth", False)
         if basic_auth:
             r_args.setdefault("auth", session.user.auth)
 
         headers = r_args.setdefault("headers", {})
         headers.setdefault(
             "User-Agent",
-            "session/{} Stressor/{}".format(session.session_id, __version__),
+            f"session/{session.session_id} Stressor/{__version__}",
         )
 
         # if debug:
         #     http_client.HTTPConnection.debuglevel = 1
         # else:
         #     http_client.HTTPConnection.debuglevel = 0
         if debug:
-            logger.info("HTTPRequest({}, {}, {})...".format(method, url, r_args))
+            logger.info(f"HTTPRequest({method}, {url}, {r_args})...")
 
         # The actual HTTP request:
         try:
             resp = bs.request(method, url, **r_args)
         except requests.exceptions.Timeout as e:
-            raise ActivityTimeoutError("{}".format(e))
+            raise ActivityTimeoutError(f"{e}")
         except RequestException as e:
-            raise ActivityError("{}".format(e))
+            raise ActivityError(f"{e}")
 
         is_json = False
         try:
             result = resp.json()
             is_json = True
         except ValueError:
             result = resp.text
@@ -201,39 +198,35 @@
 
         assert_status = expanded_args.get("assert_status")
         if not assert_status:
             # requests.exceptions.HTTPError: On 404, 500, etc.
             resp.raise_for_status()
         elif resp.status_code not in assert_status:
             self._raise_assertion(
-                "HTTP status does not match {}: {}".format(
-                    assert_status, resp.status_code
-                ),
+                f"HTTP status does not match {assert_status}: {resp.status_code}",
                 resp,
             )
 
         arg = expanded_args.get("assert_match_headers")
         if arg:
             text = str(resp.headers)
             if not re.match(arg, text):
-                self._raise_assertion(
-                    "Result headers do not match `{}`".format(arg), resp
-                )
+                self._raise_assertion(f"Result headers do not match `{arg}`", resp)
 
         arg = expanded_args.get("assert_json")
         if arg:
             if not is_json:
                 self._raise_assertion("Unexpected result type (expected JSON)", resp)
 
             for key, pattern in arg.items():
                 value = get_dict_attr(result, key)
                 # print(result, key, value)
                 match, msg = match_value(pattern, value, key)
                 if not match:
-                    self._raise_assertion("Unexpected JSON result {}".format(msg), resp)
+                    self._raise_assertion(f"Unexpected JSON result {msg}", resp)
 
         arg = expanded_args.get("assert_html")
         if arg:
             if is_json:
                 self._raise_assertion("Unexpected result type (expected HTML)", resp)
 
             for xpath, pattern in arg.items():
@@ -249,15 +242,15 @@
                 elif not match:
                     ok = False
                 else:
                     # print("match", html.tostring(match))
                     raise NotImplementedError
                 if not ok:
                     self._raise_assertion(
-                        "Unexpected HTML result: XPath {!r} -> {}".format(xpath, match),
+                        f"Unexpected HTML result: XPath {xpath!r} -> {match}",
                         resp,
                     )
 
         return result
 
 
 class GetRequestActivity(HTTPRequestActivity):
@@ -310,15 +303,15 @@
         basic_auth = session.sessions.get("basic_auth", False)
         if basic_auth:
             r_args.setdefault("auth", session.user.auth)
 
         headers = r_args.setdefault("headers", {})
         headers.setdefault(
             "User-Agent",
-            "session/{} Stressor/{}".format(session.session_id, __version__),
+            f"session/{session.session_id} Stressor/{__version__}",
         )
 
         # TODO: requests.Session is not guaranteed to be thread-safe!
         bs = session.browser_session
         # Queue-up all pending request
         queue = Queue()
         for url in url_list:
@@ -332,50 +325,46 @@
             while not session.stop_request.is_set():
                 try:
                     url = queue.get(False)
                 except Empty:
                     break
 
                 if debug:
-                    logger.info("StaticRequests({}, {})...".format(name, url))
+                    logger.info(f"StaticRequests({name}, {url})...")
                 # The actual HTTP request:
                 # TODO: requests.Session is not guaranteed to be thread-safe!
                 try:
                     res = bs.request(method, url, **r_args)
                     res.raise_for_status()
                     results.append((True, name, url, None))
                 except Exception as e:
-                    results.append((False, name, url, "{}".format(e)))
+                    results.append((False, name, url, f"{e}"))
                 queue.task_done()
-            logger.debug("StaticRequests({}) stopped.".format(name))
+            logger.debug(f"StaticRequests({name}) stopped.")
             return
 
-        logger.debug(
-            "Starting {} StaticRequestsActivity workers...".format(thread_count)
-        )
+        logger.debug(f"Starting {thread_count} StaticRequestsActivity workers...")
 
         thread_list = []
         for i in range(thread_count):
-            name = "{}.{:02}".format(session.session_id, i + 1)
+            name = f"{session.session_id}.{i + 1:02}"
             t = threading.Thread(name=name, target=_work, args=[name])
             t.setDaemon(True)  # Required to make Ctrl-C work
             thread_list.append(t)
 
         for t in thread_list:
             t.start()
 
         logger.debug("All StaticRequestsActivity workers running...")
         queue.join()
         for t in thread_list:
             t.join()
-        errors = ["{}".format(error) for ok, name, url, error in results if not ok]
+        errors = [f"{error}" for ok, name, url, error in results if not ok]
         if errors:
-            raise ActivityError(
-                "{} reqests failed:\n{}".format(len(errors), format(errors))
-            )
+            raise ActivityError(f"{len(errors)} reqests failed:\n{format(errors)}")
             # logger.error(pformat(errors))
         return bool(errors)
 
 
 class PollRequestActivity(HTTPRequestActivity):
     """
     TODO: This activity simulates a peridodical request to a single URL.
```

### Comparing `stressor-0.5.2/stressor/plugins/script_activities.py` & `stressor-0.6.0/stressor/plugins/script_activities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 from pprint import pformat
 from textwrap import dedent
 
 from stressor.plugins.base import (
@@ -40,15 +39,15 @@
 
         if path:
             if script:
                 raise ActivityCompileError(
                     "`path` and `script` args are mutually exclusive"
                 )
             path = config_manager.resolve_path(path)
-            with open(path, "rt") as f:
+            with open(path) as f:
                 script = f.read()
             #:
             self.script = compile(script, path, "exec")
         elif script:
             # script = dedent(self.script)
             self.script = compile(script, "<string>", "exec")
         else:
@@ -82,18 +81,18 @@
         prev_global_keys = set(globals())
         prev_context_keys = set(local_vars.keys())
 
         try:
             exec(self.script, global_vars, local_vars)
         except ConnectionError as e:
             # TODO: more requests-exceptions?
-            msg = "Script failed: {!r}: {}".format(e, e)
+            msg = f"Script failed: {e!r}: {e}"
             raise ScriptActivityError(msg)
         except Exception as e:
-            msg = "Script failed: {!r}: {}".format(e, e)
+            msg = f"Script failed: {e!r}: {e}"
             if session.verbose >= 4:
                 logger.exception(msg)
                 raise ScriptActivityError(msg) from e
             raise ScriptActivityError(msg)
         finally:
             local_vars.pop("session")
 
@@ -110,42 +109,34 @@
                     )
                 )
             else:
                 for k in self.export:
                     v = local_vars.get(k)
                     assert type(v) in (int, float, str, list, dict)
                     session.context[k] = v
-                    logger.debug("Set context.{} = {!r}".format(k, v))
+                    logger.debug(f"Set context.{k} = {v!r}")
                 # store_keys = new_keys.intersection(self.export)
 
         # TODO: this cannot happen?
         new_globals = set(globals().keys()).difference(prev_global_keys)
         if new_globals:
-            logger.warning("Script-defined globals: {}".format(new_globals))
+            logger.warning(f"Script-defined globals: {new_globals}")
             raise ScriptActivityError("Script introduced globals")
 
         # new_context = context_keys.difference(prev_context_keys)
         # logger.info("Script-defined context-keys: {}".format(new_context))
 
         # new_locals = set(locals().keys()).difference(prev_local_keys)
         # if new_locals:
         #     logger.info("Script-defined locals: {}".format(new_locals))
 
         # logger.info("Script locals:\n{}".format(pformat(local_vars)))
         if expanded_args.get("debug") or session.verbose >= 5:
             logger.info(
-                "{} {}\n  Context after execute:\n    {}\n  return value: {!r}".format(
-                    session.context_stack,
-                    self,
-                    pformat(session.context, indent=4),
-                    result,
-                )
+                f"{session.context_stack} {self}\n  Context after execute:\n    {pformat(session.context, indent=4)}\n  return value: {result!r}"
             )
         elif session.verbose >= 3 and result is not None:
             logger.info(
-                "{} returnd: {!r}".format(
-                    session.context_stack,
-                    shorten_string(result, 200) if isinstance(result, str) else result,
-                )
+                f"{session.context_stack} returnd: {shorten_string(result, 200) if isinstance(result, str) else result!r}"
             )
 
         return result
```

### Comparing `stressor-0.5.2/stressor/run_manager.py` & `stressor-0.6.0/stressor/run_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import itertools
 import sys
 import threading
 import time
 from collections import defaultdict
 from datetime import datetime
 
 from snazzy import emoji, green, red, yellow
 
+from stressor import __version__
 from stressor.config_manager import ConfigManager
 from stressor.monitor.server import MonitorServer
 from stressor.session_manager import SessionManager, User
 from stressor.statistic_manager import StatisticManager
 from stressor.util import (
     check_arg,
     format_elap,
@@ -91,15 +91,15 @@
         # register_plugins()
         self.CURRENT_RUN_MANAGER = self
         self.set_console_ctrl_handler()
 
     def __str__(self):
         # name = self.config_manager.path if self.config_manager else "?"
         # name = self.run_config.get("name") if self.run_config else "?"
-        return "RunManager<{}>".format(self.stage.upper())
+        return f"RunManager<{self.stage.upper()}>"
 
     @staticmethod
     def set_console_ctrl_handler():
         if RunManager.CTRL_HANDLER_SET is None:
             RunManager.CTRL_HANDLER_SET = set_console_ctrl_handler(
                 RunManager._console_ctrl_handler
             )
@@ -120,24 +120,26 @@
             False if not handled, i.e. next registered handler will be called
         """
         # if self.stop_request.is_set():
         #     print("Got Ctrl-C 2nd time: terminating...")
         #     logger.warning("Got Ctrl-C a 2nd time: terminating...")
         #     time.sleep(0.1)
         #     # sys.exit(2)
-        print("Got Ctrl-C (windows handler), terminating...", file=sys.stderr)
+        print(  # noqa: T201
+            "Got Ctrl-C (windows handler), terminating...", file=sys.stderr
+        )
         logger.warning("Got Ctrl-C (windows handler), terminating...")
         # self.stop_request.set()
         self.stop()
         # return False
         return True
 
     def set_stage(self, stage):
         check_arg(stage, str, stage in self.STAGES)
-        logger.info("Enter stage '{}'".format(stage.upper()))
+        logger.info(f"Enter stage '{stage.upper()}'")
         self.stage = stage
 
     def publish(self, channel, allow_cancel=False, *args, **kwargs):
         """Notify all subscribed handlers."""
         assert channel in self.CHANNELS
         result_list = []
         if not self.has_hooks:
@@ -180,15 +182,15 @@
 
         ap = lines.append
         col = red if has_errors else green
         horz_line = col("=-" * 38 + "=")
 
         ap("Result Summary:")
         ap(horz_line)
-        ap("Stressor scenario '{}' finished.".format(cm.name))
+        ap(f"Stressor scenario '{cm.name}' finished.")
         ap("  Tag:      '{}'".format(cm.config.get("tag", "n.a.")))
         ap("  Base URL: {}".format(cm.config.get("base_url", "")))
         ap("  Start:    {}".format(self.start_dt.strftime("%Y-%m-%d %H:%M:%S")))
         ap("  End:      {}".format(self.end_dt.strftime("%Y-%m-%d %H:%M:%S")))
         ap(
             "Run time {}, net: {}.".format(
                 format_elap(run_time, high_prec=True),
@@ -222,30 +224,30 @@
                     format_num(self.stats["act_count"] / run_time),
                     format_num(self.stats["act_count"] / (run_time * user_count)),
                 )
             )
 
         # --- List of all activities that are marked `monitor: true`
         if self.stats["monitored"]:
-            print(self.stats["monitored"])
+            print(self.stats["monitored"])  # noqa: T201
             ap("{} monitored activities:".format(len(self.stats["monitored"])))
             for path, info in self.stats["monitored"].items():
                 errors = info.get("errors")
-                ap("  - {}".format(path))
+                ap(f"  - {path}")
                 if not info:
                     ap("    n: 0, min: n.a., avg: n.a., max: n.a.")
                     continue
 
                 ap(
                     "    n: {:,}, min: {}, avg: {}, max: {}{}".format(
                         info["act_count"],
                         format_elap(info["act_time_min"], high_prec=True),
                         format_elap(info["act_time_avg"], high_prec=True),
                         format_elap(info["act_time_max"], high_prec=True),
-                        red(", {} errors".format(errors)) if errors else "",
+                        red(f", {errors} errors") if errors else "",
                     )
                 )
 
         if has_errors:
             pics = emoji(" 💥 💔 💥", "")
             ap(
                 red(
@@ -282,40 +284,39 @@
             "stageDisplay": "done" if self.stage == "waiting" else self.stage,
             "hasErrors": self.has_errors(),
             "startTimeStr": "{}".format(self.start_dt.strftime("%Y-%m-%d %H:%M:%S")),
             "baseUrl": cm.get("config.base_url"),
             "sessionCount": self.stats["sess_count"],
             "sessionsRunning": self.stats["sess_running"],
             "stats": stats_info,
+            "version": __version__,
         }
         if self.end_dt:
             elap = self.end_dt - self.start_dt
             res["endTimeStr"] = "{} ({})".format(
                 self.end_dt.strftime("%Y-%m-%d %H:%M:%S"),
                 format_elap(elap.total_seconds()),
             )
         else:
             elap = datetime.now() - self.start_dt
-            res["endTimeStr"] = "(running for {}...)".format(
-                format_elap(elap.total_seconds())
-            )
+            res["endTimeStr"] = f"(running for {format_elap(elap.total_seconds())}...)"
 
         return res
 
     def log_info(self, *args, **kwargs):
         self.publish("log", level="info", *args, **kwargs)
 
     def load_config(self, run_config_file):
         """Load configuration file and set shortcuts."""
         cr = ConfigManager(self.stats)
         cr.read(run_config_file, load_files=True)
 
         self.config_manager = cr
         # self.run_config = cr.run_config
-        logger.info("Successfully compiled configuration {}.".format(cr.path))
+        logger.info(f"Successfully compiled configuration {cr.path}.")
 
     def _run_one(self, session_manager):
         """Run inside a separate thread."""
         try:
             session_manager.run()
             # We don't need to print results if only one session was run, since
             # it is also part of the global stats:
@@ -340,54 +341,50 @@
 
     def run_in_threads(self, user_list, context):
         self.publish("start_run", run_manager=self)
         self.stop_request.clear()
         thread_list = []
         self.session_list = []
         for i, user in enumerate(user_list, 1):
-            name = "t{:02}".format(i)
+            name = f"t{i:02}"
             sess = SessionManager(self, context, name, user)
             self.session_list.append(sess)
             t = threading.Thread(name=name, target=self._run_one, args=[sess])
-            t.setDaemon(True)  # Required to make Ctrl-C work
+            t.daemon = True  # Required to make Ctrl-C work
             thread_list.append(t)
 
-        logger.info("Starting {} session workers...".format(len(thread_list)))
+        logger.info(f"Starting {len(thread_list)} session workers...")
         self.set_stage("running")
         self.stats.report_start(None, None, None)
 
         ramp_up_delay = self.config_manager.sessions.get("ramp_up_delay")
 
         start_run = time.monotonic()
         for i, t in enumerate(thread_list):
             if ramp_up_delay and i > 1:
                 delay = get_random_number(ramp_up_delay)
-                logger.info(
-                    "Ramp-up delay for t{:02}: {:.2f} seconds...".format(i, delay)
-                )
+                logger.info(f"Ramp-up delay for t{i:02}: {delay:.2f} seconds...")
                 time.sleep(delay)
             t.start()
 
         logger.important(
-            "All {} sessions running, waiting for them to terminate...".format(
-                len(thread_list)
-            )
+            f"All {len(thread_list)} sessions running, waiting for them to terminate..."
         )
         for t in thread_list:
             t.join()
 
         self.set_stage("done")
         elap = time.monotonic() - start_run
 
         # self.stats.add_timing("run", elap)
         self.stats.report_end(None, None, None)
 
         self.publish("end_run", run_manager=self, elap=elap)
 
-        logger.debug("Results for {}:\n{}".format(self, self.stats.format_result()))
+        logger.debug(f"Results for {self}:\n{self.stats.format_result()}")
 
         return not self.has_errors()
 
     def run(self, options, extra_context=None):
         """Run the current
 
         Args:
```

### Comparing `stressor-0.5.2/stressor/session_manager.py` & `stressor-0.6.0/stressor/session_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import re
 import time
 from copy import deepcopy
 
@@ -37,15 +36,15 @@
         self.password = password
         for arg_name, arg_val in kwargs.items():
             assert type(arg_name) in (int, float, str)
             setattr(self, arg_name, arg_val)
         return
 
     def __str__(self):
-        return "User<{}>".format(self.name)
+        return f"User<{self.name}>"
 
     # Provide nicer display for pprint(), etc.
     __repr__ = __str__
 
     @property
     def auth(self):
         """Return (name, password) tuple or None."""
@@ -135,15 +134,15 @@
         self.sequence_start = None
         self.pending_activity = None
         self.activity_start = None
 
         self.stats.register_session(self)
 
     def __str__(self):
-        return "SessionManager<{}>".format(self.session_id)
+        return f"SessionManager<{self.session_id}>"
 
     # Provide nicer display for pprint(), etc.
     __repr__ = __str__
 
     def publish(self, channel, *args, **kwargs):
         kwargs["session_id"] = self.session_id
         return self.run_manager.publish(channel, *args, **kwargs)
@@ -210,21 +209,17 @@
         time_limit_reached = self.max_time and run_time > self.max_time
 
         if not cs and (err_limit_reached or time_limit_reached):
             # We just hit a limit: issue a warning and take a note of the sequence
             self._cancelled_seq = seq_name
             # self.stats.stats["run_limit_reached"] = True
             if err_limit_reached:
-                msg = "Reached max. error limit of {}: stopping...".format(
-                    self.max_errors
-                )
+                msg = f"Reached max. error limit of {self.max_errors}: stopping..."
             elif time_limit_reached:
-                msg = "Reached max. run time limit of {}: stopping...".format(
-                    self.max_time
-                )
+                msg = f"Reached max. run time limit of {self.max_time}: stopping..."
             self.stats.report_limit_violation(msg)
             logger.warning(yellow(msg))
             return False
         elif cs in ("init", "end"):
             # The limit was reached inside the init or end sequence: always skip
             return False
         elif cs:
@@ -240,34 +235,34 @@
         logger.info("{} {}".format("DRY-RUN" if self.dry_run else "Execute", path))
 
     def report_activity_error(self, sequence, activity, activity_args, exc):
         """Called session runner when activity `execute()` or assertions raise an error."""
         # self.stats.inc("errors")
 
         if isinstance(exc, SkippedError):
-            logger.warning(yellow("Skipped {}".format(activity)))
+            logger.warning(yellow(f"Skipped {activity}"))
             self.pending_activity = None
             return
 
         # Create a copy of the current context, so we can shorten values
         context = self.context_stack.context.copy()
         context["last_result"] = shorten_string(context.get("last_result"), 500, 100)
 
         msg = []
         # msg.append("{} {}: {!r}:".format(self.context_stack, activity, exc))
         # msg.append("{!r}:".format(exc))
-        msg.append("{!r}:".format(exc))
+        msg.append(f"{exc!r}:")
         if isinstance(exc, ActivityAssertionError):
             msg.append("Failed assertions:")
             for err in exc.assertion_list:
-                msg.append("  - {}".format(err))
-        msg.append("Execution path: {}".format(self.context_stack))
-        msg.append("Activity: {}".format(activity))
-        msg.append("Activity args: {}".format(activity_args))
-        msg.append("Context: {}".format(context))
+                msg.append(f"  - {err}")
+        msg.append(f"Execution path: {self.context_stack}")
+        msg.append(f"Activity: {activity}")
+        msg.append(f"Activity args: {activity_args}")
+        msg.append(f"Context: {context}")
 
         msg = "\n    ".join(msg)
         logger.error(red(msg))
         self.stats.report_error(self, sequence, activity, error=msg)
         return
 
     def report_activity_result(self, sequence, activity, activity_args, result, elap):
@@ -283,41 +278,35 @@
         context = self.context_stack.context
         errors = []
         # warnings = []
 
         arg = float(activity_args.get("assert_max_time", 0))
         if arg and elap > arg:
             errors.append(
-                "Execution time limit of {} seconds exceeded: {:.3} sec.".format(
-                    arg, elap
-                )
+                f"Execution time limit of {arg} seconds exceeded: {elap:.3} sec."
             )
 
         arg = activity_args.get("assert_match")
         if arg:
             text = str(result)
             # Note: use re.search (not .match)!
             if not re.search(arg, text, re.MULTILINE):
                 errors.append(
-                    "Result does not match `{}`: {!r}".format(
-                        arg, shorten_string(text, 500, 100)
-                    )
+                    f"Result does not match `{arg}`: {shorten_string(text, 500, 100)!r}"
                 )
 
         arg = activity_args.get("store_json")
         if arg:
             for var_name, key_path in arg.items():
                 try:
                     val = get_dict_attr(result, key_path)
                     context[var_name] = val
                 except Exception:
                     errors.append(
-                        "store_json could not find `{}` in activity result {!r}".format(
-                            key_path, result
-                        )
+                        f"store_json could not find `{key_path}` in activity result {result!r}"
                     )
 
         if errors:
             raise ActivityAssertionError(errors)
         return
 
     def run_sequence(self, seq_name, sequence):
@@ -340,17 +329,15 @@
             activity_args = deepcopy(activity_args)
             activity_args.pop("activity")
 
             # Add activity info to path
             # Note: `get_info()` is not as detailed as it could, since we don't
             # pass the expanded args here. We set it anyway, so we have a valid
             # stack in case `_evaluate_macros()` blows.
-            with stack.enter(
-                "#{:02}-{}".format(act_idx, activity.get_info(session=self))
-            ):
+            with stack.enter(f"#{act_idx:02}-{activity.get_info(session=self)}"):
                 expanded_args = self._evaluate_macros(activity_args, context)
 
                 # Let activity do internal calculations, that might be used by
                 # the follwing call to `get_info()`
                 activity.prepare_execute(self, expanded_args)
 
                 # Enhance the path info with expanded args
@@ -447,15 +434,15 @@
         start_session = time.monotonic()
         skip_all = False
         skip_all_but_end = False
 
         for seq_idx, seq_def in enumerate(scenario, 1):
             seq_name = seq_def["sequence"]
             if skip_all or (skip_all_but_end and seq_name != "end"):
-                logger.warning("Skipping sequence '{}'.".format(seq_name))
+                logger.warning(f"Skipping sequence '{seq_name}'.")
                 continue
 
             sequence = sequences.get(seq_name)
             loop_repeat = int(seq_def.get("repeat", 0))
             loop_duration = float(seq_def.get("duration", 0.0))
             start_seq_loop = time.monotonic()
             loop_idx = 0
@@ -479,34 +466,30 @@
                     )
                     break
 
                 now = time.monotonic()
                 # `Sequence duration: SECS`:
                 if loop_duration > 0 and now > (start_seq_loop + loop_duration):
                     logger.info(
-                        "Stopping sequence '{}' loop after {} sec.".format(
-                            seq_name, loop_duration
-                        )
+                        f"Stopping sequence '{seq_name}' loop after {loop_duration} sec."
                     )
                     break
                 # `Session duration: SECS` (but run 'end' sequence):
                 elif (
                     seq_name != "end"
                     and session_duration > 0
                     and now > (start_session + session_duration)
                 ):
                     logger.info(
-                        "Stopping scenario '{}' loop after {} sec.".format(
-                            seq_name, session_duration
-                        )
+                        f"Stopping scenario '{seq_name}' loop after {session_duration} sec."
                     )
                     skip_all_but_end = True
                     break
 
-                with stack.enter("#{:02}-{}@{}".format(seq_idx, seq_name, loop_idx)):
+                with stack.enter(f"#{seq_idx:02}-{seq_name}@{loop_idx}"):
                     is_ok = self.run_sequence(seq_name, sequence)
                     if seq_name == "init" and not is_ok:
                         logger.error(
                             "Stopping scenario due to an error in the 'init' sequence."
                         )
                         skip_all = True
                         break
```

### Comparing `stressor-0.5.2/stressor/statistic_manager.py` & `stressor-0.6.0/stressor/statistic_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import logging
 import threading
 import time
 from collections import OrderedDict
@@ -257,26 +256,26 @@
             p = "net_" + key_prefix
             self._add_timing(d, p, elap)
         return
 
     def _add_error(self, d, error):
         d.setdefault("errors", 0)
         d["errors"] += 1
-        d["last_error"] = shorten_string("{}".format(error), 500, 100)
+        d["last_error"] = shorten_string(f"{error}", 500, 100)
 
     def error_count(self, or_warnings=False):
         error_count = self.stats["errors"]
         return error_count
 
     def has_errors(self, or_warnings=False):
         return self.error_count(or_warnings) > 0
 
     def format_result(self):
         s = dict(self.stats)
-        return "{}".format(pformat(s))
+        return f"{pformat(s)}"
 
     def get_monitor_info(self, config_all):
         stats = self.stats
 
         def f(d, k, secs=False):
             v = d.get(k, 0)
             if secs:
@@ -388,8 +387,8 @@
         if type_ == "sequence":
             errors = self.stats["sequence_stats"][key]["last_error"]
         elif type_ == "session":
             errors = self.stats["sessions"][key]["last_error"]
         elif type_ == "monitored":
             errors = self.stats["monitored"][key]["last_error"]
 
-        return "Last Error Info ({}):\n\n{}".format(args, errors)
+        return f"Last Error Info ({args}):\n\n{errors}"
```

### Comparing `stressor-0.5.2/stressor/stressor_cli.py` & `stressor-0.6.0/stressor/stressor_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
 """
 Stress-test your web app.
 
-(c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+(c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 
 Usage examples:
     $ stressor --help
     $ stressor run .
 """
+
 import argparse
 import logging
 import os
 import sys
 
 import yaml
 from snazzy import enable_colors
@@ -38,23 +38,23 @@
         # "dry_run": args.dry_run,
     }
     extra_context = {}
     # Parse `--option=NAME:VALUE` arguments:
     try:
         extra_context.update(parse_option_args(args.option, coerce_values=True))
     except Exception as e:
-        parser.error("--option: {}".format(e))
+        parser.error(f"--option: {e}")
     # Make sure that --dry-run arg is always honored:
     if args.dry_run:
         extra_context["dry_run"] = True
 
     scenario_fspec = args.scenario
     if os.path.isdir(scenario_fspec):
         scenario_fspec = os.path.join(scenario_fspec, "scenario.yaml")
-        logger.info("Looking for {}".format(scenario_fspec))
+        logger.info(f"Looking for {scenario_fspec}")
 
     rm = RunManager()
     rm.load_config(scenario_fspec)
     if args.single:
         rm.config_manager.config["force_single"] = True
     if args.max_time:
         rm.config_manager.config["max_time"] = float(args.max_time)
@@ -62,24 +62,24 @@
         rm.config_manager.config["max_errors"] = int(args.max_errors)
 
     res = rm.run(options, extra_context)
 
     if not res:
         logger.error("Finished with errors.")
         return 1
-    logger.info("Stressor run succesfully completed.")
+    logger.info("Stressor run successfully completed.")
     return 0
 
 
 def handle_init_command(parser, args):
     opts = {}
     if args.opts:
         if not os.path.isfile(args.opts):
-            parser.error("File not found: {}".format(args.opts))
-        with open(args.opts, "rt") as f:
+            parser.error(f"File not found: {args.opts}")
+        with open(args.opts) as f:
             opts = yaml.safe_load(f)
 
     opts.update(
         {
             "fspec": args.har_file,
             "target_folder": args.target,
             "force": args.force,
@@ -244,27 +244,27 @@
     if not args.no_color:
         # Enable snazzy colors and emojis if terminal supports them
         enable_colors(True, force=False)
 
     if getattr(args, "version", None):
         if args.verbose >= 4:
             info = version_info
-            info += "\nPython from: {}".format(sys.executable)
+            info += f"\nPython from: {sys.executable}"
         else:
             info = __version__
-        print(info)
+        print(info)  # noqa: T201
         sys.exit(0)
 
     if not callable(getattr(args, "command", None)):
         parser.error("missing command")
 
     try:
         return args.command(parser, args)
     except KeyboardInterrupt:
-        print("\nAborted by user.", file=sys.stderr)
+        print("\nAborted by user.", file=sys.stderr)  # noqa: T201
         sys.exit(3)
     # Unreachable...
     return
 
 
 # Script entry point
 if __name__ == "__main__":
```

### Comparing `stressor-0.5.2/stressor/util.py` & `stressor-0.6.0/stressor/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import logging
 import os
 import platform
 import random
@@ -34,17 +33,15 @@
 logging.Logger.important = log_important
 
 
 #: Check if a a string may be used as YAML dictionary key without using quotes.
 #: NOTE: YAML evaluates `0_` as "0" and `0_1_` as "1", so we don't accept leading numbers
 RE_YAML_KEYWORD = re.compile(r"^[a-zA-Z_]+\w*$")
 
-PYTHON_VERSION = "{}.{}.{}".format(
-    sys.version_info[0], sys.version_info[1], sys.version_info[2]
-)
+PYTHON_VERSION = f"{sys.version_info[0]}.{sys.version_info[1]}.{sys.version_info[2]}"
 version_info = "stressor/{} Python/{}({} bit) {}".format(
     __version__,
     PYTHON_VERSION,
     "64" if sys.maxsize > 2**32 else "32",
     platform.platform(),
 )
 
@@ -138,15 +135,15 @@
 
 def timetag(seconds=True, ms=False):
     """Return a time stamp string that can be used as (part of a) filename (also sorts well)."""
     now = datetime.now()
     if ms or seconds:
         s = now.strftime("%Y%m%d_%H%M%S")
         if ms:
-            s = "{}_{}".format(s, now.microsecond)
+            s = f"{s}_{now.microsecond}"
     else:
         s = now.strftime("%Y%m%d_%H%M")
     return s
 
 
 def check_cli_verbose(default=3):
     """Check for presence of `--verbose`/`--quiet` or `-v`/`-q` without using argparse."""
@@ -183,28 +180,28 @@
         datefmt="%H:%M:%S",
     )
     # Make sure it is set (when running from tox, the above basicConfig() did not set it)
     logger.setLevel(level)
 
     if path:
         if os.path.isdir(path):
-            fname = "stressor_{}.log".format(timetag())
+            fname = f"stressor_{timetag()}.log"
             path = os.path.join(path, fname)
-        logger.info("Writing log to '{}'".format(path))
+        logger.info(f"Writing log to '{path}'")
         if os.path.isfile(path):
-            logger.warning("Removing log file '{}'".format(path))
+            logger.warning(f"Removing log file '{path}'")
             os.remove(path)
         hdlr = logging.FileHandler(path)
         formatter = logging.Formatter(
             "%(asctime)s.%(msecs)-3d - %(levelname)s: %(message)s", "%H:%M:%S"
         )
         hdlr.setFormatter(formatter)
         logger.addHandler(hdlr)
         # logger.setLevel(logging.DEBUG)
-        logger.info("Start log ({})".format(datetime.now()))
+        logger.info(f"Start log ({datetime.now()})")
         logger.info(version_info)
         logger.info("Running {}".format(" ".join(sys.argv)))
 
         # redirect `logger` to our special log file as well:
         logger.addHandler(hdlr)
 
     # Silence requests `InsecureRequestWarning` messages
@@ -236,15 +233,15 @@
     try:
         import ctypes
         from ctypes import wintypes
 
         kernel32 = ctypes.WinDLL("kernel32", use_last_error=True)
         logger.info("Loaded kernel32 DLL on Windows.")
     except Exception as e:
-        logger.warning("Could not load kernel32 DLL on Windows: {}".format(e))
+        logger.warning(f"Could not load kernel32 DLL on Windows: {e}")
         return False
 
     CTRL_C_EVENT = 0
     CTRL_BREAK_EVENT = 1
     CTRL_CLOSE_EVENT = 2
 
     HANDLER_ROUTINE = ctypes.WINFUNCTYPE(wintypes.BOOL, wintypes.DWORD)
@@ -270,16 +267,14 @@
 
 def assert_always(condition, msg=None):
     """`assert` even in production code."""
     try:
         if not condition:
             raise AssertionError(msg) if msg is not None else AssertionError
     except AssertionError as e:
-        if sys.version_info < (3, 7):
-            raise
         # Strip last frames, so the exception's stacktrace points to the call
         # Credits: https://stackoverflow.com/a/58821552/19166
         _exc_type, _exc_value, traceback = sys.exc_info()
         back_frame = traceback.tb_frame.f_back
 
         back_tb = types.TracebackType(
             tb_next=None,
@@ -303,21 +298,17 @@
         if argument is None:
             return
         extra_msg = "`None` or "
     else:
         extra_msg = ""
 
     if not isinstance(argument, types):
-        raise TypeError(
-            "Expected {}{}, but got {}".format(extra_msg, types, type(argument))
-        )
+        raise TypeError(f"Expected {extra_msg}{types}, but got {type(argument)}")
     if condition is not NO_DEFAULT and not bool(condition):
-        raise ValueError(
-            "Invalid argument value: {} {}".format(type(argument), argument)
-        )
+        raise ValueError(f"Invalid argument value: {type(argument)} {argument}")
 
 
 def check_arg(argument, allowed_types, condition=NO_DEFAULT, or_none=False):
     """Check if `argument` has the expected type and value.
 
     **Note:** the exception's traceback is manipulated, so that the back frame
     points to the ``check_arg()`` line, instead of the actual ``raise``.
@@ -342,16 +333,14 @@
             check_arg(name, str)
             check_arg(amount, (int, float), amount > 0)
             check_arg(options, dict, or_none=True)
     """
     try:
         _check_arg(argument, allowed_types, condition, accept_none=or_none)
     except (TypeError, ValueError) as e:
-        if sys.version_info < (3, 7):
-            raise
         # Strip last frames, so the exception's stacktrace points to the call
         _exc_type, _exc_value, traceback = sys.exc_info()
         back_frame = traceback.tb_frame.f_back
 
         back_tb = types.TracebackType(
             tb_next=None,
             tb_frame=back_frame,
@@ -434,15 +423,15 @@
     check_arg(opt_list, list, or_none=True)
     res = {}
     if not opt_list:
         return res
     for opt in opt_list:
         # print(opt_list, opt)
         if ":" not in opt:
-            raise ValueError("Expected 'NAME:VALUE', got {!r}".format(opt))
+            raise ValueError(f"Expected 'NAME:VALUE', got {opt!r}")
         config_name, config_val = opt.split(":", 1)
         if coerce_values:
             res[config_name.strip()] = coerce_str(config_val)
         else:
             res[config_name.strip()] = config_val
     # print(opt_list, res)
     return res
@@ -493,28 +482,24 @@
     for arg_def in arg_defs:
         check_arg(arg_def, (list, tuple))
         if len(arg_def) == 2:
             arg_name, arg_type = arg_def
             arg_default = NO_DEFAULT
             if optional_mode:
                 raise AssertionError(
-                    "Mandatory arg definition must not follow optional args: `{}`".format(
-                        arg_def
-                    )
+                    f"Mandatory arg definition must not follow optional args: `{arg_def}`"
                 )
         elif len(arg_def) == 3:
             arg_name, arg_type, arg_default = arg_def
             optional_mode = True
         else:
-            raise AssertionError("Expected 2- or 3-tuple: {}".format(arg_def))
+            raise AssertionError(f"Expected 2- or 3-tuple: {arg_def}")
 
         if arg_type not in (float, int, str):
-            raise AssertionError(
-                "Unsupported argument definition type: {}".format(arg_def)
-            )
+            raise AssertionError(f"Unsupported argument definition type: {arg_def}")
 
         try:
             # Get next arg
             arg_val = arg_list.pop(0)
             # Allow quotes
             is_quoted = (arg_val.startswith('"') and arg_val.endswith('"')) or (
                 arg_val.startswith("'") and arg_val.endswith("'")
@@ -526,17 +511,15 @@
                 # The arg seems to be a macro: don't try to cast.
                 pass
             else:
                 # Raises ValueError:
                 arg_val = arg_type(arg_val)
         except IndexError:
             if arg_default is NO_DEFAULT:
-                raise ValueError(
-                    "Missing mandatory arg `{}` in '{}'.".format(arg_name, arg_str)
-                )
+                raise ValueError(f"Missing mandatory arg `{arg_name}` in '{arg_str}'.")
             arg_val = arg_default
 
         res[arg_name] = arg_val
 
     if arg_list:
         raise ValueError("Extra args `{}`.".format(", ".join(arg_list)))
 
@@ -562,17 +545,17 @@
     """Convert relative URL to absolute, using `root` as default."""
     return urljoin(root, url)
 
 
 def base_url(url):
     parsed_uri = urlparse(url)
     if parsed_uri.netloc:
-        res = "{uri.scheme}://{uri.netloc}{uri.path}".format(uri=parsed_uri)
+        res = f"{parsed_uri.scheme}://{parsed_uri.netloc}{parsed_uri.path}"
     else:
-        res = "{uri.path}".format(uri=parsed_uri)
+        res = f"{parsed_uri.path}"
     return res
 
 
 def shorten_string(long_string, max_chars, min_tail_chars=0, place_holder="[...]"):
     """Return string, shortened to max_chars characters.
 
     long_string = "This is a long string, that will be truncated."
@@ -650,48 +633,48 @@
     """Return elapsed time as H:M:S.h string with reasonable precision."""
     days, seconds = divmod(seconds, 86400) if seconds else (0, 0)
 
     if seconds >= 3600:
         m, s = divmod(seconds, 60)
         h, m = divmod(m, 60)
         if high_prec:
-            res = "{:d}:{:02d}:{:04.1f} hrs".format(int(h), int(m), s)
+            res = f"{int(h):d}:{int(m):02d}:{s:04.1f} hrs"
         else:
-            res = "{:d}:{:02d}:{:02d} hrs".format(int(h), int(m), int(s))
+            res = f"{int(h):d}:{int(m):02d}:{int(s):02d} hrs"
     elif seconds >= 60:
         m, s = divmod(seconds, 60)
         if high_prec:
-            res = "{:d}:{:05.2f} min".format(int(m), s)
+            res = f"{int(m):d}:{s:05.2f} min"
         else:
-            res = "{:d}:{:02d} min".format(int(m), int(s))
+            res = f"{int(m):d}:{int(s):02d} min"
     else:
         if high_prec:
             if seconds > 0.01:
-                res = "{:.3f} sec".format(seconds)
+                res = f"{seconds:.3f} sec"
             else:
-                res = "{:f} sec".format(seconds)
+                res = f"{seconds:f} sec"
         elif seconds > 5:
-            res = "{:.1f} sec".format(seconds)
+            res = f"{seconds:.1f} sec"
         else:
-            res = "{:.2f} sec".format(seconds)
+            res = f"{seconds:.2f} sec"
 
     if days == 1:
-        res = "{} day {}".format(int(days), res)
+        res = f"{int(days)} day {res}"
     elif days:
-        res = "{} days {}".format(int(days), res)
+        res = f"{int(days)} days {res}"
 
     if count and (seconds > 0):
-        res += ", {:,.1f} {}/sec".format(float(count) / seconds, unit)
+        res += f", {float(count) / seconds:,.1f} {unit}/sec"
     return res
 
 
 def format_num(num):
     """Return num rounded to reasonable precision (promille)."""
     if num >= 1000.0:
-        res = "{:,}".format(round(num))
+        res = f"{round(num):,}"
     elif num >= 100.0:
         res = str(round(num, 1))
         # res = "{:,.1f}".format(num)
     elif num >= 10.0:
         res = str(round(num, 2))
         # res = "{:,.2f}".format(num)
     elif num >= 1.0:
@@ -706,21 +689,21 @@
 def format_rate(count, time, unit=None, high_prec=False):
     """Return count / time with reasonable precision."""
     if not time or not count:
         return "0"
 
     rate = float(count) / float(time)
     if rate >= 1000:
-        res = "{}".format(int(round(rate)))
+        res = f"{int(round(rate))}"
     elif rate >= 100:
-        res = "{}".format(round(rate, 1))
+        res = f"{round(rate, 1)}"
     elif rate >= 10:
-        res = "{}".format(round(rate, 2))
+        res = f"{round(rate, 2)}"
     else:
-        res = "{}".format(round(rate, 3))
+        res = f"{round(rate, 3)}"
     return res
 
 
 # def format_relative_datetime(dt, as_html=False):
 #     """Format a datetime object as relative expression (i.e. '3 minutes ago')."""
 #     try:
 #         diff = datetime.utcnow() - dt
```

### Comparing `stressor-0.5.2/stressor.egg-info/PKG-INFO` & `stressor-0.6.0/stressor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stressor
-Version: 0.5.2
+Version: 0.6.0
 Summary: Stress-test your web app
 Home-page: https://github.com/mar10/stressor
 Author: Martin Wendt
 Author-email: stressor@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: stressor@wwwendt.de
 License: MIT
@@ -19,97 +19,103 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: fabulist
+Requires-Dist: lxml
+Requires-Dist: python-dateutil
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: snazzy
 
 # ![logo](https://raw.githubusercontent.com/mar10/stressor/master/stressor/monitor/htdocs/stressor_48x48.png) stressor
-[![Build Status](https://travis-ci.com/mar10/stressor.svg?branch=master)](https://app.travis-ci.com/github/mar10/stressor)
+
+[![Tests](https://github.com/mar10/stressor/actions/workflows/tests.yml/badge.svg)](https://github.com/mar10/stressor/actions/workflows/tests.yml)
 [![Latest Version](https://img.shields.io/pypi/v/stressor.svg)](https://pypi.python.org/pypi/stressor/)
 [![License](https://img.shields.io/pypi/l/stressor.svg)](https://github.com/mar10/stressor/blob/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/stressor/badge/?version=latest)](http://stressor.readthedocs.io/)
-[![Coverage Status](https://coveralls.io/repos/github/mar10/stressor/badge.svg?branch=master)](https://coveralls.io/github/mar10/stressor?branch=master)
+[![codecov](https://codecov.io/github/mar10/stressor/graph/badge.svg?token=WW9WQ0R0JL)](https://codecov.io/github/mar10/stressor)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: stressor](https://img.shields.io/badge/StackOverflow-stressor-blue.svg)](https://stackoverflow.com/questions/tagged/stressor)
 
 > Stress-test your web app.
 
-*Stressor* is a tool, that runs a sequence of activities in one or more
+_Stressor_ is a tool, that runs a sequence of activities in one or more
 parallel sessions.
 The most common use case is to run a test script with HTTP commands
 against a web server, simulating a bunch of parallel user sessions.
 As a result we get metrics about reponse times, failures, resource usage,
 etc.
 
 Stressor can be used for testing, benchmarking, load testing, or to generate
 test data.
 Stressor comes with prebuilt activities for HTTP-request and more, and can be
 extended by custom activity-plugins.
 
 Test scripts can be defined as text files, using a special syntax, that is then
 executed by the `stressor` command line tool.
 Stressor is also an Open Source Python library that can be included into your
-own projects. This allows to define test *scenarios* programmtically.
-
+own projects. This allows to define test _scenarios_ programmtically.
 
 ## Quickstart
 
-1. Install *stressor* ([details](https://stressor.readthedocs.io/en/latest/installation.html))
+1. Install _stressor_ ([details](https://stressor.readthedocs.io/en/latest/installation.html))
 
 2. Create a new scenario folder. For example:
 
-    ```bash
-    $ stressor init ./scenario_1
-    ```
-
-    or alternatively import an existing HAR file as a starting point
-    ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html#importing-har-files)):
-
-    ```bash
-    $ stressor init ./scenario_1 --convert /path/to/output.har
-    ```
+   ```bash
+   $ stressor init ./scenario_1
+   ```
+
+   or alternatively import an existing HAR file as a starting point
+   ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html#importing-har-files)):
+
+   ```bash
+   $ stressor init ./scenario_1 --convert /path/to/output.har
+   ```
 
-3. Edit the scripts as needed (*users.yaml*, *main_sequence.yaml*, *scenario.yaml*)
-  ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html))
+3. Edit the scripts as needed (_users.yaml_, _main_sequence.yaml_, _scenario.yaml_)
+   ([details](https://stressor.readthedocs.io/en/latest/ug_writing_scripts.html))
 
 4. Run the script:
 
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml
-    ```
-
-    Use the `--monitor` option to view the progress in a separate window:
-
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml --monitor
-    ```
-
-    Use the `--log` argument to write output to a file or folder:
-
-    ```bash
-    $ stressor run ./scenario_1/scenario.yaml --no-color --log .
-    ```
-    (Hit <kbd>Ctrl</kbd>+<kbd>C</kbd> to stop.)
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml
+   ```
+
+   Use the `--monitor` option to view the progress in a separate window:
+
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml --monitor
+   ```
+
+   Use the `--log` argument to write output to a file or folder:
+
+   ```bash
+   $ stressor run ./scenario_1/scenario.yaml --no-color --log .
+   ```
+
+   (Hit <kbd>Ctrl</kbd>+<kbd>C</kbd> to stop.)
 
 5. [Read The Docs](https://stressor.readthedocs.io/en/latest/ug_tutorial.html)
    for details.
 
 <img src="https://stressor.readthedocs.io/en/latest/_images/summary.png">
 
 <img src="https://stressor.readthedocs.io/en/latest/_images/teaser.png">
```

### Comparing `stressor-0.5.2/stressor.egg-info/SOURCES.txt` & `stressor-0.6.0/stressor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stressor-0.5.2/tests/test_config_manager.py` & `stressor-0.6.0/tests/test_config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import os
 
 import pytest
```

### Comparing `stressor-0.5.2/tests/test_context_stack.py` & `stressor-0.6.0/tests/test_context_stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 
 import os
 
 import pytest
@@ -57,8 +56,8 @@
         with pytest.raises(IndexError):
             cm.pop()
         with pytest.raises(IndexError):
             cm.peek()
 
         with pytest.raises(RuntimeError):
             for i in range(ContextStack.MAX_DEPTH + 1):
-                cm.push("t{:02}".format(i), {})
+                cm.push(f"t{i:02}", {})
```

### Comparing `stressor-0.5.2/tests/test_convert.py` & `stressor-0.6.0/tests/test_convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 
 import os
 import tempfile
 
@@ -25,15 +24,15 @@
                 "fspec": os.path.join(self.fixtures_path, "har_1.har"),
                 "target_folder": target_folder,
                 "collate_max_len": 0,
             }
             conv = HarConverter(opts)
             conv.run()
             act_yaml_path = os.path.join(target_folder, "main_sequence.yaml")
-            yaml = open(act_yaml_path, "rt").read()
+            yaml = open(act_yaml_path).read()
             # print(yaml)
             assert len(conv.entries) == 5
             assert conv.har_version == "1.2"
         assert "activity: GetRequest" in yaml
         assert "url: '/test1.json'" in yaml
         # assert 'url: "http://127.0.0.1:8082/test1.json"' in yaml
         # assert 0
```

### Comparing `stressor-0.5.2/tests/test_plugin_manager.py` & `stressor-0.6.0/tests/test_plugin_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 from stressor.plugin_manager import PluginManager
 
 
 class TestPluginManager:
```

### Comparing `stressor-0.5.2/tests/test_run_manager.py` & `stressor-0.6.0/tests/test_run_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
+# ruff: noqa: T201, T203 `print` found
+
 import os
 
 from stressor.run_manager import RunManager
 from stressor.session_manager import User
 
 
 class TestRunManager:
```

### Comparing `stressor-0.5.2/tests/test_script_activities.py` & `stressor-0.6.0/tests/test_script_activities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
+# ruff: noqa: T201, T203 `print` found
+
 import os
 from textwrap import dedent
 
 
 class TestScripts:
     def setup_method(self):
         self.fixtures_path = os.path.join(os.path.dirname(__file__), "fixtures")
@@ -51,11 +52,11 @@
             #     # "__builtins__": None,
             #     "foo": "bar",
             # },
             local_vars,
         )
         assert res is None
         print("New built-ins:", set(__builtins__.keys()).difference(prev_builtins))
-        print("Result: {}".format(res))
-        print("Globals: {}".format(global_vars.keys()))
-        print("Locals: {}".format(local_vars))
+        print(f"Result: {res}")
+        print(f"Globals: {global_vars.keys()}")
+        print(f"Locals: {local_vars}")
         # assert 0
```

### Comparing `stressor-0.5.2/tests/test_util.py` & `stressor-0.6.0/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2020-2023 Martin Wendt and contributors; see https://github.com/mar10/stressor
+# (c) 2020-2024 Martin Wendt and contributors; see https://github.com/mar10/stressor
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import pytest
 
 from stressor.util import (
     PathStack,
@@ -160,15 +159,15 @@
         assert format_rate(12345, 10000.0) == "1.234"
         assert format_rate(12345, 100000.0) == "0.123"
         assert format_rate(12345, 1000000.0) == "0.012"
 
     def test_coerce_str(self):
         assert coerce_str("1.2") == 1.2
         assert coerce_str("1") == 1
-        assert type(coerce_str("1")) is int
+        assert isinstance(coerce_str("1"), int)
         assert coerce_str("") == ""
         assert coerce_str("1.2.3") == "1.2.3"
         assert coerce_str(None) is None
 
     def test_parse_option_args(self):
         res = parse_option_args([])
         assert res == {}
```

