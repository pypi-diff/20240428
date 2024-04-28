# Comparing `tmp/langevals_ragas-0.1.1.tar.gz` & `tmp/langevals_ragas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_ragas-0.1.1.tar", max compression
+gzip compressed data, was "langevals_ragas-0.1.2.tar", max compression
```

## Comparing `langevals_ragas-0.1.1.tar` & `langevals_ragas-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1093 2024-03-08 20:30:22.089547 langevals_ragas-0.1.1/langevals_ragas/answer_relevancy.py
--rw-r--r--   0        0        0     1209 2024-03-08 20:30:22.089547 langevals_ragas-0.1.1/langevals_ragas/context_precision.py
--rw-r--r--   0        0        0     1151 2024-03-08 20:30:22.089547 langevals_ragas-0.1.1/langevals_ragas/context_recall.py
--rw-r--r--   0        0        0     1179 2024-03-08 20:30:22.089547 langevals_ragas-0.1.1/langevals_ragas/context_relevancy.py
--rw-r--r--   0        0        0     1110 2024-03-08 20:30:22.089547 langevals_ragas-0.1.1/langevals_ragas/faithfulness.py
--rw-r--r--   0        0        0     4054 2024-03-08 20:30:22.089547 langevals_ragas-0.1.1/langevals_ragas/lib/common.py
--rw-r--r--   0        0        0      509 2024-03-08 20:31:02.705560 langevals_ragas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 langevals_ragas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/answer_relevancy.py
+-rw-r--r--   0        0        0     1189 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_precision.py
+-rw-r--r--   0        0        0     1131 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_recall.py
+-rw-r--r--   0        0        0     1159 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_relevancy.py
+-rw-r--r--   0        0        0     1173 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_utilization.py
+-rw-r--r--   0        0        0     1090 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/faithfulness.py
+-rw-r--r--   0        0        0     5441 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/lib/common.py
+-rw-r--r--   0        0        0      589 2024-04-28 19:57:32.208456 langevals_ragas-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 langevals_ragas-0.1.2/PKG-INFO
```

### Comparing `langevals_ragas-0.1.1/langevals_ragas/answer_relevancy.py` & `langevals_ragas-0.1.2/langevals_ragas/faithfulness.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluatorEntry,
     SingleEvaluationResult,
 )
-from .lib.common import evaluate_ragas, RagasSettings, RagasResult
+from .lib.common import env_vars, evaluate_ragas, RagasSettings, RagasResult
 
 
-class RagasAnswerRelevancyEntry(EvaluatorEntry):
-    input: str
+class RagasFaithfulnessEntry(EvaluatorEntry):
     output: str
+    contexts: list[str]
 
 
-class RagasAnswerRelevancyEvaluator(
-    BaseEvaluator[RagasAnswerRelevancyEntry, RagasSettings, RagasResult]
+class RagasFaithfulnessEvaluator(
+    BaseEvaluator[RagasFaithfulnessEntry, RagasSettings, RagasResult]
 ):
     """
-    Ragas Answer Relevancy
-
-    This evaluator focuses on assessing how pertinent the generated answer is to the given prompt. Higher scores indicate better relevancy.
+    This evaluator assesses the extent to which the generated answer is consistent with the provided context. Higher scores indicate better faithfulness to the context.
     """
 
+    name = "Ragas Faithfulness"
     category = "rag"
-    env_vars = [
-        "OPENAI_API_KEY",
-        "AZURE_CONTENT_SAFETY_ENDPOINT",
-        "AZURE_CONTENT_SAFETY_KEY",
-    ]
-    docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/answer_relevance.html"
+    env_vars = env_vars
+    default_settings = RagasSettings()
+    docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/faithfulness.html"
+    is_guardrail = False
 
-    def evaluate(self, entry: RagasAnswerRelevancyEntry) -> SingleEvaluationResult:
+    def evaluate(self, entry: RagasFaithfulnessEntry) -> SingleEvaluationResult:
         return evaluate_ragas(
             evaluator=self,
-            metric="answer_relevancy",
-            question=entry.input,
+            metric="faithfulness",
             answer=entry.output,
+            contexts=entry.contexts,
             settings=self.settings,
         )
```

### Comparing `langevals_ragas-0.1.1/langevals_ragas/context_precision.py` & `langevals_ragas-0.1.2/langevals_ragas/context_precision.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluatorEntry,
     SingleEvaluationResult,
 )
-from .lib.common import evaluate_ragas, RagasSettings, RagasResult
+from .lib.common import env_vars, evaluate_ragas, RagasSettings, RagasResult
 
 
 class RagasContextPrecisionEntry(EvaluatorEntry):
     input: str
     contexts: list[str]
     expected_output: str
 
 
 class RagasContextPrecisionEvaluator(
     BaseEvaluator[RagasContextPrecisionEntry, RagasSettings, RagasResult]
 ):
     """
-    Ragas Context Precision
-
     This metric evaluates whether all of the ground-truth relevant items present in the contexts are ranked higher or not. Higher scores indicate better precision.
     """
 
+    name = "Ragas Context Precision"
     category = "rag"
-    env_vars = [
-        "OPENAI_API_KEY",
-        "AZURE_CONTENT_SAFETY_ENDPOINT",
-        "AZURE_CONTENT_SAFETY_KEY",
-    ]
+    env_vars = env_vars
+    default_settings = RagasSettings()
     docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/context_precision.html"
+    is_guardrail = False
 
     def evaluate(self, entry: RagasContextPrecisionEntry) -> SingleEvaluationResult:
         return evaluate_ragas(
             evaluator=self,
             metric="context_precision",
             question=entry.input,
             contexts=entry.contexts,
```

### Comparing `langevals_ragas-0.1.1/langevals_ragas/context_recall.py` & `langevals_ragas-0.1.2/langevals_ragas/context_recall.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluatorEntry,
     SingleEvaluationResult,
 )
-from .lib.common import evaluate_ragas, RagasSettings, RagasResult
+from .lib.common import env_vars, evaluate_ragas, RagasSettings, RagasResult
 
 
 class RagasContextRecallEntry(EvaluatorEntry):
     contexts: list[str]
     expected_output: str
 
 
 class RagasContextRecallEvaluator(
     BaseEvaluator[RagasContextRecallEntry, RagasSettings, RagasResult]
 ):
     """
-    Ragas Context Recall
-
     This evaluator measures the extent to which the retrieved context aligns with the annotated answer, treated as the ground truth. Higher values indicate better performance.
     """
 
+    name = "Ragas Context Recall"
     category = "rag"
-    env_vars = [
-        "OPENAI_API_KEY",
-        "AZURE_CONTENT_SAFETY_ENDPOINT",
-        "AZURE_CONTENT_SAFETY_KEY",
-    ]
+    env_vars = env_vars
+    default_settings = RagasSettings()
     docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/context_recall.html"
+    is_guardrail = False
 
     def evaluate(self, entry: RagasContextRecallEntry) -> SingleEvaluationResult:
         return evaluate_ragas(
             evaluator=self,
             metric="context_recall",
             contexts=entry.contexts,
             ground_truth=entry.expected_output,
```

### Comparing `langevals_ragas-0.1.1/langevals_ragas/context_relevancy.py` & `langevals_ragas-0.1.2/langevals_ragas/context_relevancy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluatorEntry,
     SingleEvaluationResult,
 )
-from .lib.common import evaluate_ragas, RagasSettings, RagasResult
+from .lib.common import env_vars, evaluate_ragas, RagasSettings, RagasResult
 
 
 class RagasContextRelevancyEntry(EvaluatorEntry):
     output: str
     contexts: list[str]
 
 
 class RagasContextRelevancyEvaluator(
     BaseEvaluator[RagasContextRelevancyEntry, RagasSettings, RagasResult]
 ):
     """
-    Ragas Context Relevancy
-
     This metric gauges the relevancy of the retrieved context, calculated based on both the question and contexts. The values fall within the range of (0, 1), with higher values indicating better relevancy.
     """
 
+    name = "Ragas Context Relevancy"
     category = "rag"
-    env_vars = [
-        "OPENAI_API_KEY",
-        "AZURE_CONTENT_SAFETY_ENDPOINT",
-        "AZURE_CONTENT_SAFETY_KEY",
-    ]
+    env_vars = env_vars
+    default_settings = RagasSettings()
     docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/context_relevancy.html"
+    is_guardrail = False
 
     def evaluate(self, entry: RagasContextRelevancyEntry) -> SingleEvaluationResult:
         return evaluate_ragas(
             evaluator=self,
             metric="context_relevancy",
             answer=entry.output,
             contexts=entry.contexts,
```

### Comparing `langevals_ragas-0.1.1/langevals_ragas/faithfulness.py` & `langevals_ragas-0.1.2/langevals_ragas/context_utilization.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluatorEntry,
     SingleEvaluationResult,
 )
-from .lib.common import evaluate_ragas, RagasSettings, RagasResult
+from .lib.common import env_vars, evaluate_ragas, RagasSettings, RagasResult
 
 
-class RagasFaithfulnessEntry(EvaluatorEntry):
+class RagasContextUtilizationEntry(EvaluatorEntry):
+    input: str
     output: str
     contexts: list[str]
 
 
-class RagasFaithfulnessEvaluator(
-    BaseEvaluator[RagasFaithfulnessEntry, RagasSettings, RagasResult]
+class RagasContextUtilizationEvaluator(
+    BaseEvaluator[RagasContextUtilizationEntry, RagasSettings, RagasResult]
 ):
     """
-    Ragas Faithfulness
-
-    This evaluator assesses the extent to which the generated answer is consistent with the provided context. Higher scores indicate better faithfulness to the context.
+    This metric evaluates whether all of the output relevant items present in the contexts are ranked higher or not. Higher scores indicate better utilization.
     """
 
+    name = "Ragas Context Utilization"
     category = "rag"
-    env_vars = [
-        "OPENAI_API_KEY",
-        "AZURE_CONTENT_SAFETY_ENDPOINT",
-        "AZURE_CONTENT_SAFETY_KEY",
-    ]
-    docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/faithfulness.html"
+    env_vars = env_vars
+    default_settings = RagasSettings()
+    docs_url = "https://docs.ragas.io/en/latest/concepts/metrics/context_precision.html"
+    is_guardrail = False
 
-    def evaluate(self, entry: RagasFaithfulnessEntry) -> SingleEvaluationResult:
+    def evaluate(self, entry: RagasContextUtilizationEntry) -> SingleEvaluationResult:
         return evaluate_ragas(
             evaluator=self,
-            metric="faithfulness",
+            metric="context_utilization",
+            question=entry.input,
             answer=entry.output,
             contexts=entry.contexts,
             settings=self.settings,
         )
```

### Comparing `langevals_ragas-0.1.1/PKG-INFO` & `langevals_ragas-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: langevals-ragas
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangEvals Ragas evaluator
 License: MIT
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
 Requires-Dist: langchain_community (>=0.0.27,<0.0.28)
-Requires-Dist: langevals-core (>=0.1.1,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: litellm (>=1.31.3,<2.0.0)
 Requires-Dist: ragas (==0.1.0)
```

