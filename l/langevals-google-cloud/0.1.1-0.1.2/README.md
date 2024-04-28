# Comparing `tmp/langevals_google_cloud-0.1.1.tar.gz` & `tmp/langevals_google_cloud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_google_cloud-0.1.1.tar", max compression
+gzip compressed data, was "langevals_google_cloud-0.1.2.tar", max compression
```

## Comparing `langevals_google_cloud-0.1.1.tar` & `langevals_google_cloud-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4036 2024-03-08 20:30:22.089547 langevals_google_cloud-0.1.1/langevals_google_cloud/dlp_pii_detection.py
--rw-r--r--   0        0        0      480 2024-03-08 20:30:55.089559 langevals_google_cloud-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 langevals_google_cloud-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4443 2024-04-28 13:24:54.116394 langevals_google_cloud-0.1.2/langevals_google_cloud/dlp_pii_detection.py
+-rw-r--r--   0        0        0      540 2024-04-28 13:25:35.780510 langevals_google_cloud-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 langevals_google_cloud-0.1.2/PKG-INFO
```

### Comparing `langevals_google_cloud-0.1.1/langevals_google_cloud/dlp_pii_detection.py` & `langevals_google_cloud-0.1.2/langevals_google_cloud/dlp_pii_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,36 +41,37 @@
         description="The minimum confidence required for failing the evaluation on a PII match.",
     )
 
 
 class GoogleCloudDLPPIIDetectionResult(EvaluationResult):
     score: float = Field(description="Amount of PII detected, 0 means no PII detected")
     passed: Optional[bool] = Field(
-        description="If true then no PII was detected, if false then at lease one PII was detected"
+        description="If true then no PII was detected, if false then at least one PII was detected"
     )
     raw_response: dict[str, Any]
 
 
 class GoogleCloudDLPPIIDetectionEvaluator(
     BaseEvaluator[
         GoogleCloudDLPPIIDetectionEntry,
         GoogleCloudDLPPIIDetectionSettings,
         GoogleCloudDLPPIIDetectionResult,
     ]
 ):
     """
-    Google Cloud DLP PII Detector
-
     Google DLP PII detects personally identifiable information in text, including phone numbers, email addresses, and
     social security numbers. It allows customization of the detection threshold and the specific types of PII to check.
     """
 
+    name = "Google Cloud DLP PII Detection"
     category = "safety"
     env_vars = ["GOOGLE_CREDENTIALS_JSON"]
+    default_settings = GoogleCloudDLPPIIDetectionSettings()
     docs_url = "https://cloud.google.com/sensitive-data-protection/docs/apis"
+    is_guardrail = True
 
     def evaluate(
         self, entry: GoogleCloudDLPPIIDetectionEntry
     ) -> SingleEvaluationResult:
         credentials_json = json.loads(self.get_env("GOOGLE_CREDENTIALS_JSON"))
         credentials = service_account.Credentials.from_service_account_info(
             credentials_json
@@ -83,21 +84,29 @@
         settings_info_types = self.settings.info_types.model_dump()
         info_types = [
             {"name": info_type.upper()}
             for info_type in settings_info_types.keys()
             if settings_info_types[info_type]
         ]
 
+        if len(content) > 524288:
+            raise ValueError(
+                "Content exceeds the maximum length of 524288 bytes allowed by Google PII Detection"
+            )
+
         response = dlp_client.inspect_content(
             request={
                 "parent": f"projects/{credentials.project_id}/locations/global",
                 "inspect_config": {
                     "info_types": info_types,
                     "min_likelihood": self.settings.min_likelihood,
                     "include_quote": True,
+                    "limits": {
+                        "max_findings_per_request": 0,  # (0 = server maximum)
+                    },
                 },
                 "item": {"value": content},
             }
         )
 
         findings = [
             f"{finding.info_type.name} ({finding.info_type.sensitivity_score.score.name}, {finding.likelihood.name})"
```

### Comparing `langevals_google_cloud-0.1.1/PKG-INFO` & `langevals_google_cloud-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langevals-google-cloud
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangEvals integration for Google Cloud APIs evaluators
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-cloud-dlp (>=3.16.0,<4.0.0)
-Requires-Dist: langevals-core (>=0.1.1,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
```

