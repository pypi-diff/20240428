# Comparing `tmp/ddeutil-0.3.0.tar.gz` & `tmp/ddeutil-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil-0.3.0.tar", last modified: Mon Mar 11 04:34:52 2024, max compression
+gzip compressed data, was "ddeutil-0.3.1.tar", last modified: Sun Apr 28 06:33:08 2024, max compression
```

## Comparing `ddeutil-0.3.0.tar` & `ddeutil-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 04:34:52.330201 ddeutil-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-11 04:34:47.000000 ddeutil-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-11 04:34:52.330201 ddeutil-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-11 04:34:47.000000 ddeutil-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-11 04:34:47.000000 ddeutil-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 04:34:52.330201 ddeutil-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 04:34:52.326201 ddeutil-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 04:34:52.326201 ddeutil-0.3.0/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 04:34:52.330201 ddeutil-0.3.0/src/ddeutil/core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-11 04:34:47.000000 ddeutil-0.3.0/src/ddeutil/core/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-11 04:34:47.000000 ddeutil-0.3.0/src/ddeutil/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-03-11 04:34:47.000000 ddeutil-0.3.0/src/ddeutil/core/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-03-11 04:34:47.000000 ddeutil-0.3.0/src/ddeutil/core/dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-11 04:34:47.000000 ddeutil-0.3.0/src/ddeutil/core/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 04:34:52.330201 ddeutil-0.3.0/src/ddeutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-11 04:34:52.000000 ddeutil-0.3.0/src/ddeutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-11 04:34:52.000000 ddeutil-0.3.0/src/ddeutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 04:34:52.000000 ddeutil-0.3.0/src/ddeutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-11 04:34:52.000000 ddeutil-0.3.0/src/ddeutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 04:34:52.000000 ddeutil-0.3.0/src/ddeutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 04:34:52.330201 ddeutil-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-11 04:34:47.000000 ddeutil-0.3.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-11 04:34:47.000000 ddeutil-0.3.0/tests/test_dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-11 04:34:47.000000 ddeutil-0.3.0/tests/test_randomly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.343832 ddeutil-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 06:33:02.000000 ddeutil-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-28 06:33:08.343832 ddeutil-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-28 06:33:02.000000 ddeutil-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-28 06:33:02.000000 ddeutil-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:33:08.343832 ddeutil-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/ddeutil/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/ddeutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-28 06:33:02.000000 ddeutil-0.3.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-28 06:33:02.000000 ddeutil-0.3.1/tests/test_dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-28 06:33:02.000000 ddeutil-0.3.1/tests/test_randomly.py
```

### Comparing `ddeutil-0.3.0/LICENSE` & `ddeutil-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.0/README.md` & `ddeutil-0.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -44,62 +44,18 @@
     - elements
     - hash
     - merge
     - sorting
     - splitter
 ```
 
-#### Hash
-
-```python
-from ddeutil.core import random_str, hash_str
-
-assert hash_str('hello world') == '05751529'
-assert len(random_str()) == 8  # Random str with default length, 8
-```
-
-#### Checker
-
-```python
-from ddeutil.core import can_int, is_int
-
-assert is_int('-3')
-assert not is_int('0.0')
-assert not is_int('-3.1')
-
-assert can_int('-1.0')
-assert not can_int('1.1')
-```
-
-#### Convert
-
-```python
-from ddeutil.core import str2bool
-
-assert str2bool('yes')
-assert not str2bool('no')
-assert not str2bool('0')
-```
-
 ### Utility Functions
 
 ```text
 core
     - decorator
     - dtutils
 ```
 
-#### Date Utilities
-
-```python
-import datetime
-from ddeutil.core.dtutils import next_date
-
-assert (
-  next_date(datetime.datetime(2023, 1, 31, 0, 0, 0), mode='day')
-  == datetime.datetime(2023, 2, 1, 0, 0)
-)
-```
-
 ## License
 
 This project was licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `ddeutil-0.3.0/pyproject.toml` & `ddeutil-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -20,27 +20,27 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.9.13"
 dependencies = [
     "ujson==5.9.0",
     "tzdata==2024.1",
-    "python-dateutil==2.9.0",
+    "python-dateutil==2.9.0.post0",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.com/korawica/ddeutil/"
-"Source Code" = "https://github.com/korawica/ddeutil/"
+Homepage = "https://github.com/ddeutils/ddeutil/"
+"Source Code" = "https://github.com/ddeutils/ddeutil/"
 
 [project.optional-dependencies]
 dev = [
     "clishelf==0.2.0",
     "pytest==8.1.1",
-    "types-python-dateutil==2.8.19.20240311",
+    "types-python-dateutil==2.9.0.20240316",
 ]
 perf = [
     "memory_profiler==0.61.0",
     "perfplot==0.10.2,<1.0.0",
 ]
 
 [build-system]
```

### Comparing `ddeutil-0.3.0/src/ddeutil/core/__init__.py` & `ddeutil-0.3.1/src/ddeutil/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     random_str,
     # prepare
     remove_pad,
     round_up,
     rsplit,
     same_pwd,
     setdot,
-    sort_list_by_priority,
+    sort_priority,
     # split
     split,
     str2any,
     str2args,
     str2bool,
     str2dict,
     # Covert string to any types
```

### Comparing `ddeutil-0.3.0/src/ddeutil/core/dtutils.py` & `ddeutil-0.3.1/src/ddeutil/core/dtutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import calendar
 import datetime
 import enum
 from typing import (
     Optional,
     Union,
 )
-
-try:
-    from zoneinfo import ZoneInfo
-except ImportError:
-    from backports.zoneinfo import ZoneInfo
+from zoneinfo import ZoneInfo
 
 from dateutil import relativedelta
 
 LOCAL_TZ: ZoneInfo = ZoneInfo("Asia/Bangkok")
 
 DATETIME_SET: tuple[str, ...] = (
     "year",
```

### Comparing `ddeutil-0.3.0/src/ddeutil/core/threader.py` & `ddeutil-0.3.1/src/ddeutil/core/threader.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.0/tests/test_randomly.py` & `ddeutil-0.3.1/tests/test_randomly.py`

 * *Files identical despite different names*

