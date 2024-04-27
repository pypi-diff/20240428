# Comparing `tmp/openinference_instrumentation_dspy-0.1.6.tar.gz` & `tmp/openinference_instrumentation_dspy-0.1.7.tar.gz`

## Comparing `openinference_instrumentation_dspy-0.1.6.tar` & `openinference_instrumentation_dspy-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    23629 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/version.py
--rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/tests/openinference/instrumentation/dspy/test_instrumentor.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/.gitignore
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/LICENSE
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    24031 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/version.py
+-rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/tests/openinference/instrumentation/dspy/test_instrumentor.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/.gitignore
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/README.md
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/PKG-INFO
```

### Comparing `openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/__init__.py` & `openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,14 +521,28 @@
                 return {
                     "fields": [self.default(field) for field in o.fields],
                     "instructions": o.instructions,
                 }
             return repr(o)
 
 
+class SafeJSONEncoder(json.JSONEncoder):
+    """
+    Safely encodes non-JSON-serializable objects.
+    """
+
+    def default(self, o: Any) -> Any:
+        try:
+            return super().default(o)
+        except TypeError:
+            if hasattr(o, "dict") and callable(o.dict):  # pydantic v1 models, e.g., from Cohere
+                return o.dict()
+            return repr(o)
+
+
 def _get_input_value(method: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
     """
     Parses a method call's inputs into a JSON string. Ensures a consistent
     output regardless of whether the those inputs are passed as positional or
     keyword arguments.
     """
 
@@ -606,15 +620,15 @@
 
 def _jsonify_output(response: Any) -> str:
     """
     Converts output to JSON string.
     """
     if _is_google_response(response):
         return json.dumps(_parse_google_response(response))
-    return json.dumps(response)
+    return json.dumps(response, cls=SafeJSONEncoder)
 
 
 def _is_google_response(response: Any) -> TypeGuard["GenerateContentResponseType"]:
     """
     Checks whether a candidate response is an instance of
     GenerateContentResponse returned by the Google generative AI SDK.
     """
```

### Comparing `openinference_instrumentation_dspy-0.1.6/tests/openinference/instrumentation/dspy/test_instrumentor.py` & `openinference_instrumentation_dspy-0.1.7/tests/openinference/instrumentation/dspy/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.6/LICENSE` & `openinference_instrumentation_dspy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.6/pyproject.toml` & `openinference_instrumentation_dspy-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -56,22 +56,36 @@
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openinference"]
 
 [tool.mypy]
-plugins = []
-disallow_untyped_calls = true
-disallow_untyped_defs = true
-disallow_incomplete_defs  = true
 strict = true
+explicit_package_bases = true
 exclude = [
-  "dist/",
+  "examples",
+  "dist",
+  "sdist",
+]
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "wrapt",
+  "dspy.*",
+  "dsp.*",
 ]
 
 [tool.ruff]
-exclude = [".git", "__pycache__", "*_pb2.py*", "*.pyi"]
-ignore-init-module-imports = true
 line-length = 100
-select = ["E", "F", "W", "I"]
 target-version = "py38"
+
+[tool.ruff.lint.per-file-ignores]
+"*.ipynb" = ["E402", "E501"]
+
+[tool.ruff.lint]
+ignore-init-module-imports = true
+select = ["E", "F", "W", "I"]
+
+[tool.ruff.lint.isort]
+force-single-line = false
```

