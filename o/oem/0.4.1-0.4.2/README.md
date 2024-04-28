# Comparing `tmp/oem-0.4.1.tar.gz` & `tmp/oem-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oem-0.4.1.tar", last modified: Sun Mar 10 00:50:03 2024, max compression
+gzip compressed data, was "oem-0.4.2.tar", last modified: Sun Apr 28 01:02:31 2024, max compression
```

## Comparing `oem-0.4.1.tar` & `oem-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-03-10 00:50:03.686819 oem-0.4.1/
--rw-rw-r--   0 brad      (1000) brad      (1000)     1066 2024-03-10 00:42:37.000000 oem-0.4.1/LICENSE
--rw-r--r--   0 brad      (1000) brad      (1000)     4863 2024-03-10 00:50:03.686819 oem-0.4.1/PKG-INFO
--rw-rw-r--   0 brad      (1000) brad      (1000)     3581 2024-03-10 00:42:37.000000 oem-0.4.1/README.md
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-03-10 00:50:03.682819 oem-0.4.1/oem/
--rw-rw-r--   0 brad      (1000) brad      (1000)      115 2024-03-10 00:42:37.000000 oem-0.4.1/oem/__init__.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     2546 2024-03-10 00:42:37.000000 oem-0.4.1/oem/base.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     9887 2024-03-10 00:42:37.000000 oem-0.4.1/oem/compare.py
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-03-10 00:50:03.682819 oem-0.4.1/oem/components/
--rw-rw-r--   0 brad      (1000) brad      (1000)      251 2024-03-10 00:42:37.000000 oem-0.4.1/oem/components/__init__.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     1845 2024-03-10 00:42:37.000000 oem-0.4.1/oem/components/header.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     6022 2024-03-10 00:42:37.000000 oem-0.4.1/oem/components/metadata.py
--rw-rw-r--   0 brad      (1000) brad      (1000)    10561 2024-03-10 00:42:37.000000 oem-0.4.1/oem/components/segment.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     5417 2024-03-10 00:42:37.000000 oem-0.4.1/oem/components/types.py
--rw-rw-r--   0 brad      (1000) brad      (1000)    11961 2024-03-10 00:42:37.000000 oem-0.4.1/oem/interface.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     5205 2024-03-10 00:42:37.000000 oem-0.4.1/oem/interp.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     7018 2024-03-10 00:42:37.000000 oem-0.4.1/oem/parsers.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     3769 2024-03-10 00:42:37.000000 oem-0.4.1/oem/tle.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     7513 2024-03-10 00:42:37.000000 oem-0.4.1/oem/tools.py
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-03-10 00:50:03.686819 oem-0.4.1/oem.egg-info/
--rw-r--r--   0 brad      (1000) brad      (1000)     4863 2024-03-10 00:50:03.000000 oem-0.4.1/oem.egg-info/PKG-INFO
--rw-rw-r--   0 brad      (1000) brad      (1000)      518 2024-03-10 00:50:03.000000 oem-0.4.1/oem.egg-info/SOURCES.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)        1 2024-03-10 00:50:03.000000 oem-0.4.1/oem.egg-info/dependency_links.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)      129 2024-03-10 00:50:03.000000 oem-0.4.1/oem.egg-info/requires.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)        4 2024-03-10 00:50:03.000000 oem-0.4.1/oem.egg-info/top_level.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)     1095 2024-03-10 00:48:27.000000 oem-0.4.1/pyproject.toml
--rw-rw-r--   0 brad      (1000) brad      (1000)       38 2024-03-10 00:50:03.686819 oem-0.4.1/setup.cfg
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-03-10 00:50:03.682819 oem-0.4.1/tests/
--rw-rw-r--   0 brad      (1000) brad      (1000)     3514 2024-03-10 00:42:37.000000 oem-0.4.1/tests/test_compare.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     5321 2024-03-10 00:42:37.000000 oem-0.4.1/tests/test_interpolation.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     3114 2024-03-10 00:42:37.000000 oem-0.4.1/tests/test_samples.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     1608 2024-03-10 00:42:37.000000 oem-0.4.1/tests/test_tle.py
--rw-rw-r--   0 brad      (1000) brad      (1000)      208 2021-05-30 21:45:46.000000 oem-0.4.1/tests/test_tools.py
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-28 01:02:31.063731 oem-0.4.2/
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1066 2024-03-10 00:42:37.000000 oem-0.4.2/LICENSE
+-rw-r--r--   0 brad      (1000) brad      (1000)     4725 2024-04-28 01:02:31.063731 oem-0.4.2/PKG-INFO
+-rw-rw-r--   0 brad      (1000) brad      (1000)     3443 2024-03-10 00:59:57.000000 oem-0.4.2/README.md
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-28 01:02:31.059731 oem-0.4.2/oem/
+-rw-rw-r--   0 brad      (1000) brad      (1000)      115 2024-03-10 00:42:37.000000 oem-0.4.2/oem/__init__.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     2546 2024-03-10 00:42:37.000000 oem-0.4.2/oem/base.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     9887 2024-03-10 00:42:37.000000 oem-0.4.2/oem/compare.py
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-28 01:02:31.059731 oem-0.4.2/oem/components/
+-rw-rw-r--   0 brad      (1000) brad      (1000)      251 2024-03-10 00:42:37.000000 oem-0.4.2/oem/components/__init__.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1845 2024-03-10 00:42:37.000000 oem-0.4.2/oem/components/header.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     6022 2024-03-10 00:42:37.000000 oem-0.4.2/oem/components/metadata.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)    10561 2024-03-10 00:42:37.000000 oem-0.4.2/oem/components/segment.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     5417 2024-03-10 00:42:37.000000 oem-0.4.2/oem/components/types.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)    11961 2024-03-10 00:42:37.000000 oem-0.4.2/oem/interface.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     5205 2024-03-10 00:42:37.000000 oem-0.4.2/oem/interp.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     7018 2024-03-10 00:42:37.000000 oem-0.4.2/oem/parsers.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     3769 2024-03-10 00:42:37.000000 oem-0.4.2/oem/tle.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     7555 2024-04-28 00:59:44.000000 oem-0.4.2/oem/tools.py
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-28 01:02:31.063731 oem-0.4.2/oem.egg-info/
+-rw-r--r--   0 brad      (1000) brad      (1000)     4725 2024-04-28 01:02:31.000000 oem-0.4.2/oem.egg-info/PKG-INFO
+-rw-rw-r--   0 brad      (1000) brad      (1000)      518 2024-04-28 01:02:31.000000 oem-0.4.2/oem.egg-info/SOURCES.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)        1 2024-04-28 01:02:31.000000 oem-0.4.2/oem.egg-info/dependency_links.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)      129 2024-04-28 01:02:31.000000 oem-0.4.2/oem.egg-info/requires.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)        4 2024-04-28 01:02:31.000000 oem-0.4.2/oem.egg-info/top_level.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1095 2024-04-28 01:01:49.000000 oem-0.4.2/pyproject.toml
+-rw-rw-r--   0 brad      (1000) brad      (1000)       38 2024-04-28 01:02:31.063731 oem-0.4.2/setup.cfg
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-28 01:02:31.063731 oem-0.4.2/tests/
+-rw-rw-r--   0 brad      (1000) brad      (1000)     3514 2024-03-10 00:42:37.000000 oem-0.4.2/tests/test_compare.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     5321 2024-03-10 00:42:37.000000 oem-0.4.2/tests/test_interpolation.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     3114 2024-03-10 00:42:37.000000 oem-0.4.2/tests/test_samples.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1608 2024-03-10 00:42:37.000000 oem-0.4.2/tests/test_tle.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)      568 2024-04-28 00:59:44.000000 oem-0.4.2/tests/test_tools.py
```

### Comparing `oem-0.4.1/LICENSE` & `oem-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/PKG-INFO` & `oem-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oem
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python Orbit Ephemeris Message (OEM) tools
 Author-email: Brad Sease <bradsease@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +37,15 @@
 Python tools for working with Orbit Ephemeris Messages (OEMs).
 
 
 ## Development Status
 
 [![GitHub Release](https://img.shields.io/github/v/release/bradsease/oem)](https://github.com/bradsease/oem/releases) [![GitHub](https://img.shields.io/github/license/bradsease/oem)](https://github.com/bradsease/oem/blob/main/LICENSE)
 
-[![GitHub last commit](https://img.shields.io/github/last-commit/bradsease/oem)](https://github.com/bradsease/oem) [![Pipeline Status](https://github.com/bradsease/oem/actions/workflows/python-package.yml/badge.svg)](https://github.com/bradsease/oem/actions/workflows/python-package.yml) [![Coverage Status](https://coveralls.io/repos/github/bradsease/oem/badge.svg)](https://coveralls.io/github/bradsease/oem) [![Documentation Status](https://readthedocs.org/projects/oem/badge/?version=latest)](https://oem.readthedocs.io/en/latest/?badge=latest)
+[![GitHub last commit](https://img.shields.io/github/last-commit/bradsease/oem)](https://github.com/bradsease/oem) [![Pipeline Status](https://github.com/bradsease/oem/actions/workflows/python-package.yml/badge.svg)](https://github.com/bradsease/oem/actions/workflows/python-package.yml) [![Coverage Status](https://coveralls.io/repos/github/bradsease/oem/badge.svg)](https://coveralls.io/github/bradsease/oem)
 
 
 ## Installation
 The `oem` package is available through `pip`.
 ```
 pip install oem
 ```
```

### Comparing `oem-0.4.1/README.md` & `oem-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Python tools for working with Orbit Ephemeris Messages (OEMs).
 
 
 ## Development Status
 
 [![GitHub Release](https://img.shields.io/github/v/release/bradsease/oem)](https://github.com/bradsease/oem/releases) [![GitHub](https://img.shields.io/github/license/bradsease/oem)](https://github.com/bradsease/oem/blob/main/LICENSE)
 
-[![GitHub last commit](https://img.shields.io/github/last-commit/bradsease/oem)](https://github.com/bradsease/oem) [![Pipeline Status](https://github.com/bradsease/oem/actions/workflows/python-package.yml/badge.svg)](https://github.com/bradsease/oem/actions/workflows/python-package.yml) [![Coverage Status](https://coveralls.io/repos/github/bradsease/oem/badge.svg)](https://coveralls.io/github/bradsease/oem) [![Documentation Status](https://readthedocs.org/projects/oem/badge/?version=latest)](https://oem.readthedocs.io/en/latest/?badge=latest)
+[![GitHub last commit](https://img.shields.io/github/last-commit/bradsease/oem)](https://github.com/bradsease/oem) [![Pipeline Status](https://github.com/bradsease/oem/actions/workflows/python-package.yml/badge.svg)](https://github.com/bradsease/oem/actions/workflows/python-package.yml) [![Coverage Status](https://coveralls.io/repos/github/bradsease/oem/badge.svg)](https://coveralls.io/github/bradsease/oem)
 
 
 ## Installation
 The `oem` package is available through `pip`.
 ```
 pip install oem
 ```
```

### Comparing `oem-0.4.1/oem/base.py` & `oem-0.4.2/oem/base.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/compare.py` & `oem-0.4.2/oem/compare.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/components/header.py` & `oem-0.4.2/oem/components/header.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/components/metadata.py` & `oem-0.4.2/oem/components/metadata.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/components/segment.py` & `oem-0.4.2/oem/components/segment.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/components/types.py` & `oem-0.4.2/oem/components/types.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/interface.py` & `oem-0.4.2/oem/interface.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/interp.py` & `oem-0.4.2/oem/interp.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/parsers.py` & `oem-0.4.2/oem/parsers.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/tle.py` & `oem-0.4.2/oem/tle.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/oem/tools.py` & `oem-0.4.2/oem/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     Args:
         epoch (str): OEM epoch string.
 
     Returns:
         parsed_epoch (Time): UTC epoch.
     """
-    return Time(parse_datetime(epoch), format="datetime", scale="utc")
+    return Time(parse_datetime(epoch), format="datetime", scale="utc", precision=6)
 
 
 def parse_epoch(epoch, metadata):
     """Parse OEM standard epoch using metadata TIME_SYSTEM.
 
     Args:
         epoch (str): OEM epoch string.
@@ -66,15 +66,15 @@
             timescale indicated by TIME_SYSTEM is not supported by astropy,
             then parsed_epoch will warn the user and fall back to DateTime. In
             this case, time calculations may be inaccurate.
     """
     time_system = metadata["TIME_SYSTEM"].lower()
     dt_epoch = parse_datetime(epoch)
     if time_system in Time.SCALES:
-        parsed_epoch = Time(dt_epoch, format="datetime", scale=time_system)
+        parsed_epoch = Time(dt_epoch, format="datetime", scale=time_system, precision=6)
     else:
         warnings.warn(
             f"Unsupported TIME_SYSTEM '{time_system}', falling back to "
             f"DateTime. Use caution with time calculations."
         )
         parsed_epoch = dt_epoch
     return parsed_epoch
@@ -107,15 +107,15 @@
     """
     time_system = metadata["TIME_SYSTEM"].lower()
     fmt = _identify_epoch_format(epochs[0])
     if fmt != "isot":
         epochs = tuple(_coerce_epoch_yday(epoch) for epoch in epochs)
 
     if time_system in Time.SCALES:
-        parsed_epochs = Time(epochs, format=fmt, scale=time_system)
+        parsed_epochs = Time(epochs, format=fmt, scale=time_system, precision=6)
     else:
         warnings.warn(
             f"Unsupported TIME_SYSTEM '{time_system}', falling back to "
             f"DateTime. Use caution with time calculations."
         )
         parsed_epochs = tuple(parse_epoch(epoch, metadata) for epoch in epochs)
 
@@ -155,15 +155,15 @@
 def format_epoch(epoch):
     """Format an epoch in the standard OEM format.
 
     Args:
         epoch (Time, DateTime): Epoch to convert to string.
 
     Returns:
-        formatted_epoch (str): Epoch in YYYY-MM-DDTHH:MM:SS.sss format.
+        formatted_epoch (str): Epoch in YYYY-MM-DDTHH:MM:SS.ssssss format.
     """
     return epoch.strftime("%Y-%m-%dT%H:%M:%S.%f")
 
 
 def require(boolean, message):
     """Require a boolean condition.
```

### Comparing `oem-0.4.1/oem.egg-info/PKG-INFO` & `oem-0.4.2/oem.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oem
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python Orbit Ephemeris Message (OEM) tools
 Author-email: Brad Sease <bradsease@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +37,15 @@
 Python tools for working with Orbit Ephemeris Messages (OEMs).
 
 
 ## Development Status
 
 [![GitHub Release](https://img.shields.io/github/v/release/bradsease/oem)](https://github.com/bradsease/oem/releases) [![GitHub](https://img.shields.io/github/license/bradsease/oem)](https://github.com/bradsease/oem/blob/main/LICENSE)
 
-[![GitHub last commit](https://img.shields.io/github/last-commit/bradsease/oem)](https://github.com/bradsease/oem) [![Pipeline Status](https://github.com/bradsease/oem/actions/workflows/python-package.yml/badge.svg)](https://github.com/bradsease/oem/actions/workflows/python-package.yml) [![Coverage Status](https://coveralls.io/repos/github/bradsease/oem/badge.svg)](https://coveralls.io/github/bradsease/oem) [![Documentation Status](https://readthedocs.org/projects/oem/badge/?version=latest)](https://oem.readthedocs.io/en/latest/?badge=latest)
+[![GitHub last commit](https://img.shields.io/github/last-commit/bradsease/oem)](https://github.com/bradsease/oem) [![Pipeline Status](https://github.com/bradsease/oem/actions/workflows/python-package.yml/badge.svg)](https://github.com/bradsease/oem/actions/workflows/python-package.yml) [![Coverage Status](https://coveralls.io/repos/github/bradsease/oem/badge.svg)](https://coveralls.io/github/bradsease/oem)
 
 
 ## Installation
 The `oem` package is available through `pip`.
 ```
 pip install oem
 ```
```

### Comparing `oem-0.4.1/oem.egg-info/SOURCES.txt` & `oem-0.4.2/oem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/pyproject.toml` & `oem-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "oem"
 description = "Python Orbit Ephemeris Message (OEM) tools"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
     { name = "Brad Sease", email = "bradsease@gmail.com" }
 ]
 readme = "README.md"
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `oem-0.4.1/tests/test_compare.py` & `oem-0.4.2/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/tests/test_interpolation.py` & `oem-0.4.2/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/tests/test_samples.py` & `oem-0.4.2/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `oem-0.4.1/tests/test_tle.py` & `oem-0.4.2/tests/test_tle.py`

 * *Files identical despite different names*

