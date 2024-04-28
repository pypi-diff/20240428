# Comparing `tmp/stringdatadeque-1.1.3.tar.gz` & `tmp/stringdatadeque-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringdatadeque-1.1.3.tar", last modified: Sat Apr 27 04:54:42 2024, max compression
+gzip compressed data, was "stringdatadeque-1.2.0.tar", last modified: Sun Apr 28 02:32:49 2024, max compression
```

## Comparing `stringdatadeque-1.1.3.tar` & `stringdatadeque-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.830778 stringdatadeque-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.822778 stringdatadeque-1.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.822778 stringdatadeque-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/gh_pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.github/workflows/tox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43790 2024-04-27 04:54:42.830778 stringdatadeque-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/StringDataDeque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43790 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 04:54:42.000000 stringdatadeque-1.1.3/StringDataDeque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/check_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.818778 stringdatadeque-1.1.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/index.rst.bak
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/docs/source/stringdatadeque.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 04:54:42.830778 stringdatadeque-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.818778 stringdatadeque-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/src/stringdatadeque/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/encryptedstringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18362 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/src/stringdatadeque/stringdatadeque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:54:42.826778 stringdatadeque-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/default.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/test_encryptedssgtringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/test_stringdatadeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-27 04:54:38.000000 stringdatadeque-1.1.3/tests/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:32:49.272399 stringdatadeque-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43831 2024-04-28 02:32:49.268399 stringdatadeque-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:32:49.272399 stringdatadeque-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:32:49.264399 stringdatadeque-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:32:49.268399 stringdatadeque-1.2.0/src/StringDataDeque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43831 2024-04-28 02:32:49.000000 stringdatadeque-1.2.0/src/StringDataDeque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-28 02:32:49.000000 stringdatadeque-1.2.0/src/StringDataDeque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:32:49.000000 stringdatadeque-1.2.0/src/StringDataDeque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-28 02:32:49.000000 stringdatadeque-1.2.0/src/StringDataDeque.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-28 02:32:49.000000 stringdatadeque-1.2.0/src/StringDataDeque.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:32:49.268399 stringdatadeque-1.2.0/src/stringdatadeque/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/src/stringdatadeque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/src/stringdatadeque/encryptedstringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/src/stringdatadeque/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/src/stringdatadeque/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18362 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/src/stringdatadeque/stringdatadeque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:32:49.268399 stringdatadeque-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/tests/test_encryptedssgtringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-28 02:32:45.000000 stringdatadeque-1.2.0/tests/test_stringdatadeque.py
```

### Comparing `stringdatadeque-1.1.3/LICENSE` & `stringdatadeque-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/PKG-INFO` & `stringdatadeque-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.1.3
+Version: 1.2.0
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,14 +702,15 @@
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
+Requires-Dist: pip-audit; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-rtd-size; extra == "docs"
```

### Comparing `stringdatadeque-1.1.3/README.md` & `stringdatadeque-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/StringDataDeque.egg-info/PKG-INFO` & `stringdatadeque-1.2.0/src/StringDataDeque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.1.3
+Version: 1.2.0
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,14 +702,15 @@
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
+Requires-Dist: pip-audit; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-rtd-size; extra == "docs"
```

### Comparing `stringdatadeque-1.1.3/pyproject.toml` & `stringdatadeque-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
+requires = ["setuptools>=67.0", "wheel"]
 
 [project]
 authors = [{"name" = "R.Broderick"}]
 description = "Useful when building a string from data that can be converted into a string, in parts."
-version = "1.1.3"
+version = "1.2.0"
 license = {"file" = "LICENSE"}
 name = "StringDataDeque"
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = ["beartype", "typing-extensions; python_version < '3.12'"]
 requires-python = ">=3.10.0"
 
 [project.optional-dependencies]
@@ -29,15 +29,16 @@
   "packaging",
   "snakeviz",
   "pre-commit",
   "tox",
   "tox-pyenv-redux",
   "pylint",
   "perflint",
-  "snakeviz"
+  "snakeviz",
+  "pip-audit"
 ]
 # pep725
 # [external]
 # build-requires = [
 # "virtual:compiler/rust",
 # "virtual:compiler/cargo",
 # ]
@@ -238,16 +239,17 @@
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"]}
 
 [tool.setuptools.package-data]
 library = ["py.typed"]
 
-[tool.setuptools.packages]
-find = {}
+[tool.setuptools.packages.find]
+exclude = ["docs*", "tests*"]
+where = ["src"]
 
 [tool.sphinx-pyproject]
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 coverage_show_missing_items = true
 extensions = [
   "sphinx.ext.autodoc",
```

### Comparing `stringdatadeque-1.1.3/src/stringdatadeque/__init__.py` & `stringdatadeque-1.2.0/src/stringdatadeque/__init__.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/src/stringdatadeque/encryptedstringdeque.py` & `stringdatadeque-1.2.0/src/stringdatadeque/encryptedstringdeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/src/stringdatadeque/protocols.py` & `stringdatadeque-1.2.0/src/stringdatadeque/protocols.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/src/stringdatadeque/stringdatadeque.py` & `stringdatadeque-1.2.0/src/stringdatadeque/stringdatadeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/tests/test_encryptedssgtringdeque.py` & `stringdatadeque-1.2.0/tests/test_encryptedssgtringdeque.py`

 * *Files identical despite different names*

### Comparing `stringdatadeque-1.1.3/tests/test_stringdatadeque.py` & `stringdatadeque-1.2.0/tests/test_stringdatadeque.py`

 * *Files identical despite different names*

