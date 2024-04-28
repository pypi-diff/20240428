# Comparing `tmp/stringdatadeque-1.1.1.tar.gz` & `tmp/stringdatadeque-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringdatadeque-1.1.1.tar", last modified: Sun Apr 21 03:27:49 2024, max compression
+gzip compressed data, was "stringdatadeque-1.1.3.tar", last modified: Sat Apr 27 04:54:42 2024, max compression
```

## Comparing `stringdatadeque-1.1.1.tar` & `stringdatadeque-1.1.3.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.449195 stringdatadeque-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.441195 stringdatadeque-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.441195 stringdatadeque-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.github/workflows/tox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43538 2024-04-21 03:27:49.449195 stringdatadeque-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.445195 stringdatadeque-1.1.1/StringDataDeque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43538 2024-04-21 03:27:49.000000 stringdatadeque-1.1.1/StringDataDeque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-21 03:27:49.000000 stringdatadeque-1.1.1/StringDataDeque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:27:49.000000 stringdatadeque-1.1.1/StringDataDeque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-21 03:27:49.000000 stringdatadeque-1.1.1/StringDataDeque.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 03:27:49.000000 stringdatadeque-1.1.1/StringDataDeque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/check_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.445195 stringdatadeque-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/index.rst.bak
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.445195 stringdatadeque-1.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/source/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/docs/source/stringdatadeque.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:27:49.449195 stringdatadeque-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.437195 stringdatadeque-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.445195 stringdatadeque-1.1.1/src/stringdatadeque/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/src/stringdatadeque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/src/stringdatadeque/encryptedstringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/src/stringdatadeque/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/src/stringdatadeque/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18362 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/src/stringdatadeque/stringdatadeque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:27:49.445195 stringdatadeque-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/tests/default.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/tests/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/tests/test_encryptedssgtringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/tests/test_stringdatadeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-21 03:27:43.000000 stringdatadeque-1.1.1/tests/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.830778 stringdatadeque-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.822778 stringdatadeque-1.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.822778 stringdatadeque-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/gh_pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/tox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43790 2024-04-27 04:54:42.830778 stringdatadeque-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/StringDataDeque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43790 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/check_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.818778 stringdatadeque-1.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/index.rst.bak
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/source/stringdatadeque.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 04:54:42.830778 stringdatadeque-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.818778 stringdatadeque-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/src/stringdatadeque/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/encryptedstringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18362 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/stringdatadeque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/default.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/test_encryptedssgtringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/test_stringdatadeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/timing.py
```

### Comparing `stringdatadeque-1.1.1/.github/workflows/pypi.yaml` & `stringdatadeque-1.1.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/.github/workflows/tox.yaml` & `stringdatadeque-1.1.3/.github/workflows/tox.yaml`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/.gitignore` & `stringdatadeque-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/.pre-commit-config.yaml` & `stringdatadeque-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/LICENSE` & `stringdatadeque-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/PKG-INFO` & `stringdatadeque-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.1.1
+Version: 1.1.3
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,14 +674,16 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
+Project-URL: homepage, https://github.com/rbroderi/StringDataDeque
+Project-URL: documentation, https://rbroderi.github.io/StringDataDeque/
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beartype
 Requires-Dist: typing-extensions; python_version < "3.12"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -693,36 +695,38 @@
 Requires-Dist: pytest-pretty; extra == "dev"
 Requires-Dist: ruamel.yaml; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: toml-sort; extra == "dev"
 Requires-Dist: uv; extra == "dev"
 Requires-Dist: validate-pyproject; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
-Requires-Dist: Sphinx; extra == "dev"
-Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
-Requires-Dist: sphinx-pyproject; extra == "dev"
-Requires-Dist: sphinx-rtd-size; extra == "dev"
-Requires-Dist: sphinx-rtd-theme; extra == "dev"
-Requires-Dist: autodocsumm; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
+Provides-Extra: docs
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinx-rtd-size; extra == "docs"
+Requires-Dist: autodocsumm; extra == "docs"
+Requires-Dist: sphinx-pyproject; extra == "docs"
+Requires-Dist: pycryptodome; extra == "docs"
 
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
 
 ## Installation
-
+https://pypi.org/project/StringDataDeque/
 ```bash
 pip install StringDataDeque
 ```
 
 ## Uses
 
 This is designed to be a drop-in replacement for when you might want to append to a string in a loop.
```

### Comparing `stringdatadeque-1.1.1/README.md` & `stringdatadeque-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
 
 ## Installation
-
+https://pypi.org/project/StringDataDeque/
 ```bash
 pip install StringDataDeque
 ```
 
 ## Uses
 
 This is designed to be a drop-in replacement for when you might want to append to a string in a loop.
```

### Comparing `stringdatadeque-1.1.1/StringDataDeque.egg-info/PKG-INFO` & `stringdatadeque-1.1.3/StringDataDeque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.1.1
+Version: 1.1.3
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,14 +674,16 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
+Project-URL: homepage, https://github.com/rbroderi/StringDataDeque
+Project-URL: documentation, https://rbroderi.github.io/StringDataDeque/
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beartype
 Requires-Dist: typing-extensions; python_version < "3.12"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -693,36 +695,38 @@
 Requires-Dist: pytest-pretty; extra == "dev"
 Requires-Dist: ruamel.yaml; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: toml-sort; extra == "dev"
 Requires-Dist: uv; extra == "dev"
 Requires-Dist: validate-pyproject; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
-Requires-Dist: Sphinx; extra == "dev"
-Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
-Requires-Dist: sphinx-pyproject; extra == "dev"
-Requires-Dist: sphinx-rtd-size; extra == "dev"
-Requires-Dist: sphinx-rtd-theme; extra == "dev"
-Requires-Dist: autodocsumm; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
+Provides-Extra: docs
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinx-rtd-size; extra == "docs"
+Requires-Dist: autodocsumm; extra == "docs"
+Requires-Dist: sphinx-pyproject; extra == "docs"
+Requires-Dist: pycryptodome; extra == "docs"
 
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
 
 ## Installation
-
+https://pypi.org/project/StringDataDeque/
 ```bash
 pip install StringDataDeque
 ```
 
 ## Uses
 
 This is designed to be a drop-in replacement for when you might want to append to a string in a loop.
```

### Comparing `stringdatadeque-1.1.1/StringDataDeque.egg-info/SOURCES.txt` & `stringdatadeque-1.1.3/StringDataDeque.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pyproject.toml
 requirements-dev.txt
 requirements-optional.txt
 requirements.txt
 .github/dependabot.yml
 .github/workflows/black.yaml
 .github/workflows/dapperdata.yaml
+.github/workflows/gh_pages.yaml
 .github/workflows/mypy.yaml
 .github/workflows/pypi.yaml
 .github/workflows/pytest.yaml
 .github/workflows/ruff.yaml
 .github/workflows/tomlsort.yaml
 .github/workflows/tox.yaml
 StringDataDeque.egg-info/PKG-INFO
@@ -28,15 +29,15 @@
 StringDataDeque.egg-info/top_level.txt
 docs/Makefile
 docs/conf.py
 docs/getting-started.rst
 docs/index.rst
 docs/index.rst.bak
 docs/make.bat
-docs/source/custom.css
+docs/_static/css/custom.css
 docs/source/modules.rst
 docs/source/stringdatadeque.rst
 src/stringdatadeque/__init__.py
 src/stringdatadeque/encryptedstringdeque.py
 src/stringdatadeque/protocols.py
 src/stringdatadeque/py.typed
 src/stringdatadeque/stringdatadeque.py
```

### Comparing `stringdatadeque-1.1.1/check_names.py` & `stringdatadeque-1.1.3/check_names.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/docs/Makefile` & `stringdatadeque-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/docs/make.bat` & `stringdatadeque-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/docs/source/stringdatadeque.rst` & `stringdatadeque-1.1.3/docs/source/stringdatadeque.rst`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/justfile` & `stringdatadeque-1.1.3/justfile`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 # install into the venv
 install:
     @# $(PYTHON_PYENV)
     {{if env("CI","false") != "false" { "" } else { "pyenv install --skip-existing $PYTHON_VERSION "} }}
     @# $(PYTHON_VENV)
     {{ if env("USE_SYSTEM_PYTHON", "false") != "false" { "" } else { "python -m venv .venv" } }}
     @# pip
-    {{PYTHON}} -m pip install -e .[dev,optional]
+    {{PYTHON}} -m pip install -e .[dev,optional,docs]
 
 # Install pre-commit
 pre-commit_install:
     pre-commit install
 
 # Setup sphynx autodoc
 setup_autodoc:
     sphinx-apidoc -f -o docs/source {{PACKAGE_SLUG}}
 
+# copy as template
+copy_as_template DEST:
+    rsync -r --exclude .mypy_cache --exclude .pytest_cache --exclude .ruff_cache --exclude .tox --exclude .venv --exclude StringDataDeque* --exclude .git --exclude stringdatadeque* ./ {{DEST}}
+    cd {{DEST}} && git init . && git commit --allow-empty -m 'Make initial root commit'
+
 # profiling
 profile:
     python -m cProfile -s time -o timing.prof tests/timing.py --profile
     snakeviz timing.prof
 
 #
 # Formatting
```

### Comparing `stringdatadeque-1.1.1/pyproject.toml` & `stringdatadeque-1.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
 
 [project]
 authors = [{"name" = "R.Broderick"}]
 description = "Useful when building a string from data that can be converted into a string, in parts."
-version = "1.1.1"
+version = "1.1.3"
 license = {"file" = "LICENSE"}
 name = "StringDataDeque"
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = ["beartype", "typing-extensions; python_version < '3.12'"]
 requires-python = ">=3.10.0"
 
 [project.optional-dependencies]
@@ -23,20 +23,14 @@
   "pytest-pretty",
   "ruamel.yaml",
   "ruff",
   "toml-sort",
   "uv",
   "validate-pyproject",
   "packaging",
-  "Sphinx",
-  "sphinx-autodoc-typehints",
-  "sphinx-pyproject",
-  "sphinx-rtd-size",
-  "sphinx-rtd-theme ",
-  "autodocsumm",
   "snakeviz",
   "pre-commit",
   "tox",
   "tox-pyenv-redux",
   "pylint",
   "perflint",
   "snakeviz"
@@ -44,14 +38,27 @@
 # pep725
 # [external]
 # build-requires = [
 # "virtual:compiler/rust",
 # "virtual:compiler/cargo",
 # ]
 optional = ["pycryptodome"]
+docs = [
+  "Sphinx",
+  "sphinx-autodoc-typehints",
+  "sphinx-rtd-theme",
+  "sphinx-rtd-size",
+  "autodocsumm",
+  "sphinx-pyproject",
+  "pycryptodome"
+]
+
+[project.urls]
+homepage = "https://github.com/rbroderi/StringDataDeque"
+documentation = "https://rbroderi.github.io/StringDataDeque/"
 
 [tool.dapperdata]
 exclude_paths = [".venv", ".mypy_cache", ".git", ".vscode"]
 
 [tool.pylint.format]
 max-line-length = 200
 
@@ -254,15 +261,15 @@
 sphinx_rtd_size_width = "90%"
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 auto_doc_default_options = {'autosummary' = true}
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 html_theme = "sphinx_rtd_theme"
-html_style = "../../../source/custom.css"
+html_style = "css/custom.css"
 html_static_path = ["_static"]
 html_theme_options = {'display_version' = true, 'sticky_navigation' = true, 'includehidden' = true, 'titles_only' = false}
 autosummary_generate = true
 
 [tool.sphinx-pyproject.autodoc_default_options]
 exclude-members = """
   __weakref__,
```

### Comparing `stringdatadeque-1.1.1/src/stringdatadeque/__init__.py` & `stringdatadeque-1.1.3/src/stringdatadeque/__init__.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/src/stringdatadeque/encryptedstringdeque.py` & `stringdatadeque-1.1.3/src/stringdatadeque/encryptedstringdeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/src/stringdatadeque/protocols.py` & `stringdatadeque-1.1.3/src/stringdatadeque/protocols.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/src/stringdatadeque/stringdatadeque.py` & `stringdatadeque-1.1.3/src/stringdatadeque/stringdatadeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/tests/private.pem` & `stringdatadeque-1.1.3/tests/private.pem`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/tests/test_encryptedssgtringdeque.py` & `stringdatadeque-1.1.3/tests/test_encryptedssgtringdeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/tests/test_stringdatadeque.py` & `stringdatadeque-1.1.3/tests/test_stringdatadeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.1/tests/timing.py` & `stringdatadeque-1.1.3/tests/timing.py`

 * *Files identical despite different names*

