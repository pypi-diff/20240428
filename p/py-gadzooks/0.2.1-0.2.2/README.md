# Comparing `tmp/py_gadzooks-0.2.1.tar.gz` & `tmp/py_gadzooks-0.2.2.tar.gz`

## Comparing `py_gadzooks-0.2.1.tar` & `py_gadzooks-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/gadzooks/__init__.py
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/gadzooks/check_version.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/gadzooks/loc_summarize.py
--rwxr-xr-x   0        0        0      858 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/gadzooks/main.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/LICENSE
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/README.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 py_gadzooks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/gadzooks/__init__.py
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/gadzooks/check_version.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/gadzooks/loc_summarize.py
+-rwxr-xr-x   0        0        0      858 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/gadzooks/main.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 py_gadzooks-0.2.2/PKG-INFO
```

### Comparing `py_gadzooks-0.2.1/gadzooks/__init__.py` & `py_gadzooks-0.2.2/gadzooks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser, Namespace
 import sys
 from typing import ClassVar
 
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 
 def error(msg: str, strict: bool = True) -> None:
     """Prints an error message and exits the program with return code 1.
     If strict=False, makes it a warning and does not exit."""
     if strict:
         print(f'ERROR: {msg}', file=sys.stderr)
```

### Comparing `py_gadzooks-0.2.1/gadzooks/check_version.py` & `py_gadzooks-0.2.2/gadzooks/check_version.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.1/gadzooks/loc_summarize.py` & `py_gadzooks-0.2.2/gadzooks/loc_summarize.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.1/gadzooks/main.py` & `py_gadzooks-0.2.2/gadzooks/main.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.1/LICENSE` & `py_gadzooks-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.1/README.md` & `py_gadzooks-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # 🪝 Gadzooks 🪝
 
-[![PyPI - Version](https://img.shields.io/pypi/v/gadzooks)](https://pypi.org/project/gadzooks)
+[![PyPI - Version](https://img.shields.io/pypi/v/py-gadzooks)](https://pypi.org/project/py-gadzooks)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/jeremander/gadzooks/main/LICENSE)
 
 <!-- [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gadzooks.svg)](https://pypi.org/project/gadzooks) -->
 
 -----
 
 A collection of code maintenance tools for Python projects. These are especially useful as [pre-commit](https://pre-commit.com) hooks.
```

### Comparing `py_gadzooks-0.2.1/pyproject.toml` & `py_gadzooks-0.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,17 @@
   "Programming Language :: Python"
 ]
 dependencies = [
   "radon",
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/gadzooks#readme"
-Issues = "https://github.com/unknown/gadzooks/issues"
-Source = "https://github.com/unknown/gadzooks"
+Documentation = "https://github.com/jeremander/gadzooks#readme"
+Issues = "https://github.com/jeremander/gadzooks/issues"
+Source = "https://github.com/jeremander/gadzooks"
 
 [project.scripts]
 gadzooks = "gadzooks.main:main"
 
 [tool.hatch.version]
 path = "gadzooks/__init__.py"
```

### Comparing `py_gadzooks-0.2.1/PKG-INFO` & `py_gadzooks-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.3
 Name: py-gadzooks
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of code maintenance tools for Python projects, intended to be used within git hooks.
-Project-URL: Documentation, https://github.com/unknown/gadzooks#readme
-Project-URL: Issues, https://github.com/unknown/gadzooks/issues
-Project-URL: Source, https://github.com/unknown/gadzooks
+Project-URL: Documentation, https://github.com/jeremander/gadzooks#readme
+Project-URL: Issues, https://github.com/jeremander/gadzooks/issues
+Project-URL: Source, https://github.com/jeremander/gadzooks
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Requires-Dist: radon
 Description-Content-Type: text/markdown
 
 # 🪝 Gadzooks 🪝
 
-[![PyPI - Version](https://img.shields.io/pypi/v/gadzooks)](https://pypi.org/project/gadzooks)
+[![PyPI - Version](https://img.shields.io/pypi/v/py-gadzooks)](https://pypi.org/project/py-gadzooks)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/jeremander/gadzooks/main/LICENSE)
 
 <!-- [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gadzooks.svg)](https://pypi.org/project/gadzooks) -->
 
 -----
 
 A collection of code maintenance tools for Python projects. These are especially useful as [pre-commit](https://pre-commit.com) hooks.
```

