# Comparing `tmp/python_repeatable_iterable-2.1.2.tar.gz` & `tmp/python_repeatable_iterable-2.1.3.tar.gz`

## Comparing `python_repeatable_iterable-2.1.2.tar` & `python_repeatable_iterable-2.1.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/CONTRIBUTORS.md
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/src/python_repeatable_iterable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/src/python_repeatable_iterable/py.typed
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/typing_test/__init__.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/COPYING.LESSER
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/README.md
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    13589 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/README_printable.md
+-rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/build_and_checks.sh
+-rwxr-xr-x   0        0        0     1021 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/build_readme.sh
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/src/python_repeatable_iterable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/src/python_repeatable_iterable/py.typed
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/typing_test/__init__.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/COPYING.LESSER
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/README.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/PKG-INFO
```

### Comparing `python_repeatable_iterable-2.1.2/src/python_repeatable_iterable/__init__.py` & `python_repeatable_iterable-2.1.3/src/python_repeatable_iterable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
 This file is part of python-repeatable-iterable library.
 
 python-repeatable-iterable is free software:
-you can redistribute it and/or modify it
-under the terms of the GNU Lesser General Public License
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
 as published by the Free Software Foundation,
 either version 3 of the License,
 or (at your option) any later version.
 
-python-repeatable-iterable is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
+python-repeatable-iterable is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with python-repeatable-iterable.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------------
+----------------------------------------------------------------------
 from typing import Iterable, NewType, Type
 from _collections_abc import dict_keys, dict_values, dict_items
 from python_none_objects import NoneIterable
 
 A first attempt at defining the RepeatableIterable type,
 but it is not generic.
 It defines a RepeatableIterable() function that cannot be subscripted.
 RepeatableIterable = NewType("RepeatableIterable", Iterable)
 
--------------------------------------------------------------------------------
+----------------------------------------------------------------------
 
-The following function is a first attempt that conveys the intent more clearly.
+The following function is a first attempt
+that conveys the intent more clearly.
 But it is not safe, see discussion just after.
 def get_repeatable_iterable(
     iterable: Iterable,
     safe_classes: Iterable[Type] = NoneIterable,
 ) -> RepeatableIterable:
     if isinstance(
         iterable,
@@ -84,17 +88,18 @@
 ... 
 >>> for x in s: print(x)
 ... 
 >>> isinstance(s, set)
 True
 
 See here a list of builtins that can be subclassed or not:
-https://stackoverflow.com/questions/10061752/which-classes-cannot-be-subclassed
+https://stackoverflow.com/questions/10061752
+/which-classes-cannot-be-subclassed
 
--------------------------------------------------------------------------------
+----------------------------------------------------------------------
 
 This second attempt has been included in the class RepeatableIterable.
 def get_repeatable_iterable(
     iterable: Iterable,
     safe_classes: Iterable[Type] = NoneIterable,
 ) -> RepeatableIterable:
     # Here is an implementation avoiding the previous problem.
@@ -143,14 +148,15 @@
         cls,
         iterable: Iterable[T],
         safe_classes: Iterable[type[object]] = NoneIterable,
     ) -> "RepeatableIterable[T]":
         """
         Here is an implementation avoiding the previous problem.
         """
+
         iterable_type = type(iterable)
         for some_class in (
             list,
             tuple,
             range,
             str,
             bytes,
```

### Comparing `python_repeatable_iterable-2.1.2/typing_test/__init__.py` & `python_repeatable_iterable-2.1.3/typing_test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 This file is part of python-repeatable-iterable library.
 
 python-repeatable-iterable is free software:
-you can redistribute it and/or modify it
-under the terms of the GNU Lesser General Public License
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
 as published by the Free Software Foundation,
 either version 3 of the License,
 or (at your option) any later version.
 
-python-repeatable-iterable is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
+python-repeatable-iterable is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with python-repeatable-iterable.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
 """
 
 import sys
@@ -35,14 +38,15 @@
     x: RepeatableIterable[List[T1]],
 ) -> List[T1]:
     """
     Check that mypy follows the types
     between the argument and the return of the function
     for the type of the content of the list.
     """
+
     result = []
     for y in x:
         result.extend(y)
     for y in x:
         result.extend(y)
     return result
 
@@ -52,14 +56,15 @@
 ) -> List[T1]:
     """
     Check that mypy follows the types
     between the argument and the return of the function
     for the type of the content of the list
     with indirections.
     """
+
     return test_arg_to_return_typing(RepeatableIterable(x))
 
 
 a: List[List[Never]] = [[], []]
 print(test_arg_to_return_via_call_typing(a))
 
 b = (x for x in a)
@@ -71,13 +76,14 @@
 ) -> RepeatableIterable[T1]:
     """
     Check that mypy follows the types
     between the argument and the return of the function
     for the type of the content of the list
     with a final cast.
     """
+
     result = []
     for y in x:
         result.extend(y)
     for y in x:
         result.extend(y)
     return RepeatableIterable(result)
```

### Comparing `python_repeatable_iterable-2.1.2/COPYING` & `python_repeatable_iterable-2.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.2/COPYING.LESSER` & `python_repeatable_iterable-2.1.3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.2/pyproject.toml` & `python_repeatable_iterable-2.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-repeatable-iterable"
-version = "2.1.2"
-description = "Add a RepeatableIterable type and a function to obtain it"
+version = "2.1.3"
+description = """\
+Add a RepeatableIterable type and a function to obtain it\
+"""
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
 license = { file = "COPYING.LESSER" }
 classifiers = [
-    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+    """\
+License :: OSI Approved :: \
+GNU Lesser General Public License v3 or later (LGPLv3+)\
+""",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Python", "Iterable", "Repeatable", "RepeatableIterable"]
 dependencies = [
    "python-none-objects==1.1.5",
@@ -31,15 +36,17 @@
     "isort",
     "mypy",
     "pylint",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/LLyaudet/python-repeatable-iterable"
-"Bug Tracker" = "https://github.com/LLyaudet/python-repeatable-iterable/issues"
+"Bug Tracker" = """\
+https://github.com/LLyaudet/python-repeatable-iterable/issues\
+"""
 
 [tool.black]
 line-length = 70
 
 [tool.isort]
 profile = "black"
 line_length = 70
```

### Comparing `python_repeatable_iterable-2.1.2/PKG-INFO` & `python_repeatable_iterable-2.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-repeatable-iterable
-Version: 2.1.2
+Version: 2.1.3
 Summary: Add a RepeatableIterable type and a function to obtain it
 Project-URL: Homepage, https://github.com/LLyaudet/python-repeatable-iterable
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-repeatable-iterable/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -184,36 +184,41 @@
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # python-repeatable-iterable
 
-[![pypi-version]][pypi]
-[![Downloads](https://img.shields.io/pypi/dm/python-repeatable-iterable)](https://pypistats.org/packages/python-repeatable-iterable)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![CodeFactor](https://www.codefactor.io/repository/github/llyaudet/python-repeatable-iterable/badge/main)](https://www.codefactor.io/repository/github/llyaudet/python-repeatable-iterable/overview/main)
-[![CodeClimateMaintainability](https://api.codeclimate.com/v1/badges/89044bfd52999e4f07f6/maintainability)](https://codeclimate.com/github/LLyaudet/python-repeatable-iterable/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1c70116c2d714e3889606519937cb11d)](https://app.codacy.com/gh/LLyaudet/python-repeatable-iterable/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-![GitHub top language](https://img.shields.io/github/languages/top/llyaudet/python-repeatable-iterable)
-![GitHub License](https://img.shields.io/github/license/llyaudet/python-repeatable-iterable)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-repeatable-iterable)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/llyaudet/python-repeatable-iterable)
-[![GitHub Sponsors](https://img.shields.io/github/sponsors/LLyaudet)](https://github.com/sponsors/LLyaudet)
+[![PyPI-version-badge]][PyPI-package-page]
+[![Downloads-badge]][PyPIStats-package-page]
+[![Code-style:black:badge]][Black-GitHub.com]
+[![Imports:isort:badge]][Isort-GitHub.io]
+[![Typecheck:mypy:badge]][Typecheck-mypy-lang.org]
+[![Linting:pylint:badge]][Pylint-GitHub.com]
+[![CodeFactor-badge]][CodeFactor-package-page]
+[![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
+[![Codacy-badge]][Codacy-package-page]
+![GitHub-top-language-badge]
+![GitHub-license-badge]
+![PyPI-python-version-badge]
+![GitHub-code-size-in-bytes-badge]
+
+| **A new type RepeatableIterable for Python** |
+|:--------------------------------------------:|
+|     **and a way to obtain one instance**     |
 
-|     **A new type RepeatableIterable for Python and a way to obtain one instance**     |
 
-Since in Python an Iterator is an Iterable and that you cannot iterate multiple times on an iterator,
+Since in Python an Iterator is an Iterable
+and that you cannot iterate multiple times on an iterator,
 you may encounter WTF bugs, even with type checking.
 This package provides possible solutions to this problem.
 See here for a discussion on this problem:
-<https://stackoverflow.com/questions/63104689/what-is-the-pythonic-way-to-represent-an-iterable-that-can-be-iterated-over-mult>
+<https://stackoverflow.com/questions/63104689>
+(/what-is-the-pythonic-way-to-represent-an-iterable
+-that-can-be-iterated-over-mult).
 
 Before:
 ```python3
 def foo(iterable: Iterable):
     for that in iterable:
         bar(that)
     for that in iterable:
@@ -247,23 +252,68 @@
         bar(that)
     for that in iterable:
         baz(that)
 
 foo(something)
 ```
 
-If you develop something where you have no control on what another dev might give you as input,
+If you develop something where you have no control on
+what another dev might give you as input,
 you have 2 possibilities:
 
 - hope for the best ;),
 - or harden your code to have less support work to do :).
 
 This applies if you dev something that is:
 
 - closed source or open source,
 - available to everyone on the Internet,
-  available only to customers or colleagues that you may personally know or not.
+  available only to customers or colleagues
+  that you may personally know or not.
 
-Solution 2 above is a nice solution with a reasonable performance cost :).
+Solution 2 above is a nice solution
+with a reasonable performance cost :).
+
+[PyPI-version-badge]: https://img.shields.io/pypi/v/python-repeatable-iterable.svg
+
+[PyPI-package-page]: https://pypi.org/project/python-repeatable-iterable/
+
+[Downloads-badge]: https://img.shields.io/pypi/dm/python-repeatable-iterable
+
+[PyPIStats-package-page]: https://pypistats.org/packages/python-repeatable-iterable
+
+[Code-style:black:badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+
+[Black-GitHub.com]: https://github.com/psf/black
+
+[Imports:isort:badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+
+[Isort-GitHub.io]: https://pycqa.github.io/isort/
+
+[Typecheck:mypy:badge]: https://www.mypy-lang.org/static/mypy_badge.svg
+
+[Typecheck-mypy-lang.org]: https://mypy-lang.org/
+
+[Linting:pylint:badge]: https://img.shields.io/badge/linting-pylint-yellowgreen
+
+[Pylint-GitHub.com]: https://github.com/pylint-dev/pylint
+
+[CodeFactor-badge]: https://www.codefactor.io/repository/github/llyaudet/python-repeatable-iterable/badge/main
+
+[CodeFactor-package-page]: https://www.codefactor.io/repository/github/llyaudet/python-repeatable-iterable/overview/main
+
+[CodeClimateMaintainability-badge]: https://api.codeclimate.com/v1/badges/89044bfd52999e4f07f6/maintainability
+
+[CodeClimateM13y-package-page]: https://codeclimate.com/github/LLyaudet/python-repeatable-iterable/maintainability
+
+[Codacy-badge]: https://app.codacy.com/project/badge/Grade/1c70116c2d714e3889606519937cb11d
+
+[Codacy-package-page]: https://app.codacy.com/gh/LLyaudet/python-repeatable-iterable/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+[GitHub-top-language-badge]: https://img.shields.io/github/languages/top/llyaudet/python-repeatable-iterable
+
+[GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/python-repeatable-iterable
+
+[PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/python-repeatable-iterable
+
+[GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/python-repeatable-iterable
 
-[pypi-version]: https://img.shields.io/pypi/v/python-repeatable-iterable.svg
-[pypi]: https://pypi.org/project/python-repeatable-iterable/
```

