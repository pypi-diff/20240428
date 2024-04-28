# Comparing `tmp/PieRakNet-1.0.6.tar.gz` & `tmp/pieraknet-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PieRakNet-1.0.6.tar", last modified: Sun Sep  3 13:59:38 2023, max compression
+gzip compressed data, was "pieraknet-1.0.7.tar", last modified: Sun Apr 28 12:31:35 2024, max compression
```

## Comparing `PieRakNet-1.0.6.tar` & `pieraknet-1.0.7.tar`

### file list

```diff
@@ -1,43 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:38.627271 PieRakNet-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (999)    35149 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     4989 2023-09-03 13:59:38.627271 PieRakNet-1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:38.623271 PieRakNet-1.0.6/PieRakNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4989 2023-09-03 13:59:38.000000 PieRakNet-1.0.6/PieRakNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1194 2023-09-03 13:59:38.000000 PieRakNet-1.0.6/PieRakNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 13:59:38.000000 PieRakNet-1.0.6/PieRakNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       10 2023-09-03 13:59:38.000000 PieRakNet-1.0.6/PieRakNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     4100 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:38.623271 PieRakNet-1.0.6/pieraknet/
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5585 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/buffer.py
--rw-r--r--   0 runner    (1001) docker     (999)    10799 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:38.627271 PieRakNet-1.0.6/pieraknet/handlers/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      716 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/handlers/connection_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     1606 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/handlers/offline_ping.py
--rw-r--r--   0 runner    (1001) docker     (999)      459 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/handlers/online_ping.py
--rw-r--r--   0 runner    (1001) docker     (999)     2613 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/handlers/open_connection_request_1.py
--rw-r--r--   0 runner    (1001) docker     (999)     1917 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/handlers/open_connection_request_2.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:38.627271 PieRakNet-1.0.6/pieraknet/packets/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2493 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/acknowledgement.py
--rw-r--r--   0 runner    (1001) docker     (999)      445 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/connection_request.py
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/connection_request_accepted.py
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (999)     3333 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/frame_set.py
--rw-r--r--   0 runner    (1001) docker     (999)      834 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/game_packet.py
--rw-r--r--   0 runner    (1001) docker     (999)      388 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/incompatible_protocol.py
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/new_incoming_connection.py
--rw-r--r--   0 runner    (1001) docker     (999)      376 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/offline_ping.py
--rw-r--r--   0 runner    (1001) docker     (999)      701 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/offline_pong.py
--rw-r--r--   0 runner    (1001) docker     (999)      317 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/online_ping.py
--rw-r--r--   0 runner    (1001) docker     (999)      446 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/online_pong.py
--rw-r--r--   0 runner    (1001) docker     (999)      470 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/open_connection_reply_1.py
--rw-r--r--   0 runner    (1001) docker     (999)      593 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/open_connection_reply_2.py
--rw-r--r--   0 runner    (1001) docker     (999)      404 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/open_connection_request_1.py
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/open_connection_request_2.py
--rw-r--r--   0 runner    (1001) docker     (999)      526 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/packets/packet.py
--rw-r--r--   0 runner    (1001) docker     (999)      587 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/protocol_info.py
--rw-r--r--   0 runner    (1001) docker     (999)     3612 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/pieraknet/server.py
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-03 13:59:38.627271 PieRakNet-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1162 2023-09-03 13:59:27.000000 PieRakNet-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:35.974782 pieraknet-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 12:31:31.000000 pieraknet-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-28 12:31:35.974782 pieraknet-1.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:35.974782 pieraknet-1.0.7/PieRakNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-28 12:31:31.000000 pieraknet-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:31:35.974782 pieraknet-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-28 12:31:31.000000 pieraknet-1.0.7/setup.py
```

### Comparing `PieRakNet-1.0.6/LICENSE` & `pieraknet-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.6/PKG-INFO` & `pieraknet-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.6
+Version: 1.0.7
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: PieMC.Developers@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.6/PieRakNet.egg-info/PKG-INFO` & `pieraknet-1.0.7/PieRakNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.6
+Version: 1.0.7
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: PieMC.Developers@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.6/README.md` & `pieraknet-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.6/setup.py` & `pieraknet-1.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 
 def readme():
-    with open('README.md', 'r') as f:
+    with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='PieRakNet',
-    version='1.0.6',
+    version='1.0.7',
     author='lapismyt',
     author_email='PieMC.Developers@gmail.com',
     description='RakNet implementation, written in Python. Created for PieMC.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PieMC-Dev/PieRakNet',
     packages=find_packages(),
```

