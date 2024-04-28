# Comparing `tmp/langevals_azure-0.1.1.tar.gz` & `tmp/langevals_azure-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_azure-0.1.1.tar", max compression
+gzip compressed data, was "langevals_azure-0.1.2.tar", max compression
```

## Comparing `langevals_azure-0.1.1.tar` & `langevals_azure-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3437 2024-03-08 20:30:22.089547 langevals_azure-0.1.1/langevals_azure/content_safety.py
--rw-r--r--   0        0        0     1800 2024-03-08 20:30:22.089547 langevals_azure-0.1.1/langevals_azure/jailbreak.py
--rw-r--r--   0        0        0      499 2024-03-08 20:30:47.233555 langevals_azure-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 langevals_azure-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3847 2024-04-28 13:24:54.112394 langevals_azure-0.1.2/langevals_azure/content_safety.py
+-rw-r--r--   0        0        0     2275 2024-04-28 13:24:54.112394 langevals_azure-0.1.2/langevals_azure/jailbreak.py
+-rw-r--r--   0        0        0      499 2024-04-28 13:25:25.604491 langevals_azure-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 langevals_azure-0.1.2/PKG-INFO
```

### Comparing `langevals_azure-0.1.1/langevals_azure/content_safety.py` & `langevals_azure-0.1.2/langevals_azure/content_safety.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,23 +14,28 @@
 
 
 class AzureContentSafetyEntry(EvaluatorEntry):
     input: Optional[str] = None
     output: Optional[str] = None
 
 
+class AzureContentSafetyCategories(BaseModel):
+    Hate: bool = True
+    SelfHarm: bool = True
+    Sexual: bool = True
+    Violence: bool = True
+
+
 class AzureContentSafetySettings(BaseModel):
-    severity_threshold: int = Field(
-        ge=1,
-        le=8,
+    severity_threshold: Literal[1, 2, 3, 4, 5, 6, 7] = Field(
         default=1,
-        description="The minimum severity level to consider content as unsafe.",
+        description="The minimum severity level to consider content as unsafe, from 1 to 7.",
     )
-    categories: list[str] = Field(
-        default=["Hate", "SelfHarm", "Sexual", "Violence"],
+    categories: AzureContentSafetyCategories = Field(
+        default=AzureContentSafetyCategories(),
         description="The categories of moderation to check for.",
     )
     output_type: Literal["FourSeverityLevels", "EightSeverityLevels"] = Field(
         default="FourSeverityLevels",
         description="The type of severity levels to return on the full 0-7 severity scale, it can be either the trimmed version with four values (0, 2, 4, 6 scores) or the whole range.",
     )
 
@@ -45,37 +50,42 @@
     BaseEvaluator[
         AzureContentSafetyEntry,
         AzureContentSafetySettings,
         AzureContentSafetyResult,
     ]
 ):
     """
-    Azure Content Safety Moderation
-
     This evaluator detects potentially unsafe content in text, including hate speech,
     self-harm, sexual content, and violence. It allows customization of the severity
     threshold and the specific categories to check.
     """
 
+    name = "Azure Content Safety"
     category = "safety"
     env_vars = ["AZURE_CONTENT_SAFETY_ENDPOINT", "AZURE_CONTENT_SAFETY_KEY"]
+    default_settings = AzureContentSafetySettings()
     docs_url = "https://learn.microsoft.com/en-us/azure/ai-services/content-safety/quickstart-text"
+    is_guardrail = True
 
     def evaluate(self, entry: AzureContentSafetyEntry) -> SingleEvaluationResult:
         endpoint = self.get_env("AZURE_CONTENT_SAFETY_ENDPOINT")
         key = self.get_env("AZURE_CONTENT_SAFETY_KEY")
 
         client = ContentSafetyClient(endpoint, AzureKeyCredential(key))
 
         content = "\n\n".join([entry.input or "", entry.output or ""]).strip()
         if not content:
             return EvaluationResultSkipped(details="Input and output are both empty")
         request = AnalyzeTextOptions(
-            text=content,
-            categories=self.settings.categories,
+            text=content[0:10000],
+            categories=[
+                key
+                for key in self.settings.categories.model_dump().keys()
+                if self.settings.categories.model_dump().get(key, False)
+            ],
             output_type=self.settings.output_type,
         )
         response = client.analyze_text(request)
 
         categories_analysis = {
             item.category: item.severity for item in response.categories_analysis
         }
@@ -88,8 +98,8 @@
                 for category, severity in categories_analysis.items()
                 if (severity or 0) >= self.settings.severity_threshold
             )
             or None
         )
         details = "Detected " + details if details else None
 
-        return EvaluationResult(score=score, passed=passed, details=details)
+        return AzureContentSafetyResult(score=score, passed=passed, details=details)
```

### Comparing `langevals_azure-0.1.1/langevals_azure/jailbreak.py` & `langevals_azure-0.1.2/langevals_azure/jailbreak.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,72 @@
+from typing import Optional
 from httpx import Client, Response
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluationResult,
     SingleEvaluationResult,
     EvaluatorEntry,
     EvaluationResultSkipped,
 )
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class AzureJailbreakEntry(EvaluatorEntry):
     input: str
 
 
 class AzureJailbreakSettings(BaseModel):
     pass
 
 
+class AzureJailbreakResult(EvaluationResult):
+    passed: Optional[bool] = Field(
+        description="If true then no jailbreak was detected, if false then a jailbreak was detected"
+    )
+
+
 class AzureJailbreakEvaluator(
-    BaseEvaluator[AzureJailbreakEntry, AzureJailbreakSettings, EvaluationResult]
+    BaseEvaluator[AzureJailbreakEntry, AzureJailbreakSettings, AzureJailbreakResult]
 ):
     """
-    Azure Jailbreak Detection
-
     This evaluator checks for jailbreak-attempt in the input using Azure's Content Safety API.
     """
 
+    name = "Azure Jailbreak Detection"
     category = "safety"
     env_vars = ["AZURE_CONTENT_SAFETY_ENDPOINT", "AZURE_CONTENT_SAFETY_KEY"]
+    default_settings = AzureJailbreakSettings()
+    is_guardrail = True
 
     def evaluate(self, entry: AzureJailbreakEntry) -> SingleEvaluationResult:
         endpoint = self.get_env("AZURE_CONTENT_SAFETY_ENDPOINT")
         key = self.get_env("AZURE_CONTENT_SAFETY_KEY")
         url = f"{endpoint}/contentsafety/text:detectJailbreak?api-version=2023-10-15-preview"
 
         content = entry.input or ""
         if not content:
             return EvaluationResultSkipped(details="Input is empty")
 
         headers = {
             "Content-Type": "application/json",
             "Ocp-Apim-Subscription-Key": key,
         }
-        body = {"text": content}
-
-        with Client() as client:
-            response: Response = client.post(url, headers=headers, json=body)
-
-        if response.is_error:
-            raise ValueError(f"Error in API response: {response.text}")
 
-        result = response.json()
-        detected = result.get("jailbreakAnalysis", {}).get("detected", False)
+        detected = False
+        for i in range(0, len(content), 1000):
+            body = {"text": content[i : i + 1000]}
+            with Client() as client:
+                response: Response = client.post(url, headers=headers, json=body)
+
+            if response.is_error:
+                raise ValueError(f"Error in API response: {response.text}")
+
+            result = response.json()
+            detected = result.get("jailbreakAnalysis", {}).get("detected", False)
+            if detected:
+                break
 
-        return EvaluationResult(
+        return AzureJailbreakResult(
             score=1 if detected else 0,
             passed=not detected,
             details="Jailbreak attempt detected" if detected else None,
         )
```

### Comparing `langevals_azure-0.1.1/PKG-INFO` & `langevals_azure-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-azure
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangEvals Azure Content Safety evaluator for LLM outputs.
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: azure-ai-contentsafety (>=1.0.0,<2.0.0)
-Requires-Dist: langevals-core (>=0.1.1,<0.2.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
```

