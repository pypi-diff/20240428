# Comparing `tmp/protokolo-2.0.1.tar.gz` & `tmp/protokolo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-2.0.1.tar", max compression
+gzip compressed data, was "protokolo-2.1.0.tar", max compression
```

## Comparing `protokolo-2.0.1.tar` & `protokolo-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     3204 2024-04-10 13:47:24.824216 protokolo-2.0.1/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-2.0.1/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-2.0.1/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-2.0.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-2.0.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     6947 2024-04-10 09:40:37.511016 protokolo-2.0.1/README.md
--rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-2.0.1/docs/Makefile
--rw-r--r--   0        0        0     2052 2024-04-10 09:40:37.511016 protokolo-2.0.1/docs/conf.py
--rw-r--r--   0        0        0      744 2024-04-10 09:40:37.511016 protokolo-2.0.1/docs/index.rst
--rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-2.0.1/docs/make.bat
--rw-r--r--   0        0        0      271 2024-04-10 09:40:37.511016 protokolo-2.0.1/docs/man/index.rst
--rw-r--r--   0        0        0     1638 2024-04-10 09:40:37.511016 protokolo-2.0.1/docs/man/protokolo-compile.rst
--rw-r--r--   0        0        0     2078 2024-04-10 09:40:37.511016 protokolo-2.0.1/docs/man/protokolo-init.rst
--rw-r--r--   0        0        0     1033 2024-04-10 10:39:43.816552 protokolo-2.0.1/docs/man/protokolo.rst
--rw-r--r--   0        0        0     7976 2024-04-10 09:40:37.511016 protokolo-2.0.1/docs/reference.md
--rw-r--r--   0        0        0     2811 2024-04-10 13:47:15.764107 protokolo-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      177 2024-04-10 13:47:15.768107 protokolo-2.0.1/src/protokolo/__init__.py
--rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-2.0.1/src/protokolo/__main__.py
--rw-r--r--   0        0        0     3825 2024-04-09 10:25:50.336818 protokolo-2.0.1/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     1424 2024-04-10 09:50:35.343820 protokolo-2.0.1/src/protokolo/_util.py
--rw-r--r--   0        0        0     9546 2024-04-10 13:42:48.268709 protokolo-2.0.1/src/protokolo/cli.py
--rw-r--r--   0        0        0    10167 2024-04-10 10:07:37.305507 protokolo-2.0.1/src/protokolo/compile.py
--rw-r--r--   0        0        0    11739 2024-04-10 13:38:09.164719 protokolo-2.0.1/src/protokolo/config.py
--rw-r--r--   0        0        0     3245 2024-04-09 10:25:50.336818 protokolo-2.0.1/src/protokolo/exceptions.py
--rw-r--r--   0        0        0     3785 2024-04-10 09:40:37.511016 protokolo-2.0.1/src/protokolo/initialise.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-2.0.1/src/protokolo/py.typed
--rw-r--r--   0        0        0     1520 2024-04-09 10:25:50.336818 protokolo-2.0.1/src/protokolo/replace.py
--rw-r--r--   0        0        0      903 2024-04-10 11:17:10.318020 protokolo-2.0.1/src/protokolo/types.py
--rw-r--r--   0        0        0     2225 2024-04-10 09:40:37.511016 protokolo-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0    20512 2024-04-10 10:52:13.491696 protokolo-2.0.1/tests/test_cli.py
--rw-r--r--   0        0        0    15759 2024-04-10 10:07:37.305507 protokolo-2.0.1/tests/test_compile.py
--rw-r--r--   0        0        0    11440 2024-04-10 09:40:37.515016 protokolo-2.0.1/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-2.0.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     6053 2024-04-10 09:24:45.458848 protokolo-2.0.1/tests/test_formatter.py
--rw-r--r--   0        0        0     3907 2024-04-10 09:40:37.515016 protokolo-2.0.1/tests/test_replace.py
--rw-r--r--   0        0        0     8021 1970-01-01 00:00:00.000000 protokolo-2.0.1/setup.py
--rw-r--r--   0        0        0     7917 1970-01-01 00:00:00.000000 protokolo-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3204 2024-04-27 21:40:40.247205 protokolo-2.1.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-2.1.0/LICENSES/
+-rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-2.1.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-2.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-2.1.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     7095 2024-04-27 21:40:40.247205 protokolo-2.1.0/README.md
+-rw-r--r--   0        0        0     2233 2024-04-27 21:40:40.251205 protokolo-2.1.0/_build.py
+-rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-2.1.0/docs/Makefile
+-rw-r--r--   0        0        0     2535 2024-04-27 21:49:12.549421 protokolo-2.1.0/docs/conf.py
+-rw-r--r--   0        0        0      744 2024-04-27 21:40:40.251205 protokolo-2.1.0/docs/index.rst
+-rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-2.1.0/docs/make.bat
+-rw-r--r--   0        0        0      271 2024-04-27 21:40:40.251205 protokolo-2.1.0/docs/man/index.rst
+-rw-r--r--   0        0        0     1638 2024-04-27 21:40:40.251205 protokolo-2.1.0/docs/man/protokolo-compile.rst
+-rw-r--r--   0        0        0     2078 2024-04-27 21:40:40.251205 protokolo-2.1.0/docs/man/protokolo-init.rst
+-rw-r--r--   0        0        0     1036 2024-04-27 21:40:40.251205 protokolo-2.1.0/docs/man/protokolo.rst
+-rw-r--r--   0        0        0     7976 2024-04-27 21:40:40.251205 protokolo-2.1.0/docs/reference.md
+-rw-r--r--   0        0        0     2944 2024-04-27 21:40:40.255205 protokolo-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     4030 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1424 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/_util.py
+-rw-r--r--   0        0        0    10749 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/cli.py
+-rw-r--r--   0        0        0    10420 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/compile.py
+-rw-r--r--   0        0        0    12133 2024-04-27 21:40:40.255205 protokolo-2.1.0/src/protokolo/config.py
+-rw-r--r--   0        0        0     3619 2024-04-27 21:40:40.259205 protokolo-2.1.0/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     1099 2024-04-27 21:40:40.259205 protokolo-2.1.0/src/protokolo/i18n.py
+-rw-r--r--   0        0        0     3785 2024-04-27 21:40:40.259205 protokolo-2.1.0/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-2.1.0/src/protokolo/py.typed
+-rw-r--r--   0        0        0     1520 2024-04-27 21:40:40.259205 protokolo-2.1.0/src/protokolo/replace.py
+-rw-r--r--   0        0        0      903 2024-04-27 21:40:40.259205 protokolo-2.1.0/src/protokolo/types.py
+-rw-r--r--   0        0        0     2263 2024-04-27 21:40:40.259205 protokolo-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0    20548 2024-04-27 21:40:40.259205 protokolo-2.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0    15759 2024-04-27 21:40:40.259205 protokolo-2.1.0/tests/test_compile.py
+-rw-r--r--   0        0        0    11400 2024-04-27 21:40:40.259205 protokolo-2.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-2.1.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6053 2024-04-27 21:40:40.259205 protokolo-2.1.0/tests/test_formatter.py
+-rw-r--r--   0        0        0     3907 2024-04-27 21:40:40.259205 protokolo-2.1.0/tests/test_replace.py
+-rw-r--r--   0        0        0     8065 1970-01-01 00:00:00.000000 protokolo-2.1.0/PKG-INFO
```

### Comparing `protokolo-2.0.1/CHANGELOG.md` & `protokolo-2.1.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-2.1.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/LICENSES/CC0-1.0.txt` & `protokolo-2.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/LICENSES/GPL-3.0-or-later.txt` & `protokolo-2.1.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/README.md` & `protokolo-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # Protokolo
 
 [![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
 [![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
+[![Translation status](https://hosted.weblate.org/widget/protokolo/protokolo/svg-badge.svg)](https://hosted.weblate.org/engage/protokolo/)
 
 Protokolo is a change log generator.
 
 Protokolo allows you to maintain your change log fragments in separate files,
 and then finally aggregate them into a new section in CHANGELOG just before
 release.
 
@@ -27,24 +28,21 @@
 - [Licensing](#licensing)
 
 ## Background
 
 Change logs are [a really good idea](https://keepachangelog.com/).
 Unfortunately, they are also a bit of a pain when combined with version control:
 
-- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll
-  need to resolve a conflict when trying to merge them both.
-- Just after you make a release, you need to create a new section in CHANGELOG
-  for your next release. If you forget this busywork, new feature branches will
-  need to create this section, which increases the chance of merge conflicts.
-- If a feature branch adds a change log entry to the section for the next v2.0
-  release, and v2.0 subsequently releases without merging that feature branch,
-  then merging that feature branch afterwards would still add the change log
-  entry to the v2.0 section, even though it should now go to the unreleased v3.0
-  section.
+- Different merge requests all edit the same area in CHANGELOG, inevitably
+  resulting in merge conflicts.
+- If a section for an unreleased version does not yet exist in the main branch's
+  CHANGELOG (typically shortly after release), feature branches must create this
+  section. If multiple feature branches do this, you get more merge conflicts.
+- Old merge requests, when merged, sometimes add their change log entry to the
+  section of a release that is already published.
 
 Life would be a lot easier if you didn't have to deal with these problems.
 
 Enter Protokolo
 ([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The
 idea is very simple: for every change log entry, create a new file. Finally,
 just before release, compile the contents of those files into a new section in
@@ -72,17 +70,18 @@
   fragment.
 
 A much younger version of me also tried her hand at writing a program like this
 in [changelogdir](https://pypi.org/project/changelogdir/).
 
 ## Install
 
-Protokolo is a regular Python package. You can install it using
-`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`
-with `pipx ensurepath`.
+Protokolo is a regular Python package
+[hosted on PyPI](https://pypi.python.org/pypi/protokolo). You can install it
+using `pipx install protokolo`. Make sure that `~/.local/share/bin` is in your
+`$PATH` with `pipx ensurepath`.
 
 ## Usage
 
 For full documentation and options, read the documentation at
 <https://protokolo.readthedocs.io>.
 
 ### Initial set-up
@@ -170,14 +169,18 @@
 ## Contributing
 
 The code and issue tracker is hosted at
 <https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any
 issues. For pull requests, bug fixes are always welcome, but new features should
 probably be discussed in any issue first.
 
+Translations are done at
+<https://hosted.weblate.org/projects/protokolo/protokolo/> using Weblate. If
+there are issues with translation, feel free to open an issue at Codeberg.
+
 ## Licensing
 
 All code is licensed under GPL-3.0-or-later.
 
 All documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.
 
 Some configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.
```

### Comparing `protokolo-2.0.1/docs/Makefile` & `protokolo-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/docs/index.rst` & `protokolo-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/docs/make.bat` & `protokolo-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/docs/man/protokolo-compile.rst` & `protokolo-2.1.0/docs/man/protokolo-compile.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/docs/man/protokolo-init.rst` & `protokolo-2.1.0/docs/man/protokolo-init.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/docs/man/protokolo.rst` & `protokolo-2.1.0/docs/man/protokolo.rst`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 :program:`protokolo` allows you to maintain your change log fragments in
 separate files, and then finally aggregate them into a new section in CHANGELOG
 just before release.
 
 For more information on how to use Protokolo beyond a reference of the
 command-line options, see the accompanying documentation or read it at
-<https://protokolo.readthedocs.io>.
+`<https://protokolo.readthedocs.io>`_.
 
 Options
 -------
 
 .. option:: --help
 
     Display help and exit. If no command is provided, this option is implied.
```

### Comparing `protokolo-2.0.1/docs/reference.md` & `protokolo-2.1.0/docs/reference.md`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/pyproject.toml` & `protokolo-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "2.0.1"
+version = "2.1.0"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
@@ -25,14 +25,15 @@
     "Topic :: Utilities"
 ]
 
 packages = [
     { include = "protokolo", from = "src" }
 ]
 include = [
+    { path = "src/protokolo/locale/**/*.mo", format="wheel" },
     { path = "docs", format = "sdist" },
     { path = "tests", format = "sdist" },
     { path = "README.md", format = "sdist" },
     { path = "CHANGELOG.md", format = "sdist" },
     { path = "LICENSES", format = "sdist" },
 ]
 
@@ -72,20 +73,24 @@
 
 [tool.poetry.group.lsp.dependencies]
 python-lsp-server = "*"
 pylsp-mypy = "*"
 pyls-isort = "*"
 python-lsp-black = "*"
 
+[tool.poetry.build]
+generate-setup-file = false
+script = "_build.py"
+
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [bumpver]
-current_version = "v2.0.1"
+current_version = "v2.1.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `protokolo-2.0.1/src/protokolo/_formatter.py` & `protokolo-2.1.0/src/protokolo/_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from datetime import date
 from inspect import cleandoc
 from string import Template
 from typing import cast
 
 from .config import SectionAttributes
 from .exceptions import HeadingFormatError
+from .i18n import _
 
 # pylint: disable=too-few-public-methods
 
 
 class MarkupFormatter(ABC):
     """A simple formatter class."""
 
@@ -29,32 +30,34 @@
         You can use ``$key`` (or ``${key}``) placeholders in the title to
         replace them with the values of the corresponding keys in *attrs*.
         ``$date`` is special in that it is replaced with today's date. ``$$`` is
         replaced by a single ``$``.
 
         Raises:
             HeadingFormatError: could not format the heading as given.
-
         """
         cls._validate(attrs)
         title = cls._format_output(attrs)
         return cls._format_section(title, attrs)
 
     @classmethod
     def _validate(cls, attrs: SectionAttributes) -> None:
         """
         Raises:
             HeadingFormatError: could not format the heading as given.
         """
         # This is technically invalid. Valid attrs do not have a non-positive
         # level.
         if attrs.level <= 0:
-            raise HeadingFormatError(f"Level {attrs.level} must be positive.")
+            raise HeadingFormatError(
+                # TRANSLATORS: level refers to the depth of a heading.
+                _("Level {level} must be positive.").format(level=attrs.level)
+            )
         if not attrs.title:
-            raise HeadingFormatError("title cannot be empty.")
+            raise HeadingFormatError(_("Title cannot be empty."))
 
     @classmethod
     @abstractmethod
     def _format_section(cls, title: str, attrs: SectionAttributes) -> str: ...
 
     @classmethod
     def _format_output(cls, attrs: SectionAttributes) -> str:
@@ -97,15 +100,17 @@
     }
 
     @classmethod
     def _validate(cls, attrs: SectionAttributes) -> None:
         super()._validate(attrs)
         if attrs.level > len(cls._levels):
             raise HeadingFormatError(
-                f"Heading level {attrs.level} is too deep."
+                _("Heading level {level} is too deep.").format(
+                    level=attrs.level
+                )
             )
 
     @classmethod
     def _format_section(cls, title: str, attrs: SectionAttributes) -> str:
         sign = cls._levels[attrs.level]
         length = len(title)
         return cleandoc(
```

### Comparing `protokolo-2.0.1/src/protokolo/_util.py` & `protokolo-2.1.0/src/protokolo/_util.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/src/protokolo/cli.py` & `protokolo-2.1.0/src/protokolo/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Main entry of program."""
 
+import gettext
+import os
 import tomllib
 from inspect import cleandoc
 from io import TextIOWrapper
 from pathlib import Path
 
 import click
 from click.formatting import wrap_text
@@ -18,61 +20,75 @@
 from .exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
     HeadingFormatError,
     ProtokoloTOMLIsADirectoryError,
     ProtokoloTOMLNotFoundError,
 )
+from .i18n import _
 from .initialise import (
     create_changelog,
     create_keep_a_changelog,
     create_root_toml,
 )
 from .replace import find_first_occurrence, insert_into_str
 from .types import SupportedMarkup
 
+# pylint: disable=missing-function-docstring
 
-@click.group(name="protokolo")
+_PACKAGE_PATH = os.path.dirname(__file__)
+_LOCALE_DIR = os.path.join(_PACKAGE_PATH, "locale")
+if gettext.find("protokolo", localedir=_LOCALE_DIR):
+    gettext.bindtextdomain("protokolo", _LOCALE_DIR)
+    # This is needed to make Click recognise our translations. Our own
+    # translations use the class-based API.
+    gettext.textdomain("protokolo")
+
+
+_VERSION_TEXT = (
+    _("%(prog)s, version %(version)s")
+    + "\n\n"
+    + _(
+        "This program is free software: you can redistribute it and/or modify"
+        " it under the terms of the GNU General Public License as published by"
+        " the Free Software Foundation, either version 3 of the License, or"
+        " (at your option) any later version."
+    )
+    + _(
+        "This program is distributed in the hope that it will be useful,"
+        " but WITHOUT ANY WARRANTY; without even the implied warranty of"
+        " MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the"
+        " GNU General Public License for more details."
+    )
+    + "\n\n"
+    + _(
+        "You should have received a copy of the GNU General Public License"
+        " along with this program. If not, see"
+        " <https://www.gnu.org/licenses/>."
+    )
+    + "\n\n"
+    + _("Written by Carmen Bianca BAKKER.")
+)
+
+_MAIN_HELP = _("Protokolo is a change log generator.")
+
+
+@click.group(name="protokolo", help=_MAIN_HELP)
 @click.version_option(
     package_name="protokolo",
-    message=wrap_text(
-        cleandoc(
-            """
-            %(prog)s, version %(version)s
-
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-            GNU General Public License for more details.
-
-            You should have received a copy of the GNU General Public License
-            along with this program. If not, see
-            <https://www.gnu.org/licenses/>.
-
-            Written by Carmen Bianca BAKKER.
-        """
-        ),
-        preserve_paragraphs=True,
-    ),
+    message=wrap_text(_VERSION_TEXT, preserve_paragraphs=True),
 )
 @click.pass_context
 def main(ctx: click.Context) -> None:
-    """Protokolo is a change log generator."""
     ctx.ensure_object(dict)
     if ctx.default_map is None:
         ctx.default_map = {}
 
     # Only load the global config if the subcommand needs it.
     if ctx.invoked_subcommand in ["compile", "init"]:
-        # TODO: Make directory to search configurable.
         cwd = Path.cwd()
         config_path = GlobalConfig.find_config(Path.cwd())
         if config_path:
             config_path = config_path.relative_to(cwd)
             try:
                 config = GlobalConfig.from_file(config_path)
             except (tomllib.TOMLDecodeError, DictTypeError, OSError) as error:
@@ -86,95 +102,115 @@
             ctx.default_map["init"] = {
                 "changelog": config.changelog,
                 "markup": config.markup,
                 "directory": config.directory,
             }
 
 
-@main.command(name="compile")
+_COMPILE_HELP = (
+    _(
+        "Aggregate all change log fragments into a change log file. The"
+        " fragments are gathered from a change log directory, and subsequently"
+        " deleted."
+    )
+    + "\n\n"
+    + _(
+        "A change log directory should contain a '.protokolo.toml' file that"
+        " defines some attributes of the section. This is an example file:"
+    )
+    + "\n\n"
+    + cleandoc(
+        """
+        \b
+        [protokolo.section]
+        title = "${version} - ${date}"
+        level = 2
+        """
+    )
+    + "\n\n"
+    + _("When the section is compiled, it looks a little like this:")
+    + "\n\n"
+    + "## 1.0.0 - 2023-11-08"
+    + "\n\n"
+    + _(
+        "The heading is followed by the contents of files in the section's"
+        " directory. If a section is empty (no change log fragments), it is not"
+        " compiled."
+    )
+    + "\n\n"
+    + cleandoc(
+        """
+        \b
+        <!-- protokolo-section-tag -->
+        """
+    )
+    + "\n\n"
+    + _(
+        "For more documentation and options, read the documentation at"
+        " <https://protokolo.readthedocs.io>."
+    )
+)
+
+
+@main.command(name="compile", help=_COMPILE_HELP)
 @click.option(
     "--changelog",
     "-c",
-    show_default="determined by config",
+    show_default=_("determined by config"),
     type=click.File("r+", encoding="utf-8", lazy=True),
     required=True,
-    help="File into which to compile.",
+    help=_("File into which to compile."),
 )
 @click.option(
     "--directory",
     "-d",
-    show_default="determined by config",
+    show_default=_("determined by config"),
     type=click.Path(
         exists=True,
         file_okay=False,
         dir_okay=True,
         readable=True,
         path_type=Path,
     ),
     required=True,
-    help="Change log directory to compile.",
+    help=_("Change log directory to compile."),
 )
 @click.option(
     "--markup",
     "-m",
     default="markdown",
-    show_default="determined by config, or markdown",
+    # TRANSLATORS: do not translate markdown.
+    show_default=_("determined by config, or markdown"),
     type=click.Choice(SupportedMarkup.__args__),  # type: ignore
-    help="Markup language.",
+    help=_("Markup language."),
 )
 @click.option(
     "--format",
     "-f",
     "format_",
     type=(str, str),
     metavar="<KEY VALUE>...",
     multiple=True,
-    help="Use key-value pairs to string-format section headings.",
+    # TRANSLATORS: string-format is a verb.
+    help=_("Use key-value pairs to string-format section headings."),
 )
 @click.option(
     "--dry-run",
     "-n",
     is_flag=True,
-    help="Do not write to file system; print result to STDOUT.",
+    # TRANSLATORS: do not translate STDOUT.
+    help=_("Do not write to file system; print result to STDOUT."),
 )
 def compile_(
     changelog: click.File,
     directory: Path,
     markup: SupportedMarkup,
     format_: tuple[tuple[str, str], ...],
     dry_run: bool,
 ) -> None:
-    """Aggregate all change log fragments into a change log file. The fragments
-    are gathered from a change log directory, and subsequently deleted.
-
-    A change log directory should contain a '.protokolo.toml' file that defines
-    some attributes of the section. This is an example file:
-
-    \b
-    [protokolo.section]
-    title = "${version} - ${date}"
-    level = 2
-
-    When the section is compiled, it looks a little like this:
-
-    ## 1.0.0 - 2023-11-08
-
-    The heading is followed by the contents of files in the section's directory.
-    If a section is empty (no change log fragments), it is not compiled.
-
-    The change log file should contain the following comment, which is the
-    location in the file after which the compiled section will be pasted:
-
-    \b
-    <!-- protokolo-section-tag -->
-
-    For more documentation and options, read the documentation at
-    <https://protokolo.readthedocs.io>.
-    """
-    # TODO: Maybe split this up.
     format_pairs: dict[str, str] = dict(format_)
 
     # Create Section
     try:
         section = Section.from_directory(
             directory, markup=markup, section_format_pairs=format_pairs
         )
@@ -191,110 +227,125 @@
     # Compile Section
     try:
         new_section = section.compile()
     except HeadingFormatError as error:
         raise click.UsageError(str(error)) from error
 
     if not new_section:
-        click.echo("There are no change log fragments to compile.")
+        click.echo(_("There are no change log fragments to compile."))
         return
 
     # Write to CHANGELOG
     try:
         fp: TextIOWrapper
         with changelog.open() as fp:  # type: ignore
             # TODO: use buffer reading, probably
             contents = fp.read()
             # TODO: magic variable
             lineno = find_first_occurrence("protokolo-section-tag", contents)
             if lineno is None:
                 raise click.UsageError(
-                    f"There is no 'protokolo-section-tag' in"
-                    f" {repr(changelog.name)}."
+                    # TRANSLATORS: do not translate protokolo-section-tag.
+                    _("There is no 'protokolo-section-tag' in {path}.").format(
+                        path=repr(changelog.name)
+                    )
                 )
             new_contents = insert_into_str(f"\n{new_section}", contents, lineno)
             if dry_run:
                 click.echo(new_contents, nl=False)
             else:
                 fp.seek(0)
                 fp.write(new_contents)
                 fp.truncate()
     except OSError as error:
-        # TODO: This is a little tricky to test. click already exits early if
-        # changelog isn't readable/writable.
         raise click.UsageError(str(error)) from error
 
     # Delete change log fragments
     if not dry_run:
         _delete_fragments(section)
 
 
-@main.command(name="init")
+_INIT_HELP = (
+    _(
+        "Set up your project to be ready to use Protokolo. It creates a change"
+        " log file, a change log directory with subsections that match the Keep"
+        " a Changelog recommendations, .protokolo.toml files with metadata for"
+        " those (sub)sections, and a root .protokolo.toml file with defaults"
+        " for subsequent Protokolo commands. Assuming defaults, the end result"
+        " looks like this:"
+    )
+    + "\n\n"
+    + cleandoc(
+        """
+        \b
+        .
+        ├── changelog.d
+        │   ├── added
+        │   │   └── .protokolo.toml
+        │   ├── changed
+        │   │   └── .protokolo.toml
+        │   ├── deprecated
+        │   │   └── .protokolo.toml
+        │   ├── fixed
+        │   │   └── .protokolo.toml
+        │   ├── removed
+        │   │   └── .protokolo.toml
+        │   ├── security
+        │   │   └── .protokolo.toml
+        │   └── .protokolo.toml
+        ├── CHANGELOG.md
+        └── .protokolo.toml
+        """
+    )
+    + "\n\n"
+    + _(
+        "Files that already exist are never overwritten, except the root"
+        " .protokolo.toml file, which is always (re-)generated."
+    )
+)
+
+
+@main.command(name="init", help=_INIT_HELP)
 @click.option(
     "--changelog",
     "-c",
     default="CHANGELOG.md",
-    show_default="determined by config, or CHANGELOG.md",
+    # TRANSLATORS: do not translate CHANGELOG.md.
+    show_default=_("determined by config, or CHANGELOG.md"),
     type=click.File("w", encoding="utf-8", lazy=True),
-    help="Change log file to create.",
+    help=_("Change log file to create."),
 )
 @click.option(
     "--directory",
     "-d",
     default="changelog.d",
-    show_default="determined by config, or changelog.d",
+    # TRANSLATORS: do not translate changelog.d.
+    show_default=_("determined by config, or changelog.d"),
     type=click.Path(
         file_okay=False,
         dir_okay=True,
         readable=True,
         path_type=Path,
     ),
-    help="Change log directory to create.",
+    help=_("Change log directory to create."),
 )
 @click.option(
     "--markup",
     "-m",
     default="markdown",
-    show_default="determined by config, or markdown",
+    # TRANSLATORS: do not translate markdown.
+    show_default=_("determined by config, or markdown"),
     type=click.Choice(SupportedMarkup.__args__),  # type: ignore
-    help="Markup language.",
+    help=_("Markup language."),
 )
 def init(
     changelog: click.File,
     directory: Path,
     markup: SupportedMarkup,
 ) -> None:
-    """Set up your project to be ready to use Protokolo. It creates a change log
-    file, a change log directory with subsections that match the Keep a
-    Changelog recommendations, .protokolo.toml files with metadata for those
-    (sub)sections, and a root .protokolo.toml file with defaults for subsequent
-    Protokolo commands. Assuming defaults, the end result looks like this:
-
-    \b
-    .
-    ├── changelog.d
-    │   ├── added
-    │   │   └── .protokolo.toml
-    │   ├── changed
-    │   │   └── .protokolo.toml
-    │   ├── deprecated
-    │   │   └── .protokolo.toml
-    │   ├── fixed
-    │   │   └── .protokolo.toml
-    │   ├── removed
-    │   │   └── .protokolo.toml
-    │   ├── security
-    │   │   └── .protokolo.toml
-    │   └── .protokolo.toml
-    ├── CHANGELOG.md
-    └── .protokolo.toml
-
-    Files that already exist are never overwritten, except the root
-    .protokolo.toml file, which is always (re-)generated.
-    """
     try:
         create_changelog(changelog.name, markup)
         create_keep_a_changelog(directory)
         create_root_toml(changelog.name, markup, directory)
     except OSError as error:
         raise click.UsageError(str(error)) from error
```

### Comparing `protokolo-2.0.1/src/protokolo/compile.py` & `protokolo-2.1.0/src/protokolo/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .config import SectionAttributes, parse_toml
 from .exceptions import (
     AttributeNotPositiveError,
     HeadingFormatError,
     ProtokoloTOMLIsADirectoryError,
     ProtokoloTOMLNotFoundError,
 )
+from .i18n import _
 from .types import StrPath, SupportedMarkup
 
 # pylint: disable=too-few-public-methods
 
 
 @attrs_.define(frozen=True)
 class Fragment:
@@ -120,21 +121,25 @@
                 errno.EISDIR, strerror(errno.EISDIR), str(protokolo_toml)
             )
         with protokolo_toml.open("rb") as fp:
             try:
                 values = parse_toml(fp, section=["protokolo", "section"])
             except tomllib.TOMLDecodeError as error:
                 raise tomllib.TOMLDecodeError(
-                    f"Invalid TOML in '{fp.name}': {error}"
+                    _("Invalid TOML in {file_name}: {error}").format(
+                        file_name=repr(fp.name), error=error
+                    )
                 ) from error
         try:
             attrs = SectionAttributes.from_dict(values, source=fp.name)
         except AttributeNotPositiveError as error:
             raise AttributeNotPositiveError(
-                f"Wrong value in '{fp.name}': {error}"
+                _("Wrong value in {file_name}: {error}").format(
+                    file_name=repr(fp.name), error=error
+                )
             ) from error
         # The level of the current section is determined first by the value
         # in the toml, second by the level value.
         level = values.get("level") or level
         attrs.level = level
         for key, val in section_format_pairs.items():
             attrs[key] = val
@@ -203,16 +208,17 @@
 
         try:
             heading = _MARKUP_FORMATTER_MAPPING[self.markup].format_section(
                 self.attrs,
             )
         except HeadingFormatError as error:
             raise HeadingFormatError(
-                f"Failed to format section heading of {repr(str(self.source))}:"
-                f" {str(error)}"
+                _(
+                    "Failed to format section heading of {source}: {error}"
+                ).format(source=repr(str(self.source)), error=str(error))
             ) from error
         buffer.write(heading)
         buffer.write("\n")
 
         if self.fragments:
             buffer.write("\n")
         for fragment in self.sorted_fragments():
```

### Comparing `protokolo-2.0.1/src/protokolo/config.py` & `protokolo-2.1.0/src/protokolo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from ._util import nested_itemgetter, type_in_expected_type
 from .exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
     DictTypeListError,
 )
+from .i18n import _
 from .types import StrPath, TOMLValue, TOMLValueType
 
 
 def parse_toml(
     toml: str | IO[bytes],
     section: Sequence[str] | None = None,
 ) -> dict[str, Any]:
@@ -41,15 +42,16 @@
         values = tomllib.loads(toml)
     else:
         try:
             values = tomllib.load(toml)
         except tomllib.TOMLDecodeError:
             raise
         except Exception as error:
-            raise TypeError("toml must be a str or IO[bytes]") from error
+            # TRANSLATORS: do not translate TOML, str, or IO[bytes]
+            raise TypeError(_("TOML must be a str or IO[bytes]")) from error
     if not section:
         return values
     try:
         return nested_itemgetter(*section)(values)
     except KeyError:
         return {}
 
@@ -208,20 +210,25 @@
                 positive.
             DictTypeError: value isn't an expected/supported type.
             DictTypeListError: if a list contains elements other than a dict.
         """
         super().validate()
         if self.level <= 0:
             raise AttributeNotPositiveError(
-                f"level must be a positive integer, got {repr(self.level)}"
+                # TRANSLATORS: do not translate level.
+                _("level must be a positive integer, got {level}").format(
+                    level=repr(self.level)
+                )
             )
         if self.order is not None and self.order <= 0:
             raise AttributeNotPositiveError(
-                f"order must be None or a positive integer, got"
-                f" {repr(self.order)}"
+                # TRANSLATORS: do not translate order.
+                _(
+                    "order must be None or a positive integer, got {order}"
+                ).format(order=repr(self.order))
             )
 
     @property
     def title(self) -> str:
         """The title of a section. If no value is provided, it defaults to
         'TODO: No section title defined'.
         """
@@ -297,15 +304,17 @@
         path = Path(path)
         section = cls._FILE_SECTION.get(path.name, ["protokolo"])
         with path.open("rb") as fp:
             try:
                 values = parse_toml(fp, section=section)
             except tomllib.TOMLDecodeError as error:
                 raise tomllib.TOMLDecodeError(
-                    f"Invalid TOML in '{fp.name}': {error}"
+                    _("Invalid TOML in {file_name}: {error}").format(
+                        file_name=repr(fp.name), error=error
+                    )
                 ) from error
         return cls.from_dict(values, source=path)
 
     @classmethod
     def find_config(cls, directory: StrPath) -> Path | None:
         """In *directory*, find the config file.
```

### Comparing `protokolo-2.0.1/src/protokolo/exceptions.py` & `protokolo-2.1.0/src/protokolo/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Exception classes."""
 
 from operator import attrgetter
 from typing import Any
 
+from .i18n import _
+
 
 class ProtokoloError(Exception):
     """Common exception class for all custom errors raised by the
     :mod:`protokolo` module.
     """
 
 
 class DictTypeError(TypeError, ProtokoloError):
     """Expected a value of a different type for a given key."""
 
     def __init__(self, *args: Any):
         if (args_count := len(args)) > 4:
             raise TypeError(
-                f"Function takes no more than 4 arguments ({args_count} given)"
+                _(
+                    "Function takes no more than 4 arguments ({args_count}"
+                    " given)"
+                ).format(args_count=args_count)
             )
         super().__init__(*args)
-        self.key = self._get_item_default(args, 0)
-        self.expected_type = self._get_item_default(args, 1)
-        self.got = self._get_item_default(args, 2)
-        self.source = self._get_item_default(args, 3)
+        self.key: str = self._get_item_default(args, 0)
+        self.expected_type: type = self._get_item_default(args, 1)
+        self.got: Any = self._get_item_default(args, 2)
+        self.source: str = self._get_item_default(args, 3)
 
     def __str__(self) -> str:
         """Custom str output."""
         amount = len(self.args)
         if amount <= 0:
             return super().__str__()
         text = self._key_text()
@@ -47,25 +52,29 @@
                     if isinstance(name, tuple):
                         name = self.expected_type
                     break
                 except AttributeError:
                     continue
             else:
                 raise TypeError(
-                    f"Expected a type, got {repr(self.expected_type)}"
+                    _("Expected a type, got {type}").format(
+                        type=repr(self.expected_type)
+                    )
                 )
-            text += f" Expected {name}."
+            text += " "
+            text += _("Expected {name}.").format(name=name)
         if amount >= 3:
-            text += f" Got {repr(self.got)}."
+            text += " "
+            text += _("Got {value}.").format(value=repr(self.got))
         if amount >= 4:
-            text = f"{self.source}: {text}"
+            text = _("{source}: {text}").format(source=self.source, text=text)
         return text
 
     def _key_text(self) -> str:
-        return f"{repr(self.key)} does not have the correct type."
+        return _("'{key}' does not have the correct type.").format(key=self.key)
 
     @staticmethod
     def _get_item_default(
         args: tuple[Any, ...], index: int, default: Any = None
     ) -> Any:
         try:
             return args[index]
@@ -75,15 +84,17 @@
 
 class DictTypeListError(DictTypeError):
     """Like :class:`DictTypeError`, but the item is in a list (inside of a
     dictionary) instead of in a dictionary.
     """
 
     def _key_text(self) -> str:
-        return f"List {repr(self.key)} contains an element with the wrong type."
+        return _(
+            "List '{key}' contains an element with the wrong type."
+        ).format(key=self.key)
 
 
 class ProtokoloTOMLError(ProtokoloError):
     """An exception that pertains to ``.protokolo.toml.``"""
 
 
 class AttributeNotPositiveError(ValueError, ProtokoloTOMLError):
```

### Comparing `protokolo-2.0.1/src/protokolo/initialise.py` & `protokolo-2.1.0/src/protokolo/initialise.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/src/protokolo/replace.py` & `protokolo-2.1.0/src/protokolo/replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/src/protokolo/types.py` & `protokolo-2.1.0/src/protokolo/types.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/tests/conftest.py` & `protokolo-2.1.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Fixtures and stuff."""
 
+import os
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 
 from protokolo._util import cleandoc_nl
 
 # pylint: disable=unused-argument
 
+os.environ["LC_ALL"] = "C"
+
 
 @pytest.fixture()
 def project_dir(tmpdir_factory, monkeypatch) -> Path:
     """Create a temporary project directory."""
     directory = Path(str(tmpdir_factory.mktemp("project_dir")))
 
     (directory / "CHANGELOG.md").write_text(
```

### Comparing `protokolo-2.0.1/tests/test_cli.py` & `protokolo-2.1.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,17 @@
             )
             in changelog
         )
         assert not Path("changelog.d/feature/foo.md").exists()
         assert Path("changelog.d/feature/bar.txt").exists()
 
     def test_no_protokolo_toml_in_changelog_d(self, runner):
-        """If changelog.d does not contain a .protokolo.toml file, TODO"""
+        """If changelog.d does not contain a .protokolo.toml file, print an
+        error message.
+        """
         Path("changelog.d/.protokolo.toml").unlink()
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
```

### Comparing `protokolo-2.0.1/tests/test_compile.py` & `protokolo-2.1.0/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/tests/test_config.py` & `protokolo-2.1.0/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Test the config code."""
 
 import tomllib
 from datetime import date, datetime
 from io import BytesIO
+from unittest.mock import MagicMock
 
 import pytest
 
 from protokolo._util import cleandoc_nl
 from protokolo.config import (
     GlobalConfig,
     SectionAttributes,
@@ -117,22 +118,21 @@
         assert config["none"] is None
         assert config["dict"] == {"foo": "bar"}
         assert config["list"] == [{"foo": "bar"}, {"baz": "quz"}]
         assert config["list-primitive"] == [1, 2]
 
     def test_from_dict_unsupported_type(self):
         """Many complex types are not supported."""
-        value = object()
+        value = MagicMock()
         with pytest.raises(DictTypeError) as exc_info:
             TOMLConfig.from_dict({"foo": value})
         error = exc_info.value
         assert error.key == "foo"
         assert error.expected_type == TOMLValueType
-        # TODO: This is not true because error.got is a (deep)copy of value.
-        # assert error.got == value
+        assert error.got == value
 
     def test_setitem(self):
         """You can set an item on the TOMLConfig object."""
         config = TOMLConfig.from_dict({"foo": "bar"})
         config["foo"] = "baz"
         assert config["foo"] == "baz"
```

### Comparing `protokolo-2.0.1/tests/test_exceptions.py` & `protokolo-2.1.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/tests/test_formatter.py` & `protokolo-2.1.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/tests/test_replace.py` & `protokolo-2.1.0/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.0.1/setup.py` & `protokolo-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,215 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: protokolo
+Version: 2.1.0
+Summary: Protokolo is a change log generator.
+Home-page: https://codeberg.org/carmenbianca/protokolo
+License: GPL-3.0-or-later
+Keywords: changelog,history,news
+Author: Carmen Bianca BAKKER
+Author-email: carmen@carmenbianca.eu
+Maintainer: Carmen Bianca BAKKER
+Maintainer-email: carmen@carmenbianca.eu
+Requires-Python: >=3.11,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Utilities
+Requires-Dist: attrs (>=22.1.0)
+Requires-Dist: click (>=8.0)
+Project-URL: Documentation, https://protokolo.readthedocs.io
+Project-URL: Repository, https://codeberg.org/carmenbianca/protokolo
+Description-Content-Type: text/markdown
+
+<!--
+SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
+
+SPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later
+-->
+
+# Protokolo
+
+[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
+[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
+[![Translation status](https://hosted.weblate.org/widget/protokolo/protokolo/svg-badge.svg)](https://hosted.weblate.org/engage/protokolo/)
+
+Protokolo is a change log generator.
+
+Protokolo allows you to maintain your change log fragments in separate files,
+and then finally aggregate them into a new section in CHANGELOG just before
+release.
+
+## Table of contents
+
+- [Background](#background)
+- [Install](#install)
+- [Usage](#usage)
+- [Maintainers](#maintainers)
+- [Contributing](#contributing)
+- [Licensing](#licensing)
+
+## Background
+
+Change logs are [a really good idea](https://keepachangelog.com/).
+Unfortunately, they are also a bit of a pain when combined with version control:
+
+- Different merge requests all edit the same area in CHANGELOG, inevitably
+  resulting in merge conflicts.
+- If a section for an unreleased version does not yet exist in the main branch's
+  CHANGELOG (typically shortly after release), feature branches must create this
+  section. If multiple feature branches do this, you get more merge conflicts.
+- Old merge requests, when merged, sometimes add their change log entry to the
+  section of a release that is already published.
+
+Life would be a lot easier if you didn't have to deal with these problems.
+
+Enter Protokolo
+([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The
+idea is very simple: for every change log entry, create a new file. Finally,
+just before release, compile the contents of those files into a new section in
+CHANGELOG, and delete the files.
+
+### See also
+
+[Towncrier](https://github.com/twisted/towncrier) is an older and more widely
+used implementation of the same idea. Protokolo is distinct in that it uses a
+directory hierarchy instead of putting all metadata in the file name of each
+change log fragment. Furthermore, Protokolo does no fancy formatting of
+fragments---what you write is what you get.
+
+There are three main problems I encountered in Towncrier that Protokolo attempts
+to address:
+
+- When using Towncrier, I would always forget which fragment types are available
+  to me and had to look them up. These fragment types can also differ per
+  repository. In Protokolo, the types are always visible because they are
+  directories.
+- Towncrier fragments are sorted by their ID, which is typically an issue or PR
+  number. This isn't always what I want.
+- Because (some) Towncrier workflows put the PR number in the file name as
+  metadata, I would have to open the PR before I could create the change log
+  fragment.
+
+A much younger version of me also tried her hand at writing a program like this
+in [changelogdir](https://pypi.org/project/changelogdir/).
+
+## Install
+
+Protokolo is a regular Python package
+[hosted on PyPI](https://pypi.python.org/pypi/protokolo). You can install it
+using `pipx install protokolo`. Make sure that `~/.local/share/bin` is in your
+`$PATH` with `pipx ensurepath`.
+
+## Usage
+
+For full documentation and options, read the documentation at
+<https://protokolo.readthedocs.io>.
+
+### Initial set-up
+
+To set up your project for use with Protokolo, run `protokolo init`. This will
+create a `CHANGELOG.md` file (if one did not already exist) and a directory
+structure under `changelog.d`. The directory structure uses the
+[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking
+like this:
+
+```
+.
+├── changelog.d
+│   ├── added
+│   │   └── .protokolo.toml
+│   ├── changed
+│   │   └── .protokolo.toml
+│   ├── deprecated
+│   │   └── .protokolo.toml
+│   ├── fixed
+│   │   └── .protokolo.toml
+│   ├── removed
+│   │   └── .protokolo.toml
+│   ├── security
+│   │   └── .protokolo.toml
+│   └── .protokolo.toml
+├── CHANGELOG.md
+└── .protokolo.toml
+```
+
+The `.protokolo.toml` files in `changelog.d` contain metadata for their
+respective sections: the section title, heading level, and order. Their
+inclusion is mandatory.
+
+The `.protokolo.toml` file in the root of the project contains configurations
+for Protokolo that reduce the amount of typing you need to do when running
+commands.
+
+If a `CHANGELOG.md` file already existed, make sure to add a line containing
+`<!-- protokolo-section-tag -->` just before the heading of the latest release.
+
+### Adding fragments
+
+To add a change log fragment, create the file `changelog.d/added/my_feature.md`,
+and write something like:
+
+```markdown
+- Added `--my-new-feature` option.
+```
+
+Note the bullet at the start---Protokolo does not add them for you. What you
+write is exactly what you get.
+
+You can add more files. Change log fragments in the same section (read:
+directory) are sorted alphabetically by their file name. If you want to make
+certain that some change log fragments go first or last, prefix the file with
+`000_` or `zzz_`. For example, you can create
+`changelog.d/added/000_important_feature.md` to make it appear first.
+
+### Compiling your change log
+
+You compile your change log with `protokolo compile`. This will take all change
+log fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run
+it now, the following section is added after the
+`<!-- protokolo-section-tag -->` comment:
+
+```markdown
+## ${version} - 2023-11-08
+
+### Added
+
+- Added important feature.
+- Added `--my-new-feature` option.
+```
+
+The Markdown files in `changelog.d/added/` are deleted. You can manually replace
+`${version}` with a release version, or you can pass the option
+`--format version 1.0.0` to `protokolo compile` to format the heading at compile
+time.
+
+## Maintainers
+
+- Carmen Bianca BAKKER <carmen@carmenbianca.eu>
+
+## Contributing
+
+The code and issue tracker is hosted at
+<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any
+issues. For pull requests, bug fixes are always welcome, but new features should
+probably be discussed in any issue first.
+
+Translations are done at
+<https://hosted.weblate.org/projects/protokolo/protokolo/> using Weblate. If
+there are issues with translation, feel free to open an issue at Codeberg.
+
+## Licensing
 
-package_dir = \
-{'': 'src'}
+All code is licensed under GPL-3.0-or-later.
 
-packages = \
-['protokolo']
+All documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.1.0', 'click>=8.0']
-
-entry_points = \
-{'console_scripts': ['protokolo = protokolo.cli:main']}
-
-setup_kwargs = {
-    'name': 'protokolo',
-    'version': '2.0.1',
-    'description': 'Protokolo is a change log generator.',
-    'long_description': "<!--\nSPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\nSPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later\n-->\n\n# Protokolo\n\n[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)\n\nProtokolo is a change log generator.\n\nProtokolo allows you to maintain your change log fragments in separate files,\nand then finally aggregate them into a new section in CHANGELOG just before\nrelease.\n\n## Table of contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Maintainers](#maintainers)\n- [Contributing](#contributing)\n- [Licensing](#licensing)\n\n## Background\n\nChange logs are [a really good idea](https://keepachangelog.com/).\nUnfortunately, they are also a bit of a pain when combined with version control:\n\n- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll\n  need to resolve a conflict when trying to merge them both.\n- Just after you make a release, you need to create a new section in CHANGELOG\n  for your next release. If you forget this busywork, new feature branches will\n  need to create this section, which increases the chance of merge conflicts.\n- If a feature branch adds a change log entry to the section for the next v2.0\n  release, and v2.0 subsequently releases without merging that feature branch,\n  then merging that feature branch afterwards would still add the change log\n  entry to the v2.0 section, even though it should now go to the unreleased v3.0\n  section.\n\nLife would be a lot easier if you didn't have to deal with these problems.\n\nEnter Protokolo\n([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The\nidea is very simple: for every change log entry, create a new file. Finally,\njust before release, compile the contents of those files into a new section in\nCHANGELOG, and delete the files.\n\n### See also\n\n[Towncrier](https://github.com/twisted/towncrier) is an older and more widely\nused implementation of the same idea. Protokolo is distinct in that it uses a\ndirectory hierarchy instead of putting all metadata in the file name of each\nchange log fragment. Furthermore, Protokolo does no fancy formatting of\nfragments---what you write is what you get.\n\nThere are three main problems I encountered in Towncrier that Protokolo attempts\nto address:\n\n- When using Towncrier, I would always forget which fragment types are available\n  to me and had to look them up. These fragment types can also differ per\n  repository. In Protokolo, the types are always visible because they are\n  directories.\n- Towncrier fragments are sorted by their ID, which is typically an issue or PR\n  number. This isn't always what I want.\n- Because (some) Towncrier workflows put the PR number in the file name as\n  metadata, I would have to open the PR before I could create the change log\n  fragment.\n\nA much younger version of me also tried her hand at writing a program like this\nin [changelogdir](https://pypi.org/project/changelogdir/).\n\n## Install\n\nProtokolo is a regular Python package. You can install it using\n`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`\nwith `pipx ensurepath`.\n\n## Usage\n\nFor full documentation and options, read the documentation at\n<https://protokolo.readthedocs.io>.\n\n### Initial set-up\n\nTo set up your project for use with Protokolo, run `protokolo init`. This will\ncreate a `CHANGELOG.md` file (if one did not already exist) and a directory\nstructure under `changelog.d`. The directory structure uses the\n[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking\nlike this:\n\n```\n.\n├── changelog.d\n│   ├── added\n│   │   └── .protokolo.toml\n│   ├── changed\n│   │   └── .protokolo.toml\n│   ├── deprecated\n│   │   └── .protokolo.toml\n│   ├── fixed\n│   │   └── .protokolo.toml\n│   ├── removed\n│   │   └── .protokolo.toml\n│   ├── security\n│   │   └── .protokolo.toml\n│   └── .protokolo.toml\n├── CHANGELOG.md\n└── .protokolo.toml\n```\n\nThe `.protokolo.toml` files in `changelog.d` contain metadata for their\nrespective sections: the section title, heading level, and order. Their\ninclusion is mandatory.\n\nThe `.protokolo.toml` file in the root of the project contains configurations\nfor Protokolo that reduce the amount of typing you need to do when running\ncommands.\n\nIf a `CHANGELOG.md` file already existed, make sure to add a line containing\n`<!-- protokolo-section-tag -->` just before the heading of the latest release.\n\n### Adding fragments\n\nTo add a change log fragment, create the file `changelog.d/added/my_feature.md`,\nand write something like:\n\n```markdown\n- Added `--my-new-feature` option.\n```\n\nNote the bullet at the start---Protokolo does not add them for you. What you\nwrite is exactly what you get.\n\nYou can add more files. Change log fragments in the same section (read:\ndirectory) are sorted alphabetically by their file name. If you want to make\ncertain that some change log fragments go first or last, prefix the file with\n`000_` or `zzz_`. For example, you can create\n`changelog.d/added/000_important_feature.md` to make it appear first.\n\n### Compiling your change log\n\nYou compile your change log with `protokolo compile`. This will take all change\nlog fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run\nit now, the following section is added after the\n`<!-- protokolo-section-tag -->` comment:\n\n```markdown\n## ${version} - 2023-11-08\n\n### Added\n\n- Added important feature.\n- Added `--my-new-feature` option.\n```\n\nThe Markdown files in `changelog.d/added/` are deleted. You can manually replace\n`${version}` with a release version, or you can pass the option\n`--format version 1.0.0` to `protokolo compile` to format the heading at compile\ntime.\n\n## Maintainers\n\n- Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\n## Contributing\n\nThe code and issue tracker is hosted at\n<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any\nissues. For pull requests, bug fixes are always welcome, but new features should\nprobably be discussed in any issue first.\n\n## Licensing\n\nAll code is licensed under GPL-3.0-or-later.\n\nAll documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.\n\nSome configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.\n\nThe repository is [REUSE](https://reuse.software)-compliant. Check the\nindividual files for their exact licensing.\n",
-    'author': 'Carmen Bianca BAKKER',
-    'author_email': 'carmen@carmenbianca.eu',
-    'maintainer': 'Carmen Bianca BAKKER',
-    'maintainer_email': 'carmen@carmenbianca.eu',
-    'url': 'https://codeberg.org/carmenbianca/protokolo',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.11,<4.0',
-}
+Some configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.
 
+The repository is [REUSE](https://reuse.software)-compliant. Check the
+individual files for their exact licensing.
 
-setup(**setup_kwargs)
```

