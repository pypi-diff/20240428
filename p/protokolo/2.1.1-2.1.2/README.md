# Comparing `tmp/protokolo-2.1.1.tar.gz` & `tmp/protokolo-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-2.1.1.tar", max compression
+gzip compressed data, was "protokolo-2.1.2.tar", max compression
```

## Comparing `protokolo-2.1.1.tar` & `protokolo-2.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3486 2024-04-27 22:14:42.922438 protokolo-2.1.1/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-2.1.1/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-2.1.1/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-2.1.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-2.1.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     7095 2024-04-27 21:40:40.247205 protokolo-2.1.1/README.md
--rw-r--r--   0        0        0     2233 2024-04-27 21:40:40.251205 protokolo-2.1.1/_build.py
--rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-2.1.1/docs/Makefile
--rw-r--r--   0        0        0     2535 2024-04-27 22:11:11.128248 protokolo-2.1.1/docs/conf.py
--rw-r--r--   0        0        0      744 2024-04-27 21:40:40.251205 protokolo-2.1.1/docs/index.rst
--rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-2.1.1/docs/make.bat
--rw-r--r--   0        0        0      271 2024-04-27 21:40:40.251205 protokolo-2.1.1/docs/man/index.rst
--rw-r--r--   0        0        0     1638 2024-04-27 21:40:40.251205 protokolo-2.1.1/docs/man/protokolo-compile.rst
--rw-r--r--   0        0        0     2078 2024-04-27 21:40:40.251205 protokolo-2.1.1/docs/man/protokolo-init.rst
--rw-r--r--   0        0        0     1036 2024-04-27 21:40:40.251205 protokolo-2.1.1/docs/man/protokolo.rst
--rw-r--r--   0        0        0     7976 2024-04-27 21:40:40.251205 protokolo-2.1.1/docs/reference.md
--rw-r--r--   0        0        0     2944 2024-04-27 22:18:04.420562 protokolo-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      177 2024-04-27 22:18:04.424562 protokolo-2.1.1/src/protokolo/__init__.py
--rw-r--r--   0        0        0      290 2024-04-27 21:40:40.255205 protokolo-2.1.1/src/protokolo/__main__.py
--rw-r--r--   0        0        0     4030 2024-04-27 21:40:40.255205 protokolo-2.1.1/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     1424 2024-04-27 21:40:40.255205 protokolo-2.1.1/src/protokolo/_util.py
--rw-r--r--   0        0        0    10749 2024-04-27 21:40:40.255205 protokolo-2.1.1/src/protokolo/cli.py
--rw-r--r--   0        0        0    10420 2024-04-27 21:40:40.255205 protokolo-2.1.1/src/protokolo/compile.py
--rw-r--r--   0        0        0    12133 2024-04-27 21:40:40.255205 protokolo-2.1.1/src/protokolo/config.py
--rw-r--r--   0        0        0     3619 2024-04-27 21:40:40.259205 protokolo-2.1.1/src/protokolo/exceptions.py
--rw-r--r--   0        0        0     1099 2024-04-27 21:40:40.259205 protokolo-2.1.1/src/protokolo/i18n.py
--rw-r--r--   0        0        0     3785 2024-04-27 21:40:40.259205 protokolo-2.1.1/src/protokolo/initialise.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-2.1.1/src/protokolo/py.typed
--rw-r--r--   0        0        0     1520 2024-04-27 21:40:40.259205 protokolo-2.1.1/src/protokolo/replace.py
--rw-r--r--   0        0        0      903 2024-04-27 21:40:40.259205 protokolo-2.1.1/src/protokolo/types.py
--rw-r--r--   0        0        0     2263 2024-04-27 21:40:40.259205 protokolo-2.1.1/tests/conftest.py
--rw-r--r--   0        0        0    20548 2024-04-27 21:40:40.259205 protokolo-2.1.1/tests/test_cli.py
--rw-r--r--   0        0        0    15759 2024-04-27 21:40:40.259205 protokolo-2.1.1/tests/test_compile.py
--rw-r--r--   0        0        0    11400 2024-04-27 21:40:40.259205 protokolo-2.1.1/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-2.1.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     6053 2024-04-27 21:40:40.259205 protokolo-2.1.1/tests/test_formatter.py
--rw-r--r--   0        0        0     3907 2024-04-27 21:40:40.259205 protokolo-2.1.1/tests/test_replace.py
--rw-r--r--   0        0        0     8065 1970-01-01 00:00:00.000000 protokolo-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3539 2024-04-27 22:37:52.193404 protokolo-2.1.2/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-2.1.2/LICENSES/
+-rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-2.1.2/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-2.1.2/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-2.1.2/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     7095 2024-04-27 21:40:40.247205 protokolo-2.1.2/README.md
+-rw-r--r--   0        0        0     2233 2024-04-27 21:40:40.251205 protokolo-2.1.2/_build.py
+-rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-2.1.2/docs/Makefile
+-rw-r--r--   0        0        0     2535 2024-04-27 22:11:11.128248 protokolo-2.1.2/docs/conf.py
+-rw-r--r--   0        0        0      744 2024-04-27 21:40:40.251205 protokolo-2.1.2/docs/index.rst
+-rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-2.1.2/docs/make.bat
+-rw-r--r--   0        0        0      271 2024-04-27 21:40:40.251205 protokolo-2.1.2/docs/man/index.rst
+-rw-r--r--   0        0        0     1638 2024-04-27 21:40:40.251205 protokolo-2.1.2/docs/man/protokolo-compile.rst
+-rw-r--r--   0        0        0     2078 2024-04-27 21:40:40.251205 protokolo-2.1.2/docs/man/protokolo-init.rst
+-rw-r--r--   0        0        0     1036 2024-04-27 21:40:40.251205 protokolo-2.1.2/docs/man/protokolo.rst
+-rw-r--r--   0        0        0     7976 2024-04-27 21:40:40.251205 protokolo-2.1.2/docs/reference.md
+-rw-r--r--   0        0        0     2944 2024-04-27 22:37:26.309122 protokolo-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-27 22:37:26.309122 protokolo-2.1.2/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-27 21:40:40.255205 protokolo-2.1.2/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     4030 2024-04-27 21:40:40.255205 protokolo-2.1.2/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1424 2024-04-27 21:40:40.255205 protokolo-2.1.2/src/protokolo/_util.py
+-rw-r--r--   0        0        0    10749 2024-04-27 21:40:40.255205 protokolo-2.1.2/src/protokolo/cli.py
+-rw-r--r--   0        0        0    10420 2024-04-27 21:40:40.255205 protokolo-2.1.2/src/protokolo/compile.py
+-rw-r--r--   0        0        0    12133 2024-04-27 21:40:40.255205 protokolo-2.1.2/src/protokolo/config.py
+-rw-r--r--   0        0        0     3619 2024-04-27 21:40:40.259205 protokolo-2.1.2/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     1099 2024-04-27 21:40:40.259205 protokolo-2.1.2/src/protokolo/i18n.py
+-rw-r--r--   0        0        0     3785 2024-04-27 21:40:40.259205 protokolo-2.1.2/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-2.1.2/src/protokolo/py.typed
+-rw-r--r--   0        0        0     1520 2024-04-27 21:40:40.259205 protokolo-2.1.2/src/protokolo/replace.py
+-rw-r--r--   0        0        0      903 2024-04-27 21:40:40.259205 protokolo-2.1.2/src/protokolo/types.py
+-rw-r--r--   0        0        0     2263 2024-04-27 21:40:40.259205 protokolo-2.1.2/tests/conftest.py
+-rw-r--r--   0        0        0    20548 2024-04-27 21:40:40.259205 protokolo-2.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0    15759 2024-04-27 21:40:40.259205 protokolo-2.1.2/tests/test_compile.py
+-rw-r--r--   0        0        0    11400 2024-04-27 21:40:40.259205 protokolo-2.1.2/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-2.1.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6053 2024-04-27 21:40:40.259205 protokolo-2.1.2/tests/test_formatter.py
+-rw-r--r--   0        0        0     3907 2024-04-27 21:40:40.259205 protokolo-2.1.2/tests/test_replace.py
+-rw-r--r--   0        0        0     8065 1970-01-01 00:00:00.000000 protokolo-2.1.2/PKG-INFO
```

### Comparing `protokolo-2.1.1/CHANGELOG.md` & `protokolo-2.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 
 The versions follow [semantic versioning](https://semver.org) for the
 `protokolo` CLI command and its behaviour. There are no guarantees of stability
 for the `protokolo` Python library.
 
 <!-- protokolo-section-tag -->
 
-## 2.1.1 - 2024-04-28 [YANKED]
+## 2.1.2 - 2024-04-28
+
+### Fixed
+
+- Fix error in change log.
+
+## 2.1.1 - 2024-04-28
 
 ### Added
 
 - Implemented internationalisation via Weblate and Forgejo Actions.
 
 ### Fixed
```

### Comparing `protokolo-2.1.1/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-2.1.2/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/LICENSES/CC0-1.0.txt` & `protokolo-2.1.2/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/LICENSES/GPL-3.0-or-later.txt` & `protokolo-2.1.2/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/README.md` & `protokolo-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/_build.py` & `protokolo-2.1.2/_build.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/Makefile` & `protokolo-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/conf.py` & `protokolo-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/index.rst` & `protokolo-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/make.bat` & `protokolo-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/man/protokolo-compile.rst` & `protokolo-2.1.2/docs/man/protokolo-compile.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/man/protokolo-init.rst` & `protokolo-2.1.2/docs/man/protokolo-init.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/man/protokolo.rst` & `protokolo-2.1.2/docs/man/protokolo.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/docs/reference.md` & `protokolo-2.1.2/docs/reference.md`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/pyproject.toml` & `protokolo-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "2.1.1"
+version = "2.1.2"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
@@ -82,15 +82,15 @@
 script = "_build.py"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [bumpver]
-current_version = "v2.1.1"
+current_version = "v2.1.2"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `protokolo-2.1.1/src/protokolo/_formatter.py` & `protokolo-2.1.2/src/protokolo/_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/_util.py` & `protokolo-2.1.2/src/protokolo/_util.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/cli.py` & `protokolo-2.1.2/src/protokolo/cli.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/compile.py` & `protokolo-2.1.2/src/protokolo/compile.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/config.py` & `protokolo-2.1.2/src/protokolo/config.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/exceptions.py` & `protokolo-2.1.2/src/protokolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/i18n.py` & `protokolo-2.1.2/src/protokolo/i18n.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/initialise.py` & `protokolo-2.1.2/src/protokolo/initialise.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/replace.py` & `protokolo-2.1.2/src/protokolo/replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/src/protokolo/types.py` & `protokolo-2.1.2/src/protokolo/types.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/conftest.py` & `protokolo-2.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/test_cli.py` & `protokolo-2.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/test_compile.py` & `protokolo-2.1.2/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/test_config.py` & `protokolo-2.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/test_exceptions.py` & `protokolo-2.1.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/test_formatter.py` & `protokolo-2.1.2/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/tests/test_replace.py` & `protokolo-2.1.2/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.1/PKG-INFO` & `protokolo-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protokolo
-Version: 2.1.1
+Version: 2.1.2
 Summary: Protokolo is a change log generator.
 Home-page: https://codeberg.org/carmenbianca/protokolo
 License: GPL-3.0-or-later
 Keywords: changelog,history,news
 Author: Carmen Bianca BAKKER
 Author-email: carmen@carmenbianca.eu
 Maintainer: Carmen Bianca BAKKER
```

