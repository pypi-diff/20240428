# Comparing `tmp/lollms_client-0.3.1.tar.gz` & `tmp/lollms_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.3.1.tar", last modified: Sun Apr 21 01:54:41 2024, max compression
+gzip compressed data, was "lollms_client-0.4.0.tar", last modified: Sat Apr 27 17:27:55 2024, max compression
```

## Comparing `lollms_client-0.3.1.tar` & `lollms_client-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 01:54:41.305966 lollms_client-0.3.1/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-21 01:54:41.304968 lollms_client-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 01:54:41.284280 lollms_client-0.3.1/lollms_client/
--rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.3.1/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    13006 2024-04-21 01:25:56.000000 lollms_client-0.3.1/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     1457 2024-04-21 01:52:34.000000 lollms_client-0.3.1/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.3.1/lollms_client/lollms_types.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:54:41.304968 lollms_client-0.3.1/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-21 01:54:41.000000 lollms_client-0.3.1/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-21 01:54:41.000000 lollms_client-0.3.1/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 01:54:41.000000 lollms_client-0.3.1/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 01:54:41.000000 lollms_client-0.3.1/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 01:54:41.000000 lollms_client-0.3.1/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 01:54:41.305966 lollms_client-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-04-21 01:54:39.000000 lollms_client-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 17:27:55.785774 lollms_client-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-27 17:27:55.784773 lollms_client-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 17:27:55.761349 lollms_client-0.4.0/lollms_client/
+-rw-rw-rw-   0        0        0      341 2024-04-27 17:10:22.000000 lollms_client-0.4.0/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.4.0/lollms_client/lollms_config.py
+-rw-rw-rw-   0        0        0    19806 2024-04-27 17:27:12.000000 lollms_client-0.4.0/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.4.0/lollms_client/lollms_discussion.py
+-rw-rw-rw-   0        0        0    20548 2024-04-27 17:05:13.000000 lollms_client-0.4.0/lollms_client/lollms_personality.py
+-rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.4.0/lollms_client/lollms_personality_worker.py
+-rw-rw-rw-   0        0        0     1457 2024-04-21 01:52:34.000000 lollms_client-0.4.0/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.4.0/lollms_client/lollms_types.py
+-rw-rw-rw-   0        0        0     2087 2024-04-27 16:48:27.000000 lollms_client-0.4.0/lollms_client/lollms_utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-27 17:27:55.783774 lollms_client-0.4.0/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-27 17:27:55.000000 lollms_client-0.4.0/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-27 17:27:55.000000 lollms_client-0.4.0/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 17:27:55.000000 lollms_client-0.4.0/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-27 17:27:55.000000 lollms_client-0.4.0/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 17:27:55.000000 lollms_client-0.4.0/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 17:27:55.785774 lollms_client-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-04-27 17:27:42.000000 lollms_client-0.4.0/setup.py
```

### Comparing `lollms_client-0.3.1/LICENSE` & `lollms_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.3.1/PKG-INFO` & `lollms_client-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.3.1
+Version: 0.4.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.3.1/README.md` & `lollms_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.3.1/lollms_client/lollms_core.py` & `lollms_client-0.4.0/lollms_client/lollms_core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,105 @@
 import requests
 from ascii_colors import ASCIIColors
 from lollms_client.lollms_types import MSG_TYPE
 import json
+from enum import Enum
+import tiktoken
 
-elf_completion_formats={
-    "openai instruct":"/v1/completions",
-    "openai chat":"/v1/chat/completions",
-    "vllm instruct":"/v1/completions",
-    "vllm chat":"/v1/chat/completions",
-    "ollama chat":"/api/generate",
-    "litellm chat":"/chat/completions",
-    "lollms":"/generate"
-}
+class ELF_GENERATION_FORMAT(Enum):
+    LOLLMS = 0
+    OPENAI = 1
+    OLLAMA = 2
+    LITELLM = 2
+
+class ELF_COMPLETION_FORMAT(Enum):
+    Instruct = 0
+    Chat = 1
 
 class LollmsClient():
-    def __init__(self, host_address=None, model_name=None, personality=-1, n_predict=1024, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="") -> None:
+    def __init__(
+                    self, 
+                    host_address=None,
+                    model_name=None,
+                    ctx_size=4096,
+                    personality=-1, 
+                    n_predict=1024, 
+                    temperature=0.1, 
+                    top_k=50, 
+                    top_p=0.95, 
+                    repeat_penalty=0.8, 
+                    repeat_last_n=40, 
+                    seed=None, 
+                    n_threads=8, 
+                    service_key:str="",
+                    tokenizer=None,
+                    default_generation_mode=ELF_GENERATION_FORMAT.LOLLMS
+                ) -> None:
+        import tiktoken
+
         self.host_address=host_address
         self.model_name = model_name
+        self.ctx_size = ctx_size
         self.n_predict = n_predict
         self.personality = personality
         self.temperature = temperature
         self.top_k = top_k
         self.top_p = top_p
         self.repeat_penalty = repeat_penalty
         self.repeat_last_n = repeat_last_n
         self.seed = seed
         self.n_threads = n_threads
-
         self.service_key = service_key
+        self.default_generation_mode = default_generation_mode
+        self.tokenizer = tiktoken.model.encoding_for_model("gpt-3.5-turbo-1106") if tokenizer is None else tokenizer
+
+
+    def tokenize(self, prompt:str):
+        """
+        Tokenizes the given prompt using the model's tokenizer.
+
+        Args:
+            prompt (str): The input prompt to be tokenized.
+
+        Returns:
+            list: A list of tokens representing the tokenized prompt.
+        """
+        tokens_list = self.tokenizer.encode(prompt)
+
+        return tokens_list
+
+    def detokenize(self, tokens_list:list):
+        """
+        Detokenizes the given list of tokens using the model's tokenizer.
+
+        Args:
+            tokens_list (list): A list of tokens to be detokenized.
+
+        Returns:
+            str: The detokenized text as a string.
+        """
+        text = self.tokenizer.decode(tokens_list)
+
+        return text
+
+    def generate(self, prompt, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
+        if self.default_generation_mode == ELF_GENERATION_FORMAT.LOLLMS:
+            return self.lollms_generate(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, service_key, streaming_callback)
+        elif self.default_generation_mode == ELF_GENERATION_FORMAT.OPENAI:
+            return self.openai_generate(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
+        elif self.default_generation_mode == ELF_GENERATION_FORMAT.OLLAMA:
+            return self.ollama_generate(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
+        elif self.default_generation_mode == ELF_GENERATION_FORMAT.LITELLM:
+            return self.litellm_generate(prompt, self.host_address, self.model_name, -1, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, ELF_COMPLETION_FORMAT.Instruct, service_key, streaming_callback)
 
 
     def generate_text(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
+        self.lollms_generate(prompt, host_address, model_name, personality, n_predict, stream, temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads, service_key, streaming_callback)
+
+    def lollms_generate(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
         # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
         temperature = temperature if temperature is not None else self.temperature
@@ -45,15 +110,15 @@
         seed = seed or self.seed  # Use the instance seed if not provided
         n_threads = n_threads if n_threads else self.n_threads
 
 
         url = f"{host_address}/lollms_generate"
         if service_key!="":
             headers = {
-                'Content-Type': 'application/json; charset=utf-8',
+                'Content-Type': 'application/json;',
                 'Authorization': f'Bearer {service_key}',
             }
         else:
             headers = {
                 'Content-Type': 'application/json',
             }
         data = {
@@ -100,16 +165,15 @@
                         text = text[:-1]
                     return text
                 except Exception as ex:
                     return {"status": False, "error": str(ex)}
             else:
                 return {"status": False, "error": response.text}
 
-
-    def generate_completion(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format="vllm instruct", service_key:str="", streaming_callback=None):
+    def openai_generate(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format:ELF_COMPLETION_FORMAT=ELF_COMPLETION_FORMAT.Instruct, service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
         # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
         temperature = temperature if temperature is not None else self.temperature
@@ -127,142 +191,207 @@
                 'Authorization': f'Bearer {service_key}',
             }
         else:
             headers = {
                 'Content-Type': 'application/json',
             }
 
-        if completion_format=="openai instruct":
+        if completion_format==ELF_COMPLETION_FORMAT.Instruct:
             data = {
                 'model':model_name,#self.config.model_name,
                 'prompt': prompt,
                 "stream":True,
                 "temperature": float(temperature),
                 "max_tokens": n_predict
             }
-        elif completion_format=="openai chat":
-            data = {
-                'model':model_name,
-                'messages': [{
-                    'role': "user",
-                    'content': prompt
-                }],
-                "stream":True,
-                "temperature": float(temperature),
-                "max_tokens": n_predict
-            }
-        elif completion_format=="vllm instruct":
-            data = {
-                'model':model_name,
-                'prompt': prompt,
-                "stream":True,
-                "temperature": float(temperature),
-                "max_tokens": n_predict
-            }
-        elif completion_format=="vllm chat":
+            completion_format_path = "/v1/completions"
+        elif completion_format==ELF_COMPLETION_FORMAT.Chat:
             data = {
                 'model':model_name,
                 'messages': [{
                     'role': "user",
                     'content': prompt
                 }],
                 "stream":True,
                 "temperature": float(temperature),
                 "max_tokens": n_predict
             }
-        elif completion_format=="ollama chat":
-            data = {
-                'model':model_name,
-                'prompt': prompt,
-                "stream":True,
-                "temperature": float(temperature),
-                "max_tokens": n_predict
-            }
-        elif completion_format=="litellm chat":
-            data = {
-                'model':model_name,
-                'prompt': prompt,
-                "stream":True,
-                "temperature": float(temperature),
-                "max_tokens": n_predict
-            }
+            completion_format_path = "/v1/chat/completions"
+
 
         if host_address.endswith("/"):
             host_address = host_address[:-1]
-        url = f'{host_address}{elf_completion_formats[completion_format]}'
+        url = f'{host_address}{completion_format_path}'
 
 
         response = requests.post(url, json=data, headers=headers)
 
         if response.status_code==400:
-            if "openai" in completion_format:
+            try:
                 content = response.content.decode("utf8")
                 content = json.loads(content)
                 self.error(content["error"]["message"])
                 return
-            elif "vllm" in completion_format:
+            except:
                 content = response.content.decode("utf8")
                 content = json.loads(content)
                 self.error(content["message"])
                 return
         elif response.status_code==404:
             ASCIIColors.error(response.content.decode("utf-8", errors='ignore'))
         text = ""
         for line in response.iter_lines():
-            if completion_format=="litellm chat":
-                text +=chunk
-                if streaming_callback:
-                    if not streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK):
-                        break            
-            else:
-                decoded = line.decode("utf-8")
-                if completion_format=="ollama chat":
-                    json_data = json.loads(decoded)
-                    chunk = json_data["response"]
+            decoded = line.decode("utf-8")
+            if decoded.startswith("data: "):
+                try:
+                    json_data = json.loads(decoded[5:].strip())
+                    if completion_format==ELF_COMPLETION_FORMAT.Chat:
+                        try:
+                            chunk = json_data["choices"][0]["delta"]["content"]
+                        except:
+                            chunk = ""
+                    else:
+                        chunk = json_data["choices"][0]["text"]
                     ## Process the JSON data here
                     text +=chunk
                     if streaming_callback:
                         if not streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK):
-                            break            
+                            break
+                except:
+                    break
+            else:
+                if decoded.startswith("{"):
+                    for line_ in response.iter_lines():
+                        decoded += line_.decode("utf-8")
+                    try:
+                        json_data = json.loads(decoded)
+                        if json_data["object"]=="error":
+                            self.error(json_data["message"])
+                            break
+                    except:
+                        self.error("Couldn't generate text, verify your key or model name")
                 else:
-                    if decoded.startswith("data: "):
-                        try:
-                            json_data = json.loads(decoded[5:].strip())
-                            if "chat" in completion_format:
-                                try:
-                                    chunk = json_data["choices"][0]["delta"]["content"]
-                                except:
-                                    chunk = ""
-                            else:
-                                chunk = json_data["choices"][0]["text"]
-                            ## Process the JSON data here
-                            text +=chunk
-                            if streaming_callback:
-                                if not streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK):
-                                    break
-                        except:
+                    text +=decoded
+                    if streaming_callback:
+                        if not streaming_callback(decoded, MSG_TYPE.MSG_TYPE_CHUNK):
                             break
-                    else:
-                        if decoded.startswith("{"):
-                            for line_ in response.iter_lines():
-                                decoded += line_.decode("utf-8")
-                            try:
-                                json_data = json.loads(decoded)
-                                if json_data["object"]=="error":
-                                    self.error(json_data["message"])
-                                    break
-                            except:
-                                self.error("Couldn't generate text, verify your key or model name")
-                        else:
-                            text +=decoded
-                            if streaming_callback:
-                                if not streaming_callback(decoded, MSG_TYPE.MSG_TYPE_CHUNK):
-                                    break
             return text
 
+    def ollama_generate(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format:ELF_COMPLETION_FORMAT=ELF_COMPLETION_FORMAT.Instruct, service_key:str="", streaming_callback=None):
+        # Set default values to instance variables if optional arguments are None
+        host_address = host_address if host_address else self.host_address
+        model_name = model_name if model_name else self.model_name
+        n_predict = n_predict if n_predict else self.n_predict
+        personality = personality if personality is not None else self.personality
+        # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
+        temperature = temperature if temperature is not None else self.temperature
+        top_k = top_k if top_k is not None else self.top_k
+        top_p = top_p if top_p is not None else self.top_p
+        repeat_penalty = repeat_penalty if repeat_penalty is not None else self.repeat_penalty
+        repeat_last_n = repeat_last_n if repeat_last_n is not None else self.repeat_last_n
+        seed = seed or self.seed  # Use the instance seed if not provided
+        n_threads = n_threads if n_threads else self.n_threads
+
+        if service_key!="":
+            headers = {
+                'Content-Type': 'application/json',
+                'Authorization': f'Bearer {service_key}',
+            }
+        else:
+            headers = {
+                'Content-Type': 'application/json',
+            }
+
+        data = {
+            'model':model_name,
+            'prompt': prompt,
+            "stream":True,
+            "temperature": float(temperature),
+            "max_tokens": n_predict
+        }
+        completion_format_path = "/api/generate"
+        if host_address.endswith("/"):
+            host_address = host_address[:-1]
+        url = f'{host_address}{completion_format_path}'
+
+        response = requests.post(url, json=data, headers=headers)
+
+        if response.status_code==404:
+            ASCIIColors.error(response.content.decode("utf-8", errors='ignore'))
+        text = ""
+        for line in response.iter_lines():
+            decoded = line.decode("utf-8")
+            json_data = json.loads(decoded)
+            chunk = json_data["response"]
+            ## Process the JSON data here
+            text +=chunk
+            if streaming_callback:
+                if not streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK):
+                    break            
+            return text
+
+    def litellm_generate(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format:ELF_COMPLETION_FORMAT=ELF_COMPLETION_FORMAT.Instruct, service_key:str="", streaming_callback=None):
+        # Set default values to instance variables if optional arguments are None
+        host_address = host_address if host_address else self.host_address
+        model_name = model_name if model_name else self.model_name
+        n_predict = n_predict if n_predict else self.n_predict
+        personality = personality if personality is not None else self.personality
+        # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
+        temperature = temperature if temperature is not None else self.temperature
+        top_k = top_k if top_k is not None else self.top_k
+        top_p = top_p if top_p is not None else self.top_p
+        repeat_penalty = repeat_penalty if repeat_penalty is not None else self.repeat_penalty
+        repeat_last_n = repeat_last_n if repeat_last_n is not None else self.repeat_last_n
+        seed = seed or self.seed  # Use the instance seed if not provided
+        n_threads = n_threads if n_threads else self.n_threads
+
+        if service_key!="":
+            headers = {
+                'Content-Type': 'application/json',
+                'Authorization': f'Bearer {service_key}',
+            }
+        else:
+            headers = {
+                'Content-Type': 'application/json',
+            }
+
+        data = {
+            'model':model_name,
+            'prompt': prompt,
+            "stream":True,
+            "temperature": float(temperature),
+            "max_tokens": n_predict
+        }
+        completion_format_path = "/api/generate"
+        if host_address.endswith("/"):
+            host_address = host_address[:-1]
+        url = f'{host_address}{completion_format_path}'
+
+        response = requests.post(url, json=data, headers=headers)
+
+        if response.status_code==404:
+            ASCIIColors.error(response.content.decode("utf-8", errors='ignore'))
+        text = ""
+        for line in response.iter_lines():
+            decoded = line.decode("utf-8")
+            if decoded.startswith("{"):
+                json_data = json.loads(decoded)
+                if "error" in json_data:
+                    self.error(json_data["error"]["message"])
+                    break
+            else:
+                text +=decoded
+                if streaming_callback:
+                    if not streaming_callback(decoded, MSG_TYPE.MSG_TYPE_CHUNK):
+                            break
+       
+            return text
+
+####
+
     def listMountedPersonalities(self, host_address:str=None):
         host_address = host_address if host_address else self.host_address
         url = f"{host_address}/list_mounted_personalities"
 
         response = requests.get(url)
 
         if response.status_code == 200:
@@ -288,8 +417,8 @@
                 return {"status": False, "error": str(ex)}
         else:
             return {"status": False, "error": response.text}
 
 if __name__=="__main__":
     lc = LollmsClient("http://localhost:9600")
     print(lc.listMountedPersonalities())
-    print(lc.listMountedPersonalities())
+    print(lc.listModels())
```

### Comparing `lollms_client-0.3.1/lollms_client/lollms_tasks.py` & `lollms_client-0.4.0/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.3.1/lollms_client/lollms_types.py` & `lollms_client-0.4.0/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.3.1/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.4.0/lollms_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.3.1
+Version: 0.4.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.3.1/setup.py` & `lollms_client-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
     
 setuptools.setup(
     name="lollms_client",
-    version="0.3.1",
+    version="0.4.0",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

