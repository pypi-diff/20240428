# Comparing `tmp/quickpub-0.8.1.tar.gz` & `tmp/quickpub-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickpub-0.8.1.tar", last modified: Sun Apr 28 07:51:36 2024, max compression
+gzip compressed data, was "quickpub-0.8.2.tar", last modified: Sun Apr 28 07:54:05 2024, max compression
```

## Comparing `quickpub-0.8.1.tar` & `quickpub-0.8.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.226354 quickpub-0.8.1/
--rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.1/LICENSE
--rw-rw-rw-   0        0        0       31 2024-04-28 07:51:35.000000 quickpub-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2765 2024-04-28 07:51:36.226354 quickpub-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-28 07:44:18.000000 quickpub-0.8.1/README.md
--rw-rw-rw-   0        0        0      929 2024-04-28 07:51:35.000000 quickpub-0.8.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.211862 quickpub-0.8.1/quickpub/
--rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.1/quickpub/__init__.py
--rw-rw-rw-   0        0        0     4283 2024-04-28 07:41:40.000000 quickpub-0.8.1/quickpub/__main__.py
--rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.1/quickpub/classifiers.py
--rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.1/quickpub/custom_types.py
--rw-rw-rw-   0        0        0     2588 2024-04-28 07:50:17.000000 quickpub-0.8.1/quickpub/enforcers.py
--rw-rw-rw-   0        0        0     2026 2024-04-28 07:41:26.000000 quickpub-0.8.1/quickpub/files.py
--rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.1/quickpub/functions.py
--rw-rw-rw-   0        0        0      549 2024-04-28 07:41:11.000000 quickpub-0.8.1/quickpub/proxy.py
--rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.1/quickpub/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.218809 quickpub-0.8.1/quickpub/runnables/
--rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.1/quickpub/runnables/__init__.py
--rw-rw-rw-   0        0        0     1854 2024-04-28 07:44:18.000000 quickpub-0.8.1/quickpub/runnables/common_check.py
--rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.1/quickpub/runnables/configurable.py
--rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.1/quickpub/runnables/has_optional_executable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.222291 quickpub-0.8.1/quickpub/runnables/implementations/
--rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.1/quickpub/runnables/implementations/__init__.py
--rw-rw-rw-   0        0        0      883 2024-04-28 07:44:18.000000 quickpub-0.8.1/quickpub/runnables/implementations/mypy.py
--rw-rw-rw-   0        0        0      990 2024-04-28 07:44:18.000000 quickpub-0.8.1/quickpub/runnables/implementations/pylint.py
--rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.1/quickpub/runnables/implementations/pytest.py
--rw-rw-rw-   0        0        0     1878 2024-04-28 07:40:16.000000 quickpub-0.8.1/quickpub/runnables/implementations/unittest.py
--rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.1/quickpub/runnables/runnable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.225350 quickpub-0.8.1/quickpub/structures/
--rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.1/quickpub/structures/__init__.py
--rw-rw-rw-   0        0        0      302 2024-04-28 07:40:28.000000 quickpub-0.8.1/quickpub/structures/additional_configuration.py
--rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.1/quickpub/structures/bound.py
--rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.1/quickpub/structures/version.py
--rw-rw-rw-   0        0        0     1234 2024-04-28 07:40:52.000000 quickpub-0.8.1/quickpub/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:51:36.214603 quickpub-0.8.1/quickpub.egg-info/
--rw-rw-rw-   0        0        0     2765 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 07:51:36.000000 quickpub-0.8.1/quickpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 07:51:36.226354 quickpub-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-28 07:51:35.000000 quickpub-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.021793 quickpub-0.8.2/
+-rw-rw-rw-   0        0        0     1071 2024-04-28 00:01:34.000000 quickpub-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-04-28 07:54:04.000000 quickpub-0.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2802 2024-04-28 07:54:05.021793 quickpub-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-04-28 07:53:52.000000 quickpub-0.8.2/README.md
+-rw-rw-rw-   0        0        0      929 2024-04-28 07:54:04.000000 quickpub-0.8.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.007634 quickpub-0.8.2/quickpub/
+-rw-rw-rw-   0        0        0       84 2024-04-27 23:58:10.000000 quickpub-0.8.2/quickpub/__init__.py
+-rw-rw-rw-   0        0        0     4283 2024-04-28 07:41:40.000000 quickpub-0.8.2/quickpub/__main__.py
+-rw-rw-rw-   0        0        0     1838 2024-03-22 00:09:08.000000 quickpub-0.8.2/quickpub/classifiers.py
+-rw-rw-rw-   0        0        0      202 2024-04-27 19:17:21.000000 quickpub-0.8.2/quickpub/custom_types.py
+-rw-rw-rw-   0        0        0     2588 2024-04-28 07:50:17.000000 quickpub-0.8.2/quickpub/enforcers.py
+-rw-rw-rw-   0        0        0     2026 2024-04-28 07:41:26.000000 quickpub-0.8.2/quickpub/files.py
+-rw-rw-rw-   0        0        0     6930 2024-04-27 23:07:36.000000 quickpub-0.8.2/quickpub/functions.py
+-rw-rw-rw-   0        0        0      549 2024-04-28 07:41:11.000000 quickpub-0.8.2/quickpub/proxy.py
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:35:10.000000 quickpub-0.8.2/quickpub/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.014821 quickpub-0.8.2/quickpub/runnables/
+-rw-rw-rw-   0        0        0       64 2024-04-27 23:51:44.000000 quickpub-0.8.2/quickpub/runnables/__init__.py
+-rw-rw-rw-   0        0        0     1854 2024-04-28 07:44:18.000000 quickpub-0.8.2/quickpub/runnables/common_check.py
+-rw-rw-rw-   0        0        0      522 2024-04-27 23:35:41.000000 quickpub-0.8.2/quickpub/runnables/configurable.py
+-rw-rw-rw-   0        0        0      854 2024-04-28 00:04:43.000000 quickpub-0.8.2/quickpub/runnables/has_optional_executable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.017617 quickpub-0.8.2/quickpub/runnables/implementations/
+-rw-rw-rw-   0        0        0       92 2024-04-27 23:51:44.000000 quickpub-0.8.2/quickpub/runnables/implementations/__init__.py
+-rw-rw-rw-   0        0        0      921 2024-04-28 07:53:52.000000 quickpub-0.8.2/quickpub/runnables/implementations/mypy.py
+-rw-rw-rw-   0        0        0     1028 2024-04-28 07:53:52.000000 quickpub-0.8.2/quickpub/runnables/implementations/pylint.py
+-rw-rw-rw-   0        0        0        8 2024-04-27 23:51:44.000000 quickpub-0.8.2/quickpub/runnables/implementations/pytest.py
+-rw-rw-rw-   0        0        0     1898 2024-04-28 07:53:52.000000 quickpub-0.8.2/quickpub/runnables/implementations/unittest.py
+-rw-rw-rw-   0        0        0      170 2024-04-27 23:35:41.000000 quickpub-0.8.2/quickpub/runnables/runnable.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.020791 quickpub-0.8.2/quickpub/structures/
+-rw-rw-rw-   0        0        0       87 2024-04-27 23:06:54.000000 quickpub-0.8.2/quickpub/structures/__init__.py
+-rw-rw-rw-   0        0        0      302 2024-04-28 07:40:28.000000 quickpub-0.8.2/quickpub/structures/additional_configuration.py
+-rw-rw-rw-   0        0        0      824 2024-04-27 23:06:33.000000 quickpub-0.8.2/quickpub/structures/bound.py
+-rw-rw-rw-   0        0        0      723 2024-04-27 23:06:33.000000 quickpub-0.8.2/quickpub/structures/version.py
+-rw-rw-rw-   0        0        0     1234 2024-04-28 07:40:52.000000 quickpub-0.8.2/quickpub/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:54:05.011311 quickpub-0.8.2/quickpub.egg-info/
+-rw-rw-rw-   0        0        0     2802 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 07:54:04.000000 quickpub-0.8.2/quickpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 07:54:05.022817 quickpub-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-28 07:54:04.000000 quickpub-0.8.2/setup.py
```

### Comparing `quickpub-0.8.1/LICENSE` & `quickpub-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/PKG-INFO` & `quickpub-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.8.1
+Version: 0.8.2
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,17 +50,17 @@
         author_email="danielnachumdev@gmail.com",
         description="A python package to quickly configure and publish a new package",
         homepage="https://github.com/danielnachumdev/quickpub",
         dependencies=["twine", "danielutils"],
         min_python="3.9.19",
         config=AdditionalConfiguration(
             runners=[
-                MypyRunner(),
-                PylintRunner(),
-                UnittestRunner(),
+                MypyRunner(bound="<15"),
+                PylintRunner(bound=">=0.8"),
+                UnittestRunner(bound=">=0.8"),
             ]
         )
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `quickpub-0.8.1/README.md` & `quickpub-0.8.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         author_email="danielnachumdev@gmail.com",
         description="A python package to quickly configure and publish a new package",
         homepage="https://github.com/danielnachumdev/quickpub",
         dependencies=["twine", "danielutils"],
         min_python="3.9.19",
         config=AdditionalConfiguration(
             runners=[
-                MypyRunner(),
-                PylintRunner(),
-                UnittestRunner(),
+                MypyRunner(bound="<15"),
+                PylintRunner(bound=">=0.8"),
+                UnittestRunner(bound=">=0.8"),
             ]
         )
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `quickpub-0.8.1/pyproject.toml` & `quickpub-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickpub"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = ['twine', 'danielutils']
 keywords = []
 license = { "file" = "./LICENSE" }
 description = "A python package to quickly configure and publish a new package"
```

### Comparing `quickpub-0.8.1/quickpub/__main__.py` & `quickpub-0.8.2/quickpub/__main__.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/classifiers.py` & `quickpub-0.8.2/quickpub/classifiers.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/enforcers.py` & `quickpub-0.8.2/quickpub/enforcers.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/files.py` & `quickpub-0.8.2/quickpub/files.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/functions.py` & `quickpub-0.8.2/quickpub/functions.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/proxy.py` & `quickpub-0.8.2/quickpub/proxy.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/runnables/common_check.py` & `quickpub-0.8.2/quickpub/runnables/common_check.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/runnables/configurable.py` & `quickpub-0.8.2/quickpub/runnables/configurable.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/runnables/has_optional_executable.py` & `quickpub-0.8.2/quickpub/runnables/has_optional_executable.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/runnables/implementations/mypy.py` & `quickpub-0.8.2/quickpub/runnables/implementations/mypy.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from danielutils.versioned_imports import t_list
 from ..common_check import CommonCheck
 
 
 class MypyRunner(CommonCheck):
     RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
 
-    def __init__(self, configuration_path: Optional[str] = None, executable_path: Optional[str] = None) -> None:
-        CommonCheck.__init__(self, "mypy", "<15", configuration_path, executable_path)
+    def __init__(self, bound: str = "<15", configuration_path: Optional[str] = None,
+                 executable_path: Optional[str] = None) -> None:
+        CommonCheck.__init__(self, "mypy", bound, configuration_path, executable_path)
 
     def _calculate_score(self, ret, lines: t_list[str]) -> float:
         from ...enforcers import exit_if
         rating_line = lines[-1]
         exit_if(not (m := self.RATING_PATTERN.match(rating_line)),
                 f"Failed running MyPy, got exit code {ret}. try running manually using:\n\t{self._build_command('TARGE')}")
         rating_string = m.group(1)
```

### Comparing `quickpub-0.8.1/quickpub/runnables/implementations/pylint.py` & `quickpub-0.8.2/quickpub/runnables/implementations/pylint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 from typing import Optional
 from danielutils.versioned_imports import t_list
 from ..common_check import CommonCheck
 
 
 class PylintRunner(CommonCheck):
-    def __init__(self, configuration_path: Optional[str] = None, executable_path: Optional[str] = None) -> None:
-        CommonCheck.__init__(self, "pylint", ">=0.8", configuration_path, executable_path)
+    def __init__(self, bound: str = ">=0.8", configuration_path: Optional[str] = None,
+                 executable_path: Optional[str] = None) -> None:
+        CommonCheck.__init__(self, "pylint", bound, configuration_path, executable_path)
 
     RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
 
     def _calculate_score(self, ret: int, lines: t_list[str]) -> float:
         from ...enforcers import exit_if
         rating_line = lines[-2]
         exit_if(not (m := self.RATING_PATTERN.match(rating_line)),
```

### Comparing `quickpub-0.8.1/quickpub/runnables/implementations/unittest.py` & `quickpub-0.8.2/quickpub/runnables/implementations/unittest.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         set_current_working_directory(os.path.join(self._cwd, self.target))
 
     def _post_command(self):
         set_current_working_directory(self._cwd)
 
     RATING_PATTERN: re.Pattern = re.compile(r".*?([\d\.\/]+)")
 
-    def __init__(self, target: Optional[str] = "./tests") -> None:
-        CommonCheck.__init__(self, "unittest", ">=0.7", target)
+    def __init__(self, target: Optional[str] = "./tests", bound: str = ">=0.8") -> None:
+        CommonCheck.__init__(self, "unittest", bound, target)
         self._cwd = ""
 
     def _build_command(self, src: str, *args) -> str:
         command: str = self.get_executable()
         rel = os.path.relpath(src, self.target).removesuffix(src.lstrip("./\\"))
         command += f" discover -s {rel}"
         return command  # f"cd {self.target}; {command}"  # f"; cd {self.target}"
```

### Comparing `quickpub-0.8.1/quickpub/structures/bound.py` & `quickpub-0.8.2/quickpub/structures/bound.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/structures/version.py` & `quickpub-0.8.2/quickpub/structures/version.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub/validators.py` & `quickpub-0.8.2/quickpub/validators.py`

 * *Files identical despite different names*

### Comparing `quickpub-0.8.1/quickpub.egg-info/PKG-INFO` & `quickpub-0.8.2/quickpub.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickpub
-Version: 0.8.1
+Version: 0.8.2
 Summary: A python package to quickly configure and publish a new package
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,17 +50,17 @@
         author_email="danielnachumdev@gmail.com",
         description="A python package to quickly configure and publish a new package",
         homepage="https://github.com/danielnachumdev/quickpub",
         dependencies=["twine", "danielutils"],
         min_python="3.9.19",
         config=AdditionalConfiguration(
             runners=[
-                MypyRunner(),
-                PylintRunner(),
-                UnittestRunner(),
+                MypyRunner(bound="<15"),
+                PylintRunner(bound=">=0.8"),
+                UnittestRunner(bound=">=0.8"),
             ]
         )
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `quickpub-0.8.1/quickpub.egg-info/SOURCES.txt` & `quickpub-0.8.2/quickpub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

