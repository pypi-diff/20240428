# Comparing `tmp/developergpt-0.7.0.tar.gz` & `tmp/developergpt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.7.0.tar", last modified: Tue Apr 23 03:07:48 2024, max compression
+gzip compressed data, was "developergpt-0.7.1.tar", last modified: Sun Apr 28 19:24:19 2024, max compression
```

## Comparing `developergpt-0.7.0.tar` & `developergpt-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.912621 developergpt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 03:07:40.000000 developergpt-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 03:07:40.000000 developergpt-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-23 03:07:48.912621 developergpt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-23 03:07:40.000000 developergpt-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.908621 developergpt-0.7.0/developergpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/gemini_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.908621 developergpt-0.7.0/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:07:48.912621 developergpt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 03:07:40.000000 developergpt-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.908621 developergpt-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:40.000000 developergpt-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-23 03:07:40.000000 developergpt-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 03:07:40.000000 developergpt-0.7.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.203080 developergpt-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-28 19:24:10.000000 developergpt-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 19:24:10.000000 developergpt-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-28 19:24:19.203080 developergpt-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-28 19:24:10.000000 developergpt-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.199080 developergpt-0.7.1/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/gemini_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.203080 developergpt-0.7.1/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:24:19.203080 developergpt-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-28 19:24:10.000000 developergpt-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.203080 developergpt-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:10.000000 developergpt-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-28 19:24:10.000000 developergpt-0.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 19:24:10.000000 developergpt-0.7.1/tests/test_cli.py
```

### Comparing `developergpt-0.7.0/LICENSE` & `developergpt-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.0/PKG-INFO` & `developergpt-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.0
+Version: 0.7.1
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -35,41 +35,41 @@
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
-As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                          | Source                                                                                                                       | Details                                                  |
-| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)              | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**                   | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Zephyr**                        | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open-Source, Hugging Face Inference API            |
-| **Gemma, Gemma-Base**             | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open-Source, Hugging Face Inference API            |
-| **Mistral-Q6, Mistral-Q4**        | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open-Source, OFFLINE, ON-DEVICE                    |
-| **Mistral** [current not working] | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open-Source, Hugging Face Inference API            |
+| Model(s)                   | Source                                                                                                                       | Details                                                  |
+| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
 # Example
-$ developergpt cmd list all commits that contain the word llm in the last 3 days
+$ developergpt cmd list all git commits that contain the word llm
 ```
 
 ![Natural Language Example 1](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmd_demo.gif)
 
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode: Commands are given without explanation (may be less accurate)
@@ -120,15 +120,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini Pro 1.0. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -151,16 +151,16 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Open-Source Hugging Face Inference API LLMs
-To use open-source LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+#### Using Hugging Face Inference API Open LLMs
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
 See https://huggingface.co/docs/api-inference/index for more details. 
 
 ```bash
 # [OPTIONAL] set Hugging Face token (using zsh for example)
 # You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -169,22 +169,22 @@
 ```
 
 ### Usage and Cost 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### Google Gemini
-As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Hugging Face Hosted Open LLMs 
 As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
-- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, generous free hosted inference API, tools, quantization, and other resources! 
+- Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini Pro API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.7.0/README.md` & `developergpt-0.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
-As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                          | Source                                                                                                                       | Details                                                  |
-| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)              | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**                   | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Zephyr**                        | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open-Source, Hugging Face Inference API            |
-| **Gemma, Gemma-Base**             | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open-Source, Hugging Face Inference API            |
-| **Mistral-Q6, Mistral-Q4**        | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open-Source, OFFLINE, ON-DEVICE                    |
-| **Mistral** [current not working] | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open-Source, Hugging Face Inference API            |
+| Model(s)                   | Source                                                                                                                       | Details                                                  |
+| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
 # Example
-$ developergpt cmd list all commits that contain the word llm in the last 3 days
+$ developergpt cmd list all git commits that contain the word llm
 ```
 
 ![Natural Language Example 1](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmd_demo.gif)
 
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode: Commands are given without explanation (may be less accurate)
@@ -84,15 +84,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini Pro 1.0. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -115,16 +115,16 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Open-Source Hugging Face Inference API LLMs
-To use open-source LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+#### Using Hugging Face Inference API Open LLMs
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
 See https://huggingface.co/docs/api-inference/index for more details. 
 
 ```bash
 # [OPTIONAL] set Hugging Face token (using zsh for example)
 # You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -133,22 +133,22 @@
 ```
 
 ### Usage and Cost 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### Google Gemini
-As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Hugging Face Hosted Open LLMs 
 As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
-- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, generous free hosted inference API, tools, quantization, and other resources! 
+- Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini Pro API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.7.0/developergpt/cli.py` & `developergpt-0.7.1/developergpt/cli.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.0/developergpt/config.py` & `developergpt-0.7.1/developergpt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "mistral-7b-instruct-v0.2.Q4_K_M.gguf",
         "mistral-instruct",
     ),
 }
 
 OPENAI_MODEL_MAP = {
     GPT35: "gpt-3.5-turbo",
-    GPT4: "gpt-4-turbo-preview",
+    GPT4: "gpt-4-turbo",
 }
 
 HF_MODEL_MAP = {
     ZEPHYR: "HuggingFaceH4/zephyr-7b-beta",
     GEMMA: "google/gemma-1.1-7b-it",
     GEMMA_BASE: "google/gemma-7b",
     MISTRAL_HF: "mistralai/Mistral-7B-Instruct-v0.2",
```

### Comparing `developergpt-0.7.0/developergpt/few_shot_prompts.py` & `developergpt-0.7.1/developergpt/few_shot_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {
     "input": "<user input>",
     "error": 0,
     "commands": [
         {
             "seq": <Order of Command>,
             "cmd_to_execute": "<commands and arguments to execute>",
-            "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
+            "cmd_explanations": ["<explanation of command 1>", "<explanation of command 2>", ...],
             "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
         },
         {
             "seq": <Order of Command>,
             "cmd_to_execute": "<commands and arguments to execute>",
             "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
             "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
```

### Comparing `developergpt-0.7.0/developergpt/gemini_adapter.py` & `developergpt-0.7.1/developergpt/gemini_adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 DeveloperGPT by luo-anthony
 """
 
-from typing import Optional
+import json
 
 import google.generativeai as genai
 from google.generativeai import ChatSession, GenerativeModel
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
@@ -107,14 +107,21 @@
         few_shot_prompts.UNKNOWN_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
     format_assistant_response(
         few_shot_prompts.UNKNOWN_QUERY_OUTPUT_EXAMPLE_ONE_FAST,
     ),
 ]
 
+# nescessary otherwise Gemini thinks a request like "kill all Python processes" is dangerous
+GEMINI_SAFETY_SETTING = {
+    "HARM_CATEGORY_DANGEROUS": "BLOCK_NONE",
+    "HARM_CATEGORY_DANGEROUS_CONTENT": "BLOCK_NONE",
+    "HARM_CATEGORY_HARASSMENT": "BLOCK_NONE",
+}
+
 
 def get_model_chat_response(
     *,
     user_input: str,
     console: Console,
     chat_session: "ChatSession",
     temperature: float,
@@ -178,9 +185,30 @@
 
     input_messages.append(format_user_request(user_input))
 
     with console.status("[bold blue]Decoding request") as _:
         response = gemini_model.generate_content(
             contents=input_messages,
             generation_config=genai.types.GenerationConfig(temperature=config.CMD_TEMP),
+            safety_settings=GEMINI_SAFETY_SETTING,
         )
-    return utils.clean_model_output(response.text)
+        raw_output = utils.clean_model_output(response.text)
+        try:
+            _ = json.loads(raw_output)
+            # valid JSON -> return the cleaned output
+            return raw_output
+        except json.decoder.JSONDecodeError as e:
+            # invalid JSON -> ask model to fix JSON
+            fix_json_request = {
+                "role": "user",
+                "parts": [
+                    f"The following JSON cannot be parsed ({e}). Please fix any errors in the JSON and return it (only return the fixed JSON itself). The output should only be a single valid JSON block:\n {raw_output}"
+                ],
+            }
+            response_2 = gemini_model.generate_content(
+                contents=[fix_json_request],
+                generation_config=genai.types.GenerationConfig(
+                    temperature=config.CMD_TEMP
+                ),
+                safety_settings=GEMINI_SAFETY_SETTING,
+            )
+            return utils.clean_model_output(response_2.text)
```

### Comparing `developergpt-0.7.0/developergpt/huggingface_adapter.py` & `developergpt-0.7.1/developergpt/huggingface_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 DeveloperGPT by luo-anthony
 """
 
+import json
 import re
 import sys
 from typing import Optional
 
 import requests
 from huggingface_hub import InferenceClient
 from huggingface_hub import errors as hf_errors
@@ -212,15 +213,14 @@
             input_messages.append(format_user_request(user_input))
             response = client.chat_completion(
                 input_messages,
                 max_tokens=MAX_RESPONSE_TOKENS,
                 temperature=config.CMD_TEMP,
             )
             raw_output = response.choices[0].message.content
-            return raw_output
         else:
             if fast_mode:
                 model_input = (
                     INITIAL_USER_CMD_MSG_FAST
                     + "\n"
                     + "\n".join(
                         HF_EXAMPLE_CMDS_FAST + [format_user_cmd_request(user_input)]
@@ -230,20 +230,40 @@
             else:
                 model_input = (
                     INITIAL_USER_CMD_MSG
                     + "\n"
                     + "\n".join(HF_EXAMPLE_CMDS + [format_user_cmd_request(user_input)])
                     + "\nAssistant:"
                 )
-            return client.text_generation(
+            raw_output = client.text_generation(
                 model_input,
                 max_new_tokens=MAX_RESPONSE_TOKENS,
                 temperature=config.CMD_TEMP,
                 stop_sequences=["User:"],
             )
+        raw_output = utils.clean_model_output(raw_output)
+        try:
+            _ = json.loads(raw_output)
+            # valid JSON -> return the cleaned output
+            return raw_output
+        except json.decoder.JSONDecodeError as e:
+            # invalid JSON -> ask model to extract and fix the JSON
+            extract_json_request = f"""
+The following JSON cannot be parsed ({e}).
+Please fix any errors in the JSON and return it (only return the fixed JSON itself).
+The output should only be a single valid JSON block:\n
+{raw_output}
+            """
+            second_attempt = client.text_generation(
+                extract_json_request,
+                max_new_tokens=MAX_RESPONSE_TOKENS,
+                temperature=config.CMD_TEMP,
+                stop_sequences=["User:"],
+            )
+            return second_attempt
 
 
 def _foundation_model_command(
     *,
     user_input: str,
     console: Console,
     api_token: Optional[str],
```

### Comparing `developergpt-0.7.0/developergpt/openai_adapter.py` & `developergpt-0.7.1/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.0/developergpt/utils.py` & `developergpt-0.7.1/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.0/developergpt.egg-info/PKG-INFO` & `developergpt-0.7.1/developergpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.0
+Version: 0.7.1
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -35,41 +35,41 @@
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
-As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                          | Source                                                                                                                       | Details                                                  |
-| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)              | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**                   | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Zephyr**                        | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open-Source, Hugging Face Inference API            |
-| **Gemma, Gemma-Base**             | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open-Source, Hugging Face Inference API            |
-| **Mistral-Q6, Mistral-Q4**        | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open-Source, OFFLINE, ON-DEVICE                    |
-| **Mistral** [current not working] | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open-Source, Hugging Face Inference API            |
+| Model(s)                   | Source                                                                                                                       | Details                                                  |
+| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
 # Example
-$ developergpt cmd list all commits that contain the word llm in the last 3 days
+$ developergpt cmd list all git commits that contain the word llm
 ```
 
 ![Natural Language Example 1](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmd_demo.gif)
 
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode: Commands are given without explanation (may be less accurate)
@@ -120,15 +120,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini Pro 1.0. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -151,16 +151,16 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Open-Source Hugging Face Inference API LLMs
-To use open-source LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+#### Using Hugging Face Inference API Open LLMs
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
 See https://huggingface.co/docs/api-inference/index for more details. 
 
 ```bash
 # [OPTIONAL] set Hugging Face token (using zsh for example)
 # You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -169,22 +169,22 @@
 ```
 
 ### Usage and Cost 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### Google Gemini
-As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Hugging Face Hosted Open LLMs 
 As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
-- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, generous free hosted inference API, tools, quantization, and other resources! 
+- Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini Pro API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.7.0/developergpt.egg-info/SOURCES.txt` & `developergpt-0.7.1/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.0/setup.py` & `developergpt-0.7.1/setup.py`

 * *Files identical despite different names*

