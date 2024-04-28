# Comparing `tmp/omniunibot-0.3.0.tar.gz` & `tmp/omniunibot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniunibot-0.3.0.tar", max compression
+gzip compressed data, was "omniunibot-0.4.0.tar", max compression
```

## Comparing `omniunibot-0.3.0.tar` & `omniunibot-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1065 2024-03-15 02:47:20.599263 omniunibot-0.3.0/LICENSE
--rw-r--r--   0        0        0     2119 2024-03-26 07:52:30.531854 omniunibot-0.3.0/README.md
--rw-r--r--   0        0        0      149 2024-03-26 07:52:30.531854 omniunibot-0.3.0/omniunibot/__init__.py
--rw-r--r--   0        0        0     4139 2024-03-26 07:25:38.784043 omniunibot-0.3.0/omniunibot/client/client.py
--rw-r--r--   0        0        0       31 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/common/constants.py
--rw-r--r--   0        0        0     5142 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/common/data_type.py
--rw-r--r--   0        0        0        0 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/common/utils.py
--rw-r--r--   0        0        0      925 2024-03-26 07:25:29.392968 omniunibot-0.3.0/omniunibot/server/__main__.py
--rw-r--r--   0        0        0     5059 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/server/server.py
--rw-r--r--   0        0        0     1891 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/server/wrapper/base.py
--rw-r--r--   0        0        0     2374 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/server/wrapper/dingtalk.py
--rw-r--r--   0        0        0     2711 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/server/wrapper/lark.py
--rw-r--r--   0        0        0     2372 2024-03-15 02:47:20.603263 omniunibot-0.3.0/omniunibot/server/wrapper/slack.py
--rw-r--r--   0        0        0      671 2024-03-26 07:52:30.531854 omniunibot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 omniunibot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-15 02:47:20.599263 omniunibot-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2756 2024-04-28 11:39:31.058875 omniunibot-0.4.0/README.md
+-rw-r--r--   0        0        0      267 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/__init__.py
+-rw-r--r--   0        0        0     4195 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/client/client.py
+-rw-r--r--   0        0        0       31 2024-03-15 02:47:20.603263 omniunibot-0.4.0/omniunibot/common/constants.py
+-rw-r--r--   0        0        0     5113 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/common/data_type.py
+-rw-r--r--   0        0        0     4008 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/connector/base.py
+-rw-r--r--   0        0        0     2227 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/connector/dingtalk.py
+-rw-r--r--   0        0        0     2584 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/connector/lark.py
+-rw-r--r--   0        0        0     2290 2024-04-28 11:39:31.058875 omniunibot-0.4.0/omniunibot/connector/slack.py
+-rw-r--r--   0        0        0      555 2024-04-28 11:39:31.062875 omniunibot-0.4.0/omniunibot/server/__main__.py
+-rw-r--r--   0        0        0     5848 2024-04-28 11:39:31.062875 omniunibot-0.4.0/omniunibot/server/server.py
+-rw-r--r--   0        0        0      618 2024-04-28 11:39:31.062875 omniunibot-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 omniunibot-0.4.0/PKG-INFO
```

### Comparing `omniunibot-0.3.0/LICENSE` & `omniunibot-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omniunibot-0.3.0/README.md` & `omniunibot-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: omniunibot
+Version: 0.4.0
+Summary: A universal multiplatform message bot
+Home-page: https://github.com/yttty/omniunibot
+License: MIT
+Author: yttty
+Author-email: yttty@noreply.com
+Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9,<4.0)
+Requires-Dist: loguru (>=0.6,<0.8)
+Requires-Dist: pyzmq (>=26.0,<27.0)
+Requires-Dist: slack-sdk (>=3.21)
+Project-URL: Repository, https://github.com/yttty/omniunibot
+Description-Content-Type: text/markdown
+
 # omniunibot
 
 <!-- [![Upload Python Package](https://github.com/yttty/omniunibot/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yttty/omniunibot/actions/workflows/python-publish.yml) -->
 
 > ⚠️ **For `omniunibot>=0.3.0`, omniunibot will only support `Python>=3.12`.** Please use `omniunibot==0.2.0` for `Python<3.12`.
 
 ### 🤖 An omnipotent universal message bot library for python
@@ -15,25 +34,25 @@
   - Send to multiple platforms with one-line code
 
 ### 💻 Installation
 
 - *(via pip)* `pip install -U omniunibot`
 - *(via source)* clone this repo && `pip install .`
 
-### 📜 Usage
+### 📜 Client-Server Mode
 
 1. Prepare a config file
     - Default config path: `$HOME/configs/omniunibot.json`
     - Config example
 
         ```json
         {
             "server": {
                 "bind": "tcp://*:58655",
-                "interval": 0.5
+                "interval": 0.1
             },
             "client": {
                 "bind": "tcp://localhost:58655"
             },
             "log": {
                 "level": "DEBUG",
                 "dir": "/home/ubuntu/logs/omniunibot"
@@ -61,9 +80,35 @@
 
 2. Start the bot server
 
     ```sh
     python -m omniunibot.server
     ```
 
-3. Use the client-side code in your code
-    - Example: [./example/client_example.py](./example/client_example.py)
+3. Use the client-side code in your code (see examples in [./tests](./tests))
+
+### 📜 Standalone Mode
+
+```py
+bot = DingTalkBot(
+    "https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxxxxxxxxxxx",
+    "xxxxxxxxxxxxxx",
+    on_success="log",
+    on_failure="trace",
+)
+await bot.send({"text": "`test_dingtalkbot_1` Pass"})
+
+bot = LarkBot(
+    "https://open.feishu.cn/open-apis/bot/v2/hook/xxxxx-d879-xxxxx-8d7b-xxxxxxxxxx",
+    "xxxxxxxxxxxxxxx",
+    on_success="log",
+    on_failure="trace",
+)
+await bot.send({"text": "`test_larkbot_1` Pass"})
+
+bot = SlackBot(
+    "https://hooks.slack.com/services/xxxxxxxx/xxxxxxxx/xxxxxxxxxx",
+    on_success="log",
+    on_failure="trace",
+)
+await bot.send({"text": "`test_slackbot_1` Pass"})
+```
```

### Comparing `omniunibot-0.3.0/omniunibot/client/client.py` & `omniunibot-0.4.0/omniunibot/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import zmq
 import json
 from loguru import logger
 from zmq.asyncio import Context
 import time
 import operator
+from typing import Any, Dict
 from typing import Optional, Union
 
 from ..common.data_type import Msg, MsgType, OmniUniBotConfig
 from ..common.constants import OMNI_ZMQ_TOPIC
 
 
 class OmniUniBotClient:
@@ -54,73 +55,73 @@
             return channel_group in self._channel_groups.keys()
         else:
             return True
 
     def _fmt_msg(
         self,
         channel_group: str,
+        msg_content: Dict[str, Any],
         msg_type: Union[str, MsgType],
-        **msg_content,
     ) -> Optional[Msg]:
         """Validate and format message
 
         Args:
             channel_group (str): The channel to send message. If the channel name is not
                 configured, the message will be disposed.
             msg_type (str): Type of the message. Defaults to 'Text'.
             msg_content (kwargs): ...
         """
         if type(msg_type) is str:
-            msg_type = MsgType(msg_type)
+            msg_type = MsgType[msg_type]
         if self._check_channel_configured(channel_group):
             return Msg.from_dict(
                 {
                     "channel_group": channel_group,
-                    "msg_type": msg_type,
                     "msg_content": msg_content,
+                    "msg_type": msg_type.name,
                 }
             )
         else:
             logger.warning(f"Channel {channel_group} not configured.")
             return None
 
     def send(
         self,
         channel_group: str,
-        msg_type: Union[str, MsgType] = "Text",
-        **msg_content,
+        msg_content: Dict[str, Any],
+        msg_type: MsgType | str = "Auto",
     ):
         """Send message to OmniUniBotServer
 
         Args:
             channel_group (str): The channel to send message. If the channel name is not
                 configured, the message will be disposed.
+            msg_content (dict): ...
             msg_type (str): Type of the message. Defaults to 'Text'.
-            msg_content (kwargs): ...
         """
-        msg = self._fmt_msg(channel_group, msg_type, **msg_content)
+        msg = self._fmt_msg(channel_group, msg_content, msg_type)
         if msg is not None:
             info = json.dumps(msg.to_dict()).encode("utf-8")
             self._socket.send_multipart([OMNI_ZMQ_TOPIC, info])
             if not self._quiet:
                 logger.debug(f"Client sent msg {info}")
 
     async def send_async(
         self,
         channel_group: str,
-        msg_type: Union[str, MsgType] = "Text",
-        **msg_content,
+        msg_content: Dict[str, Any],
+        msg_type: MsgType | str = "Auto",
     ):
         """Async send message to OmniUniBotServer
 
         Args:
             channel_group (str): The channel to send message. If the channel name is not
                 configured, the message will be disposed.
+            msg_content (dict): ...
             msg_type (str): Type of the message. Defaults to 'Text'.
-            msg_content (kwargs): ...
         """
-        msg = self._fmt_msg(channel_group, msg_type, **msg_content)
+        msg = self._fmt_msg(channel_group, msg_content, msg_type)
         if msg is not None:
             info = json.dumps(msg.to_dict()).encode("utf-8")
             await self._socket.send_multipart([OMNI_ZMQ_TOPIC, info])
             if not self._quiet:
                 logger.debug(f"Client sent msg {info}")
```

### Comparing `omniunibot-0.3.0/omniunibot/common/data_type.py` & `omniunibot-0.4.0/omniunibot/common/data_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from enum import Enum, auto
-from abc import abstractmethod, abstractclassmethod, ABC
+from abc import abstractmethod, ABC
 from dataclasses import dataclass
 from typing import Optional, Dict
 from pathlib import Path
 
 
 class OmniUniBotPlatform(Enum):
-    Slack = "Slack"
-    Lark = "Lark"
-    DingTalk = "DingTalk"
-    WeChatWork = "WeChatWork"
+    Slack = auto()
+    Lark = auto()
+    DingTalk = auto()
 
 
 class DictCompatibleADT(ABC):
     @abstractmethod
     def to_dict(self):
         pass
 
-    @abstractclassmethod
+    @classmethod
+    @abstractmethod
     def from_dict(cls):
         pass
 
 
 @dataclass
 class OmniUniBotChannelConfig(DictCompatibleADT):
     platform: OmniUniBotPlatform
     webhook: str
     secret: Optional[str] = None
 
     def to_dict(self) -> dict:
         d = {
-            "platform": self.platform.value,
+            "platform": self.platform.name,
             "webhook": self.webhook,
         }
         if self.secret is not None:
             d["secret"] = self.secret
         return d
 
     @classmethod
     def from_dict(cls, d: dict):
         return cls(
-            OmniUniBotPlatform(d["platform"]),
+            OmniUniBotPlatform[d["platform"]],
             d["webhook"],
             d.get("secret", None),
         )
 
     def __eq__(self, __value: object) -> bool:
         if not isinstance(__value, OmniUniBotChannelConfig):
             raise TypeError(f"{type(__value)}")
@@ -163,31 +163,32 @@
                 self.log == __value.log,
                 self.channel_groups == __value.channel_groups,
             ]
         )
 
 
 class MsgType(Enum):
-    Text = "Text"
-    Image = "Image"
+    Text = auto()
+    Image = auto()
+    Auto = auto()
 
 
 @dataclass
 class Msg(DictCompatibleADT):
     channel_group: str
     msg_type: MsgType
     msg_content: dict
 
     def to_dict(self) -> dict:
         return {
             "channel_group": self.channel_group,
-            "msg_type": self.msg_type.value,
+            "msg_type": self.msg_type.name,
             "msg_content": self.msg_content,
         }
 
     @classmethod
     def from_dict(cls, d: dict):
         return cls(
             d["channel_group"],
-            MsgType(d["msg_type"]),
+            MsgType[d["msg_type"]],
             d["msg_content"],
         )
```

### Comparing `omniunibot-0.3.0/omniunibot/server/server.py` & `omniunibot-0.4.0/omniunibot/server/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 import os
 import zmq
 import json
 import asyncio
 from loguru import logger
 from zmq.asyncio import Context
 import traceback
-from typing import Union, Dict, Optional
-from concurrent.futures import ThreadPoolExecutor
-
-from .wrapper.dingtalk import DingTalkBot
-from .wrapper.lark import LarkBot
-from .wrapper.slack import SlackBot
-from .wrapper.base import BaseBot
+from typing import Dict, Any, Deque
+from pathlib import Path
+from collections import deque
+
+from ..connector.dingtalk import DingTalkBot
+from ..connector.lark import LarkBot
+from ..connector.slack import SlackBot
+from ..connector.base import BaseBot
 from ..common.data_type import OmniUniBotConfig, OmniUniBotPlatform, OmniUniBotChannelConfig, MsgType, Msg
 from ..common.constants import OMNI_ZMQ_TOPIC
 
 
 class OmniUniBotServer:
-    def __init__(self, config: OmniUniBotConfig) -> None:
+    def __init__(self, config: OmniUniBotConfig | str | Path | None) -> None:
         """Initialize OmniUniBot Server
 
         Args:
             config (dict): the config dict
 
         Raises:
             ValueError: Raised there is no such channel in config
         """
-        assert isinstance(config, OmniUniBotConfig), "Invalid config"
-        self._config = config
+
+        if config is None:
+            self._config = OmniUniBotConfig.from_dict(
+                json.load(open(Path.home() / "configs" / "omniunibot.json", "r"))
+            )
+        elif isinstance(config, str) or isinstance(config, Path):
+            self._config = OmniUniBotConfig.from_dict(json.load(open(config, "r")))
+        elif isinstance(config, OmniUniBotConfig):
+            self._config = config
+        else:
+            raise TypeError("Invalid config")
+
         self._init_logger()
+        logger.debug(f"Config: {self._config.to_dict()}")
         self._init_bots()
+        self._msg_queue:Deque[Msg] = deque()
 
         # Initialize ZMQ
         self._addr = self._config.server.bind
         self._ctx = Context()
         self._socket = self._ctx.socket(zmq.SUB)
         self._socket.setsockopt(zmq.SUBSCRIBE, "".encode("utf-8"))
 
-        # Initialize loop
-        self._loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(self._loop)
-
     def _init_logger(self):
         handlers_cfg = []
         assert self._config.log.level in ["TRACE", "DEBUG", "INFO", "SUCCESS", "WARNING", "ERROR", "CRITICAL"]
         log_file_handler_cfg = dict(
             sink=str(self._config.log.dir / ("omniunibot.server" + ".{time:YYYY-MM-DD}" + ".log")),
             level=self._config.log.level,
             rotation="00:00",
         )
         handlers_cfg.append(log_file_handler_cfg)
         logger.configure(handlers=handlers_cfg)
 
-    def _get_bot(self, channel_config: OmniUniBotChannelConfig) -> Optional[Union[LarkBot, DingTalkBot, SlackBot]]:
+    def _get_bot(self, channel_config: OmniUniBotChannelConfig) -> LarkBot | DingTalkBot | SlackBot | None:
         if channel_config.platform == OmniUniBotPlatform.Slack:
             return SlackBot(channel_config.webhook)
         elif channel_config.platform == OmniUniBotPlatform.DingTalk:
             return DingTalkBot(channel_config.webhook, channel_config.secret)
         elif channel_config.platform == OmniUniBotPlatform.Lark:
             return LarkBot(channel_config.webhook, channel_config.secret)
         else:
@@ -74,58 +83,65 @@
                 else:
                     logger.error(f"Fail to initialize {channel_config.to_dict()} in group {channel_group_name}")
             logger.info(
                 f"Initialized {len(self._bots[channel_group_name])} destinations in channel group {channel_group_name}"
             )
         logger.info(f"Total {len(self._bots)} channel groups ready.")
 
-    def _bulk_send(
+    async def _bulk_send(
         self,
         channel_group_name: str,
+        msg_content: Dict[str, Any],
         msg_type: MsgType,
-        msg_content: dict,
     ):
         """_summary_
 
         Args:
             channel_group_name (str): _description_
             msg_type (MsgType): _description_
         """
-        executors = []
-        with ThreadPoolExecutor(max_workers=len(self._bots[channel_group_name])) as executor:
-            for bot in self._bots[channel_group_name]:
-                executors.append(
-                    executor.submit(
-                        bot.send,
-                        msg_type=msg_type,
-                        msg_content=msg_content,
-                    )
-                )
+        for bot in self._bots[channel_group_name]:
+            asyncio.create_task(bot.send(msg_content=msg_content, msg_type=msg_type))
 
-    async def _start_server(self):
+    async def _pull_zmq(self):
         self._socket.bind(self._addr)
         logger.info(f"Server bind to {self._addr}")
         while True:
             try:
                 mtPart = await self._socket.recv_multipart()
                 if mtPart[0] == OMNI_ZMQ_TOPIC:
                     part: dict = json.loads(mtPart[1].decode("utf-8"))
                     msg = Msg.from_dict(part)
                     if msg.channel_group not in self._bots.keys():
-                        raise ValueError(f"No such channel {msg.channel_group}")
-                    self._bulk_send(
-                        channel_group_name=msg.channel_group,
-                        msg_type=msg.msg_type,
-                        msg_content=msg.msg_content,
+                        logger.warning(f"Ignore msg because of no such channel. Channel={msg.channel_group} Msg={msg.to_dict()}")
+                    else:
+                        self._msg_queue.append(msg)
+            except Exception as e:
+                logger.error(f"_pull_zmq encounter {str(e)}. Data={part}")
+                logger.debug(traceback.format_exc())
+
+    async def _send_msg(self):
+        while True:
+            try:
+                if len(self._msg_queue) > 0:
+                    msg = self._msg_queue.popleft()
+                    asyncio.create_task(
+                        self._bulk_send(
+                            channel_group_name=msg.channel_group,
+                            msg_content=msg.msg_content,
+                            msg_type=msg.msg_type,
+                        )
                     )
-            except KeyboardInterrupt:
-                logger.info("Bye")
-                exit(0)
             except Exception as e:
-                logger.error(f"Server encounter {str(e)}. Data={part}")
+                logger.error(f"_send_msg encounter {str(e)}.")
                 logger.debug(traceback.format_exc())
             finally:
                 await asyncio.sleep(self._config.server.interval)
 
-    def start(self):
-        asyncio.ensure_future(self._start_server(), loop=self._loop)
-        self._loop.run_forever()
+    async def start(self):
+        try:
+            async with asyncio.TaskGroup() as tg:
+                _ = tg.create_task(self._pull_zmq())
+                _ = tg.create_task(self._send_msg())
+        except (KeyboardInterrupt, asyncio.exceptions.CancelledError):
+            logger.info("Stop {}. Bye.", self.__class__.__name__)
+            exit(0)
```

### Comparing `omniunibot-0.3.0/omniunibot/server/wrapper/dingtalk.py` & `omniunibot-0.4.0/omniunibot/connector/lark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-"""
-Description : Bots for DingDing
-"""
-
+import base64
 import time
-import hmac
 import hashlib
-import base64
-import urllib.parse
-from typing import List, Optional
-import requests
-from typing import Optional, Union
+import hmac
 from pathlib import Path
-from loguru import logger
+import aiohttp
 
+from ..common.data_type import MsgType
 from .base import BaseBot
-from ...common.data_type import MsgType
 
 
-class DingTalkBot(BaseBot):
+class LarkBot(BaseBot):
     """
-    https://open.dingtalk.com/document/robots/custom-robot-access
+    https://open.feishu.cn/document/client-docs/bot-v3/add-custom-bot
     """
 
+    _platform = "Lark"
+
     def __init__(self, webhook: str, secret: str, **kwargs):
-        self.webhook = webhook
-        self.secret = secret
-        assert self.secret is not None
-
-    def _get_signed_url(self):
-        timestamp = str(round(time.time() * 1000))
-        secret_enc = self.secret.encode("utf-8")
-        string_to_sign = "{}\n{}".format(timestamp, self.secret)
-        string_to_sign_enc = string_to_sign.encode("utf-8")
-        hmac_code = hmac.new(secret_enc, string_to_sign_enc, digestmod=hashlib.sha256).digest()
-        sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
-        signed_url = self.webhook + "&timestamp=" + str(timestamp) + "&sign=" + sign
-        return signed_url
-
-    def _on_success_response(self) -> None:
-        logger.debug("Successully sent message to DingTalk.")
-
-    def _on_error_response(self, response) -> None:
-        logger.error(f"Code={response['errcode']}. ErrMsg={response['errmsg']}.")
-
-    def _on_response(self, resp: dict) -> None:
-        if resp["errcode"] == 0:
-            self._on_success_response()
+        """
+        Args:
+            webhook (str): webhook from feishu
+            secret (str): secret from feishu
+        """
+
+        super().__init__(**kwargs)
+        self._webhook = webhook
+        self._secret = secret
+        assert self._secret is not None
+
+    def _sign(self):
+        """concat timestamp and secret
+
+        Returns:
+            timestamp, sign: _description_
+        """
+        timestamp = str(round(time.time()))
+        string_to_sign = "{}\n{}".format(timestamp, self._secret)
+        hmac_code = hmac.new(string_to_sign.encode("utf-8"), digestmod=hashlib.sha256).digest()
+        # b64 encoding
+        sign = base64.b64encode(hmac_code).decode("utf-8")
+        return timestamp, sign
+
+    async def _on_response(self, msg_id: str, rsp: dict | None) -> None:
+        """_summary_
+
+        Args:
+            msg_id (str): _description_
+            rsp (dict): _description_
+        """
+        if rsp.get("code", None) != 0:
+            await self._on_error_response(msg_id, rsp)
         else:
-            self._on_error_response(resp)
+            await self._on_success_response(msg_id)
 
-    def _generate_payload(
-        self,
-        msg_type: MsgType,
-        text: Optional[str] = None,
-        atMobiles: Optional[List[str]] = None,
-        atAll: bool = False,
-    ):
+    def _generate_payload(self, msg_type: MsgType, text: str | None = None, title: str | None = None, **kwargs):
+        """Generate payload to send, using message type `post`, see the document for details
+
+        Args:
+            text (str): _description_
+            title (Optional[str], optional): _description_. Defaults to None.
+            at_uid (Optional[List[str]], optional): uids to at. Defaults to None.
+        """
+        timestamp, sign = self._sign()
+        post_zh_cn = {"content": [[{"tag": "text", "text": text}]]}
+        if title is not None:
+            post_zh_cn["title"] = title
         payload = {
-            "msgtype": "text",
-            "text": {"content": text},
-            "at": {"isAtAll": atAll},
+            "timestamp": timestamp,
+            "sign": sign,
+            "msg_type": "post",
+            "content": {"post": {"zh_cn": post_zh_cn}},
         }
-        if atMobiles is not None:
-            payload["at"]["atMobiles"] = atMobiles
         return payload
 
-    def _send_image(self, msg_id: str, img_path: Union[str, Path], **kwargs):
-        raise NotImplementedError
-
-    def _send_text(self, msg_id: str, text: str, **kwargs):
-        logger.debug(f"UUID={msg_id}. Receive text message: {text}")
-        resp = requests.post(self._get_signed_url(), json=self._generate_payload(msg_type=MsgType.Text, text=text))
-        self._on_response(resp.json())
+    async def _send_text(self, text: str, **kwargs) -> dict:
+        async with aiohttp.ClientSession() as session:
+            async with session.request(
+                "POST", url=self._webhook, json=self._generate_payload(msg_type=MsgType.Text, text=text, **kwargs)
+            ) as rsp:
+                return await rsp.json()
```

### Comparing `omniunibot-0.3.0/omniunibot/server/wrapper/slack.py` & `omniunibot-0.4.0/omniunibot/connector/slack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from loguru import logger
-from typing import Optional, Dict, Union
-from slack_sdk.webhook import WebhookClient, WebhookResponse
 from pathlib import Path
+from typing import Optional, Dict, Any
+from slack_sdk.webhook import WebhookResponse
+from slack_sdk.webhook.async_client import AsyncWebhookClient
 
+from ..common.data_type import MsgType
 from .base import BaseBot
-from ...common.data_type import MsgType
 
 
 class SlackBot(BaseBot):
     """
     https://slack.dev/python-slack-sdk/
     """
 
-    def __init__(self, webhook: str, **kwargs):
+    _platform = "Slack"
+
+    def __init__(self, webhook: str, slack_webhoot_client_kwargs: Dict[str, Any] = {"timeout": 5}, **kwargs):
         """
         Args:
             webhook (str): webhook from slack `Incoming Webhooks`
+            slack_webhoot_client_kwargs: to be passed to slack sdk
         """
 
-        self.webhook = webhook
-        self.slack_client = WebhookClient(self.webhook)
+        super().__init__(**kwargs)
+        self._webhook = webhook
+        self._slack_client = AsyncWebhookClient(self._webhook, **slack_webhoot_client_kwargs)
 
-    def _on_success_response(self) -> None:
-        logger.debug("Successully sent message to Slack.")
+    async def _on_response(self, msg_id: str, rsp: WebhookResponse) -> None:
+        """_summary_
 
-    def _on_error_response(self, response: WebhookResponse) -> None:
-        """
         Args:
-            response (WebhookResponse): https://slack.dev/python-slack-sdk/api-docs/slack_sdk/webhook/webhook_response.html
+            msg_id (str): _description_
+            rsp (WebhookResponse): https://slack.dev/python-slack-sdk/api-docs/slack_sdk/webhook/webhook_response.html
         """
-        logger.error(f"Code={response.status_code}. ErrMsg={response.body}.")
-
-    def _on_response(self, response: WebhookResponse) -> None:
-        if response.status_code != 200:
-            self._on_error_response(response)
+        if rsp.status_code != 200:
+            await self._on_error_response(msg_id, {"code": rsp.status_code, "err_msg": rsp.body})
         else:
-            self._on_success_response()
+            await self._on_success_response(msg_id)
 
     def _generate_payload(self, msg_type: MsgType, text: Optional[str], **kwargs) -> Dict:
         payload = {
             "channel": " ",
             "blocks": [
                 {
                     "type": "section",
@@ -61,14 +61,10 @@
                         }
                     ]
                 }
             ],
         }
         return payload
 
-    def _send_image(self, msg_id: str, img_path: Union[str, Path], **kwargs):
-        raise NotImplementedError
-
-    def _send_text(self, msg_id: str, text: str, **kwargs):
-        logger.debug(f"UUID={msg_id}. Receive text message: {text}")
-        resp: WebhookResponse = self.slack_client.send_dict(self._generate_payload(msg_type=MsgType.Text, text=text))
-        self._on_response(resp)
+    async def _send_text(self, text: str, **kwargs) -> WebhookResponse:
+        rsp = await self._slack_client.send_dict(self._generate_payload(msg_type=MsgType.Text, text=text))
+        return rsp
```

