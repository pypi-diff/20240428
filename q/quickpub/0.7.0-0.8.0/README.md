# Comparing `tmp/quickpub-0.7.0.tar.gz` & `tmp/quickpub-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickpub-0.7.0.tar", last modified: Sun Apr 21 21:56:44 2024, max compression
+gzip compressed data, was "quickpub-0.8.0.tar", last modified: Sun Apr 28 07:36:49 2024, max compression
```

## Comparing `quickpub-0.7.0.tar` & `quickpub-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 21:56:44.092589 quickpub-0.7.0/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 quickpub-0.7.0/LICENSE
--rw-rw-rw-   0        0        0       31 2024-04-21 21:56:42.000000 quickpub-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2513 2024-04-21 21:56:44.092589 quickpub-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-03-22 20:10:11.000000 quickpub-0.7.0/README.md
--rw-rw-rw-   0        0        0      966 2024-04-21 21:56:42.000000 quickpub-0.7.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-21 21:56:44.085520 quickpub-0.7.0/quickpub/
--rw-rw-rw-   0        0        0       72 2024-03-29 09:27:23.000000 quickpub-0.7.0/quickpub/__init__.py
--rw-rw-rw-   0        0        0     3954 2024-04-21 21:56:32.000000 quickpub-0.7.0/quickpub/__main__.py
--rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.7.0/quickpub/classifiers.py
--rw-rw-rw-   0        0        0      117 2024-03-29 09:27:23.000000 quickpub-0.7.0/quickpub/custom_types.py
--rw-rw-rw-   0        0        0     1158 2024-03-29 09:27:23.000000 quickpub-0.7.0/quickpub/enforcers.py
--rw-rw-rw-   0        0        0     1972 2024-04-21 21:56:42.000000 quickpub-0.7.0/quickpub/files.py
--rw-rw-rw-   0        0        0     6935 2024-04-21 19:35:06.000000 quickpub-0.7.0/quickpub/functions.py
--rw-rw-rw-   0        0        0      396 2024-04-21 19:35:06.000000 quickpub-0.7.0/quickpub/proxy.py
--rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.7.0/quickpub/py.typed
--rw-rw-rw-   0        0        0      820 2024-03-29 21:06:30.000000 quickpub-0.7.0/quickpub/structures.py
--rw-rw-rw-   0        0        0     1178 2024-03-29 09:35:46.000000 quickpub-0.7.0/quickpub/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:56:44.090596 quickpub-0.7.0/quickpub.egg-info/
--rw-rw-rw-   0        0        0     2513 2024-04-21 21:56:43.000000 quickpub-0.7.0/quickpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-04-21 21:56:43.000000 quickpub-0.7.0/quickpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 21:56:43.000000 quickpub-0.7.0/quickpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-21 21:56:43.000000 quickpub-0.7.0/quickpub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 21:56:43.000000 quickpub-0.7.0/quickpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 21:56:44.092589 quickpub-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-21 21:56:42.000000 quickpub-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.789421 quickpub-0.8.0/
+-rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-04-28 07:36:48.000000 quickpub-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2708 2024-04-28 07:36:49.789421 quickpub-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2024-04-28 07:27:00.000000 quickpub-0.8.0/README.md
+-rw-rw-rw-   0        0        0      930 2024-04-28 07:36:48.000000 quickpub-0.8.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.769626 quickpub-0.8.0/quickpub/
+-rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.0/quickpub/__init__.py
+-rw-rw-rw-   0        0        0     4229 2024-04-28 07:26:21.000000 quickpub-0.8.0/quickpub/__main__.py
+-rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.0/quickpub/classifiers.py
+-rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.0/quickpub/custom_types.py
+-rw-rw-rw-   0        0        0     1878 2024-04-28 06:51:36.000000 quickpub-0.8.0/quickpub/enforcers.py
+-rw-rw-rw-   0        0        0     1972 2024-04-27 23:07:44.000000 quickpub-0.8.0/quickpub/files.py
+-rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.0/quickpub/functions.py
+-rw-rw-rw-   0        0        0      498 2024-04-27 18:32:16.000000 quickpub-0.8.0/quickpub/proxy.py
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.0/quickpub/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.779443 quickpub-0.8.0/quickpub/runnables/
+-rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.0/quickpub/runnables/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-28 07:32:26.000000 quickpub-0.8.0/quickpub/runnables/common_check.py
+-rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.0/quickpub/runnables/configurable.py
+-rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.0/quickpub/runnables/has_optional_executable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.784497 quickpub-0.8.0/quickpub/runnables/implementations/
+-rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.0/quickpub/runnables/implementations/__init__.py
+-rw-rw-rw-   0        0        0      921 2024-04-28 07:30:41.000000 quickpub-0.8.0/quickpub/runnables/implementations/mypy.py
+-rw-rw-rw-   0        0        0     1028 2024-04-28 07:30:41.000000 quickpub-0.8.0/quickpub/runnables/implementations/pylint.py
+-rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.0/quickpub/runnables/implementations/pytest.py
+-rw-rw-rw-   0        0        0     1826 2024-04-28 07:35:53.000000 quickpub-0.8.0/quickpub/runnables/implementations/unittest.py
+-rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.0/quickpub/runnables/runnable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.788095 quickpub-0.8.0/quickpub/structures/
+-rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.0/quickpub/structures/__init__.py
+-rw-rw-rw-   0        0        0      250 2024-04-27 23:58:10.000000 quickpub-0.8.0/quickpub/structures/additional_configuration.py
+-rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.0/quickpub/structures/bound.py
+-rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.0/quickpub/structures/version.py
+-rw-rw-rw-   0        0        0     1178 2024-04-27 23:07:15.000000 quickpub-0.8.0/quickpub/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:36:49.774701 quickpub-0.8.0/quickpub.egg-info/
+-rw-rw-rw-   0        0        0     2708 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 07:36:49.000000 quickpub-0.8.0/quickpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 07:36:49.789421 quickpub-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-28 07:36:48.000000 quickpub-0.8.0/setup.py
```

### Comparing `quickpub-0.7.0/LICENSE` & `quickpub-0.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 danielnachumdev
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 danielnachumdev
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `quickpub-0.7.0/PKG-INFO` & `quickpub-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,39 +22,46 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/danielnachumdev/quickpub
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/quickpub/issues
-Keywords: Utils,PyPi,Publish,Quick
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10.13
+Requires-Python: >=3.9.19
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quickpub
 
 Example usage of how this package was published
 ```python
-from quickpub import publish
+from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
 
 
 def main() -> None:
     publish(
         name="quickpub",
-        version="0.5.2",
+        version="0.8.0",
         author="danielnachumdev",
         author_email="danielnachumdev@gmail.com",
         description="A python package to quickly configure and publish a new package",
         homepage="https://github.com/danielnachumdev/quickpub",
-        keywords=["Utils", "PyPi", "Publish", "Quick"],
-        dependencies=["twine", "danielutils"]
+        dependencies=["twine", "danielutils"],
+        min_python="3.9.19",
+        config=AdditionalConfiguration(
+            runners=[
+                MypyRunner(),
+                PylintRunner(),
+                UnittestRunner(),
+            ]
+        )
     )
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
+
 ```
```

### Comparing `quickpub-0.7.0/pyproject.toml` & `quickpub-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickpub"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = ['twine', 'danielutils']
-keywords = ['Utils', 'PyPi', 'Publish', 'Quick']
+keywords = []
 license = { "file" = "./LICENSE" }
 description = "A python package to quickly configure and publish a new package"
 readme = {file = "./README.md", content-type = "text/markdown"}
-requires-python = ">=3.10.13"
+requires-python = ">=3.9.19"
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
 	"Programming Language :: Python :: 3",
 	"Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `quickpub-0.7.0/quickpub/__main__.py` & `quickpub-0.8.0/quickpub/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, Union
 from danielutils import warning, file_exists
 from .validators import validate_version, validate_python_version, validate_keywords, validate_dependencies, \
     validate_source
 from .functions import build, upload, commit, metrics
-from .structures import Version, Config
+from .structures import Version, AdditionalConfiguration
 from .files import create_toml, create_setup, create_manifest
 from .classifiers import *
-from .enforcers import enforce_correct_version, enforce_pypirc_exists, exit_if
+from .enforcers import enforce_local_correct_version, enforce_pypirc_exists, exit_if, enforce_remote_correct_version
 from .custom_types import Path
 
 
 def publish(
         *,
         name: str,
         author: str,
@@ -22,15 +22,15 @@
         readme: Path = "./README.md",
         license: Path = "./LICENSE",
 
         min_python: Optional[Union[Version, str]] = None,
 
         keywords: Optional[list[str]] = None,
         dependencies: Optional[list[str]] = None,
-        config: Optional[Config] = None
+        config: Optional[AdditionalConfiguration] = None
 ) -> None:
     """The main function of this package. will do all the heavy lifting in order for you to publish your package.
 
     Args:
         name (str): The name of the package
         author (str): The name of the author
         author_email (str): The email of the author
@@ -50,18 +50,24 @@
     if src != f"./{name}":
         warning(
             "The source folder's name is different from the package's name. this may not be currently supported correctly")
     exit_if(not file_exists(readme), f"Could not find readme file at {readme}")
     exit_if(not file_exists(license),
             f"Could not find license file at {license}")
     version = validate_version(version)
-    enforce_correct_version(name, version)
+    enforce_local_correct_version(name, version)
     min_python = validate_python_version(min_python)  # type:ignore
     keywords = validate_keywords(keywords)
     dependencies = validate_dependencies(dependencies)
+    enforce_remote_correct_version(name, version)
+
+    if config is not None:
+        if config.runners is not None:
+            for runner in config.runners:
+                runner.run(src)
 
     create_setup()
     create_toml(
         name=name,
         src=src,
         readme=readme,
         license=license,
```

### Comparing `quickpub-0.7.0/quickpub/classifiers.py` & `quickpub-0.8.0/quickpub/classifiers.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.7.0/quickpub/files.py` & `quickpub-0.8.0/quickpub/files.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.7.0/quickpub/functions.py` & `quickpub-0.8.0/quickpub/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sys
 from typing import Optional, Literal
-
-from danielutils import info, error
+from danielutils import info
 
 from .enforcers import exit_if
 from .structures import Version
 import quickpub.proxy
 
 
+
+
 def prev_main():
     import re
     from danielutils import cmrt, cm, read_file, get_files, directory_exists, create_directory  # type:ignore
 
     NAME = "danielutils"
 
     VERSION_PATTERN = r"^(?P<major>0|[1-9]\d*)\.(?P<minor>0|[1-9]\d*)\.(?P<patch>0|[1-9]\d*)(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$"
```

### Comparing `quickpub-0.7.0/quickpub/structures.py` & `quickpub-0.8.0/quickpub/structures/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,17 +18,10 @@
         self.minor = minor
         self.patch = patch
 
     def __str__(self) -> str:
         return f"{self.major}.{self.minor}.{self.patch}"
 
 
-@dataclass
-class Config:
-    pylint: bool = False
-    mypy: bool = False
-
-
 __all__ = [
-    "Version",
-    "Config",
+    'Version'
 ]
```

### Comparing `quickpub-0.7.0/quickpub/validators.py` & `quickpub-0.8.0/quickpub/validators.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.7.0/quickpub.egg-info/PKG-INFO` & `quickpub-0.8.0/quickpub.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,39 +22,46 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/danielnachumdev/quickpub
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/quickpub/issues
-Keywords: Utils,PyPi,Publish,Quick
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10.13
+Requires-Python: >=3.9.19
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quickpub
 
 Example usage of how this package was published
 ```python
-from quickpub import publish
+from quickpub import publish, AdditionalConfiguration, MypyRunner, PylintRunner, UnittestRunner
 
 
 def main() -> None:
     publish(
         name="quickpub",
-        version="0.5.2",
+        version="0.8.0",
         author="danielnachumdev",
         author_email="danielnachumdev@gmail.com",
         description="A python package to quickly configure and publish a new package",
         homepage="https://github.com/danielnachumdev/quickpub",
-        keywords=["Utils", "PyPi", "Publish", "Quick"],
-        dependencies=["twine", "danielutils"]
+        dependencies=["twine", "danielutils"],
+        min_python="3.9.19",
+        config=AdditionalConfiguration(
+            runners=[
+                MypyRunner(),
+                PylintRunner(),
+                UnittestRunner(),
+            ]
+        )
     )
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
+
 ```
```

