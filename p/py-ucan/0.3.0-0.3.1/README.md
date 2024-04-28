# Comparing `tmp/py_ucan-0.3.0.tar.gz` & `tmp/py_ucan-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ucan-0.3.0.tar", max compression
+gzip compressed data, was "py_ucan-0.3.1.tar", max compression
```

## Comparing `py_ucan-0.3.0.tar` & `py_ucan-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-04-27 10:53:59.719839 py_ucan-0.3.0/LICENSE
--rw-r--r--   0        0        0       10 2024-04-27 10:53:59.719839 py_ucan-0.3.0/README.md
--rw-r--r--   0        0        0    10294 2024-04-27 10:54:00.675832 py_ucan-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1630 2024-04-27 10:54:00.683832 py_ucan-0.3.0/src/ucan/__init__.py
--rw-r--r--   0        0        0      744 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/constants.py
--rw-r--r--   0        0        0       30 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/__init__.py
--rw-r--r--   0        0        0     6739 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/attenuation.py
--rw-r--r--   0        0        0     1754 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/plugins.py
--rw-r--r--   0        0        0     1484 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/semver.py
--rw-r--r--   0        0        0     6735 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/token.py
--rw-r--r--   0        0        0     4284 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/types.py
--rw-r--r--   0        0        0     5889 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/verify.py
--rw-r--r--   0        0        0      181 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/default_plugins/__init__.py
--rw-r--r--   0        0        0     2851 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/default_plugins/ed25519.py
--rw-r--r--   0        0        0        0 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/py.typed
--rw-r--r--   0        0        0      914 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/schemas.py
--rw-r--r--   0        0        0      205 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/typing.py
--rw-r--r--   0        0        0     2192 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/utils.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 py_ucan-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-27 11:06:17.782066 py_ucan-0.3.1/LICENSE
+-rw-r--r--   0        0        0       10 2024-04-27 11:06:17.782066 py_ucan-0.3.1/README.md
+-rw-r--r--   0        0        0    10293 2024-04-27 11:06:19.634090 py_ucan-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1630 2024-04-27 11:06:19.642090 py_ucan-0.3.1/src/ucan/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/constants.py
+-rw-r--r--   0        0        0       30 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/__init__.py
+-rw-r--r--   0        0        0     6739 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/attenuation.py
+-rw-r--r--   0        0        0     1754 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/plugins.py
+-rw-r--r--   0        0        0     1484 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/semver.py
+-rw-r--r--   0        0        0     6735 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/token.py
+-rw-r--r--   0        0        0     4284 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/types.py
+-rw-r--r--   0        0        0     5889 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/verify.py
+-rw-r--r--   0        0        0      181 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2851 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/default_plugins/ed25519.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/py.typed
+-rw-r--r--   0        0        0      914 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/schemas.py
+-rw-r--r--   0        0        0      205 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/typing.py
+-rw-r--r--   0        0        0     2192 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/utils.py
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 py_ucan-0.3.1/PKG-INFO
```

### Comparing `py_ucan-0.3.0/LICENSE` & `py_ucan-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/pyproject.toml` & `py_ucan-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # ----------------------------------------------------------------------------------------------------------------------
 # poetry
 [tool.poetry]
 package-mode = true
 name = "py-ucan"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python Ucan"
 readme = "README.md"
 authors = [
     "Subham Agarwal <subhamagr@users.noreply.github.com>",
 ]
 maintainers = []
 # links
@@ -44,21 +44,21 @@
 python = "^3.10"
 typing_extensions = "4.10.0"
 pydantic = "2.7.1"
 pydantic-settings = "2.2.1"
 cryptography = "42.0.5"
 base58 = "2.1.1"
 pyjwt = "2.8.0"
-pytest-asyncio = "^0.23.6"
 
 [tool.poetry.group.release.dependencies]
 python-semantic-release = "9.5.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "8.1.1"
+pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
 
 [tool.poetry.group.qa.dependencies]
 mypy = "1.9.0"
 ruff = "0.4.1"
 
 [tool.poetry.urls]
```

### Comparing `py_ucan-0.3.0/src/ucan/__init__.py` & `py_ucan-0.3.1/src/ucan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ucan.core import attenuation as attenuationlib
 from ucan.core import token as tokenlib
 from ucan.core import verify as verifylib
 from ucan.core.plugins import Plugins
 from ucan.default_plugins import ed25519_plugin, EdKeypair
 
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 __all__ = (
     "Plugins",
     "PluginInjectedAPI",
     "default_plugins",
     "injected_api",
```

### Comparing `py_ucan-0.3.0/src/ucan/constants.py` & `py_ucan-0.3.1/src/ucan/constants.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/core/attenuation.py` & `py_ucan-0.3.1/src/ucan/core/attenuation.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/core/plugins.py` & `py_ucan-0.3.1/src/ucan/core/plugins.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/core/semver.py` & `py_ucan-0.3.1/src/ucan/core/semver.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/core/token.py` & `py_ucan-0.3.1/src/ucan/core/token.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/core/types.py` & `py_ucan-0.3.1/src/ucan/core/types.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/core/verify.py` & `py_ucan-0.3.1/src/ucan/core/verify.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/default_plugins/ed25519.py` & `py_ucan-0.3.1/src/ucan/default_plugins/ed25519.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/schemas.py` & `py_ucan-0.3.1/src/ucan/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/src/ucan/utils.py` & `py_ucan-0.3.1/src/ucan/utils.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.0/PKG-INFO` & `py_ucan-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ucan
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Ucan
 Home-page: https://github.com/fileverse/py-ucan
 Author: Subham Agarwal
 Author-email: subhamagr@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: base58 (==2.1.1)
 Requires-Dist: cryptography (==42.0.5)
 Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: pydantic-settings (==2.2.1)
 Requires-Dist: pyjwt (==2.8.0)
-Requires-Dist: pytest-asyncio (>=0.23.6,<0.24.0)
 Requires-Dist: typing_extensions (==4.10.0)
 Project-URL: Bug Tracker, https://github.com/fileverse/py-ucan/issues
 Project-URL: Documentation, https://github.com/fileverse/py-ucan
 Project-URL: Repository, https://github.com/fileverse/py-ucan
 Description-Content-Type: text/markdown
 
 # py-ucan
```

