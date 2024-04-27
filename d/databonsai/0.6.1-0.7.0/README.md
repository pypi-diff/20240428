# Comparing `tmp/databonsai-0.6.1.tar.gz` & `tmp/databonsai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databonsai-0.6.1.tar", last modified: Wed Apr 24 20:54:36 2024, max compression
+gzip compressed data, was "databonsai-0.7.0.tar", last modified: Sat Apr 27 22:52:09 2024, max compression
```

## Comparing `databonsai-0.6.1.tar` & `databonsai-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.676715 databonsai-0.6.1/
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     8579 2024-04-24 20:54:36.675716 databonsai-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     7700 2024-04-22 23:08:59.000000 databonsai-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.619974 databonsai-0.6.1/databonsai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.6.1/databonsai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.656737 databonsai-0.6.1/databonsai/categorize/
--rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.6.1/databonsai/categorize/__init__.py
--rw-rw-rw-   0        0        0     8937 2024-04-24 20:53:10.000000 databonsai-0.6.1/databonsai/categorize/base_categorizer.py
--rw-rw-rw-   0        0        0     5830 2024-04-24 19:19:34.000000 databonsai-0.6.1/databonsai/categorize/multi_categorizer.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.663900 databonsai-0.6.1/databonsai/llm_providers/
--rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.6.1/databonsai/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     6003 2024-04-18 21:09:15.000000 databonsai-0.6.1/databonsai/llm_providers/anthropic_provider.py
--rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.6.1/databonsai/llm_providers/llm_provider.py
--rw-rw-rw-   0        0        0     3950 2024-04-18 21:09:34.000000 databonsai-0.6.1/databonsai/llm_providers/ollama_provider.py
--rw-rw-rw-   0        0        0     6266 2024-04-22 23:05:34.000000 databonsai-0.6.1/databonsai/llm_providers/openai_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.666761 databonsai-0.6.1/databonsai/transform/
--rw-rw-rw-   0        0        0      100 2024-04-22 22:21:51.000000 databonsai-0.6.1/databonsai/transform/__init__.py
--rw-rw-rw-   0        0        0     5650 2024-04-22 20:55:37.000000 databonsai-0.6.1/databonsai/transform/base_transformer.py
--rw-rw-rw-   0        0        0     9868 2024-04-22 22:12:09.000000 databonsai-0.6.1/databonsai/transform/extract_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.669716 databonsai-0.6.1/databonsai/utils/
--rw-rw-rw-   0        0        0       86 2024-04-24 19:46:10.000000 databonsai-0.6.1/databonsai/utils/__init__.py
--rw-rw-rw-   0        0        0     9781 2024-04-24 20:49:28.000000 databonsai-0.6.1/databonsai/utils/apply.py
--rw-rw-rw-   0        0        0      256 2024-04-24 19:58:30.000000 databonsai-0.6.1/databonsai/utils/logs.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.673715 databonsai-0.6.1/databonsai.egg-info/
--rw-rw-rw-   0        0        0     8579 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      580 2024-04-24 19:08:15.000000 databonsai-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 20:54:36.677715 databonsai-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-04-24 19:08:19.000000 databonsai-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.671714 databonsai-0.6.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.6.1/tests/__init__.py
--rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.6.1/tests/test_categorization.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.956708 databonsai-0.7.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     8677 2024-04-27 22:52:09.955716 databonsai-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7798 2024-04-24 21:01:07.000000 databonsai-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.907603 databonsai-0.7.0/databonsai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.7.0/databonsai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.936028 databonsai-0.7.0/databonsai/categorize/
+-rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.7.0/databonsai/categorize/__init__.py
+-rw-rw-rw-   0        0        0    10482 2024-04-27 22:43:24.000000 databonsai-0.7.0/databonsai/categorize/base_categorizer.py
+-rw-rw-rw-   0        0        0     7072 2024-04-27 21:14:07.000000 databonsai-0.7.0/databonsai/categorize/multi_categorizer.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.943540 databonsai-0.7.0/databonsai/llm_providers/
+-rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.7.0/databonsai/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     4505 2024-04-27 22:46:27.000000 databonsai-0.7.0/databonsai/llm_providers/anthropic_provider.py
+-rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.7.0/databonsai/llm_providers/llm_provider.py
+-rw-rw-rw-   0        0        0     2734 2024-04-27 22:47:12.000000 databonsai-0.7.0/databonsai/llm_providers/ollama_provider.py
+-rw-rw-rw-   0        0        0     4714 2024-04-27 22:46:33.000000 databonsai-0.7.0/databonsai/llm_providers/openai_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.946539 databonsai-0.7.0/databonsai/transform/
+-rw-rw-rw-   0        0        0      100 2024-04-22 22:21:51.000000 databonsai-0.7.0/databonsai/transform/__init__.py
+-rw-rw-rw-   0        0        0     5711 2024-04-27 21:38:20.000000 databonsai-0.7.0/databonsai/transform/base_transformer.py
+-rw-rw-rw-   0        0        0     9868 2024-04-22 22:12:09.000000 databonsai-0.7.0/databonsai/transform/extract_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.950710 databonsai-0.7.0/databonsai/utils/
+-rw-rw-rw-   0        0        0       86 2024-04-27 19:25:10.000000 databonsai-0.7.0/databonsai/utils/__init__.py
+-rw-rw-rw-   0        0        0    10040 2024-04-27 20:13:50.000000 databonsai-0.7.0/databonsai/utils/apply.py
+-rw-rw-rw-   0        0        0      256 2024-04-24 19:58:30.000000 databonsai-0.7.0/databonsai/utils/logs.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.953709 databonsai-0.7.0/databonsai.egg-info/
+-rw-rw-rw-   0        0        0     8677 2024-04-27 22:52:09.000000 databonsai-0.7.0/databonsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-04-27 22:52:09.000000 databonsai-0.7.0/databonsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 22:52:09.000000 databonsai-0.7.0/databonsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-27 22:52:09.000000 databonsai-0.7.0/databonsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 22:52:09.000000 databonsai-0.7.0/databonsai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      580 2024-04-27 22:50:39.000000 databonsai-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 22:52:09.957711 databonsai-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-04-27 22:50:33.000000 databonsai-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 22:52:09.952707 databonsai-0.7.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.7.0/tests/test_categorization.py
```

### Comparing `databonsai-0.6.1/LICENSE` & `databonsai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.1/PKG-INFO` & `databonsai-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.6.1
+Version: 0.7.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -85,16 +85,16 @@
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
     llm_provider=provider,
-    examples = few_shot_examples
-
+    examples = few_shot_examples,
+    #strict = False # Default true, set to False to allow for categories not in the provided dict
 )
 category = categorizer.categorize("It's been raining outside all day")
 print(category)
 ```
 
 Output:
```

### Comparing `databonsai-0.6.1/README.md` & `databonsai-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
     llm_provider=provider,
-    examples = few_shot_examples
-
+    examples = few_shot_examples,
+    #strict = False # Default true, set to False to allow for categories not in the provided dict
 )
 category = categorizer.categorize("It's been raining outside all day")
 print(category)
 ```
 
 Output:
```

### Comparing `databonsai-0.6.1/databonsai/categorize/base_categorizer.py` & `databonsai-0.7.0/databonsai/categorize/base_categorizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -84,53 +84,68 @@
                         f"Example response '{response}' is not one of the provided categories, {str(list(self.categories.keys()))}."
                     )
 
         return self
 
     @computed_field
     @property
+    def category_mapping(self) -> Dict[int, str]:
+        return {i: category for i, category in enumerate(self.categories.keys())}
+
+    @computed_field
+    @property
+    def inverse_category_mapping(self) -> Dict[str, int]:
+        return {category: i for i, category in self.category_mapping.items()}
+
+    @computed_field
+    @property
     def system_message(self) -> str:
+        categories_with_numbers = "\n".join(
+            [f"{i}: {desc}" for i, desc in enumerate(self.categories.values())]
+        )
         system_message = f"""
-        Each category is formatted as <category>: <description of data that fits the category>
-        {str(self.categories)}
+        You are a categorization expert, specializing in classifying text data into predefined categories. You cannot use any other categories except those provided.
+        Each category is formatted as <number>: <description of data that fits the category>
+        {categories_with_numbers}
         Classify the given text snippet into one of the following categories:
-        {str(list(self.categories.keys()))}
+        {str(list(range(len(self.categories))))}
         Do not use any other categories.
-        Only reply with the category. Do not make any other conversation.
+        Only reply with the category number. Do not make any other conversation.
         """
-
         # Add in fewshot examples
         if self.examples:
             for example in self.examples:
-                system_message += (
-                    f"\nEXAMPLE: {example['example']}  RESPONSE: {example['response']}"
-                )
+                system_message += f"\nEXAMPLE: {example['example']}  RESPONSE: {self.inverse_category_mapping[example['response']]}"
         return system_message
 
     @computed_field
     @property
     def system_message_batch(self) -> str:
+        categories_with_numbers = "\n".join(
+            [f"{i}: {desc}" for i, desc in enumerate(self.categories.values())]
+        )
         system_message = f"""
-        Each category is formatted as <category>: <description of data that fits the category>
-        {str(self.categories)}
+        You are a categorization expert, specializing in classifying text data into predefined categories. You cannot use any other categories except those provided.
+        Each category is formatted as <number>: <description of data that fits the category>
+        {categories_with_numbers}
         Classify each given text snippet into one of the following categories:
-        {str(list(self.categories.keys()))}.
-         Do not use any other categories. If there are multiple snippets, separate each category with ||. 
-        EXAMPLE: <Text about category 1>  RESPONSE: <Category 1> 
-        EXAMPLE: Content 1: <Text about category 1>, Content 2: <Text about category 2> RESPONSE: <Category 1> || <Category 2>
+        {str(list(range(len(self.categories))))}.
+         Do not use any other categories. If there are multiple snippets, separate each category number with ||. 
+        EXAMPLE: <Text about category 1>  RESPONSE: <Category Number 1> 
+        EXAMPLE: <Text about category 1>||<Text about category 2> RESPONSE: <Category Number 1>||<Category Number 2>
         Choose one category for each text snippet.
-        Only reply with the categories. Do not make any other conversation.
+        Only reply with the category numbers. Do not make any other conversation.
         """
-
         # Add in fewshot examples
         if self.examples:
             system_message += "\n EXAMPLE:"
-            for idx, example in enumerate(self.examples):
-                system_message += f"Content {idx+1}: {example['example']}, "
-            system_message += f"\n RESPONSE: {'||'.join([example['response'] for example in self.examples])}"
+            system_message += (
+                f"{'||'.join([example['example'] for example in self.examples])}"
+            )
+            system_message += f"\n RESPONSE: {'||'.join([str(self.inverse_category_mapping[example['response']]) for example in self.examples])}"
 
         return system_message
 
     def categorize(self, input_data: str) -> str:
         """
         Categorizes the input data using the specified LLM provider.
 
@@ -139,29 +154,31 @@
 
         Returns:
             str: The predicted category for the input data.
 
         Raises:
             ValueError: If the predicted category is not one of the provided categories.
         """
-        # Call the LLM provider to get the predicted category
+        # Call the LLM provider to get the predicted category number
         response = self.llm_provider.generate(self.system_message, input_data)
-        predicted_category = response.strip()
+        predicted_category_number = int(response.strip())
 
-        # Validate that the predicted category is one of the provided categories
-        if predicted_category not in self.categories:
+        # Validate that the predicted category number is within the valid range
+        if predicted_category_number not in self.category_mapping:
             if self.strict:
                 raise ValueError(
-                    f"Predicted category '{predicted_category}' is not one of the provided categories. Use 'strict=False' when instantiating the categorizer to allow categories not in the categories dict."
+                    f"Predicted category number '{predicted_category_number}' is not one of the provided categories. Use 'strict=False' when instantiating the categorizer to allow categories not in the categories dict."
                 )
             else:
                 logger.warning(
-                    f"Predicted category '{predicted_category}' is not one of the provided categories. Use 'strict=True' when instantiating the categorizer to raise an error."
+                    f"Predicted category number '{predicted_category_number}' is not one of the provided categories. Use 'strict=True' when instantiating the categorizer to raise an error."
                 )
 
+        # Convert the category number back to the category key
+        predicted_category = self.category_mapping[predicted_category_number]
         return predicted_category
 
     def categorize_batch(self, input_data: List[str]) -> List[str]:
         """
         Categorizes a batch of input data using the specified LLM provider. For less advanced LLMs, call this method on batches of 3-5 inputs (depending on the length of the input data).
 
         Args:
@@ -171,24 +188,34 @@
             List[str]: A list of predicted categories for the input data.
 
         Raises:
             ValueError: If the predicted categories are not a subset of the provided categories.
         """
         # If there is only one input, call the categorize method
         if len(input_data) == 1:
-            return self.validate_predicted_categories([self.categorize(input_data[0])])
-        # Call the LLM provider to get the predicted category
-        response = self.llm_provider.generate_batch(
-            self.system_message_batch, input_data
+            return self.validate_predicted_categories(
+                [self.categorize(next(iter(input_data)))]
+            )
+
+        input_data_prompt = "||".join(input_data)
+        # Call the LLM provider to get the predicted category numbers
+        response = self.llm_provider.generate(
+            self.system_message_batch, input_data_prompt
         )
-        predicted_categories = [category.strip() for category in response.split("||")]
-        if len(predicted_categories) != len(input_data):
+        predicted_category_numbers = [
+            int(category.strip()) for category in response.split("||")
+        ]
+        if len(predicted_category_numbers) != len(input_data):
             raise ValueError(
-                f"Number of predicted categories ({len(predicted_categories)}) does not match the number of input data ({len(input_data)})."
+                f"Number of predicted categories ({len(predicted_category_numbers)}) does not match the number of input data ({len(input_data)})."
             )
+        # Convert the category numbers back to category keys
+        predicted_categories = [
+            self.category_mapping[number] for number in predicted_category_numbers
+        ]
         return self.validate_predicted_categories(predicted_categories)
 
     def validate_predicted_categories(
         self, predicted_categories: List[str]
     ) -> List[str]:
         # Filter out empty strings from the predicted categories
         filtered_categories = [
```

### Comparing `databonsai-0.6.1/databonsai/categorize/multi_categorizer.py` & `databonsai-0.7.0/databonsai/categorize/multi_categorizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Dict
 from databonsai.categorize.base_categorizer import BaseCategorizer
 from pydantic import model_validator, computed_field
 
 
 class MultiCategorizer(BaseCategorizer):
     """
     A class for categorizing input data into multiple categories using a specified LLM provider.
@@ -32,48 +32,65 @@
                         )
 
         return self
 
     @computed_field
     @property
     def system_message(self) -> str:
+        categories_with_numbers = "\n".join(
+            [f"{i}: {desc}" for i, desc in enumerate(self.categories.values())]
+        )
         system_message = f"""
-        Each category is formatted as <category>: <description of data that fits the category>
-        {str(self.categories)}
+        Each category is formatted as <number>: <description of data that fits the category>
+        {categories_with_numbers}
         Classify the given text snippet into one or more of the following categories:
-        {str(list(self.categories.keys()))}
+        {str(list(range(len(self.categories))))}
         Do not use any other categories.
-        Reply with a list of categories separated by || for each text snippet. Do not make any other conversation.
+        Assign multiple categories to one content snippet by separating the categories with ||. Do not make any other conversation.
         """
 
         # Add in fewshot examples
         if self.examples:
             for example in self.examples:
-                system_message += f"\nEXAMPLE: {example['example']}  RESPONSE: {example['response'].replace(',', '||')}"
+                response_numbers = [
+                    str(self.inverse_category_mapping[category.strip()])
+                    for category in example["response"].split(",")
+                ]
+                system_message += f"\nEXAMPLE: {example['example']}  RESPONSE: {'||'.join(response_numbers)}"
         return system_message
 
     @computed_field
     @property
     def system_message_batch(self) -> str:
-        categories = self.categories
+        categories_with_numbers = "\n".join(
+            [f"{i}: {desc}" for i, desc in enumerate(self.categories.values())]
+        )
         system_message = f"""
-        Each category is formatted as <category>: <description of data that fits the category>
-        {str(categories)}
+        Each category is formatted as <number>: <description of data that fits the category>
+        {categories_with_numbers}
         Classify the given text snippet into one or more of the following categories:
-        {str(list(categories.keys()))}
+        {str(list(range(len(self.categories))))}
         Do not use any other categories.
-        Reply with a list of || separated categories for each content snippet. Separate them with ##. EXAMPLE: Content 1: <content>, Content 2: <content> \n RESPONSE: <category of content1>||<category of content1>##<category of content2> Do not make any other conversation. Do not mention Content in your response.
+        Assign multiple categories to one content snippet by separating the categories with ||. Differentiate between each content snippet using ##. EXAMPLE: <content1>##<content2> \n RESPONSE: <category number of content1>||<category number of content1>##<category number of content2> Do not make any other conversation.
         """
 
         # Add in fewshot examples
         if self.examples:
             system_message += "\nEXAMPLE: "
-            for idx, example in enumerate(self.examples):
-                system_message += f"Content {str(idx+1)}: {example['example']}, "
-            system_message += f"\nRESPONSE: {'##'.join([example['response'].replace(',', '||') for example in self.examples])}"
+            system_message += (
+                f"{'##'.join([example['example'] for example in self.examples])}"
+            )
+            response_numbers_list = []
+            for example in self.examples:
+                response_numbers = [
+                    str(self.inverse_category_mapping[category.strip()])
+                    for category in example["response"].split(",")
+                ]
+                response_numbers_list.append("||".join(response_numbers))
+            system_message += f"\nRESPONSE: {'##'.join(response_numbers_list)}"
         return system_message
 
     def categorize(self, input_data: str) -> str:
         """
         Categorizes the input data into multiple categories using the specified LLM provider.
 
         Args:
@@ -82,18 +99,24 @@
         Returns:
             str: A string of categories for the input data, separated by commas.
 
         Raises:
             ValueError: If the predicted categories are not a subset of the provided categories.
         """
 
-        # Call the LLM provider to get the predicted categories
+        # Call the LLM provider to get the predicted category numbers
         response = self.llm_provider.generate(self.system_message, input_data)
-        predicted_categories = [category.strip() for category in response.split("||")]
-
+        predicted_category_numbers = [
+            int(category.strip()) for category in response.split("||")
+        ]
+
+        # Convert the category numbers back to category keys
+        predicted_categories = [
+            self.category_mapping[number] for number in predicted_category_numbers
+        ]
         return ",".join(self.validate_predicted_categories(predicted_categories))
 
     def categorize_batch(self, input_data: List[str]) -> List[str]:
         """
         Categorizes the input data into multiple categories using the specified LLM provider.
 
         Args:
@@ -102,31 +125,36 @@
         Returns:
             List[str]: A list of predicted categories for the input data. If there are multiple categories, they will be separated by commas.
 
         Raises:
             ValueError: If the predicted categories are not a subset of the provided categories.
         """
         if len(input_data) == 1:
-            return self.validate_predicted_categories([self.categorize(input_data[0])])
-        # Call the LLM provider to get the predicted categories
-        response = self.llm_provider.generate_batch(
-            self.system_message_batch, input_data
+            return [self.categorize(next(iter(input_data)))]
+
+        input_data_prompt = "##".join(input_data)
+        # Call the LLM provider to get the predicted category numbers
+        response = self.llm_provider.generate(
+            self.system_message_batch, input_data_prompt
         )
-        # Split the response into category sets for each input data
-        category_sets = response.split("##")
+        # Split the response into category number sets for each input data
+        category_number_sets = response.split("##")
 
-        if len(category_sets) != len(input_data):
+        if len(category_number_sets) != len(input_data):
             raise ValueError(
-                f"Number of predicted category sets ({len(category_sets)}) does not match the number of input data ({len(input_data)})."
+                f"Number of predicted category sets ({len(category_number_sets)}) does not match the number of input data ({len(input_data)})."
             )
 
         predicted_categories_list = []
-        for category_set in category_sets:
+        for category_number_set in category_number_sets:
+            predicted_category_numbers = [
+                int(category.strip()) for category in category_number_set.split("||")
+            ]
             predicted_categories = [
-                category.strip() for category in category_set.split("||")
+                self.category_mapping[number] for number in predicted_category_numbers
             ]
             predicted_categories_str = ",".join(
                 self.validate_predicted_categories(predicted_categories)
             )
             predicted_categories_list.append(predicted_categories_str)
 
         return predicted_categories_list
```

### Comparing `databonsai-0.6.1/databonsai/llm_providers/anthropic_provider.py` & `databonsai-0.7.0/databonsai/llm_providers/openai_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,62 @@
-import anthropic
+from openai import OpenAI
 from .llm_provider import LLMProvider
 import os
 from functools import wraps
 from tenacity import retry, wait_exponential, stop_after_attempt
 from dotenv import load_dotenv
-from typing import List
+from databonsai.utils.logs import logger
 
 load_dotenv()
 
 
-class AnthropicProvider(LLMProvider):
+class OpenAIProvider(LLMProvider):
     """
-    A provider class to interact with Anthropic's Claude API.
+    A provider class to interact with OpenAI's API.
     Supports exponential backoff retries, since we'll often deal with large datasets.
     """
 
     def __init__(
         self,
         api_key: str = None,
         multiplier: int = 1,
         min_wait: int = 1,
-        max_wait: int = 60,
-        max_tries: int = 10,
-        model: str = "claude-3-haiku-20240307",
+        max_wait: int = 30,
+        max_tries: int = 5,
+        model: str = "gpt-4-turbo",
         temperature: float = 0,
     ):
         """
-        Initializes the ClaudeProvider with an API key and retry parameters.
+        Initializes the OpenAIProvider with an API key and retry parameters.
 
         Parameters:
-        api_key (str): Anthropic API key.
+        api_key (str): OpenAI API key.
         multiplier (int): The multiplier for the exponential backoff in retries.
         min_wait (int): The minimum wait time between retries.
         max_wait (int): The maximum wait time between retries.
         max_tries (int): The maximum number of attempts before giving up.
         model (str): The default model to use for text generation.
         temperature (float): The temperature parameter for text generation.
         """
         super().__init__()
 
         # Provider related configs
         if api_key:
             self.api_key = api_key
         else:
-            self.api_key = os.getenv("ANTHROPIC_API_KEY")
+            self.api_key = os.getenv("OPENAI_API_KEY")
             if not self.api_key:
-                raise ValueError("Anthropic API key not provided.")
+                raise ValueError("OpenAI API key not provided.")
         self.model = model
-        self.client = anthropic.Anthropic(api_key=self.api_key)
+        self.client = OpenAI(api_key=self.api_key)
+        try:
+            self.client.models.retrieve(model)
+        except Exception as e:
+            logger.warning(e.response.status_code)
+            raise ValueError(f"Invalid OpenAI model: {model}") from e
         self.temperature = temperature
         self.input_tokens = 0
         self.output_tokens = 0
 
         # Retry related configs
         self.multiplier = multiplier
         self.min_wait = min_wait
@@ -73,88 +78,46 @@
                 stop=stop_after_attempt(self.max_tries),
             )
             return retry_decorator(method)(self, *args, **kwargs)
 
         return wrapper
 
     @retry_with_exponential_backoff
-    def generate(self, system_prompt: str, user_prompt: str, max_tokens=1000) -> str:
-        """
-        Generates a text completion using Anthropic's Claude API, with a given system and user prompt.
-        This method is decorated with retry logic to handle temporary failures.
-
-        Parameters:
-        system_prompt (str): The system prompt to provide context or instructions for the generation.
-        user_prompt (str): The user's prompt, based on which the text completion is generated.
-        max_tokens (int): The maximum number of tokens to generate in the response.
-
-        Returns:
-        str: The generated text completion.
-        """
-        if not system_prompt:
-            raise ValueError("System prompt is required.")
-        if not user_prompt:
-            raise ValueError("User prompt is required.")
-        response = self.client.messages.create(
-            model=self.model,
-            max_tokens=max_tokens,
-            temperature=self.temperature,
-            system=f"{system_prompt}",
-            messages=[
-                {
-                    "role": "user",
-                    "content": [
-                        {
-                            "type": "text",
-                            "text": user_prompt,
-                        }
-                    ],
-                }
-            ],
-        )
-        self.input_tokens += response.usage.input_tokens
-        self.output_tokens += response.usage.output_tokens
-        return response.content[0].text
-
-    # @retry_with_exponential_backoff
-    def generate_batch(
-        self, system_prompt: str, user_prompts: List[str], max_tokens=1000
+    def generate(
+        self, system_prompt: str, user_prompt: str, max_tokens=1000, json=False
     ) -> str:
         """
         Generates a text completion using OpenAI's API, with a given system and user prompt.
         This method is decorated with retry logic to handle temporary failures.
 
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
         max_tokens (int): The maximum number of tokens to generate in the response.
+        json (bool): Whether to use OpenAI's JSON response format.
 
         Returns:
         str: The generated text completion.
         """
         if not system_prompt:
             raise ValueError("System prompt is required.")
-        if len(user_prompts) == 0:
+        if not user_prompt:
             raise ValueError("User prompt is required.")
-        input_data_prompt = ", ".join(
-            [f"Content {idx+1}: {prompt}" for idx, prompt in enumerate(user_prompts)]
-        )
-        response = self.client.messages.create(
-            model=self.model,
-            max_tokens=max_tokens,
-            temperature=self.temperature,
-            system=f"{system_prompt}",
-            messages=[
-                {
-                    "role": "user",
-                    "content": [
-                        {
-                            "type": "text",
-                            "text": input_data_prompt,
-                        }
-                    ],
-                }
-            ],
-        )
-        self.input_tokens += response.usage.input_tokens
-        self.output_tokens += response.usage.output_tokens
-        return response.content[0].text
+        try:
+            response = self.client.chat.completions.create(
+                model=self.model,
+                messages=[
+                    {"role": "system", "content": system_prompt},
+                    {"role": "user", "content": f"{user_prompt}"},
+                ],
+                temperature=self.temperature,
+                max_tokens=max_tokens,
+                frequency_penalty=0,
+                presence_penalty=0,
+                response_format={"type": "json_object"} if json else {"type": "text"},
+            )
+            self.input_tokens += response.usage.prompt_tokens
+            self.output_tokens += response.usage.completion_tokens
+            return response.choices[0].message.content
+        except Exception as e:
+            logger.warning(f"Error occurred during generation: {str(e)}")
+            raise
```

### Comparing `databonsai-0.6.1/databonsai/llm_providers/llm_provider.py` & `databonsai-0.7.0/databonsai/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.1/databonsai/transform/base_transformer.py` & `databonsai-0.7.0/databonsai/transform/base_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,19 @@
             input_data (List[str]): A list of text data to be transformed.
             max_tokens (int, optional): The maximum number of tokens to generate in each response. Defaults to 1000.
 
         Returns:
             List[str]: A list of transformed data, where each element corresponds to the transformed version of the respective input data.
         """
         if len(input_data) == 1:
-            return [self.transform(input_data[0])]
+            return [self.transform(next(iter(input_data)))]
         # Call the LLM provider to perform the batch transformation
-        response = self.llm_provider.generate_batch(
-            self.system_message_batch, input_data, max_tokens=max_tokens
+        input_data_prompt = "||".join(input_data)
+        response = self.llm_provider.generate(
+            self.system_message_batch, input_data_prompt, max_tokens=max_tokens
         )
 
         # Split the response into individual transformed data
         transformed_data_list = response.split("||")
 
         # Strip any leading/trailing whitespace from each transformed data
         transformed_data_list = [data.strip() for data in transformed_data_list]
```

### Comparing `databonsai-0.6.1/databonsai/transform/extract_transformer.py` & `databonsai-0.7.0/databonsai/transform/extract_transformer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.1/databonsai/utils/apply.py` & `databonsai-0.7.0/databonsai/utils/apply.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,29 +93,34 @@
     if len(output_column) > len(input_column):
         raise ValueError(
             f"The length of the output_column list ({len(output_column)}) is greater than the length of th input_column ({len(input_column)})."
         )
 
     check_func(func)
     success_idx = start_idx
+    num_items = len(input_column)
     try:
-        for i in tqdm(
-            range(start_idx, len(input_column), batch_size),
-            desc="Processing data..",
-            unit="batch",
-        ):
-            batch_end = min(i + batch_size, len(input_column))
-            batch = input_column[i:batch_end]
-            batch_result = func(batch)
-            if i >= len(output_column):
-                output_column.extend(batch_result)
-            else:
-                output_column[i : i + len(batch_result)] = batch_result
-            success_idx = batch_end
+        with tqdm(total=num_items, desc="Processing data..", unit="item") as pbar:
+            for i in range(start_idx, num_items, batch_size):
+                batch_end = min(i + batch_size, num_items)
+                batch = input_column[i:batch_end]
+                batch_result = func(batch)
+
+                # Update output column
+                if i >= len(output_column):
+                    output_column.extend(batch_result)
+                else:
+                    output_column[i : i + len(batch_result)] = batch_result
+
+                # Update progress bar by the number of items processed in this batch
+                pbar.update(len(batch_result))
+
+                success_idx = batch_end
     except Exception as e:
+
         print(f"Error occurred at batch starting at index {success_idx}: {str(e)}")
         print(f"Processing stopped at batch ending at index {success_idx - 1}")
         return success_idx
 
     return min(success_idx, len(input_column))
 
 
@@ -174,52 +179,53 @@
     check_func(func)
     success_idx = start_idx
     ramp_factor = ramp_factor
     reduce_factor = reduce_factor
 
     try:
         remaining_data = input_column[start_idx:]
-        processed_results = []
         batch_size = batch_size
         retry_count = 0
 
         with tqdm(
             total=len(remaining_data), desc="Processing data..", unit="row"
         ) as pbar:
             while len(remaining_data) > 0:
                 try:
                     batch_size = min(batch_size, len(remaining_data))
                     batch = remaining_data[:batch_size]
                     batch_results = func(batch)
-                    processed_results.extend(batch_results)
+
+                    # Update output_column in place
+                    output_column[success_idx : success_idx + batch_size] = (
+                        batch_results
+                    )
+
                     remaining_data = remaining_data[batch_size:]
                     retry_count = 0
+                    success_idx += batch_size
 
                     # Update progress bar
                     pbar.update(batch_size)
 
                     # Increase the batch size using the decayed ramp factor
                     batch_size = min(round(batch_size * ramp_factor), max_batch_size)
                     ramp_factor = max(ramp_factor * ramp_factor_decay, 1.0)
 
                 except Exception as e:
-
                     if retry_count >= max_retries:
                         raise ValueError(
                             f"Processing failed after {max_retries} retries. Error: {str(e)}"
                         )
                     retry_count += 1
-
                     # Decrease the batch size using the decayed reduce factor
                     batch_size = max(round(batch_size * reduce_factor), 1)
                     print(f"Retrying with smaller batch size: {batch_size}")
                     reduce_factor *= reduce_factor_decay
 
-        output_column[start_idx:] = processed_results
-        success_idx = start_idx + len(processed_results)
     except Exception as e:
         print(f"Error occurred at batch starting at index {success_idx}: {str(e)}")
         print(f"Processing stopped at batch ending at index {success_idx - 1}")
         return success_idx
 
     return min(success_idx, len(input_column))
```

### Comparing `databonsai-0.6.1/databonsai.egg-info/PKG-INFO` & `databonsai-0.7.0/databonsai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.6.1
+Version: 0.7.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -85,16 +85,16 @@
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
     llm_provider=provider,
-    examples = few_shot_examples
-
+    examples = few_shot_examples,
+    #strict = False # Default true, set to False to allow for categories not in the provided dict
 )
 category = categorizer.categorize("It's been raining outside all day")
 print(category)
 ```
 
 Output:
```

### Comparing `databonsai-0.6.1/databonsai.egg-info/SOURCES.txt` & `databonsai-0.7.0/databonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.1/pyproject.toml` & `databonsai-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databonsai"
-version = "0.6.1"
+version = "0.7.0"
 description = "A Python package to clean and curate your data with LLMs"
 authors = ["Alvin Ryanputra <databonsai.ai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"  
 
 openai = "^1.16.2"
```

### Comparing `databonsai-0.6.1/setup.py` & `databonsai-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="databonsai",
-    version="0.6.1",
+    version="0.7.0",
     description="A package for cleaning and curating data with LLMs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Alvin Ryanputra",
     author_email="databonsai.ai@gmail.com",
     url="https://github.com/databonsai/databonsai",
     packages=find_packages(),
```

### Comparing `databonsai-0.6.1/tests/test_categorization.py` & `databonsai-0.7.0/tests/test_categorization.py`

 * *Files identical despite different names*

