# Comparing `tmp/langevals_langevals-0.1.0.tar.gz` & `tmp/langevals_langevals-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_langevals-0.1.0.tar", max compression
+gzip compressed data, was "langevals_langevals-0.1.1.tar", max compression
```

## Comparing `langevals_langevals-0.1.0.tar` & `langevals_langevals-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1984 2024-04-09 14:42:59.212500 langevals_langevals-0.1.0/langevals_langevals/blocklist.py
--rw-r--r--   0        0        0     5790 2024-04-09 14:42:59.212500 langevals_langevals-0.1.0/langevals_langevals/off_topic.py
--rw-r--r--   0        0        0      470 2024-04-09 14:43:20.768353 langevals_langevals-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 langevals_langevals-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2186 2024-04-28 19:56:44.504808 langevals_langevals-0.1.1/langevals_langevals/competitor_blocklist.py
+-rw-r--r--   0        0        0     6375 2024-04-28 19:56:44.504808 langevals_langevals-0.1.1/langevals_langevals/competitor_llm.py
+-rw-r--r--   0        0        0     6710 2024-04-28 19:56:44.504808 langevals_langevals-0.1.1/langevals_langevals/off_topic.py
+-rw-r--r--   0        0        0      470 2024-04-28 19:57:20.820565 langevals_langevals-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 langevals_langevals-0.1.1/PKG-INFO
```

### Comparing `langevals_langevals-0.1.0/langevals_langevals/blocklist.py` & `langevals_langevals-0.1.1/langevals_langevals/competitor_blocklist.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,58 +5,66 @@
     SingleEvaluationResult,
 )
 from pydantic import BaseModel, Field
 from typing import List, Optional
 import re
 
 
-class BlocklistEntry(EvaluatorEntry):
+class CompetitorBlocklistEntry(EvaluatorEntry):
     output: Optional[str] = None
     input: Optional[str] = None
 
 
-class BlocklistSettings(BaseModel):
+class CompetitorBlocklistSettings(BaseModel):
     competitors: List[str] = Field(
-        default=[""], description="The competitors that must not be mentioned."
+        default=["OpenAI", "Google", "Microsoft"],
+        description="The competitors that must not be mentioned.",
     )
 
 
-class BlocklistResult(EvaluationResult):
+class CompetitorBlocklistResult(EvaluationResult):
     score: float = Field(
         description="Number of competitors mentioned in the input and output"
     )
     passed: Optional[bool] = Field(
         description="Is the message containing explicit mention of competitor"
     )
-    # details: Optional[str] = Field(
-    #     default="Input or Output contained the mention of the competitor",
-    #     description="Where the competitor mention was detected",
-    # )
 
 
-class BlocklistEvaluator(
-    BaseEvaluator[BlocklistEntry, BlocklistSettings, BlocklistResult]
+class CompetitorBlocklistEvaluator(
+    BaseEvaluator[
+        CompetitorBlocklistEntry, CompetitorBlocklistSettings, CompetitorBlocklistResult
+    ]
 ):
     """
     This evaluator checks if any of the specified competitors was mentioned
     """
 
     name = "Competitor Blocklist"
-    category = "other"
-    env_vars = ["NECESSARY_ENV_VAR"]
+    category = "policy"
+    env_vars = []
+    default_settings = CompetitorBlocklistSettings()
     docs_url = "https://path/to/official/docs"
     is_guardrail = True
 
-    def evaluate(self, entry: BlocklistEntry) -> SingleEvaluationResult:
+    def evaluate(self, entry: CompetitorBlocklistEntry) -> SingleEvaluationResult:
         passed = True
         escaped_words = [re.escape(word) for word in self.settings.competitors]
         pattern_str = "|".join(escaped_words)
         pattern = re.compile(pattern_str, re.IGNORECASE)
         input_mentioned = re.findall(pattern, entry.input if entry.input else " ")
         output_mentioned = re.findall(pattern, entry.output if entry.output else " ")
         if input_mentioned:
             passed = False
         if output_mentioned:
             passed = False
-        return BlocklistResult(
-            score=len(input_mentioned) + len(output_mentioned), passed=passed
+
+        details = None
+        if not passed:
+            details = "Competitors mentioned: " + ", ".join(
+                input_mentioned + output_mentioned
+            )
+        return CompetitorBlocklistResult(
+            score=len(input_mentioned) + len(output_mentioned),
+            passed=passed,
+            details=details,
         )
```

### Comparing `langevals_langevals-0.1.0/langevals_langevals/off_topic.py` & `langevals_langevals-0.1.1/langevals_langevals/off_topic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,150 @@
+import litellm
+from litellm import get_max_tokens
+from litellm import ModelResponse, Choices, Message
+from litellm.utils import completion_cost, trim_messages
+
+from pydantic import BaseModel, Field
+from typing import Optional, List, Literal, cast
+import json
+import os
+
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     EvaluatorEntry,
     EvaluationResult,
     SingleEvaluationResult,
     EvaluationResultSkipped,
     Money,
 )
-import litellm
-from litellm import ModelResponse, Choices, Message
-from litellm.utils import completion_cost
-from pydantic import BaseModel, Field
-from typing import Optional, List, Literal, cast
-import json
-import os
 
 
 class OffTopicEntry(EvaluatorEntry):
     input: str
 
 
 class AllowedTopic(BaseModel):
-    topic: str 
+    topic: str
     description: str
 
 
 class OffTopicSettings(BaseModel):
     allowed_topics: List[AllowedTopic] = Field(
         default=[
-            AllowedTopic(topic="other", description="Any other topic"),
-            AllowedTopic(topic="simple_chat", description="Smalltalk with user"),
-            AllowedTopic(topic="programming_question", description="Question concerning programming and software development")
+            AllowedTopic(topic="simple_chat", description="Smalltalk with the user"),
+            AllowedTopic(
+                topic="company",
+                description="Questions about the company, what we do, etc",
+            ),
         ],
         description="The list of topics and their short descriptions that the chatbot is allowed to talk about",
-        min_length=3
     )
     model: Literal[
         "openai/gpt-3.5-turbo-1106",
         "openai/gpt-3.5-turbo-0125",
         "openai/gpt-4-1106-preview",
         "openai/gpt-4-0125-preview",
         "azure/gpt-35-turbo-1106",
         "azure/gpt-4-1106-preview",
     ] = Field(
         default="openai/gpt-3.5-turbo-0125",
         description="The model to use for evaluation",
     )
-    
+    max_tokens: int = Field(
+        default=get_max_tokens("gpt-3.5-turbo-0125"),
+        description="Max tokens allowed for evaluation",
+    )
 
 
 class OffTopicResult(EvaluationResult):
     score: float = Field(description="Confidence level of the intent prediction")
     passed: Optional[bool] = Field(
         description="Is the message concerning allowed topic"
     )
     details: Optional[str] = Field(
-        default="1.0 confidence that the actual intent is other", description="Predicted intent of the message and the confidence"
+        default="1.0 confidence that the actual intent is other",
+        description="Predicted intent of the message and the confidence",
     )
 
 
 class OffTopicEvaluator(BaseEvaluator[OffTopicEntry, OffTopicSettings, OffTopicResult]):
     """
     This evaluator checks if the user message is concerning one of the allowed topics of the chatbot
     """
 
     name = "Off Topic Evaluator"
-    category = "other"
+    category = "policy"
     env_vars = ["OPENAI_API_KEY", "AZURE_API_KEY", "AZURE_API_BASE"]
     docs_url = "https://path/to/official/docs"  # The URL to the official documentation of the evaluator
     is_guardrail = True  # If the evaluator is a guardrail or not, a guardrail evaluator must return a boolean result on the `passed` result field in addition to the score
 
     def evaluate(self, entry: OffTopicEntry) -> SingleEvaluationResult:
         vendor, model = self.settings.model.split("/")
         if vendor == "azure":
             os.environ["AZURE_API_KEY"] = self.get_env("AZURE_API_KEY")
             os.environ["AZURE_API_BASE"] = self.get_env("AZURE_API_BASE")
             os.environ["AZURE_API_VERSION"] = "2023-07-01-preview"
 
         content = entry.input or ""
         if not content:
             return EvaluationResultSkipped(details="Input is empty")
-        topics_descriptions = [f"Intent: {allowed_topic.topic} - description: {allowed_topic.description}" for allowed_topic in self.settings.allowed_topics]
+        topics_descriptions = "\n #".join(
+            [
+                f"Intent: {allowed_topic.topic} - Description: {allowed_topic.description}"
+                for allowed_topic in self.settings.allowed_topics
+            ]
+        )
         litellm_model = model if vendor == "openai" else f"{vendor}/{model}"
-        prompt = f"You are an intent classification system. Your goal is to identify the intent of the message. Consider these intents and their following descriptions: {"\n #".join(topics_descriptions)}"
+        prompt = f"You are an intent classification system. Your goal is to identify the intent of the message. Consider these intents and their following descriptions: {topics_descriptions}"
+
+        max_tokens_retrieved = get_max_tokens(litellm_model)
+        if max_tokens_retrieved is None:
+            raise ValueError("Model not mapped yet, cannot retrieve max tokens.")
+        llm_max_tokens: int = int(max_tokens_retrieved)
+        max_tokens = (
+            min(self.settings.max_tokens, llm_max_tokens)
+            if self.settings.max_tokens
+            else llm_max_tokens
+        )
+        messages = [
+            {
+                "role": "system",
+                "content": prompt,
+            },
+            {
+                "role": "user",
+                "content": content,
+            },
+        ]
+        messages = cast(
+            List[dict[str, str]],
+            trim_messages(messages, litellm_model, max_tokens=max_tokens),
+        )
+
         response = litellm.completion(
             model=litellm_model,
-            messages=[
-                {
-                    "role": "system",
-                    "content": prompt,
-                },
-                {
-                    "role": "user",
-                    "content": content,
-                },
-            ],
+            messages=messages,
             tools=[
                 {
                     "type": "function",
                     "function": {
                         "name": "identify_intent",
                         "description": "Identify the intent of the message",
                         "parameters": {
                             "type": "object",
                             "properties": {
                                 "intent": {
                                     "type": "string",
                                     "description": "The intent of the user message, what is the message about",
-                                    "enum": list(set(allowed_topic.topic for allowed_topic in self.settings.allowed_topics))
+                                    "enum": list(
+                                        set(
+                                            allowed_topic.topic
+                                            for allowed_topic in self.settings.allowed_topics
+                                        )
+                                    )
                                     + ["other"],
                                 },
                                 "confidence": {
                                     "type": "number",
                                     "description": "Confidence in the identified intent on the scale from 0.0 to 1.0",
                                 },
                             },
@@ -130,11 +164,11 @@
         confidence = arguments["confidence"]
         cost = completion_cost(completion_response=response, prompt=prompt)
 
         passed: bool = intent not in ["other"]
         cost = completion_cost(completion_response=response)
         return OffTopicResult(
             score=float(confidence),
-            details=f"{confidence} confidence that the actual intent is {intent}",
+            details=f"Detected intent: {intent}",
             passed=passed,
             cost=Money(amount=cost, currency="USD") if cost else None,
         )
```

### Comparing `langevals_langevals-0.1.0/PKG-INFO` & `langevals_langevals-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-langevals
-Version: 0.1.0
+Version: 0.1.1
 Summary: LangEvals house-made classification.
 License: MIT
 Author: Yevhenii Budnyk
 Author-email: y.budnyk789@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langevals-core (>=0.1.1,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
 Requires-Dist: litellm (>=1.31.3,<2.0.0)
 Requires-Dist: openai (==1.13.3)
```

