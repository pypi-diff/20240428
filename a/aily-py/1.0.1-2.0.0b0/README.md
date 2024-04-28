# Comparing `tmp/aily-py-1.0.1.tar.gz` & `tmp/aily_py-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily-py-1.0.1.tar", last modified: Mon Apr  8 16:49:06 2024, max compression
+gzip compressed data, was "aily_py-2.0.0b0.tar", last modified: Thu Apr 25 01:04:57 2024, max compression
```

## Comparing `aily-py-1.0.1.tar` & `aily_py-2.0.0b0.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.632009 aily-py-1.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-28 02:48:35.000000 aily-py-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      372 2024-04-08 16:49:06.632009 aily-py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4029 2024-04-08 16:46:35.000000 aily-py-1.0.1/README.md
--rw-rw-rw-   0        0        0      487 2024-04-08 16:47:20.000000 aily-py-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      292 2024-04-08 16:49:06.632009 aily-py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      506 2024-04-08 16:47:11.000000 aily-py-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.603968 aily-py-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.616277 aily-py-1.0.1/src/aily/
--rw-rw-rw-   0        0        0       24 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/__init__.py
--rw-rw-rw-   0        0        0      201 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/__version__.py
--rw-rw-rw-   0        0        0     9181 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/aigc.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.618606 aily-py-1.0.1/src/aily/hardwares/
--rw-rw-rw-   0        0        0        0 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/hardwares/__init__.py
--rw-rw-rw-   0        0        0    15721 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/hardwares/audio130x.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.621341 aily-py-1.0.1/src/aily/llm/
--rw-rw-rw-   0        0        0       23 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/llm/__init__.py
--rw-rw-rw-   0        0        0     4028 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/llm/llm.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.625934 aily-py-1.0.1/src/aily/tools/
--rw-rw-rw-   0        0        0      152 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/tools/__init__.py
--rw-rw-rw-   0        0        0     1561 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/tools/speech_to_text.py
--rw-rw-rw-   0        0        0      826 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/tools/speex_decoder.py
--rw-rw-rw-   0        0        0      711 2024-04-08 16:46:35.000000 aily-py-1.0.1/src/aily/tools/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:49:06.632009 aily-py-1.0.1/src/aily_py.egg-info/
--rw-rw-rw-   0        0        0      372 2024-04-08 16:49:06.000000 aily-py-1.0.1/src/aily_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-08 16:49:06.000000 aily-py-1.0.1/src/aily_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:49:06.000000 aily-py-1.0.1/src/aily_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-04-08 16:49:06.000000 aily-py-1.0.1/src/aily_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 16:49:06.000000 aily-py-1.0.1/src/aily_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.696834 aily_py-2.0.0b0/
+-rw-rw-rw-   0        0        0     1091 2024-03-28 02:48:35.000000 aily_py-2.0.0b0/LICENSE
+-rw-rw-rw-   0        0        0      407 2024-04-25 01:04:57.695839 aily_py-2.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2024-04-08 16:52:34.000000 aily_py-2.0.0b0/README.md
+-rw-rw-rw-   0        0        0      519 2024-04-18 12:02:14.000000 aily_py-2.0.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0      318 2024-04-25 01:04:57.697851 aily_py-2.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0      542 2024-04-18 12:02:14.000000 aily_py-2.0.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.650507 aily_py-2.0.0b0/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.664615 aily_py-2.0.0b0/src/aily/
+-rw-rw-rw-   0        0        0       24 2024-04-08 16:46:35.000000 aily_py-2.0.0b0/src/aily/__init__.py
+-rw-rw-rw-   0        0        0      201 2024-04-08 16:46:35.000000 aily_py-2.0.0b0/src/aily/__version__.py
+-rw-rw-rw-   0        0        0     9958 2024-04-25 00:59:22.000000 aily_py-2.0.0b0/src/aily/aigc.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.668936 aily_py-2.0.0b0/src/aily/db/
+-rw-rw-rw-   0        0        0       25 2024-04-25 00:52:47.000000 aily_py-2.0.0b0/src/aily/db/__init__.py
+-rw-rw-rw-   0        0        0     1948 2024-04-25 00:36:49.000000 aily_py-2.0.0b0/src/aily/db/crud.py
+-rw-rw-rw-   0        0        0      801 2024-04-25 01:02:58.000000 aily_py-2.0.0b0/src/aily/db/main.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.672055 aily_py-2.0.0b0/src/aily/hardwares/
+-rw-rw-rw-   0        0        0        0 2024-04-08 16:46:35.000000 aily_py-2.0.0b0/src/aily/hardwares/__init__.py
+-rw-rw-rw-   0        0        0    16516 2024-04-23 08:02:55.000000 aily_py-2.0.0b0/src/aily/hardwares/audio130x.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.674100 aily_py-2.0.0b0/src/aily/llm/
+-rw-rw-rw-   0        0        0       23 2024-04-08 16:46:35.000000 aily_py-2.0.0b0/src/aily/llm/__init__.py
+-rw-rw-rw-   0        0        0     4922 2024-04-25 01:04:38.000000 aily_py-2.0.0b0/src/aily/llm/llm.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.681182 aily_py-2.0.0b0/src/aily/tools/
+-rw-rw-rw-   0        0        0      130 2024-04-18 12:02:14.000000 aily_py-2.0.0b0/src/aily/tools/__init__.py
+-rw-rw-rw-   0        0        0     4006 2024-04-25 00:31:41.000000 aily_py-2.0.0b0/src/aily/tools/speech_to_text.py
+-rw-rw-rw-   0        0        0      826 2024-04-08 16:46:35.000000 aily_py-2.0.0b0/src/aily/tools/speex_decoder.py
+-rw-rw-rw-   0        0        0     1939 2024-04-18 12:02:14.000000 aily_py-2.0.0b0/src/aily/tools/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.694840 aily_py-2.0.0b0/src/aily_py.egg-info/
+-rw-rw-rw-   0        0        0      407 2024-04-25 01:04:57.000000 aily_py-2.0.0b0/src/aily_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-25 01:04:57.000000 aily_py-2.0.0b0/src/aily_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 01:04:57.000000 aily_py-2.0.0b0/src/aily_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2024-04-25 01:04:57.000000 aily_py-2.0.0b0/src/aily_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 01:04:57.000000 aily_py-2.0.0b0/src/aily_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 01:04:57.692541 aily_py-2.0.0b0/tests/
+-rw-rw-rw-   0        0        0      438 2024-04-18 12:02:14.000000 aily_py-2.0.0b0/tests/test_speech_to_text.py
+-rw-rw-rw-   0        0        0      379 2024-04-18 12:02:14.000000 aily_py-2.0.0b0/tests/test_text_to_speech.py
```

### Comparing `aily-py-1.0.1/LICENSE` & `aily_py-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `aily-py-1.0.1/README.md` & `aily_py-2.0.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # aily-py
 
 ## 安装
 
 ```
-pip install aily
+pip install aily-py
 ```
 
 ## 快速开始
 
 ```python
 import os
 from aily import AIGC
```

### Comparing `aily-py-1.0.1/src/aily/aigc.py` & `aily_py-2.0.0b0/src/aily/aigc.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,60 +2,73 @@
 import asyncio
 import sys
 import random
 import threading
 import time
 from reactivex.subject import Subject
 from loguru import logger
-from queue import SimpleQueue
+from queue import Queue
+from dotenv import load_dotenv
 from .hardwares.audio130x import AudioModule
+from .db import Cache
 from .llm import LLMs
 from .tools import text_to_speech
+import threading
 
 
 class AIGC:
     # 事件
     wakeup = Subject()
     on_record_begin = Subject()
     on_record_end = Subject()
     on_play_begin = Subject()
     on_play_end = Subject()
     on_recognition = Subject()
     on_direction = Subject()
     on_invoke_start = Subject()
     on_invoke_end = Subject()
 
-    audio_playlist_queue = SimpleQueue()
-    llm_invoke_queue = SimpleQueue()
-    event_queue = SimpleQueue()
-
-    def __init__(self, port=None, baudrate: int = 1000000):
-        self.port = port
-        self.baudrate = baudrate
+    audio_playlist_queue = Queue()
+    llm_invoke_queue = Queue()
+    event_queue = Queue()
+    cache_queue = Queue()
+
+    @staticmethod
+    def load_config(env_file: str):
+        if not load_dotenv(dotenv_path=env_file, override=True):
+            raise RuntimeError("Failed to load the configuration file")
+        logger.info("Configuration file loaded successfully")
+        logger.info("model: {0}".format(os.getenv("LLM_MODEL")))
+
+    def __init__(self, env_file: str):
+        self.load_config(env_file)
+
+        self.port = os.getenv("PORT")
+        self.baudrate = os.getenv("BAUDRATE")
 
         self.hardware = None
-        self.conversation_mode = "multi"
+        self.conversation_mode = os.getenv("CONVERSATION_MODE")
 
         self.audio_upload_cancel = False
 
         self.custom_llm_invoke = None
         self.llm = None
         self.llm_key = os.getenv("LLM_KEY")
-        self.llm_model_name = os.getenv("LLM_MODEL_NAME", "gpt-3.5-turbo")
+        self.llm_model_name = os.getenv("LLM_MODEL", "gpt-3.5-turbo")
         self.llm_server = os.getenv("LLM_URL")
-        self.llm_temperature = os.getenv("LLM_TEMPERATURE", 0.5)
+        self.llm_temperature = float(os.getenv("LLM_TEMPERATURE", 0.5))
         self.llm_pre_prompt = os.getenv("LLM_PRE_PROMPT")
-        self.llm_max_token_length = os.getenv("LLM_MAX_TOKEN_LENGTH", 16384)
+        self.llm_max_token_length = int(os.getenv("LLM_MAX_TOKEN_LENGTH", 16384))
 
         self.wait_words_list = []
         self.wait_words_voice_list = []
         self.wait_words_init = True
         self.wait_words_voice_auto_play = True
         self.wait_words_data = bytearray()
-        self.wait_words_voice_loop_play = False
+        self.wait_words_voice_loop_play = os.getenv("WAIT_WORDS_LOOP_PLAY", False)
 
         self.invalid_words = os.getenv("INVALID_WORDS")
         self.invalid_voice = None
 
         # 获取系统类型
         if sys.platform == "win32":
             self.root_path = "D://temp"
@@ -65,14 +78,20 @@
         self.wait_words_voice_path = self.root_path + "/wait_words_voice"
 
         # 最后对话时间
         self.last_conversation_time = 0
         # 聊天记录有效时间
         self.conversation_expired_at = 5 * 60
 
+        # 数据库初始化
+        if os.environ.get("DB_NAME"):
+            os.environ["DB_NAME"] = os.path.abspath(os.environ.get("DB_NAME"))
+        else:
+            os.environ["DB_NAME"] = os.path.abspath("aigc.db")
+
     def set_hardware(self, module):
         self.hardware = module
 
     def set_root_path(self, path):
         self.root_path = path
 
     def set_custom_llm_invoke(self, custom_invoke: callable):
@@ -109,19 +128,22 @@
         self.hardware.set_conversation_mode(self.conversation_mode)
         self.hardware.init()
 
     def _llm_init(self):
         self.llm = LLMs(self)
         if self.custom_llm_invoke:
             self.llm.set_custom_invoke(self.custom_llm_invoke)
+    
+    def _cache_init(self):
+        self.cache = Cache(self)
 
     def _init(self):
         # 初始化等待词
         if self.wait_words_list:
-            logger.info("初始化等待词...")
+            logger.info("Initializing wait words...")
 
             for words in self.wait_words_list:
                 # 判断是纯文本还是语音文件地址
                 if os.path.exists(words):
                     # self.wait_words_voice_list.append(words)
                     with open(words, "rb") as f:
                         data = f.read()
@@ -132,82 +154,54 @@
                     self.wait_words_voice_list.append(speech_data)
                     # filename = str(int(time.time() * 1000)) + ".mp3"
                     # save_path = self.wait_words_voice_path + "/" + filename
                     # with open(save_path, "wb") as f:
                     #     f.write(speech_data)
                     # self.wait_words_voice_list.append(save_path)
 
-            logger.info("初始化等待词完成")
+            logger.info("Wait words initialization completed")
 
         # 读取默认
         if self.invalid_words:
             if os.path.exists(self.invalid_words):
                 with open(self.invalid_words, "rb") as f:
                     self.invalid_voice = f.read()
             else:
                 voice = text_to_speech(self.invalid_words)
                 self.invalid_voice = voice
 
     def init(self):
         self._hardware_init()
         self._llm_init()
+        self._cache_init()
         self._init()
 
-    def msg_handler(self):
-        while True:
-            if self.event_queue.empty():
-                time.sleep(0.0001)
-                continue
-
-            event = self.event_queue.get()
-            if event["type"] == "wakeup":
-                self.wakeup.on_next(event["data"])
-            elif event["type"] == "on_record_begin":
-                self.on_record_begin.on_next(event["data"])
-            elif event["type"] == "on_record_end":
-                # 播放等待音频
-                if self.wait_words_voice_auto_play:
-                    self._auto_play_wait_words()
-                self.on_record_end.on_next(event["data"])
-            elif event["type"] == "on_play_begin":
-                self.on_play_begin.on_next(event["data"])
-            elif event["type"] == "on_play_end":
-                self.on_play_end.on_next(event["data"])
-            elif event["type"] == "on_recognition":
-                self.on_recognition.on_next(event["data"])
-            elif event["type"] == "on_direction":
-                self.on_direction.on_next(event["data"])
-            elif event["type"] == "on_invoke_start":
-                self.on_invoke_start.on_next(event["data"])
-            elif event["type"] == "on_invoke_end":
-                self.on_invoke_end.on_next(event["data"])
-            else:
-                pass
-
     def set_conversation_mode(self, mode):
         self.conversation_mode = mode
 
     def play_wait_words(self, data):
         self.audio_playlist_queue.put({"type": "play_wait_words", "data": data})
 
     def play_invalid_words(self):
         if self.invalid_voice:
-            self.audio_playlist_queue.put({"type": "play_mp3", "data": self.invalid_voice})
+            self.audio_playlist_queue.put(
+                {"type": "play_mp3", "data": self.invalid_voice}
+            )
         else:
-            logger.warning("未设置无效词")
+            logger.warning("Invalid words not set")
 
     def _auto_play_wait_words(self):
         if self.wait_words_voice_list:
             words_index = random.randint(0, len(self.wait_words_voice_list) - 1)
             self.play_wait_words(self.wait_words_voice_list[words_index])
             # with open(self.wait_words_voice_list[words_index], "rb") as f:
             #     data = f.read()
             # self.play_wait_words(data)
         else:
-            logger.warning("未设置等待词")
+            logger.warning("Wait words not set")
 
     def send_message(self, content):
         if not content:
             self.play_invalid_words()
         else:
             # 聊天记录过期清理
             if time.time() - self.last_conversation_time > 60 * 60 * 24:
@@ -239,25 +233,52 @@
         if self.llm:
             self.llm.set_pre_prompt(pre_prompt)
         self.llm_pre_prompt = pre_prompt
 
     def play(self, data):
         self.audio_playlist_queue.put({"type": "play_tts", "data": data})
 
+    def run_msg_handler(self):
+        logger.success("AIGC service started")
+        for event in iter(self.event_queue.get, None):
+            if event["type"] == "wakeup":
+                self.wakeup.on_next(event["data"])
+            elif event["type"] == "on_record_begin":
+                self.on_record_begin.on_next(event["data"])
+            elif event["type"] == "on_record_end":
+                # 播放等待音频
+                if self.wait_words_voice_auto_play:
+                    self._auto_play_wait_words()
+                self.on_record_end.on_next(event["data"])
+            elif event["type"] == "on_play_begin":
+                self.on_play_begin.on_next(event["data"])
+            elif event["type"] == "on_play_end":
+                self.on_play_end.on_next(event["data"])
+            elif event["type"] == "on_recognition":
+                self.on_recognition.on_next(event["data"])
+            elif event["type"] == "on_direction":
+                self.on_direction.on_next(event["data"])
+            elif event["type"] == "on_invoke_start":
+                self.on_invoke_start.on_next(event["data"])
+            elif event["type"] == "on_invoke_end":
+                self.on_invoke_end.on_next(event["data"])
+            else:
+                pass
+
     async def main(self):
         self.init()
         tasks = [
-            threading.Thread(target=self.msg_handler, daemon=True),
-            threading.Thread(target=self.llm.run, daemon=True),
+            threading.Thread(target=self.run_msg_handler, daemon=True),
+            self.hardware,
+            self.llm,
+            self.cache
         ]
-        self.hardware.start()
         for task in tasks:
             task.start()
 
-        self.hardware.join()
         for task in tasks:
             task.join()
 
     def run(self):
         loop = asyncio.get_event_loop()
         try:
             loop.run_until_complete(self.main())
```

### Comparing `aily-py-1.0.1/src/aily/hardwares/audio130x.py` & `aily_py-2.0.0b0/src/aily/hardwares/audio130x.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import struct
 import asyncio
 import threading
 import time
+import os
 
 import serial
 
 from reactivex.subject import Subject
 from loguru import logger
 from ..tools.speex_decoder import speex_decoder
 
@@ -20,17 +21,17 @@
 
 
 class FillCode:
     DEF_FILL = 0x12345678
     INVAILD_SPEAK = 0x12345666
     TTS_FILL = 0x12345677
     MP3_FILL = 0x12345688
-    M4A_FILL = 0x123456aa
-    REPEAT_FILL = 0x123456ab
-    WAV_FILL = 0x123456bb
+    M4A_FILL = 0x123456AA
+    REPEAT_FILL = 0x123456AB
+    WAV_FILL = 0x123456BB
     NO_WAKE_FILL = 0x0
 
 
 class TypeCode:
     DEVICE_SLEEP = 0x0000
     LOCAL_ASR_NOTIFY = 0x0101
     WAKE_UP = 0x0102
@@ -44,20 +45,20 @@
     NET_PLAY_RESUME = 0x0203
     NET_PLAY_STOP = 0x0204
     NET_PLAY_RESTART = 0x0205
     NET_PLAY_NEXT = 0x0206
     NET_PLAY_LOCAL_TTS = 0x0207
     NET_PLAY_END = 0x0208
     NET_PLAY_RECONECT_URL = 0x0209
-    PLAY_DATA_GET = 0x020a
-    PLAY_DATA_RECV = 0x020b
-    PLAY_DATA_END = 0x020c
-    PLAY_TTS_END = 0x020d
-    PLAY_EMPTY = 0x020e
-    PLAY_NEXT = 0x020f
+    PLAY_DATA_GET = 0x020A
+    PLAY_DATA_RECV = 0x020B
+    PLAY_DATA_END = 0x020C
+    PLAY_TTS_END = 0x020D
+    PLAY_EMPTY = 0x020E
+    PLAY_NEXT = 0x020F
     PLAYING_TTS = 0x0210
     PLAY_RESUME_ERRO = 0x0211
     PLAY_LAST = 0x0212
     QCLOUD_IOT_CMD = 0x0301
     NET_VOLUME = 0x0302
     LOCAL_VOLUME = 0x0303
     VOLUME_INC = 0x0304
@@ -69,28 +70,28 @@
     EXIT_NET_CONFIG = 0x0403
     INIT_SMARTCONFIG = 0x0404
     WIFI_DISCONNECTED = 0x0405
     WIFI_CONNECTED = 0x0406
     GET_PROFILE = 0x0407
     NEED_PROFILE = 0x0408
     CLOUD_CONNECTED = 0x0409
-    CLOUD_DISCONNECTED = 0x040a
-    NET_CONFIG_SUCCESS = 0x040b
-    NET_CONFIG_FAIL = 0x040c
+    CLOUD_DISCONNECTED = 0x040A
+    NET_CONFIG_SUCCESS = 0x040B
+    NET_CONFIG_FAIL = 0x040C
     CIAS_OTA_START = 0x0501
     CIAS_OTA_DATA = 0x0502
     CIAS_OTA_SUCESS = 0x0503
     CIAS_FACTORY_START = 0x0504
     CIAS_FACTORY_OK = 0x0505
     CIAS_FACTORY_FAIL = 0x0506
     CIAS_FACTORY_SELF_TEST_START = 0x0507
     CIAS_IR_DATA = 0x0508
     CIAS_IR_LOADING_DATA = 0x0509
-    CIAS_IR_LOAD_DATA_OVER = 0x050a
-    CIAS_IR_LOAD_DATA_START = 0x050b
+    CIAS_IR_LOAD_DATA_OVER = 0x050A
+    CIAS_IR_LOAD_DATA_START = 0x050B
     CIAS_CJSON_DATA = 0x0601
     CIAS_SIGNLE_WAKEUP = 0x0701
     CIAS_PHYSICAL_WAKEUP = 0x0702
     CIAS_CONTINUOUS_WAKEUP = 0x0703
 
 
 class MediaState:
@@ -109,169 +110,231 @@
 
 
 class AudioModule(threading.Thread):
     event = Subject()
 
     def __init__(self, device):
         super(AudioModule, self).__init__()
+
+        self.daemon = True
+
         self.device = device
         self.port = device.port
         self.baud = device.baudrate
         self.serial = None
         self.running = True
 
         self.audio_event_queue = device.event_queue
 
         self.state = TypeCode.DEVICE_SLEEP
         # self.prev_state = TypeCode.DEVICE_SLEEP
         self.media_state = TypeCode.DEVICE_SLEEP
         self.conversation_mode = TypeCode.CIAS_SIGNLE_WAKEUP
 
-        self.format_string = 'IHHHHI'
+        self.format_string = "IHHHHI"
         self.read_length = STANDARD_HEAD_LEN
         self.pcm_data = bytearray()
         self.decode_data = bytes()
         self.media_data = bytes()
         self.media_read_start = 0
         self.media_read_end = MEDIA_READ_LENGTH
         self.media_count = 0
         self.process_media_data = bytes()
 
-        self.cmd_action = {TypeCode.WAKE_UP: self.wakeup,
-                           TypeCode.LOCAL_ASR_NOTIFY: self.local,
-                           TypeCode.PCM_MIDDLE: self.record,
-                           TypeCode.PCM_FINISH: self.upload,
-                           TypeCode.PLAY_DATA_GET: self.media,
-                           TypeCode.PLAY_DATA_RECV: self.media,
-                           TypeCode.NET_PLAY_END: self.media_end}
+        self.cmd_action = {
+            TypeCode.WAKE_UP: self.wakeup,
+            TypeCode.LOCAL_ASR_NOTIFY: self.local,
+            TypeCode.PCM_MIDDLE: self.record,
+            TypeCode.PCM_FINISH: self.upload,
+            TypeCode.PLAY_DATA_GET: self.media,
+            TypeCode.PLAY_DATA_RECV: self.media,
+            TypeCode.NET_PLAY_END: self.media_end,
+        }
 
         self.lasted_event = ""
 
-        start_data = 'A5 A5 5A 5A 00 00 01 02 00 00 00 00 77 56 34 12'
-        head_data = 'A5 A5 5A 5A 00 00 0A 02 00 00 00 00 77 56 34 12'
-        end_data = 'A5 A5 5A 5A 00 00 0C 02 00 00 00 00 77 56 34 12'
-        stop_data = 'A5 A5 5A 5A 00 00 0D 02 00 00 00 00 77 56 34 12'
+        start_data = "A5 A5 5A 5A 00 00 01 02 00 00 00 00 77 56 34 12"
+        head_data = "A5 A5 5A 5A 00 00 0A 02 00 00 00 00 77 56 34 12"
+        end_data = "A5 A5 5A 5A 00 00 0C 02 00 00 00 00 77 56 34 12"
+        stop_data = "A5 A5 5A 5A 00 00 0D 02 00 00 00 00 77 56 34 12"
         hex_values = start_data.split()
-        self.start_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_START, 0, 0,
-                                                       FillCode.MP3_FILL)
-        self.head_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_GET, 0, 0,
-                                                      FillCode.MP3_FILL)
-        self.end_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_END, 0, 0,
-                                                     FillCode.MP3_FILL)
-        self.stop_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_STOP, 0, 0,
-                                                      FillCode.MP3_FILL)
+        self.start_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_START, 0, 0, FillCode.MP3_FILL
+        )
+        self.head_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_GET, 0, 0, FillCode.MP3_FILL
+        )
+        self.end_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_END, 0, 0, FillCode.MP3_FILL
+        )
+        self.stop_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_STOP, 0, 0, FillCode.MP3_FILL
+        )
         # self.single_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.CIAS_SIGNLE_WAKEUP, 0, 0,
         #                                                 FillCode.DEF_FILL)
 
         self.file_code = FillCode.MP3_FILL
 
         # 订阅aigc发出得事件
         # self.aigc_event.subscribe(lambda i: self.event_handler(i))
 
     def update_fill_code(self, fill_code):
-        self.start_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_START, 0, 0,
-                                                       fill_code)
-        self.head_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_GET, 0, 0,
-                                                      fill_code)
-        self.end_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_END, 0, 0,
-                                                     fill_code)
-        self.stop_byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_STOP, 0, 0,
-                                                      fill_code)
+        self.start_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_START, 0, 0, fill_code
+        )
+        self.head_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_GET, 0, 0, fill_code
+        )
+        self.end_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.PLAY_DATA_END, 0, 0, fill_code
+        )
+        self.stop_byte_data = self.protocol_head_pack(
+            MAGIC_DATA, CHECK_SUM, TypeCode.NET_PLAY_STOP, 0, 0, fill_code
+        )
         self.file_code = fill_code
 
-    def protocol_head_pack(self, magic, checksum, head_type, data_len, version, fill_data):
-        head_data = bytearray(struct.pack('<I', magic))
-        head_data += bytearray(struct.pack('<H', checksum))
-        head_data += bytearray(struct.pack('<H', head_type))
-        head_data += bytearray(struct.pack('<H', data_len))
-        head_data += bytearray(struct.pack('<H', version))
-        head_data += bytearray(struct.pack('<I', fill_data))
+    def protocol_head_pack(
+        self, magic, checksum, head_type, data_len, version, fill_data
+    ):
+        head_data = bytearray(struct.pack("<I", magic))
+        head_data += bytearray(struct.pack("<H", checksum))
+        head_data += bytearray(struct.pack("<H", head_type))
+        head_data += bytearray(struct.pack("<H", data_len))
+        head_data += bytearray(struct.pack("<H", version))
+        head_data += bytearray(struct.pack("<I", fill_data))
         return head_data
 
     def init(self):
-        # logger.debug(f'{self.port, self.baud}')
-        self.serial = serial.Serial(self.port, self.baud, timeout=2)
-
-    def run(self):
-        logger.info('serial run')
+        self.serial = serial.Serial(
+            self.port, self.baud, timeout=float(os.environ.get("SERIAL_TIMEOUT", 1))
+        )
 
         # 初始化对话模式
         if self.conversation_mode == TypeCode.CIAS_SIGNLE_WAKEUP:
-            byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.CIAS_SIGNLE_WAKEUP, 0, 0,
-                                                FillCode.DEF_FILL)
+            byte_data = self.protocol_head_pack(
+                MAGIC_DATA,
+                CHECK_SUM,
+                TypeCode.CIAS_SIGNLE_WAKEUP,
+                0,
+                0,
+                FillCode.DEF_FILL,
+            )
         elif self.conversation_mode == TypeCode.CIAS_CONTINUOUS_WAKEUP:
-            byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.CIAS_CONTINUOUS_WAKEUP, 0, 0,
-                                                FillCode.DEF_FILL)
+            byte_data = self.protocol_head_pack(
+                MAGIC_DATA,
+                CHECK_SUM,
+                TypeCode.CIAS_CONTINUOUS_WAKEUP,
+                0,
+                0,
+                FillCode.DEF_FILL,
+            )
         else:
-            byte_data = self.protocol_head_pack(MAGIC_DATA, CHECK_SUM, TypeCode.CIAS_PHYSICAL_WAKEUP, 0, 0,
-                                                FillCode.DEF_FILL)
+            byte_data = self.protocol_head_pack(
+                MAGIC_DATA,
+                CHECK_SUM,
+                TypeCode.CIAS_PHYSICAL_WAKEUP,
+                0,
+                0,
+                FillCode.DEF_FILL,
+            )
 
         self.write(byte_data)
 
-        while True:
-            if not self.device.audio_playlist_queue.empty():
-                event = self.device.audio_playlist_queue.get()
-                logger.info("Audio download event: {0}".format(event["type"]))
-                if event["type"] == "play_tts":
-                    # 发起播放开始事件
-                    self.update_fill_code(FillCode.TTS_FILL)
-                    logger.info("开始播放tts，先停止当前播放")
+    def run_msg_handler(self):
+        logger.success("Audio service started")
+        for event in iter(self.device.audio_playlist_queue.get, None):
+            logger.info("Audio download event: {0}".format(event["type"]))
+            if event["type"] == "play_tts":
+                # 发起播放开始事件
+                self.update_fill_code(FillCode.TTS_FILL)
+                logger.info("开始播放tts，先停止当前播放")
+                self.write(self.stop_byte_data)
+                # await asyncio.sleep(0.5)
+                logger.info("停止播放")
+                self.media_data = event["data"]
+                self.write(self.start_byte_data)
+                self.media_count = 0
+                self.media_read_start = 0
+                self.media_read_end = MEDIA_READ_LENGTH
+                self.media(event["data"])
+
+                self.audio_event_queue.put({"type": "on_play_begin", "data": ""})
+            elif event["type"] == "play_mp3":
+                if self.file_code != FillCode.MP3_FILL:
+                    pass
+                else:
+                    self.update_fill_code(FillCode.MP3_FILL)
                     self.write(self.stop_byte_data)
-                    # await asyncio.sleep(0.5)
-                    logger.info("停止播放")
+                    self.write(self.start_byte_data)
                     self.media_data = event["data"]
+                    self.media_count = 0
+                    self.media_read_start = 0
+                    self.media_read_end = MEDIA_READ_LENGTH
+                    self.media(event["data"])
+            elif event["type"] == "play_wait_words":
+                logger.info("Play wait words, file_code: {0}".format(self.file_code))
+                if self.file_code != FillCode.MP3_FILL:
+                    pass
+                else:
+                    self.update_fill_code(FillCode.MP3_FILL)
+                    self.write(self.stop_byte_data)
                     self.write(self.start_byte_data)
+                    self.media_data = event["data"]
                     self.media_count = 0
                     self.media_read_start = 0
                     self.media_read_end = MEDIA_READ_LENGTH
                     self.media(event["data"])
+                    logger.info("Play wait words end")
 
-                    self.audio_event_queue.put({"type": "on_play_begin", "data": ""})
-                elif event["type"] == "play_mp3":
-                    if self.file_code != FillCode.MP3_FILL:
-                        pass
-                    else:
-                        self.update_fill_code(FillCode.MP3_FILL)
-                        self.write(self.stop_byte_data)
-                        self.write(self.start_byte_data)
-                        self.media_data = event["data"]
-                        self.media_count = 0
-                        self.media_read_start = 0
-                        self.media_read_end = MEDIA_READ_LENGTH
-                        self.media(event["data"])
-                elif event["type"] == "play_wait_words":
-                    logger.info("Play wait words, file_code: {0}".format(self.file_code))
-                    if self.file_code != FillCode.MP3_FILL:
-                        pass
-                    else:
-                        self.update_fill_code(FillCode.MP3_FILL)
-                        self.write(self.stop_byte_data)
-                        self.write(self.start_byte_data)
-                        self.media_data = event["data"]
-                        self.media_count = 0
-                        self.media_read_start = 0
-                        self.media_read_end = MEDIA_READ_LENGTH
-                        self.media(event["data"])
-                        logger.info("Play wait words end")
-
-            if self.serial.in_waiting > 0:
+    def run_serial(self):
+        logger.info("Serial service started")
+        while True:
+            try:
                 data = self.serial.read(self.read_length)
                 if len(data) < self.read_length:
                     continue
 
                 self.data_parse(data)
                 func = self.cmd_action.get(self.state)
                 if func:
                     func(data)
                 else:
                     # logger.debug(f'>>>>>>>>>>>>>>>>>>>>>{self.state}')
                     hex_string = ' '.join(format(x, '02X') for x in data)
                     logger.debug(f'->{hex_string}')
+            except Exception as e:
+                logger.error("Serial run error: {0}".format(e))
+
+    def run(self):
+        tasks = [
+            threading.Thread(target=self.run_msg_handler),
+            threading.Thread(target=self.run_serial),
+        ]
+
+        for task in tasks:
+            task.start()
+
+        for task in tasks:
+            task.join()
+
+            # if self.serial.in_waiting > 0:
+            #     data = self.serial.read(self.read_length)
+            #     if len(data) < self.read_length:
+            #         continue
+
+            #     self.data_parse(data)
+            #     func = self.cmd_action.get(self.state)
+            #     if func:
+            #         func(data)
+            #     else:
+            #         # logger.debug(f'>>>>>>>>>>>>>>>>>>>>>{self.state}')
+            #         hex_string = ' '.join(format(x, '02X') for x in data)
+            #         logger.debug(f'->{hex_string}')
 
-            time.sleep(0.0001)
+            # time.sleep(0.0001)
 
         self.serial.close()
         # await asyncio.sleep(0)
 
     def data_parse(self, data):
         read_length = len(data)
         if read_length >= STANDARD_HEAD_LEN:
@@ -289,15 +352,15 @@
             if self.read_length < STANDARD_HEAD_LEN:
                 self.read_length = STANDARD_HEAD_LEN
 
     def upload(self, data):
         if not len(self.pcm_data):
             return
 
-        logger.info('Pcm data to upload.')
+        logger.info("Pcm data to upload.")
 
         # self.device.audio_upload_queue.put(self.pcm_data)
 
         # with open('greatest_16k_s16le.mp3', 'rb') as file:
         #     self.media_data = file.read()
         #
         # print('media mp3 get')
@@ -313,30 +376,30 @@
         # self.write(self.start_byte_data)
         # # self.media_state = MEDIA_MP3_CHECK
         # self.media_count = 0
         # self.media_read_start = 0
         # self.media_read_end = MEDIA_READ_LENGTH
 
     def send_media_data(self):
-        send_data = self.media_data[self.media_read_start: self.media_read_end]
+        send_data = self.media_data[self.media_read_start : self.media_read_end]
         if send_data:
             data_length = len(send_data)
-            packed_data = bytearray(struct.pack('<H', data_length))
-            self.head_byte_data[8: 10] = packed_data
+            packed_data = bytearray(struct.pack("<H", data_length))
+            self.head_byte_data[8:10] = packed_data
             send_data = self.head_byte_data + send_data
             self.write(send_data)
             self.media_count += 1
             self.media_read_start += MEDIA_READ_LENGTH
             self.media_read_end += MEDIA_READ_LENGTH
         else:
             self.write(self.end_byte_data)
             self.media_count = 0
             self.media_read_start = 0
             self.media_read_end = MEDIA_READ_LENGTH
-            logger.info('Media data send completed')
+            logger.info("Media data send completed")
 
             # 发起播放结束事件
             # self.event.on_next({"type": "on_play_end", "data": ""})
             # self.event_queue.put({"type": "on_play_end", "data": ""})
 
     def media(self, data):
         if self.media_count == 0:
@@ -358,18 +421,18 @@
     def wakeup(self, data):
         self.pcm_data = bytearray()
         self.audio_event_queue.put({"type": "wakeup", "data": data})
 
     def local(self, data):
         self.pcm_data = bytearray()
         self.device.audio_upload_cancel = True
-        logger.info(f'LOCAL ASR NOTIFY')
+        logger.info(f"LOCAL ASR NOTIFY")
         if len(data) == 2:
-            data_int = struct.unpack('<h', data)[0]
-            logger.info(f'LOCAL ASR NOTIFY: {data_int}')
+            data_int = struct.unpack("<h", data)[0]
+            logger.info(f"LOCAL ASR NOTIFY: {data_int}")
             # 发起离线指令识别事件
             # self.event.on_next({"type": "on_recognition", "data": data_int})
             self.audio_event_queue.put({"type": "on_recognition", "data": data_int})
 
     def record(self, data):
         # 发起录音开始事件
         # 判断当前录音事件是否已经发起
@@ -397,8 +460,8 @@
         if mode == "single":
             self.conversation_mode = TypeCode.CIAS_SIGNLE_WAKEUP
         elif mode == "manual":
             self.conversation_mode = TypeCode.CIAS_PHYSICAL_WAKEUP
         elif mode == "multi":
             self.conversation_mode = TypeCode.CIAS_CONTINUOUS_WAKEUP
         else:
-            raise Exception("Invalid conversation mode")
+            raise Exception("Unsupported conversation mode")
```

### Comparing `aily-py-1.0.1/src/aily/llm/llm.py` & `aily_py-2.0.0b0/src/aily/llm/llm.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 import time
 
 import tiktoken
 
 from reactivex.subject import Subject
 from openai import OpenAI
 from loguru import logger
+import threading
 
 
-class LLMs:
+class LLMs(threading.Thread):
     def __init__(self, device):
+        super(LLMs, self).__init__()
+        self.daemon = True
+
         self.device = device
         self.chat_records = []
 
         self.url = device.llm_server
         # self.url = "https://braintrustproxy.com/v1"
         self.api_key = device.llm_key
         self.model = device.llm_model_name
         self.temperature = float(device.llm_temperature)
         self.pre_prompt = device.llm_pre_prompt
         self.max_token_length = device.llm_max_token_length
         self.custom_invoke = None
 
         self.event_queue = device.event_queue
         self.handler_queue = device.llm_invoke_queue
+        self.cache_queue = device.cache_queue
 
     def set_custom_invoke(self, custom_invoke: callable):
         self.custom_invoke = custom_invoke
 
     @staticmethod
     def get_text_token_count(text):
         encoding = tiktoken.get_encoding("cl100k_base")
@@ -38,22 +43,21 @@
         if self.pre_prompt:
             current_token_length = self.get_text_token_count(self.pre_prompt)
         else:
             current_token_length = 0
 
         new_messages = []
         for message in reversed(messages):
-            new_message = {
-                "role": message["role"],
-                "content": message["content"]
-            }
+            new_message = {"role": message["role"], "content": message["content"]}
             current_token_length += self.get_text_token_count(message["content"])
             if "function_call" in message:
                 new_message["function_call"] = message["function_call"]
-                current_token_length += self.get_text_token_count(str(message["function_call"]))
+                current_token_length += self.get_text_token_count(
+                    str(message["function_call"])
+                )
             if current_token_length < self.max_token_length:
                 new_messages.insert(0, new_message)
             else:
                 break
 
         if self.pre_prompt:
             new_messages.insert(0, {"role": "system", "content": self.pre_prompt})
@@ -63,51 +67,74 @@
     @staticmethod
     def default_invoke(**kwargs):
         client = OpenAI(base_url=kwargs["url"], api_key=kwargs["api_key"])
         response = client.chat.completions.create(
             model=kwargs["model"],
             messages=kwargs["messages"],
             temperature=kwargs["temperature"],
-            stream=False
+            stream=False,
         )
 
         return {
             "role": response.choices[0].message.role,
             "content": response.choices[0].message.content,
-            "tool_calls": response.choices[0].message.tool_calls
+            "tool_calls": response.choices[0].message.tool_calls,
         }
 
     def invoke(self, url, api_key, model, temperature, messages):
         if self.custom_invoke:
-            return self.custom_invoke(url=url, api_key=api_key, model=model, temperature=temperature, messages=messages)
-        return self.default_invoke(url=url, api_key=api_key, model=model, temperature=temperature, messages=messages)
+            return self.custom_invoke(
+                url=url,
+                api_key=api_key,
+                model=model,
+                temperature=temperature,
+                messages=messages,
+            )
+        return self.default_invoke(
+            url=url,
+            api_key=api_key,
+            model=model,
+            temperature=temperature,
+            messages=messages,
+        )
 
     def send_message(self, content):
         # 开始调用事件发起
         self.event_queue.put({"type": "on_invoke_start", "data": ""})
         # 获取缓存聊天记录
+        current_msg = {"role": "user", "content": content}
+        self.cache_queue.put({"type": "conversations", "data": [time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), current_msg["role"], current_msg["content"]]})
+        
         messages = self.chat_records
-        messages.append({"role": "user", "content": content})
+        messages.append(current_msg)
         messages = self.build_prompt(messages)
-        response = self.invoke(self.url, self.api_key, self.model, self.temperature, messages)
-        self.chat_records.append({
-            "role": response["role"],
-            "content": response["content"],
-        })
+        response = self.invoke(
+            self.url, self.api_key, self.model, self.temperature, messages
+        )
+        self.chat_records.append(
+            {
+                "role": response["role"],
+                "content": response["content"],
+            }
+        )
 
         # TODO function call处理
         self.event_queue.put({"type": "on_invoke_end", "data": response["content"]})
+        self.cache_queue.put({"type": "conversations", "data": [time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), response["role"], response["content"]]})
+        
 
     def clear_chat_records(self):
         self.chat_records.clear()
 
+    def run_msg_handler(self):
+        logger.success("LLM service started")
+        for event in iter(self.handler_queue.get, None):
+            try:
+                if event["type"] == "invoke":
+                    self.send_message(event["data"])
+                else:
+                    pass
+            except Exception as e:
+                logger.error("LLM invoke error: {0}".format(e))
+
     def run(self):
-        while True:
-            if self.handler_queue.empty():
-                time.sleep(0.0001)
-                continue
-
-            event = self.handler_queue.get()
-            if event["type"] == "invoke":
-                self.send_message(event["data"])
-            else:
-                pass
+        self.run_msg_handler()
```

### Comparing `aily-py-1.0.1/src/aily/tools/speex_decoder.py` & `aily_py-2.0.0b0/src/aily/tools/speex_decoder.py`

 * *Files identical despite different names*

