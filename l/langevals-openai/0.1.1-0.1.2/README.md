# Comparing `tmp/langevals_openai-0.1.1.tar.gz` & `tmp/langevals_openai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_openai-0.1.1.tar", max compression
+gzip compressed data, was "langevals_openai-0.1.2.tar", max compression
```

## Comparing `langevals_openai-0.1.1.tar` & `langevals_openai-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4201 2024-03-08 20:30:22.089547 langevals_openai-0.1.1/langevals_openai/moderation.py
--rw-r--r--   0        0        0      463 2024-03-08 20:30:59.281559 langevals_openai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 langevals_openai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4293 2024-04-28 19:56:44.504808 langevals_openai-0.1.2/langevals_openai/moderation.py
+-rw-r--r--   0        0        0      463 2024-04-28 19:57:28.260482 langevals_openai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 langevals_openai-0.1.2/PKG-INFO
```

### Comparing `langevals_openai-0.1.1/langevals_openai/moderation.py` & `langevals_openai-0.1.2/langevals_openai/moderation.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class OpenAIModerationSettings(BaseModel):
     model: Literal["text-moderation-stable", "text-moderation-latest"] = Field(
         default="text-moderation-stable",
         description="The model version to use, `text-moderation-latest` will be automatically upgraded over time, while `text-moderation-stable` will only be updated with advanced notice by OpenAI.",
     )
     categories: OpenAIModerationCategories = Field(
-        default_factory=OpenAIModerationCategories,
+        default=OpenAIModerationCategories(),
         description="The categories of content to check for moderation.",
     )
 
 
 class OpenAIModerationResult(EvaluationResult):
     score: float = Field(
         description="The model's confidence on primary category where the input violates the OpenAI's policy. The value is between 0 and 1, where higher values denote higher confidence."
@@ -50,33 +50,34 @@
 
 class OpenAIModerationEvaluator(
     BaseEvaluator[
         OpenAIModerationEntry, OpenAIModerationSettings, OpenAIModerationResult
     ]
 ):
     """
-    OpenAI Moderation
-
     This evaluator uses OpenAI's moderation API to detect potentially harmful content in text,
     including harassment, hate speech, self-harm, sexual content, and violence.
     """
 
-    category = "policy"
+    name = "OpenAI Moderation"
+    category = "safety"
     env_vars = ["OPENAI_API_KEY"]
+    default_settings = OpenAIModerationSettings()
     docs_url = "https://platform.openai.com/docs/guides/moderation/overview"
+    is_guardrail = True
 
     def evaluate_batch(
         self, data: list[OpenAIModerationEntry]
     ) -> BatchEvaluationResult:
         client = OpenAI(api_key=self.get_env("OPENAI_API_KEY"))
 
         results: list[SingleEvaluationResult] = []
 
         contents = [
-            "\n\n".join([entry.input or "", entry.output or ""]).strip()
+            "\n\n".join([entry.input or "", entry.output or ""]).strip()[0:10_000]
             for entry in data
         ]
         response = client.moderations.create(input=contents)
         for index, moderation_result in enumerate(response.results):
             if not contents[index]:
                 results.append(
                     EvaluationResultSkipped(details="Input and output are both empty")
@@ -117,11 +118,11 @@
                     )
                 )
                 if not passed
                 else None
             )
 
             results.append(
-                EvaluationResult(score=score, passed=passed, details=details)
+                OpenAIModerationResult(score=score, passed=passed, details=details)
             )
 
         return results
```

