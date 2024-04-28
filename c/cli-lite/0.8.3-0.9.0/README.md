# Comparing `tmp/cli-lite-0.8.3.tar.gz` & `tmp/cli_lite-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-lite-0.8.3.tar", last modified: Thu Jan  4 03:29:54 2024, max compression
+gzip compressed data, was "cli_lite-0.9.0.tar", last modified: Sun Apr 28 14:27:01 2024, max compression
```

## Comparing `cli-lite-0.8.3.tar` & `cli_lite-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      160 2023-05-12 07:56:09.908946 cli-lite-0.8.3/clilte/__init__.py
--rw-r--r--   0        0        0     2484 2023-12-12 07:51:09.695213 cli-lite-0.8.3/clilte/builtin.py
--rw-r--r--   0        0        0    10789 2024-01-04 03:24:57.697949 cli-lite-0.8.3/clilte/core.py
--rw-r--r--   0        0        0     1092 2022-07-03 16:27:16.504000 cli-lite-0.8.3/LICENSE
--rw-r--r--   0        0        0     1174 2024-01-04 03:28:46.919548 cli-lite-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1073 2023-12-12 07:54:02.156789 cli-lite-0.8.3/README.md
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 cli-lite-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-28 14:08:50.772385 cli_lite-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1073 2024-04-28 14:08:50.772385 cli_lite-0.9.0/README.md
+-rw-r--r--   0        0        0      160 2024-04-28 14:08:50.772385 cli_lite-0.9.0/clilte/__init__.py
+-rw-r--r--   0        0        0     2484 2024-04-28 14:08:50.772385 cli_lite-0.9.0/clilte/builtin.py
+-rw-r--r--   0        0        0    10872 2024-04-28 14:15:29.310161 cli_lite-0.9.0/clilte/core.py
+-rw-r--r--   0        0        0     1164 2024-04-28 14:27:01.636374 cli_lite-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 cli_lite-0.9.0/PKG-INFO
```

### Comparing `cli-lite-0.8.3/clilte/builtin.py` & `cli_lite-0.9.0/clilte/builtin.py`

 * *Files identical despite different names*

### Comparing `cli-lite-0.8.3/clilte/core.py` & `cli_lite-0.9.0/clilte/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,18 @@
     author: list[str] = field(default_factory=list)
     priority: int = field(default=16)
 
 
 class BasePlugin(metaclass=ABCMeta):
     def __init__(self):
         self.metadata: PluginMetadata = self.meta()
-        self.command: Alconna | str = self.init()
-        if isinstance(self.command, Alconna):
-            self.name: str = self.command.name
+        command = self.init()
+        if isinstance(command, Alconna):
+            self.name: str = command.name
+            self.command: Alconna = command
             if (
                 not self.command.meta.description
                 or self.command.meta.description == "Unknown"
             ):
                 self.command.meta.description = self.metadata.description or self.metadata.name or "Unknown"
             if (
                 not self.command.help_text
@@ -77,15 +78,15 @@
             )
             self.command.meta.raise_exception = (
                 ns.raise_exception or self.command.meta.raise_exception
             )
             self.command._hash = self.command._calc_hash()
             command_manager.register(self.command)
         else:
-            self.name: str = self.command
+            self.name: str = command
 
     @property
     def local(self):
         """以插件所在的模块名作为子命令的名称"""
         module = self.__module__.split(".")[-1]
         if module == "__main__":
             return handle_argv()
@@ -197,15 +198,15 @@
         self.callback = callback
 
     def add(self, *command: type[TPlugin]):
         with self.using():
             res: list[TPlugin] = [cls() for cls in command]
         for plg in res:
             self.plugins[plg.name] = plg
-            if isinstance(plg.command, Alconna):
+            if hasattr(plg, "command") and isinstance(plg.command, Alconna):
                 self._command.add(plg.command)
             if _opts := plg.supply_options():
                 for _opt in _opts:
                     self._command.add(_opt)
         return res
 
     def preset(self):
@@ -226,31 +227,31 @@
         if isinstance(name, Path):
             module = importlib.import_module(".".join(name.parts[:-1] + (name.stem,)))
             for _, plug in inspect.getmembers(
                 module, lambda x: isinstance(x, type) and issubclass(x, BasePlugin)
             ):
                 if plug is BasePlugin:
                     continue
-                self.add(plug)
+                self.add(plug)  # type: ignore
             return
         match = pattern.match(name)
         if not match:
             raise ModuleNotFoundError(name)
         module = importlib.import_module(match.group("module"))
         if not match.group("attr"):
             for _, plug in inspect.getmembers(
                 module, lambda x: isinstance(x, type) and issubclass(x, BasePlugin)
             ):
                 if plug is BasePlugin:
                     continue
-                self.add(plug)
+                self.add(plug)  # type: ignore
             return
         attrs = filter(None, (match.group("attr") or "").split("."))
         plug = functools.reduce(getattr, attrs, module)
-        if not issubclass(plug, BasePlugin):
+        if not issubclass(plug, BasePlugin):  # type: ignore
             raise TypeError(f"target {plug} is not a plugin")
         self.add(plug)
 
     def load_plugins(self, dirname: str | Path):
         dir_path = Path(dirname)
         if not dir_path.exists():
             raise FileNotFoundError(f"directory {dirname} not exists")
@@ -270,15 +271,15 @@
 
     @overload
     def get_plugin(self, plg: type[TPlugin], default: Literal[True]) -> TPlugin:
         ...
 
     def get_plugin(self, plg: type[TPlugin], default: bool = False) -> TPlugin | None:
         return next(
-            filter(lambda x: isinstance(x, plg), self.plugins.values()),
+            (x for x in self.plugins.values() if isinstance(x, plg)),
             self.add(plg)[0] if default else None,
         )
 
     def query(self, *tag: str):
         yield from filter(
             lambda x: set(x.metadata.tags).issuperset(tag), self.plugins.values()
         )
```

### Comparing `cli-lite-0.8.3/LICENSE` & `cli_lite-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-lite-0.8.3/pyproject.toml` & `cli_lite-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "cli-lite"
-version = "0.8.3"
+version = "0.9.0"
 description = "A simple framework to build a cli tool, base on Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "arclet-alconna>=1.7.39",
-    "arclet-alconna-tools>=0.6.10",
+    "arclet-alconna>=1.8.11",
+    "arclet-alconna-tools>=0.7.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "commandline",
     "cli-tool",
     "plugin",
@@ -44,10 +44,10 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "fix-future-annotations>=0.5.0",
 ]
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm.backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `cli-lite-0.8.3/README.md` & `cli_lite-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cli-lite-0.8.3/PKG-INFO` & `cli_lite-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: cli-lite
-Version: 0.8.3
+Version: 0.9.0
 Summary: A simple framework to build a cli tool, base on Alconna
-License: MIT
 Keywords: commandline,cli-tool,plugin,cli,litecli
-Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
-Requires-Python: >=3.8
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
+License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Bug Reports, https://github.com/RF-Tar-Railt/cli-lite/issues
 Project-URL: Homepage, https://github.com/RF-Tar-Railt/cli-lite
+Project-URL: Bug reports, https://github.com/RF-Tar-Railt/cli-lite/issues
 Project-URL: Source, https://github.com/RF-Tar-Railt/cli-lite
+Requires-Python: >=3.8
+Requires-Dist: arclet-alconna>=1.8.11
+Requires-Dist: arclet-alconna-tools>=0.7.3
 Description-Content-Type: text/markdown
 
 # Cli-Lite
 
 A simple framework to build a cli tool. Base on [`Alconna`](https://github.com/ArcletProject/Alconna)
 
 ## install
@@ -65,8 +67,7 @@
 
 you will get the result:
 
 ```shell
 Hello! world
 ```
 
-
```

