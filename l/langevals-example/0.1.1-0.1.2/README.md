# Comparing `tmp/langevals_example-0.1.1.tar.gz` & `tmp/langevals_example-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_example-0.1.1.tar", max compression
+gzip compressed data, was "langevals_example-0.1.2.tar", max compression
```

## Comparing `langevals_example-0.1.1.tar` & `langevals_example-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     1623 2024-03-08 20:30:22.089547 langevals_example-0.1.1/langevals_example/word_count.py
--rw-r--r--   0        0        0      438 2024-03-08 20:30:51.645557 langevals_example-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 langevals_example-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2204 2024-04-28 13:24:54.116394 langevals_example-0.1.2/langevals_example/word_count.py
+-rw-r--r--   0        0        0      438 2024-04-28 13:25:31.828509 langevals_example-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 langevals_example-0.1.2/PKG-INFO
```

### Comparing `langevals_example-0.1.1/langevals_example/word_count.py` & `langevals_example-0.1.2/langevals_example/word_count.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,30 +18,35 @@
     pass
 
 
 # The structure that holds the result of the evaluation, if a score is used, it's a good idea to overwrite the
 # EvaluationResult class to add a pydantic description to the field explaning what the score means for this evaluator,
 # as shown here
 class ExampleWordCountResult(EvaluationResult):
-    score: float = Field(description="How nice the output is, from 0 to 100")
+    score: float = Field(
+        description="How many words are there in the output, split by space"
+    )
 
 
 class ExampleWordCountEvaluator(
     BaseEvaluator[
         ExampleWordCountEntry, ExampleWordCountSettings, ExampleWordCountResult
     ]
 ):
     """
-    Example Evaluator
-
     This evaluator serves as a boilerplate for creating new evaluators.
     """
 
-    category = "other"
-    env_vars = ["NECESSARY_ENV_VAR"]
-    docs_url = "https://path/to/official/docs"
+    name = "Example Evaluator"
+    category = "other"  # The category of the evaluator, can be "safety", "quality", "other", etc, check BaseEvaluator for all options
+    env_vars = [
+        "NECESSARY_ENV_VAR"
+    ]  # The environment variables that are necessary for the evaluator to run
+    default_settings = ExampleWordCountSettings()  # The default settings for the evaluator in case no settings are provided
+    docs_url = "https://path/to/official/docs"  # The URL to the official documentation of the evaluator
+    is_guardrail = False  # If the evaluator is a guardrail or not, a guardrail evaluator must return a boolean result on the `passed` result field in addition to the score
 
     def evaluate(self, entry: ExampleWordCountEntry) -> SingleEvaluationResult:
         words = entry.output.split(" ")
         return ExampleWordCountResult(
-            score=len(words), passed=True, details=f"Words found: {', '.join(words)}"
+            score=len(words), details=f"Words found: {', '.join(words)}"
         )
```

