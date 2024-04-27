# Comparing `tmp/text2img_bot-0.1.2-py3-none-any.whl.zip` & `tmp/text2img_bot-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 16653 bytes, number of entries: 9
--rw-r--r--  2.0 unx      179 b- defN 24-Mar-26 09:49 text2img_bot/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 24-Mar-26 09:49 text2img_bot/__main__.py
--rw-r--r--  2.0 unx     4097 b- defN 24-Mar-26 09:49 text2img_bot/hooks.py
--rw-r--r--  2.0 unx    35141 b- defN 24-Mar-26 09:49 text2img_bot-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1989 b- defN 24-Mar-26 09:49 text2img_bot-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 09:49 text2img_bot-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 24-Mar-26 09:49 text2img_bot-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-26 09:49 text2img_bot-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      749 b- defN 24-Mar-26 09:49 text2img_bot-0.1.2.dist-info/RECORD
-9 files, 42401 bytes uncompressed, 15351 bytes compressed:  63.8%
+Zip file size: 17118 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      179 b- defN 24-Apr-27 22:19 text2img_bot/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 24-Apr-27 22:19 text2img_bot/__main__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-27 22:19 text2img_bot/_version.py
+-rw-r--r--  2.0 unx     4237 b- defN 24-Apr-27 22:19 text2img_bot/hooks.py
+-rw-r--r--  2.0 unx    35141 b- defN 24-Apr-27 22:19 text2img_bot-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2058 b- defN 24-Apr-27 22:19 text2img_bot-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 22:19 text2img_bot-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 24-Apr-27 22:19 text2img_bot-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-27 22:19 text2img_bot-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      829 b- defN 24-Apr-27 22:19 text2img_bot-0.2.0.dist-info/RECORD
+10 files, 43101 bytes uncompressed, 15692 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: text2img_bot/__init__.py
 Comment: 
 
 Filename: text2img_bot/__main__.py
 Comment: 
 
+Filename: text2img_bot/_version.py
+Comment: 
+
 Filename: text2img_bot/hooks.py
 Comment: 
 
-Filename: text2img_bot-0.1.2.dist-info/LICENSE
+Filename: text2img_bot-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: text2img_bot-0.1.2.dist-info/METADATA
+Filename: text2img_bot-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: text2img_bot-0.1.2.dist-info/WHEEL
+Filename: text2img_bot-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: text2img_bot-0.1.2.dist-info/entry_points.txt
+Filename: text2img_bot-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: text2img_bot-0.1.2.dist-info/top_level.txt
+Filename: text2img_bot-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: text2img_bot-0.1.2.dist-info/RECORD
+Filename: text2img_bot-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text2img_bot/hooks.py

```diff
@@ -1,19 +1,32 @@
 """Event handlers and hooks."""
 
 from argparse import Namespace
 from tempfile import NamedTemporaryFile
 from typing import Callable
 
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
 from diffusers import AutoPipelineForImage2Image, AutoPipelineForText2Image
 from PIL import Image
 from rich.logging import RichHandler
 
+from ._version import __version__
+
 cli = BotCli("text2img-bot")
+cli.add_generic_option("-v", "--version", action="version", version=__version__)
 cli.add_generic_option(
     "--no-time",
     help="do not display date timestamp in log messages",
     action="store_false",
 )
 cli.add_generic_option(
     "--model",
@@ -37,62 +50,64 @@
         RichHandler(show_path=False, omit_repeated_times=False, show_time=args.no_time)
     ]
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "Text To Image")
             status = "I'm a Delta Chat bot, send me a message describing the image you want to generate"
             bot.rpc.set_config(accid, "selfstatus", status)
-            bot.rpc.set_config(accid, "delete_server_after", "1")
             bot.rpc.set_config(accid, "delete_device_after", str(60 * 60 * 24))
 
 
 @cli.on_start
 def on_start(_bot: Bot, args: Namespace) -> None:
     global text2img, img2img  # pylint: disable=W0603
     text2img = AutoPipelineForText2Image.from_pretrained(args.model)
     img2img = AutoPipelineForImage2Image.from_pretrained(args.model)
 
 
 @cli.on(events.RawEvent)
-def on_core_event(bot: Bot, accid: int, event: AttrDict) -> None:
+def on_core_event(bot: Bot, accid: int, event: CoreEvent) -> None:
     if event.kind == EventType.INFO:
         bot.logger.debug(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
     elif event.kind == EventType.MSG_DELIVERED:
         bot.rpc.delete_messages(accid, [event.msg_id])
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000:
             if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
                 bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
                 chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-                bot.rpc.send_msg(accid, chatid, {"text": HELP})
+                bot.rpc.send_msg(accid, chatid, MsgData(text=HELP))
 
 
-@cli.on(events.NewMessage(is_bot=None))
-def generate_img(bot: Bot, accid: int, event: AttrDict) -> None:
+@cli.on(events.NewMessage(is_info=False))
+def generate_img(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
-    if not msg.is_bot and not msg.is_info:
-        chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
-        if chat.chat_type == ChatType.SINGLE:
-            bot.rpc.markseen_msgs(accid, [msg.id])
-            if msg.text:
-                if msg.view_type == ViewType.IMAGE:
-                    image = Image.open(msg.file).convert("RGB")
-                    image.thumbnail((768, 768))
-                    image = img2img(msg.text, image, safety_checker=None).images[0]
-                else:
-                    image = text2img(msg.text, safety_checker=None).images[0]
-                with NamedTemporaryFile(suffix=".png") as tfile:
-                    image.save(tfile.name)
-                    bot.rpc.send_msg(
-                        accid,
-                        msg.chat_id,
-                        {"file": tfile.name, "quotedMessageId": msg.id},
-                    )
+    chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
+    if chat.chat_type == ChatType.SINGLE:
+        bot.rpc.markseen_msgs(accid, [msg.id])
+        if msg.text:
+            if msg.view_type == MessageViewtype.IMAGE:
+                image = Image.open(msg.file).convert("RGB")
+                image.thumbnail((768, 768))
+                image = img2img(msg.text, image, safety_checker=None).images[0]
             else:
+                image = text2img(msg.text, safety_checker=None).images[0]
+            with NamedTemporaryFile(suffix=".png") as tfile:
+                image.save(tfile.name)
                 bot.rpc.send_msg(
-                    accid, msg.chat_id, {"text": HELP, "quotedMessageId": msg.id}
+                    accid,
+                    msg.chat_id,
+                    MsgData(file=tfile.name, quoted_message_id=msg.id),
                 )
-    bot.rpc.delete_messages(accid, [msg.id])
+        else:
+            bot.rpc.send_msg(
+                accid, msg.chat_id, MsgData(text=HELP, quoted_message_id=msg.id)
+            )
+
+
+@cli.after(events.NewMessage)
+def delete_msgs(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    bot.rpc.delete_messages(accid, [event.msg.id])
```

## Comparing `text2img_bot-0.1.2.dist-info/LICENSE` & `text2img_bot-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `text2img_bot-0.1.2.dist-info/METADATA` & `text2img_bot-0.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: text2img-bot
-Version: 0.1.2
+Version: 0.2.0
 Summary: Delta Chat bot to generate images from text prompts
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/text2img-bot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltabot-cli <6.0,>=5.0.0
+Requires-Dist: deltabot-cli <7.0,>=6.1.0
 Requires-Dist: diffusers[torch]
 Requires-Dist: transformers
 Requires-Dist: pillow
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
```

## Comparing `text2img_bot-0.1.2.dist-info/RECORD` & `text2img_bot-0.2.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 text2img_bot/__init__.py,sha256=2E08_EhuRMgatraxAvRLDD0BGup52r6CgFCWahINFIk,179
 text2img_bot/__main__.py,sha256=g1i1HUavRziEp3Tg1EXeI8nyPv0PfogSdBP2ONPUJ8E,90
-text2img_bot/hooks.py,sha256=LUC-cDxUHOOdLXtX5Naoa5ieZd7JVBM-qKNXe6JgOF8,4097
-text2img_bot-0.1.2.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-text2img_bot-0.1.2.dist-info/METADATA,sha256=IHsWKYakyUo4ZPWFocmQG1glqroCCH2_fWdFJWDIxuU,1989
-text2img_bot-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-text2img_bot-0.1.2.dist-info/entry_points.txt,sha256=2L4p3vMewQ2FyWW-JyW5KliGHEsip7XJhL5UI_6I9UM,51
-text2img_bot-0.1.2.dist-info/top_level.txt,sha256=ijvP2cgBnZb4nNWlex9E6kbCz5hN-WdS1rfwhYkivBg,13
-text2img_bot-0.1.2.dist-info/RECORD,,
+text2img_bot/_version.py,sha256=H-qsvrxCpdhaQzyddR-yajEqI71hPxLa4KxzpP3uS1g,411
+text2img_bot/hooks.py,sha256=-ZzrAp1Gke-aPdOJOhyX73_-9j9plVk8jUpU1v6SGUc,4237
+text2img_bot-0.2.0.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+text2img_bot-0.2.0.dist-info/METADATA,sha256=MvrftdbTAMWAF-ZPOn1QMBOycgvlEKLMz3nGgYffnNw,2058
+text2img_bot-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+text2img_bot-0.2.0.dist-info/entry_points.txt,sha256=2L4p3vMewQ2FyWW-JyW5KliGHEsip7XJhL5UI_6I9UM,51
+text2img_bot-0.2.0.dist-info/top_level.txt,sha256=ijvP2cgBnZb4nNWlex9E6kbCz5hN-WdS1rfwhYkivBg,13
+text2img_bot-0.2.0.dist-info/RECORD,,
```

