# Comparing `tmp/easytl-0.2.1.tar.gz` & `tmp/easytl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.2.1.tar", last modified: Thu Apr 25 01:33:50 2024, max compression
+gzip compressed data, was "easytl-0.3.0.tar", last modified: Sun Apr 28 07:30:18 2024, max compression
```

## Comparing `easytl-0.2.1.tar` & `easytl-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.466145 easytl-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.466145 easytl-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-25 01:32:16.000000 easytl-0.2.1/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-25 01:32:16.000000 easytl-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-25 01:32:16.000000 easytl-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-25 01:33:50.470145 easytl-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-25 01:32:16.000000 easytl-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 01:32:16.000000 easytl-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:33:50.470145 easytl-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.466145 easytl-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    52195 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-25 01:32:16.000000 easytl-0.2.1/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-25 01:32:16.000000 easytl-0.2.1/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.779622 easytl-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.771622 easytl-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.775622 easytl-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-28 07:28:44.000000 easytl-0.3.0/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-28 07:28:44.000000 easytl-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-28 07:28:44.000000 easytl-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-28 07:30:18.779622 easytl-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-04-28 07:28:44.000000 easytl-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-28 07:28:44.000000 easytl-0.3.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-28 07:28:44.000000 easytl-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:30:18.779622 easytl-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.771622 easytl-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.775622 easytl-0.3.0/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68885 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.779622 easytl-0.3.0/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.779622 easytl-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-28 07:28:44.000000 easytl-0.3.0/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-04-28 07:28:44.000000 easytl-0.3.0/tests/passing.py
```

### Comparing `easytl-0.2.1/.github/workflows/workflow.yml` & `easytl-0.3.0/.github/workflows/workflow.yml`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
           python -m pip install build
 
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
+          GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Build the package
         run: |
           python -m build
@@ -62,14 +63,15 @@
           python -m pip install build
 
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
+          GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Build the package
         run: |
           python -m build
@@ -97,14 +99,15 @@
           python -m pip install build
 
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
+          GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Install twine
         run: |
           python -m pip install twine
```

### Comparing `easytl-0.2.1/.gitignore` & `easytl-0.3.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -161,7 +161,8 @@
 .vscode/settings.json
 
 ## test files
 tests/gemini.txt
 tests/openai.txt
 tests/deepl.txt
 tests/easytl-log.txt
+tests/google_translate_key.json
```

### Comparing `easytl-0.2.1/LICENSE.md` & `easytl-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/PKG-INFO` & `easytl-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: easytl
-Version: 0.2.1
-Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, and Gemini.
-Author-email: Bikatr7 <Tetralon07@gmail.com>
-Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
-Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.1
-Requires-Dist: deepl==1.16.1
-Requires-Dist: openai==1.13.3
-Requires-Dist: backoff==2.2.1
-Requires-Dist: tiktoken==0.6.0
-
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
 - [API Usage](#api-usage)
@@ -31,42 +10,42 @@
 - [Contribution](#contribution)
 - [Notes](#notes)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
-Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
+Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 
-EasyTL has a Trello board for tracking features and issues:
+EasyTL has a Trello board for tracking planned features and issues:
 https://trello.com/b/Td555CoW/easytl
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
-Then, you can translate Japanese text using by importing the global client.
+Then, you can translate text using by importing the global client.
 
 For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
 ## Set your API key
-EasyTL.set_api_key("deepL", "your_api_key_here")
+EasyTL.credentials("deepl", "your_api_key_here")
 
 ## You can also validate your API keys; translation functions will do this automatically
-is_valid, e = EasyTL.validate_api_key("deepL")
+is_valid, e = EasyTL.validate_credentials("deepl")
 
-translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality.
+translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN-US") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality and other services.
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
 Python 3.10+
@@ -76,73 +55,88 @@
 ```bash
 pip install easytl
 ```
 
 This will install EasyTL along with its dependencies and requirements.
 
 These are the dependencies/requirements that will be installed:
-```
+```bash
 setuptools>=61.0
 wheel
 setuptools_scm>=6.0
 tomli
 google-generativeai==0.5.1
 deepl==1.16.1
 openai==1.13.3
 backoff==2.2.1
 tiktoken==0.6.0
+google-cloud-translate==3.15.3
 ```
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Features**<a name="features"></a>
 
 EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
 
-- Support for multiple translation APIs including OpenAI, DeepL, and Gemini.
-- Simple API key management.
-- Methods to validate API keys before usage.
-- Cost estimation tools to help manage usage based on text length and service.
+- Support for multiple translation APIs including OpenAI, DeepL, Gemini, and Google Translate.
+- Simple API key and credential management.
+- Methods to validate credentials before usage.
+- Cost estimation tools to help manage usage based on text length, translation instructions for LLMs, and translation services.
 - Highly customizable translation options, with the API's original features.
 - Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **API Usage**<a name="api-usage"></a>
 
 ### Translating Text
 
-Use `deepl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+Use `deepl_translate`, `googletl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+
+All services offer asynchronous translation methods that return a future object for concurrent processing. These methods are suffixed with `_async` and can be awaited to retrieve the translated text.
+
+Instead of receiving the translated text directly, you can also use the `response` parameter to get the full response object from the API.
+
+## Generic Translation Methods
+
+EasyTL has generic translation methods `translate` and `translate_async` that can be used to translate text with any of the supported services. These methods accept the text, service, and kwargs of the respective service as parameters.
 
 ### Cost Calculation
 
 The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
 
 characters or tokens depending on the service.
 
 ```python
-num_characters, cost, model = EasyTL.calculate_cost("Example text.", "deepL")
+num_characters, cost, model = EasyTL.calculate_cost("This has a lot of characters", "deepl")
+```
+
+or 
+
+```python
+num_tokens, cost, model = EasyTL.calculate_cost("This has a lot of tokens.", "openai", model="gpt-4", translation_instructions="Translate this text to Japanese.")
 ```
 
-### API Key Management
+### Credentials Management
 
-API keys can be set and validated using `set_api_key` and `validate_api_key` methods to ensure they are active and correct before submitting translation requests.
+Credentials can be set and validated using `set_credentials` and `validate_credentials` methods to ensure they are active and correct before submitting translation requests.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
-If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
+If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/EasyTL/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
@@ -154,8 +148,8 @@
 
 **Notes**<a name="notes"></a>
 
 EasyTL was originally developed as a part of [Kudasai](https://github.com/Bikatr7/Kudasai), a Japanese preprocessor later turned Machine Translator. It was later split off into its own package to be used independently of Kudasai for multiple reasons.
 
 This package is also my second serious attempt at creating a Python package, so I'm sure there are some things that could be improved. Feedback is welcomed.
 
----------------------------------------------------------------------------------------------------------------------------------------------------
+---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.2.1/README.md` & `easytl-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: easytl
+Version: 0.3.0
+Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
+Author-email: Bikatr7 <Bikatr7@proton.me>
+Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
+Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: google-generativeai==0.5.1
+Requires-Dist: deepl==1.16.1
+Requires-Dist: openai==1.13.3
+Requires-Dist: backoff==2.2.1
+Requires-Dist: tiktoken==0.6.0
+Requires-Dist: google-cloud-translate==3.15.3
+
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
 - [API Usage](#api-usage)
@@ -10,42 +32,42 @@
 - [Contribution](#contribution)
 - [Notes](#notes)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
-Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
+Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 
-EasyTL has a Trello board for tracking features and issues:
+EasyTL has a Trello board for tracking planned features and issues:
 https://trello.com/b/Td555CoW/easytl
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
-Then, you can translate Japanese text using by importing the global client.
+Then, you can translate text using by importing the global client.
 
 For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
 ## Set your API key
-EasyTL.set_api_key("deepL", "your_api_key_here")
+EasyTL.credentials("deepl", "your_api_key_here")
 
 ## You can also validate your API keys; translation functions will do this automatically
-is_valid, e = EasyTL.validate_api_key("deepL")
+is_valid, e = EasyTL.validate_credentials("deepl")
 
-translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality.
+translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN-US") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality and other services.
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
 Python 3.10+
@@ -55,73 +77,88 @@
 ```bash
 pip install easytl
 ```
 
 This will install EasyTL along with its dependencies and requirements.
 
 These are the dependencies/requirements that will be installed:
-```
+```bash
 setuptools>=61.0
 wheel
 setuptools_scm>=6.0
 tomli
 google-generativeai==0.5.1
 deepl==1.16.1
 openai==1.13.3
 backoff==2.2.1
 tiktoken==0.6.0
+google-cloud-translate==3.15.3
 ```
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Features**<a name="features"></a>
 
 EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
 
-- Support for multiple translation APIs including OpenAI, DeepL, and Gemini.
-- Simple API key management.
-- Methods to validate API keys before usage.
-- Cost estimation tools to help manage usage based on text length and service.
+- Support for multiple translation APIs including OpenAI, DeepL, Gemini, and Google Translate.
+- Simple API key and credential management.
+- Methods to validate credentials before usage.
+- Cost estimation tools to help manage usage based on text length, translation instructions for LLMs, and translation services.
 - Highly customizable translation options, with the API's original features.
 - Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **API Usage**<a name="api-usage"></a>
 
 ### Translating Text
 
-Use `deepl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+Use `deepl_translate`, `googletl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+
+All services offer asynchronous translation methods that return a future object for concurrent processing. These methods are suffixed with `_async` and can be awaited to retrieve the translated text.
+
+Instead of receiving the translated text directly, you can also use the `response` parameter to get the full response object from the API.
+
+## Generic Translation Methods
+
+EasyTL has generic translation methods `translate` and `translate_async` that can be used to translate text with any of the supported services. These methods accept the text, service, and kwargs of the respective service as parameters.
 
 ### Cost Calculation
 
 The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
 
 characters or tokens depending on the service.
 
 ```python
-num_characters, cost, model = EasyTL.calculate_cost("Example text.", "deepL")
+num_characters, cost, model = EasyTL.calculate_cost("This has a lot of characters", "deepl")
+```
+
+or 
+
+```python
+num_tokens, cost, model = EasyTL.calculate_cost("This has a lot of tokens.", "openai", model="gpt-4", translation_instructions="Translate this text to Japanese.")
 ```
 
-### API Key Management
+### Credentials Management
 
-API keys can be set and validated using `set_api_key` and `validate_api_key` methods to ensure they are active and correct before submitting translation requests.
+Credentials can be set and validated using `set_credentials` and `validate_credentials` methods to ensure they are active and correct before submitting translation requests.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
-If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
+If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/EasyTL/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
@@ -133,8 +170,8 @@
 
 **Notes**<a name="notes"></a>
 
 EasyTL was originally developed as a part of [Kudasai](https://github.com/Bikatr7/Kudasai), a Japanese preprocessor later turned Machine Translator. It was later split off into its own package to be used independently of Kudasai for multiple reasons.
 
 This package is also my second serious attempt at creating a Python package, so I'm sure there are some things that could be improved. Feedback is welcomed.
 
----------------------------------------------------------------------------------------------------------------------------------------------------
+---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.2.1/pyproject.toml` & `easytl-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 
 [project]
 dependencies = [
     "google-generativeai==0.5.1",
     "deepl==1.16.1",
     "openai==1.13.3",
     "backoff==2.2.1",
-    "tiktoken==0.6.0"
+    "tiktoken==0.6.0",
+    "google-cloud-translate==3.15.3"
 ]
 
 name = "easytl"
-version = "v0.2.1"
+version = "v0.3.0"
 authors = [
-  { name="Bikatr7", email="Tetralon07@gmail.com" },
+  { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
-description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, and Gemini."
+description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
```

### Comparing `easytl-0.2.1/src/easytl/__init__.py` & `easytl-0.3.0/src/easytl/__init__.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/src/easytl/classes.py` & `easytl-0.3.0/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/src/easytl/decorators.py` & `easytl-0.3.0/src/easytl/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,23 @@
 
 def _get_nested_attribute(obj, attrs):
     for attr in attrs:
         try:
             if(isinstance(obj, list) and attr.isdigit()):
                 obj = obj[int(attr)]
             else:
-                obj = getattr(obj, attr)
-        except (AttributeError, IndexError):
+                try:
+                    obj = getattr(obj, attr)
+                except AttributeError:
+                    ## Try dictionary access
+                    obj = obj[attr]
+
+        except (AttributeError, IndexError, KeyError):
             raise ValueError(f"Attribute {attr} in object {obj} not found.")
+        
     return obj
 
 ##-------------------start-of-logging_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _async_logging_decorator(func):
 
     @wraps(func)
@@ -135,9 +141,10 @@
     
     return wrapper
 
 ## Since we're dealing with objects here...
 log_attributes = {
     'GeminiService': ['text'],
     'DeepLService': ['text'],
-    'OpenAIService': ['choices', '0', 'message', 'content']
+    'OpenAIService': ['choices', '0', 'message', 'content'],
+    'GoogleTLService': ['translatedText']
 }
```

### Comparing `easytl-0.2.1/src/easytl/deepl_service.py` & `easytl-0.3.0/src/easytl/deepl_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,19 +106,14 @@
         Prepares the parameters for the translation.
 
         Parameters:
         text (string) : The text to translate.
 
         """
 
-        _is_valid, _e = DeepLService._test_api_key_validity()
-
-        if(not _is_valid and _e):
-            raise _e
-
         if(isinstance(DeepLService._split_sentences, str)):
             DeepLService._split_sentences = SplitSentences[DeepLService._split_sentences]
 
         params = {
             "text": text,
             "target_lang": DeepLService._target_lang,
             "source_lang": DeepLService._source_lang,
@@ -167,19 +162,19 @@
             else:
                 decorated_function = DeepLService._decorator_to_use(DeepLService._translate_text)
                 return decorated_function(**params)
             
         except Exception as _e:
             raise _e
         
-##-------------------start-of-_async_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+##-------------------start-of-_translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     @_async_logging_decorator
-    async def _async_translate_text(text:str) -> typing.Union[typing.List[TextResult], TextResult]:
+    async def _translate_text_async(text:str) -> typing.Union[typing.List[TextResult], TextResult]:
 
         """
 
         Translates the given text to the target language asynchronously.
 
         Parameters:
         text (string) : The text to translate.
@@ -198,15 +193,15 @@
 
             try:
                 if(DeepLService._decorator_to_use is None):
                     loop = asyncio.get_running_loop()
                     return await loop.run_in_executor(None, lambda: DeepLService._translator.translate_text(**params))
                 
                 else:
-                    decorated_function = DeepLService._decorator_to_use(DeepLService._async_translate_text)
+                    decorated_function = DeepLService._decorator_to_use(DeepLService._translate_text_async)
                     return await decorated_function(**params)
                 
             except Exception as _e:
                 raise _e
 
 ##-------------------start-of-_set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.2.1/src/easytl/easytl.py` & `easytl-0.3.0/src/easytl/easytl.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 ## Use of this source code is governed by a GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
+import warnings
+
 ## third-party libraries
 from .classes import Language, SplitSentences, Formality, GlossaryInfo
 
 ## custom modules
 from .deepl_service import DeepLService
 from .gemini_service import GeminiService
 from .openai_service import OpenAIService
+from .googletl_service import GoogleTLService
 
 from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion
 from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException
 
-from .util import _convert_to_correct_type, _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences
+from .util import _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences
 
 class EasyTL:
 
     """
     
     EasyTL global client, used to interact with Translation APIs.
 
-    Use set_api_key() to set the API key for the specified API type.
+    Use set_credentials() to set the credentials for the specified API type. (e.g. set_credentials("deepl", "your_api_key") or set_credentials("google translate", "path/to/your/credentials.json"))
 
-    Use test_api_key_validity() to test the validity of the API key for the specified API type. (Optional) Will be done automatically when calling translation functions.
+    Use test_credentials() to test the validity of the credentials for the specified API type. (e.g. test_credentials("deepl")) (Optional) Done automatically when translating.
 
     Use translate() to translate text using the specified service with it's appropriate kwargs. Or specify the service by calling the specific translation function. (e.g. openai_translate())
 
     Use calculate_cost() to calculate the cost of translating text using the specified service. (Optional)
 
     See the documentation for each function for more information.
 
@@ -41,48 +44,86 @@
 
     @staticmethod
     def set_api_key(api_type:typing.Literal["deepl", "gemini", "openai"], api_key:str) -> None:
         
         """
 
         Sets the API key for the specified API type.
+        For Google Translate, use set_credentials() instead.
+
+        Deprecated: This function is deprecated and will be removed in a future version.
+        Use set_credentials(auth_info) instead.
 
         Parameters:
         api_type (literal["deepl", "gemini", "openai"]) : The API type to set the key for.
         api_key (string) : The API key to set.
 
         """
 
+        warnings.warn("set_api_key is deprecated and will be removed in a future version. Use set_credentials instead.", DeprecationWarning, stacklevel=2)
+
         service_map = {
             "deepl": DeepLService,
             "gemini": GeminiService,
             "openai": OpenAIService
         }
 
         assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini' and 'openai'.")
 
         service_map[api_type]._set_api_key(api_key)
 
+##-------------------start-of-set_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def set_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate"], credentials:str) -> None:
+
+        """
+
+        Sets the credentials for the specified API type.
+
+        Parameters:
+        api_type (literal["deepl", "gemini", "openai", "google translate"]) : The API type to set the credentials for.
+        credentials (string) : The credentials to set. This is an api key for deepl, gemini and openai. For google translate, this is a path to your json that has your service account key.
+
+        """
+
+        service_map = {
+            "deepl": DeepLService._set_api_key,
+            "gemini": GeminiService._set_api_key,
+            "openai": OpenAIService._set_api_key,
+            "google translate": GoogleTLService._set_credentials
+
+        }
+
+        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai' and 'google translate'.")
+
+        service_map[api_type](credentials)
+
 ##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
             
     @staticmethod
     def test_api_key_validity(api_type:typing.Literal["deepl", "gemini", "openai"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
         
         """
 
         Tests the validity of the API key for the specified API type.
+        
+        Deprecated: This function is deprecated and will be removed in a future version.
+        Use test_credentials() instead.
 
         Parameters:
         api_type (literal["deepl", "gemini", "openai"]) : The API type to test the key for.
 
         Returns:
         (bool) : Whether the API key is valid.
         (Exception) : The exception that was raised, if any. None otherwise.
 
         """
+
+        warnings.warn("test_api_key_validity is deprecated and will be removed in a future version. Use test_credentials instead.", DeprecationWarning, stacklevel=2)
         
         api_services = {
             "deepl": {"service": DeepLService, "exception": DeepLException},
             "gemini": {"service": GeminiService, "exception": GoogleAPIError},
             "openai": {"service": OpenAIService, "exception": OpenAIError}
         }
 
@@ -92,15 +133,210 @@
 
         if(not _is_valid):
             ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
             assert isinstance(_e, api_services[api_type]["exception"]), _e
             return False, _e
 
         return True, None
+    
+##-------------------start-of-test_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
+
+        """
+
+        Tests the validity of the credentials for the specified API type.
+
+        Parameters:
+        api_type (literal["deepl", "gemini", "openai", "google translate"]) : The API type to test the credentials for.
+
+        Returns:
+        (bool) : Whether the credentials are valid.
+        (Exception) : The exception that was raised, if any. None otherwise.
+
+        """
+
+        api_services = {
+            "deepl": {"service": DeepLService, "exception": DeepLException, "test_func": DeepLService._test_api_key_validity},
+            "gemini": {"service": GeminiService, "exception": GoogleAPIError, "test_func": GeminiService._test_api_key_validity},
+            "openai": {"service": OpenAIService, "exception": OpenAIError, "test_func": OpenAIService._test_api_key_validity},
+            "google translate": {"service": GoogleTLService, "exception": GoogleAPIError, "test_func": GoogleTLService._test_credentials}
+        }
+
+        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai' and 'google translate'.")
+
+        _is_valid, _e = api_services[api_type]["test_func"]()
+
+        if(not _is_valid):
+            ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
+            assert isinstance(_e, api_services[api_type]["exception"]), _e
+            return False, _e
+
+        return True, None
+    
+##-------------------start-of-googletl_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def googletl_translate(text:typing.Union[str, typing.Iterable[str]],
+                           target_lang:str = "en",
+                           override_previous_settings:bool = True,
+                           decorator:typing.Callable | None = None,
+                           logging_directory:str | None = None,
+                           response_type:typing.Literal["text", "raw"] | None = "text",
+                           translation_delay:float | None = None,
+                           format:typing.Literal["text", "html"] = "text",
+                           source_lang:str | None = None) -> typing.Union[typing.List[str], str, typing.List[typing.Any], typing.Any]:
         
+        """
+
+        Translates the given text to the target language using Google Translate.
+
+        This function assumes that the credentials have already been set.
+
+        It is unknown whether Google Translate has backoff retrying implemented. Assume it does not exist.
+
+        Due to how Google Translate's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
+
+        Google Translate v2 API is poorly documented and type hints are near non-existent. typing.Any return types are used for the raw response type.
+
+        Parameters:
+        text (string or iterable) : The text to translate.
+        target_lang (string) : The target language to translate to.
+        override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Google Translate function.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        format (string or None) : The format of the text. Can be 'text' or 'html'. Default is 'text'. Google Translate appears to be able to translate html but this has not been tested thoroughly by EasyTL.
+        source_lang (string or None) : The source language to translate from.
+
+        Returns:
+        result (string or list - string or any or list - any) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise.
+
+        """
+
+        assert response_type in ["text", "raw"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'raw'.")
+
+        assert format in ["text", "html"], InvalidResponseFormatException("Invalid format specified. Must be 'text' or 'html'.")
+
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_credentials("google translate")
+
+        if(override_previous_settings == True):
+            GoogleTLService._set_attributes(target_language=target_lang, 
+                                            format=format, 
+                                            source_language=source_lang, 
+                                            decorator=decorator, 
+                                            logging_directory=logging_directory, 
+                                            semaphore=None, 
+                                            rate_limit_delay=translation_delay)
+            
+        if(isinstance(text, str)):
+            result = GoogleTLService._translate_text(text)
+        
+            assert not isinstance(result, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = result if response_type == "raw" else result["translatedText"]
+        
+        elif(_is_iterable_of_strings(text)):
+
+            results = [GoogleTLService._translate_text(t) for t in text]
+
+            assert isinstance(results, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = [r["translatedText"] for r in results] if response_type == "text" else results # type: ignore
+            
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
+        
+        return result
+    
+##-------------------start-of-googletl_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    async def googletl_translate_async(text:typing.Union[str, typing.Iterable[str]],
+                                       target_lang:str = "en",
+                                       override_previous_settings:bool = True,
+                                       decorator:typing.Callable | None = None,
+                                       logging_directory:str | None = None,
+                                       response_type:typing.Literal["text", "raw"] | None = "text",
+                                       semaphore:int | None = None,
+                                       translation_delay:float | None = None,
+                                       format:typing.Literal["text", "html"] = "text",
+                                       source_lang:str | None = None) -> typing.Union[typing.List[str], str, typing.List[typing.Any], typing.Any]:
+        
+        """
+
+        Asynchronous version of googletl_translate().
+
+        Translates the given text to the target language using Google Translate.
+        Will generally be faster for iterables. Order is preserved.
+
+        This function assumes that the credentials have already been set.
+
+        It is unknown whether Google Translate has backoff retrying implemented. Assume it does not exist.
+
+        Due to how Google Translate's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
+
+        Google Translate v2 API is poorly documented and type hints are near non-existent. typing.Any return types are used for the raw response type.
+
+        Parameters:
+        text (string or iterable) : The text to translate.
+        target_lang (string) : The target language to translate to.
+        override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Google Translate function.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response.
+        semaphore (int) : The number of concurrent requests to make. Default is 15.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        format (string or None) : The format of the text. Can be 'text' or 'html'. Default is 'text'. Google Translate appears to be able to translate html but this has not been tested thoroughly by EasyTL.
+        source_lang (string or None) : The source language to translate from.
+
+        Returns:
+        result (string or list - string or any or list - any) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise.
+
+        """
+
+        assert response_type in ["text", "raw"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'raw'.")
+
+        assert format in ["text", "html"], InvalidResponseFormatException("Invalid format specified. Must be 'text' or 'html'.")
+
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_credentials("google translate")
+
+        if(override_previous_settings == True):
+            GoogleTLService._set_attributes(target_language=target_lang, 
+                                            format=format, 
+                                            source_language=source_lang, 
+                                            decorator=decorator, 
+                                            logging_directory=logging_directory, 
+                                            semaphore=semaphore, 
+                                            rate_limit_delay=translation_delay)
+            
+        if(isinstance(text, str)):
+            _result = await GoogleTLService._translate_text_async(text)
+
+            assert not isinstance(_result, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = _result if response_type == "raw" else _result["translatedText"]
+            
+        elif(_is_iterable_of_strings(text)):
+            _tasks = [GoogleTLService._translate_text_async(t) for t in text]
+            _results = await asyncio.gather(*_tasks)
+            
+            assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = [_r["translatedText"] for _r in _results] if response_type == "text" else _results # type: ignore
+                
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
+        
+        return result
+    
 ##-------------------start-of-deepl_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def deepl_translate(text:typing.Union[str, typing.Iterable[str]],
                         target_lang:str | Language = "EN-US",
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
@@ -152,15 +388,15 @@
         Returns:
         result (string or list - string or TextResult or list - TextResult) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise.
 
         """
 
         assert response_type in ["text", "raw"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'raw'.")
 
-        EasyTL.test_api_key_validity("deepl")
+        EasyTL.test_credentials("deepl")
 
         if(override_previous_settings == True):
             DeepLService._set_attributes(target_lang = target_lang, 
                                         source_lang = source_lang, 
                                         context = context, 
                                         split_sentences = split_sentences,
                                         preserve_formatting = preserve_formatting, 
@@ -256,15 +492,15 @@
         Returns:
         result (string or list - string or TextResult or list - TextResult) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise.
 
         """
 
         assert response_type in ["text", "raw"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'raw'.")
 
-        EasyTL.test_api_key_validity("deepl")
+        EasyTL.test_credentials("deepl")
 
         if(override_previous_settings == True):
             DeepLService._set_attributes(target_lang=target_lang, 
                                         source_lang=source_lang, 
                                         context=context, 
                                         split_sentences=split_sentences,
                                         preserve_formatting=preserve_formatting, 
@@ -276,22 +512,22 @@
                                         splitting_tags=splitting_tags, 
                                         ignore_tags=ignore_tags,
                                         decorator=decorator,
                                         logging_directory=logging_directory,
                                         semaphore=semaphore,
                                         rate_limit_delay=translation_delay)
         if(isinstance(text, str)):
-            _result = await DeepLService._async_translate_text(text)
+            _result = await DeepLService._translate_text_async(text)
 
             assert not isinstance(_result, list), EasyTLException("Malformed response received. Please try again.")
 
             result = _result if response_type == "raw" else _result.text
             
         elif(_is_iterable_of_strings(text)):
-            _tasks = [DeepLService._async_translate_text(t) for t in text]
+            _tasks = [DeepLService._translate_text_async(t) for t in text]
             _results = await asyncio.gather(*_tasks)
             
             assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
 
             result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
                 
         else:
@@ -353,15 +589,15 @@
         _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
         ## Should be done after validating the settings to reduce cost to the user
-        EasyTL.test_api_key_validity("gemini")
+        EasyTL.test_credentials("gemini")
 
         json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
@@ -459,15 +695,15 @@
         _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
         ## Should be done after validating the settings to reduce cost to the user
-        EasyTL.test_api_key_validity("gemini")
+        EasyTL.test_credentials("gemini")
 
         json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
@@ -558,15 +794,15 @@
         _settings = _return_curated_openai_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "openai")
 
         _validate_stop_sequences(stop)
 
         ## Should be done after validating the settings to reduce cost to the user
-        EasyTL.test_api_key_validity("openai")
+        EasyTL.test_credentials("openai")
 
         json_mode = True if response_type == "json" else False
         
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
@@ -669,15 +905,15 @@
         _settings = _return_curated_openai_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "openai")
 
         _validate_stop_sequences(stop)
 
         ## Should be done after validating the settings to reduce cost to the user
-        EasyTL.test_api_key_validity("openai")
+        EasyTL.test_credentials("openai")
 
         json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
@@ -721,135 +957,158 @@
 
         return result
     
 ##-------------------start-of-translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def translate(text:str | typing.Iterable[str],
-                  service:typing.Optional[typing.Literal["deepl", "openai", "gemini"]] = "deepl", 
+                  service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate"]] = "deepl",
                   **kwargs) -> typing.Union[typing.List[str], str, 
                                             typing.List[TextResult], TextResult, 
+                                            typing.List[ChatCompletion], ChatCompletion,
                                             typing.List[GenerateContentResponse], GenerateContentResponse, 
-                                            typing.List[ChatCompletion], ChatCompletion]:
+                                            typing.List[typing.Any], typing.Any]:
         
         """
 
         Translates the given text to the target language using the specified service.
 
         Please see the documentation for the specific translation function for the service you want to use.
 
-        DeepL: deepl_translate()
-        OpenAI: openai_translate()
-        Gemini: gemini_translate()
+        DeepL: deepl_translate() 
+        OpenAI: openai_translate() 
+        Gemini: gemini_translate() 
+        Google Translate: googletl_translate() 
+
+        All functions can return a list of strings or a string, depending on the input. The response type can be specified to return the raw response instead:
+        DeepL: TextResult
+        OpenAI: ChatCompletion
+        Gemini: GenerateContentResponse
+        Google Translate: any
 
         Parameters:
         service (string) : The service to use for translation.
         text (string) : The text to translate.
         **kwargs : The keyword arguments to pass to the translation function.
 
         Returns:
-        translation (TextResult or list - TextResult) : The translation result.
+        result (string or list - string or TextResult or list - TextResult or ChatCompletion or list - ChatCompletion or GenerateContentResponse or list - GenerateContentResponse or any or list - any) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise. A list of GenerateContentResponse objects if the response type is 'raw' and input was an iterable, a GenerateContentResponse object otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise.
 
         """
 
+        assert service in ["deepl", "openai", "gemini", "google translate"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini' or 'google translate'.")
+
         if(service == "deepl"):
             return EasyTL.deepl_translate(text, **kwargs)
 
         elif(service == "openai"):
             return EasyTL.openai_translate(text, **kwargs)
 
         elif(service == "gemini"):
            return EasyTL.gemini_translate(text, **kwargs)
         
-        else:
-            raise ValueError("Invalid service specified.")
+        elif(service == "google translate"):
+            return EasyTL.googletl_translate(text, **kwargs)
         
 ##-------------------start-of-translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def translate_async(text:str | typing.Iterable[str],
-                              service:typing.Optional[typing.Literal["deepl", "openai", "gemini"]] = "deepl", 
+                              service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate"]] = "deepl",
                               **kwargs) -> typing.Union[typing.List[str], str, 
-                                                        typing.List[TextResult], TextResult, 
-                                                        typing.List[GenerateContentResponse], GenerateContentResponse, 
+                                                        typing.List[TextResult], TextResult,  
                                                         typing.List[ChatCompletion], ChatCompletion,
-                                                        AsyncGenerateContentResponse, typing.List[AsyncGenerateContentResponse]]:
+                                                        typing.List[AsyncGenerateContentResponse], AsyncGenerateContentResponse,
+                                                        typing.List[typing.Any], typing.Any]:
+
         
         """
 
         Asynchronous version of translate().
         
         Translates the given text to the target language using the specified service.
         This function assumes that the API key has already been set.
         translate_async() will generally be faster for iterables. Order is preserved.
 
         Please see the documentation for the specific translation function for the service you want to use.
 
         DeepL: deepl_translate_async()
-        OpenAI: openai_translate_async()
-        Gemini: gemini_translate_async()
+        OpenAI: openai_translate_async() 
+        Gemini: gemini_translate_async() 
+        Google Translate: googletl_translate_async()
+
+        All functions can return a list of strings or a string, depending on the input. The response type can be specified to return the raw response instead:
+        DeepL: TextResult
+        OpenAI: ChatCompletion
+        Gemini: AsyncGenerateContentResponse
+        Google Translate: any
 
         Parameters:
         service (string) : The service to use for translation.
         text (string) : The text to translate.
         **kwargs : The keyword arguments to pass to the translation function.
 
         Returns:
-        translation (TextResult or list - TextResult) : The translation result.
+        result (string or list - string or TextResult or list - TextResult or AsyncGenerateContentResponse or list - AsyncGenerateContentResponse or ChatCompletion or list - ChatCompletion or any or list - any) : The translation result according to the service used.
 
         """
 
+        assert service in ["deepl", "openai", "gemini", "google translate"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini' or 'google translate'.")
+
         if(service == "deepl"):
             return await EasyTL.deepl_translate_async(text, **kwargs)
 
         elif(service == "openai"):
             return await EasyTL.openai_translate_async(text, **kwargs)
 
         elif(service == "gemini"):
             return await EasyTL.gemini_translate_async(text, **kwargs)
         
-        else:
-            raise ValueError("Invalid service specified.")
-        
+        elif(service == "google translate"):
+            return await EasyTL.googletl_translate_async(text, **kwargs)
+
 ##-------------------start-of-calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def calculate_cost(text:str | typing.Iterable[str],
-                       service:typing.Optional[typing.Literal["deepl", "openai", "gemini"]] = "deepl",
+                       service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate"]] = "deepl",
                        model:typing.Optional[str] = None,
                        translation_instructions:typing.Optional[str] = None
                        ) -> typing.Tuple[int, float, str]:
         
         """
 
         Calculates the cost of translating the given text using the specified service.
 
         For LLMs, the cost is based on the default model unless specified.
 
-        Model and Translation Instructions are ignored for DeepL.
+        Model and Translation Instructions are ignored for DeepL and Google Translate.
 
-        For deepl, number of tokens is the number of characters, the returned model is always "deepl"
+        For deepl, number of tokens is the number of characters, the returned model is always "deepl".
+        The same applies for google translate, but the model is "google translate".
 
         Parameters:
         text (string or iterable) : The text to translate.
         service (string) : The service to use for translation.
         model (string or None) : The model to use for translation. If None, the default model is used.
         translation_instructions (string or None) : The translation instructions to use.
 
         Returns:
         num_tokens (int) : The number of tokens/characters in the text.
         cost (float) : The cost of translating the text.
         model (string) : The model used for translation.
 
         """
 
+        assert service in ["deepl", "openai", "gemini", "google translate"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini' or 'google translate'.")
+
         if(service == "deepl"):
             return DeepLService._calculate_cost(text)
         
         elif(service == "openai"):
             return OpenAIService._calculate_cost(text, translation_instructions, model)
 
         elif(service == "gemini"):
             return GeminiService._calculate_cost(text, translation_instructions, model)
         
-        else:
-            raise ValueError("Invalid service specified.")
+        elif(service == "google translate"):
+            return GoogleTLService._calculate_cost(text)
```

### Comparing `easytl-0.2.1/src/easytl/exceptions.py` & `easytl-0.3.0/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/src/easytl/gemini_service.py` & `easytl-0.3.0/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/src/easytl/openai_service.py` & `easytl-0.3.0/src/easytl/openai_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/src/easytl/util.py` & `easytl-0.3.0/src/easytl/util.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/src/easytl.egg-info/PKG-INFO` & `easytl-0.3.0/src/easytl.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.2.1
-Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, and Gemini.
-Author-email: Bikatr7 <Tetralon07@gmail.com>
+Version: 0.3.0
+Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
+Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: google-generativeai==0.5.1
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
+Requires-Dist: google-cloud-translate==3.15.3
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
@@ -31,42 +32,42 @@
 - [Contribution](#contribution)
 - [Notes](#notes)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
-Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
+Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 
-EasyTL has a Trello board for tracking features and issues:
+EasyTL has a Trello board for tracking planned features and issues:
 https://trello.com/b/Td555CoW/easytl
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
-Then, you can translate Japanese text using by importing the global client.
+Then, you can translate text using by importing the global client.
 
 For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
 ## Set your API key
-EasyTL.set_api_key("deepL", "your_api_key_here")
+EasyTL.credentials("deepl", "your_api_key_here")
 
 ## You can also validate your API keys; translation functions will do this automatically
-is_valid, e = EasyTL.validate_api_key("deepL")
+is_valid, e = EasyTL.validate_credentials("deepl")
 
-translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality.
+translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN-US") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality and other services.
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
 Python 3.10+
@@ -76,73 +77,88 @@
 ```bash
 pip install easytl
 ```
 
 This will install EasyTL along with its dependencies and requirements.
 
 These are the dependencies/requirements that will be installed:
-```
+```bash
 setuptools>=61.0
 wheel
 setuptools_scm>=6.0
 tomli
 google-generativeai==0.5.1
 deepl==1.16.1
 openai==1.13.3
 backoff==2.2.1
 tiktoken==0.6.0
+google-cloud-translate==3.15.3
 ```
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Features**<a name="features"></a>
 
 EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
 
-- Support for multiple translation APIs including OpenAI, DeepL, and Gemini.
-- Simple API key management.
-- Methods to validate API keys before usage.
-- Cost estimation tools to help manage usage based on text length and service.
+- Support for multiple translation APIs including OpenAI, DeepL, Gemini, and Google Translate.
+- Simple API key and credential management.
+- Methods to validate credentials before usage.
+- Cost estimation tools to help manage usage based on text length, translation instructions for LLMs, and translation services.
 - Highly customizable translation options, with the API's original features.
 - Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **API Usage**<a name="api-usage"></a>
 
 ### Translating Text
 
-Use `deepl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+Use `deepl_translate`, `googletl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+
+All services offer asynchronous translation methods that return a future object for concurrent processing. These methods are suffixed with `_async` and can be awaited to retrieve the translated text.
+
+Instead of receiving the translated text directly, you can also use the `response` parameter to get the full response object from the API.
+
+## Generic Translation Methods
+
+EasyTL has generic translation methods `translate` and `translate_async` that can be used to translate text with any of the supported services. These methods accept the text, service, and kwargs of the respective service as parameters.
 
 ### Cost Calculation
 
 The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
 
 characters or tokens depending on the service.
 
 ```python
-num_characters, cost, model = EasyTL.calculate_cost("Example text.", "deepL")
+num_characters, cost, model = EasyTL.calculate_cost("This has a lot of characters", "deepl")
+```
+
+or 
+
+```python
+num_tokens, cost, model = EasyTL.calculate_cost("This has a lot of tokens.", "openai", model="gpt-4", translation_instructions="Translate this text to Japanese.")
 ```
 
-### API Key Management
+### Credentials Management
 
-API keys can be set and validated using `set_api_key` and `validate_api_key` methods to ensure they are active and correct before submitting translation requests.
+Credentials can be set and validated using `set_credentials` and `validate_credentials` methods to ensure they are active and correct before submitting translation requests.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
-If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
+If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/EasyTL/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.2.1/src/easytl.egg-info/SOURCES.txt` & `easytl-0.3.0/src/easytl.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .gitignore
 LICENSE.md
 README.md
+SECURITY.md
 pyproject.toml
 .github/workflows/workflow.yml
 src/easytl/__init__.py
 src/easytl/classes.py
 src/easytl/decorators.py
 src/easytl/deepl_service.py
 src/easytl/easytl.py
 src/easytl/exceptions.py
 src/easytl/gemini_service.py
+src/easytl/googletl_service.py
 src/easytl/openai_service.py
 src/easytl/util.py
 src/easytl/version.py
 src/easytl.egg-info/PKG-INFO
 src/easytl.egg-info/SOURCES.txt
 src/easytl.egg-info/dependency_links.txt
 src/easytl.egg-info/requires.txt
```

### Comparing `easytl-0.2.1/tests/issue_template.py` & `easytl-0.3.0/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.1/tests/passing.py` & `easytl-0.3.0/tests/passing.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,40 +12,52 @@
             return file.read().strip()
         
     except:
         pass
 
 def setup_preconditions():
 
-
     gemini_time_delay = 30
 
     deepl_api_key = os.environ.get('DEEPL_API_KEY')
     gemini_api_key = os.environ.get('GEMINI_API_KEY')
     openai_api_key = os.environ.get('OPENAI_API_KEY')
+    json_value = os.environ.get('GOOGLE_TRANSLATE_SERVICE_KEY_VALUE')
+
+    if(json_value is not None):
+
+        with open("json_value.txt", "w") as file:
+            file.write(json_value)
+
+        google_tl_key_path = "json_value.txt"
 
     logging_directory = os.getenv('LOGGING_DIRECTORY', '/tmp/')
 
     if(deepl_api_key is None):
         deepl_api_key = read_api_key("tests/deepl.txt")
     if(gemini_api_key is None):
         gemini_api_key = read_api_key("tests/gemini.txt")
     if(openai_api_key is None):
         openai_api_key = read_api_key("tests/openai.txt")
+
+    if(json_value is None):
+        google_tl_key_path = "tests/google_translate_key.json"
         
         logging_directory = "tests/"
         gemini_time_delay = 5
 
     assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
     assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
     assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
+    assert google_tl_key_path is not None, "GOOGLE_TRANSLATE_SERVICE_KEY_VALUE environment variable must be set"
 
-    EasyTL.set_api_key("deepl", deepl_api_key)
-    EasyTL.set_api_key("gemini", gemini_api_key)
-    EasyTL.set_api_key("openai", openai_api_key)
+    EasyTL.set_credentials("deepl", deepl_api_key)
+    EasyTL.set_credentials("gemini", gemini_api_key)
+    EasyTL.set_credentials("openai", openai_api_key)
+    EasyTL.set_credentials("google translate", google_tl_key_path)
 
     return gemini_time_delay, logging_directory
 
 ##-------------------start-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def main():
 
@@ -76,14 +88,43 @@
 
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="deepl", model=None, translation_instructions=None)
 
     print(f"Characters: {characters}, Cost: {cost}, Model: {model}")
 
+    print("------------------------------------------------Google Translate------------------------------------------------")
+
+    print("------------------------------------------------Text response------------------------------------------------")
+
+    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", logging_directory=logging_directory))
+    print(await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", logging_directory=logging_directory))
+
+    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory)["translatedText"]) # type: ignore
+    result = await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory)
+
+    print(result["translatedText"]) # type: ignore
+
+    print("------------------------------------------------Raw response------------------------------------------------")
+
+    results = EasyTL.googletl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory)
+    async_results = await EasyTL.googletl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory)
+
+    for result in results: # type: ignore
+        print(result["translatedText"]) # type: ignore
+
+    for result in async_results: # type: ignore
+        print(result["translatedText"]) # type: ignore
+
+    print("------------------------------------------------Cost calculation------------------------------------------------")
+
+    characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="google translate", model=None, translation_instructions=None)
+
+    print(f"Characters: {characters}, Cost: {cost}, Model: {model}")
+
     print("------------------------------------------------Gemini------------------------------------------------")
 
     print("-----------------------------------------------Text response-----------------------------------------------")
 
     print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory))
     print(await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory))
```

