# Comparing `tmp/openaichatlib-1.0.6.tar.gz` & `tmp/openaichatlib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openaichatlib-1.0.6.tar", last modified: Sun Apr 28 00:58:13 2024, max compression
+gzip compressed data, was "openaichatlib-1.0.7.tar", last modified: Sun Apr 28 02:17:18 2024, max compression
```

## Comparing `openaichatlib-1.0.6.tar` & `openaichatlib-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 00:58:13.702372 openaichatlib-1.0.6/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.6/LICENSE
--rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 00:58:13.701737 openaichatlib-1.0.6/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.6/README.md
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 00:58:13.698096 openaichatlib-1.0.6/openaichatlib/
--rw-r--r--   0 chenshuai   (501) staff       (20)    18676 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/V3.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/__init__.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/typings.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/utils.py
--rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.0.6/openaichatlib/version.py
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 00:58:13.701080 openaichatlib-1.0.6/openaichatlib.egg-info/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       45 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/requires.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-04-28 00:58:13.000000 openaichatlib-1.0.6/openaichatlib.egg-info/top_level.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-04-28 00:58:13.702518 openaichatlib-1.0.6/setup.cfg
--rw-r--r--   0 chenshuai   (501) staff       (20)     1164 2024-04-28 00:56:45.000000 openaichatlib-1.0.6/setup.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 02:17:18.616042 openaichatlib-1.0.7/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.7/LICENSE
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 02:17:18.615527 openaichatlib-1.0.7/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.7/README.md
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 02:17:18.611616 openaichatlib-1.0.7/openaichatlib/
+-rw-r--r--   0 chenshuai   (501) staff       (20)    18683 2024-04-28 02:16:58.000000 openaichatlib-1.0.7/openaichatlib/V3.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.0.7/openaichatlib/__init__.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.0.7/openaichatlib/typings.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.0.7/openaichatlib/utils.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.0.7/openaichatlib/version.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 02:17:18.614953 openaichatlib-1.0.7/openaichatlib.egg-info/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 02:17:18.000000 openaichatlib-1.0.7/openaichatlib.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-04-28 02:17:18.000000 openaichatlib-1.0.7/openaichatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-04-28 02:17:18.000000 openaichatlib-1.0.7/openaichatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       45 2024-04-28 02:17:18.000000 openaichatlib-1.0.7/openaichatlib.egg-info/requires.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-04-28 02:17:18.000000 openaichatlib-1.0.7/openaichatlib.egg-info/top_level.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-04-28 02:17:18.616153 openaichatlib-1.0.7/setup.cfg
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1164 2024-04-28 02:17:14.000000 openaichatlib-1.0.7/setup.py
```

### Comparing `openaichatlib-1.0.6/LICENSE` & `openaichatlib-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.6/PKG-INFO` & `openaichatlib-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.6
+Version: 1.0.7
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `openaichatlib-1.0.6/README.md` & `openaichatlib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.6/openaichatlib/V3.py` & `openaichatlib-1.0.7/openaichatlib/V3.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,16 +88,14 @@
             engine: str = os.environ.get("GPT_ENGINE") or "gpt-3.5-turbo",
             proxy: str = None,
             timeout: float = None,
             max_tokens: int = None,
             customize_header: dict = None,
             temperature: float = 0.5,
             top_p: float = 1.0,
-            presence_penalty: float = 0.0,
-            frequency_penalty: float = 0.0,
             reply_count: int = 1,
             truncate_limit: int = None,
             system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
             count_tokens: bool = True,
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
@@ -136,16 +134,14 @@
             if engine in ENGINES_CLAUDE_MAX
             else 99_500
             if engine in ENGINES_CLAUDE_LOW
             else 3_500
         )
         self.temperature: float = temperature
         self.top_p: float = top_p
-        self.presence_penalty: float = presence_penalty
-        self.frequency_penalty: float = frequency_penalty
         self.reply_count: int = reply_count
         self.timeout: float = timeout
         self.proxy = proxy
         self.session = requests.Session()
         self.session.proxies.update(
             {
                 "http": proxy,
@@ -289,32 +285,32 @@
         payload = {
             "model": os.environ.get("MODEL_NAME") or model or self.engine,
             "messages": self.conversation[convo_id] if pass_history else [prompt],
             "stream": stream,
             # kwargs
             "temperature": kwargs.get("temperature", self.temperature),
             "top_p": kwargs.get("top_p", self.top_p),
-            "presence_penalty": kwargs.get(
-                "presence_penalty",
-                self.presence_penalty,
-            ),
-            "frequency_penalty": kwargs.get(
-                "frequency_penalty",
-                self.frequency_penalty,
-            ),
             "n": kwargs.get("n", self.reply_count),
-            "user": role,
         }
         max_tokens = kwargs.get("max_tokens", None) or self.get_max_tokens(convo_id=convo_id)
         if max_tokens:
             payload["max_tokens"] = max_tokens
         if json_format:
             payload["response_format"] = {
                 "type": "json_object"
             }
+        presence_penalty = kwargs.get("presence_penalty", None)
+        if presence_penalty:
+            payload["presence_penalty"] = presence_penalty
+        frequency_penalty = kwargs.get("frequency_penalty", None)
+        if frequency_penalty:
+            payload["frequency_penalty"] = frequency_penalty
+        user = kwargs.get("user", None)
+        if user:
+            payload["user"] = user
         if self.customize_header:
             headers.update(self.customize_header)
         response = self.session.post(
             url,
             headers=headers,
             json=payload,
             timeout=kwargs.get("timeout", self.timeout),
@@ -378,32 +374,32 @@
         payload = {
             "model": model or self.engine,
             "messages": self.conversation[convo_id] if pass_history else [prompt],
             "stream": True,
             # kwargs
             "temperature": kwargs.get("temperature", self.temperature),
             "top_p": kwargs.get("top_p", self.top_p),
-            "presence_penalty": kwargs.get(
-                "presence_penalty",
-                self.presence_penalty,
-            ),
-            "frequency_penalty": kwargs.get(
-                "frequency_penalty",
-                self.frequency_penalty,
-            ),
             "n": kwargs.get("n", self.reply_count),
-            "user": role,
         }
         max_tokens = kwargs.get("max_tokens", None) or self.get_max_tokens(convo_id=convo_id)
         if max_tokens:
             payload["max_tokens"] = max_tokens
         if json_format:
             payload["response_format"] = {
                 "type": "json_object"
             }
+        presence_penalty = kwargs.get("presence_penalty", None)
+        if presence_penalty:
+            payload["presence_penalty"] = presence_penalty
+        frequency_penalty = kwargs.get("frequency_penalty", None)
+        if frequency_penalty:
+            payload["frequency_penalty"] = frequency_penalty
+        user = kwargs.get("user", None)
+        if user:
+            payload["user"] = user
         headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
         if self.customize_header:
             headers.update(self.customize_header)
         # Get response
         async with self.aclient.stream(
                 "post",
                 self.api_url,
```

### Comparing `openaichatlib-1.0.6/openaichatlib/__init__.py` & `openaichatlib-1.0.7/openaichatlib/__init__.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.6/openaichatlib/typings.py` & `openaichatlib-1.0.7/openaichatlib/typings.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.6/openaichatlib/utils.py` & `openaichatlib-1.0.7/openaichatlib/utils.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.6/openaichatlib.egg-info/PKG-INFO` & `openaichatlib-1.0.7/openaichatlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.6
+Version: 1.0.7
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `openaichatlib-1.0.6/setup.py` & `openaichatlib-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "httpx[socks]",
     "requests[socks]",
     "tiktoken>=0.3.0",
 ]
 
 setup(
     name="openaichatlib",
-    version="1.0.6",
+    version="1.0.7",
     description="OpenAI Chat API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IAn2018cs/OpenAIChatLib",
     author="IAn2018",
     author_email="ian2018cs@gmail.com",
     classifiers=[
```

