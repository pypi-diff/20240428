# Comparing `tmp/voice2text_deltabot-1.2.2-py3-none-any.whl.zip` & `tmp/voice2text_deltabot-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 16823 bytes, number of entries: 9
--rw-r--r--  2.0 unx      189 b- defN 24-Mar-26 03:23 voice2text_deltabot/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 24-Mar-26 03:23 voice2text_deltabot/__main__.py
--rw-r--r--  2.0 unx     3917 b- defN 24-Mar-26 03:23 voice2text_deltabot/hooks.py
--rw-r--r--  2.0 unx    35141 b- defN 24-Mar-26 03:24 voice2text_deltabot-1.2.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1971 b- defN 24-Mar-26 03:24 voice2text_deltabot-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 03:24 voice2text_deltabot-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 24-Mar-26 03:24 voice2text_deltabot-1.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Mar-26 03:24 voice2text_deltabot-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      816 b- defN 24-Mar-26 03:24 voice2text_deltabot-1.2.2.dist-info/RECORD
-9 files, 42296 bytes uncompressed, 15387 bytes compressed:  63.6%
+Zip file size: 17482 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      189 b- defN 24-Apr-28 00:58 voice2text_deltabot/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 24-Apr-28 00:58 voice2text_deltabot/__main__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-28 00:59 voice2text_deltabot/_version.py
+-rw-r--r--  2.0 unx     4650 b- defN 24-Apr-28 00:58 voice2text_deltabot/hooks.py
+-rw-r--r--  2.0 unx    35141 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2047 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      903 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/RECORD
+10 files, 43603 bytes uncompressed, 15908 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: voice2text_deltabot/__init__.py
 Comment: 
 
 Filename: voice2text_deltabot/__main__.py
 Comment: 
 
+Filename: voice2text_deltabot/_version.py
+Comment: 
+
 Filename: voice2text_deltabot/hooks.py
 Comment: 
 
-Filename: voice2text_deltabot-1.2.2.dist-info/LICENSE.txt
+Filename: voice2text_deltabot-1.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: voice2text_deltabot-1.2.2.dist-info/METADATA
+Filename: voice2text_deltabot-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: voice2text_deltabot-1.2.2.dist-info/WHEEL
+Filename: voice2text_deltabot-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: voice2text_deltabot-1.2.2.dist-info/entry_points.txt
+Filename: voice2text_deltabot-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: voice2text_deltabot-1.2.2.dist-info/top_level.txt
+Filename: voice2text_deltabot-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: voice2text_deltabot-1.2.2.dist-info/RECORD
+Filename: voice2text_deltabot-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## voice2text_deltabot/hooks.py

```diff
@@ -1,18 +1,31 @@
 """Event handlers and hooks."""
 
 import logging
 import time
 from argparse import Namespace
 
-from deltabot_cli import AttrDict, Bot, BotCli, ChatType, EventType, ViewType, events
+from deltabot_cli import BotCli
+from deltachat2 import (
+    Bot,
+    ChatType,
+    CoreEvent,
+    EventType,
+    MessageViewtype,
+    MsgData,
+    NewMsgEvent,
+    events,
+)
 from faster_whisper import WhisperModel
 from rich.logging import RichHandler
 
+from ._version import __version__
+
 cli = BotCli("voice2text-bot")
+cli.add_generic_option("-v", "--version", action="version", version=__version__)
 cli.add_generic_option(
     "--no-time",
     help="do not display date timestamp in log messages",
     action="store_false",
 )
 cli.add_generic_option(
     "--model",
@@ -43,59 +56,76 @@
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "Voice To Text")
             status = (
                 "I'm a Delta Chat bot, send me any voice message to convert it to text"
             )
             bot.rpc.set_config(accid, "selfstatus", status)
-            bot.rpc.set_config(accid, "delete_server_after", "1")
             bot.rpc.set_config(accid, "delete_device_after", str(60 * 60 * 24))
 
 
 @cli.on_start
 def on_start(_bot: Bot, args: Namespace) -> None:
     global MODEL  # pylint: disable=W0603
     MODEL = WhisperModel(args.model, device="auto", compute_type=args.compute_type)
 
 
 @cli.on(events.RawEvent)
-def _log_event(bot: Bot, accid: int, event: AttrDict) -> None:
+def _log_event(bot: Bot, accid: int, event: CoreEvent) -> None:
     if event.kind == EventType.INFO:
         bot.logger.debug(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
-    elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
-        if event.progress == 1000:
-            bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
-            chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-            bot.rpc.send_msg(accid, chatid, {"text": HELP})
     elif event.kind == EventType.MSG_DELIVERED:
         bot.rpc.delete_messages(accid, [event.msg_id])
+    elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
+        if event.progress == 1000:
+            if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
+                bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
+                chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
+                bot.rpc.send_msg(accid, chatid, MsgData(text=HELP))
+
+
+@cli.after(events.NewMessage)
+def delete_msgs(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.delete_messages(accid, [event.msg.id])
 
 
 @cli.on(events.NewMessage(is_info=False, is_bot=None))
-def on_newmsg(bot: Bot, accid: int, event: AttrDict) -> None:
+def on_newmsg(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE:
         bot.rpc.markseen_msgs(accid, [msg.id])
         if msg.is_bot:
-            bot.rpc.delete_messages(accid, [msg.id])
             return
 
-    if msg.view_type in (ViewType.VOICE, ViewType.AUDIO):
+    if msg.view_type in (MessageViewtype.VOICE, MessageViewtype.AUDIO):
         start = time.time()
         segments, info = MODEL.transcribe(msg.file)
-        text = "\n".join(seg.text.strip() for seg in segments)
+        lines = []
+        for seg in segments:
+            if (
+                seg.avg_logprob < -0.7
+                or seg.no_speech_prob > 0.5
+                or seg.compression_ratio < 0.9
+            ):
+                continue
+            text = seg.text.strip()
+            if text.strip("."):
+                lines.append(text)
         took = time.time() - start
         percent = int(info.language_probability * 100)
         bot.logger.info(
             f"[chat={msg.chat_id}, msg={msg.id}] Voice extracted: duration={info.duration:.1f}"
             f" language={info.language} (probability={percent}%) took {took:.1f} seconds"
         )
-        bot.rpc.send_msg(accid, msg.chat_id, {"text": text, "quotedMessageId": msg.id})
+        if lines:
+            reply = MsgData(text="\n".join(lines), quoted_message_id=msg.id)
+            bot.rpc.send_msg(accid, msg.chat_id, reply)
+        else:
+            bot.rpc.send_reaction(accid, msg.id, ["😶"])
     elif chat.chat_type == ChatType.SINGLE:
-        bot.rpc.send_msg(accid, msg.chat_id, {"text": HELP})
-
-    bot.rpc.delete_messages(accid, [msg.id])
+        reply = MsgData(text=HELP)
+        bot.rpc.send_msg(accid, msg.chat_id, reply)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `voice2text_deltabot-1.2.2.dist-info/LICENSE.txt` & `voice2text_deltabot-1.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `voice2text_deltabot-1.2.2.dist-info/METADATA` & `voice2text_deltabot-1.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: voice2text-deltabot
-Version: 1.2.2
+Version: 1.3.0
 Summary: Delta Chat bot to extract text from voice messages
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/voice2text_deltabot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: deltabot-cli <6.0,>=5.0.0
+Requires-Dist: deltabot-cli <7.0,>=6.1.0
 Requires-Dist: faster-whisper
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: pylama ; extra == 'dev'
```

