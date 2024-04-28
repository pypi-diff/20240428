# Comparing `tmp/duty-1.2.0.tar.gz` & `tmp/duty-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duty-1.2.0.tar", last modified: Wed Jan 31 17:26:42 2024, max compression
+gzip compressed data, was "duty-1.3.0.tar", last modified: Sun Apr 28 11:33:30 2024, max compression
```

## Comparing `duty-1.2.0.tar` & `duty-1.3.0.tar`

### file list

```diff
@@ -1,45 +1,29 @@
--rw-r--r--   0        0        0      754 2024-01-18 19:13:40.750831 duty-1.2.0/LICENSE
--rw-r--r--   0        0        0     1320 2024-01-18 19:13:43.274102 duty-1.2.0/README.md
--rw-r--r--   0        0        0     2478 2024-01-31 17:26:42.327600 duty-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      144 2024-01-18 19:13:43.274102 duty-1.2.0/src/duty/__init__.py
--rw-r--r--   0        0        0      333 2024-01-18 19:13:40.897494 duty-1.2.0/src/duty/__main__.py
--rw-r--r--   0        0        0     1661 2023-04-10 14:47:07.887091 duty-1.2.0/src/duty/callables/__init__.py
--rw-r--r--   0        0        0      367 2023-04-13 14:11:08.482199 duty-1.2.0/src/duty/callables/_io.py
--rw-r--r--   0        0        0     4699 2023-04-13 14:16:42.639974 duty-1.2.0/src/duty/callables/autoflake.py
--rw-r--r--   0        0        0     7153 2023-04-10 14:49:36.264138 duty-1.2.0/src/duty/callables/black.py
--rw-r--r--   0        0        0     3221 2023-04-10 14:49:09.981212 duty-1.2.0/src/duty/callables/blacken_docs.py
--rw-r--r--   0        0        0    23843 2023-06-26 13:00:14.421342 duty-1.2.0/src/duty/callables/coverage.py
--rw-r--r--   0        0        0     8476 2023-06-26 13:00:14.418009 duty-1.2.0/src/duty/callables/flake8.py
--rw-r--r--   0        0        0     5060 2023-06-26 13:00:14.418009 duty-1.2.0/src/duty/callables/interrogate.py
--rw-r--r--   0        0        0    26437 2023-06-26 13:00:14.424676 duty-1.2.0/src/duty/callables/isort.py
--rw-r--r--   0        0        0     7902 2023-04-10 14:48:43.645095 duty-1.2.0/src/duty/callables/mkdocs.py
--rw-r--r--   0        0        0    19797 2023-07-29 12:54:54.885248 duty-1.2.0/src/duty/callables/mypy.py
--rw-r--r--   0        0        0    18345 2023-07-29 12:54:54.885248 duty-1.2.0/src/duty/callables/pytest.py
--rw-r--r--   0        0        0    13312 2023-10-25 15:48:08.558711 duty-1.2.0/src/duty/callables/ruff.py
--rw-r--r--   0        0        0     2389 2024-01-31 17:21:26.267901 duty-1.2.0/src/duty/callables/safety.py
--rw-r--r--   0        0        0      842 2023-07-29 12:54:54.885248 duty-1.2.0/src/duty/callables/ssort.py
--rw-r--r--   0        0        0     8436 2024-01-18 19:13:43.274102 duty-1.2.0/src/duty/cli.py
--rw-r--r--   0        0        0     6590 2024-01-31 17:20:51.348290 duty-1.2.0/src/duty/collection.py
--rw-r--r--   0        0        0     2985 2024-01-31 17:20:51.331623 duty-1.2.0/src/duty/context.py
--rw-r--r--   0        0        0     2683 2024-01-18 19:13:40.894161 duty-1.2.0/src/duty/debug.py
--rw-r--r--   0        0        0     2986 2024-01-31 17:22:07.087443 duty-1.2.0/src/duty/decorator.py
--rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-1.2.0/src/duty/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-18 19:13:40.894161 duty-1.2.0/src/duty/py.typed
--rw-r--r--   0        0        0     7305 2024-01-31 17:20:51.444955 duty-1.2.0/src/duty/validation.py
--rw-r--r--   0        0        0      157 2024-01-18 19:13:40.907493 duty-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2024-01-18 19:13:40.907493 duty-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0      130 2021-06-18 16:29:00.138929 duty-1.2.0/tests/fixtures/arguments.py
--rw-r--r--   0        0        0       55 2021-06-18 16:29:00.155592 duty-1.2.0/tests/fixtures/basic.py
--rw-r--r--   0        0        0      105 2021-06-18 16:29:00.155592 duty-1.2.0/tests/fixtures/booleans.py
--rw-r--r--   0        0        0       82 2021-06-18 16:29:00.172255 duty-1.2.0/tests/fixtures/code.py
--rw-r--r--   0        0        0      102 2021-06-18 16:29:00.172255 duty-1.2.0/tests/fixtures/list.py
--rw-r--r--   0        0        0      180 2021-06-18 16:29:00.182252 duty-1.2.0/tests/fixtures/multiple.py
--rw-r--r--   0        0        0      121 2021-06-18 16:29:00.182252 duty-1.2.0/tests/fixtures/precedence.py
--rw-r--r--   0        0        0      875 2023-06-27 21:07:36.016860 duty-1.2.0/tests/fixtures/validation.py
--rw-r--r--   0        0        0     7199 2024-01-18 19:13:43.274102 duty-1.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     2157 2023-04-13 14:33:11.976230 duty-1.2.0/tests/test_collection.py
--rw-r--r--   0        0        0     3417 2023-10-25 15:48:20.635084 duty-1.2.0/tests/test_context.py
--rw-r--r--   0        0        0      796 2023-04-13 14:32:18.229261 duty-1.2.0/tests/test_decorator.py
--rw-r--r--   0        0        0     3264 2023-05-18 09:12:31.970572 duty-1.2.0/tests/test_running.py
--rw-r--r--   0        0        0     4903 2023-06-27 21:42:16.266864 duty-1.2.0/tests/test_validation.py
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 duty-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-04-28 09:16:59.233481 duty-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1313 2024-04-28 09:17:01.843375 duty-1.3.0/README.md
+-rw-r--r--   0        0        0     1815 2024-04-28 11:33:30.514749 duty-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-28 09:17:01.843375 duty-1.3.0/src/duty/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-28 09:16:59.326811 duty-1.3.0/src/duty/__main__.py
+-rw-r--r--   0        0        0     1661 2023-04-10 14:47:07.887091 duty-1.3.0/src/duty/callables/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-13 14:11:08.482199 duty-1.3.0/src/duty/callables/_io.py
+-rw-r--r--   0        0        0     4699 2023-04-13 14:16:42.639974 duty-1.3.0/src/duty/callables/autoflake.py
+-rw-r--r--   0        0        0     7153 2023-04-10 14:49:36.264138 duty-1.3.0/src/duty/callables/black.py
+-rw-r--r--   0        0        0     3221 2023-04-10 14:49:09.981212 duty-1.3.0/src/duty/callables/blacken_docs.py
+-rw-r--r--   0        0        0    23843 2023-06-26 13:00:14.421342 duty-1.3.0/src/duty/callables/coverage.py
+-rw-r--r--   0        0        0     8476 2023-06-26 13:00:14.418009 duty-1.3.0/src/duty/callables/flake8.py
+-rw-r--r--   0        0        0     5060 2023-06-26 13:00:14.418009 duty-1.3.0/src/duty/callables/interrogate.py
+-rw-r--r--   0        0        0    26437 2023-06-26 13:00:14.424676 duty-1.3.0/src/duty/callables/isort.py
+-rw-r--r--   0        0        0     7902 2023-04-10 14:48:43.645095 duty-1.3.0/src/duty/callables/mkdocs.py
+-rw-r--r--   0        0        0    19797 2023-07-29 12:54:54.885248 duty-1.3.0/src/duty/callables/mypy.py
+-rw-r--r--   0        0        0    18345 2023-07-29 12:54:54.885248 duty-1.3.0/src/duty/callables/pytest.py
+-rw-r--r--   0        0        0    13312 2023-10-25 15:48:08.558711 duty-1.3.0/src/duty/callables/ruff.py
+-rw-r--r--   0        0        0     2389 2024-01-31 17:21:26.267901 duty-1.3.0/src/duty/callables/safety.py
+-rw-r--r--   0        0        0      842 2023-07-29 12:54:54.885248 duty-1.3.0/src/duty/callables/ssort.py
+-rw-r--r--   0        0        0     8436 2024-04-28 09:17:01.843375 duty-1.3.0/src/duty/cli.py
+-rw-r--r--   0        0        0     6590 2024-01-31 17:20:51.348290 duty-1.3.0/src/duty/collection.py
+-rw-r--r--   0        0        0     2985 2024-01-31 17:20:51.331623 duty-1.3.0/src/duty/context.py
+-rw-r--r--   0        0        0     2813 2024-04-28 09:16:59.320144 duty-1.3.0/src/duty/debug.py
+-rw-r--r--   0        0        0     2986 2024-01-31 17:22:07.087443 duty-1.3.0/src/duty/decorator.py
+-rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-1.3.0/src/duty/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 09:16:59.323478 duty-1.3.0/src/duty/py.typed
+-rw-r--r--   0        0        0     8052 2024-04-28 11:21:33.351666 duty-1.3.0/src/duty/validation.py
+-rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 duty-1.3.0/PKG-INFO
```

### Comparing `duty-1.2.0/LICENSE` & `duty-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/README.md` & `duty-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # duty
 
 [![ci](https://github.com/pawamoy/duty/workflows/ci/badge.svg)](https://github.com/pawamoy/duty/actions?query=workflow%3Aci)
-[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/duty/)
+[![documentation](https://img.shields.io/badge/docs-mkdocs-708FCC.svg?style=flat)](https://pawamoy.github.io/duty/)
 [![pypi version](https://img.shields.io/pypi/v/duty.svg)](https://pypi.org/project/duty/)
-[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/duty)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-708FCC.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/duty)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://app.gitter.im/#/room/#duty:gitter.im)
 
 A simple task runner.
 
 Inspired by [Invoke](https://github.com/pyinvoke/invoke).
 
 ![demo](demo.svg)
```

### Comparing `duty-1.2.0/src/duty/callables/__init__.py` & `duty-1.3.0/src/duty/callables/__init__.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/autoflake.py` & `duty-1.3.0/src/duty/callables/autoflake.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/black.py` & `duty-1.3.0/src/duty/callables/black.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/blacken_docs.py` & `duty-1.3.0/src/duty/callables/blacken_docs.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/coverage.py` & `duty-1.3.0/src/duty/callables/coverage.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/flake8.py` & `duty-1.3.0/src/duty/callables/flake8.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/interrogate.py` & `duty-1.3.0/src/duty/callables/interrogate.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/isort.py` & `duty-1.3.0/src/duty/callables/isort.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/mkdocs.py` & `duty-1.3.0/src/duty/callables/mkdocs.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/mypy.py` & `duty-1.3.0/src/duty/callables/mypy.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/pytest.py` & `duty-1.3.0/src/duty/callables/pytest.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/ruff.py` & `duty-1.3.0/src/duty/callables/ruff.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/safety.py` & `duty-1.3.0/src/duty/callables/safety.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/callables/ssort.py` & `duty-1.3.0/src/duty/callables/ssort.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/cli.py` & `duty-1.3.0/src/duty/cli.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/collection.py` & `duty-1.3.0/src/duty/collection.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/context.py` & `duty-1.3.0/src/duty/context.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/debug.py` & `duty-1.3.0/src/duty/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 class Environment:
     """Dataclass to store environment information."""
 
     interpreter_name: str
     """Python interpreter name."""
     interpreter_version: str
     """Python interpreter version."""
+    interpreter_path: str
+    """Path to Python executable."""
     platform: str
     """Operating System."""
     packages: list[Package]
     """Installed packages."""
     variables: list[Variable]
     """Environment variables."""
 
@@ -79,25 +81,26 @@
     """
     py_name, py_version = _interpreter_name_version()
     packages = ["duty"]
     variables = ["PYTHONPATH", *[var for var in os.environ if var.startswith("DUTY")]]
     return Environment(
         interpreter_name=py_name,
         interpreter_version=py_version,
+        interpreter_path=sys.executable,
         platform=platform.platform(),
         variables=[Variable(var, val) for var in variables if (val := os.getenv(var))],
         packages=[Package(pkg, get_version(pkg)) for pkg in packages],
     )
 
 
 def print_debug_info() -> None:
     """Print debug/environment information."""
     info = get_debug_info()
     print(f"- __System__: {info.platform}")
-    print(f"- __Python__: {info.interpreter_name} {info.interpreter_version}")
+    print(f"- __Python__: {info.interpreter_name} {info.interpreter_version} ({info.interpreter_path})")
     print("- __Environment variables__:")
     for var in info.variables:
         print(f"  - `{var.name}`: `{var.value}`")
     print("- __Installed packages__:")
     for pkg in info.packages:
         print(f"  - `{pkg.name}` v{pkg.version}")
```

### Comparing `duty-1.2.0/src/duty/decorator.py` & `duty-1.3.0/src/duty/decorator.py`

 * *Files identical despite different names*

### Comparing `duty-1.2.0/src/duty/validation.py` & `duty-1.3.0/src/duty/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,29 @@
 if they are incorrect.
 """
 
 from __future__ import annotations
 
 import sys
 import textwrap
+from contextlib import suppress
 from functools import cached_property
 from inspect import Parameter, Signature, signature
-from typing import Any, Callable, Sequence
+from typing import Any, Callable, ForwardRef, Sequence, Union, get_args, get_origin
+
+# TODO: Update once support for Python 3.9 is dropped.
+if sys.version_info < (3, 10):
+    from eval_type_backport import eval_type_backport as eval_type
+
+    union_types = (Union,)
+else:
+    from types import UnionType
+    from typing import _eval_type as eval_type  # type: ignore[attr-defined]
+
+    union_types = (Union, UnionType)
 
 
 def to_bool(value: str) -> bool:
     """Convert a string to a boolean.
 
     Parameters:
         value: The string to convert.
@@ -36,14 +48,20 @@
     Returns:
         The cast value.
     """
     if annotation is Parameter.empty:
         return arg
     if annotation is bool:
         annotation = to_bool
+    if get_origin(annotation) in union_types:
+        for sub_annotation in get_args(annotation):
+            if sub_annotation is type(None):
+                continue
+            with suppress(Exception):
+                return cast_arg(arg, sub_annotation)
     try:
         return annotation(arg)
     except Exception:  # noqa: BLE001
         return arg
 
 
 class ParamsCaster:
@@ -61,19 +79,17 @@
     @cached_property
     def var_positional_position(self) -> int:
         """Give the position of the variable positional parameter in the signature.
 
         Returns:
             The position of the variable positional parameter.
         """
-        pos = 0
-        for param in self.params_list:
+        for pos, param in enumerate(self.params_list):
             if param.kind is Parameter.VAR_POSITIONAL:
                 return pos
-            pos += 1
         return -1
 
     @cached_property
     def has_var_positional(self) -> bool:
         """Tell if there is a variable positional parameter.
 
         Returns:
@@ -171,30 +187,32 @@
     duties_module = sys.modules[func.__module__]
     exec_globals = dict(duties_module.__dict__)
     eval_str = False
     for name in list(exec_globals.keys()):
         if exec_globals[name] is annotations:
             eval_str = True
             del exec_globals[name]
+            break
     exec_globals["__context_above"] = {}
 
     # Don't keep first parameter: context.
     params = list(signature(func).parameters.values())[1:]
     params_no_types = [Parameter(param.name, param.kind, default=param.default) for param in params]
     code_sig = Signature(parameters=params_no_types)
     if eval_str:
         params_types = [
             Parameter(
                 param.name,
                 param.kind,
                 default=param.default,
                 annotation=(
-                    eval(  # noqa: PGH001,S307
-                        param.annotation,
+                    eval_type(
+                        ForwardRef(param.annotation) if isinstance(param.annotation, str) else param.annotation,
                         exec_globals,
+                        {},
                     )
                     if param.annotation is not Parameter.empty
                     else type(param.default)
                 ),
             )
             for param in params
         ]
```

### Comparing `duty-1.2.0/PKG-INFO` & `duty-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: duty
-Version: 1.2.0
+Version: 1.3.0
 Summary: A simple task runner.
-Keywords: task-runner task runner cross-platform
-Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
+Keywords: task-runner,task,runner,cross-platform
+Author-Email: =?utf-8?q?Timoth=C3=A9e_Mazzucotelli?= <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://pawamoy.github.io/duty
 Project-URL: Documentation, https://pawamoy.github.io/duty
 Project-URL: Changelog, https://pawamoy.github.io/duty/changelog
 Project-URL: Repository, https://github.com/pawamoy/duty
 Project-URL: Issues, https://github.com/pawamoy/duty/issues
 Project-URL: Discussions, https://github.com/pawamoy/duty/discussions
 Project-URL: Gitter, https://gitter.im/duty/community
 Project-URL: Funding, https://github.com/sponsors/pawamoy
 Requires-Python: >=3.8
+Requires-Dist: eval-type-backport; python_version < "3.10"
 Requires-Dist: failprint!=1.0.0,>=0.11
 Description-Content-Type: text/markdown
 
 # duty
 
 [![ci](https://github.com/pawamoy/duty/workflows/ci/badge.svg)](https://github.com/pawamoy/duty/actions?query=workflow%3Aci)
-[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/duty/)
+[![documentation](https://img.shields.io/badge/docs-mkdocs-708FCC.svg?style=flat)](https://pawamoy.github.io/duty/)
 [![pypi version](https://img.shields.io/pypi/v/duty.svg)](https://pypi.org/project/duty/)
-[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/duty)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-708FCC.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/duty)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://app.gitter.im/#/room/#duty:gitter.im)
 
 A simple task runner.
 
 Inspired by [Invoke](https://github.com/pyinvoke/invoke).
 
 ![demo](demo.svg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

