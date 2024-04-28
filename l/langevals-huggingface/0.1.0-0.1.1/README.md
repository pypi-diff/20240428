# Comparing `tmp/langevals_huggingface-0.1.0.tar.gz` & `tmp/langevals_huggingface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_huggingface-0.1.0.tar", max compression
+gzip compressed data, was "langevals_huggingface-0.1.1.tar", max compression
```

## Comparing `langevals_huggingface-0.1.0.tar` & `langevals_huggingface-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,5 @@
--rw-r--r--   0        0        0     2375 2024-03-26 13:24:46.670873 langevals_huggingface-0.1.0/langevals_huggingface/bert_precision.py
--rw-r--r--   0        0        0      474 2024-03-26 13:25:14.091254 langevals_huggingface-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 langevals_huggingface-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1768 2024-04-28 19:56:44.504808 langevals_huggingface-0.1.1/langevals_huggingface/bert_f1.py
+-rw-r--r--   0        0        0     1876 2024-04-28 19:56:44.504808 langevals_huggingface-0.1.1/langevals_huggingface/bert_precision.py
+-rw-r--r--   0        0        0     2082 2024-04-28 19:56:44.504808 langevals_huggingface-0.1.1/langevals_huggingface/bert_recall.py
+-rw-r--r--   0        0        0      805 2024-04-28 19:57:16.624596 langevals_huggingface-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 langevals_huggingface-0.1.1/PKG-INFO
```

### Comparing `langevals_huggingface-0.1.0/langevals_huggingface/bert_precision.py` & `langevals_huggingface-0.1.1/langevals_huggingface/bert_precision.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,55 +5,59 @@
     EvaluationResult,
     SingleEvaluationResult,
 )
 from pydantic import BaseModel, Field
 import evaluate
 
 
-# Type definition of what keys are necessary for each entry to have for the evaluator to process it, in this example
-# we only need the `output` to be available, options are `input`, `output`, `contexts` and `expected_output`
 class BertPrecisionEntry(EvaluatorEntry):
     output: str
     expected_output: str
 
 
-# Generic settings for the evaluator, in this example we don't need any settings, but any fields can be added here
 class BertPrecisionSettings(BaseModel):
     pass
 
 
-# The structure that holds the result of the evaluation, if a score is used, it's a good idea to overwrite the
-# EvaluationResult class to add a pydantic description to the field explaning what the score means for this evaluator,
-# as shown here
 class BertPrecisionResult(EvaluationResult):
     score: float = Field(description="Score from 0 to 1.")
 
 
 class BertPrecisionEvaluator(
     BaseEvaluator[BertPrecisionEntry, BertPrecisionSettings, BertPrecisionResult]
 ):
     """
     How well the words in the generated text match with anything in the expected text.
     If everything in the generated text matches well with things in the expected text, precision is high.
     """
 
-    name = "BERTPrecision"
+    name = "BERT Precision Score"
     category = "similarity"
     env_vars = []
-    docs_url = "https://huggingface.co/spaces/evaluate-metric/bertscore"  # The URL to the official documentation of the evaluator
-    is_guardrail = False  # If the evaluator is a guardrail or not, a guardrail evaluator must return a boolean result on the `passed` result field in addition to the score
+    default_settings = BertPrecisionSettings()
+    docs_url = "https://huggingface.co/spaces/evaluate-metric/bertscore"
+    is_guardrail = False
+
+    @classmethod
+    def preload(cls):
+        cls.metric = evaluate.load("bertscore")
+        cls.metric.compute(
+            predictions=["sample"],
+            references=["sample"],
+            model_type="bert-base-multilingual-cased",
+        )
+        super().preload()
 
     def evaluate(self, entry: BertPrecisionEntry) -> SingleEvaluationResult:
-        metric = evaluate.load("bertscore")
         output_list = [entry.output]
         expected_output_list = [entry.expected_output]
-        result = metric.compute(
+        result = self.metric.compute(
             predictions=output_list,
             references=expected_output_list,
             model_type="bert-base-multilingual-cased",
         )
         if result is None:
-            raise Exception("Unexpected error: BertPrecision did not generate a score")
+            raise Exception("Unexpected error: BERT Precision did not generate a score")
 
         precision = cast(list[float], result.get("precision"))
 
         return BertPrecisionResult(score=precision[0])
```

### Comparing `langevals_huggingface-0.1.0/PKG-INFO` & `langevals_huggingface-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: langevals-huggingface
-Version: 0.1.0
+Version: 0.1.1
 Summary: LangEvals huggingface evaluators.
 License: MIT
 Author: Yevhenii Budnyk
 Author-email: y.budnyk789@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bert-score (>=0.3.13,<0.4.0)
 Requires-Dist: evaluate (>=0.4.1,<0.5.0)
-Requires-Dist: langevals-core (>=0.1.1,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0) ; sys_platform != "linux"
+Requires-Dist: torch (>=2.2.2,<3.0.0) ; sys_platform == "linux"
```

