# Comparing `tmp/pytak-6.3.2.tar.gz` & `tmp/pytak-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytak-6.3.2.tar", last modified: Sat Mar  2 00:53:30 2024, max compression
+gzip compressed data, was "pytak-6.4.0.tar", last modified: Sun Apr 28 21:12:18 2024, max compression
```

## Comparing `pytak-6.3.2.tar` & `pytak-6.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:53:30.486235 pytak-6.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-02 00:53:21.000000 pytak-6.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-02 00:53:21.000000 pytak-6.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-02 00:53:30.486235 pytak-6.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-02 00:53:21.000000 pytak-6.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-02 00:53:21.000000 pytak-6.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:53:30.482235 pytak-6.3.2/pytak/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:53:30.486235 pytak-6.3.2/pytak/asyncio_dgram/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/asyncio_dgram/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/asyncio_dgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/asyncio_dgram/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)    14506 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16097 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/client_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/crypto_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-03-02 00:53:21.000000 pytak-6.3.2/pytak/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:53:30.486235 pytak-6.3.2/pytak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-02 00:53:30.000000 pytak-6.3.2/pytak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-02 00:53:30.000000 pytak-6.3.2/pytak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 00:53:30.000000 pytak-6.3.2/pytak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-02 00:53:30.000000 pytak-6.3.2/pytak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-02 00:53:30.000000 pytak-6.3.2/pytak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-02 00:53:30.486235 pytak-6.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-02 00:53:21.000000 pytak-6.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:53:30.486235 pytak-6.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-03-02 00:53:21.000000 pytak-6.3.2/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-03-02 00:53:21.000000 pytak-6.3.2/tests/test_client_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-02 00:53:21.000000 pytak-6.3.2/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-02 00:53:21.000000 pytak-6.3.2/tests/test_pref_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-02 00:53:21.000000 pytak-6.3.2/tests/test_pytak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:18.049484 pytak-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-28 21:12:06.000000 pytak-6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 21:12:06.000000 pytak-6.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-28 21:12:18.049484 pytak-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-28 21:12:06.000000 pytak-6.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-28 21:12:06.000000 pytak-6.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:18.045484 pytak-6.4.0/pytak/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:18.049484 pytak-6.4.0/pytak/asyncio_dgram/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/asyncio_dgram/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/asyncio_dgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/asyncio_dgram/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14506 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16097 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/client_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/crypto_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-28 21:12:06.000000 pytak-6.4.0/pytak/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:18.049484 pytak-6.4.0/pytak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-28 21:12:18.000000 pytak-6.4.0/pytak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-28 21:12:18.000000 pytak-6.4.0/pytak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:12:18.000000 pytak-6.4.0/pytak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-28 21:12:18.000000 pytak-6.4.0/pytak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 21:12:18.000000 pytak-6.4.0/pytak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-28 21:12:18.049484 pytak-6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-28 21:12:06.000000 pytak-6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:18.049484 pytak-6.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-28 21:12:06.000000 pytak-6.4.0/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-28 21:12:06.000000 pytak-6.4.0/tests/test_client_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-28 21:12:06.000000 pytak-6.4.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-28 21:12:06.000000 pytak-6.4.0/tests/test_pref_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-28 21:12:06.000000 pytak-6.4.0/tests/test_pytak.py
```

### Comparing `pytak-6.3.2/LICENSE` & `pytak-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/PKG-INFO` & `pytak-6.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytak
-Version: 6.3.2
+Version: 6.4.0
 Summary: PyTAK: Python Team Awareness Kit Module
 Home-page: https://github.com/snstac/pytak
 Author-email: Greg Albrecht <oss@undef.net>
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Keywords: Cursor on Target,CoT,ATAK,TAK,WinTAK,TAK,TAK Server
```

### Comparing `pytak-6.3.2/README.rst` & `pytak-6.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/__init__.py` & `pytak-6.4.0/pytak/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 
 """Python Team Awareness Kit (PyTAK) Module.
 
 :source: <https://github.com/snstac/pytak>
 """
 
-__version__ = "6.3.2"
+__version__ = "6.4.0"
 
 
 from .constants import (  # NOQA
     LOG_LEVEL,
     LOG_FORMAT,
     DEFAULT_COT_PORT,
     DEFAULT_BACKOFF,
```

### Comparing `pytak-6.3.2/pytak/asyncio_dgram/LICENSE` & `pytak-6.4.0/pytak/asyncio_dgram/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/asyncio_dgram/aio.py` & `pytak-6.4.0/pytak/asyncio_dgram/aio.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/classes.py` & `pytak-6.4.0/pytak/classes.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/client_functions.py` & `pytak-6.4.0/pytak/client_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/commands.py` & `pytak-6.4.0/pytak/commands.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/constants.py` & `pytak-6.4.0/pytak/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 
 # await asyncio.sleep(0) should allow co-routines to yield, but they end up
 # eating 100% CPU. @PeterQFR found bumping this to 0.1 solved the high CPU
 # issue. See: https://github.com/snstac/pytak/pull/22
 DEFAULT_MIN_ASYNC_SLEEP: float = 0.1
 
 # TAK Protocol to use for CoT output, one of: 0 (XML, default), 1 (Mesh/Stream).
-DEFAULT_TAK_PROTO: str = "1"
+# Doesn't always work with iTAK. Recommend sticking with 0 (XML).
+DEFAULT_TAK_PROTO: str = "0"
 
 # Python <3.8 has no way of including XML Declaration in ET.tostring():
 DEFAULT_XML_DECLARATION: bytes = (
     b'<?xml version="1.0" encoding="UTF-8" standalone="yes" ?>'
 )
 
 # Multicast
```

### Comparing `pytak-6.3.2/pytak/crypto_functions.py` & `pytak-6.4.0/pytak/crypto_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak/functions.py` & `pytak-6.4.0/pytak/functions.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/pytak.egg-info/PKG-INFO` & `pytak-6.4.0/pytak.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytak
-Version: 6.3.2
+Version: 6.4.0
 Summary: PyTAK: Python Team Awareness Kit Module
 Home-page: https://github.com/snstac/pytak
 Author-email: Greg Albrecht <oss@undef.net>
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Keywords: Cursor on Target,CoT,ATAK,TAK,WinTAK,TAK,TAK Server
```

### Comparing `pytak-6.3.2/pytak.egg-info/SOURCES.txt` & `pytak-6.4.0/pytak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/setup.cfg` & `pytak-6.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/setup.py` & `pytak-6.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/tests/test_classes.py` & `pytak-6.4.0/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/tests/test_client_functions.py` & `pytak-6.4.0/tests/test_client_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/tests/test_functions.py` & `pytak-6.4.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/tests/test_pref_packages.py` & `pytak-6.4.0/tests/test_pref_packages.py`

 * *Files identical despite different names*

### Comparing `pytak-6.3.2/tests/test_pytak.py` & `pytak-6.4.0/tests/test_pytak.py`

 * *Files identical despite different names*

