# Comparing `tmp/quaxed-0.4.tar.gz` & `tmp/quaxed-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr 25 15:09:51 2024, max compression
+gzip compressed data, last modified: Fri Apr 26 20:56:36 2024, max compression
```

## Comparing `quaxed-0.4.tar` & `quaxed-0.4.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      380 2024-04-25 15:09:51.000000 quaxed-0.4/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-04-25 15:09:51.000000 quaxed-0.4/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-25 15:09:51.000000 quaxed-0.4/.gitattributes
--rw-r--r--   0        0        0     2900 2024-04-25 15:09:51.000000 quaxed-0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-25 15:09:51.000000 quaxed-0.4/.readthedocs.yml
--rw-r--r--   0        0        0     2778 2024-04-25 15:09:51.000000 quaxed-0.4/noxfile.py
--rw-r--r--   0        0        0     2387 2024-04-25 15:09:51.000000 quaxed-0.4/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-25 15:09:51.000000 quaxed-0.4/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-25 15:09:51.000000 quaxed-0.4/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1539 2024-04-25 15:09:51.000000 quaxed-0.4/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1641 2024-04-25 15:09:51.000000 quaxed-0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      834 2024-04-25 15:09:51.000000 quaxed-0.4/docs/conf.py
--rw-r--r--   0        0        0      193 2024-04-25 15:09:51.000000 quaxed-0.4/docs/index.md
--rw-r--r--   0        0        0      945 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/__init__.py
--rw-r--r--   0        0        0     1728 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_jax.py
--rw-r--r--   0        0        0      707 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_types.py
--rw-r--r--   0        0        0      231 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_utils.py
--rw-r--r--   0        0        0      406 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_version.py
--rw-r--r--   0        0        0       82 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_version.pyi
--rw-r--r--   0        0        0      620 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/lax.py
--rw-r--r--   0        0        0      407 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/operator.py
--rw-r--r--   0        0        0     2044 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/operator.pyi
--rw-r--r--   0        0        0        0 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/py.typed
--rw-r--r--   0        0        0     1764 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/__init__.py
--rw-r--r--   0        0        0      145 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_constants.py
--rw-r--r--   0        0        0     7849 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_creation_functions.py
--rw-r--r--   0        0        0      894 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_data_type_functions.py
--rw-r--r--   0        0        0      124 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_dispatch.py
--rw-r--r--   0        0        0     6645 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_elementwise_functions.py
--rw-r--r--   0        0        0      293 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_indexing_functions.py
--rw-r--r--   0        0        0      762 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_linear_algebra_functions.py
--rw-r--r--   0        0        0     1722 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_manipulation_functions.py
--rw-r--r--   0        0        0      778 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_searching_functions.py
--rw-r--r--   0        0        0      636 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_set_functions.py
--rw-r--r--   0        0        0      629 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_sorting_functions.py
--rw-r--r--   0        0        0     1925 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_statistical_functions.py
--rw-r--r--   0        0        0      575 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_utility_functions.py
--rw-r--r--   0        0        0     3453 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/fft.py
--rw-r--r--   0        0        0     3726 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/linalg.py
--rw-r--r--   0        0        0      532 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/__init__.py
--rw-r--r--   0        0        0     9218 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_core.py
--rw-r--r--   0        0        0     5767 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_creation_functions.py
--rw-r--r--   0        0        0      106 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_dispatch.py
--rw-r--r--   0        0        0     7533 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_higher_order.py
--rw-r--r--   0        0        0       60 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/fft.py
--rw-r--r--   0        0        0       63 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/linalg.py
--rw-r--r--   0        0        0       84 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/scipy/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/scipy/special.py
--rw-r--r--   0        0        0     1925 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/scipy/special.pyi
--rw-r--r--   0        0        0       21 2024-04-25 15:09:51.000000 quaxed-0.4/tests/__init__.py
--rw-r--r--   0        0        0    38875 2024-04-25 15:09:51.000000 quaxed-0.4/tests/myarray.py
--rw-r--r--   0        0        0      177 2024-04-25 15:09:51.000000 quaxed-0.4/tests/test_package.py
--rw-r--r--   0        0        0       31 2024-04-25 15:09:51.000000 quaxed-0.4/tests/array_api/__init__.py
--rw-r--r--   0        0        0     1710 2024-04-25 15:09:51.000000 quaxed-0.4/tests/array_api/test_jax.py
--rw-r--r--   0        0        0    35919 2024-04-25 15:09:51.000000 quaxed-0.4/tests/array_api/test_myarray.py
--rw-r--r--   0        0        0       27 2024-04-25 15:09:51.000000 quaxed-0.4/tests/numpy/__init__.py
--rw-r--r--   0        0        0    50801 2024-04-25 15:09:51.000000 quaxed-0.4/tests/numpy/test_jax.py
--rw-r--r--   0        0        0     2218 2024-04-25 15:09:51.000000 quaxed-0.4/.gitignore
--rw-r--r--   0        0        0     1528 2024-04-25 15:09:51.000000 quaxed-0.4/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-25 15:09:51.000000 quaxed-0.4/README.md
--rw-r--r--   0        0        0     4291 2024-04-25 15:09:51.000000 quaxed-0.4/pyproject.toml
--rw-r--r--   0        0        0     3287 2024-04-25 15:09:51.000000 quaxed-0.4/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-04-26 20:56:36.000000 quaxed-0.4.1/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-26 20:56:36.000000 quaxed-0.4.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-26 20:56:36.000000 quaxed-0.4.1/.gitattributes
+-rw-r--r--   0        0        0     2942 2024-04-26 20:56:36.000000 quaxed-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-26 20:56:36.000000 quaxed-0.4.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2778 2024-04-26 20:56:36.000000 quaxed-0.4.1/noxfile.py
+-rw-r--r--   0        0        0     2387 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1539 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1641 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      834 2024-04-26 20:56:36.000000 quaxed-0.4.1/docs/conf.py
+-rw-r--r--   0        0        0      193 2024-04-26 20:56:36.000000 quaxed-0.4.1/docs/index.md
+-rw-r--r--   0        0        0     1058 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/__init__.py
+-rw-r--r--   0        0        0     1728 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_jax.py
+-rw-r--r--   0        0        0      707 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_types.py
+-rw-r--r--   0        0        0      231 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_utils.py
+-rw-r--r--   0        0        0      411 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_version.py
+-rw-r--r--   0        0        0       82 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_version.pyi
+-rw-r--r--   0        0        0      620 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/lax.py
+-rw-r--r--   0        0        0      547 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/operator.py
+-rw-r--r--   0        0        0     2044 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/operator.pyi
+-rw-r--r--   0        0        0        0 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/py.typed
+-rw-r--r--   0        0        0     1764 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_constants.py
+-rw-r--r--   0        0        0     7849 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_creation_functions.py
+-rw-r--r--   0        0        0      894 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_data_type_functions.py
+-rw-r--r--   0        0        0      124 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_dispatch.py
+-rw-r--r--   0        0        0     6645 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_elementwise_functions.py
+-rw-r--r--   0        0        0      293 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_indexing_functions.py
+-rw-r--r--   0        0        0      762 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_linear_algebra_functions.py
+-rw-r--r--   0        0        0     1722 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_manipulation_functions.py
+-rw-r--r--   0        0        0      778 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_searching_functions.py
+-rw-r--r--   0        0        0      636 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_set_functions.py
+-rw-r--r--   0        0        0      629 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_sorting_functions.py
+-rw-r--r--   0        0        0     1925 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_statistical_functions.py
+-rw-r--r--   0        0        0      575 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_utility_functions.py
+-rw-r--r--   0        0        0     3453 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/fft.py
+-rw-r--r--   0        0        0     3726 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/linalg.py
+-rw-r--r--   0        0        0      532 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/__init__.py
+-rw-r--r--   0        0        0    16627 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/__init__.pyi
+-rw-r--r--   0        0        0     9490 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_core.py
+-rw-r--r--   0        0        0     5767 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_creation_functions.py
+-rw-r--r--   0        0        0      106 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_dispatch.py
+-rw-r--r--   0        0        0     7533 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_higher_order.py
+-rw-r--r--   0        0        0       60 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/fft.py
+-rw-r--r--   0        0        0       63 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/linalg.py
+-rw-r--r--   0        0        0       84 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/scipy/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/scipy/special.py
+-rw-r--r--   0        0        0     1925 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/scipy/special.pyi
+-rw-r--r--   0        0        0       21 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0    38875 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/myarray.py
+-rw-r--r--   0        0        0      177 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/test_package.py
+-rw-r--r--   0        0        0       31 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/array_api/__init__.py
+-rw-r--r--   0        0        0     1710 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/array_api/test_jax.py
+-rw-r--r--   0        0        0    35919 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/array_api/test_myarray.py
+-rw-r--r--   0        0        0       27 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/numpy/__init__.py
+-rw-r--r--   0        0        0    50679 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/numpy/test_jax.py
+-rw-r--r--   0        0        0     2218 2024-04-26 20:56:36.000000 quaxed-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1528 2024-04-26 20:56:36.000000 quaxed-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-26 20:56:36.000000 quaxed-0.4.1/README.md
+-rw-r--r--   0        0        0     4339 2024-04-26 20:56:36.000000 quaxed-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3289 2024-04-26 20:56:36.000000 quaxed-0.4.1/PKG-INFO
```

### Comparing `quaxed-0.4/.pre-commit-config.yaml` & `quaxed-0.4.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     hooks:
       - id: mypy
         files: src
         additional_dependencies:
           - pytest
         exclude: |
           (?x)^(
+            src/quaxed/numpy/__init__.py|
             src/quaxed/operator.py|
             src/quaxed/scipy/special.py
           )$
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
```

### Comparing `quaxed-0.4/noxfile.py` & `quaxed-0.4.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/.github/CONTRIBUTING.md` & `quaxed-0.4.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/.github/matchers/pylint.json` & `quaxed-0.4.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/.github/workflows/cd.yml` & `quaxed-0.4.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/.github/workflows/ci.yml` & `quaxed-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/docs/conf.py` & `quaxed-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/__init__.py` & `quaxed-0.4.1/src/quaxed/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 quaxed: Array-API JAX compatibility
 """
 
 # pylint: disable=redefined-builtin
 
 __all__ = ["__version__", "array_api"]
 
+import sys
 from typing import Any
 
 import plum
 from jaxtyping import ArrayLike
 
 from . import _jax, array_api
 from ._jax import *
@@ -27,8 +28,13 @@
     """Forward all other attribute accesses to Quaxified JAX."""
     import jax  # pylint: disable=C0415,W0621
     from quax import quaxify  # pylint: disable=C0415,W0621
 
     # TODO: detect if the attribute is a function or a module.
     # If it is a function, quaxify it. If it is a module, return a proxy object
     # that quaxifies all of its attributes.
-    return quaxify(getattr(jax, name))
+    out = quaxify(getattr(jax, name))
+
+    # Cache the function in this module
+    setattr(sys.modules[__name__], name, out)
+
+    return out
```

### Comparing `quaxed-0.4/src/quaxed/_jax.py` & `quaxed-0.4.1/src/quaxed/_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/_types.py` & `quaxed-0.4.1/src/quaxed/_types.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/lax.py` & `quaxed-0.4.1/src/quaxed/lax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/operator.pyi` & `quaxed-0.4.1/src/quaxed/operator.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/__init__.py` & `quaxed-0.4.1/src/quaxed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_creation_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_creation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_data_type_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_data_type_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_elementwise_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_linear_algebra_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_manipulation_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_searching_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_searching_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_set_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_set_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_sorting_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_sorting_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_statistical_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_statistical_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/_utility_functions.py` & `quaxed-0.4.1/src/quaxed/array_api/_utility_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/fft.py` & `quaxed-0.4.1/src/quaxed/array_api/fft.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/array_api/linalg.py` & `quaxed-0.4.1/src/quaxed/array_api/linalg.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/numpy/__init__.py` & `quaxed-0.4.1/src/quaxed/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/numpy/_core.py` & `quaxed-0.4.1/src/quaxed/numpy/_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     "dstack",
     "dtype",
     "e",
     "ediff1d",
     "einsum",
     "einsum_path",
     "empty",
-    "empty_like",
+    # "empty_like",  # in _creation_functions
     "equal",
     "euler_gamma",
     "exp",
     "exp2",
     "expand_dims",
     "expm1",
     "extract",
@@ -160,16 +160,16 @@
     "from_dlpack",
     "frombuffer",
     # "fromfile",
     "fromfunction",
     "fromiter",
     "frompyfunc",
     "fromstring",
-    "full",
-    "full_like",
+    # "full",  # in _creation_functions
+    # "full_like",  # in _creation_functions
     "gcd",
     "generic",
     "geomspace",
     "get_printoptions",
     "gradient",
     "greater",
     "greater_equal",
@@ -223,15 +223,15 @@
     "kron",
     "lcm",
     "ldexp",
     "left_shift",
     "less",
     "less_equal",
     "lexsort",
-    "linspace",
+    # "linspace",  # in _creation_functions
     "load",
     "log",
     "log10",
     "log1p",
     "log2",
     "logaddexp",
     "logaddexp2",
@@ -243,15 +243,15 @@
     "mask_indices",
     "matmul",
     "matrix_transpose",
     "max",
     "maximum",
     "mean",
     "median",
-    "meshgrid",
+    # "meshgrid",  # in _creation_functions
     "mgrid",
     "min",
     "minimum",
     "mod",
     "modf",
     "moveaxis",
     "multiply",
@@ -278,15 +278,15 @@
     "nextafter",
     "nonzero",
     "not_equal",
     "number",
     "object_",
     "ogrid",
     "ones",
-    "ones_like",
+    # "ones_like",  # in _creation_functions
     "outer",
     "packbits",
     "pad",
     "partition",
     "percentile",
     "permute_dims",
     "pi",
@@ -363,19 +363,19 @@
     "tan",
     "tanh",
     "tensordot",
     "tile",
     "trace",
     "transpose",
     "tri",
-    "tril",
+    # "tril",  # in _creation_functions
     "tril_indices",
     "tril_indices_from",
     "trim_zeros",
-    "triu",
+    # "triu",  # in _creation_functions
     "triu_indices",
     "triu_indices_from",
     "true_divide",
     "trunc",
     # "ufunc",  # higher-order function
     "uint",
     "uint16",
@@ -398,15 +398,15 @@
     "vdot",
     "vecdot",
     # "vectorize",
     "vsplit",
     "vstack",
     "where",
     "zeros",
-    "zeros_like",
+    # "zeros_like",  # in _creation_functions
 ]
 
 import sys
 from collections.abc import Callable
 from typing import Any, Literal
 
 import jax.numpy as jnp
@@ -452,14 +452,15 @@
 
 # =============================================================================
 # Automated lazy construction
 
 # Direct transfers
 _DIRECT_TRANSFER: frozenset[str] = frozenset(
     (
+        "bfloat16",
         "character",
         "e",
         "euler_gamma",
         "flexible",
         "floating",
         "generic",
         "index_exp",
```

### Comparing `quaxed-0.4/src/quaxed/numpy/_creation_functions.py` & `quaxed-0.4.1/src/quaxed/numpy/_creation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/numpy/_higher_order.py` & `quaxed-0.4.1/src/quaxed/numpy/_higher_order.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/src/quaxed/scipy/special.py` & `quaxed-0.4.1/src/quaxed/scipy/special.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,16 +50,20 @@
 from collections.abc import Callable
 from typing import Any
 
 from jax.scipy import special as jsp
 from quax import quaxify
 
 
+def __dir__() -> list[str]:
+    return sorted(__all__)
+
+
 # TODO: better return type annotation
 def __getattr__(name: str) -> Callable[..., Any]:
+    # Quaxify the func
     func = quaxify(getattr(jsp, name))
-    setattr(sys.modules[__name__], name, func)
-    return func
 
+    # Cache the function in this module
+    setattr(sys.modules[__name__], name, func)
 
-def __dir__() -> list[str]:
-    return sorted(__all__)
+    return func
```

### Comparing `quaxed-0.4/src/quaxed/scipy/special.pyi` & `quaxed-0.4.1/src/quaxed/scipy/special.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/tests/myarray.py` & `quaxed-0.4.1/tests/myarray.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/tests/array_api/test_jax.py` & `quaxed-0.4.1/tests/array_api/test_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/tests/array_api/test_myarray.py` & `quaxed-0.4.1/tests/array_api/test_myarray.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/tests/numpy/test_jax.py` & `quaxed-0.4.1/tests/numpy/test_jax.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,19 +293,14 @@
 
 
 def test_bartlett():
     """Test `quaxed.numpy.bartlett`."""
     assert jnp.all(qnp.bartlett(3) == jnp.bartlett(3))
 
 
-def test_bfloat16(x1):
-    """Test `quaxed.numpy.bfloat16`."""
-    assert jnp.all(qnp.bfloat16(x1) == jnp.bfloat16(x1))
-
-
 def test_bincount():
     """Test `quaxed.numpy.bincount`."""
     x = jnp.asarray([0, 1, 1, 2, 2, 2])
     assert jnp.all(qnp.bincount(x) == jnp.bincount(x))
 
 
 def test_bitwise_and(xbool):
```

### Comparing `quaxed-0.4/.gitignore` & `quaxed-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/LICENSE` & `quaxed-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/README.md` & `quaxed-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.4/pyproject.toml` & `quaxed-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 """
 
 
 [tool.coverage]
 run.source = ["quaxed"]
 port.exclude_lines = ['pragma: no cover', '\.\.\.', 'if typing.TYPE_CHECKING:']
 
+
 [tool.mypy]
 files = ["src"]
 python_version = "3.10"
 warn_unused_configs = true
 strict = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
@@ -143,9 +144,10 @@
 messages_control.disable = [
     "design",
     "fixme",
     "line-too-long",
     "missing-function-docstring", # TODO: reinstate.
     "missing-module-docstring",
     "redefined-builtin",
+    "useless-import-alias",  # handled by ruff
     "wrong-import-position",
 ]
```

### Comparing `quaxed-0.4/PKG-INFO` & `quaxed-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quaxed
-Version: 0.4
+Version: 0.4.1
 Summary: Array-API JAX compatibility
 Project-URL: Homepage, https://github.com/GalacticDynamics/quaxed
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/quaxed/issues
 Project-URL: Discussions, https://github.com/GalacticDynamics/quaxed/discussions
 Project-URL: Changelog, https://github.com/GalacticDynamics/quaxed/releases
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License-File: LICENSE
```

