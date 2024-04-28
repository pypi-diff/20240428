# Comparing `tmp/python_none_objects-1.1.5.tar.gz` & `tmp/python_none_objects-1.1.6.tar.gz`

## Comparing `python_none_objects-1.1.5.tar` & `python_none_objects-1.1.6.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/src/python_none_objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/src/python_none_objects/py.typed
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/typing_test/__init__.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/COPYING.LESSER
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/README.md
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/pyproject.toml
--rw-r--r--   0        0        0    13849 2020-02-02 00:00:00.000000 python_none_objects-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/README_printable.md
+-rwxr-xr-x   0        0        0     1664 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/build_and_checks.sh
+-rwxr-xr-x   0        0        0      993 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/build_readme.sh
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/src/python_none_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/src/python_none_objects/py.typed
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/typing_test/__init__.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/COPYING.LESSER
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/README.md
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0    14616 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/PKG-INFO
```

### Comparing `python_none_objects-1.1.5/src/python_none_objects/__init__.py` & `python_none_objects-1.1.6/src/python_none_objects/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """
 This file is part of python-none-objects library.
 
-python-none-objects is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
+python-none-objects is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
 
-python-none-objects is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
+python-none-objects is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with python-none-objects.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
---------------------------------------------------------------------------
+----------------------------------------------------------------------
 The empty tuple is really useful.
 But it is implementation dependent for it to be a constant:
-https://docs.python.org/3.12/reference/expressions.html#parenthesized-forms
-https://stackoverflow.com/questions/41983180/is-the-empty-tuple-in-python-a-constant
-https://stackoverflow.com/questions/8185776/compare-object-to-empty-tuple-with-the-is-operator-in-python-2-x
-https://stackoverflow.com/questions/38328857/why-does-is-return-true-when-is-and-is-return-false
-https://stackoverflow.com/questions/14135542/how-is-tuple-implemented-in-cpython
+https://docs.python.org/3.12/reference/expressions.html
+#parenthesized-forms
+https://stackoverflow.com/questions/41983180
+/is-the-empty-tuple-in-python-a-constant
+https://stackoverflow.com/questions/8185776
+/compare-object-to-empty-tuple-with-the-is-operator-in-python-2-x
+https://stackoverflow.com/questions/38328857
+/why-does-is-return-true-when-is-and-is-return-false
+https://stackoverflow.com/questions/14135542
+/how-is-tuple-implemented-in-cpython
 I'm wondering if there would be additional efficiency gains
 to treat the empty tuple and the constants here differently
 at execution of Python scripts.
 """
 
 from types import MappingProxyType
 from typing import (
```

### Comparing `python_none_objects-1.1.5/typing_test/__init__.py` & `python_none_objects-1.1.6/typing_test/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 This file is part of python-none-objects library.
 
-python-none-objects is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-python-none-objects is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
+python-none-objects is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+python-none-objects is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with python-none-objects.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
 """
 
 import sys
@@ -31,38 +36,42 @@
 )
 
 
 def foo_collection(x: Collection[str] = NoneCollection) -> bool:
     """
     Check typing for NoneCollection.
     """
+
     for y in x:
         print(f"foo {y}")
     return "toto" in x
 
 
 def foo_iterable(x: Iterable[str] = NoneIterable) -> None:
     """
     Check typing for NoneIterable.
     """
+
     for y in x:
         print(f"foo {y}")
 
 
 def foo_container(x: Container[str] = NoneContainer) -> bool:
     """
     Check typing for NoneContainer.
     """
+
     return "toto" in x
 
 
 def foo_mapping(x: Mapping[str, str] = NoneMapping) -> None:
     """
     Check typing for NoneMapping.
     """
+
     for y, z in x.items():
         print(f"foo {y} bar {z}")
 
 
 foo_collection()
 foo_iterable()
 foo_container()
```

### Comparing `python_none_objects-1.1.5/COPYING` & `python_none_objects-1.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.5/COPYING.LESSER` & `python_none_objects-1.1.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.5/pyproject.toml` & `python_none_objects-1.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-none-objects"
-version = "1.1.5"
-description = "Add more constant \"None\" objects to Python to avoid boilerplate code"
+version = "1.1.6"
+description = """\
+Add more constant \"None\" objects to Python \
+to avoid boilerplate code\
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
 keywords = ["Python", "None", "Immutable", "Default values"]
 dependencies = [
 ]
@@ -30,15 +36,17 @@
     "isort",
     "mypy",
     "pylint",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/LLyaudet/python-none-objects"
-"Bug Tracker" = "https://github.com/LLyaudet/python-none-objects/issues"
+"Bug Tracker" = """\
+https://github.com/LLyaudet/python-none-objects/issues\
+"""
 
 [tool.black]
 line-length = 70
 
 [tool.isort]
 profile = "black"
 line_length = 70
```

### Comparing `python_none_objects-1.1.5/PKG-INFO` & `python_none_objects-1.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-none-objects
-Version: 1.1.5
+Version: 1.1.6
 Summary: Add more constant "None" objects to Python to avoid boilerplate code
 Project-URL: Homepage, https://github.com/LLyaudet/python-none-objects
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-none-objects/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -183,89 +183,151 @@
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # python-none-objects
 
-[![pypi-version]][pypi]
-[![Downloads](https://img.shields.io/pypi/dm/python-none-objects)](https://pypistats.org/packages/python-none-objects)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![CodeFactor](https://www.codefactor.io/repository/github/llyaudet/python-none-objects/badge)](https://www.codefactor.io/repository/github/llyaudet/python-none-objects)
-[![CodeClimateMaintainability](https://api.codeclimate.com/v1/badges/266efb337cabd7d7941e/maintainability)](https://codeclimate.com/github/LLyaudet/python-none-objects/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/4be488463e31459bb2ba02794091610d)](https://app.codacy.com/gh/LLyaudet/python-none-objects/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-![GitHub top language](https://img.shields.io/github/languages/top/llyaudet/python-none-objects)
-![GitHub License](https://img.shields.io/github/license/llyaudet/python-none-objects)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-none-objects)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/llyaudet/python-none-objects)
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
+|    **A collection of "None" objects**    |
+|:----------------------------------------:|
+| **compatible with various Python types** |
 
-|     **A collection of "None" objects compatible with various Python types**     |
 
-The following code yields warning for "Default argument value is mutable".
+The following code yields warning
+for "Default argument value is mutable".
 
 ```python3
 from typing import List, Dict
 
 def foo(some: int, other: List = [], thing: Dict = {}):
     for o in other:
         bar(some, o, thing)
 ```
 
 It is usually recommended to use None instead
-(<https://stackoverflow.com/questions/41686829/why-does-pycharm-warn-about-mutable-default-arguments-how-can-i-work-around-the>):
+(<https://stackoverflow.com/questions/41686829>
+/why-does-pycharm-warn-about-mutable-default-arguments-
+how-can-i-work-around-the):
 
 ```python3
 from typing import List, Dict, Optional
 
-def foo(some: int, other: Optional[List] = None, thing: Optional[Dict] = None):
+def foo(
+    some: int,
+    other: Optional[List] = None,
+    thing: Optional[Dict] = None,
+):
     if other is None:
         other = []
     if thing is None:
         thing = {}
     for o in other:
         bar(some, o, thing)
 ```
 
 But I prefer less boilerplate code like this:
 
 ```python3
 from typing import Iterable, Mapping
 from types import MappingProxyType
 
-def foo(some: int, other: Iterable = (), thing: Mapping = MappingProxyType({})):
+def foo(
+    some: int,
+    other: Iterable = (),
+    thing: Mapping = MappingProxyType({}),
+):
     for o in other:
         bar(some, o, thing)
 ```
 
 This package introduces constants to make the code more readable:
 
 ```python3
 from typing import Iterable, Mapping
 from python_none_objects import NoneIterable, NoneMapping
 
-def foo(some: int, other: Iterable = NoneIterable, thing: Mapping = NoneMapping):
+def foo(
+    some: int,
+    other: Iterable = NoneIterable,
+    thing: Mapping = NoneMapping,
+):
     for o in other:
         bar(some, o, thing)
 ```
 
 Be sure to look at the discussions on GitHub:
 <https://github.com/LLyaudet/python-none-objects/discussions>.
 
 There is a poll on the naming convention you would prefer:
 <https://github.com/LLyaudet/python-none-objects/discussions/2>.
 
-And there is a discussion on various ideas to optimize the code with these constants:
+And there is a discussion on various ideas
+to optimize the code with these constants:
 <https://github.com/LLyaudet/python-none-objects/discussions/3>.
 
-I think it would be better to have this kind of constants in the standard library.
+I think it would be better to have this kind of constants
+in the standard library.
 If you think after reading everything, that it is indeed a good idea,
-add a star to this repository to let the rest of the Python community know
-that you would like to see such constant objects in the language :).
+add a star to this repository to let the rest
+of the Python community
+know that you would like to see such constant objects
+in the language :).
 <https://github.com/LLyaudet/python-none-objects/>
 If the project gains popularity, I'll try to propose it officially.
 
-[pypi-version]: https://img.shields.io/pypi/v/python-none-objects.svg
-[pypi]: https://pypi.org/project/python-none-objects/
+[PyPI-version-badge]: https://img.shields.io/pypi/v/python-none-objects.svg
+
+[PyPI-package-page]: https://pypi.org/project/python-none-objects/
+
+[Downloads-badge]: https://img.shields.io/pypi/dm/python-none-objects
+
+[PyPIStats-package-page]: https://pypistats.org/packages/python-none-objects
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
+[CodeFactor-badge]: https://www.codefactor.io/repository/github/llyaudet/python-none-objects/badge
+
+[CodeFactor-package-page]: https://www.codefactor.io/repository/github/llyaudet/python-none-objects
+
+[CodeClimateMaintainability-badge]: https://api.codeclimate.com/v1/badges/266efb337cabd7d7941e/maintainability
+
+[CodeClimateM13y-package-page]: https://codeclimate.com/github/LLyaudet/python-none-objects/maintainability
+
+[Codacy-badge]: https://app.codacy.com/project/badge/Grade/4be488463e31459bb2ba02794091610d
+
+[Codacy-package-page]: https://app.codacy.com/gh/LLyaudet/python-none-objects/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+[GitHub-top-language-badge]: https://img.shields.io/github/languages/top/llyaudet/python-none-objects
+
+[GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/python-none-objects
+
+[PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/python-none-objects
+
+[GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/python-none-objects
```

