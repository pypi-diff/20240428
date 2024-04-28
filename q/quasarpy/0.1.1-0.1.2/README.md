# Comparing `tmp/quasarpy-0.1.1.tar.gz` & `tmp/quasarpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.1.1.tar", max compression
+gzip compressed data, was "quasarpy-0.1.2.tar", max compression
```

## Comparing `quasarpy-0.1.1.tar` & `quasarpy-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    31941 2024-04-28 12:15:31.480987 quasarpy-0.1.1/LICENSE
--rw-r--r--   0        0        0      628 2024-04-28 12:15:31.480987 quasarpy-0.1.1/README.md
--rw-r--r--   0        0        0      992 2024-04-28 12:15:31.492987 quasarpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      698 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/__main__.py
--rw-r--r--   0        0        0       21 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2549 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4172 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2586 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4494 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 quasarpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-04-28 12:24:29.197163 quasarpy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      628 2024-04-28 12:24:29.197163 quasarpy-0.1.2/README.md
+-rw-r--r--   0        0        0     1044 2024-04-28 12:24:29.205163 quasarpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      698 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/__main__.py
+-rw-r--r--   0        0        0       21 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2748 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4172 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4494 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 quasarpy-0.1.2/PKG-INFO
```

### Comparing `quasarpy-0.1.1/LICENSE` & `quasarpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/README.md` & `quasarpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/pyproject.toml` & `quasarpy-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.1.1"
+version = "0.1.2"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
 license = "GNU GENERAL PUBLIC LICENSE"
 readme = "README.md"
 
+[tool.poetry.scripts]
+quasar = "quasarpy.cli:main"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "^7.2.6"
 click = "^8.1.7"
 pytest = "^8.0.0"
 python-dotenv = "^1.0.1"
 radon = "^6.0.1"
```

### Comparing `quasarpy-0.1.1/quasarpy/__init__.py` & `quasarpy-0.1.2/quasarpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/algorithm/detector.py` & `quasarpy-0.1.2/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/algorithm/llm.py` & `quasarpy-0.1.2/quasarpy/algorithm/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,21 @@
         )
         if not is_online:
             self.tokenizer = AutoTokenizer.from_pretrained(model_config.model_name)
             self.model = AutoModelForCausalLM.from_pretrained(model_config.model_name)
 
     def _generate_online(self, prompt: str, **kwargs) -> str:
         try:
-            client = huggingface_hub.InferenceClient(token=os.getenv("HUGGINGFACE_TOKEN"))
+            try:
+                token = os.getenv("HUGGINGFACE_TOKEN")
+            except KeyError:
+                self.logger.error("Hugging Face API token not found in the environment variables.")
+                raise
+
+            client = huggingface_hub.InferenceClient(token=token)
             response = client.text_generation(
                 prompt=prompt,
                 model="mistralai/Mistral-7B-Instruct-v0.2",
                 max_new_tokens=self.model_config.max_new_tokens,
                 **kwargs
             )
             return response
```

### Comparing `quasarpy-0.1.1/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.1.2/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.1.2/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/cli/__init__.py` & `quasarpy-0.1.2/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/handler/issue.py` & `quasarpy-0.1.2/quasarpy/handler/issue.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/tests/test_handler.py` & `quasarpy-0.1.2/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/tests/test_utils.py` & `quasarpy-0.1.2/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/utils/analyser.py` & `quasarpy-0.1.2/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/utils/ascii.py` & `quasarpy-0.1.2/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/utils/prompt_template.py` & `quasarpy-0.1.2/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/utils/redis_server.py` & `quasarpy-0.1.2/quasarpy/utils/redis_server.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/quasarpy/utils/templates/report_template.html` & `quasarpy-0.1.2/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.1/PKG-INFO` & `quasarpy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasarpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc.
 License: GNU GENERAL PUBLIC LICENSE
 Author: Khushiyant
 Author-email: khushiyant2002@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

