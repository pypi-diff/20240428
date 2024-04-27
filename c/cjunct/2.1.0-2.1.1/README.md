# Comparing `tmp/cjunct-2.1.0.tar.gz` & `tmp/cjunct-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjunct-2.1.0.tar", max compression
+gzip compressed data, was "cjunct-2.1.1.tar", max compression
```

## Comparing `cjunct-2.1.0.tar` & `cjunct-2.1.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.1.0/LICENSE
--rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.1.0/README.md
--rw-r--r--   0        0        0     4651 2024-04-10 14:13:33.921498 cjunct-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.1.0/src/cjunct/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.1.0/src/cjunct/actions/__init__.py
--rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.1.0/src/cjunct/actions/base.py
--rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.1.0/src/cjunct/actions/bundled/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.1.0/src/cjunct/actions/bundled/docker_shell.py
--rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.1.0/src/cjunct/actions/bundled/echo.py
--rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.1.0/src/cjunct/actions/bundled/shell.py
--rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.1.0/src/cjunct/actions/constants.py
--rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.1.0/src/cjunct/actions/types.py
--rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.1.0/src/cjunct/config/__init__.py
--rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.1.0/src/cjunct/config/constants/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.1.0/src/cjunct/config/constants/cli.py
--rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.1.0/src/cjunct/config/constants/helpers.py
--rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.1.0/src/cjunct/config/environment.py
--rw-r--r--   0        0        0     4644 2024-04-08 10:02:51.818144 cjunct-2.1.0/src/cjunct/console.py
--rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.1.0/src/cjunct/display/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.1.0/src/cjunct/display/base.py
--rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.1.0/src/cjunct/display/color.py
--rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.1.0/src/cjunct/display/default.py
--rw-r--r--   0        0        0     1597 2024-04-10 14:13:33.922149 cjunct-2.1.0/src/cjunct/exceptions.py
--rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.1.0/src/cjunct/loader/__init__.py
--rw-r--r--   0        0        0     9373 2024-04-10 14:13:33.923249 cjunct-2.1.0/src/cjunct/loader/base.py
--rw-r--r--   0        0        0     7183 2024-04-10 14:13:33.923931 cjunct-2.1.0/src/cjunct/loader/default.py
--rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.1.0/src/cjunct/loader/helpers.py
--rw-r--r--   0        0        0     1931 2024-04-08 10:02:51.831758 cjunct-2.1.0/src/cjunct/loader/inspect.py
--rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.1.0/src/cjunct/py.typed
--rw-r--r--   0        0        0     4917 2024-04-10 14:13:33.924720 cjunct-2.1.0/src/cjunct/rendering/__init__.py
--rw-r--r--   0        0        0      100 2024-04-10 14:13:33.925246 cjunct-2.1.0/src/cjunct/rendering/constants.py
--rw-r--r--   0        0        0     2372 2024-04-10 14:13:33.925738 cjunct-2.1.0/src/cjunct/rendering/containers.py
--rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.1.0/src/cjunct/rendering/tokenizing.py
--rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.1.0/src/cjunct/runner.py
--rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.1.0/src/cjunct/strategy.py
--rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.1.0/src/cjunct/types.py
--rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.1.0/src/cjunct/version.py
--rw-r--r--   0        0        0     4262 2024-04-10 14:13:33.926361 cjunct-2.1.0/src/cjunct/workflow.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.1.1/README.md
+-rw-r--r--   0        0        0     4686 2024-04-27 22:43:02.399592 cjunct-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.1.1/src/cjunct/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.1.1/src/cjunct/actions/__init__.py
+-rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.1.1/src/cjunct/actions/base.py
+-rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.1.1/src/cjunct/actions/bundled/__init__.py
+-rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.1.1/src/cjunct/actions/bundled/docker_shell.py
+-rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.1.1/src/cjunct/actions/bundled/echo.py
+-rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.1.1/src/cjunct/actions/bundled/shell.py
+-rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.1.1/src/cjunct/actions/constants.py
+-rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.1.1/src/cjunct/actions/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.1.1/src/cjunct/config/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.1.1/src/cjunct/config/constants/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.1.1/src/cjunct/config/constants/cli.py
+-rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.1.1/src/cjunct/config/constants/helpers.py
+-rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.1.1/src/cjunct/config/environment.py
+-rw-r--r--   0        0        0     5583 2024-04-27 22:43:02.403087 cjunct-2.1.1/src/cjunct/console.py
+-rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.1.1/src/cjunct/display/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.1.1/src/cjunct/display/base.py
+-rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.1.1/src/cjunct/display/color.py
+-rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.1.1/src/cjunct/display/default.py
+-rw-r--r--   0        0        0     1597 2024-04-10 14:13:33.922149 cjunct-2.1.1/src/cjunct/exceptions.py
+-rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.1.1/src/cjunct/loader/__init__.py
+-rw-r--r--   0        0        0     9380 2024-04-27 22:43:15.282638 cjunct-2.1.1/src/cjunct/loader/base.py
+-rw-r--r--   0        0        0     7183 2024-04-10 14:13:33.923931 cjunct-2.1.1/src/cjunct/loader/default.py
+-rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.1.1/src/cjunct/loader/helpers.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.1.1/src/cjunct/py.typed
+-rw-r--r--   0        0        0     4917 2024-04-10 14:13:33.924720 cjunct-2.1.1/src/cjunct/rendering/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-10 14:13:33.925246 cjunct-2.1.1/src/cjunct/rendering/constants.py
+-rw-r--r--   0        0        0     2372 2024-04-10 14:13:33.925738 cjunct-2.1.1/src/cjunct/rendering/containers.py
+-rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.1.1/src/cjunct/rendering/tokenizing.py
+-rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.1.1/src/cjunct/runner.py
+-rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.1.1/src/cjunct/strategy.py
+-rw-r--r--   0        0        0     1911 2024-04-27 22:36:27.848112 cjunct-2.1.1/src/cjunct/tools/inspect.py
+-rw-r--r--   0        0        0     1348 2024-04-27 22:57:28.402560 cjunct-2.1.1/src/cjunct/tools/proxy.py
+-rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.1.1/src/cjunct/types.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.1.1/src/cjunct/version.py
+-rw-r--r--   0        0        0     4262 2024-04-10 14:13:33.926361 cjunct-2.1.1/src/cjunct/workflow.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.1.1/PKG-INFO
```

### Comparing `cjunct-2.1.0/LICENSE` & `cjunct-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/README.md` & `cjunct-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/pyproject.toml` & `cjunct-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjunct"
-version = "2.1.0"
+version = "2.1.1"
 description = "Declarative task runner"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/cjunct"
@@ -70,14 +70,15 @@
     "ignore:.*:builtins.DeprecationWarning",
 ]
 
 [tool.coverage.run]
 source = ["src"]
 omit = [
     "src/cjunct/console.py",
+    "src/cjunct/tools/inspect.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
     "def __str__",
```

### Comparing `cjunct-2.1.0/src/cjunct/__init__.py` & `cjunct-2.1.1/src/cjunct/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/actions/base.py` & `cjunct-2.1.1/src/cjunct/actions/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/actions/bundled/docker_shell.py` & `cjunct-2.1.1/src/cjunct/actions/bundled/docker_shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/actions/bundled/shell.py` & `cjunct-2.1.1/src/cjunct/actions/bundled/shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/config/constants/__init__.py` & `cjunct-2.1.1/src/cjunct/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/config/constants/cli.py` & `cjunct-2.1.1/src/cjunct/config/constants/cli.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/config/constants/helpers.py` & `cjunct-2.1.1/src/cjunct/config/constants/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/config/environment.py` & `cjunct-2.1.1/src/cjunct/config/environment.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/console.py` & `cjunct-2.1.1/src/cjunct/console.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Command-line interface entry"""
 
 import functools
+import os
 import sys
 import typing as t
 from pathlib import Path
 
 import classlogging
 import click
-import dotenv
+from dotenv.main import DotEnv
 
 import cjunct
 from cjunct.config.constants import C, LOG_LEVELS
 from cjunct.config.constants.cli import cliargs_receiver
 from cjunct.config.environment import Env
 from cjunct.exceptions import BaseError, ExecutionFailed
 from cjunct.strategy import KNOWN_STRATEGIES
+from cjunct.tools.proxy import DeferredCallsProxy
 
-logger = classlogging.get_module_logger()
+logger = DeferredCallsProxy(obj=classlogging.get_module_logger())
 
 
 class WorkflowPositionalArgument(click.Argument):
     """Optional positional argument for the workflow source"""
 
     NAME: str = "WORKFLOW"
 
@@ -59,33 +61,55 @@
     type=click.Choice(list(LOG_LEVELS)),
 )
 @cliargs_receiver
 def main() -> None:
     """Declarative task runner"""
 
 
+def load_dotenv() -> None:
+    """Try loading environment from the dotenv file.
+    Special variable called "HERE" is injected into the environment during dotenv loading,
+    which points to the directory of the dotenv file (if not specified in advance)."""
+    here_var_name: str = "HERE"
+    here_value_was_defined: bool = here_var_name in os.environ
+    dotenv_path: Path = C.ENV_FILE
+    if not here_value_was_defined:
+        os.environ[here_var_name] = str(dotenv_path.parent)
+    else:
+        logger.debug(f"{here_var_name!r} was set externally")
+    try:
+        dotenv = DotEnv(dotenv_path=dotenv_path)
+        if here_var_name in dotenv.dict():
+            logger.debug(f"{here_var_name!r} is explicitly set via dotenv file")
+            here_value_was_defined = True
+        if dotenv.set_as_environment_variables():
+            logger.info(f"Loaded environment variables from {str(dotenv_path)!r}")
+        else:
+            logger.debug(f"Dotenv not found: {str(dotenv_path)!r}")
+
+    finally:
+        if not here_value_was_defined:
+            os.environ.pop(here_var_name)
+
+
 def wrap_cli_command(func):
     """Standard loading and error handling"""
 
     @main.command
     @cliargs_receiver
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
-        dotenv_path: Path = C.ENV_FILE
-        dotenv_loaded: bool = dotenv.load_dotenv(dotenv_path=dotenv_path)
+        load_dotenv()
         classlogging.configure_logging(
             level=C.LOG_LEVEL,
             colorize=C.USE_COLOR and not C.LOG_FILE,
             main_file=C.LOG_FILE,
             stream=None if C.LOG_FILE else classlogging.LogStream.STDERR,
         )
-        if dotenv_loaded:
-            logger.info(f"Loaded environment variables from {str(dotenv_path)!r}")
-        else:
-            logger.debug(f"Dotenv not found: {dotenv_path!r}")
+        logger.uncork()
         try:
             return func(*args, **kwargs)
         except BaseError as e:
             logger.debug("", exc_info=True)
             sys.stderr.write(f"! {e}\n")
             sys.exit(e.CODE)
         except ExecutionFailed:
```

### Comparing `cjunct-2.1.0/src/cjunct/display/base.py` & `cjunct-2.1.1/src/cjunct/display/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/display/color.py` & `cjunct-2.1.1/src/cjunct/display/color.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/display/default.py` & `cjunct-2.1.1/src/cjunct/display/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/exceptions.py` & `cjunct-2.1.1/src/cjunct/exceptions.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/loader/base.py` & `cjunct-2.1.1/src/cjunct/loader/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import typing as t
 from enum import Enum
 from pathlib import Path
 
 import dacite
 from classlogging import LoggerMixin
 
-from .inspect import get_class_annotations
 from ..actions.base import ActionBase, ArgsBase, ActionDependency
 from ..actions.types import StringTemplate
 from ..exceptions import LoadError
+from ..tools.inspect import get_class_annotations
 from ..workflow import Workflow
 
 __all__ = [
     "AbstractBaseWorkflowLoader",
 ]
```

### Comparing `cjunct-2.1.0/src/cjunct/loader/default.py` & `cjunct-2.1.1/src/cjunct/loader/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/loader/helpers.py` & `cjunct-2.1.1/src/cjunct/loader/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/loader/inspect.py` & `cjunct-2.1.1/src/cjunct/tools/inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __all__ = [
     "get_class_annotations",
 ]
 
 OptionalDict = t.Optional[t.Dict[str, t.Any]]
 
 
-def get_class_annotations(obj: t.Any) -> t.Dict[str, t.Any]:  # pragma: no cover
+def get_class_annotations(obj: t.Any) -> t.Dict[str, t.Any]:
     """Different pythons hold __annotations__ attribute values as strings or real types, depending on the version."""
     # Resolve class first
     class_definition: type = obj if isinstance(obj, type) else obj.__class__
     class_dict: OptionalDict = getattr(class_definition, "__dict__", None)
     annotations_source: OptionalDict = None
     if class_dict is not None and hasattr(class_dict, "get"):
         annotations_source = class_dict.get("__annotations__", None)
```

### Comparing `cjunct-2.1.0/src/cjunct/rendering/__init__.py` & `cjunct-2.1.1/src/cjunct/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/rendering/containers.py` & `cjunct-2.1.1/src/cjunct/rendering/containers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/rendering/tokenizing.py` & `cjunct-2.1.1/src/cjunct/rendering/tokenizing.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/runner.py` & `cjunct-2.1.1/src/cjunct/runner.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/strategy.py` & `cjunct-2.1.1/src/cjunct/strategy.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/src/cjunct/workflow.py` & `cjunct-2.1.1/src/cjunct/workflow.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.0/PKG-INFO` & `cjunct-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjunct
-Version: 2.1.0
+Version: 2.1.1
 Summary: Declarative task runner
 Home-page: https://github.com/reartnew/cjunct
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 4 - Beta
```

