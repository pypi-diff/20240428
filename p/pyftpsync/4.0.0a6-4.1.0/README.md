# Comparing `tmp/pyftpsync-4.0.0a6.tar.gz` & `tmp/pyftpsync-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftpsync-4.0.0a6.tar", last modified: Sun Jul 31 11:43:07 2022, max compression
+gzip compressed data, was "pyftpsync-4.1.0.tar", last modified: Sun Apr 28 10:29:41 2024, max compression
```

## Comparing `pyftpsync-4.0.0a6.tar` & `pyftpsync-4.1.0.tar`

### file list

```diff
@@ -1,33 +1,48 @@
-drwxrwxrwx   0        0        0        0 2022-07-31 11:43:07.417122 pyftpsync-4.0.0a6/
--rw-rw-rw-   0        0        0     1099 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/LICENSE.txt
--rw-rw-rw-   0        0        0       61 2021-12-29 12:37:58.000000 pyftpsync-4.0.0a6/MANIFEST.in
--rw-rw-rw-   0        0        0     3963 2022-07-31 11:43:07.418122 pyftpsync-4.0.0a6/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2022-07-06 10:56:03.000000 pyftpsync-4.0.0a6/README.md
-drwxrwxrwx   0        0        0        0 2022-07-31 11:43:07.405260 pyftpsync-4.0.0a6/ftpsync/
--rw-rw-rw-   0        0        0      469 2022-07-03 15:33:04.000000 pyftpsync-4.0.0a6/ftpsync/__init__.py
--rw-rw-rw-   0        0        0     3866 2022-07-06 10:56:03.000000 pyftpsync-4.0.0a6/ftpsync/cli_common.py
--rw-rw-rw-   0        0        0    31936 2022-07-04 08:06:43.000000 pyftpsync-4.0.0a6/ftpsync/ftp_target.py
--rw-rw-rw-   0        0        0     9434 2022-07-04 08:06:56.000000 pyftpsync-4.0.0a6/ftpsync/metadata.py
--rw-rw-rw-   0        0        0    11239 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/pyftpsync.py
--rw-rw-rw-   0        0        0    14782 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/resources.py
--rw-rw-rw-   0        0        0    11627 2022-07-10 14:57:22.000000 pyftpsync-4.0.0a6/ftpsync/run_command.py
--rw-rw-rw-   0        0        0     4523 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/scan_command.py
--rw-rw-rw-   0        0        0    21448 2022-07-04 08:06:43.000000 pyftpsync-4.0.0a6/ftpsync/sftp_target.py
--rw-rw-rw-   0        0        0    51105 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/synchronizers.py
--rw-rw-rw-   0        0        0    19900 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/targets.py
--rw-rw-rw-   0        0        0     2504 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/tree_command.py
--rw-rw-rw-   0        0        0    16118 2022-07-04 06:47:21.000000 pyftpsync-4.0.0a6/ftpsync/util.py
-drwxrwxrwx   0        0        0        0 2022-07-31 11:43:07.417122 pyftpsync-4.0.0a6/pyftpsync.egg-info/
--rw-rw-rw-   0        0        0     3963 2022-07-31 11:43:07.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2022-07-31 11:43:07.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-31 11:43:07.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-07-31 11:43:07.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-06-19 11:52:10.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2022-07-31 11:43:07.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-31 11:43:07.000000 pyftpsync-4.0.0a6/pyftpsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      566 2022-06-19 08:17:19.000000 pyftpsync-4.0.0a6/pyproject.toml
--rw-rw-rw-   0        0        0      858 2022-07-31 10:09:07.000000 pyftpsync-4.0.0a6/readme_pypi.rst
--rw-rw-rw-   0        0        0      259 2022-07-31 10:09:17.000000 pyftpsync-4.0.0a6/requirements-dev.txt
--rw-rw-rw-   0        0        0       62 2021-12-29 12:37:58.000000 pyftpsync-4.0.0a6/requirements.txt
--rw-rw-rw-   0        0        0     2365 2022-07-31 11:43:07.419123 pyftpsync-4.0.0a6/setup.cfg
--rw-rw-rw-   0        0        0      178 2022-07-31 10:09:17.000000 pyftpsync-4.0.0a6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:29:41.959693 pyftpsync-4.1.0/
+-rw-rw-rw-   0        0        0     5094 2024-04-28 10:26:29.000000 pyftpsync-4.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1099 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       61 2021-12-29 12:37:58.000000 pyftpsync-4.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4405 2024-04-28 10:29:41.958450 pyftpsync-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2687 2024-04-28 10:04:59.000000 pyftpsync-4.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 10:29:41.933614 pyftpsync-4.1.0/ftpsync/
+-rw-rw-rw-   0        0        0      441 2024-04-28 10:29:39.000000 pyftpsync-4.1.0/ftpsync/__init__.py
+-rw-rw-rw-   0        0        0     3843 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/cli_common.py
+-rw-rw-rw-   0        0        0    31629 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/ftp_target.py
+-rw-rw-rw-   0        0        0     9383 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/metadata.py
+-rw-rw-rw-   0        0        0    11208 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/pyftpsync.py
+-rw-rw-rw-   0        0        0    14653 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/resources.py
+-rw-rw-rw-   0        0        0    11609 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/run_command.py
+-rw-rw-rw-   0        0        0     4455 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/scan_command.py
+-rw-rw-rw-   0        0        0    21300 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/sftp_target.py
+-rw-rw-rw-   0        0        0    50896 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/synchronizers.py
+-rw-rw-rw-   0        0        0    19854 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/targets.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/tree_command.py
+-rw-rw-rw-   0        0        0    15468 2024-04-28 10:02:58.000000 pyftpsync-4.1.0/ftpsync/util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:29:41.958450 pyftpsync-4.1.0/pyftpsync.egg-info/
+-rw-rw-rw-   0        0        0     4405 2024-04-28 10:29:41.000000 pyftpsync-4.1.0/pyftpsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2024-04-28 10:29:41.000000 pyftpsync-4.1.0/pyftpsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 10:29:41.000000 pyftpsync-4.1.0/pyftpsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-28 10:29:41.000000 pyftpsync-4.1.0/pyftpsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-06-19 11:52:10.000000 pyftpsync-4.1.0/pyftpsync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2024-04-28 10:29:41.000000 pyftpsync-4.1.0/pyftpsync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 10:29:41.000000 pyftpsync-4.1.0/pyftpsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1147 2024-04-28 10:00:01.000000 pyftpsync-4.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      997 2024-04-28 10:04:49.000000 pyftpsync-4.1.0/readme_pypi.rst
+-rw-rw-rw-   0        0        0      210 2024-04-28 10:01:04.000000 pyftpsync-4.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2024-04-28 10:00:01.000000 pyftpsync-4.1.0/requirements.txt
+-rw-rw-rw-   0        0        0     2118 2024-04-28 10:29:41.966695 pyftpsync-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      178 2022-07-31 10:09:17.000000 pyftpsync-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:29:41.957451 pyftpsync-4.1.0/tests/
+-rw-rw-rw-   0        0        0     9231 2022-06-19 11:57:43.000000 pyftpsync-4.1.0/tests/test_1x.py
+-rw-rw-rw-   0        0        0    10930 2021-12-29 12:37:58.000000 pyftpsync-4.1.0/tests/test_1x_ftp.py
+-rw-rw-rw-   0        0        0     6850 2022-06-19 11:49:04.000000 pyftpsync-4.1.0/tests/test_basic.py
+-rw-rw-rw-   0        0        0     4123 2021-12-29 12:37:58.000000 pyftpsync-4.1.0/tests/test_bench.py
+-rw-rw-rw-   0        0        0     2183 2024-04-28 10:24:25.000000 pyftpsync-4.1.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0     3995 2023-03-13 17:16:38.000000 pyftpsync-4.1.0/tests/test_develop.py
+-rw-rw-rw-   0        0        0     2672 2021-12-29 12:37:58.000000 pyftpsync-4.1.0/tests/test_regressions.py
+-rw-rw-rw-   0        0        0     4376 2022-06-19 11:49:34.000000 pyftpsync-4.1.0/tests/test_scan.py
+-rw-rw-rw-   0        0        0     2864 2021-12-29 12:37:58.000000 pyftpsync-4.1.0/tests/test_sftp.py
+-rw-rw-rw-   0        0        0    17757 2023-03-13 17:16:38.000000 pyftpsync-4.1.0/tests/test_sync_bidir.py
+-rw-rw-rw-   0        0        0    10263 2022-06-19 11:50:03.000000 pyftpsync-4.1.0/tests/test_sync_download.py
+-rw-rw-rw-   0        0        0    10171 2022-06-19 11:50:15.000000 pyftpsync-4.1.0/tests/test_sync_upload.py
+-rw-rw-rw-   0        0        0     3466 2022-06-19 11:50:22.000000 pyftpsync-4.1.0/tests/test_tree.py
```

### Comparing `pyftpsync-4.0.0a6/LICENSE.txt` & `pyftpsync-4.1.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) 2012-2022 Martin Wendt
+Copyright (c) 2012-2024 Martin Wendt
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyftpsync-4.0.0a6/PKG-INFO` & `pyftpsync-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftpsync
-Version: 4.0.0a6
+Version: 4.1.0
 Summary: Synchronize directories using FTP(S), SFTP, or file system access
 Home-page: https://github.com/mar10/pyftpsync
 Author: Martin Wendt
 Author-email: pyftpsync@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: pyftpsync@wwwendt.de
 License: MIT
@@ -19,74 +19,83 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: colorama
+Requires-Dist: keyring
+Requires-Dist: pysftp
+Requires-Dist: PyYAML
 
 # ![logo](https://raw.githubusercontent.com/mar10/pyftpsync/master/docs/logo_48x48.png) pyftpsync
-[![Build Status](https://travis-ci.com/mar10/pyftpsync.svg?branch=master)](https://app.travis-ci.com/github/mar10/pyftpsync)
+
+[![Tests](https://github.com/mar10/pyftpsync/actions/workflows/python-app.yml/badge.svg)](https://github.com/mar10/pyftpsync/actions/workflows/python-app.yml)
 [![Latest Version](https://img.shields.io/pypi/v/pyftpsync.svg)](https://pypi.python.org/pypi/pyftpsync/)
 [![License](https://img.shields.io/pypi/l/pyftpsync.svg)](https://github.com/mar10/pyftpsync/blob/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/pyftpsync/badge/?version=latest)](https://pyftpsync.readthedocs.io/)
+[![codecov](https://codecov.io/github/mar10/pyftpsync/graph/badge.svg?token=0JM9CN8RYW)](https://codecov.io/github/mar10/pyftpsync)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: pyftpsync](https://img.shields.io/badge/StackOverflow-pyftpsync-blue.svg)](https://stackoverflow.com/questions/tagged/pyftpsync)
 
 > Synchronize directories using FTP(S), SFTP, or file system access.
 
 [ ![sample](teaser.png?raw=true) ](https://github.com/mar10/pyftpsync "Live demo")
 
-
 ## Summary
 
 Synchronize directories using FTP(S), SFTP, or file system access.
 
-  * This is a command line tool...
-  * ... and a library for use in your Python projects.
-  * Upload, download, and bi-directional synch mode.
-  * Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
-  * Architecture is open to add other target types.
+-   This is a command line tool...
+-   ... and a library for use in your Python projects.
+-   Upload, download, and bi-directional synch mode.
+-   Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
+-   Architecture is open to add other target types.
 
 **Note:** Version 4.0 drops support for Python 2.
 
-
 ## Quickstart
 
-[Python](https://www.python.org/download/Python) 3.7+ is required,
+[Python](https://www.python.org/download/Python) 3.8+ is required,
 [pip](http://www.pip-installer.org/) recommended:
 
 ```bash
 $ pip install pyftpsync --upgrade
 $ pyftpsync --help
 ```
 
-See [Command Line Interface](https://pyftpsync.readthedocs.io/en/latest/ug_cli.html) 
+**Note:** <br>
+MS Windows users that only need the command line interface may prefer the
+[MSI Installer](https://github.com/mar10/pyftpsync/releases/latest) or install
+using the Windows Package Manager:
+
+```ps1
+> winget install pyftpsync
+```
+
+See [Command Line Interface](https://pyftpsync.readthedocs.io/en/latest/ug_cli.html)
 for details.
 
 In addition to the direct invocation of `upload`, `download`, or `sync`
-commands, version 3.x allows to define a ``pyftpsync_yaml`` file
+commands, version 3.x allows to define a `pyftpsync_yaml` file
 in your project's root folder which then can be executed like so::
 
     $ pyftpsync run
 
-See [Run from pyftpsync.yaml](https://pyftpsync.readthedocs.io/en/latest/ug_run.html) 
+See [Run from pyftpsync.yaml](https://pyftpsync.readthedocs.io/en/latest/ug_run.html)
 for details.
 
-
-**Note:** Windows users may prefer the 
-[MSI Installer](https://github.com/mar10/pyftpsync/releases/latest).
-
-
 ## Documentation
 
 [Read the Docs](https://pyftpsync.readthedocs.io/) for details.
```

### Comparing `pyftpsync-4.0.0a6/README.md` & `pyftpsync-4.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 # ![logo](https://raw.githubusercontent.com/mar10/pyftpsync/master/docs/logo_48x48.png) pyftpsync
-[![Build Status](https://travis-ci.com/mar10/pyftpsync.svg?branch=master)](https://app.travis-ci.com/github/mar10/pyftpsync)
+
+[![Tests](https://github.com/mar10/pyftpsync/actions/workflows/python-app.yml/badge.svg)](https://github.com/mar10/pyftpsync/actions/workflows/python-app.yml)
 [![Latest Version](https://img.shields.io/pypi/v/pyftpsync.svg)](https://pypi.python.org/pypi/pyftpsync/)
 [![License](https://img.shields.io/pypi/l/pyftpsync.svg)](https://github.com/mar10/pyftpsync/blob/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/pyftpsync/badge/?version=latest)](https://pyftpsync.readthedocs.io/)
+[![codecov](https://codecov.io/github/mar10/pyftpsync/graph/badge.svg?token=0JM9CN8RYW)](https://codecov.io/github/mar10/pyftpsync)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: pyftpsync](https://img.shields.io/badge/StackOverflow-pyftpsync-blue.svg)](https://stackoverflow.com/questions/tagged/pyftpsync)
 
 > Synchronize directories using FTP(S), SFTP, or file system access.
 
 [ ![sample](teaser.png?raw=true) ](https://github.com/mar10/pyftpsync "Live demo")
 
-
 ## Summary
 
 Synchronize directories using FTP(S), SFTP, or file system access.
 
-  * This is a command line tool...
-  * ... and a library for use in your Python projects.
-  * Upload, download, and bi-directional synch mode.
-  * Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
-  * Architecture is open to add other target types.
+-   This is a command line tool...
+-   ... and a library for use in your Python projects.
+-   Upload, download, and bi-directional synch mode.
+-   Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
+-   Architecture is open to add other target types.
 
 **Note:** Version 4.0 drops support for Python 2.
 
-
 ## Quickstart
 
-[Python](https://www.python.org/download/Python) 3.7+ is required,
+[Python](https://www.python.org/download/Python) 3.8+ is required,
 [pip](http://www.pip-installer.org/) recommended:
 
 ```bash
 $ pip install pyftpsync --upgrade
 $ pyftpsync --help
 ```
 
-See [Command Line Interface](https://pyftpsync.readthedocs.io/en/latest/ug_cli.html) 
+**Note:** <br>
+MS Windows users that only need the command line interface may prefer the
+[MSI Installer](https://github.com/mar10/pyftpsync/releases/latest) or install
+using the Windows Package Manager:
+
+```ps1
+> winget install pyftpsync
+```
+
+See [Command Line Interface](https://pyftpsync.readthedocs.io/en/latest/ug_cli.html)
 for details.
 
 In addition to the direct invocation of `upload`, `download`, or `sync`
-commands, version 3.x allows to define a ``pyftpsync_yaml`` file
+commands, version 3.x allows to define a `pyftpsync_yaml` file
 in your project's root folder which then can be executed like so::
 
     $ pyftpsync run
 
-See [Run from pyftpsync.yaml](https://pyftpsync.readthedocs.io/en/latest/ug_run.html) 
+See [Run from pyftpsync.yaml](https://pyftpsync.readthedocs.io/en/latest/ug_run.html)
 for details.
 
-
-**Note:** Windows users may prefer the 
-[MSI Installer](https://github.com/mar10/pyftpsync/releases/latest).
-
-
 ## Documentation
 
 [Read the Docs](https://pyftpsync.readthedocs.io/) for details.
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/cli_common.py` & `pyftpsync-4.1.0/ftpsync/cli_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
+
 import argparse
 
 from ftpsync.synchronizers import DEFAULT_OMIT
 
 # --- verbose_parser ----------------------------------------------------------
 
 verbose_parser = argparse.ArgumentParser(add_help=False)
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/ftp_target.py` & `pyftpsync-4.1.0/ftpsync/ftp_target.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
+
 import calendar
 import codecs
 import ftplib
 import json
 import os
 import time
 from posixpath import join as join_url
@@ -114,15 +114,15 @@
     def __str__(self):
         return "<{} + {}>".format(
             self.get_base_name(), relpath_url(self.cur_dir or "/", self.root_dir)
         )
 
     def get_base_name(self):
         scheme = "ftps" if self.tls else "ftp"
-        return "{}://{}{}".format(scheme, self.host, self.root_dir)
+        return f"{scheme}://{self.host}{self.root_dir}"
 
     def open(self):
         assert not self.ftp_socket_connected
 
         super().open()
 
         options = self.get_options_dict()
@@ -164,17 +164,15 @@
                     )
                 break
             except ftplib.error_perm as e:
                 # If credentials were passed, but authentication fails, prompt
                 # for new password
                 if not e.args[0].startswith("530"):
                     raise  # error other then '530 Login incorrect'
-                write_error(
-                    "Could not login to {}@{}: {}".format(self.username, self.host, e)
-                )
+                write_error(f"Could not login to {self.username}@{self.host}: {e}")
                 if no_prompt or not self.username:
                     raise
                 creds = prompt_for_password(self.host, self.username)
                 self.username, self.password = creds
                 # Continue while-loop
 
         if self.tls:
@@ -184,23 +182,23 @@
         try:
             self.syst_response = self.ftp.sendcmd("SYST")
             if verbose >= 5:
                 write("SYST: '{}'.".format(self.syst_response.replace("\n", " ")))
             # self.is_unix = "unix" in resp.lower() # not necessarily true, better check with r/w tests
             # TODO: case sensitivity?
         except Exception as e:
-            write("SYST command failed: '{}'".format(e))
+            write(f"SYST command failed: '{e}'")
 
         try:
             self.feat_response = self.ftp.sendcmd("FEAT")
             self.support_utf8 = "UTF8" in self.feat_response
             if verbose >= 5:
                 write("FEAT: '{}'.".format(self.feat_response.replace("\n", " ")))
         except Exception as e:
-            write("FEAT command failed: '{}'".format(e))
+            write(f"FEAT command failed: '{e}'")
 
         if self.encoding == "utf-8":
             if not self.support_utf8 and verbose >= 4:
                 write(
                     "Server does not list utf-8 as supported feature (using it anyway).",
                     warning=True,
                 )
@@ -210,26 +208,26 @@
                 # See https://tools.ietf.org/html/draft-ietf-ftpext-utf-8-option-00
                 # Note: this RFC is inactive, expired, and failed on Strato
                 self.ftp.sendcmd("OPTS UTF-8")
                 if verbose >= 4:
                     write("Sent 'OPTS UTF-8'.")
             except Exception as e:
                 if verbose >= 4:
-                    write("Could not send 'OPTS UTF-8': '{}'".format(e), warning=True)
+                    write(f"Could not send 'OPTS UTF-8': '{e}'", warning=True)
 
             try:
                 # Announce our wish to use UTF-8 to the server as proposed here:
                 # See https://tools.ietf.org/html/rfc2389
                 # https://www.cerberusftp.com/phpBB3/viewtopic.php?t=2608
                 # Note: this was accepted on Strato
                 self.ftp.sendcmd("OPTS UTF8 ON")
                 if verbose >= 4:
                     write("Sent 'OPTS UTF8 ON'.")
             except Exception as e:
-                write("Could not send 'OPTS UTF8 ON': '{}'".format(e), warning=True)
+                write(f"Could not send 'OPTS UTF8 ON': '{e}'", warning=True)
 
         if hasattr(self.ftp, "encoding"):
             # Python 3 encodes using latin-1 by default(!)
             # (In Python 2 ftp.encoding does not exist, but ascii is used)
             if self.encoding != codecs.lookup(self.ftp.encoding).name:
                 write(
                     "Setting FTP encoding to {} (was {}).".format(
@@ -296,15 +294,15 @@
         if self.lock_data:
             self._unlock(closing=True)
 
         if self.ftp_socket_connected:
             try:
                 self.ftp.quit()
             except (ConnectionError, EOFError) as e:
-                write_error("ftp.quit() failed: {}".format(e))
+                write_error(f"ftp.quit() failed: {e}")
             self.ftp_socket_connected = False
 
         super().close()
 
     def _lock(self, break_existing=False):
         """Write a special file to the target root folder."""
         # write("_lock")
@@ -312,16 +310,16 @@
 
         try:
             assert self.cur_dir == self.root_dir
             self.write_text(DirMetadata.LOCK_FILE_NAME, json.dumps(data))
             self.lock_data = data
             self.lock_write_time = time.time()
         except Exception as e:
-            errmsg = "{}".format(e)
-            write_error("Could not write lock file: {}".format(errmsg))
+            errmsg = f"{e}"
+            write_error(f"Could not write lock file: {errmsg}")
             if errmsg.startswith("550") and self.ftp.passiveserver:
                 try:
                     self.ftp.makepasv()
                 except Exception:
                     write_error(
                         "The server probably requires FTP Active mode. "
                         "Try passing the --ftp-active option."
@@ -367,36 +365,36 @@
                     if e.args[0][:3] == "226":
                         write_error("Ignoring 226 response for ftp.delete() lockfile")
                     else:
                         raise
 
             self.lock_data = None
         except Exception as e:
-            write_error("Could not remove lock file: {}".format(e))
+            write_error(f"Could not remove lock file: {e}")
             raise
 
     def _probe_lock_file(self, reported_mtime):
         """Called by get_dir"""
         delta = reported_mtime - self.lock_data["lock_time"]
         # delta2 = reported_mtime - self.lock_write_time
         self.server_time_ofs = delta
         if self.get_option("verbose", 3) >= 4:
-            write("Server time offset: {:.2f} seconds.".format(delta))
+            write(f"Server time offset: {delta:.2f} seconds.")
             # write("Server time offset2: {:.2f} seconds.".format(delta2))
 
     def get_id(self):
         return self.host + self.root_dir
 
     def cwd(self, dir_name):
         assert is_native(dir_name)
         path = normpath_url(join_url(self.cur_dir, dir_name))
         if not path.startswith(self.root_dir):
             # paranoic check to prevent that our sync tool goes berserk
             raise RuntimeError(
-                "Tried to navigate outside root {!r}: {!r}".format(self.root_dir, path)
+                f"Tried to navigate outside root {self.root_dir!r}: {path!r}"
             )
         self.ftp.cwd(dir_name)
         self.cur_dir = path
         self.cur_dir_meta = None
         return self.cur_dir
 
     def pwd(self):
@@ -520,17 +518,17 @@
                     # local upload time
                     self._probe_lock_file(mtime)
                 else:
                     entry = FileEntry(self, self.cur_dir, name, size, mtime, unique)
             elif res_type in ("cdir", "pdir"):
                 pass
             else:
-                write_error("Could not parse '{}'".format(line))
+                write_error(f"Could not parse '{line}'")
                 raise NotImplementedError(
-                    "MLSD returned unsupported type: {!r}".format(res_type)
+                    f"MLSD returned unsupported type: {res_type!r}"
                 )
 
             if entry:
                 entry_map[name] = entry
                 entry_list.append(entry)
 
         try:
@@ -551,17 +549,15 @@
 
         if local_var["has_meta"]:
             try:
                 self.cur_dir_meta.read()
             except IncompatibleMetadataVersionError:
                 raise  # this should end the script (user should pass --migrate)
             except Exception as e:
-                write_error(
-                    "Could not read meta info {}: {}".format(self.cur_dir_meta, e)
-                )
+                write_error(f"Could not read meta info {self.cur_dir_meta}: {e}")
 
             meta_files = self.cur_dir_meta.list
 
             # Adjust file mtime from meta-data if present
             missing = []
             for n in meta_files:
                 meta = meta_files[n]
@@ -617,17 +613,15 @@
             name (str): file name, located in self.curdir
         Returns:
             file-like (must support read() method)
         """
         # print("FTP open_readable({})".format(name))
         assert is_native(name)
         out = SpooledTemporaryFile(max_size=self.MAX_SPOOL_MEM, mode="w+b")
-        self.ftp.retrbinary(
-            "RETR {}".format(name), out.write, FTPTarget.DEFAULT_BLOCKSIZE
-        )
+        self.ftp.retrbinary(f"RETR {name}", out.write, FTPTarget.DEFAULT_BLOCKSIZE)
         out.seek(0)
         return out
 
     def write_file(self, name, fp_src, blocksize=DEFAULT_BLOCKSIZE, callback=None):
         """Write file-like `fp_src` to cur_dir/name.
 
         Args:
@@ -636,15 +630,15 @@
             blocksize (int, optional):
             callback (function, optional):
                 Called like `func(buf)` for every written chunk
         """
         # print("FTP write_file({})".format(name), blocksize)
         assert is_native(name)
         self.check_write(name)
-        self.ftp.storbinary("STOR {}".format(name), fp_src, blocksize, callback)
+        self.ftp.storbinary(f"STOR {name}", fp_src, blocksize, callback)
         # TODO: check result
 
     def copy_to_file(self, name, fp_dest, callback=None):
         """Write cur_dir/name to file-like `fp_dest`.
 
         Args:
             name (str): file name, located in self.curdir
@@ -656,17 +650,15 @@
 
         def _write_to_file(data):
             # print("_write_to_file() {} bytes.".format(len(data)))
             fp_dest.write(data)
             if callback:
                 callback(data)
 
-        self.ftp.retrbinary(
-            "RETR {}".format(name), _write_to_file, FTPTarget.DEFAULT_BLOCKSIZE
-        )
+        self.ftp.retrbinary(f"RETR {name}", _write_to_file, FTPTarget.DEFAULT_BLOCKSIZE)
 
     def remove_file(self, name):
         """Remove cur_dir/name."""
         assert is_native(name)
         self.check_write(name)
         # self.cur_dir_meta.remove(name)
         self.ftp.delete(name)
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/metadata.py` & `pyftpsync-4.1.0/ftpsync/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 
 import json
 import time
 
 from ftpsync import __version__
@@ -54,15 +53,15 @@
         self.modified_list = False
         #: bool: True if a least one peer data entry was changed since last read/write
         self.modified_sync = False
         #: bool: True if a meta data file was read (valid or not)
         self.was_read = False
 
     def __str__(self):
-        return "DirMetadata<{}>".format(self.get_full_path())
+        return f"DirMetadata<{self.get_full_path()}>"
 
     def get_full_path(self):
         return "/".join((self.path, self.filename))
 
     def set_mtime(self, filename, mtime, size):
         """Store real file mtime in meta data.
 
@@ -142,15 +141,15 @@
             self.list = self.dir["mtimes"]
             self.peer_sync = self.dir["peer_sync"]
             is_valid_file = True
             # write"DirMetadata: read(%s)" % (self.filename, ), self.dir)
         # except IncompatibleMetadataVersionError:
         #     raise  # We want version errors to terminate the app
         except Exception as e:
-            write_error("Could not read meta info {}: {!r}".format(self, e))
+            write_error(f"Could not read meta info {self}: {e!r}")
 
         # If the version is incompatible, we stop, unless:
         # if --migrate is set, we simply ignore this file (and probably replace it
         # with a current version)
         if is_valid_file and self.dir.get("_file_version", 0) != self.VERSION:
             if not self.target or not self.target.get_option("migrate"):
                 raise IncompatibleMetadataVersionError(
@@ -180,15 +179,15 @@
         #     return
         assert self.path == self.target.cur_dir
         if self.target.dry_run:
             # write("DirMetadata.flush(%s): dry-run; nothing to do" % self.target)
             pass
 
         elif self.was_read and len(self.list) == 0 and len(self.peer_sync) == 0:
-            write("Remove empty meta data file: {}".format(self.target))
+            write(f"Remove empty meta data file: {self.target}")
             self.target.remove_file(self.filename)
 
         elif not self.modified_list and not self.modified_sync:
             # write("DirMetadata.flush(%s): unmodified; nothing to do" % self.target)
             pass
 
         else:
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/pyftpsync.py` & `pyftpsync-4.1.0/ftpsync/pyftpsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
 """
 Simple folder synchronization using FTP.
 
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 
 Usage examples:
   > pyftpsync.py --help
   > pyftpsync.py upload . ftps://example.com/myfolder
 """
+
 import argparse
 import platform
 import sys
 from pprint import pprint
 
 from ftpsync import __version__
 from ftpsync.cli_common import (
@@ -282,15 +282,15 @@
     if args.command == "upload":
         s = UploadSynchronizer(args.local_target, args.remote_target, opts)
     elif args.command == "download":
         s = DownloadSynchronizer(args.local_target, args.remote_target, opts)
     elif args.command == "sync":
         s = BiDirSynchronizer(args.local_target, args.remote_target, opts)
     else:
-        parser.error("unknown command '{}'".format(args.command))
+        parser.error(f"unknown command '{args.command}'")
 
     # Allow prompting
     s.is_script = True
 
     try:
         s.run()
     except CliSilentRuntimeError as e:
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/resources.py` & `pyftpsync-4.1.0/ftpsync/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
+
 import os
 from datetime import datetime
 from posixpath import join as join_url
 from posixpath import normpath as normpath_url
 from posixpath import relpath as relpath_url
 
 from ftpsync.util import DEBUG_FLAGS, eps_compare, write
@@ -95,15 +95,15 @@
         #: str:
         self.re_class_reason = None
         # #: bool:
         # self.was_skipped = None
 
     def __str__(self):
         s = "<EntryPair({})>: ({}, {}) => {}".format(
-            "[{}]".format(self.rel_path) if self.is_dir else self.rel_path,
+            f"[{self.rel_path}]" if self.is_dir else self.rel_path,
             self.local_classification,
             self.remote_classification,
             self.operation,
         )
         return s
 
     @property
@@ -162,20 +162,18 @@
         else:
             self.remote_classification = "missing"
 
         c_pair = (self.local_classification, self.remote_classification)
 
         self.operation = operation_map.get(c_pair)
         if not self.operation:
-            raise RuntimeError(
-                "Undefined operation for pair classification {}".format(c_pair)
-            )
+            raise RuntimeError(f"Undefined operation for pair classification {c_pair}")
         if "classify" in DEBUG_FLAGS:
             write(
-                "Classified pair {}, meta={}".format(self, peer_entry_meta),
+                f"Classified pair {self}, meta={peer_entry_meta}",
                 debug=True,
             )
         # if not entry.meta:
         # assert self.classification in PAIR_CLASSIFICATIONS
         assert self.operation in PAIR_OPERATIONS
         return self.operation
 
@@ -229,25 +227,25 @@
         #: bool: May be set to true by synchronizer
         self.was_deleted = None
 
     def __str__(self):
         dt_modified = datetime.fromtimestamp(self.mtime)
         path = os.path.join(self.rel_path, self.name)
         if self.is_dir():
-            res = "{}([{}])".format(self.__class__.__name__, path)
+            res = f"{self.__class__.__name__}([{path}])"
         else:
             res = "{}('{}', size:{}, modified:{})".format(
                 self.__class__.__name__,
                 path,
-                "{:,}".format(self.size) if self.size is not None else self.size,
+                f"{self.size:,}" if self.size is not None else self.size,
                 dt_modified,
             )
             # + " ## %s, %s" % (self.mtime, time.asctime(time.gmtime(self.mtime)))
         if self.classification:
-            res += " => {}".format(self.classification)
+            res += f" => {self.classification}"
         return res
 
     def as_string(self, other_resource=None):
         # dt = datetime.fromtimestamp(self.get_adjusted_mtime())
         dt = datetime.fromtimestamp(self.mtime)
         res = "{}, {:>8,} bytes".format(dt.strftime("%Y-%m-%d %H:%M:%S"), self.size)
         if other_resource:
@@ -286,15 +284,15 @@
         return None
 
     def set_sync_info(self, local_file):
         raise NotImplementedError
 
     def classify(self, peer_dir_meta):
         """Classify this entry as 'new', 'unmodified', or 'modified'."""
-        assert self.classification is None, "{}, {}".format(self, peer_dir_meta)
+        assert self.classification is None, f"{self}, {peer_dir_meta}"
         peer_entry_meta = None
         if peer_dir_meta:
             # Metadata is generally available, so we can detect 'new' or 'modified'
             peer_entry_meta = peer_dir_meta.get(self.name, False)
 
             if self.is_dir():
                 # Directories are considered 'unmodified' (would require deep
@@ -325,24 +323,23 @@
                 # traversal to check otherwise)
                 self.classification = "unmodified"
             else:
                 # That's all we know, but EntryPair.classify() may adjust this
                 self.classification = "existing"
 
         if "classify" in DEBUG_FLAGS:
-            write("Classified {}, meta={}".format(self, peer_entry_meta), debug=True)
+            write(f"Classified {self}, meta={peer_entry_meta}", debug=True)
         assert self.classification in ENTRY_CLASSIFICATIONS
         return self.classification
 
 
 # ===============================================================================
 # FileEntry
 # ===============================================================================
 class FileEntry(_Resource):
-
     # 2 seconds difference is considered equal.
     # mtime stamp resolution depends on filesystem: FAT32. 2 seconds, NTFS ms, OSX. 1 sec.
     EPS_TIME = 2.01
     #     EPS_TIME = 0.1
 
     def __init__(self, target, rel_path, name, size, mtime, unique):
         super().__init__(target, rel_path, name, size, mtime, unique)
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/run_command.py` & `pyftpsync-4.1.0/ftpsync/run_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 
 import os
 
 import yaml
 
@@ -174,15 +173,15 @@
         parser.error(
             f"Could not locate `pyftpsync.yaml` in {os.getcwd()} or {cur_level} parent folders."
         )
 
     # --- Parse and validate `pyftpsync.yaml` ---
 
     try:
-        with open(config_path, "rt", encoding="utf-8-sig") as f:
+        with open(config_path, encoding="utf-8-sig") as f:
             config = yaml.safe_load(f)
     except Exception as e:
         parser.error(f"Error parsing {config_path}: {e}")
 
     if "tasks" not in config:
         parser.error(f"Missing entry `tasks` in {config_path}")
 
@@ -275,15 +274,15 @@
                 override = True
                 if name == "no_dry_run" and task.get("dry_run"):
                     # Already logged above
                     task["dry_run"] = False
             elif name in {"here", "root"} and (cli_args.here or cli_args.root):
                 override = True
             elif name == "verbose" and cli_val != 3:
-                assert type(cli_val) is int
+                assert isinstance(cli_val, int), cli_val
                 override = True
 
             if override:
                 if cli_args.verbose >= 4:  # and name != "no_dry_run":
                     write(
                         f"Override yaml entry `tasks.{task_name}.{name}: {task_val}` "
                         f"with CLI arg `--{name}={cli_val!r}`"
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/scan_command.py` & `pyftpsync-4.1.0/ftpsync/scan_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 
 import time
 from datetime import timedelta
 
 from ftpsync.cli_common import (
@@ -40,20 +39,20 @@
     parser.add_argument("--list", action="store_true", help="print target files")
     parser.add_argument(
         "-r", "--recursive", action="store_true", help="visit sub folders"
     )
     parser.add_argument(
         "--remove-meta",
         action="store_true",
-        help="delete all {} files".format(DirMetadata.META_FILE_NAME),
+        help=f"delete all {DirMetadata.META_FILE_NAME} files",
     )
     parser.add_argument(
         "--remove-locks",
         action="store_true",
-        help="delete all {} files".format(DirMetadata.LOCK_FILE_NAME),
+        help=f"delete all {DirMetadata.LOCK_FILE_NAME} files",
     )
 
     parser.set_defaults(command=scan_handler)
 
     return parser
 
 
@@ -87,15 +86,15 @@
             if is_dir:
                 dir_count += 1
             else:
                 file_count += 1
 
             if args.list:
                 if is_dir:
-                    print(indent, "[{e.name}]".format(e=e))
+                    print(indent, f"[{e.name}]")
                 else:
                     delta = e.mtime_org - e.mtime
                     dt_modified = pretty_stamp(e.mtime)
                     if delta:
                         prefix = "+" if delta > 0 else ""
                         print(
                             indent,
@@ -118,23 +117,23 @@
                 args.remove_meta
                 and target.cur_dir_meta
                 and target.cur_dir_meta.was_read
             ):
                 fspec = target.cur_dir_meta.get_full_path()
                 if fspec not in processed_files:
                     processed_files.add(fspec)
-                    print("DELETE {}".format(fspec))
+                    print(f"DELETE {fspec}")
 
             if (
                 args.remove_locks
                 and not is_dir
                 and e.name == DirMetadata.LOCK_FILE_NAME
             ):
                 fspec = e.get_rel_path()
-                print("DELETE {}".format(fspec))
+                print(f"DELETE {fspec}")
     finally:
         target.close()
 
     print(
         "Scanning {:,} files in {:,} directories took {:02.2f} seconds.".format(
             file_count, dir_count, time.time() - start
         )
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/sftp_target.py` & `pyftpsync-4.1.0/ftpsync/sftp_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
+
 import json
 import logging
 import os
 import stat
 import time
 from posixpath import join as join_url
 from posixpath import normpath as normpath_url
@@ -115,15 +115,15 @@
     def __str__(self):
         return "<{} + {}>".format(
             self.get_base_name(), relpath_url(self.cur_dir or "/", self.root_dir)
         )
 
     def get_base_name(self):
         scheme = "sftp"
-        return "{}://{}{}".format(scheme, self.host, self.root_dir)
+        return f"{scheme}://{self.host}{self.root_dir}"
 
     def open(self):
         assert not self.ftp_socket_connected
 
         super().open()
 
         options = self.get_options_dict()
@@ -145,31 +145,29 @@
         if self.username is None or self.password is None:
             creds = get_credentials_for_url(
                 self.host, options, force_user=self.username
             )
             if creds:
                 self.username, self.password = creds
 
-        write("Connecting {}:*** to sftp://{}".format(self.username, self.host))
+        write(f"Connecting {self.username}:*** to sftp://{self.host}")
 
         assert self.sftp is None
         while True:
             try:
                 self.sftp = PatchedPysftpConnection(
                     self.host,
                     username=self.username,
                     password=self.password,
                     port=self.port,
                     cnopts=cnopts,
                 )
                 break
             except paramiko.ssh_exception.AuthenticationException as e:
-                write_error(
-                    "Could not login to {}@{}: {}".format(self.username, self.host, e)
-                )
+                write_error(f"Could not login to {self.username}@{self.host}: {e}")
                 if no_prompt or not self.username:
                     raise
                 creds = prompt_for_password(self.host, self.username)
                 self.username, self.password = creds
                 # Continue while-loop
             except paramiko.ssh_exception.SSHException as e:
                 raise CliSilentRuntimeError(
@@ -179,21 +177,21 @@
                 )
 
         if verbose >= 4:
             write(
                 "Login as '{}'.".format(self.username if self.username else "anonymous")
             )
         if self.sftp.logfile:
-            write("Logging to {}".format(self.sftp.logfile))
+            write(f"Logging to {self.sftp.logfile}")
         self.sftp.timeout = self.timeout
         self.ftp_socket_connected = True
 
         try:
             self.sftp.cwd(self.root_dir)
-        except IOError as e:
+        except OSError as e:
             # '550 No such directory' is not reliably detectable with SFTP?
 
             # Implement --create-folder option for remote targets:
             if self.is_unbound():
                 # E.g. 'tree' command
                 write_error(
                     f"Could not change directory to {self.root_dir} ({e}): missing permissions?"
@@ -244,15 +242,15 @@
         if self.lock_data:
             self._unlock(closing=True)
 
         if self.ftp_socket_connected:
             try:
                 self.sftp.close()
             except (ConnectionError, EOFError) as e:
-                write_error("sftp.close() failed: {}".format(e))
+                write_error(f"sftp.close() failed: {e}")
             self.ftp_socket_connected = False
 
         super().close()
 
     def _lock(self, break_existing=False):
         """Write a special file to the target root folder."""
         # write("_lock")
@@ -260,15 +258,15 @@
 
         try:
             assert self.cur_dir == self.root_dir
             self.write_text(DirMetadata.LOCK_FILE_NAME, json.dumps(data))
             self.lock_data = data
             self.lock_write_time = time.time()
         except Exception as e:
-            write_error("Could not write lock file: {}".format(e))
+            write_error(f"Could not write lock file: {e}")
             # Set to False, so we don't try to remove later
             self.lock_data = False
 
     def _unlock(self, closing=False):
         """Remove lock file to the target root folder."""
         # write("_unlock", closing)
         try:
@@ -294,36 +292,36 @@
             else:
                 # direct delete, without updating metadata or checking for target access:
                 self.sftp.remove(DirMetadata.LOCK_FILE_NAME)
                 # self.remove_file(DirMetadata.LOCK_FILE_NAME)
 
             self.lock_data = None
         except Exception as e:
-            write_error("Could not remove lock file: {}".format(e))
+            write_error(f"Could not remove lock file: {e}")
             raise
 
     def _probe_lock_file(self, reported_mtime):
         """Called by get_dir"""
         delta = reported_mtime - self.lock_data["lock_time"]
         # delta2 = reported_mtime - self.lock_write_time
         self.server_time_ofs = delta
         if self.get_option("verbose", 3) >= 4:
-            write("Server time offset: {:.2f} seconds.".format(delta))
+            write(f"Server time offset: {delta:.2f} seconds.")
             # write("Server time offset2: {:.2f} seconds.".format(delta2))
 
     def get_id(self):
         return self.host + self.root_dir
 
     def cwd(self, dir_name):
         assert is_native(dir_name)
         path = normpath_url(join_url(self.cur_dir, dir_name))
         if not path.startswith(self.root_dir):
             # paranoic check to prevent that our sync tool goes berserk
             raise RuntimeError(
-                "Tried to navigate outside root {!r}: {!r}".format(self.root_dir, path)
+                f"Tried to navigate outside root {self.root_dir!r}: {path!r}"
             )
         self.sftp.cwd(dir_name)
         self.cur_dir = path
         self.cur_dir_meta = None
         return self.cur_dir
 
     def pwd(self):
@@ -361,15 +359,15 @@
         if len(names) > 0:
             self.sftp.cwd(dir_name)
             try:
                 for name in names:
                     try:
                         # try to delete this as a file
                         self.sftp.remove(name)
-                    except IOError:  # ftplib.all_errors as _e:
+                    except OSError:  # ftplib.all_errors as _e:
                         # write(f"    sftp.remove({name}) failed (not empty?), trying recursive...", debug=True)
                         # assume <name> is a folder
                         self.rmdir(name)
             finally:
                 if dir_name != ".":
                     self.sftp.cwd("..")
         #        write("sftp.rmd(%s)..." % (dir_name, ))
@@ -378,24 +376,25 @@
         return
 
     def rmdir(self, dir_name):
         # self.check_write(dir_name)
         # return self.sftp.rmdir(dir_name)
         return self._rmdir_impl(dir_name)
 
-    _paramiko_py3compat_u = paramiko.py3compat.u
+    try:
+        _paramiko_py3compat_u = paramiko.util.u
+    except AttributeError:
+        _paramiko_py3compat_u = paramiko.py3compat.u
 
     @staticmethod
     def _paramiko_py3compat_u_wrapper(s, encoding="utf8"):
         try:
             return SFTPTarget._paramiko_py3compat_u(s, encoding)
         except UnicodeDecodeError:
-            write_error(
-                "Failed to decode {} using {}. Trying cp1252...".format(s, encoding)
-            )
+            write_error(f"Failed to decode {s} using {encoding}. Trying cp1252...")
             s = s.decode("cp1252")
         return s
 
     def get_dir(self):
         # Fallback to cp1252 if utf8 fails
         with patch("paramiko.message.u", SFTPTarget._paramiko_py3compat_u_wrapper):
             res = self._get_dir_impl()
@@ -439,17 +438,15 @@
 
         if has_meta:
             try:
                 self.cur_dir_meta.read()
             except IncompatibleMetadataVersionError:
                 raise  # this should end the script (user should pass --migrate)
             except Exception as e:
-                write_error(
-                    "Could not read meta info {}: {}".format(self.cur_dir_meta, e)
-                )
+                write_error(f"Could not read meta info {self.cur_dir_meta}: {e}")
 
             meta_files = self.cur_dir_meta.list
 
             # Adjust file mtime from meta-data if present
             missing = []
             for n in meta_files:
                 meta = meta_files[n]
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/synchronizers.py` & `pyftpsync-4.1.0/ftpsync/synchronizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
+
 import fnmatch
 import sys
 import time
 
 from ftpsync.ftp_target import FTPTarget
 from ftpsync.metadata import DirMetadata
 from ftpsync.resources import DirectoryEntry, EntryPair, FileEntry, operation_map
@@ -37,26 +37,26 @@
 _ts = pretty_stamp
 
 
 def process_options(opts):
     """Check and prepare options dict."""
     # Convert match and exclude args into pattern lists
     match = opts.get("match")
-    if match and type(match) is str:
+    if match and isinstance(match, str):
         opts["match"] = [pat.strip() for pat in match.split(",")]
     elif match:
-        assert type(match) is list
+        assert isinstance(match, list), match
     else:
         opts["match"] = []
 
     exclude = opts.get("exclude")
-    if exclude and type(exclude) is str:
+    if exclude and isinstance(exclude, str):
         opts["exclude"] = [pat.strip() for pat in exclude.split(",")]
     elif exclude:
-        assert type(exclude) is list
+        assert isinstance(exclude, list), exclude
     else:
         # opts["exclude"] = DEFAULT_OMIT
         opts["exclude"] = []
     # print(match, exclude, opts)
 
 
 def match_path(entry, opts):
@@ -67,22 +67,22 @@
     # We also might allow glob syntax and match against the whole relative path instead
     # path = entry.get_rel_path()
     path = entry.name
     ok = True
     match = opts.get("match")
     exclude = opts.get("exclude")
     if entry.is_file() and match:
-        assert type(match) is list
+        assert isinstance(match, list), match
         ok = False
         for pat in match:
             if fnmatch.fnmatch(path, pat):
                 ok = True
                 break
     if ok and exclude:
-        assert type(exclude) is list
+        assert isinstance(exclude, list), exclude
         for pat in exclude:
             if fnmatch.fnmatch(path, pat):
                 ok = False
                 break
     # write("match", ok, entry)
     return ok
 
@@ -211,26 +211,26 @@
 
         stats = self._stats
         stats["elap_secs"] = time.time() - start
         stats["elap_str"] = "{:0.2f} sec".format(stats["elap_secs"])
 
         def _add(rate, size, time):
             if stats.get(time) and stats.get(size):
-                stats[rate] = "{:0.2f} kB/sec".format(0.001 * stats[size] / stats[time])
+                stats[rate] = f"{0.001 * stats[size] / stats[time]:0.2f} kB/sec"
 
         _add("upload_rate_str", "upload_bytes_written", "upload_write_time")
         _add("download_rate_str", "download_bytes_written", "download_write_time")
         return res
 
     def _compare_file(self, local, remote):
         """Byte compare two files (early out on first difference)."""
         assert isinstance(local, FileEntry) and isinstance(remote, FileEntry)
 
         if not local or not remote:
-            write("    Files cannot be compared ({} != {}).".format(local, remote))
+            write(f"    Files cannot be compared ({local} != {remote}).")
             return False
         elif local.size != remote.size:
             write(
                 "    Files are different (size {:,d} != {:,d}).".format(
                     local.size, remote.size
                 )
             )
@@ -238,15 +238,15 @@
 
         with local.target.open_readable(
             local.name
         ) as fp_src, remote.target.open_readable(remote.name) as fp_dest:
             res, ofs = byte_compare(fp_src, fp_dest)
 
         if not res:
-            write("    Files are different at offset {:,d}.".format(ofs))
+            write(f"    Files are different at offset {ofs:,d}.")
         else:
             write("    Files are equal.")
         return res
 
     def _copy_file(self, src, dest, file_entry):
         # TODO: safe replace:
         # 1. remove temp file
@@ -260,19 +260,17 @@
         is_upload = dest is self.remote
         if is_upload:
             self._inc_stat("upload_files_written")
         else:
             self._inc_stat("download_files_written")
         self._tick()
         if self.dry_run:
-            return self._dry_run_action(
-                "copy file ({}, {} --> {})".format(file_entry, src, dest)
-            )
+            return self._dry_run_action(f"copy file ({file_entry}, {src} --> {dest})")
         elif dest.readonly:
-            raise RuntimeError("target is read-only: {}".format(dest))
+            raise RuntimeError(f"target is read-only: {dest}")
 
         start = time.time()
 
         def _show_error(msg, exc):
             write_error(
                 f"{ansi_code('Fore.LIGHTRED_EX')}{msg}: {exc} {ansi_code('Style.RESET_ALL')}"
             )
@@ -334,18 +332,18 @@
         # write("_copy_recursive(%s, %s --> %s)" % (dir_entry, src, dest))
         assert isinstance(dir_entry, DirectoryEntry)
         self._inc_stat("entries_touched")
         self._inc_stat("dirs_created")
         self._tick()
         if self.dry_run:
             return self._dry_run_action(
-                "copy directory ({}, {} --> {})".format(dir_entry, src, dest)
+                f"copy directory ({dir_entry}, {src} --> {dest})"
             )
         elif dest.readonly:
-            raise RuntimeError("target is read-only: {}".format(dest))
+            raise RuntimeError(f"target is read-only: {dest}")
 
         dest.set_sync_info(dir_entry.name, None, None)
 
         src.push_meta()
         dest.push_meta()
 
         src.cwd(dir_entry.name)
@@ -373,29 +371,29 @@
     def _remove_file(self, file_entry):
         # TODO: honor backup
         # write("_remove_file(%s)" % (file_entry, ))
         assert isinstance(file_entry, FileEntry)
         self._inc_stat("entries_touched")
         self._inc_stat("files_deleted")
         if self.dry_run:
-            return self._dry_run_action("delete file ({})".format(file_entry))
+            return self._dry_run_action(f"delete file ({file_entry})")
         elif file_entry.target.readonly:
-            raise RuntimeError("target is read-only: {}".format(file_entry.target))
+            raise RuntimeError(f"target is read-only: {file_entry.target}")
         file_entry.target.remove_file(file_entry.name)
         file_entry.target.remove_sync_info(file_entry.name)
 
     def _remove_dir(self, dir_entry):
         # TODO: honor backup
         assert isinstance(dir_entry, DirectoryEntry)
         self._inc_stat("entries_touched")
         self._inc_stat("dirs_deleted")
         if self.dry_run:
-            return self._dry_run_action("delete directory ({})".format(dir_entry))
+            return self._dry_run_action(f"delete directory ({dir_entry})")
         elif dir_entry.target.readonly:
-            raise RuntimeError("target is read-only: {}".format(dir_entry.target))
+            raise RuntimeError(f"target is read-only: {dir_entry.target}")
         dir_entry.target.rmdir(dir_entry.name)
         dir_entry.target.remove_sync_info(dir_entry.name)
 
     def _log_action(self, action, status, symbol, entry, min_level=3):
         if self.verbose < min_level:
             return
 
@@ -438,24 +436,24 @@
         else:
             final += " " * 10
         prefix = ""
         if self.dry_run:
             prefix = DRY_RUN_PREFIX
 
         if action and status:
-            tag = ("{} {}".format(action, status)).upper()
+            tag = (f"{action} {status}").upper()
         else:
             assert status
-            tag = ("{}".format(status)).upper()
+            tag = (f"{status}").upper()
 
         name = entry.get_rel_path()
         if entry.is_dir():
-            name = "[{}]".format(name)
+            name = f"[{name}]"
 
-        write("{}{}{:<16} {:^3} {}{}".format(prefix, color, tag, symbol, name, final))
+        write(f"{prefix}{color}{tag:<16} {symbol:^3} {name}{final}")
 
     def _tick(self):
         """Write progress info and move cursor to beginning of line."""
         if (self.verbose >= 3 and not IS_REDIRECTED) or self.options.get("progress"):
             stats = self.get_stats()
             prefix = DRY_RUN_PREFIX if self.dry_run else ""
             sys.stdout.write(
@@ -595,15 +593,14 @@
         peer_dir_meta = self.local.cur_dir_meta.peer_sync.get(self.remote.get_id())
 
         for pair in entry_pair_list:
             pair.classify(peer_dir_meta)
 
         # 4. Perform (or schedule) resulting file operations
         for pair in entry_pair_list:
-
             # print(pair)
 
             # Let synchronizer modify the default operation (e.g. apply `--force` option)
             hook_result = self.re_classify_pair(pair)
 
             # Let synchronizer implement special handling of unmatched entries
             # (e.g. `--delete_unmatched`)
@@ -617,15 +614,15 @@
                     try:
                         handler(pair)
                     except Exception as e:
                         if self.on_error(e, pair) is not True:
                             raise
                 else:
                     # write("NO HANDLER")
-                    raise NotImplementedError("No handler for {}".format(pair))
+                    raise NotImplementedError(f"No handler for {pair}")
 
             if pair.is_conflict():
                 self._inc_stat("conflict_files")
 
         # 5. Let the target provider write its meta data for the files in the
         #    current directory.
         self.local.flush_meta()
@@ -790,15 +787,15 @@
             resolve = self.resolve_all
         else:
             # A resolution strategy was configured
             resolve = self.options.get("resolve", "skip")
 
         if resolve in ("new", "old") and pair.is_same_time():
             # We cannot apply this resolution: force an alternative
-            print("Cannot resolve using '{}' strategy: {}".format(resolve, pair))
+            print(f"Cannot resolve using '{resolve}' strategy: {pair}")
             resolve = "ask" if self.is_script else "skip"
 
         if resolve == "ask" or self.verbose >= 5:
             self._print_pair_diff(pair)
 
         if resolve in ("local", "remote", "old", "new", "skip"):
             # self.resolve_all = resolve
@@ -951,19 +948,17 @@
 
         pair.local_classification = c_pair[0]
         pair.remote_classification = c_pair[1]
 
         pair.operation = operation_map.get(c_pair)
         # print("on_need_compare {} => {}".format(org_pair, pair))
         if not pair.operation:
-            raise RuntimeError(
-                "Undefined operation for pair classification {}".format(c_pair)
-            )
+            raise RuntimeError(f"Undefined operation for pair classification {c_pair}")
         elif pair.operation == org_operation:
-            raise RuntimeError("Could not re-classify  {}".format(org_pair))
+            raise RuntimeError(f"Could not re-classify  {org_pair}")
 
         handler = getattr(self, "on_" + pair.operation, None)
         res = handler(pair)
         # self._log_action("", "different", "?", pair.local, min_level=2)
         return res
 
     def on_conflict(self, pair):
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/targets.py` & `pyftpsync-4.1.0/ftpsync/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 
 import codecs
 import contextlib
 import io
 import os
 import shutil
 import sys
 import threading
 from posixpath import join as join_url
 from posixpath import normpath as normpath_url
-from urllib.parse import urlparse
+from urllib.parse import unquote, urlparse
 
 from ftpsync.metadata import DirMetadata
 from ftpsync.resources import DirectoryEntry, FileEntry
 from ftpsync.util import is_native, to_bytes, to_native, to_unicode, write
 
 
 # ===============================================================================
@@ -33,38 +32,39 @@
         url (str):
         extra_opts (dict, optional): Passed to Target constructor. Default: None.
     Returns:
         :class:`_Target`
     """
     # debug = extra_opts.get("debug", 1)
     parts = urlparse(url, allow_fragments=False)
+    password = unquote(parts.password) if parts.password else None
     # scheme is case-insensitive according to https://tools.ietf.org/html/rfc3986
     scheme = parts.scheme.lower()
     if scheme in ("ftp", "ftps"):
         from ftpsync.ftp_target import FTPTarget
 
         target = FTPTarget(
             parts.path,
             parts.hostname,
             parts.port,
             username=parts.username,
-            password=parts.password,
+            password=password,
             tls=(scheme == "ftps"),
             timeout=None,
             extra_opts=extra_opts,
         )
     elif scheme == "sftp":
         from ftpsync.sftp_target import SFTPTarget
 
         target = SFTPTarget(
             parts.path,
             parts.hostname,
             parts.port,
             username=parts.username,
-            password=parts.password,
+            password=password,
             timeout=None,
             extra_opts=extra_opts,
         )
     else:
         target = FsTarget(url, extra_opts)
 
     return target
@@ -138,15 +138,15 @@
     #     self.open()
     #     return self
 
     # def __exit__(self, exc_type, exc_value, traceback):
     #     self.close()
 
     def get_base_name(self):
-        return "{}".format(self.root_dir)
+        return f"{self.root_dir}"
 
     def is_local(self):
         if not self.synchronizer:
             raise RuntimeError(
                 "Unbound target: Consider calling target.is_remote(or_unbound=True)"
             )
         return self.synchronizer.local is self
@@ -169,37 +169,37 @@
         """Return option from synchronizer (possibly overridden by target extra_opts)."""
         if self.synchronizer:
             return self.extra_opts.get(key, self.synchronizer.options.get(key, default))
         return self.extra_opts.get(key, default)
 
     def open(self):
         if self.connected:
-            raise RuntimeError("Target already open: {}.  ".format(self))
+            raise RuntimeError(f"Target already open: {self}.  ")
         # Not thread safe (issue #20)
         if not self._rlock.acquire(False):
             raise RuntimeError("Could not acquire _Target lock on open")
         self.connected = True
 
     def close(self):
         if not self.connected:
             return
         if self.get_option("verbose", 3) >= 5:
-            write("Closing target {}.".format(self))
+            write(f"Closing target {self}.")
         self.connected = False
         self.readonly = False  # issue #20
         self._rlock.release()
 
     def check_write(self, name):
         """Raise exception if writing cur_dir/name is not allowed."""
         assert is_native(name)
         if self.readonly and name not in (
             DirMetadata.META_FILE_NAME,
             DirMetadata.LOCK_FILE_NAME,
         ):
-            raise RuntimeError("Target is read-only: {} + {} / ".format(self, name))
+            raise RuntimeError(f"Target is read-only: {self} + {name} / ")
 
     def get_id(self):
         return self.root_dir
 
     def get_sync_info(self, name, key=None):
         """Get mtime/size when this target's current dir was last synchronized with remote."""
         peer_target = self.peer
@@ -271,16 +271,15 @@
                 continue
 
             yield entry
 
             if recursive:
                 if isinstance(entry, DirectoryEntry):
                     self.cwd(entry.name)
-                    for e in self.walk(pred):
-                        yield e
+                    yield from self.walk(pred)
                     self.cwd("..")
         return
 
     def walk_tree(self, sort=True, files=False, pred=None, _prefixes=None):
         """Iterate over target hierarchy, depth-first, adding a connector prefix.
 
         This iterator walks the tree nodes, but slightly delays the output, in
@@ -414,28 +413,27 @@
 
 # ===============================================================================
 # FsTarget
 # ===============================================================================
 
 
 class FsTarget(_Target):
-
     DEFAULT_BLOCKSIZE = 16 * 1024  # shutil.copyobj() uses 16k blocks by default
 
     def __init__(self, root_dir, extra_opts=None):
         def_enc = sys.getfilesystemencoding()
         if not def_enc:
             def_enc = "utf-8"
         self.encoding = _get_encoding_opt(None, extra_opts, def_enc)
         # root_dir = self.to_unicode(root_dir)
         root_dir = os.path.expanduser(root_dir)
         root_dir = os.path.abspath(root_dir)
         super().__init__(root_dir, extra_opts)
         if not os.path.isdir(root_dir):
-            raise ValueError("{} is not a directory.".format(root_dir))
+            raise ValueError(f"{root_dir} is not a directory.")
         self.support_set_time = True
 
     def __str__(self):
         return "<FS:{} + {}>".format(
             self.root_dir, os.path.relpath(self.cur_dir, self.root_dir)
         )
 
@@ -446,15 +444,15 @@
     def close(self):
         super().close()
 
     def cwd(self, dir_name):
         path = normpath_url(join_url(self.cur_dir, dir_name))
         if not path.startswith(self.root_dir):
             raise RuntimeError(
-                "Tried to navigate outside root {!r}: {!r}".format(self.root_dir, path)
+                f"Tried to navigate outside root {self.root_dir!r}: {path!r}"
             )
         self.cur_dir_meta = None
         self.cur_dir = path
         return self.cur_dir
 
     def pwd(self):
         return self.cur_dir
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/tree_command.py` & `pyftpsync-4.1.0/ftpsync/tree_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 
 import time
 
 from ftpsync.cli_common import (
     common_parser,
@@ -61,25 +60,25 @@
         """Walker predicate that check match/exclude options."""
         if not match_path(entry, opts):
             return False
 
     try:
         target.open()
 
-        print("[{}]".format(target.root_dir))
+        print(f"[{target.root_dir}]")
         for path, entry in target.walk_tree(
             sort=args.sort, files=args.files, pred=_pred
         ):
             name = entry.name
             if entry.is_dir():
                 dir_count += 1
-                line = "{}[{}]".format(path, name)
+                line = f"{path}[{name}]"
             else:
                 file_count += 1
-                line = "{}{:<20} {}".format(path, name, entry.as_string())
+                line = f"{path}{name:<20} {entry.as_string()}"
             print(line)
     finally:
         target.close()
 
     print(
         "Scanning {:,} files in {:,} directories took {:02.2f} seconds.".format(
             file_count, dir_count, time.time() - start
```

### Comparing `pyftpsync-4.0.0a6/ftpsync/util.py` & `pyftpsync-4.1.0/ftpsync/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-(c) 2012-2022 Martin Wendt; see https://github.com/mar10/pyftpsync
+(c) 2012-2024 Martin Wendt; see https://github.com/mar10/pyftpsync
 Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
+
 import configparser
 import getpass
 import logging
 import netrc
 import os
 import sys
 from datetime import datetime
@@ -24,46 +24,31 @@
 
     def __init__(self, msg, *, min_verbosity, exit_code=1) -> None:
         self.min_verbosity = min_verbosity
         self.exit_code = exit_code
         super().__init__(msg)
 
 
-# def is_basestring(s):
-#     """Return True for any string type, i.e. for str/unicode on Py2 and bytes/str on Py3."""
-#     return isinstance(s, (str, bytes))
-
-
-# def is_bytes(s):
-#     """Return True for bytestrings, i.e. for str on Py2 and bytes on Py3."""
-#     return isinstance(s, bytes)
-
-
 def is_native(s):
     """Return True for native strings, i.e. for str on Py2 and Py3."""
     return isinstance(s, str)
 
 
-# def is_unicode(s):
-#     """Return True for unicode strings, i.e. for unicode on Py2 and str on Py3."""
-#     return isinstance(s, str)
-
-
 def to_bytes(s, encoding="utf-8"):
     """Convert a text string (unicode) to bytestring, i.e. str on Py2 and bytes on Py3."""
-    if type(s) is not bytes:
+    if not isinstance(s, bytes):
         s = bytes(s, encoding)
     return s
 
 
 def to_native(s, encoding="utf-8"):
     """Convert data to native str type, i.e. bytestring on Py2 and unicode on Py3."""
-    if type(s) is bytes:
+    if isinstance(s, bytes):
         s = str(s, encoding)
-    elif type(s) is not str:
+    elif not isinstance(s, str):
         s = str(s)
     return s
 
 
 to_unicode = to_native
 """Convert binary data to unicode (text strings) on Python 2 and 3."""
 
@@ -256,21 +241,19 @@
         KeyboardInterrupt if user hits Ctrl-C
     Returns:
         (username, password) or None
     """
     if user is None:
         default_user = default_user or getpass.getuser()
         while user is None:
-            user = input("Enter username for {} [{}]: ".format(url, default_user))
+            user = input(f"Enter username for {url} [{default_user}]: ")
             if user.strip() == "" and default_user:
                 user = default_user
     if user:
-        pw = getpass.getpass(
-            "Enter password for {}@{} (Ctrl+C to abort): ".format(user, url)
-        )
+        pw = getpass.getpass(f"Enter password for {user}@{url} (Ctrl+C to abort): ")
         if pw or pw == "":
             return (user, pw)
     return None
 
 
 def get_credentials_for_url(url, opts, force_user=None):
     """Lookup credentials for a given target in keyring and .netrc.
@@ -327,33 +310,33 @@
                         "No credentials found in keyring('pyftpsync', '{}').".format(
                             url
                         )
                     )
         # except keyring.errors.TransientKeyringError:
         except Exception as e:
             # e.g. user clicked 'no'
-            write_error("Could not get password from keyring {}".format(e))
+            write_error(f"Could not get password from keyring {e}")
 
     # 2. Try .netrc file
     if creds is None and allow_netrc and not force_prompt:
         try:
             authenticators = None
             authenticators = netrc.netrc().authenticators(url)
         except FileNotFoundError:
             if verbose >= 4:
                 write("Could not get password (no .netrc file).")
         except Exception as e:
-            write_error("Could not read .netrc: {}.".format(e))
+            write_error(f"Could not read .netrc: {e}.")
 
         if authenticators:
             creds = (authenticators[0], authenticators[2])
-            write("Using credentials from .netrc file: {}:***.".format(creds[0]))
+            write(f"Using credentials from .netrc file: {creds[0]}:***.")
         else:
             if verbose >= 4:
-                write("Could not find entry for '{}' in .netrc file.".format(url))
+                write(f"Could not find entry for '{url}' in .netrc file.")
 
     # 3. Prompt for password if we don't have credentials yet, or --prompt was set.
     if creds is None and allow_prompt and not force_prompt:
         creds = prompt_for_password(url, user=force_user)
     if force_prompt:
         # --prompt was set but we can provide a default for the user name
         assert not creds
@@ -373,25 +356,21 @@
                 )
             )
 
         try:
             # Note: we pass the url as `username` and username:password as `password`
             if password is None:
                 keyring.delete_password("pyftpsync", url)
-                write("Delete credentials from keyring ({})".format(url))
+                write(f"Delete credentials from keyring ({url})")
             else:
-                keyring.set_password(
-                    "pyftpsync", url, "{}:{}".format(username, password)
-                )
-                write(
-                    "Store credentials in keyring ({}, {}:***).".format(url, username)
-                )
+                keyring.set_password("pyftpsync", url, f"{username}:{password}")
+                write(f"Store credentials in keyring ({url}, {username}:***).")
         #        except keyring.errors.TransientKeyringError:
         except Exception as e:
-            write("Could not delete/set password {}.".format(e))
+            write(f"Could not delete/set password {e}.")
             pass  # e.g. user clicked 'no'
     else:
         write("Could not store credentials (missing keyring support).")
     return
 
 
 def str_to_bool(val):
@@ -459,15 +438,15 @@
 
 
 def make_native_dict_keys(d):
     """Convert all keys to native `str` type (recursively)."""
     res = {}
     for k, v in d.items():  #
         k = to_native(k)
-        if type(v) is dict:
+        if isinstance(v, dict):
             v = make_native_dict_keys(v)
         res[k] = v
     return res
 
 
 # def decode_utf8_safe(s, fallback="cp1252", raise_error=True):
 #     """Try to decode a binary string using UTF-8 but fall back to CP-1252.
```

### Comparing `pyftpsync-4.0.0a6/pyftpsync.egg-info/PKG-INFO` & `pyftpsync-4.1.0/pyftpsync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftpsync
-Version: 4.0.0a6
+Version: 4.1.0
 Summary: Synchronize directories using FTP(S), SFTP, or file system access
 Home-page: https://github.com/mar10/pyftpsync
 Author: Martin Wendt
 Author-email: pyftpsync@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: pyftpsync@wwwendt.de
 License: MIT
@@ -19,74 +19,83 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: colorama
+Requires-Dist: keyring
+Requires-Dist: pysftp
+Requires-Dist: PyYAML
 
 # ![logo](https://raw.githubusercontent.com/mar10/pyftpsync/master/docs/logo_48x48.png) pyftpsync
-[![Build Status](https://travis-ci.com/mar10/pyftpsync.svg?branch=master)](https://app.travis-ci.com/github/mar10/pyftpsync)
+
+[![Tests](https://github.com/mar10/pyftpsync/actions/workflows/python-app.yml/badge.svg)](https://github.com/mar10/pyftpsync/actions/workflows/python-app.yml)
 [![Latest Version](https://img.shields.io/pypi/v/pyftpsync.svg)](https://pypi.python.org/pypi/pyftpsync/)
 [![License](https://img.shields.io/pypi/l/pyftpsync.svg)](https://github.com/mar10/pyftpsync/blob/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/pyftpsync/badge/?version=latest)](https://pyftpsync.readthedocs.io/)
+[![codecov](https://codecov.io/github/mar10/pyftpsync/graph/badge.svg?token=0JM9CN8RYW)](https://codecov.io/github/mar10/pyftpsync)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: pyftpsync](https://img.shields.io/badge/StackOverflow-pyftpsync-blue.svg)](https://stackoverflow.com/questions/tagged/pyftpsync)
 
 > Synchronize directories using FTP(S), SFTP, or file system access.
 
 [ ![sample](teaser.png?raw=true) ](https://github.com/mar10/pyftpsync "Live demo")
 
-
 ## Summary
 
 Synchronize directories using FTP(S), SFTP, or file system access.
 
-  * This is a command line tool...
-  * ... and a library for use in your Python projects.
-  * Upload, download, and bi-directional synch mode.
-  * Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
-  * Architecture is open to add other target types.
+-   This is a command line tool...
+-   ... and a library for use in your Python projects.
+-   Upload, download, and bi-directional synch mode.
+-   Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
+-   Architecture is open to add other target types.
 
 **Note:** Version 4.0 drops support for Python 2.
 
-
 ## Quickstart
 
-[Python](https://www.python.org/download/Python) 3.7+ is required,
+[Python](https://www.python.org/download/Python) 3.8+ is required,
 [pip](http://www.pip-installer.org/) recommended:
 
 ```bash
 $ pip install pyftpsync --upgrade
 $ pyftpsync --help
 ```
 
-See [Command Line Interface](https://pyftpsync.readthedocs.io/en/latest/ug_cli.html) 
+**Note:** <br>
+MS Windows users that only need the command line interface may prefer the
+[MSI Installer](https://github.com/mar10/pyftpsync/releases/latest) or install
+using the Windows Package Manager:
+
+```ps1
+> winget install pyftpsync
+```
+
+See [Command Line Interface](https://pyftpsync.readthedocs.io/en/latest/ug_cli.html)
 for details.
 
 In addition to the direct invocation of `upload`, `download`, or `sync`
-commands, version 3.x allows to define a ``pyftpsync_yaml`` file
+commands, version 3.x allows to define a `pyftpsync_yaml` file
 in your project's root folder which then can be executed like so::
 
     $ pyftpsync run
 
-See [Run from pyftpsync.yaml](https://pyftpsync.readthedocs.io/en/latest/ug_run.html) 
+See [Run from pyftpsync.yaml](https://pyftpsync.readthedocs.io/en/latest/ug_run.html)
 for details.
 
-
-**Note:** Windows users may prefer the 
-[MSI Installer](https://github.com/mar10/pyftpsync/releases/latest).
-
-
 ## Documentation
 
 [Read the Docs](https://pyftpsync.readthedocs.io/) for details.
```

### Comparing `pyftpsync-4.0.0a6/pyftpsync.egg-info/SOURCES.txt` & `pyftpsync-4.1.0/pyftpsync.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 readme_pypi.rst
 requirements-dev.txt
 requirements.txt
@@ -35,8 +36,21 @@
 ftpsync/util.py
 pyftpsync.egg-info/PKG-INFO
 pyftpsync.egg-info/SOURCES.txt
 pyftpsync.egg-info/dependency_links.txt
 pyftpsync.egg-info/entry_points.txt
 pyftpsync.egg-info/not-zip-safe
 pyftpsync.egg-info/requires.txt
-pyftpsync.egg-info/top_level.txt
+pyftpsync.egg-info/top_level.txt
+tests/test_1x.py
+tests/test_1x_ftp.py
+tests/test_basic.py
+tests/test_bench.py
+tests/test_cli.py
+tests/test_develop.py
+tests/test_regressions.py
+tests/test_scan.py
+tests/test_sftp.py
+tests/test_sync_bidir.py
+tests/test_sync_download.py
+tests/test_sync_upload.py
+tests/test_tree.py
```

### Comparing `pyftpsync-4.0.0a6/readme_pypi.rst` & `pyftpsync-4.1.0/readme_pypi.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-Copyright (c) 2012-2022 Martin Wendt
+Copyright (c) 2012-2024 Martin Wendt
 
 Summary
 -------
 Synchronize directories using FTP(S), SFTP, or file system access.
 
   * This is a command line tool...
   * ... and a library for use in your Python projects.
   * Upload, download, and bi-directional synch mode.
   * Allows FTP-to-FTP and Filesystem-to-Filesystem synchronization as well.
   * Architecture is open to add other target types.
 
 .. note::
     Version 4.0 drops support for Python 2.
 
-Requires `Python <https://www.python.org/download/>`_ 3.7+.
+Requires `Python <https://www.python.org/download/>`_ 3.8+.
 
-A Windows `MSI installer is also available on GitHub <https://github.com/mar10/pyftpsync/releases>`_.
+.. note::
+   MS Windows users that only need the command line interface may prefer the
+   `MSI installer <https://github.com/mar10/pyftpsync/releases>`_ or install
+   using the Windows Package Manager::
+
+     > winget install pyftpsync
 
 See also https://github.com/mar10/pyftpsync for details
 and `Read the Docs <https://pyftpsync.readthedocs.io/>`_.
 
 Change Log
 ----------
 See `CHANGELOG.md <https://github.com/mar10/pyftpsync/blob/master/CHANGELOG.md>`_.
```

### Comparing `pyftpsync-4.0.0a6/setup.cfg` & `pyftpsync-4.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -67,82 +67,67 @@
 00000420: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000430: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 00000440: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
 00000450: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 00000460: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
 00000470: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
 00000480: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000490: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+00000490: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
 000004a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 000004b0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000004c0: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+000004c0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
 000004d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000004e0: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
-000004f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000500: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000510: 3130 0d0a 0954 6f70 6963 203a 3a20 496e  10...Topic :: In
-00000520: 7465 726e 6574 203a 3a20 4669 6c65 2054  ternet :: File T
-00000530: 7261 6e73 6665 7220 5072 6f74 6f63 6f6c  ransfer Protocol
-00000540: 2028 4654 5029 0d0a 0954 6f70 6963 203a   (FTP)...Topic :
-00000550: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000560: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-00000570: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
-00000580: 6475 6c65 730d 0a09 546f 7069 6320 3a3a  dules...Topic ::
-00000590: 2055 7469 6c69 7469 6573 0d0a 0d0a 5b6f   Utilities....[o
-000005a0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-000005b0: 5f64 6972 203d 200d 0a09 3d20 2e0d 0a70  _dir = ...= ...p
-000005c0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000005d0: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
-000005e0: 650d 0a69 6e73 7461 6c6c 5f72 6571 7569  e..install_requi
-000005f0: 7265 7320 3d20 0d0a 0963 6f6c 6f72 616d  res = ...coloram
-00000600: 610d 0a09 6b65 7972 696e 670d 0a09 7079  a...keyring...py
-00000610: 7366 7470 0d0a 0950 7959 414d 4c0d 0a0d  sftp...PyYAML...
-00000620: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000630: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000640: 3d20 2e0d 0a69 6e63 6c75 6465 5f70 6163  = ...include_pac
-00000650: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000660: 0d0a 6578 636c 7564 6520 3d20 0d0a 0974  ..exclude = ...t
-00000670: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
-00000680: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000690: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
-000006a0: 3d20 0d0a 0970 7966 7470 7379 6e63 203d  = ...pyftpsync =
-000006b0: 2066 7470 7379 6e63 2e70 7966 7470 7379   ftpsync.pyftpsy
-000006c0: 6e63 3a72 756e 0d0a 0d0a 5b63 6f76 6572  nc:run....[cover
-000006d0: 6167 653a 7275 6e5d 0d0a 6272 616e 6368  age:run]..branch
-000006e0: 203d 2054 7275 650d 0a6f 6d69 7420 3d20   = True..omit = 
-000006f0: 0d0a 0974 6573 7473 2f2a 0d0a 0d0a 5b63  ...tests/*....[c
-00000700: 6f76 6572 6167 653a 7265 706f 7274 5d0d  overage:report].
-00000710: 0a70 7265 6369 7369 6f6e 203d 2032 0d0a  .precision = 2..
-00000720: 736f 7274 203d 204e 616d 650d 0a65 7863  sort = Name..exc
-00000730: 6c75 6465 5f6c 696e 6573 203d 200d 0a09  lude_lines = ...
-00000740: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00000750: 0d0a 0969 6620 5f5f 6e61 6d65 5f5f 203d  ...if __name__ =
-00000760: 3d20 2e5f 5f6d 6169 6e5f 5f2e 3a0d 0a0d  = .__main__.:...
-00000770: 0a5b 636f 7665 7261 6765 3a68 746d 6c5d  .[coverage:html]
-00000780: 0d0a 6469 7265 6374 6f72 7920 3d20 6275  ..directory = bu
-00000790: 696c 642f 636f 7665 7261 6765 0d0a 0d0a  ild/coverage....
-000007a0: 5b74 6f6f 6c3a 7079 7465 7374 5d0d 0a6a  [tool:pytest]..j
-000007b0: 756e 6974 5f66 616d 696c 7920 3d20 6c65  unit_family = le
-000007c0: 6761 6379 0d0a 0d0a 5b66 6c61 6b65 385d  gacy....[flake8]
-000007d0: 0d0a 656e 6162 6c65 2d65 7874 656e 7369  ..enable-extensi
-000007e0: 6f6e 7320 3d20 470d 0a65 7863 6c75 6465  ons = G..exclude
-000007f0: 203d 200d 0a09 5f5f 7079 6361 6368 655f   = ...__pycache_
-00000800: 5f2c 0d0a 092e 6361 6368 652c 0d0a 092e  _,....cache,....
-00000810: 6567 6773 2c0d 0a09 2e67 6974 2c0d 0a09  eggs,....git,...
-00000820: 2e74 6f78 2c0d 0a09 2e76 7363 6f64 652c  .tox,....vscode,
-00000830: 0d0a 0962 7569 6c64 2c0d 0a09 6469 7374  ...build,...dist
-00000840: 2c0d 0a09 646f 6373 0d0a 6d61 782d 6c69  ,...docs..max-li
-00000850: 6e65 2d6c 656e 6774 6820 3d20 3939 0d0a  ne-length = 99..
-00000860: 6967 6e6f 7265 203d 2045 3230 332c 2045  ignore = E203, E
-00000870: 3530 312c 2057 3530 332c 2050 3130 312c  501, W503, P101,
-00000880: 2041 3030 332c 204e 3830 360d 0a64 6f63   A003, N806..doc
-00000890: 7374 7269 6e67 2d63 6f6e 7665 6e74 696f  string-conventio
-000008a0: 6e20 3d20 616c 6c20 2023 2067 6f6f 676c  n = all  # googl
-000008b0: 653f 0d0a 696e 6c69 6e65 2d71 756f 7465  e?..inline-quote
-000008c0: 7320 3d20 646f 7562 6c65 0d0a 6d75 6c74  s = double..mult
-000008d0: 696c 696e 652d 7175 6f74 6573 203d 2022  iline-quotes = "
-000008e0: 2222 0d0a 646f 6373 7472 696e 672d 7175  ""..docstring-qu
-000008f0: 6f74 6573 203d 2022 2222 0d0a 6176 6f69  otes = """..avoi
-00000900: 642d 6573 6361 7065 203d 2054 7275 650d  d-escape = True.
-00000910: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000920: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000930: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000004e0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+000004f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000500: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000510: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
+00000520: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000530: 7468 6f6e 203a 3a20 332e 3132 0d0a 0954  thon :: 3.12...T
+00000540: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000550: 203a 3a20 4669 6c65 2054 7261 6e73 6665   :: File Transfe
+00000560: 7220 5072 6f74 6f63 6f6c 2028 4654 5029  r Protocol (FTP)
+00000570: 0d0a 0954 6f70 6963 203a 3a20 536f 6674  ...Topic :: Soft
+00000580: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000590: 203a 3a20 4c69 6272 6172 6965 7320 3a3a   :: Libraries ::
+000005a0: 2050 7974 686f 6e20 4d6f 6475 6c65 730d   Python Modules.
+000005b0: 0a09 546f 7069 6320 3a3a 2055 7469 6c69  ..Topic :: Utili
+000005c0: 7469 6573 0d0a 0d0a 5b6f 7074 696f 6e73  ties....[options
+000005d0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+000005e0: 200d 0a09 3d20 2e0d 0a70 6163 6b61 6765   ...= ...package
+000005f0: 7320 3d20 6669 6e64 3a0d 0a7a 6970 5f73  s = find:..zip_s
+00000600: 6166 6520 3d20 4661 6c73 650d 0a69 6e73  afe = False..ins
+00000610: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000620: 0d0a 0963 6f6c 6f72 616d 610d 0a09 6b65  ...colorama...ke
+00000630: 7972 696e 670d 0a09 7079 7366 7470 0d0a  yring...pysftp..
+00000640: 0950 7959 414d 4c0d 0a0d 0a5b 6f70 7469  .PyYAML....[opti
+00000650: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000660: 645d 0d0a 7768 6572 6520 3d20 2e0d 0a69  d]..where = ...i
+00000670: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000680: 6174 6120 3d20 5472 7565 0d0a 6578 636c  ata = True..excl
+00000690: 7564 6520 3d20 0d0a 0974 6573 7473 0d0a  ude = ...tests..
+000006a0: 0d0a 5b6f 7074 696f 6e73 2e64 6174 615f  ..[options.data_
+000006b0: 6669 6c65 735d 0d0a 2e20 3d20 4348 414e  files]... = CHAN
+000006c0: 4745 4c4f 472e 6d64 0d0a 0d0a 5b6f 7074  GELOG.md....[opt
+000006d0: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
+000006e0: 735d 0d0a 636f 6e73 6f6c 655f 7363 7269  s]..console_scri
+000006f0: 7074 7320 3d20 0d0a 0970 7966 7470 7379  pts = ...pyftpsy
+00000700: 6e63 203d 2066 7470 7379 6e63 2e70 7966  nc = ftpsync.pyf
+00000710: 7470 7379 6e63 3a72 756e 0d0a 0d0a 5b63  tpsync:run....[c
+00000720: 6f76 6572 6167 653a 7275 6e5d 0d0a 6272  overage:run]..br
+00000730: 616e 6368 203d 2054 7275 650d 0a6f 6d69  anch = True..omi
+00000740: 7420 3d20 0d0a 0974 6573 7473 2f2a 0d0a  t = ...tests/*..
+00000750: 0d0a 5b63 6f76 6572 6167 653a 7265 706f  ..[coverage:repo
+00000760: 7274 5d0d 0a70 7265 6369 7369 6f6e 203d  rt]..precision =
+00000770: 2032 0d0a 736f 7274 203d 204e 616d 650d   2..sort = Name.
+00000780: 0a65 7863 6c75 6465 5f6c 696e 6573 203d  .exclude_lines =
+00000790: 200d 0a09 7072 6167 6d61 3a20 6e6f 2063   ...pragma: no c
+000007a0: 6f76 6572 0d0a 0969 6620 5f5f 6e61 6d65  over...if __name
+000007b0: 5f5f 203d 3d20 2e5f 5f6d 6169 6e5f 5f2e  __ == .__main__.
+000007c0: 3a0d 0a0d 0a5b 636f 7665 7261 6765 3a68  :....[coverage:h
+000007d0: 746d 6c5d 0d0a 6469 7265 6374 6f72 7920  tml]..directory 
+000007e0: 3d20 6275 696c 642f 636f 7665 7261 6765  = build/coverage
+000007f0: 0d0a 0d0a 5b74 6f6f 6c3a 7079 7465 7374  ....[tool:pytest
+00000800: 5d0d 0a6a 756e 6974 5f66 616d 696c 7920  ]..junit_family 
+00000810: 3d20 6c65 6761 6379 0d0a 0d0a 5b65 6767  = legacy....[egg
+00000820: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000830: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000840: 2030 0d0a 0d0a                            0....
```

