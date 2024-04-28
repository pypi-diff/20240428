# Comparing `tmp/yandex-chain-0.0.6.tar.gz` & `tmp/yandex-chain-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandex-chain-0.0.6.tar", last modified: Thu Feb 15 14:56:48 2024, max compression
+gzip compressed data, was "yandex-chain-0.0.7.tar", last modified: Sun Apr 28 14:13:33 2024, max compression
```

## Comparing `yandex-chain-0.0.6.tar` & `yandex-chain-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 14:56:48.169632 yandex-chain-0.0.6/
--rw-rw-rw-   0        0        0     1105 2023-10-05 08:54:06.000000 yandex-chain-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       13 2023-10-10 15:43:55.000000 yandex-chain-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4897 2024-02-15 14:56:48.166620 yandex-chain-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4172 2024-01-25 13:16:44.000000 yandex-chain-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-02-15 14:56:48.170631 yandex-chain-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1067 2024-02-15 14:38:27.000000 yandex-chain-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-15 14:56:48.124619 yandex-chain-0.0.6/yandex_chain/
--rw-rw-rw-   0        0        0     1380 2023-12-11 13:18:45.000000 yandex-chain-0.0.6/yandex_chain/ChatYandexGPT.py
--rw-rw-rw-   0        0        0     4161 2024-02-15 14:48:44.000000 yandex-chain-0.0.6/yandex_chain/YandexGPT.py
--rw-rw-rw-   0        0        0     1966 2023-12-11 11:54:23.000000 yandex-chain-0.0.6/yandex_chain/YandexGPTEmbeddings.py
--rw-rw-rw-   0        0        0      284 2024-02-15 14:38:12.000000 yandex-chain-0.0.6/yandex_chain/__init__.py
--rw-rw-rw-   0        0        0     1532 2023-10-09 20:45:18.000000 yandex-chain-0.0.6/yandex_chain/util.py
-drwxrwxrwx   0        0        0        0 2024-02-15 14:56:48.159620 yandex-chain-0.0.6/yandex_chain.egg-info/
--rw-rw-rw-   0        0        0     4897 2024-02-15 14:56:47.000000 yandex-chain-0.0.6/yandex_chain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-02-15 14:56:47.000000 yandex-chain-0.0.6/yandex_chain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 14:56:47.000000 yandex-chain-0.0.6/yandex_chain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-02-15 14:56:47.000000 yandex-chain-0.0.6/yandex_chain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-02-15 14:56:47.000000 yandex-chain-0.0.6/yandex_chain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 14:13:33.025991 yandex-chain-0.0.7/
+-rw-rw-rw-   0        0        0     1105 2023-10-05 08:54:06.000000 yandex-chain-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-10-10 15:43:55.000000 yandex-chain-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5206 2024-04-28 14:13:33.024990 yandex-chain-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4481 2024-04-28 14:12:52.000000 yandex-chain-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 14:13:33.026990 yandex-chain-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2024-04-28 14:13:27.000000 yandex-chain-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:13:32.999110 yandex-chain-0.0.7/yandex_chain/
+-rw-rw-rw-   0        0        0     1380 2023-12-11 13:18:45.000000 yandex-chain-0.0.7/yandex_chain/ChatYandexGPT.py
+-rw-rw-rw-   0        0        0     4847 2024-04-28 14:07:45.000000 yandex-chain-0.0.7/yandex_chain/YandexGPT.py
+-rw-rw-rw-   0        0        0     1966 2023-12-11 11:54:23.000000 yandex-chain-0.0.7/yandex_chain/YandexGPTEmbeddings.py
+-rw-rw-rw-   0        0        0      300 2024-04-28 14:13:22.000000 yandex-chain-0.0.7/yandex_chain/__init__.py
+-rw-rw-rw-   0        0        0     1532 2023-10-09 20:45:18.000000 yandex-chain-0.0.7/yandex_chain/util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:13:33.021952 yandex-chain-0.0.7/yandex_chain.egg-info/
+-rw-rw-rw-   0        0        0     5206 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/top_level.txt
```

### Comparing `yandex-chain-0.0.6/LICENSE` & `yandex-chain-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.6/PKG-INFO` & `yandex-chain-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-chain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Yandex GPT Support for LangChain
 Home-page: https://github.com/yandex-datasphere/yandex-chain
 Author: Dmitri Soshnikov
 Author-email: dmitri@soshnikov.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -109,15 +109,20 @@
 This chain can now answer our questions:
 ```python
 chain.invoke(query)
 ```
 
 ## Lite vs. Full Models
 
-YandexGPT model comes in two flavours - YandexGPT Lite and full YandexGPT. By default, YandexGPT Lite is used. If you want to use full YandexGPT, you need to specify `use_lite=False` parameter when instantiating `YandexLLM` language model class.
+YandexGPT model comes in three flavours - YandexGPT Lite, YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
+* **Pro** : `model=YandexGPTModel.Pro`
+* **Lite** : `model=YandexGPTModel.Lite`
+* **Summarization** : `model=YandexGPTModel.Summarization`
+
+> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated.
 
 ## Testing
 
 This repository contains some basic unit tests. To run them, you need to place a configuration file `config.json` with your credentials into `tests` folder. Use `config_sample.json` as a reference. After that, please run the following at the repository root directory:
 
 ```bash
 python -m unittest discover -s tests
```

### Comparing `yandex-chain-0.0.6/README.md` & `yandex-chain-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -89,15 +89,20 @@
 This chain can now answer our questions:
 ```python
 chain.invoke(query)
 ```
 
 ## Lite vs. Full Models
 
-YandexGPT model comes in two flavours - YandexGPT Lite and full YandexGPT. By default, YandexGPT Lite is used. If you want to use full YandexGPT, you need to specify `use_lite=False` parameter when instantiating `YandexLLM` language model class.
+YandexGPT model comes in three flavours - YandexGPT Lite, YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
+* **Pro** : `model=YandexGPTModel.Pro`
+* **Lite** : `model=YandexGPTModel.Lite`
+* **Summarization** : `model=YandexGPTModel.Summarization`
+
+> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated.
 
 ## Testing
 
 This repository contains some basic unit tests. To run them, you need to place a configuration file `config.json` with your credentials into `tests` folder. Use `config_sample.json` as a reference. After that, please run the following at the repository root directory:
 
 ```bash
 python -m unittest discover -s tests
```

### Comparing `yandex-chain-0.0.6/setup.py` & `yandex-chain-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name='yandex-chain',
     packages=setuptools.find_namespace_packages('.',exclude=['tests','examples']),
-    version='0.0.6',
+    version='0.0.7',
     install_requires=['requests','langchain==0.1.0','tenacity'],
     description='Yandex GPT Support for LangChain',
     author='Dmitri Soshnikov',
     author_email='dmitri@soshnikov.com',
     url='https://github.com/yandex-datasphere/yandex-chain',
     long_description=readme,
     long_description_content_type='text/markdown; charset=UTF-8',
```

### Comparing `yandex-chain-0.0.6/yandex_chain/ChatYandexGPT.py` & `yandex-chain-0.0.7/yandex_chain/ChatYandexGPT.py`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.6/yandex_chain/YandexGPT.py` & `yandex-chain-0.0.7/yandex_chain/YandexGPT.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 from typing import Any, List, Mapping, Optional
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 import requests
 import langchain
 from langchain_core.language_models.llms import LLM
 from yandex_chain.util import YAuth, YException
 from tenacity import Retrying, RetryError, stop_after_attempt, wait_fixed
+from enum import Enum
+
+class YandexGPTModel(Enum):
+    Lite = 0
+    Pro = 1
+    Summarization = 2
+    Custom = 3
 
 class YandexLLM(LLM):
     temperature : float = 1.0
     max_tokens : int = 1500
     sleep_interval : float = 1.0
     retries = 3
-    use_lite = True
+    use_lite : bool = None
+    model : YandexGPTModel = None
     instruction_text : str = None
     instruction_id : str = None
     iam_token : str = None
     folder_id : str = None
     api_key : str = None
     config : str = None
 
@@ -32,20 +40,30 @@
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
         """Get the identifying parameters."""
         return { "max_tokens": self.max_tokens, "temperature" : self.temperature }
 
     @property
     def _modelUri(self):
+        if self.model is None:
+            if self.use_lite is None:
+                self.model = YandexGPTModel.Lite
+            else:
+                self.model = YandexGPTModel.Lite if self.use_lite else YandexGPTModel.Pro
         if self.instruction_id:
+            self.model = YandexGPTModel.Custom
             return f"ds://{self.instruction_id}"
-        if self.use_lite:
+        if self.model == YandexGPTModel.Lite:
             return f"gpt://{self.folder_id}/yandexgpt-lite/latest"
-        else:
+        elif self.model == YandexGPTModel.Pro:
             return f"gpt://{self.folder_id}/yandexgpt/latest"
+        elif self.model == YandexGPTModel.Summarization:
+            return f"gpt://{self.folder_id}/summarization/latest"
+        else:
+            raise YException("Invalid model flag")
 
     @staticmethod
     def UserMessage(message):
         return { "role" : "user", "text" : message }
 
     @staticmethod
     def AssistantMessage(message):
```

### Comparing `yandex-chain-0.0.6/yandex_chain/YandexGPTEmbeddings.py` & `yandex-chain-0.0.7/yandex_chain/YandexGPTEmbeddings.py`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.6/yandex_chain/util.py` & `yandex-chain-0.0.7/yandex_chain/util.py`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.6/yandex_chain.egg-info/PKG-INFO` & `yandex-chain-0.0.7/yandex_chain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-chain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Yandex GPT Support for LangChain
 Home-page: https://github.com/yandex-datasphere/yandex-chain
 Author: Dmitri Soshnikov
 Author-email: dmitri@soshnikov.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -109,15 +109,20 @@
 This chain can now answer our questions:
 ```python
 chain.invoke(query)
 ```
 
 ## Lite vs. Full Models
 
-YandexGPT model comes in two flavours - YandexGPT Lite and full YandexGPT. By default, YandexGPT Lite is used. If you want to use full YandexGPT, you need to specify `use_lite=False` parameter when instantiating `YandexLLM` language model class.
+YandexGPT model comes in three flavours - YandexGPT Lite, YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
+* **Pro** : `model=YandexGPTModel.Pro`
+* **Lite** : `model=YandexGPTModel.Lite`
+* **Summarization** : `model=YandexGPTModel.Summarization`
+
+> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated.
 
 ## Testing
 
 This repository contains some basic unit tests. To run them, you need to place a configuration file `config.json` with your credentials into `tests` folder. Use `config_sample.json` as a reference. After that, please run the following at the repository root directory:
 
 ```bash
 python -m unittest discover -s tests
```

