# Comparing `tmp/cjunct-2.1.2.tar.gz` & `tmp/cjunct-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjunct-2.1.2.tar", max compression
+gzip compressed data, was "cjunct-2.1.3.tar", max compression
```

## Comparing `cjunct-2.1.2.tar` & `cjunct-2.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.1.2/LICENSE
--rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.1.2/README.md
--rw-r--r--   0        0        0     4686 2024-04-27 23:25:29.362797 cjunct-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      512 2024-04-28 00:22:48.250391 cjunct-2.1.2/src/cjunct/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.1.2/src/cjunct/actions/__init__.py
--rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.1.2/src/cjunct/actions/base.py
--rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.1.2/src/cjunct/actions/bundled/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.1.2/src/cjunct/actions/bundled/docker_shell.py
--rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.1.2/src/cjunct/actions/bundled/echo.py
--rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.1.2/src/cjunct/actions/bundled/shell.py
--rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.1.2/src/cjunct/actions/constants.py
--rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.1.2/src/cjunct/actions/types.py
--rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.1.2/src/cjunct/config/__init__.py
--rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.1.2/src/cjunct/config/constants/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.1.2/src/cjunct/config/constants/cli.py
--rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.1.2/src/cjunct/config/constants/helpers.py
--rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.1.2/src/cjunct/config/environment.py
--rw-r--r--   0        0        0     5583 2024-04-27 22:43:02.403087 cjunct-2.1.2/src/cjunct/console.py
--rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.1.2/src/cjunct/display/__init__.py
--rw-r--r--   0        0        0     1281 2024-04-27 23:03:46.470627 cjunct-2.1.2/src/cjunct/display/base.py
--rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.1.2/src/cjunct/display/color.py
--rw-r--r--   0        0        0     4619 2024-04-27 23:12:24.609622 cjunct-2.1.2/src/cjunct/display/default.py
--rw-r--r--   0        0        0     1597 2024-04-10 14:13:33.922149 cjunct-2.1.2/src/cjunct/exceptions.py
--rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.1.2/src/cjunct/loader/__init__.py
--rw-r--r--   0        0        0     9380 2024-04-27 22:43:15.282638 cjunct-2.1.2/src/cjunct/loader/base.py
--rw-r--r--   0        0        0     7183 2024-04-10 14:13:33.923931 cjunct-2.1.2/src/cjunct/loader/default.py
--rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.1.2/src/cjunct/loader/helpers.py
--rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.1.2/src/cjunct/py.typed
--rw-r--r--   0        0        0     4917 2024-04-10 14:13:33.924720 cjunct-2.1.2/src/cjunct/rendering/__init__.py
--rw-r--r--   0        0        0      100 2024-04-10 14:13:33.925246 cjunct-2.1.2/src/cjunct/rendering/constants.py
--rw-r--r--   0        0        0     2372 2024-04-10 14:13:33.925738 cjunct-2.1.2/src/cjunct/rendering/containers.py
--rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.1.2/src/cjunct/rendering/tokenizing.py
--rw-r--r--   0        0        0     9973 2024-04-28 00:25:16.465588 cjunct-2.1.2/src/cjunct/runner.py
--rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.1.2/src/cjunct/strategy.py
--rw-r--r--   0        0        0     1911 2024-04-27 22:36:27.848112 cjunct-2.1.2/src/cjunct/tools/inspect.py
--rw-r--r--   0        0        0     1348 2024-04-27 22:57:28.402560 cjunct-2.1.2/src/cjunct/tools/proxy.py
--rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.1.2/src/cjunct/types.py
--rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.1.2/src/cjunct/version.py
--rw-r--r--   0        0        0     4262 2024-04-10 14:13:33.926361 cjunct-2.1.2/src/cjunct/workflow.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.1.3/LICENSE
+-rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.1.3/README.md
+-rw-r--r--   0        0        0     4686 2024-04-28 14:34:24.073342 cjunct-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-04-28 00:22:48.250391 cjunct-2.1.3/src/cjunct/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.1.3/src/cjunct/actions/__init__.py
+-rw-r--r--   0        0        0    10641 2024-04-28 16:14:13.923783 cjunct-2.1.3/src/cjunct/actions/base.py
+-rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.1.3/src/cjunct/actions/bundled/__init__.py
+-rw-r--r--   0        0        0     6698 2024-04-28 14:20:56.193590 cjunct-2.1.3/src/cjunct/actions/bundled/docker_shell.py
+-rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.1.3/src/cjunct/actions/bundled/echo.py
+-rw-r--r--   0        0        0     2256 2024-04-28 14:20:56.180345 cjunct-2.1.3/src/cjunct/actions/bundled/shell.py
+-rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.1.3/src/cjunct/actions/constants.py
+-rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.1.3/src/cjunct/actions/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.1.3/src/cjunct/config/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.1.3/src/cjunct/config/constants/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.1.3/src/cjunct/config/constants/cli.py
+-rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.1.3/src/cjunct/config/constants/helpers.py
+-rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.1.3/src/cjunct/config/environment.py
+-rw-r--r--   0        0        0     5583 2024-04-27 22:43:02.403087 cjunct-2.1.3/src/cjunct/console.py
+-rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.1.3/src/cjunct/display/__init__.py
+-rw-r--r--   0        0        0     1281 2024-04-27 23:03:46.470627 cjunct-2.1.3/src/cjunct/display/base.py
+-rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.1.3/src/cjunct/display/color.py
+-rw-r--r--   0        0        0     4636 2024-04-28 19:15:16.186627 cjunct-2.1.3/src/cjunct/display/default.py
+-rw-r--r--   0        0        0     1597 2024-04-10 14:13:33.922149 cjunct-2.1.3/src/cjunct/exceptions.py
+-rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.1.3/src/cjunct/loader/__init__.py
+-rw-r--r--   0        0        0     9380 2024-04-27 22:43:15.282638 cjunct-2.1.3/src/cjunct/loader/base.py
+-rw-r--r--   0        0        0     7183 2024-04-10 14:13:33.923931 cjunct-2.1.3/src/cjunct/loader/default.py
+-rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.1.3/src/cjunct/loader/helpers.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.1.3/src/cjunct/py.typed
+-rw-r--r--   0        0        0     4917 2024-04-10 14:13:33.924720 cjunct-2.1.3/src/cjunct/rendering/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-10 14:13:33.925246 cjunct-2.1.3/src/cjunct/rendering/constants.py
+-rw-r--r--   0        0        0     2372 2024-04-10 14:13:33.925738 cjunct-2.1.3/src/cjunct/rendering/containers.py
+-rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.1.3/src/cjunct/rendering/tokenizing.py
+-rw-r--r--   0        0        0     9973 2024-04-28 00:25:16.465588 cjunct-2.1.3/src/cjunct/runner.py
+-rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.1.3/src/cjunct/strategy.py
+-rw-r--r--   0        0        0     1911 2024-04-27 22:36:27.848112 cjunct-2.1.3/src/cjunct/tools/inspect.py
+-rw-r--r--   0        0        0     1348 2024-04-27 22:57:28.402560 cjunct-2.1.3/src/cjunct/tools/proxy.py
+-rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.1.3/src/cjunct/types.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.1.3/src/cjunct/version.py
+-rw-r--r--   0        0        0     4262 2024-04-10 14:13:33.926361 cjunct-2.1.3/src/cjunct/workflow.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.1.3/PKG-INFO
```

### Comparing `cjunct-2.1.2/LICENSE` & `cjunct-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/README.md` & `cjunct-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/pyproject.toml` & `cjunct-2.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjunct"
-version = "2.1.2"
+version = "2.1.3"
 description = "Declarative task runner"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/cjunct"
@@ -20,15 +20,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.13"
 named-env = "^2.3.2"
 classlogging = "^1.1.1"
 python-dotenv = "^1.0.1"
-async-shell = "^1.0.5"
+async-shell = "^1.0.6"
 pyyaml = "^6.0.1"
 click = "^8.1.7"
 dacite = "^1.8.1"
 inquirer = "^3.2.3"
 aiodocker = { version = "^0.21.0", optional = true }
 
 [tool.poetry.extras]
```

### Comparing `cjunct-2.1.2/src/cjunct/__init__.py` & `cjunct-2.1.3/src/cjunct/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/actions/base.py` & `cjunct-2.1.3/src/cjunct/actions/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -226,48 +226,72 @@
         return self.get_future().done() or self._status in (ActionStatus.SKIPPED, ActionStatus.OMITTED)
 
 
 # pylint: disable=abstract-method
 class EmissionScannerActionBase(ActionBase):
     """Base class for stream-scanning actions"""
 
-    _YIELD_SCAN_PATTERN: t.ClassVar[t.Pattern] = re.compile(r"^(.*?)##cjunct\[yield-outcome-b64\s*(\S+)\s+(\S*)\s*]##$")
-    _YIELD_SHELL_FUNCTION_DEFINITION: str = textwrap.dedent(
+    _SERVICE_MESSAGES_SCAN_PATTERN: t.ClassVar[t.Pattern] = re.compile(
+        r"""^
+          (.*?)  # possible preceding content
+          \#\#cjunct\[  # message prefix
+            ([A-Za-z0-9+/=\- ]+)  # message itself
+          ]\#\#  # message suffix
+        $""",
+        re.VERBOSE,
+    )
+    _SHELL_SERVICE_FUNCTIONS_DEFINITIONS: str = textwrap.dedent(
         r"""
             yield_outcome(){
               [ "$1" = "" ] && echo "Missing key (first argument)" && return 1
               command -v base64 >/dev/null || ( echo "Missing command: base64" && return 2 )
               [ "$2" = "" ] && value="$(cat /dev/stdin)" || value="$2"
               echo "##cjunct[yield-outcome-b64 $(
                 printf "$1" | base64 | tr -d '\n'
               ) $(
                 printf "$value" | base64 | tr -d '\n'
               )]##"
               return 0
             }
+            skip(){
+              echo "##cjunct[skip]##"
+              exit 0
+            }
         """
     ).lstrip()
 
+    def _process_service_message_expression(self, expression: str) -> None:
+        try:
+            expression_type, *encoded_args = expression.split()
+            decoded_args: t.List[str] = [base64.b64decode(part, validate=True).decode() for part in encoded_args]
+            if expression_type == "skip":
+                self.skip()
+            elif expression_type == "yield-outcome-b64":
+                key, value = decoded_args
+                self.logger.debug(f"Action {self.name!r} emission stream " f"reported an outcome: {key!r}")
+                self.yield_outcome(key, value)
+                return
+            else:
+                raise ValueError(f"Unrecognized expression: {expression!r}")
+        except ActionSkip:  # pylint: disable=try-except-raise
+            raise
+        except Exception:
+            self.logger.warning("Failed while parsing system message", exc_info=True)
+
     def emit(self, message: EventType) -> None:
         # Do not check stderr
         if isinstance(message, Stderr):
             super().emit(message)
             return
         memorized_prefix: str = ""
         for line in message.splitlines():
             # `endswith` is a cheaper check than re.findall
-            if line.endswith("]##") and (matches := self._YIELD_SCAN_PATTERN.findall(line)):
-                try:
-                    for preceding_content, encoded_key, encoded_value in matches:
-                        memorized_prefix += preceding_content
-                        self.logger.debug(f"Action {self.name!r} emission stream reported an outcome: {encoded_key!r}")
-                        key: str = base64.b64decode(encoded_key, validate=True).decode()
-                        value: str = base64.b64decode(encoded_value, validate=True).decode()
-                        self.yield_outcome(key, value)
-                except Exception:
-                    self.logger.warning("Failed while parsing system message", exc_info=True)
-            else:
+            if not line.endswith("]##") or not (matches := self._SERVICE_MESSAGES_SCAN_PATTERN.findall(line)):
                 super().emit(memorized_prefix + line)
                 memorized_prefix = ""
-            # Do not forget to report system message prefix, if any
+                continue
+            for preceding_content, expression in matches:
+                memorized_prefix += preceding_content
+                self._process_service_message_expression(expression)
+        # Do not forget to report system message prefix, if any
         if memorized_prefix:
             super().emit(memorized_prefix)
```

### Comparing `cjunct-2.1.2/src/cjunct/actions/bundled/docker_shell.py` & `cjunct-2.1.3/src/cjunct/actions/bundled/docker_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             tmp_dir_path: Path = Path(tmp_directory)
             script_container_directory: str = f"{self._CONTAINER_TMP_DIRECTORY}/{container_name}-exec-source"
             script_container_file: Path = tmp_dir_path / self._ENTRY_SCRIPT_FILE_NAME
             script_container_file_clauses: t.List[str] = [
                 self.args.command,
             ]
             if C.SHELL_INJECT_YIELD_FUNCTION:
-                script_container_file_clauses.insert(0, self._YIELD_SHELL_FUNCTION_DEFINITION)
+                script_container_file_clauses.insert(0, self._SHELL_SERVICE_FUNCTIONS_DEFINITIONS)
             script_container_file.write_text(
                 data="\n".join(script_container_file_clauses),
                 encoding="utf-8",
             )
             container_binds: t.List[str] = [f"{tmp_directory}:{script_container_directory}:ro"]
             for bind_config in self.args.bind or []:
                 if bind_config.src is not None:
@@ -163,14 +163,17 @@
                     auth=self._make_auth(),
                 )
             async with self._make_container(client) as container:
                 tasks: t.List[asyncio.Task] = [
                     asyncio.create_task(self._read_stdout(container)),
                     asyncio.create_task(self._read_stderr(container)),
                 ]
+                # Wait for all tasks to complete
+                await asyncio.wait(tasks)
+                # Check exceptions
                 await asyncio.gather(*tasks)
                 result: dict = await container.wait()
                 self.logger.debug(f"Docker container result: {result}")
                 if (code := result.get("StatusCode", -1)) != 0:
                     self.fail(f"Exit code: {code}")
 
     async def _read_stdout(self, container: DockerContainer) -> None:
```

### Comparing `cjunct-2.1.2/src/cjunct/actions/bundled/shell.py` & `cjunct-2.1.3/src/cjunct/actions/bundled/shell.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,24 +42,27 @@
     async def _read_stderr(self, shell_process: Shell) -> None:
         async for line in shell_process.read_stderr():
             self.emit(Stderr(line))
 
     async def _create_shell(self) -> Shell:
         command: str = self.args.command or f"source '{self.args.file}'"
         if C.SHELL_INJECT_YIELD_FUNCTION:
-            command = f"{self._YIELD_SHELL_FUNCTION_DEFINITION}\n{command}"
+            command = f"{self._SHELL_SERVICE_FUNCTIONS_DEFINITIONS}\n{command}"
         return Shell(
             command=command,
             environment=self.args.environment,  # type: ignore[arg-type]
             cwd=self.args.cwd,
         )
 
     async def run(self) -> None:
         async with await self._create_shell() as shell_process:
             tasks: t.List[asyncio.Task] = [
                 asyncio.create_task(self._read_stdout(shell_process)),
                 asyncio.create_task(self._read_stderr(shell_process)),
             ]
+            # Wait for all tasks to complete
+            await asyncio.wait(tasks)
+            # Check exceptions
             await asyncio.gather(*tasks)
             result: ShellResult = await shell_process
             if result.code:
                 self.fail(f"Exit code: {result.code}")
```

### Comparing `cjunct-2.1.2/src/cjunct/config/constants/__init__.py` & `cjunct-2.1.3/src/cjunct/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/config/constants/cli.py` & `cjunct-2.1.3/src/cjunct/config/constants/cli.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/config/constants/helpers.py` & `cjunct-2.1.3/src/cjunct/config/constants/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/config/environment.py` & `cjunct-2.1.3/src/cjunct/config/environment.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/console.py` & `cjunct-2.1.3/src/cjunct/console.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/display/base.py` & `cjunct-2.1.3/src/cjunct/display/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/display/color.py` & `cjunct-2.1.3/src/cjunct/display/color.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/display/default.py` & `cjunct-2.1.3/src/cjunct/display/default.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,11 +107,11 @@
                 )
             ]
         )
         selected_action_names: t.List[str] = answers["actions"]
         return selected_action_names
 
     def on_action_start(self, action: ActionBase) -> None:
-        print(f"Go, {action}")
+        self.display(f"Start: {action}")
 
     def on_action_finish(self, action: ActionBase) -> None:
-        print(f"Thanks, {action}")
+        self.display(f"Finish: {action}")
```

### Comparing `cjunct-2.1.2/src/cjunct/exceptions.py` & `cjunct-2.1.3/src/cjunct/exceptions.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/loader/base.py` & `cjunct-2.1.3/src/cjunct/loader/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/loader/default.py` & `cjunct-2.1.3/src/cjunct/loader/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/loader/helpers.py` & `cjunct-2.1.3/src/cjunct/loader/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/rendering/__init__.py` & `cjunct-2.1.3/src/cjunct/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/rendering/containers.py` & `cjunct-2.1.3/src/cjunct/rendering/containers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/rendering/tokenizing.py` & `cjunct-2.1.3/src/cjunct/rendering/tokenizing.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/runner.py` & `cjunct-2.1.3/src/cjunct/runner.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/strategy.py` & `cjunct-2.1.3/src/cjunct/strategy.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/tools/inspect.py` & `cjunct-2.1.3/src/cjunct/tools/inspect.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/tools/proxy.py` & `cjunct-2.1.3/src/cjunct/tools/proxy.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/src/cjunct/workflow.py` & `cjunct-2.1.3/src/cjunct/workflow.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.1.2/PKG-INFO` & `cjunct-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjunct
-Version: 2.1.2
+Version: 2.1.3
 Summary: Declarative task runner
 Home-page: https://github.com/reartnew/cjunct
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Typing :: Typed
 Provides-Extra: docker
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0) ; extra == "docker"
-Requires-Dist: async-shell (>=1.0.5,<2.0.0)
+Requires-Dist: async-shell (>=1.0.6,<2.0.0)
 Requires-Dist: classlogging (>=1.1.1,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: inquirer (>=3.2.3,<4.0.0)
 Requires-Dist: named-env (>=2.3.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
```

