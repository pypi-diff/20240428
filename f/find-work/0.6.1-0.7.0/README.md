# Comparing `tmp/find_work-0.6.1.tar.gz` & `tmp/find_work-0.7.0.tar.gz`

## Comparing `find_work-0.6.1.tar` & `find_work-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,45 @@
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 find_work-0.6.1/Makefile
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/conf.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/configuration.rst
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/contributing.rst
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/getting-started.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/index.rst
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/installation.rst
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/release-notes.rst
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/toc.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-alt.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-alt.svg.license
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-button.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-button.html.license
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/__main__.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cache.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/config.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/py.typed
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/types.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/utils.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/__init__.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/bugzilla.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/execute.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/pgo.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/pkgcheck.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/repology.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/data/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/data/default_config.toml
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 find_work-0.6.1/man/find-work.1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_bugzilla.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_cache.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_config.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_repology.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/cassettes/test_bugzilla/test_bugs_json_roundtrip.yaml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/alias_sample.toml
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/bug74072.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/bug74072.json.license
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/flag_sample.toml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 find_work-0.6.1/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 find_work-0.6.1/LICENSE
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 find_work-0.6.1/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 find_work-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 find_work-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 find_work-0.7.0/Makefile
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/configuration.rst
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/contributing.rst
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/getting-started.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/installation.rst
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/release-notes.rst
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/toc.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/_templates/git-alt.svg
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/_templates/git-alt.svg.license
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/_templates/git-button.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 find_work-0.7.0/docs/_templates/git-button.html.license
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/__main__.py
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cache.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/config.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/py.typed
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/utils.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cli/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cli/bugzilla.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cli/execute.py
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cli/pgo.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cli/pkgcheck.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/cli/repology.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/data/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/data/default_config.toml
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/types/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/types/_config.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 find_work-0.7.0/find_work/types/_pgo.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 find_work-0.7.0/man/find-work.1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 find_work-0.7.0/tests/test_cache.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 find_work-0.7.0/tests/test_config.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 find_work-0.7.0/tests/test_repology.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 find_work-0.7.0/tests/data/alias_sample.toml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 find_work-0.7.0/tests/data/flag_sample.toml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 find_work-0.7.0/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 find_work-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 find_work-0.7.0/README.md
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 find_work-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 find_work-0.7.0/PKG-INFO
```

### Comparing `find_work-0.6.1/Makefile` & `find_work-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/conf.py` & `find_work-0.7.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'find-work'
 author = 'Anna (cybertailor) Vyalkova'
 copyright = f'2024, {author}'
-release = '0.6.1'
+release = '0.7.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.extlinks',
     'sphinx.ext.intersphinx',
```

### Comparing `find_work-0.6.1/docs/configuration.rst` & `find_work-0.7.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/contributing.rst` & `find_work-0.7.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/getting-started.rst` & `find_work-0.7.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/index.rst` & `find_work-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/installation.rst` & `find_work-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/release-notes.rst` & `find_work-0.7.0/docs/release-notes.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,136 @@
 .. SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 .. SPDX-License-Identifier: WTFPL
 .. No warranty.
 
 Release Notes
 =============
 
+0.7.0
+-----
+
+- **New**: Filter oudated packages by version part (:bug:`4`).
+
+- Use Pydantic models to load and serialize caches. This could have better
+  perfomance and correctness but also introduce new bugs.
+
+*Modules changelog:*
+
+- **bugzilla**:
+
+  - Switch to REST API from XMLRPC.
+
+- **pgo**:
+
+  - **outdated**:
+
+    - Improve error text for trying to filter by maintainer (:bug:`3`).
+
 0.6.1
 -----
 
-* [pkgcheck/scan]: drop ``--quiet`` flag. Before pkgcheck v0.10.21, this option
-  was used only in pkgcore internals. Now it's used to filter out non-error
-  results from pkgcheck.
+*Modules changelog:*
+
+- **pkgcheck**:
+
+  - **scan**:
+
+    - Drop ``--quiet`` flag. Before pkgcheck v0.10.21, this option was used
+      only in pkgcore internals. Now it's used to filter out non-error results
+      from pkgcheck.
 
 0.6.0
 -----
 
-* **New:** Define custom global flags to override global options.
+- **New:** Define custom global flags to override global options.
+
+*Modules changelog:*
 
-* **New:** Filter ``pkgcheck`` results by keyword or message.
+- **pkgcheck**:
 
-* Silence pkgcore warnings and pkgcheck status messages.
+  - **New:** Filter results by keyword or message.
+
+  - Silence pkgcore warnings and pkgcheck status messages.
 
 0.5.0
 -----
 
-* **New:** Scan repository for QA issues (command: ``pkgcheck scan``).
+- **New:** Scan repository for QA issues (command: ``pkgcheck scan``).
 
-* Fix caching with maintainer filter applied.
+- Fix caching with maintainer filter applied.
 
-* Dependencies introduced:
+*Dependencies introduced:*
 
-  * :pypi:`pkgcheck`
+* :pypi:`pkgcheck`
 
 0.4.0
 -----
 
-* **New:** Execute custom aliases.
+- **New:** Execute custom aliases.
 
-* **New:** List all bugs on Bugzilla (command: ``bugzilla list``).
+- **New:** List all bugs on Bugzilla (command: ``bugzilla list``).
 
-* **Gone:** ``bugzilla outdated`` is now ``execute bump-requests``.
+- **Gone:** ``bugzilla outdated`` is now ``execute bump-requests``.
 
-* **Gone:** Python 3.10 support.
+- **Gone:** Python 3.10 support.
 
-* Fix parsing atoms that contain revision.
+- Fix parsing atoms that contain revision.
 
-* Dependencies introduced:
+*Dependencies introduced:*
 
-  * :pypi:`deepmerge`
-  * :pypi:`platformdirs`
+* :pypi:`deepmerge`
+* :pypi:`platformdirs`
 
 0.3.0
 -----
 
-* **New:** Discover version bump requests on Bugzilla (command: ``bugzilla
+- **New:** Discover version bump requests on Bugzilla (command: ``bugzilla
   outdated``).
 
-* **New:** Discover outdated packages in the Gentoo repository (command: ``pgo
+- **New:** Discover outdated packages in the Gentoo repository (command: ``pgo
   outdated``).
 
-* **New:** Discover stabilization candidates in the Gentoo repository (command:
+- **New:** Discover stabilization candidates in the Gentoo repository (command:
   ``pgo stabilization``).
 
-* **New:** Filter results by maintainer.
+- **New:** Filter results by maintainer.
 
-* Dependencies introduced:
+*Dependencies introduced:*
 
-  * :pypi:`python-bugzilla`
-  * :pypi:`requests`
-  * :pypi:`tabulate`
-  * :pypi:`pytest-recording` *(test)*
+* :pypi:`python-bugzilla`
+* :pypi:`requests`
+* :pypi:`tabulate`
+* :pypi:`pytest-recording` *(test)*
 
 0.2.0
 -----
 
-* Add progress indication with the option to disable it.
+- Add progress indication with the option to disable it.
+
+- Support ``NO_COLOR`` variable in addition to ``NOCOLOR``.
 
-* Support ``NO_COLOR`` variable in addition to ``NOCOLOR``.
+*Modules changelog:*
 
-* [repology/outdated]: fix :bug:`2`, where different packages of the same
-  projects crashed the utility.
+- **repology**:
 
-* [repology/outdated]: use ``origversion`` if defined to prevent crashes.
+  - **outdated**:
+
+    - Fix :bug:`2`, where different packages of the same project crashed the
+      utility.
+
+    - Use ``origversion`` if defined to prevent crashes.
 
 0.1.1
 -----
 
-* [repology/outdated]: print latest of packaged version instead of a random one.
+*Modules changelog:*
+
+- **repology**:
+
+  - **outdated**:
+
+    - Output the latest of packaged versions instead of a choosing a random one.
 
 0.1.0
 -----
 
-* First release.
+- First release.
```

### Comparing `find_work-0.6.1/docs/toc.rst` & `find_work-0.7.0/docs/toc.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/docs/_templates/git-alt.svg` & `find_work-0.7.0/docs/_templates/git-alt.svg`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/find_work/__main__.py` & `find_work-0.7.0/find_work/__main__.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/find_work/cache.py` & `find_work-0.7.0/find_work/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 # No warranty
 
 """ Implementation of caching functionality. """
 
 import hashlib
-import json
 import tempfile
 from pathlib import Path
-from typing import Any
+from typing import Any, SupportsBytes
 
-from pydantic.dataclasses import dataclass
+from pydantic import BaseModel, PrivateAttr
 
 from find_work.constants import PACKAGE
 
 
-@dataclass
-class CacheKey:
+class CacheKey(BaseModel):
     """
     Cache key constructor.
 
     >>> key = CacheKey()
     >>> key.feed(b"bytes")
     True
     >>> key.feed("string")
@@ -37,15 +35,15 @@
     b'bytes\\x00string\\x00count:42\\x00flag:1\\x00keywords:amazing\\x19wow\\x00'
     >>> key.feed({1, 2, 3})
     Traceback (most recent call last):
         ...
     TypeError: Unsupported type: set
     """
 
-    data: bytes = b""
+    _data: bytes = PrivateAttr(default=b"")
 
     @staticmethod
     def _unsupported_type(value: Any) -> TypeError:
         return TypeError(f"Unsupported type: {type(value).__name__}")
 
     @classmethod
     def _encode(cls, value: Any) -> bytes:
@@ -80,71 +78,72 @@
         Update the key with new data.
 
         :return: ``True`` if data was accepted, ``False`` otherwise
         """
 
         accepted: bool = False
         for value in filter(self._feedable, args):
-            self.data += self._encode(value) + b"\0"
+            self._data += self._encode(value) + b"\0"
             accepted = True
         return accepted
 
     def feed_option(self, key: str, value: Any) -> bool:
         """
         Update the key with new key-value data.
 
         :return: ``True`` if data was accepted, ``False`` otherwise
         """
 
         if self._feedable(value):
-            self.data += self._encode(key) + b":"
-            self.data += self._encode(value) + b"\0"
+            self._data += self._encode(key) + b":"
+            self._data += self._encode(value) + b"\0"
             return True
         return False
 
     def __bytes__(self) -> bytes:
-        return self.data
+        return self._data
 
 
-def _get_cache_path(cache_key: bytes) -> Path:
-    hexdigest = hashlib.sha256(cache_key).hexdigest()
+def _get_cache_path(cache_key: SupportsBytes) -> Path:
+    hexdigest = hashlib.sha256(bytes(cache_key)).hexdigest()
     file = Path(tempfile.gettempdir()) / PACKAGE / hexdigest
     return file.with_suffix(".json")
 
 
-def write_json_cache(data: Any, cache_key: CacheKey, **kwargs: Any) -> None:
+def write_raw_json_cache(data: SupportsBytes, cache_key: SupportsBytes) -> None:
     """
-    Write a JSON cache file in a temporary directory. Keyword arguments are
-    passed to :py:function:`json.dump` as is.
+    Write a JSON cache file in a temporary directory.
 
-    :param data: data to serialize
+    This function silently fails on OS errors.
+
+    :param data: raw JSON
     :param cache_key: cache key object
     """
 
-    cache = _get_cache_path(bytes(cache_key))
+    cache = _get_cache_path(cache_key)
     try:
         cache.parent.mkdir(parents=True, exist_ok=True)
     except OSError:
         return
 
-    with open(cache, "w") as file:
+    with open(cache, "wb") as file:
         try:
-            json.dump(data, file, **kwargs)
+            file.write(bytes(data))
         except OSError:
             pass
 
 
-def read_json_cache(cache_key: CacheKey, **kwargs: Any) -> Any | None:
+def read_raw_json_cache(cache_key: SupportsBytes) -> bytes:
     """
-    Read a JSON cache file stored in a temporary directory. Keyword arguments
-    are passed to :py:function:`json.load` as is.
+    Read a JSON cache file stored in a temporary directory.
 
     :param cache_key: cache key object
-    :return: decoded data or ``None``
+
+    :return: raw JSON file contents or empty byte string
     """
 
-    cache = _get_cache_path(bytes(cache_key))
+    cache = _get_cache_path(cache_key)
     if not cache.is_file():
-        return None
+        return b""
 
-    with open(cache) as file:
-        return json.load(file, **kwargs)
+    with open(cache, "rb") as file:
+        return file.read()
```

### Comparing `find_work-0.6.1/find_work/config.py` & `find_work-0.7.0/find_work/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import gentoopm
 from deepmerge import always_merger
 from platformdirs import PlatformDirs
 
 import find_work.data
 from find_work.constants import DEFAULT_CONFIG, ENTITY, PACKAGE
-from find_work.types import CliOptionKind
+from find_work.types._config import CliOptionKind
 
 
 # FIXME: Find out how to use Pydantic for type validation
 class ConfigBase(ABC):
     """ Base class for all configuration objects. """
 
     _obj: dict
```

### Comparing `find_work-0.6.1/find_work/constants.py` & `find_work-0.7.0/find_work/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """ All important constants in one place. """
 
 # Application package name.
 PACKAGE = "find-work"
 
 # Application version.
-VERSION = "0.6.1"
+VERSION = "0.7.0"
 
 # Application homepage.
 HOMEPAGE = "https://find-work.sysrq.in"
 
 # Application affiliation.
 ENTITY = "sysrq.in"
```

### Comparing `find_work-0.6.1/find_work/utils.py` & `find_work-0.7.0/find_work/utils.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/find_work/cli/__init__.py` & `find_work-0.7.0/find_work/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,17 @@
     def __setitem__(self, key: str, value: Any) -> None:
         setattr(self, key, value)
 
 
 class ModuleOptionsBase(OptionsBase, ABC):
     """ Base class for module-specific options. """
 
+    #: Extra options used in the command scope.
+    extra_options: dict[str, Any] | None = None
+
     @property
     @abstractmethod
     def cache_order(self) -> list[str]:
         ...
 
 
 @dataclass
@@ -92,14 +95,23 @@
 
     @cached_property
     def cache_order(self) -> list[str]:
         return ["chronological_sort", "short_desc", "product", "component"]
 
 
 @dataclass
+class PgoOptions(ModuleOptionsBase):
+    """ Gentoo Packages subcommand options. """
+
+    @cached_property
+    def cache_order(self) -> list[str]:
+        return []
+
+
+@dataclass
 class PkgcheckOptions(ModuleOptionsBase):
     """ pkgcheck subcommand options. """
 
     # Repository name or absolute path.
     repo: str = ""
 
     # Class of the pkgcheck warning, e.g. DeprecatedEapi
@@ -151,16 +163,17 @@
 
     # Filter installed packages only
     only_installed: bool = False
 
     # Byte string used for creating cache key.
     cache_key: CacheKey = field(default_factory=CacheKey)
 
-    # Subcommand options.
+    #: Subcommand options.
     bugzilla: BugzillaOptions = field(default_factory=BugzillaOptions)
+    pgo: PgoOptions = field(default_factory=PgoOptions)
     pkgcheck: PkgcheckOptions = field(default_factory=PkgcheckOptions)
     repology: RepologyOptions = field(default_factory=RepologyOptions)
 
     @staticmethod
     def echo(*args: Any, **kwargs: Any) -> None:
         """
         Simple alias to :py:function:`click.echo`.
```

### Comparing `find_work-0.6.1/find_work/cli/bugzilla.py` & `find_work-0.7.0/find_work/cli/bugzilla.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 # No warranty
 
 """
 CLI subcommands for everything Bugzilla.
-
-This Python module also defines some regular expressions.
-
-``isodate_re`` matches ISO 8601 time/date strings:
-
->>> isodate_re.fullmatch("2024") is None
-True
->>> isodate_re.fullmatch("20090916T09:04:18") is None
-False
 """
 
-import json
-import re
-import time
 import warnings
-from collections.abc import Iterable
+from collections.abc import Collection
+from datetime import datetime
 from typing import Any
-from xmlrpc.client import DateTime
 
 import click
 import gentoopm
+import pydantic_core
 from tabulate import tabulate
 
 from find_work.cache import (
-    read_json_cache,
-    write_json_cache,
+    read_raw_json_cache,
+    write_raw_json_cache,
 )
 from find_work.cli import Message, Options, ProgressDots
 from find_work.constants import BUGZILLA_URL
 from find_work.types import BugView
 from find_work.utils import (
     extract_package_name,
     requests_session,
@@ -41,103 +30,86 @@
 
 with warnings.catch_warnings():
     # Disable annoying warning shown to LibreSSL users
     warnings.simplefilter("ignore")
     import bugzilla
     from bugzilla.bug import Bug
 
-isodate_re = re.compile(r"\d{4}\d{2}\d{2}T\d{2}:\d{2}:\d{2}")
-
-
-class BugEncoder(json.JSONEncoder):
-    def default(self, o: Any) -> Any:
-        if isinstance(o, DateTime):
-            return o.value
-        return json.JSONEncoder.default(self, o)
-
-
-def as_datetime(obj: dict) -> dict:
-    result: dict = {}
-    for key, value in obj.items():
-        # FIXME: every matching string will be converted to DateTime
-        if isinstance(value, str) and isodate_re.fullmatch(value):
-            result[key] = DateTime(value)
-            continue
-        result[key] = value
-    return result
-
 
-def _bugs_from_json(data: list[dict]) -> list[Bug]:
+def _bugs_from_raw_json(raw_json: str | bytes) -> list[Bug]:
+    data: list[dict] = pydantic_core.from_json(raw_json)
     with requests_session() as session:
-        bz = bugzilla.Bugzilla(BUGZILLA_URL, requests_session=session)
+        bz = bugzilla.Bugzilla(BUGZILLA_URL, requests_session=session,
+                               force_rest=True)
         return [Bug(bz, dict=bug) for bug in data]
 
 
-def _bugs_to_json(data: Iterable[Bug]) -> list[dict]:
-    return [bug.get_raw_data() for bug in data]
+def _bugs_to_raw_json(data: Collection[Bug]) -> bytes:
+    raw_data = [bug.get_raw_data() for bug in data]
+    return pydantic_core.to_json(raw_data, exclude_none=True)
 
 
 def _fetch_bugs(options: Options, **kwargs: Any) -> list[Bug]:
     with requests_session() as session:
-        bz = bugzilla.Bugzilla(BUGZILLA_URL, requests_session=session)
+        bz = bugzilla.Bugzilla(BUGZILLA_URL, requests_session=session,
+                               force_rest=True)
         query = bz.build_query(
             short_desc=options.bugzilla.short_desc or None,
             product=options.bugzilla.product or None,
             component=options.bugzilla.component or None,
             assigned_to=options.maintainer or None,
         )
         query["resolution"] = "---"
         if options.bugzilla.chronological_sort:
             query["order"] = "changeddate DESC"
         else:
             query["order"] = "bug_id DESC"
         return bz.query(query)
 
 
-def _collect_bugs(data: Iterable[Bug], options: Options) -> list[BugView]:
+def _collect_bugs(data: Collection[Bug], options: Options) -> list[BugView]:
     if options.only_installed:
         pm = gentoopm.get_package_manager()
 
     result: list[BugView] = []
     for bug in data:
         if options.only_installed:
             if (package := extract_package_name(bug.summary)) is None:
                 continue
             if package not in pm.installed:
                 continue
 
-        date = time.strftime("%F", bug.last_change_time.timetuple())
+        date = datetime.fromisoformat(bug.last_change_time).date().isoformat()
         item = BugView(bug.id, date, bug.assigned_to, bug.summary)
         result.append(item)
     return result
 
 
 def _list_bugs(cmd: str, options: Options, **filters: Any) -> None:
     options.cache_key.feed(cmd)
     dots = ProgressDots(options.verbose)
 
     options.say(Message.CACHE_LOAD)
     with dots():
-        cached_data = read_json_cache(options.cache_key,
-                                      object_hook=as_datetime)
-    if cached_data is not None:
+        raw_data = read_raw_json_cache(options.cache_key)
+    if raw_data:
         options.say(Message.CACHE_READ)
         with dots():
-            data = _bugs_from_json(cached_data)
+            data = _bugs_from_raw_json(raw_data)
     else:
         options.vecho("Fetching data from Bugzilla API", nl=False, err=True)
         with dots():
             data = _fetch_bugs(options, **filters)
         if len(data) == 0:
             options.say(Message.EMPTY_RESPONSE)
             return
         options.say(Message.CACHE_WRITE)
         with dots():
-            json_data = _bugs_to_json(data)
-            write_json_cache(json_data, options.cache_key, cls=BugEncoder)
+            raw_json = _bugs_to_raw_json(data)
+            write_raw_json_cache(raw_json, options.cache_key)
 
     bumps = _collect_bugs(data, options)
     if len(bumps) != 0:
         options.echo(tabulate(bumps, tablefmt="plain"))  # type: ignore
     else:
         options.say(Message.NO_WORK)
```

### Comparing `find_work-0.6.1/find_work/cli/execute.py` & `find_work-0.7.0/find_work/cli/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Any
 
 import click
 from click_aliases import ClickAliasedGroup
 
 from find_work.cli import Options
 from find_work.config import ConfigAlias, ConfigModuleOption, load_config
-from find_work.types import CliOptionKind
+from find_work.types._config import CliOptionKind
 
 
 def _new_click_option(opt: ConfigModuleOption) -> Callable:
 
     def callback(ctx: click.Context, param: str, value: Any) -> None:
         options: Options = ctx.obj
         options[opt.module][opt.name] = value
```

### Comparing `find_work-0.6.1/find_work/cli/pgo.py` & `find_work-0.7.0/find_work/cli/pgo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,181 +1,229 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 # No warranty
 
 """ CLI subcommands for Gentoo Packages website. """
 
 import asyncio
-from collections.abc import Iterable
 
 import click
 import gentoopm
+from pydantic import TypeAdapter
 from sortedcontainers import SortedDict, SortedSet
 from tabulate import tabulate
 
 from find_work.cache import (
-    read_json_cache,
-    write_json_cache,
+    read_raw_json_cache,
+    write_raw_json_cache,
+)
+from find_work.cli import (
+    Message,
+    Options,
+    ProgressDots,
+)
+from find_work.constants import (
+    PGO_BASE_URL,
+    PGO_API_URL,
+)
+from find_work.types import (
+    VersionBump,
+    VersionPart,
+)
+from find_work.types._pgo import (
+    GraphQlResponse,
+    OutdatedPackage,
+    PkgCheckResult,
+    StableCandidate,
 )
-from find_work.cli import Message, Options, ProgressDots
-from find_work.constants import PGO_BASE_URL, PGO_API_URL
-from find_work.types import VersionBump
 from find_work.utils import aiohttp_session
 
+OutdatedPackageSet = frozenset[OutdatedPackage]
+PkgCheckResultSet = frozenset[PkgCheckResult]
+StableCandidateSet = frozenset[StableCandidate]
+
 
-async def _fetch_outdated() -> list[dict]:
+async def _fetch_outdated() -> OutdatedPackageSet:
     query = """query {
         outdatedPackages{
             Atom
             GentooVersion
             NewestVersion
         }
     }"""
 
     async with aiohttp_session() as session:
         async with session.post(PGO_API_URL, json={"query": query},
                                 raise_for_status=True) as response:
-            data = await response.json()
-    return data.get("data", {}).get("outdatedPackages", [])
+            raw_data = await response.read()
 
+    graphql = GraphQlResponse.model_validate_json(raw_data)
+    return graphql.data.outdated
 
-def _collect_version_bumps(data: Iterable[dict],
+
+def _collect_version_bumps(data: OutdatedPackageSet,
                            options: Options) -> SortedSet[VersionBump]:
     if options.only_installed:
         pm = gentoopm.get_package_manager()
 
     result: SortedSet[VersionBump] = SortedSet()
     for item in data:
-        bump = VersionBump(item["Atom"],
-                           item.get("GentooVersion", "(unknown)"),
-                           item.get("NewestVersion", "(unknown)"))
-
-        if options.only_installed and bump.atom not in pm.installed:
+        if options.only_installed and item.atom not in pm.installed:
             continue
-        result.add(bump)
+        result.add(item.as_version_bump)
     return result
 
 
 async def _outdated(options: Options) -> None:
     if options.maintainer:
-        raise NotImplementedError("-m option is not implemented for this command")
+        raise NotImplementedError(
+            "Filtering by maintainer is not implemented for this command"
+        )
+
+    if (extra_options := options.pgo.extra_options) is not None:
+        version_part: VersionPart | None = extra_options.get("version_part")
 
     dots = ProgressDots(options.verbose)
 
     options.say(Message.CACHE_LOAD)
     with dots():
-        data = read_json_cache(options.cache_key)
-    if data is None:
+        raw_data = read_raw_json_cache(options.cache_key)
+    if raw_data:
+        options.say(Message.CACHE_READ)
+        with dots():
+            data = TypeAdapter(OutdatedPackageSet).validate_json(raw_data)
+    else:
         options.vecho("Fetching data from Gentoo Packages API",
                       nl=False, err=True)
         with dots():
             data = await _fetch_outdated()
         if len(data) == 0:
             options.say(Message.EMPTY_RESPONSE)
             return
         options.say(Message.CACHE_WRITE)
         with dots():
-            write_json_cache(data, options.cache_key)
+            raw_json = TypeAdapter(OutdatedPackageSet).dump_json(
+                data, by_alias=True, exclude_none=True
+            )
+            write_raw_json_cache(raw_json, options.cache_key)
+
+    no_work = True
+    for bump in _collect_version_bumps(data, options):
+        if version_part and not bump.changed(version_part):
+            continue
 
-    outdated_set = _collect_version_bumps(data, options)
-    for bump in outdated_set:
         options.echo(bump.atom + " ", nl=False)
         options.secho(bump.old_version, fg="red", nl=False)
         options.echo(" → ", nl=False)
         options.secho(bump.new_version, fg="green")
+        no_work = False
 
-    if len(outdated_set) == 0:
+    if no_work:
         options.say(Message.NO_WORK)
 
 
-async def _fetch_maintainer_stabilization(maintainer: str) -> list[dict]:
-    url = f"{PGO_BASE_URL}/maintainer/{maintainer}/stabilization.json"
+async def _fetch_maintainer_stabilization(maintainer: str) -> PkgCheckResultSet:
+
+    url = PGO_BASE_URL + f"/maintainer/{maintainer}/stabilization.json"
     async with aiohttp_session() as session:
         async with session.get(url, raise_for_status=True) as response:
-            data = await response.json()
+            raw_data = await response.read()
 
-    # bring data to a common structure
-    return [
-        {
-            "Atom": f"{item['category']}/{item['package']}",
-            "Version": item["version"],
-            "Message": item["message"],
-        }
-        for item in data
-    ]
+    data = TypeAdapter(StableCandidateSet).validate_json(raw_data)
+    return frozenset(item.as_pkgcheck_result for item in data)
 
 
-async def _fetch_all_stabilization() -> list[dict]:
+async def _fetch_all_stabilization() -> PkgCheckResultSet:
     query = """query {
         pkgCheckResults(Class: "StableRequest") {
             Atom
             Version
             Message
         }
     }"""
 
     async with aiohttp_session() as session:
         async with session.post(PGO_API_URL, json={"query": query},
                                 raise_for_status=True) as response:
-            data = await response.json()
-    return data.get("data", {}).get("pkgCheckResults", [])
+            raw_data = await response.read()
 
+    graphql = GraphQlResponse.model_validate_json(raw_data)
+    return graphql.data.pkgcheck
 
-async def _fetch_stabilization(options: Options) -> list[dict]:
+
+async def _fetch_stabilization(options: Options) -> PkgCheckResultSet:
     if options.maintainer:
         return await _fetch_maintainer_stabilization(options.maintainer)
     return await _fetch_all_stabilization()
 
 
-def _collect_stable_candidates(data: list[dict],
+def _collect_stable_candidates(data: PkgCheckResultSet,
                                options: Options) -> SortedDict[str, str]:
     if options.only_installed:
         pm = gentoopm.get_package_manager()
 
     result: SortedDict[str, str] = SortedDict()
     for item in data:
-        if options.only_installed and item["Atom"] not in pm.installed:
+        if options.only_installed and item.atom not in pm.installed:
             continue
-        key = "-".join([item["Atom"], item["Version"]])
-        result[key] = item["Message"]
+        key = "-".join([item.atom, item.version])
+        result[key] = item.message
     return result
 
 
 async def _stabilization(options: Options) -> None:
     dots = ProgressDots(options.verbose)
 
     options.say(Message.CACHE_LOAD)
     with dots():
-        data = read_json_cache(options.cache_key)
-    if data is None:
+        raw_data = read_raw_json_cache(options.cache_key)
+    if raw_data:
+        options.say(Message.CACHE_READ)
+        with dots():
+            data = TypeAdapter(PkgCheckResultSet).validate_json(raw_data)
+    else:
         options.vecho("Fetching data from Gentoo Packages API",
                       nl=False, err=True)
         with dots():
             data = await _fetch_stabilization(options)
         if len(data) == 0:
             options.say(Message.EMPTY_RESPONSE)
             return
         options.say(Message.CACHE_WRITE)
         with dots():
-            write_json_cache(data, options.cache_key)
+            raw_data = TypeAdapter(PkgCheckResultSet).dump_json(
+                data, by_alias=True, exclude_none=True
+            )
+            write_raw_json_cache(raw_data, options.cache_key)
 
     candidates = _collect_stable_candidates(data, options)
     if len(candidates) != 0:
         options.echo(tabulate(candidates.items(), tablefmt="plain"))
     else:
         options.say(Message.NO_WORK)
 
 
 @click.command()
+@click.option("-F", "--filter", "version_part",
+              type=click.Choice(["major", "minor", "patch"]),
+              help="Version part filter.")
 @click.pass_obj
-def outdated(options: Options) -> None:
-    """ Find outdated packages. """
+def outdated(options: Options, version_part: VersionPart | None = None) -> None:
+    """
+    Find outdated packages.
+    """
+
     options.cache_key.feed("outdated")
+
+    options.pgo.extra_options = {"version_part": version_part}
     asyncio.run(_outdated(options))
 
 
 @click.command()
 @click.pass_obj
 def stabilization(options: Options) -> None:
-    """ Find outdated packages. """
+    """
+    Find stable candidates.
+    """
+
     options.cache_key.feed("stabilization")
     asyncio.run(_stabilization(options))
```

### Comparing `find_work-0.6.1/find_work/cli/pkgcheck.py` & `find_work-0.7.0/find_work/cli/pkgcheck.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/find_work/cli/repology.py` & `find_work-0.7.0/find_work/cli/repology.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,60 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 # No warranty
 
 """ CLI subcommands for everything Repology. """
 
 import asyncio
-from collections.abc import Iterable
+from collections.abc import Collection
 
 import click
 import gentoopm
 import repology_client
 import repology_client.exceptions
 from gentoopm.basepm.atom import PMAtom
-from pydantic import RootModel
+from pydantic import TypeAdapter
 from repology_client.types import Package
 from sortedcontainers import SortedSet
 
 from find_work.cache import (
-    read_json_cache,
-    write_json_cache,
+    read_raw_json_cache,
+    write_raw_json_cache,
 )
 from find_work.cli import Message, Options, ProgressDots
-from find_work.types import VersionBump
+from find_work.types import VersionBump, VersionPart
 from find_work.utils import aiohttp_session
 
+PackageSet = set[Package]
+ProjectsMapping = dict[str, PackageSet]
 
-async def _fetch_outdated(options: Options) -> dict[str, set[Package]]:
+
+async def _fetch_outdated(options: Options) -> ProjectsMapping:
     filters: dict = {}
     if options.maintainer:
         filters["maintainer"] = options.maintainer
 
     async with aiohttp_session() as session:
         return await repology_client.get_projects(inrepo=options.repology.repo,
                                                   outdated="on", count=5_000,
                                                   session=session, **filters)
 
 
-def _projects_from_json(data: dict[str, list]) -> dict[str, set[Package]]:
-    result: dict[str, set[Package]] = {}
-    for project, packages in data.items():
-        result[project] = set()
-        for pkg in packages:
-            result[project].add(Package(**pkg))
-    return result
-
-
-def _projects_to_json(data: dict[str, set[Package]]) -> dict[str, list]:
-    result: dict[str, list] = {}
-    for project, packages in data.items():
-        result[project] = []
-        for pkg in packages:
-            pkg_model = RootModel[Package](pkg)
-            pkg_dump = pkg_model.model_dump(mode="json", exclude_none=True)
-            result[project].append(pkg_dump)
-    return result
-
-
-def _collect_version_bumps(data: Iterable[set[Package]],
+def _collect_version_bumps(data: Collection[PackageSet],
                            options: Options) -> SortedSet[VersionBump]:
     pm = gentoopm.get_package_manager()
 
     result: SortedSet[VersionBump] = SortedSet()
     for packages in data:
         latest_pkgs: dict[str, PMAtom] = {}  # latest in repo, not across repos!
         new_version: str | None = None
 
         for pkg in packages:
             if pkg.status == "outdated" and pkg.repo == options.repology.repo:
-                # ``pkg.version`` can contain spaces, better avoid it!
+                # "pkg.version" can contain spaces, better avoid it!
                 origversion = pkg.origversion or pkg.version
                 atom = pm.Atom(f"={pkg.visiblename}-{origversion}")
 
                 latest = latest_pkgs.get(pkg.visiblename)
                 if latest is None or atom.version > latest.version:
                     latest_pkgs[pkg.visiblename] = atom
             elif pkg.status == "newest":
@@ -83,44 +66,61 @@
                                        new_version or "(unknown)"))
     return result
 
 
 async def _outdated(options: Options) -> None:
     dots = ProgressDots(options.verbose)
 
+    if (extra_options := options.repology.extra_options) is not None:
+        version_part: VersionPart | None = extra_options.get("version_part")
+
     options.say(Message.CACHE_LOAD)
     with dots():
-        cached_data = read_json_cache(options.cache_key)
-    if cached_data is not None:
+        raw_data = read_raw_json_cache(options.cache_key)
+    if raw_data:
         options.say(Message.CACHE_READ)
         with dots():
-            data = _projects_from_json(cached_data)
+            data = TypeAdapter(ProjectsMapping).validate_json(raw_data)
     else:
         options.vecho("Fetching data from Repology API", nl=False, err=True)
         try:
             with dots():
                 data = await _fetch_outdated(options)
         except repology_client.exceptions.EmptyResponse:
             options.say(Message.EMPTY_RESPONSE)
             return
         options.say(Message.CACHE_WRITE)
         with dots():
-            json_data = _projects_to_json(data)
-            write_json_cache(json_data, options.cache_key)
+            raw_json = TypeAdapter(ProjectsMapping).dump_json(
+                data, exclude_none=True
+            )
+            write_raw_json_cache(raw_json, options.cache_key)
+
+    no_work = True
+    for bump in _collect_version_bumps(data.values(), options):
+        if version_part and not bump.changed(version_part):
+            continue
 
-    outdated_set = _collect_version_bumps(data.values(), options)
-    for bump in outdated_set:
         options.echo(bump.atom + " ", nl=False)
         options.secho(bump.old_version, fg="red", nl=False)
         options.echo(" → ", nl=False)
         options.secho(bump.new_version, fg="green")
+        no_work = False
 
-    if len(outdated_set) == 0:
+    if no_work:
         options.say(Message.NO_WORK)
 
 
 @click.command()
+@click.option("-F", "--filter", "version_part",
+              type=click.Choice(["major", "minor", "patch"]),
+              help="Version part filter.")
 @click.pass_obj
-def outdated(options: Options) -> None:
-    """ Find outdated packages. """
+def outdated(options: Options, version_part: VersionPart | None = None) -> None:
+    """
+    Find outdated packages.
+    """
+
     options.cache_key.feed("outdated")
+
+    options.repology.extra_options = {"version_part": version_part}
     asyncio.run(_outdated(options))
```

### Comparing `find_work-0.6.1/find_work/data/default_config.toml` & `find_work-0.7.0/find_work/data/default_config.toml`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/man/find-work.1` & `find_work-0.7.0/man/find-work.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 .\" SPDX-FileType: DOCUMENTATION
 .\" SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 .\" SPDX-License-Identifier: WTFPL
 .\" No warranty
-.Dd January 14, 2024
+.Dd April 23, 2024
 .Dt FIND-WORK 1
 .Os
 .Sh NAME
 .Nm find-work
 .Nd discover ebuilds to improve
 .Sh SYNOPSIS
 .Nm
 .Op Fl hV
 .Nm
 .Op Fl qI
 .Op Fl m Ar email
 .Ar module
 .Op Ar arg ...
 .Ar command
+.Op Ar arg ...
 .Sh DESCRIPTION
 .Nm
-is a fun little tool that lets you discover what you can do for Gentoo as a package mantainer.
+is a fun little tool
+that lets you discover what you can do for Gentoo as a package mantainer.
 It contains filters to show only packages you might be interested in.
 .Pp
 .Nm
 provides global and module-specific options.
 Global options must precede the module name, and are as follows:
 .Bl -tag -width Ds
 .It Fl h , -help
@@ -80,16 +82,36 @@
 .Dl Pq alias: Cm p
 .Pp
 This module uses Gentoo Packages API to find work.
 .Pp
 .Ar command
 can be one of the following:
 .Bl -tag -width Ds
-.It Ic outdated Pq alias: Ic out , Ic o
+.It Xo
+.Ic outdated
+.Fl F Ar part
+.Xc
+.Dl Pq alias: Ic out , Ic o
+.Pp
 Find outdated packages.
+.Pp
+This command accepts the following options:
+.Bl -tag width Ds
+.It Fl F Ar part , Fl -filter Ar part
+Least important version part
+.Po
+major,
+minor,
+patch
+.Pc
+change to be displayed.
+Version part matching is implemented very roughly
+and can lead to false matches.
+.El
+.
 .It Ic stabilization Pq alias: Ic stab , Ic s
 Find stabilization candidates.
 .El
 .
 .It Xo
 .Cm pkgcheck
 .Fl r Ar repo
@@ -129,16 +151,36 @@
 .Dl Pq alias: Cm rep , Cm r
 .Pp
 This module uses Repology API to find work.
 .Pp
 .Ar command
 can be one of the following:
 .Bl -tag -width Ds
-.It Ic outdated Pq alias: Ic out , Ic o
+.It Xo
+.Ic outdated
+.Fl F Ar part
+.Xc
+.Dl Pq alias: Ic out , Ic o
+.Pp
 Find outdated packages.
+.Pp
+This command accepts the following options:
+.Bl -tag width Ds
+.It Fl F Ar part , Fl -filter Ar part
+Least important version part
+.Po
+major,
+minor,
+patch
+.Pc
+change to be displayed.
+Version part matching is implemented very roughly
+and can lead to false matches.
+.El
+.
 .El
 .Pp
 The options for
 .Cm find-work repology
 are as follows:
 .Bl -tag -width Ds
 .It Fl r Ar repo , Fl -repo Ar repo
```

### Comparing `find_work-0.6.1/tests/test_config.py` & `find_work-0.7.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tomllib
 from pathlib import Path
 
 import pytest
 
 from find_work.config import Config
-from find_work.types import CliOptionKind
+from find_work.types._config import CliOptionKind
 
 
 def test_alias_empty():
     assert not Config({}).aliases
 
 
 def test_alias_type_error():
```

### Comparing `find_work-0.6.1/tests/test_repology.py` & `find_work-0.7.0/tests/test_repology.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,41 +3,15 @@
 # No warranty
 
 from sortedcontainers import SortedSet
 from repology_client.types import Package
 
 from find_work.types import VersionBump
 from find_work.cli import Options
-from find_work.cli.repology import (
-    _collect_version_bumps,
-    _projects_from_json,
-    _projects_to_json,
-)
-
-
-def test_projects_json_roundtrip():
-    data = {
-        "firefox": {
-            Package(
-                repo="gentoo",
-                visiblename="www-client/firefox",
-                version="9999",
-                status="test",
-                licenses=frozenset(["GPL-2", "LGPL-2.1", "MPL-2.0"]),
-            ),
-            Package(
-                repo="gentoo",
-                visiblename="www-client/firefox-bin",
-                version="9999",
-                status="test",
-                licenses=frozenset(["GPL-2", "LGPL-2.1", "MPL-2.0"]),
-            ),
-        },
-    }
-    assert data == _projects_from_json(_projects_to_json(data))
+from find_work.cli.repology import _collect_version_bumps
 
 
 def test_collect_version_bumps():
     options = Options()
     options.only_installed = False
     options.repology.repo = "example_linux"
```

### Comparing `find_work-0.6.1/README.md` & `find_work-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `find_work-0.6.1/pyproject.toml` & `find_work-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,22 +20,23 @@
     "click",
     "click-aliases",
     "deepmerge",
     "gentoopm<2",
     "pkgcheck",
     "platformdirs<5,>=4",
     "pydantic<3,>=2",
+    "pydantic-core<3,>=2",
     "python-bugzilla",
     "repology-client<2,>=0.0.2",
     "requests<3,>=2",
     "sortedcontainers",
     "tabulate",
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: DFSG approved",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: System :: Software Distribution",
     "Topic :: Utilities",
@@ -48,15 +49,14 @@
     "insipid-sphinx-theme",
     "sphinx",
     "sphinx-prompt",
 ]
 test = [
     "pkgcore",
     "pytest",
-    "pytest-recording",
 ]
 
 [project.scripts]
 find-work = "find_work.__main__:cli"
 
 [project.urls]
 Home = "https://find-work.sysrq.in"
@@ -74,15 +74,15 @@
     "/Makefile",
     "/docs",
     "/man",
     "/tests",
 ]
 
 [tool.pytest.ini_options]
-addopts = "--doctest-modules --block-network"
+addopts = "--doctest-modules"
 
 [tool.mypy]
 disallow_untyped_defs = true
 no_implicit_optional = true
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `find_work-0.6.1/PKG-INFO` & `find_work-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: find-work
-Version: 0.6.1
+Version: 0.7.0
 Summary: Personal advice utility for Gentoo package maintainers
 Project-URL: Home, https://find-work.sysrq.in
 Project-URL: Source, https://git.sysrq.in/find-work
 Project-URL: Issues, https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=find-work
 Project-URL: Changelog, https://find-work.sysrq.in/release-notes.html
 Author-email: Anna <cyber@sysrq.in>
 License-Expression: WTFPL
 License-File: LICENSE
 Keywords: ebuild,gentoo,maintainer,repository
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
@@ -23,28 +23,28 @@
 Requires-Dist: aiohttp<4,>=3
 Requires-Dist: click
 Requires-Dist: click-aliases
 Requires-Dist: deepmerge
 Requires-Dist: gentoopm<2
 Requires-Dist: pkgcheck
 Requires-Dist: platformdirs<5,>=4
+Requires-Dist: pydantic-core<3,>=2
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: python-bugzilla
 Requires-Dist: repology-client<2,>=0.0.2
 Requires-Dist: requests<3,>=2
 Requires-Dist: sortedcontainers
 Requires-Dist: tabulate
 Provides-Extra: docs
 Requires-Dist: insipid-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-prompt; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pkgcore; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-recording; extra == 'test'
 Description-Content-Type: text/markdown
 
 <!-- SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in> -->
 <!-- SPDX-License-Identifier: CC0-1.0 -->
 
 find-work
 =========
```

