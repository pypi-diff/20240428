# Comparing `tmp/async_shell-1.0.4.tar.gz` & `tmp/async_shell-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_shell-1.0.4.tar", max compression
+gzip compressed data, was "async_shell-1.0.5.tar", max compression
```

## Comparing `async_shell-1.0.4.tar` & `async_shell-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:40:06.000000 async_shell-1.0.4/LICENSE
--rw-r--r--   0        0        0      112 2023-01-23 11:42:18.000000 async_shell-1.0.4/README.md
--rw-r--r--   0        0        0     3826 2024-03-15 12:12:05.052695 async_shell-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     6174 2024-03-15 12:18:01.383068 async_shell-1.0.4/src/async_shell/__init__.py
--rw-r--r--   0        0        0      172 2023-02-05 15:45:42.000000 async_shell-1.0.4/src/async_shell/constants.py
--rw-r--r--   0        0        0        0 2023-01-23 11:40:06.000000 async_shell-1.0.4/src/async_shell/py.typed
--rw-r--r--   0        0        0      328 2023-01-23 11:40:06.000000 async_shell-1.0.4/src/async_shell/version.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 async_shell-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:40:06.000000 async_shell-1.0.5/LICENSE
+-rw-r--r--   0        0        0      112 2023-01-23 11:42:18.000000 async_shell-1.0.5/README.md
+-rw-r--r--   0        0        0     3826 2024-03-15 12:47:12.827680 async_shell-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6283 2024-03-15 12:45:34.550643 async_shell-1.0.5/src/async_shell/__init__.py
+-rw-r--r--   0        0        0      172 2023-02-05 15:45:42.000000 async_shell-1.0.5/src/async_shell/constants.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:40:06.000000 async_shell-1.0.5/src/async_shell/py.typed
+-rw-r--r--   0        0        0      328 2023-01-23 11:40:06.000000 async_shell-1.0.5/src/async_shell/version.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 async_shell-1.0.5/PKG-INFO
```

### Comparing `async_shell-1.0.4/LICENSE` & `async_shell-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_shell-1.0.4/pyproject.toml` & `async_shell-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-shell"
-version = "1.0.4"
+version = "1.0.5"
 description = "Asyncio subprocess shell command wrapper"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/async-shell"
```

### Comparing `async_shell-1.0.4/src/async_shell/__init__.py` & `async_shell-1.0.5/src/async_shell/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,23 +66,25 @@
     MISSING_PROCESS_PID: int = -1
 
     def __init__(
         self,
         command: str,
         encoding: t.Optional[str] = None,
         environment: t.Optional[t.Dict[str, str]] = None,
+        cwd: t.Optional[str] = None,
     ) -> None:
         self._command: str = command
         self._proc: t.Optional[Process] = None
         self._encoding: str = encoding or self._DEFAULT_ENCODING
         self._start_time: t.Optional[float] = None
         self._post_validate: bool = False
         self._was_stopped: bool = False
         self._was_finalized: bool = False
         self._env: t.Optional[t.Dict[str, str]] = environment
+        self._cwd: t.Optional[str] = cwd
 
     @property
     def was_stopped(self) -> bool:
         """Tell if the process was stopped during execution"""
         return self._was_stopped
 
     @property
@@ -101,14 +103,15 @@
             self.logger.trace(f"Starting subprocess: {self._command!r}")
             self._proc = await create_subprocess_shell(
                 cmd=self._command,
                 stdin=None,
                 stdout=PIPE,
                 stderr=PIPE,
                 env=self._env,
+                cwd=self._cwd,
             )
             self.logger.debug(f"Started process with PID {self.pid}")
         return self._proc
 
     async def read_stdout(self, strip_linesep: bool = True) -> t.AsyncGenerator[str, None]:
         """Run through stdout data and yield decoded strings line by line"""
         proc: Process = await self._get_proc()
```

### Comparing `async_shell-1.0.4/PKG-INFO` & `async_shell-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-shell
-Version: 1.0.4
+Version: 1.0.5
 Summary: Asyncio subprocess shell command wrapper
 Home-page: https://github.com/reartnew/async-shell
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

