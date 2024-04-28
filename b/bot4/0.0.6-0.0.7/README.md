# Comparing `tmp/bot4-0.0.6.tar.gz` & `tmp/bot4-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot4-0.0.6.tar", last modified: Wed Feb 14 17:36:01 2024, max compression
+gzip compressed data, was "bot4-0.0.7.tar", last modified: Sun Apr 28 17:32:20 2024, max compression
```

## Comparing `bot4-0.0.6.tar` & `bot4-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.699101 bot4-0.0.6/
--rw-rw-rw-   0        0        0      469 2024-02-14 17:36:01.699101 bot4-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-02-07 15:00:24.000000 bot4-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.650815 bot4-0.0.6/bot4/
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.660817 bot4-0.0.6/bot4/net/
--rw-rw-rw-   0        0        0        0 2023-10-08 12:24:36.000000 bot4-0.0.6/bot4/net/__init__.py
--rw-rw-rw-   0        0        0      538 2024-02-04 15:58:00.000000 bot4-0.0.6/bot4/net/auth.py
--rw-rw-rw-   0        0        0     4230 2024-01-09 19:17:00.000000 bot4-0.0.6/bot4/net/crypto.py
--rw-rw-rw-   0        0        0     2405 2024-02-14 17:32:05.000000 bot4-0.0.6/bot4/pars_packets_name.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.668820 bot4-0.0.6/bot4/protocol/
--rw-rw-rw-   0        0        0     8849 2024-01-09 16:13:47.000000 bot4-0.0.6/bot4/protocol/bot_quarry_v2.py
--rw-rw-rw-   0        0        0     4675 2024-02-11 16:54:40.000000 bot4-0.0.6/bot4/protocol/client.py
--rw-rw-rw-   0        0        0    16743 2024-02-11 16:52:15.000000 bot4-0.0.6/bot4/protocol/protocol.py
--rw-rw-rw-   0        0        0     2772 2024-02-07 14:50:58.000000 bot4-0.0.6/bot4/protocol/server.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.678247 bot4-0.0.6/bot4/types/
--rw-rw-rw-   0        0        0        0 2023-10-08 12:24:36.000000 bot4-0.0.6/bot4/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.691100 bot4-0.0.6/bot4/types/buffer/
--rw-rw-rw-   0        0        0      683 2024-01-09 19:04:08.000000 bot4-0.0.6/bot4/types/buffer/__init__.py
--rw-rw-rw-   0        0        0    14300 2024-01-09 19:08:34.000000 bot4-0.0.6/bot4/types/buffer/v1_13.py
--rw-rw-rw-   0        0        0      921 2024-01-09 19:08:47.000000 bot4-0.0.6/bot4/types/buffer/v1_13_2.py
--rw-rw-rw-   0        0        0    10350 2024-01-09 19:09:04.000000 bot4-0.0.6/bot4/types/buffer/v1_14.py
--rw-rw-rw-   0        0        0      779 2024-01-09 19:10:39.000000 bot4-0.0.6/bot4/types/buffer/v1_19.py
--rw-rw-rw-   0        0        0     2893 2024-01-09 19:11:20.000000 bot4-0.0.6/bot4/types/buffer/v1_19_1.py
--rw-rw-rw-   0        0        0    14327 2024-01-09 19:07:28.000000 bot4-0.0.6/bot4/types/buffer/v1_7.py
--rw-rw-rw-   0        0        0     5533 2024-01-09 19:08:27.000000 bot4-0.0.6/bot4/types/buffer/v1_9.py
--rw-rw-rw-   0        0        0     8623 2024-01-09 19:14:23.000000 bot4-0.0.6/bot4/types/chat.py
--rw-rw-rw-   0        0        0    14120 2024-01-25 17:51:10.000000 bot4-0.0.6/bot4/types/chunk.py
--rw-rw-rw-   0        0        0    10828 2024-01-09 19:15:09.000000 bot4-0.0.6/bot4/types/nbt.py
--rw-rw-rw-   0        0        0     5454 2024-01-09 18:59:55.000000 bot4-0.0.6/bot4/types/registry.py
--rw-rw-rw-   0        0        0      600 2024-02-11 16:44:32.000000 bot4-0.0.6/bot4/types/settings.py
--rw-rw-rw-   0        0        0      749 2023-10-08 12:24:36.000000 bot4-0.0.6/bot4/types/uuid.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.697101 bot4-0.0.6/bot4/versions/
--rw-rw-rw-   0        0        0     7816 2023-12-31 15:18:15.000000 bot4-0.0.6/bot4/versions/754.json
--rw-rw-rw-   0        0        0     8474 2024-02-14 17:32:36.000000 bot4-0.0.6/bot4/versions/757.json
--rw-rw-rw-   0        0        0     7080 2024-02-11 16:44:23.000000 bot4-0.0.6/bot4/versions/packets.py
--rw-rw-rw-   0        0        0       46 2024-02-14 17:26:53.000000 bot4-0.0.6/bot4/versions/version_protocols
-drwxrwxrwx   0        0        0        0 2024-02-14 17:36:01.657817 bot4-0.0.6/bot4.egg-info/
--rw-rw-rw-   0        0        0      469 2024-02-14 17:36:01.000000 bot4-0.0.6/bot4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-02-14 17:36:01.000000 bot4-0.0.6/bot4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 17:36:01.000000 bot4-0.0.6/bot4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-02-14 17:36:01.000000 bot4-0.0.6/bot4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-02-14 17:36:01.000000 bot4-0.0.6/bot4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-14 17:36:01.700101 bot4-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      852 2024-02-14 17:35:27.000000 bot4-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.757641 bot4-0.0.7/
+-rw-rw-rw-   0        0        0      469 2024-04-28 17:32:20.758639 bot4-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-02-07 15:00:24.000000 bot4-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.569371 bot4-0.0.7/bot4/
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.591570 bot4-0.0.7/bot4/net/
+-rw-rw-rw-   0        0        0        0 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/net/__init__.py
+-rw-rw-rw-   0        0        0      538 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/net/auth.py
+-rw-rw-rw-   0        0        0     4230 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/net/crypto.py
+-rw-rw-rw-   0        0        0     2405 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/pars_packets_name.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.593570 bot4-0.0.7/bot4/protocol/
+-rw-rw-rw-   0        0        0     4400 2024-04-28 16:32:04.000000 bot4-0.0.7/bot4/protocol/protocolbase.py
+-rw-rw-rw-   0        0        0     4803 2024-04-28 17:21:04.000000 bot4-0.0.7/bot4/protocol/protocols.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.615510 bot4-0.0.7/bot4/types/
+-rw-rw-rw-   0        0        0        0 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.748638 bot4-0.0.7/bot4/types/buffer/
+-rw-rw-rw-   0        0        0      683 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/buffer/__init__.py
+-rw-rw-rw-   0        0        0    14300 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/buffer/v1_13.py
+-rw-rw-rw-   0        0        0      921 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/buffer/v1_13_2.py
+-rw-rw-rw-   0        0        0    10350 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/buffer/v1_14.py
+-rw-rw-rw-   0        0        0      779 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/buffer/v1_19.py
+-rw-rw-rw-   0        0        0     2893 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/buffer/v1_19_1.py
+-rw-rw-rw-   0        0        0    14162 2024-04-27 12:42:15.000000 bot4-0.0.7/bot4/types/buffer/v1_7.py
+-rw-rw-rw-   0        0        0     5538 2024-03-05 21:16:25.000000 bot4-0.0.7/bot4/types/buffer/v1_9.py
+-rw-rw-rw-   0        0        0     8623 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/chat.py
+-rw-rw-rw-   0        0        0    14120 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/chunk.py
+-rw-rw-rw-   0        0        0    10828 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/nbt.py
+-rw-rw-rw-   0        0        0     5454 2024-04-27 12:36:41.000000 bot4-0.0.7/bot4/types/registry.py
+-rw-rw-rw-   0        0        0      598 2024-04-05 12:34:59.000000 bot4-0.0.7/bot4/types/settings.py
+-rw-rw-rw-   0        0        0      749 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/types/uuid.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.756639 bot4-0.0.7/bot4/versions/
+-rw-rw-rw-   0        0        0     7816 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/versions/754.json
+-rw-rw-rw-   0        0        0     8474 2024-02-14 17:36:59.000000 bot4-0.0.7/bot4/versions/757.json
+-rw-rw-rw-   0        0        0     5934 2024-04-27 18:25:17.000000 bot4-0.0.7/bot4/versions/packets.py
+-rw-rw-rw-   0        0        0      448 2024-04-27 15:21:04.000000 bot4-0.0.7/bot4/versions/test.py
+-rw-rw-rw-   0        0        0       58 2024-04-21 19:04:13.000000 bot4-0.0.7/bot4/versions/version_protocols.json
+drwxrwxrwx   0        0        0        0 2024-04-28 17:32:20.576373 bot4-0.0.7/bot4.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-04-28 17:32:20.000000 bot4-0.0.7/bot4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-04-28 17:32:20.000000 bot4-0.0.7/bot4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 17:32:20.000000 bot4-0.0.7/bot4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-28 17:32:20.000000 bot4-0.0.7/bot4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 17:32:20.000000 bot4-0.0.7/bot4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 17:32:20.759641 bot4-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      852 2024-04-28 17:29:24.000000 bot4-0.0.7/setup.py
```

### Comparing `bot4-0.0.6/bot4/net/auth.py` & `bot4-0.0.7/bot4/net/auth.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/net/crypto.py` & `bot4-0.0.7/bot4/net/crypto.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/pars_packets_name.py` & `bot4-0.0.7/bot4/pars_packets_name.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/protocol/client.py` & `bot4-0.0.7/bot4/protocol/protocols.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from bot4.protocol.protocol import Protocol, ProtocolError
-from bot4.types.settings import Settings_auth
+from bot4.protocol.protocolbase import PortocolConnect, PortocolBase
 from bot4.types.buffer.v1_19_1 import Buffer1_19_1
-from threading import Barrier
-from bot4.protocol.protocol import create_thread
-from time import sleep
-
-
-class Protocol_auth(Protocol):
-    def __init__(self, settings: Settings_auth):
-        super().__init__(settings)
-        self.profile = settings.profile
-
-    def set_compression(self, byff: Buffer1_19_1):
-        self.compression_threshold = byff.unpack_varint()
-        self.logger.debug(f'set_comression "{self.compression_threshold}"')
-
-    def disconect(self, byff: Buffer1_19_1):
-        self.logger.error(f'Client disconneced; status_client:{self.name_id.state}, massage: {byff.unpack_json()}')
-        self.close()
-
-    def connect(self):
-        self.name_id.state = 0
-        super().connect()
-
-    def setup(self):
-        super().setup()
-        br = Barrier(2)
+import bot4.bot.bots as BB
+import asyncio
 
+
+class ProtocolError(Exception):
+    pass
+
+
+class ProtocolState(PortocolBase):
+    def _run(self):
+        super()._run()
+        raise NotImplementedError('protocol not runing')
+
+
+class ProtocolHandshake(PortocolConnect):
+    state_or_login = 2
+
+    def connection_made(self, transport: asyncio.Transport) -> None:
+        super().connection_made(transport)
         self.send_packet('Handshake',
-                    self.buff_type.pack_varint(754),
-                    self.buff_type.pack_string('mc.prostocraft.ru'),
-                    self.buff_type.pack('H', 25565),
-                    self.buff_type.pack_varint(2))
-        self.name_id.state = 2
-        self.on('Set Compression', self.set_compression)
-        self.on('Disconnect (login)', self.disconect)
-
-        if not self.profile.online:
-            @self.once('Login Success')
-            def success(byff: Buffer1_19_1):
-                self.lock_data_received.clear()
-                self.uuid = byff.unpack_uuid()
-
-                self.name_id.state = 3
-                self.on('Disconnect (play)', self.disconect)
-                self.logger.info(f'Login success "{self.profile.display_name}"')
-                self.lock_data_received.set()
-                br.wait()
+                        self.buff_type.pack_varint(self.bot._name_id.protocol_version),
+                        self.buff_type.pack_string(self.bot.ip),
+                        self.buff_type.pack('H', self.bot.port),
+                        self.buff_type.pack_varint(self.state_or_login)
+                        )
+        self.bot.switch_protocol(self.state_or_login)
+
+
+class ProtocolAuth(PortocolBase):
+    bot: 'BB.BotAuth'
+
+    def __init__(self, bot: 'BB.BotAuth', data_pack, state: int, dispatcher_type):
+        super().__init__(bot, data_pack, state, dispatcher_type)
+
+    async def set_compression(self, byff: Buffer1_19_1):
+        value = byff.unpack_varint()
+        self.bot.compression_threshold = value
+        self.logger.debug(f'Set compression to {value}')
+
+    async def disconect(self, byff: Buffer1_19_1):
+        self.logger.info(f'Disconect in mode {self.state} {byff.unpack_json()}')
+
+    async def success(self, byff: Buffer1_19_1):
+        self.bot.uuid = byff.unpack_uuid()
+        self.logger.info('Client login')
+
+    def _run(self):
+        super()._run()
+        self.dispatcher.on('Disconnect (login)', self.disconect)
+
+        if not self.bot.profile.online:
+            self.dispatcher.once('Set Compression', self.set_compression)
+            
+            def _w(byff: Buffer1_19_1):
+                self.bot.switch_right()
+                return self.success(byff)
+            
+            self.dispatcher.once('Login Success', _w)
+            self.loop.create_task(self.asend_packet('Login Start', self.buff_type.pack_string(self.bot.profile.display_name)))
+        
         else:
-            raise ProtocolError('Online profiles Not supported')
+            raise NotImplementedError('online mode not implemented')
 
-        self.send_packet('Login Start',
-                self.buff_type.pack_string(self.profile.display_name))
-        br.wait()
-
-class Protocol_spawn(Protocol_auth):
-    def __init__(self, settings: Settings_auth):
-        super().__init__(settings)
-        self.position_look_list: list[float] = [0.0, 0.0, 0.0, 0.0, 0.0]
+
+class ProtocolSpawn(PortocolBase):
+    bot: 'BB.BotSpawn'
 
     def flag_to_num(self, flag: int):
         for i in range(5):
             if (flag >> i) == 1:
                 return i
 
-    def position_look(self, buff: Buffer1_19_1):
+    async def update_player_inc(self):
+        while not self.bot.is_close:
+            await asyncio.sleep(1 / 20)
+            await self.asend_packet('Client Status', self.buff_type.pack('?', True))
+
+    async def resource_pack(self, byff: Buffer1_19_1):
+        self.send_packet('Resource Pack Status', b'\x01')
+
+    async def keep_alive(self, buff: Buffer1_19_1):
+            self.send_packet('Keep Alive (serverbound)', buff.read())
+
+    async def set_position_look(self, buff: Buffer1_19_1):
         position = buff.unpack('dddff')
         flag = buff.unpack('B')
 
         for i in range(5):
             if (flag >> i) == 1:
-                self.position_look_list[i] += position[i]
+                self.bot.position_look[i] += position[i]
             else:
-                self.position_look_list[i] = position[i]
+                self.bot.position_look[i] = position[i]
 
         self.send_packet('Teleport Confirm', buff.read())
 
-    def setup(self):
-        super().setup()
-        self.lock_data_received.clear()
-        br = Barrier(2)
-
-        @self.on('Resource Pack Send')
-        def resource(byff: Buffer1_19_1):
-            self.send_packet('Resource Pack Status', b'\x01')
-
-        @self.on('Keep Alive (clientbound)')
-        def keep_alive(buff: Buffer1_19_1):
-            self.send_packet('Keep Alive (serverbound)', buff.read())
-
-        @self.once('Player Position And Look (clientbound)')
-        def positon(buff: Buffer1_19_1):
-            self.position_look(buff)
-            @create_thread(daemon=self.daemon)
-            def update_position_and_look():
-                while not self.is_close:
-                    sleep(1)
-                    self.send_packet(
-                        "Player Position And Rotation (serverbound)",
-                        self.buff_type.pack(
-                            'dddff?',
-                            self.position_look_list[0],
-                            self.position_look_list[1] - 1.62,
-                            self.position_look_list[2],
-                            self.position_look_list[3],
-                            self.position_look_list[4],
-                            True))
-            update_position_and_look()
-
-            self.on('Player Position And Look (clientbound)', self.position_look)
-            br.wait()
-
-        self.lock_data_received.set()
-
-        self.send_packet('Client Settings', b'\x05ru_ru\x10\x00\x01\x7f\x01')
-        self.send_packet('Plugin Message (serverbound)', b'\x0fminecraft:brand\x06fabric')
-
-        @create_thread(daemon=self.daemon)
-        def update_player_inc():
-            while not self.is_close:
-                sleep(1 / 20)
-                self.send_packet('Client Status', b'\x00')
-        update_player_inc()
-        br.wait()
-
+    async def update_position_and_look(self):
+        while not self.bot.is_close:
+            await asyncio.sleep(1)
+            await self.asend_packet(
+                "Player Position And Rotation (serverbound)",
+                self.buff_type.pack(
+                    'dddff?',
+                    self.bot.position_look[0],
+                    self.bot.position_look[1] - 1.62,
+                    self.bot.position_look[2],
+                    self.bot.position_look[3],
+                    self.bot.position_look[4],
+                    True))
+
+    def _run(self):
+        super()._run()
+        self.bot.position_look: list[float] = [0.0, 0.0, 0.0, 0.0, 0.0]
+        self.dispatcher.on('Keep Alive (clientbound)', self.keep_alive)
+        self.loop.create_task(self.update_player_inc())
+        
+        self.dispatcher.once('Resource Pack Send', self.resource_pack)
+
+        @self.dispatcher.once('Player Position And Look (clientbound)')
+        async def _w(byff: Buffer1_19_1):
+            await self.set_position_look(byff)
+            self.dispatcher.on('Player Position And Look (clientbound)', self.set_position_look)
+            self.loop.create_task(self.update_position_and_look())
 
+        self.loop.create_task(self.asend_packet('Client Settings', b'\x05ru_ru\x10\x00\x01\x7f\x01'))
+        self.loop.create_task(self.asend_packet('Plugin Message (serverbound)', b'\x0fminecraft:brand\x06fabric'))
```

### Comparing `bot4-0.0.6/bot4/types/buffer/__init__.py` & `bot4-0.0.7/bot4/types/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_13.py` & `bot4-0.0.7/bot4/types/buffer/v1_13.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_13_2.py` & `bot4-0.0.7/bot4/types/buffer/v1_13_2.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_14.py` & `bot4-0.0.7/bot4/types/buffer/v1_14.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_19.py` & `bot4-0.0.7/bot4/types/buffer/v1_19.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_19_1.py` & `bot4-0.0.7/bot4/types/buffer/v1_19_1.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_7.py` & `bot4-0.0.7/bot4/types/buffer/v1_7.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 import zlib
 
 from bot4.types.buffer import BufferUnderrun
 from bot4.types.registry import OpaqueRegistry
 from bot4.types.uuid import UUID
 
 
-directions = ("down", "up", "north", "south", "west", "east")
-
-
 class Buffer1_7(object):
     buff = b""
     pos = 0
     registry = OpaqueRegistry(13)
 
     def __init__(self, data=None):
         if data:
             self.buff = data
 
     def __len__(self):
         return len(self.buff) - self.pos
 
+    def clear(self):
+        self.buff = b''
+        self.pos = 0
+
+    def copy(self):
+        self2 = self.__class__(self.buff)
+        self2.pos = self.pos
+        return self2
+
     def add(self, data):
         """
         Add some bytes to the end of the buffer.
         """
 
         self.buff += data
 
@@ -142,15 +148,19 @@
         """
         return cls.pack_varint(len(data)) + data
 
     def unpack_byte_array(self):
         """
         Unpack an array of bytes preceded by variant denoting the array length.
         """
-        return self.read(self.unpack_varint())
+        try:
+            return self.read(self.unpack_varint())
+        except BufferUnderrun:
+            self.pos -= 1
+            return self.read()
 
     # Optional ----------------------------------------------------------------
 
     @classmethod
     def pack_optional(cls, packer, val):
         """
         Packs a boolean indicating whether *val* is None. If not,
@@ -484,31 +494,14 @@
                 val = self.unpack('iii')
             elif ty == 7:
                 val = self.unpack_rotation()
             else:
                 raise ValueError(f"Unknown entity metadata type: {ty:d}")
             metadata[ty, key] = val
 
-    # Direction ---------------------------------------------------------------
-
-    @classmethod
-    def pack_direction(cls, direction):
-        """
-        Packs a direction.
-        """
-
-        return cls.pack_varint(directions.index(direction))
-
-    def unpack_direction(self):
-        """
-        Unpacks a direction.
-        """
-
-        return directions[self.unpack_varint()]
-
     # Rotation ----------------------------------------------------------------
 
     @classmethod
     def pack_rotation(cls, x, y, z):
         """
         Packs a rotation.
         """
```

### Comparing `bot4-0.0.6/bot4/types/buffer/v1_9.py` & `bot4-0.0.7/bot4/types/buffer/v1_9.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         return cls.pack_varint(len(palette)) + b"".join(
             cls.pack_varint(x) for x in palette)
 
     @classmethod
     def pack_chunk_section_array(cls, data):
         return cls.pack_varint(len(data) // 8) + data
 
-    def unpack_chunk(self, bitmask, overworld=True):
+    def unpack_chunk(self, bitmask: int, overworld=True):
         sections = []
         for idx in range(16):
             if bitmask & (1 << idx):
                 section = self.unpack_chunk_section(overworld)
             else:
                 section = None
             sections.append(section)
```

### Comparing `bot4-0.0.6/bot4/types/chat.py` & `bot4-0.0.7/bot4/types/chat.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/chunk.py` & `bot4-0.0.7/bot4/types/chunk.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/nbt.py` & `bot4-0.0.7/bot4/types/nbt.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/registry.py` & `bot4-0.0.7/bot4/types/registry.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/types/uuid.py` & `bot4-0.0.7/bot4/types/uuid.py`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/versions/754.json` & `bot4-0.0.7/bot4/versions/754.json`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/bot4/versions/757.json` & `bot4-0.0.7/bot4/versions/757.json`

 * *Files identical despite different names*

### Comparing `bot4-0.0.6/setup.py` & `bot4-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='bot4',
-  version='0.0.6',
+  version='0.0.7',
   author='Jeelesk',
   author_email='eywevynriimnetyiu@gmail.com',
   description='This is a module for creating bots',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Jeelesk/bot4',
   packages=['bot4', 'bot4.net', 'bot4.protocol', 'bot4.types', 'bot4.versions'],
```

