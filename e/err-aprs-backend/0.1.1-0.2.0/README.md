# Comparing `tmp/err_aprs_backend-0.1.1.tar.gz` & `tmp/err_aprs_backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "err_aprs_backend-0.1.1.tar", max compression
+gzip compressed data, was "err_aprs_backend-0.2.0.tar", max compression
```

## Comparing `err_aprs_backend-0.1.1.tar` & `err_aprs_backend-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1063 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/LICENSE
--rw-r--r--   0        0        0     4541 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/README.md
--rw-r--r--   0        0        0       57 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/__init__.py
--rw-r--r--   0        0        0       81 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/aprs.plug
--rw-r--r--   0        0        0    15477 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/aprs.py
--rw-r--r--   0        0        0      104 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/clients/__init__.py
--rw-r--r--   0        0        0     5152 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/clients/aprsis.py
--rw-r--r--   0        0        0       82 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/clients/kiss.py
--rw-r--r--   0        0        0       48 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      151 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/client/__init__.py
--rw-r--r--   0        0        0      311 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/client/aprsis.py
--rw-r--r--   0        0        0      113 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/packets/__init__.py
--rw-r--r--   0        0        0      112 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/packets/parser.py
--rw-r--r--   0        0        0      742 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/message.py
--rw-r--r--   0        0        0     5420 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/packets/__init__.py
--rw-r--r--   0        0        0    10018 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/packets/parser.py
--rw-r--r--   0        0        0      748 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/person.py
--rw-r--r--   0        0        0       83 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/room.py
--rw-r--r--   0        0        0      500 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/utils/__init__.py
--rw-r--r--   0        0        0      601 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/utils/counter.py
--rw-r--r--   0        0        0       26 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/utils/version.py
--rw-r--r--   0        0        0     1334 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 err_aprs_backend-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4600 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/README.md
+-rw-r--r--   0        0        0      105 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/aprs.plug
+-rw-r--r--   0        0        0    17599 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/aprs.py
+-rw-r--r--   0        0        0      212 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/clients/__init__.py
+-rw-r--r--   0        0        0     2719 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/clients/aprs_registry.py
+-rw-r--r--   0        0        0     5374 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/clients/aprsis.py
+-rw-r--r--   0        0        0       82 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/clients/kiss.py
+-rw-r--r--   0        0        0       48 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/exceptions/client/__init__.py
+-rw-r--r--   0        0        0      311 2024-04-28 03:41:50.720802 err_aprs_backend-0.2.0/aprs_backend/exceptions/client/aprsis.py
+-rw-r--r--   0        0        0      113 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/exceptions/packets/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/exceptions/packets/parser.py
+-rw-r--r--   0        0        0      744 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/message.py
+-rw-r--r--   0        0        0     5372 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/packets/__init__.py
+-rw-r--r--   0        0        0     9997 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/packets/parser.py
+-rw-r--r--   0        0        0     1038 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/person.py
+-rw-r--r--   0        0        0       83 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/room.py
+-rw-r--r--   0        0        0      495 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/utils/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/utils/counter.py
+-rw-r--r--   0        0        0       26 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/utils/version.py
+-rw-r--r--   0        0        0       22 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/aprs_backend/version.py
+-rw-r--r--   0        0        0     1412 2024-04-28 03:41:50.724802 err_aprs_backend-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.2.0/PKG-INFO
```

### Comparing `err_aprs_backend-0.1.1/LICENSE` & `err_aprs_backend-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.1/README.md` & `err_aprs_backend-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 # use bot_identity to provide your callsign and APRS password
 BOT_IDENTITY = {
     "callsign": "YOURCALL-1",
     "password": "123456"
 }
 ```
 
+See [CONFIG.md](CONFIG.md) for more configuration options
+
 ### Disable the default plugins
 
 The default plugins allow configuring the bot, installing plugins, and returing detailed help information. These don't work well over APRS because
 you cannot authenticate an admin. You don't want just anyone able to install a plugin on your machine!
 
 The backend has a built in Help that you can set to a static string in the config with APRS_HELP_TEXT. Setting this to a website with help info
 or more info about your bot would be a good way to send a user more details on your bot without needing to send Errbot's normal detailed help info.
@@ -88,15 +90,15 @@
 
 ```python
 SUPPRESS_CMD_NOT_FOUND = True
 ```
 
 ### Bot Prefix
 You can leave your bot prefix on, but that's just extra characters. I prefer to make it optional so users don't have to
-send it on every commadn
+send it on every command
 
 ```python
 BOT_PREFIX_OPTIONAL_ON_CHAT = True
 ```
 
 ### Full Example Config
```

### Comparing `err_aprs_backend-0.1.1/aprs_backend/clients/aprsis.py` & `err_aprs_backend-0.2.0/aprs_backend/clients/aprsis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 import logging
 import asyncio
 from functools import cached_property
 import time
-from aprs_backend.exceptions.client.aprsis import APRSISClientError, APRSISConnnectError, APRSISPacketError, APRSISDeadConnectionError, APRSISPacketDecodeError
+from aprs_backend.exceptions.client.aprsis import (
+    APRSISClientError,
+    APRSISConnnectError,
+    APRSISPacketError,
+    APRSISDeadConnectionError,
+    APRSISPacketDecodeError,
+)
+
 
 class APRSISClient:
-    def __init__(self, callsign: str,
-               password: int,
-               host: str = "rotate.aprs2.net",
-               port: int = 14580,
-               aprs_filter: str = "DEFAULT",
-               aprs_app_name: str = "ErrbotAPRS",
-               app_version: str = "",
-               logger: logging.Logger | None = None,
-               keepalive_seconds: int = 120):
+    def __init__(
+        self,
+        callsign: str,
+        password: int,
+        host: str = "rotate.aprs2.net",
+        port: int = 14580,
+        aprs_filter: str = "DEFAULT",
+        aprs_app_name: str = "ErrbotAPRS",
+        app_version: str = "",
+        logger: logging.Logger | None = None,
+        keepalive_seconds: int = 120,
+    ):
         self.callsign = callsign
         self.password = password
         self.aprs_host = host
         self.aprs_port = port
         self.aprs_filter = aprs_filter
         self._aprs_app_name = aprs_app_name
         self._app_version = app_version
@@ -33,40 +43,41 @@
         self.__packet_count = 0
         self._writer = None
         self._reader = None
         self._keepalive_last_sent = 0
         self._last_successful_connect = 0
 
     @cached_property
-    def _aprs_login(self)->bytes:
+    def _aprs_login(self) -> bytes:
         return f"user {self.callsign} pass {self.password} vers {self._aprs_app_name} {self._app_version} filter {self.aprs_filter}\n"
 
     @cached_property
-    def _keepalive_packet(self)->bytes:
+    def _keepalive_packet(self) -> bytes:
         return b"#keepalive\n"
 
     async def connect(self) -> None:
         self.__connect_count += 1
         try:
             self._reader, self._writer = await asyncio.open_connection(self.aprs_host, self.aprs_port)
             # login to aprsis
             await self._send(self._aprs_login)
             self._last_successful_connect = time.perf_counter()
-            self._log.info("Connected to %s/%s:%s as %s with filter %s",
-                        self.aprs_host,
-                        self._get_sock_peer_ip(self._writer),
-                        self.aprs_port,
-                        self.callsign,
-                        self.aprs_filter
-                        )
+            self._log.info(
+                "Connected to %s/%s:%s as %s with filter %s",
+                self.aprs_host,
+                self._get_sock_peer_ip(self._writer),
+                self.aprs_port,
+                self.callsign,
+                self.aprs_filter,
+            )
             self.connected = True
         except Exception as exc:
-             self._log.error("Error while connecting: %s", exc)
-             self.connected = False
-             raise APRSISConnnectError from exc
+            self._log.error("Error while connecting: %s", exc)
+            self.connected = False
+            raise APRSISConnnectError from exc
 
     async def disconnect(self):
         self._log.info("Disconnecting from aprsis")
         self._writer.close()
         self._reader.close()
         await self._writer.wait_closed()
         await self._reader.wait_closed()
@@ -74,26 +85,32 @@
         self._reader = None
         self.connected = False
         self._log.info("Disconnected")
 
     async def _send(self, packet: str, encoding: str = "utf-8") -> None:
         self._log.debug("Sending '%s'", packet)
         packet = packet.rstrip("\r\n") + "\r\n"
-        self._writer.write(packet.encode(encoding))
-        await self._writer.drain()
+        if packet is None:
+            self._log.error("Packet is None - %s - Dropping", packet)
+            return
+        if self._writer is not None:
+            self._writer.write(packet.encode(encoding))
+            await self._writer.drain()
+        else:
+            self._log.error("Disconnected, unable to send packet %s, dropped", packet)
 
     async def _send_keepalive(self) -> bool:
         """
         Send KeepAlive packet if necessary. _writer must be connected.
         :return Whether or not one was sent.
         """
         now = time.perf_counter()
         if self.connected:
             if (now - self._keepalive_last_sent) > self._keepalive_seconds:
-                self._log.debug(f'Sending keepalive to {self._get_sock_peer_ip(self._writer)}')
+                self._log.debug(f"Sending keepalive to {self._get_sock_peer_ip(self._writer)}")
                 await self._send(self._keepalive_packet)
                 self._keepalive_last_sent = now
                 return True
         return False
 
     async def get_packet(self) -> str:
         """Get a packet from APRSIS
@@ -107,15 +124,15 @@
         """
         if not self.connected:
             raise APRSISConnnectError("Not connected")
         try:
             # Read packet string from socket
             packet_bytes = await self._reader.readline()
         except Exception as exc:
-            logging.error('Could not read packet: %s', exc)
+            logging.error("Could not read packet: %s", exc)
             raise APRSISPacketError from exc
 
         if not packet_bytes:
             # zero length packets can be returned if keepalives have failed after ~30m
             self._log.warning("Empty packet received. Probably missed keepalives.")
             raise APRSISDeadConnectionError("Empty packet received. Probably missed keepalives")
 
@@ -127,11 +144,11 @@
             raise APRSISClientError from exc
         self.__packet_count += 1
         self._log.debug("Received %d total packets", self.__packet_count)
         return return_packet
 
     @staticmethod
     def _get_sock_peer_ip(writer):
-        sock = writer.get_extra_info('socket')
+        sock = writer.get_extra_info("socket")
         if sock:
             return sock.getpeername()[0]
         return None
```

### Comparing `err_aprs_backend-0.1.1/aprs_backend/message.py` & `err_aprs_backend-0.2.0/aprs_backend/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from errbot.backends.base import Message
 from aprs_backend.packets import MessagePacket
 from aprs_backend.person import APRSPerson
 
+
 class APRSMessage(Message):
     @property
     def is_direct(self):
         return True
 
     @classmethod
     def from_message_packet(cls, packet: MessagePacket) -> "APRSMessage":
@@ -13,12 +14,12 @@
             body=packet.message_text,
             extras={
                 "msgNo": packet.msgNo,
                 "via": packet.via,
                 "path": packet.path,
                 "raw": packet.raw,
                 "packet": packet,
-            }
+            },
         )
         this_msg.frm = APRSPerson(callsign=packet.from_call)
         this_msg.to = APRSPerson(callsign=packet.addresse)
         return this_msg
```

### Comparing `err_aprs_backend-0.1.1/aprs_backend/packets/__init__.py` & `err_aprs_backend-0.2.0/aprs_backend/packets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from aprs_backend.utils.counter import MessageCounter
 
 
 def _init_timestamp():
     """Build a unix style timestamp integer"""
     return int(round(time.time()))
 
+
 @dataclass_json
 @dataclass(unsafe_hash=True)
 class Packet:
     _type: str = field(default="Packet", hash=False)
     from_call: str | None = field(default=None)
     to_call: str | None = field(default=None)
     addresse: str | None = field(default=None)
     format: str | None = field(default=None)
-    msgNo: str | None = field(default=None)   # noqa: N815
+    msgNo: str | None = field(default=None)  # noqa: N815
     packet_type: str | None = field(default=None)
     timestamp: float = field(default_factory=_init_timestamp, compare=False, hash=False)
     # Holds the raw text string to be sent over the wire
     # or holds the raw string from input packet
     raw: str | None = field(default=None, compare=False, hash=False)
     raw_dict: dict = field(repr=False, default_factory=lambda: {}, compare=False, hash=False)
     # Built by calling prepare().  raw needs this built first.
@@ -82,17 +83,15 @@
 
     def _build_payload(self) -> None:
         """The payload is the non headers portion of the packet."""
         if not self.to_call:
             raise ValueError("to_call isn't set. Must set to_call before calling prepare()")
 
         # The base packet class has no real payload
-        self.payload = (
-            f":{self.to_call.ljust(9)}"
-        )
+        self.payload = f":{self.to_call.ljust(9)}"
 
     def _build_raw(self) -> None:
         """Build the self.raw which is what is sent over the air."""
         self.raw = "{}>APZ100:{}".format(
             self.from_call,
             self.payload,
         )
@@ -105,33 +104,31 @@
         # feature req: break long ones into two msgs
         if not msg:
             return ""
 
         message = msg[:67]
         # We all miss George Carlin
         return re.sub(
-            "fuck|shit|cunt|piss|cock|bitch", "****",
-            message, flags=re.IGNORECASE,
+            "fuck|shit|cunt|piss|cock|bitch",
+            "****",
+            message,
+            flags=re.IGNORECASE,
         )
 
     def __str__(self) -> str:
         """Show the raw version of the packet"""
         self._build_payload()
         self._build_raw()
         if not self.raw:
             raise ValueError("self.raw is unset")
         return self.raw
 
     def __repr__(self) -> str:
         """Build the repr version of the packet."""
-        repr = (
-            f"{self.__class__.__name__}:"
-            f" From: {self.from_call}  "
-            f"   To: {self.to_call}"
-        )
+        repr = f"{self.__class__.__name__}:" f" From: {self.from_call}  " f"   To: {self.to_call}"
         return repr
 
 
 @dataclass_json
 @dataclass(unsafe_hash=True)
 class AckPacket(Packet):
     _type: str = field(default="AckPacket", hash=False)
```

### Comparing `err_aprs_backend-0.1.1/aprs_backend/packets/parser.py` & `err_aprs_backend-0.2.0/aprs_backend/packets/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,21 @@
     # the user for all messages that relate to the original one.
     # aprslib does currently not recognise these new message IDs
     # If we don't have a msg_no already and do have message_text, this might
     # be a new ack/rej
     if msg_no is None and message_text is not None:
         message_text, msg_no, is_new_ackrej = check_for_new_ackrej_format(message_text=message_text)
 
-    raw_aprs_packet['from'] = from_callsign
-    raw_aprs_packet['message_text'] = message_text
-    raw_aprs_packet['msgNo'] = msg_no
-    raw_aprs_packet['is_new_ackrej'] = is_new_ackrej
-    raw_aprs_packet['packet_type'] = get_packet_type(raw_aprs_packet)
+    raw_aprs_packet["from"] = from_callsign
+    raw_aprs_packet["message_text"] = message_text
+    raw_aprs_packet["msgNo"] = msg_no
+    raw_aprs_packet["is_new_ackrej"] = is_new_ackrej
+    raw_aprs_packet["packet_type"] = get_packet_type(raw_aprs_packet)
 
-    match raw_aprs_packet['packet_type']:
+    match raw_aprs_packet["packet_type"]:
         case "MESSAGE":
             packet = MessagePacket.from_dict(raw_aprs_packet)
             packet.from_call = from_callsign
 
         case "ACK":
             packet = AckPacket.from_dict(raw_aprs_packet)
             packet.from_call = from_callsign
@@ -92,14 +92,15 @@
 
         case _:
             log.info("Packet is not a message, ack, or reject. Not parsing it")
             packet = None
 
     return packet
 
+
 def check_for_new_ackrej_format(message_text: str) -> tuple[str, str, bool]:
     """
     Have a look at the incoming APRS message and check if it
     contains a message no which does not follow the APRS
     standard (see aprs101.pdf chapter 14)
 
     http://www.aprs.org/aprs11/replyacks.txt
@@ -204,17 +205,15 @@
     new_ackrej_format = False
 
     # if message text is present, split up between aaaaaa{bb}cc
     # where aaaaaa = message text
     # bb = message number
     # cc = message retry (may or may not be present)
     if message_text:
-        matches = re.search(
-            r"^(.*){([a-zA-Z0-9]{2})}(\w*)$", message_text, re.IGNORECASE
-        )
+        matches = re.search(r"^(.*){([a-zA-Z0-9]{2})}(\w*)$", message_text, re.IGNORECASE)
         if matches:
             try:
                 msg = matches[1].rstrip()
                 msgno = matches[2]
                 new_ackrej_format = True
             except Exception:
                 msg = message_text
```

### Comparing `err_aprs_backend-0.1.1/aprs_backend/person.py` & `err_aprs_backend-0.2.0/aprs_backend/person.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,7 +34,18 @@
     @property
     def email(self) -> None:
         return None
 
     @property
     def callsign(self) -> str:
         return self._callsign
+
+    def __eq__(self, other: any) -> bool:
+        if isinstance(other, APRSPerson):
+            return self._callsign.lower() == other._callsign.lower()
+        return False
+
+    def __hash__(self):
+        return hash(self._callsign)
+
+    def __str__(self):
+        return self._callsign
```

### Comparing `err_aprs_backend-0.1.1/aprs_backend/utils/counter.py` & `err_aprs_backend-0.2.0/aprs_backend/utils/counter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
+from threading import RLock
 
 
 class MessageCounter:
     def __init__(self, initial_value: int = 1, max_message_count: int = 999):
         self._lock = asyncio.Lock()
+        self._sync_lock = RLock()
         self._value = initial_value
         self._max = max_message_count
 
     async def increment(self):
         async with self._lock:
             self._value += 1
             if self._value > self._max:
@@ -15,7 +17,17 @@
 
     async def get_value(self, increment: bool = True) -> int:
         if increment:
             await self.increment()
         async with self._lock:
             this_val = self._value
         return this_val
+
+    def get_value_sync(self, increment: bool = True) -> int:
+        if increment:
+            with self._sync_lock:
+                self._value += 1
+            if self._value > self._max:
+                self._value = 1
+        with self._sync_lock:
+            this_val = self._value
+        return this_val
```

### Comparing `err_aprs_backend-0.1.1/pyproject.toml` & `err_aprs_backend-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "err-aprs-backend"
-version = "0.1.1"
+version = "0.2.0"
 description = "Errbot APRS backend plugin"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aprs_backend"}]
 include = ["*.plug"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aprslib = "^0.7.2"
 expiringdict = "^1.2.2"
 dataclasses-json = "^0.6.4"
 better-profanity = "^0.7.0"
+httpx = "^0.27.0"
 
 
 [tool.poetry.plugins]
 
 [tool.poetry.plugins."errbot.backend_plugins"]
 aprs = "aprs_backend:APRSBackend"
 
@@ -26,18 +27,20 @@
 coverage = {extras = ["toml"], version = ">=6.5,<8.0"}
 pre-commit = ">=2.12.1"
 pep8-naming = "^0.13.2"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.2.0"
 pyupgrade = "^3.15.2"
 pytest-xdist = "^3.1.0"
-ruff = ">=0.0.249,<0.3.8"
+ruff = ">=0.0.249,<0.4.3"
 bandit = "^1.7.8"
 pytest-subtests = "^0.12.1"
 pytest-cov = "^5.0.0"
+pytest-asyncio = "^0.23.6"
+pytest-httpx = "^0.30.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
@@ -49,8 +52,8 @@
 
 [tool.errbot.backend_plugins]
 supported_errbot_version = ">=6.2.0"
 
 
 [tool.pytest.ini_options]
 norecursedirs = ".github ci .git .idea"
-addopts = "--cov=aprs_backend --cov-report xml:.coverage.xml --cov-report=term-missing"
+addopts = "-n auto --cov=aprs_backend --cov-report xml:.coverage.xml --cov-report=term-missing"
```

### Comparing `err_aprs_backend-0.1.1/PKG-INFO` & `err_aprs_backend-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: err-aprs-backend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Errbot APRS backend plugin
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aprslib (>=0.7.2,<0.8.0)
 Requires-Dist: better-profanity (>=0.7.0,<0.8.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: expiringdict (>=1.2.2,<2.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Description-Content-Type: text/markdown
 
 # err-aprs-backend
 
 An APRS Backend for Errbot
 
 ## Requirements
@@ -83,14 +84,16 @@
 # use bot_identity to provide your callsign and APRS password
 BOT_IDENTITY = {
     "callsign": "YOURCALL-1",
     "password": "123456"
 }
 ```
 
+See [CONFIG.md](CONFIG.md) for more configuration options
+
 ### Disable the default plugins
 
 The default plugins allow configuring the bot, installing plugins, and returing detailed help information. These don't work well over APRS because
 you cannot authenticate an admin. You don't want just anyone able to install a plugin on your machine!
 
 The backend has a built in Help that you can set to a static string in the config with APRS_HELP_TEXT. Setting this to a website with help info
 or more info about your bot would be a good way to send a user more details on your bot without needing to send Errbot's normal detailed help info.
@@ -106,15 +109,15 @@
 
 ```python
 SUPPRESS_CMD_NOT_FOUND = True
 ```
 
 ### Bot Prefix
 You can leave your bot prefix on, but that's just extra characters. I prefer to make it optional so users don't have to
-send it on every commadn
+send it on every command
 
 ```python
 BOT_PREFIX_OPTIONAL_ON_CHAT = True
 ```
 
 ### Full Example Config
```

