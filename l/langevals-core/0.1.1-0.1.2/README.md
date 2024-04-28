# Comparing `tmp/langevals_core-0.1.1.tar.gz` & `tmp/langevals_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_core-0.1.1.tar", max compression
+gzip compressed data, was "langevals_core-0.1.2.tar", max compression
```

## Comparing `langevals_core-0.1.1.tar` & `langevals_core-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     5843 2024-03-08 20:30:22.093547 langevals_core-0.1.1/langevals_core/base_evaluator.py
--rw-r--r--   0        0        0      377 2024-03-08 20:30:22.093547 langevals_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 langevals_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6566 2024-04-28 13:24:54.120394 langevals_core-0.1.2/langevals_core/base_evaluator.py
+-rw-r--r--   0        0        0      455 2024-04-28 13:24:54.120394 langevals_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 langevals_core-0.1.2/PKG-INFO
```

### Comparing `langevals_core-0.1.1/langevals_core/base_evaluator.py` & `langevals_core-0.1.2/langevals_core/base_evaluator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 from dataclasses import dataclass
 import os
 from abc import ABC
 import traceback
-from typing import ClassVar, Generic, List, Literal, Optional, TypeVar, get_type_hints
+from typing import (
+    ClassVar,
+    Generic,
+    List,
+    Literal,
+    Optional,
+    Type,
+    TypeVar,
+    get_args,
+    get_type_hints,
+)
 
 from pydantic import BaseModel, ConfigDict, Field
+import pandas as pd
 
-EvalCategories = Literal["quality", "rag", "safety", "policy", "other"]
+EvalCategories = Literal[
+    "quality", "rag", "safety", "policy", "other", "custom", "similarity"
+]
 
 TSettings = TypeVar("TSettings", bound=BaseModel)
 
 
 class EvaluatorEntry(BaseModel):
     """
     Entry datapoint for an evaluator, it should contain all the necessary information for the evaluator to run.
@@ -19,24 +32,29 @@
 
     input: The user or LLM input given to the model
     output: The LLM generated output
     contexts: A list of strings of the contexts that were considered when generating the LLM response
     expected_output: The ground truth of what the LLM should have generated, for comparison with the actual generated output
     """
 
-    model_config = ConfigDict(extra="forbid")
+    model_config = ConfigDict(extra="ignore")
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)  # Always call super()!
 
         required_fields_types = {
             "input": [str, Optional[str]],
             "output": [str, Optional[str]],
-            "contexts": [List[str], list[str]],
-            "expected_output": [str],
+            "contexts": [
+                List[str],
+                list[str],
+                Optional[List[str]],
+                Optional[list[str]],
+            ],
+            "expected_output": [str, Optional[str]],
         }
 
         subclass_fields_types = get_type_hints(cls)
 
         extra_fields = subclass_fields_types.keys() - required_fields_types.keys()
         if extra_fields:
             raise TypeError(
@@ -45,15 +63,15 @@
 
         for field, expected_types in required_fields_types.items():
             if (
                 field in subclass_fields_types
                 and subclass_fields_types[field] not in expected_types
             ):
                 raise TypeError(
-                    f"Field '{field}' in {cls.__name__} must be of type {expected_type.__name__}, got {subclass_fields_types[field].__name__}"
+                    f"Field '{field}' in {cls.__name__} must be of type {expected_types}, got {subclass_fields_types[field].__name__}"
                 )
 
 
 TEntry = TypeVar("TEntry", bound=EvaluatorEntry)
 
 
 class Money(BaseModel):
@@ -109,26 +127,41 @@
 
 @dataclass
 class EnvMissingException(Exception):
     message: str
 
 
 class BaseEvaluator(BaseModel, Generic[TEntry, TSettings, TResult], ABC):
-    settings: TSettings
+    default_settings: ClassVar[TSettings]  # type: ignore
+    settings: TSettings = Field(default=None)
     env: Optional[dict[str, str]] = None
     entry: Optional[TEntry] = (
         None  # dummy field just to read the type later when creating the routes
     )
     result: Optional[TResult] = (
         None  # dummy field just to read the type later when creating the route
     )
 
+    name: ClassVar[str]
     category: ClassVar[EvalCategories]
     env_vars: ClassVar[list[str]] = []
     docs_url: ClassVar[str] = ""
+    is_guardrail: ClassVar[bool] = False
+    __preloaded: ClassVar[bool] = False
+
+    def __init__(self, **kwargs):
+        if "settings" not in kwargs:
+            kwargs["settings"] = self.default_settings
+        super().__init__(**kwargs)
+        if not self.__preloaded:
+            self.__class__.preload()
+
+    @classmethod
+    def preload(cls):
+        cls.__preloaded = True
 
     def get_env(self, var: str):
         if var not in self.env_vars and (self.env is None or var not in self.env):
             raise ValueError(
                 f"Variable {var} not defined in evaluator env_vars, cannot access it."
             )
```

