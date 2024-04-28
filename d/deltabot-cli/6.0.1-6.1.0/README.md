# Comparing `tmp/deltabot-cli-6.0.1.tar.gz` & `tmp/deltabot_cli-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltabot-cli-6.0.1.tar", last modified: Sat Apr  6 20:47:00 2024, max compression
+gzip compressed data, was "deltabot_cli-6.1.0.tar", last modified: Sat Apr 27 18:12:18 2024, max compression
```

## Comparing `deltabot-cli-6.0.1.tar` & `deltabot_cli-6.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.137868 deltabot-cli-6.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.129868 deltabot-cli-6.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/deltabot_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/deltabot_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/deltabot_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/deltabot_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/deltabot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/examples/echobot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/examples/echobot_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:47:00.137868 deltabot-cli-6.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:12:18.932673 deltabot_cli-6.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/deltabot_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/deltabot_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/deltabot_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/deltabot_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/deltabot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-27 18:12:18.000000 deltabot_cli-6.1.0/deltabot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-27 18:12:18.000000 deltabot_cli-6.1.0/deltabot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:12:18.000000 deltabot_cli-6.1.0/deltabot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-27 18:12:18.000000 deltabot_cli-6.1.0/deltabot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 18:12:18.000000 deltabot_cli-6.1.0/deltabot_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/examples/echobot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/examples/echobot_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-27 18:12:05.000000 deltabot_cli-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:12:18.936673 deltabot_cli-6.1.0/setup.cfg
```

### Comparing `deltabot-cli-6.0.1/.github/workflows/python-ci.yml` & `deltabot_cli-6.1.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.1/LICENSE` & `deltabot_cli-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.1/PKG-INFO` & `deltabot_cli-6.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: deltabot-cli
-Version: 6.0.1
+Version: 6.1.0
 Summary: Library to speedup Delta Chat bot development
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/deltabot-cli-py
 Keywords: deltachat,bot,deltabot-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltachat2[full]
+Requires-Dist: deltachat2[full]>=0.5.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: rich>=12.6.0
 Requires-Dist: qrcode>=7.4.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `deltabot-cli-6.0.1/README.md` & `deltabot_cli-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.1/deltabot_cli/_utils.py` & `deltabot_cli-6.1.0/deltabot_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.1/deltabot_cli/cli.py` & `deltabot_cli-6.1.0/deltabot_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,22 @@
         self._parser = ArgumentParser(app_name)
         self._subparsers = self._parser.add_subparsers(title="subcommands")
         self._hooks = HookCollection()
         self._init_hooks: Set[CliEventHook] = set()
         self._start_hooks: Set[CliEventHook] = set()
         self._bot: Bot
 
-    def on(self, event: Union[type, EventFilter]) -> HookDecorator:  # noqa
+    def on(self, event: Union[type, EventFilter]) -> HookDecorator:
         """Register decorated function as listener for the given event."""
         return self._hooks.on(event)
 
+    def after(self, event: Union[type, EventFilter]) -> HookDecorator:
+        """Register decorated function as listener for the given event."""
+        return self._hooks.after(event)
+
     def on_init(self, func: CliEventHook) -> CliEventHook:
         """Register function to be called before the bot starts serving requests.
 
         The function will receive the bot instance and the CLI arguments received.
         """
         self._init_hooks.add(func)
         return func
```

### Comparing `deltabot-cli-6.0.1/deltabot_cli.egg-info/PKG-INFO` & `deltabot_cli-6.1.0/deltabot_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: deltabot-cli
-Version: 6.0.1
+Version: 6.1.0
 Summary: Library to speedup Delta Chat bot development
 Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/deltachat-bot/deltabot-cli-py
 Keywords: deltachat,bot,deltabot-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deltachat2[full]
+Requires-Dist: deltachat2[full]>=0.5.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: rich>=12.6.0
 Requires-Dist: qrcode>=7.4.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `deltabot-cli-6.0.1/examples/echobot_advanced.py` & `deltabot_cli-6.1.0/examples/echobot_advanced.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,34 +29,41 @@
 def log_event(bot, accid, event):
     if event.kind == EventType.INFO:
         bot.logger.debug(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
+    elif event.kind == EventType.MSG_DELIVERED:
+        bot.rpc.delete_messages(accid, [event.msg_id])
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000 and not bot.rpc.get_contact(accid, event.contact_id).is_bot:
             # bot's QR scanned by an user, send introduction message
             chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
             reply = MsgData(text="Hi, I will repeat anything you say to me")
             bot.rpc.send_msg(accid, chatid, reply)
 
 
+@cli.on(events.NewMessage(command="/help"))
+def _help(bot, accid, event):
+    msg = event.msg
+    bot.rpc.send_msg(accid, msg.chat_id, MsgData(text="I will repeat anything you say to me"))
+
+
 @cli.on(events.NewMessage(is_info=False))
 def echo(bot, accid, event):
     if bot.has_command(event.command):
         return
     msg = event.msg
     bot.rpc.send_msg(accid, msg.chat_id, MsgData(text=msg.text))
 
 
-@cli.on(events.NewMessage(command="/help"))
-def _help(bot, accid, event):
-    msg = event.msg
-    bot.rpc.send_msg(accid, msg.chat_id, MsgData(text="I will repeat anything you say to me"))
+@cli.after(events.NewMessage)
+def delete_msgs(bot, accid, event):
+    bot.rpc.delete_messages(accid, [event.msg.id])
 
 
 def test(_cli, bot, args):
     """just some example subcommand"""
     bot.logger.info("Hello %s, this is an example subcommand!", args.name)
```

### Comparing `deltabot-cli-6.0.1/pyproject.toml` & `deltabot_cli-6.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 dependencies = [
-    "deltachat2[full]",
+    "deltachat2[full]>=0.5.0",
     "appdirs>=1.4.4",
     "rich>=12.6.0",
     "qrcode>=7.4.2",
 ]
 
+[project.urls]
+Homepage = "https://github.com/deltachat-bot/deltabot-cli-py"
+
 [project.optional-dependencies]
 dev = [
   "black",
   "mypy",
   "isort",
   "pylint",
   "pylama",
```

