# Comparing `tmp/deltachat2-0.5.0.tar.gz` & `tmp/deltachat2-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat2-0.5.0.tar", last modified: Sat Apr 27 17:50:25 2024, max compression
+gzip compressed data, was "deltachat2-0.5.1.tar", last modified: Sun Apr 28 13:35:49 2024, max compression
```

## Comparing `deltachat2-0.5.0.tar` & `deltachat2-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.544716 deltachat2-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.536716 deltachat2-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-27 17:50:13.000000 deltachat2-0.5.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 17:50:13.000000 deltachat2-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 17:50:13.000000 deltachat2-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-27 17:50:25.544716 deltachat2-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-27 17:50:13.000000 deltachat2-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/deltachat2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/deltachat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-27 17:50:13.000000 deltachat2-0.5.0/examples/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-27 17:50:13.000000 deltachat2-0.5.0/examples/echobot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-27 17:50:13.000000 deltachat2-0.5.0/examples/echobot_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 17:50:13.000000 deltachat2-0.5.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-27 17:50:13.000000 deltachat2-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:50:25.544716 deltachat2-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:49.216350 deltachat2-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:49.212350 deltachat2-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:49.212350 deltachat2-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-28 13:35:39.000000 deltachat2-0.5.1/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-28 13:35:39.000000 deltachat2-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-28 13:35:39.000000 deltachat2-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-28 13:35:49.216350 deltachat2-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-28 13:35:39.000000 deltachat2-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:49.212350 deltachat2-0.5.1/deltachat2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-28 13:35:39.000000 deltachat2-0.5.1/deltachat2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:49.216350 deltachat2-0.5.1/deltachat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-28 13:35:49.000000 deltachat2-0.5.1/deltachat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-28 13:35:49.000000 deltachat2-0.5.1/deltachat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:35:49.000000 deltachat2-0.5.1/deltachat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-28 13:35:49.000000 deltachat2-0.5.1/deltachat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 13:35:49.000000 deltachat2-0.5.1/deltachat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:49.216350 deltachat2-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-28 13:35:39.000000 deltachat2-0.5.1/examples/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-28 13:35:39.000000 deltachat2-0.5.1/examples/echobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-28 13:35:39.000000 deltachat2-0.5.1/examples/echobot_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 13:35:39.000000 deltachat2-0.5.1/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-28 13:35:39.000000 deltachat2-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:35:49.216350 deltachat2-0.5.1/setup.cfg
```

### Comparing `deltachat2-0.5.0/.github/workflows/python-ci.yml` & `deltachat2-0.5.1/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/LICENSE` & `deltachat2-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/PKG-INFO` & `deltachat2-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.5.0
+Version: 0.5.1
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: deltachat-rpc-server>=1.136.6; extra == "full"
+Requires-Dist: deltachat-rpc-server>=1.137.4; extra == "full"
 Provides-Extra: dev
 Requires-Dist: deltachat-rpc-server; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pylama; extra == "dev"
```

### Comparing `deltachat2-0.5.0/README.md` & `deltachat2-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/_utils.py` & `deltachat2-0.5.1/deltachat2/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/bot.py` & `deltachat2-0.5.1/deltachat2/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import Callable, Iterable, Optional, Tuple, Union
 
 from .client import Client
 from .events import EventFilter, HookCallback, NewMessage
 from .rpc import Rpc
+from .transport import JsonRpcError
 from .types import Event, EventType, Message, NewMsgEvent, SpecialContactId
 
 
 class Bot(Client):
     """A Delta Chat client with the bot setting set to 1.
 
     This bot client triggers "NewMessage" highlevel events
@@ -99,13 +100,18 @@
 
     def _on_new_msg(self, accid: int, msg: Message) -> None:
         event = NewMsgEvent(command="", payload="", msg=msg)
         if not msg.is_info and msg.text.startswith(self.command_prefix):
             self._parse_command(accid, event)
         self._on_event(Event(accid, event), NewMessage)  # noqa
 
-    def _process_messages(self, accid: int) -> None:
-        for msgid in self.rpc.get_next_msgs(accid):
-            msg = self.rpc.get_message(accid, msgid)
-            if msg.from_id > SpecialContactId.LAST_SPECIAL:
-                self._on_new_msg(accid, msg)
-            self.rpc.set_config(accid, "last_msg_id", str(msgid))
+    def _process_messages(self, accid: int, retry=True) -> None:
+        try:
+            for msgid in self.rpc.get_next_msgs(accid):
+                msg = self.rpc.get_message(accid, msgid)
+                if msg.from_id > SpecialContactId.LAST_SPECIAL:
+                    self._on_new_msg(accid, msg)
+                self.rpc.set_config(accid, "last_msg_id", str(msgid))
+        except JsonRpcError as err:
+            self.logger.exception(err)
+            if retry:
+                self._process_messages(accid, False)
```

### Comparing `deltachat2-0.5.0/deltachat2/client.py` & `deltachat2-0.5.1/deltachat2/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/events.py` & `deltachat2-0.5.1/deltachat2/events.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/rpc.py` & `deltachat2-0.5.1/deltachat2/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/transport.py` & `deltachat2-0.5.1/deltachat2/transport.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/types.py` & `deltachat2-0.5.1/deltachat2/types.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2/util.py` & `deltachat2-0.5.1/deltachat2/util.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/deltachat2.egg-info/PKG-INFO` & `deltachat2-0.5.1/deltachat2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.5.0
+Version: 0.5.1
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: deltachat-rpc-server>=1.136.6; extra == "full"
+Requires-Dist: deltachat-rpc-server>=1.137.4; extra == "full"
 Provides-Extra: dev
 Requires-Dist: deltachat-rpc-server; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pylama; extra == "dev"
```

### Comparing `deltachat2-0.5.0/examples/client.py` & `deltachat2-0.5.1/examples/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/examples/echobot.py` & `deltachat2-0.5.1/examples/echobot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/examples/echobot_advanced.py` & `deltachat2-0.5.1/examples/echobot_advanced.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.5.0/pyproject.toml` & `deltachat2-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: 3",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 
 [project.optional-dependencies]
 full = [
-    "deltachat-rpc-server>=1.136.6",
+    "deltachat-rpc-server>=1.137.4",
 ]
 dev = [
   "deltachat-rpc-server",
   "black",
   "mypy",
   "isort",
   "pylint",
```

