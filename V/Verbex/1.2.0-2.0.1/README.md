# Comparing `tmp/Verbex-1.2.0.tar.gz` & `tmp/verbex-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Verbex-1.2.0.tar", last modified: Sun May 22 15:11:16 2022, max compression
+gzip compressed data, was "verbex-2.0.1.tar", last modified: Sun Apr 28 15:00:43 2024, max compression
```

## Comparing `Verbex-1.2.0.tar` & `verbex-2.0.1.tar`

### file list

```diff
@@ -1,53 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:16.075000 Verbex-1.2.0/
--rw-rw-rw-   0        0        0      956 2021-09-19 03:50:37.000000 Verbex-1.2.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:11.629000 Verbex-1.2.0/.github/
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:13.613000 Verbex-1.2.0/.github/workflows/
--rw-rw-rw-   0        0        0     1392 2022-05-08 16:21:37.000000 Verbex-1.2.0/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      180 2022-05-08 13:37:44.000000 Verbex-1.2.0/.gitignore
--rw-rw-rw-   0        0        0     7987 2022-05-08 21:33:08.000000 Verbex-1.2.0/.pre-commit-config.yaml
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:13.703000 Verbex-1.2.0/.vscode/
--rw-rw-rw-   0        0        0      298 2022-05-08 13:09:31.000000 Verbex-1.2.0/.vscode/settings.json
--rw-rw-rw-   0        0        0      131 2022-04-30 18:08:46.000000 Verbex-1.2.0/.yamllint
--rw-rw-rw-   0        0        0    35149 2022-05-08 13:09:31.000000 Verbex-1.2.0/GPLv3_LICENSE.txt
--rw-rw-rw-   0        0        0     1847 2022-05-08 13:09:32.000000 Verbex-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       84 2022-05-08 17:31:06.000000 Verbex-1.2.0/MANIFEST.IN
--rw-rw-rw-   0        0        0     2703 2022-05-22 15:11:15.995000 Verbex-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1653 2022-05-08 13:09:32.000000 Verbex-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:14.148000 Verbex-1.2.0/Verbex.egg-info/
--rw-rw-rw-   0        0        0     2703 2022-05-22 15:11:09.000000 Verbex-1.2.0/Verbex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-05-22 15:11:11.000000 Verbex-1.2.0/Verbex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-22 15:11:09.000000 Verbex-1.2.0/Verbex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-05-22 15:11:09.000000 Verbex-1.2.0/Verbex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-05-22 15:11:09.000000 Verbex-1.2.0/Verbex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:14.469000 Verbex-1.2.0/archive/
--rw-rw-rw-   0        0        0     3764 2022-05-08 15:53:41.000000 Verbex-1.2.0/archive/archive-20220508115341-c1a945c08ab1170c.tar.gz
--rw-rw-rw-   0        0        0     3767 2022-05-08 15:54:32.000000 Verbex-1.2.0/archive/archive-20220508115432-8f4db45c4efcdff6.tar.gz
--rw-rw-rw-   0        0        0     3766 2022-05-08 15:59:31.000000 Verbex-1.2.0/archive/archive-20220508115930-3a2864bd92a8e920.tar.gz
--rwxrwxrwx   0        0        0       47 2022-05-08 13:44:00.000000 Verbex-1.2.0/builddoc.bat
--rw-rw-rw-   0        0        0     2552 2022-05-08 15:10:59.000000 Verbex-1.2.0/check_names.py
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:14.905000 Verbex-1.2.0/dist/
--rw-rw-rw-   0        0        0    27017 2022-05-08 13:09:32.000000 Verbex-1.2.0/dist/Verbex-1.0.2.win-amd64.zip
--rw-rw-rw-   0        0        0    27010 2022-05-08 17:36:13.000000 Verbex-1.2.0/dist/Verbex-1.0.3.win-amd64.zip
--rw-rw-rw-   0        0        0    27913 2022-05-08 17:34:21.000000 Verbex-1.2.0/dist/Verbex-1.1.0.win-amd64.zip
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:15.117000 Verbex-1.2.0/docs/
--rw-rw-rw-   0        0        0      137 2022-05-08 21:44:13.000000 Verbex-1.2.0/docs/index.html
--rw-rw-rw-   0        0        0    39053 2022-05-08 21:44:13.000000 Verbex-1.2.0/docs/search.js
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:15.282000 Verbex-1.2.0/docs/verbex/
--rw-rw-rw-   0        0        0   389534 2022-05-08 21:44:12.000000 Verbex-1.2.0/docs/verbex/verbex.html
--rw-rw-rw-   0        0        0      802 2022-05-08 16:17:54.000000 Verbex-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       70 2022-05-08 21:18:37.000000 Verbex-1.2.0/requirements.in
--rw-rw-rw-   0        0        0      226 2022-05-08 21:24:10.000000 Verbex-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       41 2022-05-08 21:18:37.000000 Verbex-1.2.0/requirements_dev.in
--rw-rw-rw-   0        0        0     1354 2022-05-08 21:24:13.000000 Verbex-1.2.0/requirements_dev.txt
--rw-rw-rw-   0        0        0       76 2022-05-08 21:19:33.000000 Verbex-1.2.0/requirements_test.txt
--rw-rw-rw-   0        0        0     1010 2022-05-22 15:11:16.072000 Verbex-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       69 2022-05-08 17:19:09.000000 Verbex-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:15.470000 Verbex-1.2.0/tests/
--rw-rw-rw-   0        0        0        0 2022-05-08 14:16:09.000000 Verbex-1.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     9085 2022-05-08 14:16:12.000000 Verbex-1.2.0/tests/test_verbex.py
-drwxrwxrwx   0        0        0        0 2022-05-22 15:11:15.958000 Verbex-1.2.0/verbex/
--rw-rw-rw-   0        0        0    35149 2022-05-08 13:09:31.000000 Verbex-1.2.0/verbex/GPLv3_LICENSE.txt
--rw-rw-rw-   0        0        0     1847 2022-05-08 13:09:32.000000 Verbex-1.2.0/verbex/LICENSE.TXT
--rw-rw-rw-   0        0        0      288 2022-05-08 21:44:09.000000 Verbex-1.2.0/verbex/__init__.py
--rw-rw-rw-   0        0        0        0 2022-05-08 13:09:33.000000 Verbex-1.2.0/verbex/py.typed
--rw-rw-rw-   0        0        0    16438 2022-05-08 21:31:53.000000 Verbex-1.2.0/verbex/verbex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:00:43.332792 verbex-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    36385 2024-04-28 15:00:39.000000 verbex-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-28 15:00:43.332792 verbex-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-28 15:00:39.000000 verbex-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-28 15:00:39.000000 verbex-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:00:43.332792 verbex-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:00:43.324792 verbex-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:00:43.328791 verbex-2.0.1/src/verbex/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-28 15:00:39.000000 verbex-2.0.1/src/verbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:00:39.000000 verbex-2.0.1/src/verbex/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-28 15:00:39.000000 verbex-2.0.1/src/verbex/verbex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:00:43.328791 verbex-2.0.1/src/verbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-28 15:00:43.000000 verbex-2.0.1/src/verbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-28 15:00:43.000000 verbex-2.0.1/src/verbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:00:43.000000 verbex-2.0.1/src/verbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-28 15:00:43.000000 verbex-2.0.1/src/verbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 15:00:43.000000 verbex-2.0.1/src/verbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:00:43.328791 verbex-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-28 15:00:39.000000 verbex-2.0.1/tests/test_verbex.py
```

### Comparing `Verbex-1.2.0/GPLv3_LICENSE.txt` & `verbex-2.0.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+Verbal Expressions
+Copyright (C) 2022 Richard Broderick
+
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
@@ -668,7 +671,32 @@
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
+
+
+ This file incorporates work covered by the following copyright and
+ permission notice:
+
+	The MIT License (MIT)
+
+	Copyright (c) 2017 jehna
+
+	Permission is hereby granted, free of charge, to any person obtaining a copy of
+	this software and associated documentation files (the "Software"), to deal in
+	the Software without restriction, including without limitation the rights to
+	use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+	the Software, and to permit persons to whom the Software is furnished to do so,
+	subject to the following conditions:
+
+	The above copyright notice and this permission notice shall be included in all
+	copies or substantial portions of the Software.
+
+	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+	FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+	COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+	IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+	CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `Verbex-1.2.0/README.md` & `verbex-2.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Verbex: Python verbal based regular expressions
 ================================================
 
-![Build Status](https://github.com/rbroderi/Verbex/actions/workflows/main.yml/badge.svg?event=push)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+<!-- ![Build Status](https://github.com/rbroderi/Verbex/actions/workflows/main.yml/badge.svg?event=push) -->
+[![Code style: black](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![PyPI license](https://img.shields.io/pypi/l/verbex)](https://www.gnu.org/licenses/gpl-3.0.en.html)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/verbex)](https://pypi.python.org/pypi/ansicolortags/)
+[![Generic badge](https://img.shields.io/badge/mypy-typed-purple.svg)](http://mypy-lang.org/)
+[![Generic badge](https://img.shields.io/badge/beartype-runtime_typed-cyan.svg)](https://github.com/beartype/beartype)
+[![Generic badge](https://img.shields.io/badge/bandit-checked-magenta.svg)](https://bandit.readthedocs.io/en/latest/)
+[![Generic badge](https://img.shields.io/badge/uv-requirements-yellow.svg)](https://shields.io/)
+![Dynamic TOML Badge](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Frbroderi%2FVerbex%2Fmaster%2Fpyproject.toml&query=%24.project.version&label=Version)
+
 
 ## Installation
 ```bash
 pip install Verbex
 ```
 ## Usage
 ```python
```

### Comparing `Verbex-1.2.0/tests/test_verbex.py` & `verbex-2.0.1/tests/test_verbex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pyright: reportPrivateUsage=false
 # flake8: noqa
 # type: ignore
+# pylint: disable-all
 import re
 import unittest
 
 from verbex import CharClass, SpecialChar, Verbex
 
 
 class verbexTest(unittest.TestCase):
@@ -15,18 +16,18 @@
 
     # def tearDown(self):
     #     ...
     #     # Verbex() = None
     #     # self.exp = None
 
     def test_should_render_verbex_as_string(self):
-        self.assertEqual(str(Verbex()._add("^$")), "^$")  # noqa
+        self.assertEqual(str(Verbex()._add("^$")), "^$")
 
     def test_should_render_verbex_list_as_string(self):
-        self.assertEqual(str(Verbex()._add(["^", "[0-9]", "$"])), "^[0-9]$")  # noqa
+        self.assertEqual(str(Verbex()._add(["^", "[0-9]", "$"])), "^[0-9]$")
 
     def test_should_match_characters_in_range(self):
         regex = Verbex().letter_range("a", "c").regex()
         for character in ["a", "b", "c"]:
             self.assertRegex(character, regex)
 
     def test_should_not_match_characters_outside_of_range(self):
@@ -41,22 +42,22 @@
         regex = Verbex().find("test").find(SpecialChar.END_OF_LINE).regex()
         self.assertRegex("IGNORE   test", regex)
 
     def test_should_match_anything(self):
         regex = Verbex().anything().regex()
         self.assertIsNotNone(re.fullmatch(regex, "!@#$%¨&*()__+{}"))
 
-    def test_should_match_anything_but_specified_element_when_element_is_not_found(  # noqa: E501
+    def test_should_match_anything_but_specified_element_when_element_is_not_found(
         self,
     ):
         regex = Verbex().anything_but("X").find(" Files").regex()
         self.assertRegex("Y Files", regex)
         self.assertNotRegex("X Files", regex)
 
-    def test_should_not_match_anything_but_specified_element_when_specified_element_is_found(  # noqa: E501
+    def test_should_not_match_anything_but_specified_element_when_specified_element_is_found(
         self,
     ):
         regex = Verbex().anything_but("X").regex()
         self.assertRegex("Y Files", regex)
         self.assertNotRegex("X", regex)
 
     def test_should_find_element(self):
```

