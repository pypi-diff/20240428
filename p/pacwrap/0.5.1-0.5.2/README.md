# Comparing `tmp/pacwrap-0.5.1.tar.gz` & `tmp/pacwrap-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacwrap-0.5.1.tar", max compression
+gzip compressed data, was "pacwrap-0.5.2.tar", max compression
```

## Comparing `pacwrap-0.5.1.tar` & `pacwrap-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-08-28 13:15:39.307970 pacwrap-0.5.1/LICENSE
--rw-r--r--   0        0        0     3819 2023-08-28 13:15:39.307970 pacwrap-0.5.1/README.md
--rw-r--r--   0        0        0       18 2023-12-05 17:45:24.951220 pacwrap-0.5.1/pacwrap/__init__.py
--rw-r--r--   0        0        0     1568 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/apt.py
--rw-r--r--   0        0        0     4719 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/cli.py
--rw-r--r--   0        0        0      347 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/dnf.py
--rw-r--r--   0        0        0     1774 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/mkhandler.py
--rw-r--r--   0        0        0     1993 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/options.py
--rw-r--r--   0        0        0     1512 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/pacman.py
--rw-r--r--   0        0        0     4596 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/pkgmgr.py
--rw-r--r--   0        0        0        0 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/py.typed
--rw-r--r--   0        0        0     1809 2023-08-28 13:15:39.307970 pacwrap-0.5.1/pacwrap/yum.py
--rw-r--r--   0        0        0     2307 2023-12-05 17:45:24.951220 pacwrap-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 pacwrap-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-08-28 13:15:39.307970 pacwrap-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3819 2023-08-28 13:15:39.307970 pacwrap-0.5.2/README.md
+-rw-r--r--   0        0        0       18 2024-04-28 15:48:23.862611 pacwrap-0.5.2/pacwrap/__init__.py
+-rw-r--r--   0        0        0     1568 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/apt.py
+-rw-r--r--   0        0        0     4719 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/cli.py
+-rw-r--r--   0        0        0      347 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/dnf.py
+-rw-r--r--   0        0        0     1774 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/mkhandler.py
+-rw-r--r--   0        0        0     2061 2024-04-28 15:48:23.862611 pacwrap-0.5.2/pacwrap/options.py
+-rw-r--r--   0        0        0     1512 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/pacman.py
+-rw-r--r--   0        0        0     4596 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/pkgmgr.py
+-rw-r--r--   0        0        0        0 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/py.typed
+-rw-r--r--   0        0        0     1809 2023-08-28 13:15:39.307970 pacwrap-0.5.2/pacwrap/yum.py
+-rw-r--r--   0        0        0     2121 2024-04-28 15:48:23.862611 pacwrap-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 pacwrap-0.5.2/PKG-INFO
```

### Comparing `pacwrap-0.5.1/LICENSE` & `pacwrap-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/README.md` & `pacwrap-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pacwrap/apt.py` & `pacwrap-0.5.2/pacwrap/apt.py`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pacwrap/cli.py` & `pacwrap-0.5.2/pacwrap/cli.py`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pacwrap/mkhandler.py` & `pacwrap-0.5.2/pacwrap/mkhandler.py`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pacwrap/options.py` & `pacwrap-0.5.2/pacwrap/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import os
 from typing import Optional
 
 from wtforglib.kinds import Fspec, StrAnyDict
 
 
-class Options(object):
-    """Class to manage opstions."""
+class Options:
+    """Class to manage options."""
 
     debug: int
-    output: Fspec
+    output: Optional[Fspec]
     quiet: bool
     names_only: bool
     refresh: bool
     verbose: int
     test: bool
     errors: int
 
     def __init__(self, opts: Optional[StrAnyDict] = None):
         """Construct options class."""
         if opts is None:
             opts = {}
         self.debug = opts.get("debug", 0)
-        self.output = str(opts.get("output", ""))
+        self.output = str(opts.get("output", None))
+        if self.output == "None":
+            self.output = None
         self.quiet = opts.get("quiet", False)
         self.names_only = opts.get("names_only", False)
         self.refresh = opts.get("refresh", False)
         self.verbose = opts.get("verbose", 0)
         self.test = opts.get("test", False)
         self.errors = 0
         if self.test:
```

### Comparing `pacwrap-0.5.1/pacwrap/pacman.py` & `pacwrap-0.5.2/pacwrap/pacman.py`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pacwrap/pkgmgr.py` & `pacwrap-0.5.2/pacwrap/pkgmgr.py`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pacwrap/yum.py` & `pacwrap-0.5.2/pacwrap/yum.py`

 * *Files identical despite different names*

### Comparing `pacwrap-0.5.1/pyproject.toml` & `pacwrap-0.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pacwrap"
 description = "Provides single interface to several common Linux package managers."
-version = "0.5.1"
+version = "0.5.2"
 license = "MIT"
 
 authors = ["Quien Sabe <qs5779@mail.com>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/wtfo-guru/pacwrap"
@@ -17,71 +17,64 @@
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
   "Intended Audience :: System Administrators",
   "Operating System :: POSIX :: Linux",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
 
 [tool.poetry.scripts]
 pacwrap = "pacwrap.cli:main"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<4.0"
 click = "^8.1.0"
-distro = "^1.8.0"
-wtforglib = ">= 0.7.0"
+distro = "^1.9"
+wtforglib = "^0.8"
 cmp-version = "^3.0.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-mypy = "^1.5.0"
-wemake-python-styleguide = "^0.18"
+mypy = "^1.9"
+wemake-python-styleguide = "^0.19"
 flake8-pytest-style = "^1.6"
 doc8 = "^1.0"
-nitpick = ">=0.32,<0.35"
-safety = "^2.3"
-pytest = "^7.1"
-pytest-cov = "^4.0"
-pytest-randomly = "^3.12"
-bump2version = "^1.0.1"
-isort = "^5.11.2"
-black = ">=22.12,<24.0"
+nitpick = "^0.35"
+safety = ">=2.3,<4.0"
+pytest = ">=7.4,<9.0"
+pytest-cov = ">=4,<6"
+pytest-randomly = "^3.13"
+isort = "^5.13"
+black = ">=22.12,<25.0"
 setuptools = ">=65.6.3,<70.0.0"
 importlib-resources = ">=5.10.1,<7.0.0"
-importlib-metadata = { version = "<5.0", python = "<3.8" }
-requests-cache = ">=0.9,<1.2"
+importlib-metadata = "^7.0"
+requests-cache = ">=0.9,<1.3"
 jmespath = "^1.0"
 pytest-click = "^1.1.0"
-wheel = ">=0.41.1,<0.43.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5.2,<8.0"
-sphinx-autodoc-typehints = "^1.19"
+sphinx-autodoc-typehints = ">=1.19,<3.0"
 m2r2 = "^0.3"
 tomli = "^2.0"
 
 
-[tool.poetry.group.dev.dependencies]
-packaging = ">=22,<24"
-
-
 [[tool.poetry.source]]
 name = "test-pypi"
 url = "https://test.pypi.org/simple/"
 priority = "supplemental"
 
 
 [[tool.poetry.source]]
```

### Comparing `pacwrap-0.5.1/PKG-INFO` & `pacwrap-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: pacwrap
-Version: 0.5.1
+Version: 0.5.2
 Summary: Provides single interface to several common Linux package managers.
 Home-page: https://github.com/wtfo-guru/pacwrap
 License: MIT
 Author: Quien Sabe
 Author-email: qs5779@mail.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: cmp-version (>=3.0.0,<4.0.0)
-Requires-Dist: distro (>=1.8.0,<2.0.0)
-Requires-Dist: wtforglib (>=0.7.0)
+Requires-Dist: distro (>=1.9,<2.0)
+Requires-Dist: wtforglib (>=0.8,<0.9)
 Project-URL: Documentation, https://python-pacwrap.readthedocs.io/en/stable
 Description-Content-Type: text/markdown
 
 # pacwrap
 
 [![Build Status](https://github.com/wtfo-guru/python-pacwrap/workflows/test/badge.svg?branch=main&event=push)](https://github.com/wtfo-guru/python-pacwrap/actions?query=workflow%3Atest)
 [![codecov](https://codecov.io/gh/wtfo-guru/python-pacwrap/branch/main/graph/badge.svg)](https://codecov.io/gh/wtfo-guru/python-pacwrap)
```

