# Comparing `tmp/langevals_custom-0.1.0.tar.gz` & `tmp/langevals_custom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_custom-0.1.0.tar", max compression
+gzip compressed data, was "langevals_custom-0.1.1.tar", max compression
```

## Comparing `langevals_custom-0.1.0.tar` & `langevals_custom-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,6 @@
--rw-r--r--   0        0        0     2366 2024-03-09 20:09:37.344198 langevals_custom-0.1.0/langevals_custom/basic.py
--rw-r--r--   0        0        0      511 2024-03-09 20:09:58.716130 langevals_custom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 langevals_custom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2638 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/basic.py
+-rw-r--r--   0        0        0     5602 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/llm_boolean.py
+-rw-r--r--   0        0        0     5445 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/llm_score.py
+-rw-r--r--   0        0        0     4320 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/similarity.py
+-rw-r--r--   0        0        0      549 2024-04-28 13:25:28.768500 langevals_custom-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 langevals_custom-0.1.1/PKG-INFO
```

### Comparing `langevals_custom-0.1.0/langevals_custom/basic.py` & `langevals_custom-0.1.1/langevals_custom/basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,32 +22,34 @@
         "matches_regex",
         "not_matches_regex",
     ]
     value: str
 
 
 class CustomBasicSettings(BaseModel):
-    rules: list[CustomBasicRule] = []
+    rules: list[CustomBasicRule] = Field(default=[
+        CustomBasicRule(field="output", rule="not_contains", value="artificial intelligence"),
+    ], description="List of rules to check, the message must pass all of them")
 
 
 class CustomBasicResult(EvaluationResult):
     score: float = Field(description="Returns 1 if all rules pass, 0 if any rule fails")
     passed: Optional[bool]
 
 
 class CustomBasicEvaluator(
     BaseEvaluator[CustomBasicEntry, CustomBasicSettings, CustomBasicResult]
 ):
     """
-    Basic Custom Evaluator
-
-    Allows you to check for simple text matches or regex evaluation
+    Allows you to check for simple text matches or regex evaluation.
     """
 
+    name = "Custom Basic Evaluator"
     category = "custom"
+    default_settings = CustomBasicSettings()
     is_guardrail = True
 
     def evaluate(self, entry: CustomBasicEntry) -> SingleEvaluationResult:
         passed = True
         score = 1
         details = None
 
@@ -72,12 +74,12 @@
             field = entry.output or ""
 
         if rule.rule == "contains":
             return rule.value in field
         elif rule.rule == "not_contains":
             return rule.value not in field
         elif rule.rule == "matches_regex":
-            return bool(re.match(rule.value, field))
+            return bool(re.search(rule.value, field, re.MULTILINE))
         elif rule.rule == "not_matches_regex":
-            return not bool(re.match(rule.value, field))
+            return not bool(re.search(rule.value, field, re.MULTILINE))
         else:
             return False
```

### Comparing `langevals_custom-0.1.0/PKG-INFO` & `langevals_custom-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-custom
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom evaluators you can build using other LLMs to do the eval, semantic matching or simple regexes or string matching.
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langevals-core (>=0.1.1,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: litellm (>=1.31.3,<2.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

