# Comparing `tmp/openaichatlib-1.0.5.tar.gz` & `tmp/openaichatlib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openaichatlib-1.0.5.tar", last modified: Fri Apr 12 01:55:13 2024, max compression
+gzip compressed data, was "openaichatlib-1.0.6.tar", last modified: Sun Apr 28 00:58:13 2024, max compression
```

## Comparing `openaichatlib-1.0.5.tar` & `openaichatlib-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-12 01:55:13.821527 openaichatlib-1.0.5/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.5/LICENSE
--rw-r--r--   0 chenshuai   (501) staff       (20)     1419 2024-04-12 01:55:13.820964 openaichatlib-1.0.5/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.5/README.md
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-12 01:55:13.817033 openaichatlib-1.0.5/openaichatlib/
--rw-r--r--   0 chenshuai   (501) staff       (20)    63458 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/V1.py
--rw-r--r--   0 chenshuai   (501) staff       (20)    18400 2024-04-12 01:52:23.000000 openaichatlib-1.0.5/openaichatlib/V3.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      886 2023-11-08 06:33:39.000000 openaichatlib-1.0.5/openaichatlib/__init__.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     4805 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/typings.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     2667 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/utils.py
--rw-r--r--   0 chenshuai   (501) staff       (20)       18 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/version.py
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-12 01:55:13.820221 openaichatlib-1.0.5/openaichatlib.egg-info/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1419 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      349 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       90 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/requires.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/top_level.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-04-12 01:55:13.821653 openaichatlib-1.0.5/setup.cfg
--rw-r--r--   0 chenshuai   (501) staff       (20)     1237 2024-04-12 01:54:50.000000 openaichatlib-1.0.5/setup.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 00:58:13.702372 openaichatlib-1.0.6/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.6/LICENSE
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 00:58:13.701737 openaichatlib-1.0.6/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.6/README.md
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 00:58:13.698096 openaichatlib-1.0.6/openaichatlib/
+-rw-r--r--   0 chenshuai   (501) staff       (20)    18676 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/V3.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/__init__.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/typings.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/utils.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/version.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 00:58:13.701080 openaichatlib-1.0.6/openaichatlib.egg-info/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       45 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/requires.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/top_level.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-04-28 00:58:13.702518 openaichatlib-1.0.6/setup.cfg
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1164 2024-04-28 00:56:45.000000 openaichatlib-1.0.6/setup.py
```

### Comparing `openaichatlib-1.0.5/LICENSE` & `openaichatlib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.5/PKG-INFO` & `openaichatlib-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.5
+Version: 1.0.6
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,21 +12,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prompt-toolkit
 Requires-Dist: httpx[socks]
 Requires-Dist: requests[socks]
-Requires-Dist: OpenAIAuth>=3.0.0
-Requires-Dist: rich
 Requires-Dist: tiktoken>=0.3.0
-Requires-Dist: openai
 
 # OpenAI Chat Python Lib
 
 ## Requirements
 ```
 python: >=3.9
 ```
```

### Comparing `openaichatlib-1.0.5/README.md` & `openaichatlib-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.5/openaichatlib/V3.py` & `openaichatlib-1.0.6/openaichatlib/V3.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,30 +78,30 @@
 
 class Chatbot:
     """
     Official ChatGPT API
     """
 
     def __init__(
-        self,
-        api_key: str,
-        api_url: str = os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions",
-        engine: str = os.environ.get("GPT_ENGINE") or "gpt-3.5-turbo",
-        proxy: str = None,
-        timeout: float = None,
-        max_tokens: int = None,
-        customize_header: dict = None,
-        temperature: float = 0.5,
-        top_p: float = 1.0,
-        presence_penalty: float = 0.0,
-        frequency_penalty: float = 0.0,
-        reply_count: int = 1,
-        truncate_limit: int = None,
-        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
-        count_tokens: bool = True,
+            self,
+            api_key: str,
+            api_url: str = os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions",
+            engine: str = os.environ.get("GPT_ENGINE") or "gpt-3.5-turbo",
+            proxy: str = None,
+            timeout: float = None,
+            max_tokens: int = None,
+            customize_header: dict = None,
+            temperature: float = 0.5,
+            top_p: float = 1.0,
+            presence_penalty: float = 0.0,
+            frequency_penalty: float = 0.0,
+            reply_count: int = 1,
+            truncate_limit: int = None,
+            system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
+            count_tokens: bool = True,
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.api_url: str = api_url
         self.engine: str = engine
         self.api_key: str = api_key
@@ -149,15 +149,15 @@
         self.session.proxies.update(
             {
                 "http": proxy,
                 "https": proxy,
             },
         )
         if proxy := (
-            proxy or os.environ.get("all_proxy") or os.environ.get("ALL_PROXY") or None
+                proxy or os.environ.get("all_proxy") or os.environ.get("ALL_PROXY") or None
         ):
             if "socks5h" not in proxy:
                 self.aclient = httpx.AsyncClient(
                     follow_redirects=True,
                     proxies=proxy,
                     timeout=timeout,
                 )
@@ -177,18 +177,18 @@
             ],
         }
 
         # if self.get_token_count("default") > self.max_tokens:
         #     raise t.ActionRefuseError("System prompt is too long")
 
     def add_to_conversation(
-        self,
-        message,
-        role: str,
-        convo_id: str = "default",
+            self,
+            message,
+            role: str,
+            convo_id: str = "default",
     ) -> None:
         """
         Add a message to the conversation
         """
         self.conversation[convo_id].append({"role": role, "content": message})
 
     def __truncate_conversation(self, convo_id: str = "default") -> None:
@@ -197,16 +197,16 @@
         """
         if not self.count_tokens:
             return
         if self.engine in ENGINES_CLAUDE:
             return
         while True:
             if (
-                self.get_token_count(convo_id) > self.truncate_limit
-                and len(self.conversation[convo_id]) > 1
+                    self.get_token_count(convo_id) > self.truncate_limit
+                    and len(self.conversation[convo_id]) > 1
             ):
                 # Don't remove the first message
                 self.conversation[convo_id].pop(1)
             else:
                 break
 
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
@@ -249,40 +249,40 @@
         if not self.count_tokens:
             return None
         if self.engine in ENGINES_GPT35_TURBO or self.engine in ENGINES_PREVIEW or self.engine in ENGINES_CLAUDE:
             return 4096
         return self.max_tokens - self.get_token_count(convo_id)
 
     def ask_stream(
-        self,
-        prompt,
-        role: str = "user",
-        convo_id: str = "default",
-        model: str = None,
-        pass_history: bool = True,
-        json_format: bool = False,
-        stream: bool = True,
-        **kwargs,
+            self,
+            prompt,
+            role: str = "user",
+            convo_id: str = "default",
+            model: str = None,
+            pass_history: bool = True,
+            json_format: bool = False,
+            stream: bool = True,
+            **kwargs,
     ):
         """
         Ask a question
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation:
             self.reset(convo_id=convo_id, system_prompt=self.system_prompt)
         self.add_to_conversation(prompt, "user", convo_id=convo_id)
         self.__truncate_conversation(convo_id=convo_id)
         # Get response
         if os.environ.get("API_URL") and os.environ.get("MODEL_NAME"):
             # https://learn.microsoft.com/en-us/azure/cognitive-services/openai/chatgpt-quickstart?tabs=command-line&pivots=rest-api
             url = (
-                os.environ.get("API_URL")
-                + "openai/deployments/"
-                + os.environ.get("MODEL_NAME")
-                + "/chat/completions?api-version=2023-05-15"
+                    os.environ.get("API_URL")
+                    + "openai/deployments/"
+                    + os.environ.get("MODEL_NAME")
+                    + "/chat/completions?api-version=2023-05-15"
             )
             headers = {"Content-Type": "application/json", "api-key": self.api_key}
         else:
             url = (
                 self.api_url
             )
             headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
@@ -354,22 +354,22 @@
             response_role = delta["role"]
             content = delta["content"]
             full_response = content
             yield content
         self.add_to_conversation(full_response, response_role, convo_id=convo_id)
 
     async def ask_stream_async(
-        self,
-        prompt,
-        role: str = "user",
-        convo_id: str = "default",
-        model: str = None,
-        pass_history: bool = True,
-        json_format: bool = False,
-        **kwargs,
+            self,
+            prompt,
+            role: str = "user",
+            convo_id: str = "default",
+            model: str = None,
+            pass_history: bool = True,
+            json_format: bool = False,
+            **kwargs,
     ) -> AsyncGenerator[str, None]:
         """
         Ask a question
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation:
             self.reset(convo_id=convo_id, system_prompt=self.system_prompt)
@@ -401,19 +401,19 @@
                 "type": "json_object"
             }
         headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
         if self.customize_header:
             headers.update(self.customize_header)
         # Get response
         async with self.aclient.stream(
-            "post",
-            self.api_url,
-            headers=headers,
-            json=payload,
-            timeout=kwargs.get("timeout", self.timeout),
+                "post",
+                self.api_url,
+                headers=headers,
+                json=payload,
+                timeout=kwargs.get("timeout", self.timeout),
         ) as response:
             if response.status_code != 200:
                 await response.aread()
                 raise t.APIConnectionError(
                     f"{response.status_code} {response.reason_phrase} {response.text}",
                 )
 
@@ -441,22 +441,22 @@
                 if "content" in delta:
                     content: str = delta["content"]
                     full_response += content
                     yield content
         self.add_to_conversation(full_response, response_role, convo_id=convo_id)
 
     async def ask_async(
-        self,
-        prompt,
-        role: str = "user",
-        convo_id: str = "default",
-        model: str = None,
-        pass_history: bool = True,
-        json_format: bool = False,
-        **kwargs,
+            self,
+            prompt,
+            role: str = "user",
+            convo_id: str = "default",
+            model: str = None,
+            pass_history: bool = True,
+            json_format: bool = False,
+            **kwargs,
     ) -> str:
         """
         Non-streaming ask
         """
         response = self.ask_stream_async(
             prompt=prompt,
             role=role,
@@ -464,22 +464,22 @@
             json_format=json_format,
             **kwargs,
         )
         full_response: str = "".join([r async for r in response])
         return full_response
 
     def ask(
-        self,
-        prompt,
-        role: str = "user",
-        convo_id: str = "default",
-        model: str = None,
-        pass_history: bool = True,
-        json_format: bool = False,
-        **kwargs,
+            self,
+            prompt,
+            role: str = "user",
+            convo_id: str = "default",
+            model: str = None,
+            pass_history: bool = True,
+            json_format: bool = False,
+            **kwargs,
     ) -> str:
         """
         Non-streaming ask
         """
         response = self.ask_stream(
             prompt=prompt,
             role=role,
@@ -533,18 +533,18 @@
         """
         with open(file, encoding="utf-8") as f:
             # load json, if session is in keys, load proxies
             loaded_config = json.load(f)
             keys = get_filtered_keys_from_object(self, *keys_)
 
             if (
-                "session" in keys
-                and loaded_config["session"]
-                or "proxy" in keys
-                and loaded_config["proxy"]
+                    "session" in keys
+                    and loaded_config["session"]
+                    or "proxy" in keys
+                    and loaded_config["proxy"]
             ):
                 self.proxy = loaded_config.get("session", loaded_config["proxy"])
                 self.session = httpx.Client(
                     follow_redirects=True,
                     proxies=self.proxy,
                     timeout=self.timeout,
                     cookies=self.session.cookies,
```

### Comparing `openaichatlib-1.0.5/openaichatlib/__init__.py` & `openaichatlib-1.0.6/openaichatlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         raise error
     if int(__import__("platform").python_version_tuple()[1]) < 9:
         error = t.NotAllowRunning(
             f"Not available Python version: {__import__('platform').python_version()}",
         )
         raise error
     if (
-        int(__import__("platform").python_version_tuple()[1]) < 10
-        and int(__import__("platform").python_version_tuple()[0]) == 3
+            int(__import__("platform").python_version_tuple()[1]) < 10
+            and int(__import__("platform").python_version_tuple()[0]) == 3
     ):
         __import__("warnings").warn(
             UserWarning(
                 "The current Python is not a recommended version, 3.10+ is recommended",
             ),
         )
```

### Comparing `openaichatlib-1.0.5/openaichatlib.egg-info/PKG-INFO` & `openaichatlib-1.0.6/openaichatlib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.5
+Version: 1.0.6
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,21 +12,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prompt-toolkit
 Requires-Dist: httpx[socks]
 Requires-Dist: requests[socks]
-Requires-Dist: OpenAIAuth>=3.0.0
-Requires-Dist: rich
 Requires-Dist: tiktoken>=0.3.0
-Requires-Dist: openai
 
 # OpenAI Chat Python Lib
 
 ## Requirements
 ```
 python: >=3.9
 ```
```

