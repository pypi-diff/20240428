# Comparing `tmp/langevals-0.1.2.tar.gz` & `tmp/langevals-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals-0.1.2.tar", max compression
+gzip compressed data, was "langevals-0.1.3.tar", max compression
```

## Comparing `langevals-0.1.2.tar` & `langevals-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0        6 2024-03-08 20:30:22.093547 langevals-0.1.2/langevals/__init__.py
--rw-r--r--   0        0        0     4274 2024-03-08 20:30:22.093547 langevals-0.1.2/langevals/server.py
--rw-r--r--   0        0        0      941 2024-03-08 20:31:06.537559 langevals-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 langevals-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/__init__.py
+-rw-r--r--   0        0        0     3447 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/evaluation.py
+-rw-r--r--   0        0        0     4358 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/expect.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/pytest_plugins/__init__.py
+-rw-r--r--   0        0        0     4074 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/pytest_plugins/pass_rate_plugin.py
+-rw-r--r--   0        0        0     3481 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/server.py
+-rw-r--r--   0        0        0     2955 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/utils.py
+-rw-r--r--   0        0        0     2114 2024-04-28 19:57:35.936431 langevals-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 langevals-0.1.3/PKG-INFO
```

### Comparing `langevals-0.1.2/langevals/server.py` & `langevals-0.1.3/langevals/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,108 @@
-import os
-import textwrap
-import warnings
+import sys
 import dotenv
 
+from langevals.utils import (
+    get_evaluator_classes,
+    get_evaluator_definitions,
+    load_evaluator_packages,
+)
+
 dotenv.load_dotenv()
 
 import asyncio
 from fastapi import FastAPI, HTTPException, Request
-from typing import List, Optional, get_args
-import importlib
-import importlib.metadata
-import pkgutil
+from typing import List, Optional
 from langevals_core.base_evaluator import (
-    BaseEvaluator,
-    EnvMissingException,
     EvaluationResultSkipped,
     EvaluationResultError,
 )
 from pydantic import BaseModel, ConfigDict, Field, ValidationError
+from mangum import Mangum
 
 app = FastAPI()
 
 
-def load_evaluator_modules():
-    evaluators = {}
-    for distribution in importlib.metadata.distributions():
-        normalized_name = distribution.metadata["Name"].replace("-", "_")
-        if normalized_name == "langevals_core":
-            continue
-        if normalized_name.startswith("langevals_"):
-            try:
-                evaluators[normalized_name] = importlib.import_module(normalized_name)
-            except ImportError:
-                pass
-    return evaluators
-
-
-def create_evaluator_routes(evaluator_package):
-    print(f"Loading {evaluator_package.__name__}")
-
-    evaluator_classes: list[BaseEvaluator] = []
-    package_path = evaluator_package.__path__
-    for _, module_name, _ in pkgutil.walk_packages(package_path):
-        module = importlib.import_module(f"{evaluator_package.__name__}.{module_name}")
-        for name, cls in module.__dict__.items():
-            if (
-                isinstance(cls, type)
-                and issubclass(cls, BaseEvaluator)
-                and cls is not BaseEvaluator
-            ):
-                evaluator_classes.append(cls)  # type: ignore
-
-    for evaluator_cls in evaluator_classes:
-        fields = evaluator_cls.model_fields
-
-        settings_type = fields["settings"].annotation
-        entry_type = get_args(fields["entry"].annotation)[0]
-        result_type = get_args(fields["result"].annotation)[0]
-
-        module_name, evaluator_name = evaluator_cls.__module__.split(".", 1)
-        module_name = module_name.split("langevals_")[1]
-
-        required_env_vars = (
-            "\n\n__Env vars:__ " + ", ".join(evaluator_cls.env_vars)
-            if len(evaluator_cls.env_vars) > 0
-            else ""
-        )
-        docs = (
-            "\n\n__Docs:__ " + evaluator_cls.docs_url if evaluator_cls.docs_url else ""
-        )
-        description = (
-            (textwrap.dedent(evaluator_cls.__doc__ or "")) + required_env_vars + docs
-        )
+def create_evaluator_routes(evaluator_cls):
+    definitions = get_evaluator_definitions(evaluator_cls)
+    module_name = definitions.module_name
+    evaluator_name = definitions.evaluator_name
+    entry_type = definitions.entry_type
+    settings_type = definitions.settings_type
+    result_type = definitions.result_type
+
+    required_env_vars = (
+        "\n\n__Env vars:__ " + ", ".join(definitions.env_vars)
+        if len(definitions.env_vars) > 0
+        else ""
+    )
+    docs_url = "\n\n__Docs:__ " + definitions.docs_url if definitions.docs_url else ""
+    description = definitions.description + required_env_vars + docs_url
 
-        class Request(BaseModel):
-            model_config = ConfigDict(extra="forbid")
+    class Request(BaseModel):
+        model_config = ConfigDict(extra="forbid")
 
-            data: List[entry_type] = Field(description="List of entries to be evaluated, check the field type for the necessary keys")  # type: ignore
-            settings: Optional[settings_type] = Field(None, description="Evaluator settings, check the field type for what settings this evaluator supports")  # type: ignore
-            env: Optional[dict[str, str]] = Field(
-                None,
-                description="Optional environment variables to override the server ones",
-                json_schema_extra={"example": {}},
-            )
-
-        @app.post(
-            f"/{module_name}/{evaluator_name}/evaluate",
-            name=f"{module_name}_{evaluator_name}_evaluate",
-            description=description,
+        data: List[entry_type] = Field(description="List of entries to be evaluated, check the field type for the necessary keys")  # type: ignore
+        settings: Optional[settings_type] = Field(None, description="Evaluator settings, check the field type for what settings this evaluator supports")  # type: ignore
+        env: Optional[dict[str, str]] = Field(
+            None,
+            description="Optional environment variables to override the server ones",
+            json_schema_extra={"example": {}},
         )
-        async def evaluate(
-            req: Request,
-        ) -> List[result_type | EvaluationResultSkipped | EvaluationResultError]:  # type: ignore
-            evaluator = evaluator_cls(settings=(req.settings or {}), env=req.env)  # type: ignore
-            return evaluator.evaluate_batch(req.data)
 
+    evaluator_cls.preload()
 
-evaluators = load_evaluator_modules()
-for evaluator_name, evaluator_module in evaluators.items():
-    create_evaluator_routes(evaluator_module)
+    @app.post(
+        f"/{module_name}/{evaluator_name}/evaluate",
+        name=f"{module_name}_{evaluator_name}_evaluate",
+        description=description,
+    )
+    async def evaluate(
+        req: Request,
+    ) -> List[result_type | EvaluationResultSkipped | EvaluationResultError]:  # type: ignore
+        evaluator = evaluator_cls(settings=(req.settings or {}), env=req.env)  # type: ignore
+        return evaluator.evaluate_batch(req.data)
+
+
+evaluators = load_evaluator_packages()
+for evaluator_name, evaluator_package in evaluators.items():
+    module_name = evaluator_package.__name__.split("langevals_")[1]
+    if (
+        len(sys.argv) > 2
+        and sys.argv[1] == "--only"
+        and module_name not in sys.argv[2].split(",")
+    ):
+        continue
+    print(f"Loading {evaluator_package.__name__}")
+    for evaluator_cls in get_evaluator_classes(evaluator_package):
+        create_evaluator_routes(evaluator_cls)
 
 
 @app.exception_handler(ValidationError)
 async def validation_exception_handler(request: Request, exc: ValidationError):
     raise HTTPException(
         status_code=400,
         detail=exc.errors(),
     )
 
 
-@app.exception_handler(EnvMissingException)
-async def missing_env_exception_handler(request: Request, exc: EnvMissingException):
-    raise HTTPException(status_code=400, detail=exc.message)
-
-
 def main():
+    if len(sys.argv) > 1 and sys.argv[1] == "--preload":
+        print("Preloading done")
+        return
+    if len(sys.argv) > 1 and sys.argv[1] == "--export-openapi-json":
+        import json
+
+        with open("openapi.json", "w") as f:
+            f.write(json.dumps(app.openapi(), indent=2))
+        print("openapi.json exported")
+        return
     from hypercorn.config import Config
     from hypercorn.asyncio import serve
 
     asyncio.run(serve(app, Config()))  # type: ignore
 
 
 if __name__ == "__main__":
     main()
+else:
+    handler = Mangum(app, lifespan="off")
```

