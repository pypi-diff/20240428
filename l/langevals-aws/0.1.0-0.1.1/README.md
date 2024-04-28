# Comparing `tmp/langevals_aws-0.1.0.tar.gz` & `tmp/langevals_aws-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_aws-0.1.0.tar", max compression
+gzip compressed data, was "langevals_aws-0.1.1.tar", max compression
```

## Comparing `langevals_aws-0.1.0.tar` & `langevals_aws-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     6609 2024-03-21 12:46:18.613970 langevals_aws-0.1.0/langevals_aws/comprehend_pii_detection.py
--rw-r--r--   0        0        0      452 2024-03-21 12:46:37.698214 langevals_aws-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 langevals_aws-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6660 2024-04-28 13:24:54.112394 langevals_aws-0.1.1/langevals_aws/comprehend_pii_detection.py
+-rw-r--r--   0        0        0      452 2024-04-28 13:25:21.412479 langevals_aws-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 langevals_aws-0.1.1/PKG-INFO
```

### Comparing `langevals_aws-0.1.0/langevals_aws/comprehend_pii_detection.py` & `langevals_aws-0.1.1/langevals_aws/comprehend_pii_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     ] = Field(
         default="eu-central-1",
         description="The AWS region to use for running the PII detection, defaults to eu-central-1 for GDPR compliance.",
     )
 
 
 class AWSPIIEntityResult(TypedDict):
-    Type: Literal[
+    Name: Literal[
         "BANK_ACCOUNT_NUMBER",
         "BANK_ROUTING",
         "CREDIT_DEBIT_NUMBER",
         "CREDIT_DEBIT_CVV",
         "CREDIT_DEBIT_EXPIRY",
         "PIN",
         "EMAIL",
@@ -135,20 +135,18 @@
         "SWIFT_CODE",
         "UK_NATIONAL_HEALTH_SERVICE_NUMBER",
         "CA_HEALTH_NUMBER",
         "IN_AADHAAR",
         "IN_VOTER_NUMBER",
     ]
     Score: float
-    BeginOffset: int
-    EndOffset: int
 
 
 class AWSPIIEntityResults(TypedDict):
-    Entities: list[AWSPIIEntityResult]
+    Labels: list[AWSPIIEntityResult]
 
 
 class AWSComprehendPIIDetectionResult(EvaluationResult):
     score: float = Field(description="Amount of PII detected, 0 means no PII detected")
     passed: Optional[bool] = Field(
         description="If true then no PII was detected, if false then at least one PII was detected"
     )
@@ -165,50 +163,51 @@
     """
     Amazon Comprehend PII detects personally identifiable information in text, including phone numbers, email addresses, and
     social security numbers. It allows customization of the detection threshold and the specific types of PII to check.
     """
 
     name = "Amazon Comprehend PII Detection"
     category = "safety"
-    env_vars = ["AWS_ACCESS_KEY_ID", "AWS_SECRET_ACCESS_KEY"]
+    env_vars = ["AWS_COMPREHEND_ACCESS_KEY_ID", "AWS_COMPREHEND_SECRET_ACCESS_KEY"]
+    default_settings = AWSComprehendPIIDetectionSettings()
     docs_url = "https://docs.aws.amazon.com/comprehend/latest/dg/how-pii.html"
     is_guardrail = True
 
     def evaluate(self, entry: AWSComprehendPIIDetectionEntry) -> SingleEvaluationResult:
         content = "\n\n".join([entry.input or "", entry.output or ""]).strip()
         if not content:
             return EvaluationResultSkipped(details="Input and output are both empty")
 
         client = boto3.client(
             "comprehend",
-            aws_access_key_id=self.get_env("AWS_ACCESS_KEY_ID"),
-            aws_secret_access_key=self.get_env("AWS_SECRET_ACCESS_KEY"),
+            aws_access_key_id=self.get_env("AWS_COMPREHEND_ACCESS_KEY_ID"),
+            aws_secret_access_key=self.get_env("AWS_COMPREHEND_SECRET_ACCESS_KEY"),
             region_name=self.settings.aws_region,
         )
 
-        response: AWSPIIEntityResults = client.detect_pii_entities(
+        response: AWSPIIEntityResults = client.contains_pii_entities(
             Text=content,
             LanguageCode=self.settings.language_code,
         )
 
-        response["Entities"] = [
+        response["Labels"] = [
             entity
-            for entity in response["Entities"]
-            if getattr(self.settings.entity_types, entity["Type"], False)
+            for entity in response["Labels"]
+            if getattr(self.settings.entity_types, entity["Name"], False)
             and entity["Score"] >= self.settings.min_confidence
         ]
 
         findings = [
-            f"{entity['Type']} (confidence: {entity['Score']:.2f})"
-            for entity in response["Entities"]
+            f"{entity['Name']} (confidence: {entity['Score']:.2f})"
+            for entity in response["Labels"]
         ]
 
         return AWSComprehendPIIDetectionResult(
-            score=len(response["Entities"]),
-            passed=len(response["Entities"]) == 0,
+            score=len(response["Labels"]),
+            passed=len(response["Labels"]) == 0,
             details=(
                 None
-                if len(response["Entities"]) == 0
+                if len(response["Labels"]) == 0
                 else f"PII detected: {', '.join(findings)}"
             ),
             raw_response=response,
         )
```

