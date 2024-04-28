# Comparing `tmp/langevals_lingua-0.1.0.tar.gz` & `tmp/langevals_lingua-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_lingua-0.1.0.tar", max compression
+gzip compressed data, was "langevals_lingua-0.1.1.tar", max compression
```

## Comparing `langevals_lingua-0.1.0.tar` & `langevals_lingua-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     6451 2024-03-13 18:51:33.438584 langevals_lingua-0.1.0/langevals_lingua/language_detection.py
--rw-r--r--   0        0        0      477 2024-03-13 18:51:55.062421 langevals_lingua-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 langevals_lingua-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6619 2024-04-28 19:56:44.504808 langevals_lingua-0.1.1/langevals_lingua/language_detection.py
+-rw-r--r--   0        0        0      477 2024-04-28 19:57:24.748537 langevals_lingua-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 langevals_lingua-0.1.1/PKG-INFO
```

### Comparing `langevals_lingua-0.1.0/langevals_lingua/language_detection.py` & `langevals_lingua-0.1.1/langevals_lingua/language_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     BaseEvaluator,
     EvaluatorEntry,
     EvaluationResult,
     EvaluationResultSkipped,
     SingleEvaluationResult,
 )
 from pydantic import BaseModel, Field
-from lingua import IsoCode639_1, LanguageDetectorBuilder
+from lingua import LanguageDetectorBuilder
 
 
 class LinguaLanguageDetectionEntry(EvaluatorEntry):
     input: str
     output: str
 
 
@@ -96,15 +96,15 @@
 
 class LinguaLanguageDetectionSettings(BaseModel):
     check_for: Literal["input_matches_output", "output_matches_language"] = Field(
         default="input_matches_output", description="What should be checked"
     )
     expected_language: Optional[AvailableLanguages] = Field(
         default=None,
-        description="(Optional) The specific language that the output is expected to be",
+        description="The specific language that the output is expected to be",
     )
     min_words: int = Field(
         default=7,
         description="Minimum number of words to check, as the language detection can be unreliable for very short texts. Inputs shorter than the minimum will be skipped.",
     )
     threshold: float = Field(
         default=0.25,
@@ -121,52 +121,57 @@
     score: float = Field(description="How many languages were detected")
     passed: Optional[bool] = Field(
         description="Passes if the detected language on the output matches the detected language on the input, or if the output matches the expected language"
     )
     raw_response: LinguaLanguageDetectionRawResponse
 
 
-detector = (
-    LanguageDetectorBuilder.from_all_languages()
-    .with_preloaded_language_models()
-    .build()
-)
-
-
 class LinguaLanguageDetectionEvaluator(
     BaseEvaluator[
         LinguaLanguageDetectionEntry,
         LinguaLanguageDetectionSettings,
         LinguaLanguageDetectionResult,
     ]
 ):
     """
     This evaluator detects the language of the input and output text to check for example if the generated answer is in the same language as the prompt,
     or if it's in a specific expected language.
     """
 
     name = "Lingua Language Detection"
     category = "quality"
+    default_settings = LinguaLanguageDetectionSettings()
     docs_url = "https://github.com/pemistahl/lingua-py"
     is_guardrail = True
 
+    @classmethod
+    def preload(cls):
+        cls.detector = (
+            LanguageDetectorBuilder.from_all_languages()
+            .with_preloaded_language_models()
+            .build()
+        )
+        super().preload()
+
     def evaluate(self, entry: LinguaLanguageDetectionEntry) -> SingleEvaluationResult:
         words = entry.input.split(" ")
         if self.settings.check_for == "input_matches_output":
             if len(words) < self.settings.min_words:
                 return EvaluationResultSkipped(
                     details=f"Skipped because the input has less than {self.settings.min_words} words"
                 )
         words = entry.output.split(" ")
         if len(words) < self.settings.min_words:
             return EvaluationResultSkipped(
                 details=f"Skipped because the output has less than {self.settings.min_words} words"
             )
 
-        output_languages = detector.compute_language_confidence_values(entry.output)
+        output_languages = self.detector.compute_language_confidence_values(
+            entry.output
+        )
         output_languages = dict(
             [
                 (lang.language.iso_code_639_1.name, lang.value)
                 for lang in output_languages
                 if lang.value > self.settings.threshold
             ]
         )
@@ -174,26 +179,26 @@
             return EvaluationResultSkipped(
                 details=f"Skipped because no language could be detected on the output with a confidence higher than {self.settings.threshold}"
             )
 
         if self.settings.check_for == "output_matches_language":
             passed = (
                 self.settings.expected_language is None
-                or self.settings.expected_language not in output_languages
+                or self.settings.expected_language in output_languages
             )
             return LinguaLanguageDetectionResult(
                 score=len(output_languages),
                 passed=passed,
                 details=f"Languages detected: {', '.join(output_languages.keys())}",
                 raw_response=LinguaLanguageDetectionRawResponse(
                     output=output_languages
                 ),
             )
 
-        input_languages = detector.compute_language_confidence_values(entry.input)
+        input_languages = self.detector.compute_language_confidence_values(entry.input)
         input_languages = dict(
             [
                 (lang.language.iso_code_639_1.name, lang.value)
                 for lang in input_languages
                 if lang.value > self.settings.threshold
             ]
         )
```

### Comparing `langevals_lingua-0.1.0/PKG-INFO` & `langevals_lingua-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langevals-lingua
-Version: 0.1.0
+Version: 0.1.1
 Summary: LangEvals lingua evaluator for language detection.
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
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
```

