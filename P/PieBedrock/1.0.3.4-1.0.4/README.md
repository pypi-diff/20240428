# Comparing `tmp/PieBedrock-1.0.3.4.tar.gz` & `tmp/piebedrock-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PieBedrock-1.0.3.4.tar", last modified: Fri Dec 22 12:29:37 2023, max compression
+gzip compressed data, was "piebedrock-1.0.4.tar", last modified: Sun Apr 28 12:34:44 2024, max compression
```

## Comparing `PieBedrock-1.0.3.4.tar` & `piebedrock-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:29:37.374149 PieBedrock-1.0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-22 12:29:37.374149 PieBedrock-1.0.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:29:37.374149 PieBedrock-1.0.3.4/PieBedrock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-22 12:29:37.000000 PieBedrock-1.0.3.4/PieBedrock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-12-22 12:29:37.000000 PieBedrock-1.0.3.4/PieBedrock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 12:29:37.000000 PieBedrock-1.0.3.4/PieBedrock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 12:29:37.000000 PieBedrock-1.0.3.4/PieBedrock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-22 12:29:37.000000 PieBedrock-1.0.3.4/PieBedrock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:29:37.374149 PieBedrock-1.0.3.4/piebedrock/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/jwt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:29:37.374149 PieBedrock-1.0.3.4/piebedrock/packets/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/play_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/resource_packs_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/packets/server_client_handshake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/server.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/piebedrock/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 12:29:37.374149 PieBedrock-1.0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-12-22 12:29:27.000000 PieBedrock-1.0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:34:44.181915 piebedrock-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-28 12:34:38.000000 piebedrock-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-28 12:34:44.181915 piebedrock-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:34:44.181915 piebedrock-1.0.4/PieBedrock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-28 12:34:44.000000 piebedrock-1.0.4/PieBedrock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-28 12:34:44.000000 piebedrock-1.0.4/PieBedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:34:44.000000 piebedrock-1.0.4/PieBedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 12:34:44.000000 piebedrock-1.0.4/PieBedrock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 12:34:44.000000 piebedrock-1.0.4/PieBedrock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 12:34:38.000000 piebedrock-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:34:44.181915 piebedrock-1.0.4/piebedrock/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:34:44.181915 piebedrock-1.0.4/piebedrock/packets/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/play_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/resource_packs_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/packets/server_client_handshake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:34:38.000000 piebedrock-1.0.4/piebedrock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:34:44.181915 piebedrock-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-28 12:34:38.000000 piebedrock-1.0.4/setup.py
```

### Comparing `PieBedrock-1.0.3.4/PKG-INFO` & `piebedrock-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieBedrock
-Version: 1.0.3.4
+Version: 1.0.4
 Summary: Minecraft: Bedrock Edition network protocol implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieBedrock
 Author: lapismyt
 Author-email: PieMC.Developers@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieBedrock/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet piebedrock bedrock-protocol mineceaft-bedrock network protocol
```

### Comparing `PieBedrock-1.0.3.4/PieBedrock.egg-info/PKG-INFO` & `piebedrock-1.0.4/PieBedrock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieBedrock
-Version: 1.0.3.4
+Version: 1.0.4
 Summary: Minecraft: Bedrock Edition network protocol implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieBedrock
 Author: lapismyt
 Author-email: PieMC.Developers@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieBedrock/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet piebedrock bedrock-protocol mineceaft-bedrock network protocol
```

### Comparing `PieBedrock-1.0.3.4/PieBedrock.egg-info/SOURCES.txt` & `piebedrock-1.0.4/PieBedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/buffer.py` & `piebedrock-1.0.4/piebedrock/buffer.py`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/const.py` & `piebedrock-1.0.4/piebedrock/const.py`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/packets/disconnect.py` & `piebedrock-1.0.4/piebedrock/packets/disconnect.py`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/packets/packet.py` & `piebedrock-1.0.4/piebedrock/packets/packet.py`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/packets/play_status.py` & `piebedrock-1.0.4/piebedrock/packets/play_status.py`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/packets/resource_packs_info.py` & `piebedrock-1.0.4/piebedrock/packets/resource_packs_info.py`

 * *Files identical despite different names*

### Comparing `PieBedrock-1.0.3.4/piebedrock/server.py` & `piebedrock-1.0.4/piebedrock/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,81 @@
 import threading
-from pieraknet import Server as PieRakNet
+from pieraknet.server import Server as PieRakNet
 from pieraknet.packets.game_packet import GamePacket
 from pieraknet.connection import Connection as RakNetConnection
 from pieraknet.packets.frame_set import Frame
 
 import logging
 import os
 import time
 import random
 
 class BedrockServer:
-    def __init__(self, hostname="0.0.0.0", port=19132, logger=logging.getLogger("PieBedrock"), gamemode="survival", timeout=20, dev_mode=False):
+    def __init__(self, hostname="0.0.0.0", port=19132, logger=None, gamemode="survival", timeout=20, logginglevel="DEBUG", dev_mode=False):
+        if logger is None:
+            logger = logging.getLogger("PieBedrock")
+            logger.setLevel(getattr(logging, logginglevel.upper()))
+            formatter = logging.Formatter('%(asctime)s [%(name)s - %(levelname)s] - %(message)s', "%H:%M:%S")
+            handler = logging.StreamHandler()
+            handler.setFormatter(formatter)
+            logger.addHandler(handler)
         self.initialized = False
         self.logger = logger
         self.server_status = None
         self.hostname = hostname
         self.port = port
         self.edition = "MCPE"
         self.protocol_version = 594
         self.version_name = "1.20.12"
-        self.motd1 = "PieBedrock Server"
-        self.motd2 = "GitHub/@PieMC-Dev"
+        self.name = "PieBedrock Server"
+        self.motd = "GitHub/@PieMC-Dev"
         self.players_online = 0
         self.max_players = 20
         self.gamemode_map = {
-            "survival": ("Survival", 1),
-            "creative": ("Creative", 2),
-            "adventure": ("Adventure", 3)
+        "survival": 1,
+        "creative": 2,
+        "adventure": 3
         }
-        self.gamemode = self.gamemode_map.get(gamemode, ("Survival", 0))
+        self.gamemode = gamemode.lower().capitalize()
+        self.gamemodeId = self.gamemode_map.get(self.gamemode.lower(), None)
         self.port_v6 = 19131
         self.guid = random.randint(1, 99999999)
         self.uid = random.randint(1, 99999999)
         self.raknet_version = 11
         self.timeout = timeout
         self.running = False
         self.start_time = int(time.time())
         self.pieraknet_thread = None
         self.dev_mode = dev_mode
 
     def pieraknet_init(self):
-        if self.dev_mode:
-            logging.getLogger("PierakNet").setLevel(logging.DEBUG)
-            logging.getLogger("PierakNet").addHandler(logging.StreamHandler())
-        self.pieraknet = PieRakNet(self.hostname, self.port, logging.getLogger("PierakNet"))
         self.update_server_status()
-        self.pieraknet.protocol_version = self.raknet_version
+        self.pieraknet = PieRakNet(self.hostname, self.port, responseData=self.server_status)
         self.pieraknet.timeout = self.timeout
         self.initialized = True
 
-    def start_pieraknet_thread(self):
-        self.pieraknet_thread = threading.Thread(target=self.pieraknet.start)
-        self.pieraknet_thread.daemon = True
-        self.pieraknet_thread.start()
-
     def get_time_ms(self):
         return round(time.time() - self.start_time, 3)
 
     def update_server_status(self):
         self.server_status = ";".join([
             self.edition,
-            self.motd1,
+            self.name,
             f"{self.protocol_version}",
             self.version_name,
             f"{self.players_online}",
             f"{self.max_players}",
             f"{self.uid}",
-            self.motd2,
-            self.gamemode[0],
-            f"{self.gamemode[1]}",
+            self.motd,
+            self.gamemode.lower().capitalize(),
+            f"{self.gamemodeId}",
             f"{self.port}",
             f"{self.port_v6}"
         ]) + ";"
-        self.pieraknet.name = self.server_status
+        self.server_status
 
     def on_game_packet(self, packet: GamePacket, connection: RakNetConnection):
         packet.decode()
         if packet.body[0] == 0x01:
             self.logger.info(f"New Login Packet: {str(packet.body)}")
 
     def on_new_incoming_connection(self, connection: RakNetConnection):
@@ -87,17 +86,17 @@
 
     def on_unknown_packet(self, packet: Frame, connection: RakNetConnection):
         self.logger.info(f"New Unknown Packet: {str(packet.body)}")
 
     def start(self):
         if not self.initialized:
             self.pieraknet_init()
-        self.start_pieraknet_thread()
         self.running = True
         self.logger.info(f"Running on {self.hostname}:{str(self.port)} ({str(self.get_time_ms())}s).")
+        self.pieraknet.start()
 
     def stop(self):
         self.logger.info("Stopping...")
         self.running = False
         if self.pieraknet_thread:
             self.pieraknet.stop()
             self.pieraknet_thread.join()
```

### Comparing `PieBedrock-1.0.3.4/setup.py` & `piebedrock-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='PieBedrock',
-    version='1.0.3.4',
+    version='1.0.4',
     author='lapismyt',
     author_email='PieMC.Developers@gmail.com',
     description='Minecraft: Bedrock Edition network protocol implementation, written in Python. Created for PieMC.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PieMC-Dev/PieBedrock',
     packages=find_packages(),
```

