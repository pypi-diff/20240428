# Comparing `tmp/quickpub-0.8.0.tar.gz` & `tmp/quickpub-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickpub-0.8.0.tar", last modified: Sun Apr 28 07:36:49 2024, max compression
+gzip compressed data, was "quickpub-0.8.1.tar", last modified: Sun Apr 28 07:51:36 2024, max compression
```

## Comparing `quickpub-0.8.0.tar` & `quickpub-0.8.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.789421 quickpub-0.8.0/
--rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.0/LICENSE
--rw-rw-rw-   0        0        0       31 2024-04-28 07:36:48.000000 quickpub-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2708 2024-04-28 07:36:49.789421 quickpub-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      794 2024-04-28 07:27:00.000000 quickpub-0.8.0/README.md
--rw-rw-rw-   0        0        0      930 2024-04-28 07:36:48.000000 quickpub-0.8.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.769626 quickpub-0.8.0/quickpub/
--rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.0/quickpub/__init__.py
--rw-rw-rw-   0        0        0     4229 2024-04-28 07:26:21.000000 quickpub-0.8.0/quickpub/__main__.py
--rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.0/quickpub/classifiers.py
--rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.0/quickpub/custom_types.py
--rw-rw-rw-   0        0        0     1878 2024-04-28 06:51:36.000000 quickpub-0.8.0/quickpub/enforcers.py
--rw-rw-rw-   0        0        0     1972 2024-04-27 23:07:44.000000 quickpub-0.8.0/quickpub/files.py
--rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.0/quickpub/functions.py
--rw-rw-rw-   0        0        0      498 2024-04-27 18:32:16.000000 quickpub-0.8.0/quickpub/proxy.py
--rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.0/quickpub/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.779443 quickpub-0.8.0/quickpub/runnables/
--rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.0/quickpub/runnables/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-28 07:32:26.000000 quickpub-0.8.0/quickpub/runnables/common_check.py
--rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.0/quickpub/runnables/configurable.py
--rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.0/quickpub/runnables/has_optional_executable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.784497 quickpub-0.8.0/quickpub/runnables/implementations/
--rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.0/quickpub/runnables/implementations/__init__.py
--rw-rw-rw-   0        0        0      921 2024-04-28 07:30:41.000000 quickpub-0.8.0/quickpub/runnables/implementations/mypy.py
--rw-rw-rw-   0        0        0     1028 2024-04-28 07:30:41.000000 quickpub-0.8.0/quickpub/runnables/implementations/pylint.py
--rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.0/quickpub/runnables/implementations/pytest.py
--rw-rw-rw-   0        0        0     1826 2024-04-28 07:35:53.000000 quickpub-0.8.0/quickpub/runnables/implementations/unittest.py
--rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.0/quickpub/runnables/runnable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.788095 quickpub-0.8.0/quickpub/structures/
--rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.0/quickpub/structures/__init__.py
--rw-rw-rw-   0        0        0      250 2024-04-27 23:58:10.000000 quickpub-0.8.0/quickpub/structures/additional_configuration.py
--rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.0/quickpub/structures/bound.py
--rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.0/quickpub/structures/version.py
--rw-rw-rw-   0        0        0     1178 2024-04-27 23:07:15.000000 quickpub-0.8.0/quickpub/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.774701 quickpub-0.8.0/quickpub.egg-info/
--rw-rw-rw-   0        0        0     2708 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 07:36:49.789421 quickpub-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-28 07:36:48.000000 quickpub-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.226354 quickpub-0.8.1/
+-rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-04-28 07:51:35.000000 quickpub-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2765 2024-04-28 07:51:36.226354 quickpub-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-28 07:44:18.000000 quickpub-0.8.1/README.md
+-rw-rw-rw-   0        0        0      929 2024-04-28 07:51:35.000000 quickpub-0.8.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.211862 quickpub-0.8.1/quickpub/
+-rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.1/quickpub/__init__.py
+-rw-rw-rw-   0        0        0     4283 2024-04-28 07:41:40.000000 quickpub-0.8.1/quickpub/__main__.py
+-rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.1/quickpub/classifiers.py
+-rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.1/quickpub/custom_types.py
+-rw-rw-rw-   0        0        0     2588 2024-04-28 07:50:17.000000 quickpub-0.8.1/quickpub/enforcers.py
+-rw-rw-rw-   0        0        0     2026 2024-04-28 07:41:26.000000 quickpub-0.8.1/quickpub/files.py
+-rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.1/quickpub/functions.py
+-rw-rw-rw-   0        0        0      549 2024-04-28 07:41:11.000000 quickpub-0.8.1/quickpub/proxy.py
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.1/quickpub/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.218809 quickpub-0.8.1/quickpub/runnables/
+-rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.1/quickpub/runnables/__init__.py
+-rw-rw-rw-   0        0        0     1854 2024-04-28 07:44:18.000000 quickpub-0.8.1/quickpub/runnables/common_check.py
+-rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.1/quickpub/runnables/configurable.py
+-rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.1/quickpub/runnables/has_optional_executable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.222291 quickpub-0.8.1/quickpub/runnables/implementations/
+-rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.1/quickpub/runnables/implementations/__init__.py
+-rw-rw-rw-   0        0        0      883 2024-04-28 07:44:18.000000 quickpub-0.8.1/quickpub/runnables/implementations/mypy.py
+-rw-rw-rw-   0        0        0      990 2024-04-28 07:44:18.000000 quickpub-0.8.1/quickpub/runnables/implementations/pylint.py
+-rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.1/quickpub/runnables/implementations/pytest.py
+-rw-rw-rw-   0        0        0     1878 2024-04-28 07:40:16.000000 quickpub-0.8.1/quickpub/runnables/implementations/unittest.py
+-rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.1/quickpub/runnables/runnable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.225350 quickpub-0.8.1/quickpub/structures/
+-rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.1/quickpub/structures/__init__.py
+-rw-rw-rw-   0        0        0      302 2024-04-28 07:40:28.000000 quickpub-0.8.1/quickpub/structures/additional_configuration.py
+-rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.1/quickpub/structures/bound.py
+-rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.1/quickpub/structures/version.py
+-rw-rw-rw-   0        0        0     1234 2024-04-28 07:40:52.000000 quickpub-0.8.1/quickpub/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.214603 quickpub-0.8.1/quickpub.egg-info/
+-rw-rw-rw-   0        0        0     2765 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 07:51:36.226354 quickpub-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-28 07:51:35.000000 quickpub-0.8.1/setup.py
```

### Comparing `quickpub-0.8.0/LICENSE` & `quickpub-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/PKG-INFO` & `quickpub-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.8.0
+Version: 0.8.1
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,19 +26,20 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/danielnachumdev/quickpub
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/quickpub/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.9.19
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quickpub
+**Tested python versions**: `3.8.0`, `3.9.0`, `3.10.13`,
 
 Example usage of how this package was published
 ```python
 from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
 
 
 def main() -> None:
```

### Comparing `quickpub-0.8.0/README.md` & `quickpub-0.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # quickpub
+**Tested python versions**: `3.8.0`, `3.9.0`, `3.10.13`,
 
 Example usage of how this package was published
 ```python
 from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
 
 
 def main() -> None:
```

### Comparing `quickpub-0.8.0/pyproject.toml` & `quickpub-0.8.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickpub"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = ['twine', 'danielutils']
 keywords = []
 license = { "file" = "./LICENSE" }
 description = "A python package to quickly configure and publish a new package"
 readme = {file = "./README.md", content-type = "text/markdown"}
-requires-python = ">=3.9.19"
+requires-python = ">=3.8.0"
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
 	"Programming Language :: Python :: 3",
 	"Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `quickpub-0.8.0/quickpub/__main__.py` & `quickpub-0.8.1/quickpub/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Union
 from danielutils import warning, file_exists
+from danielutils.versioned_imports import t_list
 from .validators import validate_version, validate_python_version, validate_keywords, validate_dependencies, \
     validate_source
 from .functions import build, upload, commit, metrics
 from .structures import Version, AdditionalConfiguration
 from .files import create_toml, create_setup, create_manifest
 from .classifiers import *
 from .enforcers import enforce_local_correct_version, enforce_pypirc_exists, exit_if, enforce_remote_correct_version
@@ -20,16 +21,16 @@
         src: Optional[Path] = None,
         version: Optional[Union[Version, str]] = None,
         readme: Path = "./README.md",
         license: Path = "./LICENSE",
 
         min_python: Optional[Union[Version, str]] = None,
 
-        keywords: Optional[list[str]] = None,
-        dependencies: Optional[list[str]] = None,
+        keywords: Optional[t_list[str]] = None,
+        dependencies: Optional[t_list[str]] = None,
         config: Optional[AdditionalConfiguration] = None
 ) -> None:
     """The main function of this package. will do all the heavy lifting in order for you to publish your package.
 
     Args:
         name (str): The name of the package
         author (str): The name of the author
```

### Comparing `quickpub-0.8.0/quickpub/classifiers.py` & `quickpub-0.8.1/quickpub/classifiers.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/quickpub/enforcers.py` & `quickpub-0.8.1/quickpub/enforcers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,55 @@
 import sys
 from typing import Union, Callable
 
 import requests
 # from bs4 import BeautifulSoup
-from danielutils import directory_exists, get_files, error, file_exists
+from danielutils import directory_exists, get_files, error, file_exists, get_python_version
 from .structures import Version
 from .proxy import get
 
 
 def exit_if(predicate: Union[bool, Callable[[], bool]], msg: str) -> None:
     if (isinstance(predicate, bool) and predicate) or (callable(predicate) and predicate()):
         error(msg)
         sys.exit(1)
 
 
+def _remove_suffix(s: str, suffix: str) -> str:
+    """
+    This function is needed because str.removesuffix is not implemented in python == 3.8.0
+    :param s: string to remove from
+    :param suffix: substring to remove
+    :return: modified string
+    """
+    if get_python_version() >= (3, 9):
+        return s.removesuffix(suffix)
+    return _remove_prefix(s[::-1], suffix[::-1])[::-1]
+
+
+def _remove_prefix(s: str, prefix: str) -> str:
+    """
+
+    :param s:
+    :param prefix:
+    :return:
+    """
+    if get_python_version() >= (3, 9):
+        return s.removeprefix(prefix)
+
+    if s.startswith(prefix):
+        return s[len(prefix):]
+    return s
+
+
 def enforce_local_correct_version(name: str, version: Version) -> None:
     if directory_exists("./dist"):
         max_version = Version(0, 0, 0)
         for d in get_files("./dist"):
-            d = d.removeprefix(f"{name}-").removesuffix(".tar.gz")
+            d = _remove_suffix(_remove_prefix(d, f"{name}-"), ".tar.gz")
             v = Version.from_str(d)
             max_version = max(max_version, v)
         exit_if(
             version <= max_version,
             f"Specified version is '{version}' but (locally available) latest existing is '{max_version}'"
         )
```

### Comparing `quickpub-0.8.0/quickpub/files.py` & `quickpub-0.8.1/quickpub/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from .custom_types import Path
 from .classifiers import Classifier
 from .structures import Version
 from danielutils import get_files
-
+from danielutils.versioned_imports import t_list
 
 def create_toml(
         *,
         name: str,
         src: Path,
         readme: Path,
         license: Path,
         version: Version,
         author: str,
         author_email: str,
         description: str,
         homepage: str,
-        keywords: list[str],
+        keywords: t_list[str],
         min_python: Version,
-        dependencies: list[str],
-        classifiers: list[Classifier]
+        dependencies: t_list[str],
+        classifiers: t_list[Classifier]
 ) -> None:
     classifiers_string = ",\n\t".join([f"\"{str(c)}\"" for c in classifiers])
     if len(classifiers_string) > 0:
         classifiers_string = f"\n\t{classifiers_string}\n"
     py_typed = ""
     for file in get_files(src):
         if file == "py.typed":
```

### Comparing `quickpub-0.8.0/quickpub/functions.py` & `quickpub-0.8.1/quickpub/functions.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/quickpub/runnables/common_check.py` & `quickpub-0.8.1/quickpub/runnables/common_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import os
 from abc import abstractmethod
 from typing import Optional, Union
 
-from danielutils import file_exists, cm, info, get_current_working_directory, set_current_working_directory
+from danielutils import cm, info
+from danielutils.versioned_imports import t_list
 
 from .has_optional_executable import HasOptionalExecutable
 from .runnable import Runnable
 from .configurable import Configurable
 from ..structures import Bound
 
 
@@ -23,21 +23,19 @@
     def _build_command(self, target: str) -> str:
         command: str = self.get_executable()
         if self.has_config:
             command += f" --rcfile {self.config_path}"
         command += f" {target}"
         return command
 
-    @abstractmethod
     def _pre_command(self):
-        ...
+        pass
 
-    @abstractmethod
     def _post_command(self):
-        ...
+        pass
 
     def run(self, target: str, *_) -> None:
         command = self._build_command(target)
         info(f"Running {self.name}")
         self._pre_command()
         try:
             ret, out, err = cm(command)
@@ -45,13 +43,13 @@
             from ..enforcers import exit_if
             exit_if(not self.bound.compare_against(score), f"{self.name} failed to pass it's defined bound")
         finally:
             self._post_command()
 
 
 @abstractmethod
-def _calculate_score(self, ret: int, command_output: list[str]) -> float: ...
+def _calculate_score(self, ret: int, command_output: t_list[str]) -> float: ...
 
 
 __all__ = [
     "CommonCheck"
 ]
```

### Comparing `quickpub-0.8.0/quickpub/runnables/configurable.py` & `quickpub-0.8.1/quickpub/runnables/configurable.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/quickpub/runnables/has_optional_executable.py` & `quickpub-0.8.1/quickpub/runnables/has_optional_executable.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/quickpub/runnables/implementations/mypy.py` & `quickpub-0.8.1/quickpub/runnables/implementations/mypy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import re
 from typing import Optional
+from danielutils.versioned_imports import t_list
 from ..common_check import CommonCheck
 
 
 class MypyRunner(CommonCheck):
-    def _pre_command(self):
-        pass
-
-    def _post_command(self):
-        pass
-
     RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
 
     def __init__(self, configuration_path: Optional[str] = None, executable_path: Optional[str] = None) -> None:
-        CommonCheck.__init__(self, "mypy","<15", configuration_path, executable_path)
+        CommonCheck.__init__(self, "mypy", "<15", configuration_path, executable_path)
 
-    def _calculate_score(self, ret, lines: list[str]) -> float:
+    def _calculate_score(self, ret, lines: t_list[str]) -> float:
         from ...enforcers import exit_if
         rating_line = lines[-1]
         exit_if(not (m := self.RATING_PATTERN.match(rating_line)),
                 f"Failed running MyPy, got exit code {ret}. try running manually using:\n\t{self._build_command('TARGE')}")
         rating_string = m.group(1)
         return float(rating_string)
```

### Comparing `quickpub-0.8.0/quickpub/runnables/implementations/pylint.py` & `quickpub-0.8.1/quickpub/runnables/implementations/pylint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import re
 from typing import Optional
+from danielutils.versioned_imports import t_list
 from ..common_check import CommonCheck
 
 
 class PylintRunner(CommonCheck):
-    def _pre_command(self):
-        pass
-
-    def _post_command(self):
-        pass
-
     def __init__(self, configuration_path: Optional[str] = None, executable_path: Optional[str] = None) -> None:
-        CommonCheck.__init__(self, "pylint",">=0.8", configuration_path, executable_path)
+        CommonCheck.__init__(self, "pylint", ">=0.8", configuration_path, executable_path)
 
     RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
 
-    def _calculate_score(self, ret: int, lines: list[str]) -> float:
+    def _calculate_score(self, ret: int, lines: t_list[str]) -> float:
         from ...enforcers import exit_if
         rating_line = lines[-2]
         exit_if(not (m := self.RATING_PATTERN.match(rating_line)),
                 f"Failed running Pylint, got exit code {ret}. try running manually using:\n\t{self._build_command('TARGET')}")
         rating_string = m.group(1)  # type:ignore
         numerator, denominator = rating_string.split("/")
         return float(numerator) / float(denominator)
```

### Comparing `quickpub-0.8.0/quickpub/runnables/implementations/unittest.py` & `quickpub-0.8.1/quickpub/runnables/implementations/unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import os
 from typing import Optional
 from danielutils import get_current_working_directory, set_current_working_directory
+from danielutils.versioned_imports import t_list
 from ..common_check import CommonCheck
 
 
 class UnittestRunner(CommonCheck):
     def _pre_command(self):
         self._cwd = get_current_working_directory()
         set_current_working_directory(os.path.join(self._cwd, self.target))
@@ -21,15 +22,15 @@
 
     def _build_command(self, src: str, *args) -> str:
         command: str = self.get_executable()
         rel = os.path.relpath(src, self.target).removesuffix(src.lstrip("./\\"))
         command += f" discover -s {rel}"
         return command  # f"cd {self.target}; {command}"  # f"; cd {self.target}"
 
-    def _calculate_score(self, ret: int, lines: list[str]) -> float:
+    def _calculate_score(self, ret: int, lines: t_list[str]) -> float:
         from ...enforcers import exit_if
         num_tests_line = lines[-3]
         num_failed_line = lines[-1] if lines[-1] != "OK" else "0"
         try:
             m = self.RATING_PATTERN.match(num_tests_line)
             if not m:
                 raise AssertionError
```

### Comparing `quickpub-0.8.0/quickpub/structures/bound.py` & `quickpub-0.8.1/quickpub/structures/bound.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/quickpub/structures/version.py` & `quickpub-0.8.1/quickpub/structures/version.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.0/quickpub/validators.py` & `quickpub-0.8.1/quickpub/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Union
 
 from danielutils import get_python_version
-
+from danielutils.versioned_imports import t_list
 from .custom_types import Path
 from .structures import Version
 
 
 def validate_version(version: Optional[Union[str, Version]]) -> Version:
     if version is None:
         version = Version(0, 0, 1)
@@ -16,21 +16,21 @@
 
 def validate_python_version(min_python: Optional[Version]) -> Version:
     if min_python is not None:
         return min_python
     return Version(*get_python_version())
 
 
-def validate_keywords(keywords: Optional[list[str]]) -> list[str]:
+def validate_keywords(keywords: Optional[t_list[str]]) -> t_list[str]:
     if keywords is None:
         return []
     return keywords
 
 
-def validate_dependencies(dependencies: Optional[list[str]]) -> list[str]:
+def validate_dependencies(dependencies: Optional[t_list[str]]) -> t_list[str]:
     if dependencies is None:
         return []
     return dependencies
 
 
 def validate_source(name: str, src: Optional[Path] = None) -> Path:
     if src is not None:
```

### Comparing `quickpub-0.8.0/quickpub.egg-info/PKG-INFO` & `quickpub-0.8.1/quickpub.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.8.0
+Version: 0.8.1
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,19 +26,20 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/danielnachumdev/quickpub
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/quickpub/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.9.19
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quickpub
+**Tested python versions**: `3.8.0`, `3.9.0`, `3.10.13`,
 
 Example usage of how this package was published
 ```python
 from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
 
 
 def main() -> None:
```

### Comparing `quickpub-0.8.0/quickpub.egg-info/SOURCES.txt` & `quickpub-0.8.1/quickpub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

