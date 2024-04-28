# Comparing `tmp/quickpub-0.8.2.tar.gz` & `tmp/quickpub-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickpub-0.8.2.tar", last modified: Sun Apr 28 07:54:05 2024, max compression
+gzip compressed data, was "quickpub-0.8.3.tar", last modified: Sun Apr 28 08:38:38 2024, max compression
```

## Comparing `quickpub-0.8.2.tar` & `quickpub-0.8.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.021793 quickpub-0.8.2/
--rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.2/LICENSE
--rw-rw-rw-   0        0        0       31 2024-04-28 07:54:04.000000 quickpub-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2802 2024-04-28 07:54:05.021793 quickpub-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-04-28 07:53:52.000000 quickpub-0.8.2/README.md
--rw-rw-rw-   0        0        0      929 2024-04-28 07:54:04.000000 quickpub-0.8.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.007634 quickpub-0.8.2/quickpub/
--rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.2/quickpub/__init__.py
--rw-rw-rw-   0        0        0     4283 2024-04-28 07:41:40.000000 quickpub-0.8.2/quickpub/__main__.py
--rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.2/quickpub/classifiers.py
--rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.2/quickpub/custom_types.py
--rw-rw-rw-   0        0        0     2588 2024-04-28 07:50:17.000000 quickpub-0.8.2/quickpub/enforcers.py
--rw-rw-rw-   0        0        0     2026 2024-04-28 07:41:26.000000 quickpub-0.8.2/quickpub/files.py
--rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.2/quickpub/functions.py
--rw-rw-rw-   0        0        0      549 2024-04-28 07:41:11.000000 quickpub-0.8.2/quickpub/proxy.py
--rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.2/quickpub/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.014821 quickpub-0.8.2/quickpub/runnables/
--rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.2/quickpub/runnables/__init__.py
--rw-rw-rw-   0        0        0     1854 2024-04-28 07:44:18.000000 quickpub-0.8.2/quickpub/runnables/common_check.py
--rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.2/quickpub/runnables/configurable.py
--rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.2/quickpub/runnables/has_optional_executable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.017617 quickpub-0.8.2/quickpub/runnables/implementations/
--rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.2/quickpub/runnables/implementations/__init__.py
--rw-rw-rw-   0        0        0      921 2024-04-28 07:53:52.000000 quickpub-0.8.2/quickpub/runnables/implementations/mypy.py
--rw-rw-rw-   0        0        0     1028 2024-04-28 07:53:52.000000 quickpub-0.8.2/quickpub/runnables/implementations/pylint.py
--rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.2/quickpub/runnables/implementations/pytest.py
--rw-rw-rw-   0        0        0     1898 2024-04-28 07:53:52.000000 quickpub-0.8.2/quickpub/runnables/implementations/unittest.py
--rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.2/quickpub/runnables/runnable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.020791 quickpub-0.8.2/quickpub/structures/
--rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.2/quickpub/structures/__init__.py
--rw-rw-rw-   0        0        0      302 2024-04-28 07:40:28.000000 quickpub-0.8.2/quickpub/structures/additional_configuration.py
--rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.2/quickpub/structures/bound.py
--rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.2/quickpub/structures/version.py
--rw-rw-rw-   0        0        0     1234 2024-04-28 07:40:52.000000 quickpub-0.8.2/quickpub/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.011311 quickpub-0.8.2/quickpub.egg-info/
--rw-rw-rw-   0        0        0     2802 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 07:54:05.022817 quickpub-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-28 07:54:04.000000 quickpub-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:38:38.470734 quickpub-0.8.3/
+-rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-04-28 08:38:37.000000 quickpub-0.8.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2809 2024-04-28 08:38:38.470734 quickpub-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      895 2024-04-28 08:37:24.000000 quickpub-0.8.3/README.md
+-rw-rw-rw-   0        0        0      929 2024-04-28 08:38:37.000000 quickpub-0.8.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-28 08:38:38.448942 quickpub-0.8.3/quickpub/
+-rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.3/quickpub/__init__.py
+-rw-rw-rw-   0        0        0     4235 2024-04-28 08:33:48.000000 quickpub-0.8.3/quickpub/__main__.py
+-rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.3/quickpub/classifiers.py
+-rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.3/quickpub/custom_types.py
+-rw-rw-rw-   0        0        0     2588 2024-04-28 07:50:17.000000 quickpub-0.8.3/quickpub/enforcers.py
+-rw-rw-rw-   0        0        0     2007 2024-04-28 08:34:29.000000 quickpub-0.8.3/quickpub/files.py
+-rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.3/quickpub/functions.py
+-rw-rw-rw-   0        0        0      524 2024-04-28 08:34:08.000000 quickpub-0.8.3/quickpub/proxy.py
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.3/quickpub/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-28 08:38:38.459694 quickpub-0.8.3/quickpub/runnables/
+-rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.3/quickpub/runnables/__init__.py
+-rw-rw-rw-   0        0        0     1811 2024-04-28 08:38:23.000000 quickpub-0.8.3/quickpub/runnables/common_check.py
+-rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.3/quickpub/runnables/configurable.py
+-rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.3/quickpub/runnables/has_optional_executable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:38:38.465381 quickpub-0.8.3/quickpub/runnables/implementations/
+-rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.3/quickpub/runnables/implementations/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-04-28 08:36:06.000000 quickpub-0.8.3/quickpub/runnables/implementations/mypy.py
+-rw-rw-rw-   0        0        0     1219 2024-04-28 08:36:06.000000 quickpub-0.8.3/quickpub/runnables/implementations/pylint.py
+-rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.3/quickpub/runnables/implementations/pytest.py
+-rw-rw-rw-   0        0        0     1852 2024-04-28 08:33:36.000000 quickpub-0.8.3/quickpub/runnables/implementations/unittest.py
+-rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.3/quickpub/runnables/runnable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:38:38.468548 quickpub-0.8.3/quickpub/structures/
+-rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.3/quickpub/structures/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-28 08:33:12.000000 quickpub-0.8.3/quickpub/structures/additional_configuration.py
+-rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.3/quickpub/structures/bound.py
+-rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.3/quickpub/structures/version.py
+-rw-rw-rw-   0        0        0     1182 2024-04-28 08:33:55.000000 quickpub-0.8.3/quickpub/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:38:38.453393 quickpub-0.8.3/quickpub.egg-info/
+-rw-rw-rw-   0        0        0     2809 2024-04-28 08:38:38.000000 quickpub-0.8.3/quickpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-04-28 08:38:38.000000 quickpub-0.8.3/quickpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 08:38:38.000000 quickpub-0.8.3/quickpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 08:38:38.000000 quickpub-0.8.3/quickpub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 08:38:38.000000 quickpub-0.8.3/quickpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 08:38:38.470734 quickpub-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-28 08:38:37.000000 quickpub-0.8.3/setup.py
```

### Comparing `quickpub-0.8.2/LICENSE` & `quickpub-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/PKG-INFO` & `quickpub-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.8.2
+Version: 0.8.3
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# quickpub
+# quickpub V0.8.3
 **Tested python versions**: `3.8.0`, `3.9.0`, `3.10.13`,
 
 Example usage of how this package was published
 ```python
 from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
```

### Comparing `quickpub-0.8.2/README.md` & `quickpub-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# quickpub
+# quickpub V0.8.3
 **Tested python versions**: `3.8.0`, `3.9.0`, `3.10.13`,
 
 Example usage of how this package was published
 ```python
 from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
```

### Comparing `quickpub-0.8.2/pyproject.toml` & `quickpub-0.8.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickpub"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = ['twine', 'danielutils']
 keywords = []
 license = { "file" = "./LICENSE" }
 description = "A python package to quickly configure and publish a new package"
```

### Comparing `quickpub-0.8.2/quickpub/__main__.py` & `quickpub-0.8.3/quickpub/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Optional, Union
+from typing import Optional, Union, List
 from danielutils import warning, file_exists
-from danielutils.versioned_imports import t_list
 from .validators import validate_version, validate_python_version, validate_keywords, validate_dependencies, \
     validate_source
 from .functions import build, upload, commit, metrics
 from .structures import Version, AdditionalConfiguration
 from .files import create_toml, create_setup, create_manifest
 from .classifiers import *
 from .enforcers import enforce_local_correct_version, enforce_pypirc_exists, exit_if, enforce_remote_correct_version
@@ -21,16 +20,16 @@
         src: Optional[Path] = None,
         version: Optional[Union[Version, str]] = None,
         readme: Path = "./README.md",
         license: Path = "./LICENSE",
 
         min_python: Optional[Union[Version, str]] = None,
 
-        keywords: Optional[t_list[str]] = None,
-        dependencies: Optional[t_list[str]] = None,
+        keywords: Optional[List[str]] = None,
+        dependencies: Optional[List[str]] = None,
         config: Optional[AdditionalConfiguration] = None
 ) -> None:
     """The main function of this package. will do all the heavy lifting in order for you to publish your package.
 
     Args:
         name (str): The name of the package
         author (str): The name of the author
```

### Comparing `quickpub-0.8.2/quickpub/classifiers.py` & `quickpub-0.8.3/quickpub/classifiers.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/enforcers.py` & `quickpub-0.8.3/quickpub/enforcers.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/files.py` & `quickpub-0.8.3/quickpub/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+from typing import List
+from danielutils import get_files
 from .custom_types import Path
 from .classifiers import Classifier
 from .structures import Version
-from danielutils import get_files
-from danielutils.versioned_imports import t_list
+
 
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
-        keywords: t_list[str],
+        keywords: List[str],
         min_python: Version,
-        dependencies: t_list[str],
-        classifiers: t_list[Classifier]
+        dependencies: List[str],
+        classifiers: List[Classifier]
 ) -> None:
     classifiers_string = ",\n\t".join([f"\"{str(c)}\"" for c in classifiers])
     if len(classifiers_string) > 0:
         classifiers_string = f"\n\t{classifiers_string}\n"
     py_typed = ""
     for file in get_files(src):
         if file == "py.typed":
@@ -59,15 +60,18 @@
     with open("pyproject.toml", "w", encoding="utf8") as f:
         f.write(s)
 
 
 def create_setup() -> None:
     with open("./setup.py", "w", encoding="utf8") as f:
         f.write("from setuptools import setup\n\nsetup()\n")
-def create_manifest(*,name:str)->None:
+
+
+def create_manifest(*, name: str) -> None:
     with open("./MANIFEST.in", "w", encoding="utf8") as f:
         f.write(f"recursive-include {name} *.py")
 
+
 __all__ = [
     "create_setup",
     "create_toml"
 ]
```

### Comparing `quickpub-0.8.2/quickpub/functions.py` & `quickpub-0.8.3/quickpub/functions.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/runnables/common_check.py` & `quickpub-0.8.3/quickpub/runnables/common_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import abstractmethod
-from typing import Optional, Union
+from typing import Optional, Union, List
 
 from danielutils import cm, info
-from danielutils.versioned_imports import t_list
 
 from .has_optional_executable import HasOptionalExecutable
 from .runnable import Runnable
 from .configurable import Configurable
 from ..structures import Bound
 
 
@@ -16,20 +15,17 @@
                  configuration_path: Optional[str] = None,
                  executable_path: Optional[str] = None) -> None:
         Configurable.__init__(self, configuration_path)
         HasOptionalExecutable.__init__(self, name, executable_path)
         self.bound: Bound = bound if isinstance(bound, Bound) else Bound.from_string(bound)
         self.target = target
 
+    @abstractmethod
     def _build_command(self, target: str) -> str:
-        command: str = self.get_executable()
-        if self.has_config:
-            command += f" --rcfile {self.config_path}"
-        command += f" {target}"
-        return command
+        ...
 
     def _pre_command(self):
         pass
 
     def _post_command(self):
         pass
 
@@ -38,18 +34,20 @@
         info(f"Running {self.name}")
         self._pre_command()
         try:
             ret, out, err = cm(command)
             score = self._calculate_score(ret, b"".join([out, err]).decode("utf-8").splitlines())
             from ..enforcers import exit_if
             exit_if(not self.bound.compare_against(score), f"{self.name} failed to pass it's defined bound")
+        except Exception as e:
+            raise RuntimeError(f"Failed to run {self.name}, try running manually:\n{self._build_command('TARGET')}") from e
         finally:
             self._post_command()
 
 
 @abstractmethod
-def _calculate_score(self, ret: int, command_output: t_list[str]) -> float: ...
+def _calculate_score(self, ret: int, command_output: List[str]) -> float: ...
 
 
 __all__ = [
     "CommonCheck"
 ]
```

### Comparing `quickpub-0.8.2/quickpub/runnables/configurable.py` & `quickpub-0.8.3/quickpub/runnables/configurable.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/runnables/has_optional_executable.py` & `quickpub-0.8.3/quickpub/runnables/has_optional_executable.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/runnables/implementations/mypy.py` & `quickpub-0.8.3/quickpub/runnables/implementations/mypy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import re
-from typing import Optional
-from danielutils.versioned_imports import t_list
+from typing import Optional, List
 from ..common_check import CommonCheck
 
 
 class MypyRunner(CommonCheck):
+    def _build_command(self, target: str) -> str:
+        command: str = self.get_executable()
+        if self.has_config:
+            command += f" --config-file {self.config_path}"
+        command += f" {target}"
+        return command
+
     RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
 
     def __init__(self, bound: str = "<15", configuration_path: Optional[str] = None,
                  executable_path: Optional[str] = None) -> None:
         CommonCheck.__init__(self, "mypy", bound, configuration_path, executable_path)
 
-    def _calculate_score(self, ret, lines: t_list[str]) -> float:
+    def _calculate_score(self, ret, lines: List[str]) -> float:
         from ...enforcers import exit_if
         rating_line = lines[-1]
         exit_if(not (m := self.RATING_PATTERN.match(rating_line)),
                 f"Failed running MyPy, got exit code {ret}. try running manually using:\n\t{self._build_command('TARGE')}")
         rating_string = m.group(1)
         return float(rating_string)
```

### Comparing `quickpub-0.8.2/quickpub/runnables/implementations/pylint.py` & `quickpub-0.8.3/quickpub/runnables/implementations/pylint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import re
-from typing import Optional
-from danielutils.versioned_imports import t_list
+from typing import Optional, List
 from ..common_check import CommonCheck
 
 
 class PylintRunner(CommonCheck):
+    RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
     def __init__(self, bound: str = ">=0.8", configuration_path: Optional[str] = None,
                  executable_path: Optional[str] = None) -> None:
         CommonCheck.__init__(self, "pylint", bound, configuration_path, executable_path)
 
-    RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
-
-    def _calculate_score(self, ret: int, lines: t_list[str]) -> float:
+    def _build_command(self, target: str) -> str:
+        command: str = self.get_executable()
+        if self.has_config:
+            command += f" --rcfile {self.config_path}"
+        command += f" {target}"
+        return command
+    def _calculate_score(self, ret: int, lines: List[str]) -> float:
         from ...enforcers import exit_if
         rating_line = lines[-2]
         exit_if(not (m := self.RATING_PATTERN.match(rating_line)),
                 f"Failed running Pylint, got exit code {ret}. try running manually using:\n\t{self._build_command('TARGET')}")
         rating_string = m.group(1)  # type:ignore
         numerator, denominator = rating_string.split("/")
         return float(numerator) / float(denominator)
```

### Comparing `quickpub-0.8.2/quickpub/runnables/implementations/unittest.py` & `quickpub-0.8.3/quickpub/runnables/implementations/unittest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 import os
-from typing import Optional
+from typing import Optional, List
 from danielutils import get_current_working_directory, set_current_working_directory
-from danielutils.versioned_imports import t_list
 from ..common_check import CommonCheck
 
 
 class UnittestRunner(CommonCheck):
     def _pre_command(self):
         self._cwd = get_current_working_directory()
         set_current_working_directory(os.path.join(self._cwd, self.target))
@@ -22,15 +21,15 @@
 
     def _build_command(self, src: str, *args) -> str:
         command: str = self.get_executable()
         rel = os.path.relpath(src, self.target).removesuffix(src.lstrip("./\\"))
         command += f" discover -s {rel}"
         return command  # f"cd {self.target}; {command}"  # f"; cd {self.target}"
 
-    def _calculate_score(self, ret: int, lines: t_list[str]) -> float:
+    def _calculate_score(self, ret: int, lines: List[str]) -> float:
         from ...enforcers import exit_if
         num_tests_line = lines[-3]
         num_failed_line = lines[-1] if lines[-1] != "OK" else "0"
         try:
             m = self.RATING_PATTERN.match(num_tests_line)
             if not m:
                 raise AssertionError
```

### Comparing `quickpub-0.8.2/quickpub/structures/bound.py` & `quickpub-0.8.3/quickpub/structures/bound.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/structures/version.py` & `quickpub-0.8.3/quickpub/structures/version.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.2/quickpub/validators.py` & `quickpub-0.8.3/quickpub/validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Optional, Union
+from typing import Optional, Union, List
 
 from danielutils import get_python_version
-from danielutils.versioned_imports import t_list
 from .custom_types import Path
 from .structures import Version
 
 
 def validate_version(version: Optional[Union[str, Version]]) -> Version:
     if version is None:
         version = Version(0, 0, 1)
@@ -16,21 +15,21 @@
 
 def validate_python_version(min_python: Optional[Version]) -> Version:
     if min_python is not None:
         return min_python
     return Version(*get_python_version())
 
 
-def validate_keywords(keywords: Optional[t_list[str]]) -> t_list[str]:
+def validate_keywords(keywords: Optional[List[str]]) -> List[str]:
     if keywords is None:
         return []
     return keywords
 
 
-def validate_dependencies(dependencies: Optional[t_list[str]]) -> t_list[str]:
+def validate_dependencies(dependencies: Optional[List[str]]) -> List[str]:
     if dependencies is None:
         return []
     return dependencies
 
 
 def validate_source(name: str, src: Optional[Path] = None) -> Path:
     if src is not None:
```

### Comparing `quickpub-0.8.2/quickpub.egg-info/PKG-INFO` & `quickpub-0.8.3/quickpub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.8.2
+Version: 0.8.3
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# quickpub
+# quickpub V0.8.3
 **Tested python versions**: `3.8.0`, `3.9.0`, `3.10.13`,
 
 Example usage of how this package was published
 ```python
 from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
```

### Comparing `quickpub-0.8.2/quickpub.egg-info/SOURCES.txt` & `quickpub-0.8.3/quickpub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

