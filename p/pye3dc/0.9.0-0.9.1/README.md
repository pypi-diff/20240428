# Comparing `tmp/pye3dc-0.9.0.tar.gz` & `tmp/pye3dc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pye3dc-0.9.0.tar", last modified: Mon Nov 13 18:04:19 2023, max compression
+gzip compressed data, was "pye3dc-0.9.1.tar", last modified: Thu Mar 21 09:07:02 2024, max compression
```

## Comparing `pye3dc-0.9.0.tar` & `pye3dc-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:04:19.916536 pye3dc-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-11-13 18:04:13.000000 pye3dc-0.9.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-11-13 18:04:13.000000 pye3dc-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2023-11-13 18:04:19.916536 pye3dc-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2023-11-13 18:04:13.000000 pye3dc-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:04:19.912536 pye3dc-0.9.0/e3dc/
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/_RSCPEncryptDecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89017 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/_e3dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/_e3dc_rscp_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    15824 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/_e3dc_rscp_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/_rscpLib.py
--rw-r--r--   0 runner    (1001) docker     (127)   154532 2023-11-13 18:04:13.000000 pye3dc-0.9.0/e3dc/_rscpTags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:04:19.916536 pye3dc-0.9.0/pye3dc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2023-11-13 18:04:19.000000 pye3dc-0.9.0/pye3dc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-11-13 18:04:19.000000 pye3dc-0.9.0/pye3dc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 18:04:19.000000 pye3dc-0.9.0/pye3dc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-13 18:04:19.000000 pye3dc-0.9.0/pye3dc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-13 18:04:19.000000 pye3dc-0.9.0/pye3dc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-11-13 18:04:13.000000 pye3dc-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 18:04:19.916536 pye3dc-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:07:02.606291 pye3dc-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-21 09:06:59.000000 pye3dc-0.9.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-21 09:06:59.000000 pye3dc-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-03-21 09:07:02.606291 pye3dc-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-03-21 09:06:59.000000 pye3dc-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:07:02.602291 pye3dc-0.9.1/e3dc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/_RSCPEncryptDecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89070 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/_e3dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/_e3dc_rscp_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/_e3dc_rscp_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/_rscpLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154532 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/_rscpTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:06:59.000000 pye3dc-0.9.1/e3dc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:07:02.606291 pye3dc-0.9.1/pye3dc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-03-21 09:07:02.000000 pye3dc-0.9.1/pye3dc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-21 09:07:02.000000 pye3dc-0.9.1/pye3dc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:07:02.000000 pye3dc-0.9.1/pye3dc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-21 09:07:02.000000 pye3dc-0.9.1/pye3dc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-21 09:07:02.000000 pye3dc-0.9.1/pye3dc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-21 09:06:59.000000 pye3dc-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 09:07:02.606291 pye3dc-0.9.1/setup.cfg
```

### Comparing `pye3dc-0.9.0/LICENSE` & `pye3dc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pye3dc-0.9.0/PKG-INFO` & `pye3dc-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pye3dc
-Version: 0.9.0
+Version: 0.9.1
 Summary: E3/DC client for python
 Author-email: Francesco Santini <francesco.santini@gmail.com>, Christopher Banck <christopher@banck.net>
 License: MIT
 Project-URL: Documentation, https://python-e3dc.readthedocs.io
 Project-URL: Repository, https://github.com/fsantini/python-e3dc
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `pye3dc-0.9.0/README.md` & `pye3dc-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pye3dc-0.9.0/e3dc/_RSCPEncryptDecrypt.py` & `pye3dc-0.9.1/e3dc/_RSCPEncryptDecrypt.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.9.0/e3dc/__init__.py` & `pye3dc-0.9.1/e3dc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     "RSCPAuthenticationError",
     "RSCPKeyError",
     "RequestTimeoutError",
     "SocketNotReady",
     "FrameError",
     "set_rscp_debug",
 ]
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `pye3dc-0.9.0/e3dc/_e3dc.py` & `pye3dc-0.9.1/e3dc/_e3dc.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,17 +314,15 @@
 
         outObj = {
             "autarky": autarky,
             "consumption": {"battery": bat, "house": home, "wallbox": wb},
             "production": {"solar": solar, "add": -add, "grid": grid},
             "selfConsumption": sc,
             "stateOfCharge": soc,
-            "time": datetime.datetime.utcfromtimestamp(ts).replace(
-                tzinfo=datetime.timezone.utc
-            ),
+            "time": datetime.datetime.fromtimestamp(ts, tz=datetime.timezone.utc),
         }
 
         self.lastRequest = outObj
         self.lastRequestTime = time.time()
         return outObj
 
     def poll_switches(self, keepAlive: bool = False):
@@ -389,23 +387,21 @@
             value (str): value
             keepAlive (bool): True to keep connection alive. Defaults to False.
 
         Returns:
             True/False
 
         """
-        cmd = "on" if value else "off"
-
         result = self.sendRequest(
             (
                 RscpTag.HA_REQ_COMMAND_ACTUATOR,
                 RscpType.Container,
                 [
                     (RscpTag.HA_DATAPOINT_INDEX, RscpType.Uint16, switchID),
-                    (RscpTag.HA_REQ_COMMAND, RscpType.CString, cmd),
+                    (RscpTag.HA_REQ_COMMAND, RscpType.CString, value),
                 ],
             ),
             keepAlive=keepAlive,
         )
 
         if result[0] == RscpTag.HA_COMMAND_ACTUATOR and result[2]:
             return True
@@ -1243,17 +1239,17 @@
                             RscpTag.BAT_REQ_DCB_ALL_CELL_VOLTAGES,
                             RscpType.Uint16,
                             dcb,
                         ),
                         (RscpTag.BAT_REQ_DCB_INFO, RscpType.Uint16, dcb),
                     ],
                 ),
-                keepAlive=True
-                if dcb != dcbs[-1]
-                else keepAlive,  # last request should honor keepAlive
+                keepAlive=(
+                    True if dcb != dcbs[-1] else keepAlive
+                ),  # last request should honor keepAlive
             )
 
             info = rscpFindTag(req, RscpTag.BAT_DCB_INFO)
             # For some devices, no info for the DCBs exists. Skip those.
             if info is None or len(info) < 3 or info[1] == "Error":
                 continue
 
@@ -1377,17 +1373,19 @@
                 dcbs = list(range(0, battery["dcbs"]))
             else:
                 dcbs = None
             outObj.append(
                 self.get_battery_data(
                     batIndex=battery["index"],
                     dcbs=dcbs,
-                    keepAlive=True
-                    if battery["index"] != batteries[-1]["index"]
-                    else keepAlive,  # last request should honor keepAlive
+                    keepAlive=(
+                        True
+                        if battery["index"] != batteries[-1]["index"]
+                        else keepAlive
+                    ),  # last request should honor keepAlive
                 )
             )
 
         return outObj
 
     def get_pvis(self, keepAlive: bool = False):
         """Scans for installed pvis via rscp protocol.
@@ -1712,17 +1710,17 @@
                         (
                             RscpTag.PVI_REQ_DC_STRING_ENERGY_ALL,
                             RscpType.Uint16,
                             string,
                         ),
                     ],
                 ),
-                keepAlive=True
-                if string != strings[-1]
-                else keepAlive,  # last request should honor keepAlive
+                keepAlive=(
+                    True if string != strings[-1] else keepAlive
+                ),  # last request should honor keepAlive
             )
             stringobj = {
                 "power": rscpFindTagIndex(
                     rscpFindTag(req, RscpTag.PVI_DC_POWER), RscpTag.PVI_VALUE
                 ),
                 "voltage": rscpFindTagIndex(
                     rscpFindTag(req, RscpTag.PVI_DC_VOLTAGE), RscpTag.PVI_VALUE
@@ -1767,17 +1765,17 @@
                 phases = None
 
             outObj.append(
                 self.get_pvi_data(
                     pviIndex=pvi["index"],
                     strings=strings,
                     phases=phases,
-                    keepAlive=True
-                    if pvi["index"] != pvis[-1]["index"]
-                    else keepAlive,  # last request should honor keepAlive
+                    keepAlive=(
+                        True if pvi["index"] != pvis[-1]["index"] else keepAlive
+                    ),  # last request should honor keepAlive
                 )
             )
 
         return outObj
 
     def get_powermeters(self, keepAlive: bool = False):
         """Scans for installed power meters via rscp protocol.
@@ -1927,17 +1925,19 @@
 
         outObj: List[Dict[str, Any]] = []
 
         for powermeter in powermeters:
             outObj.append(
                 self.get_powermeter_data(
                     pmIndex=powermeter["index"],
-                    keepAlive=True
-                    if powermeter["index"] != powermeters[-1]["index"]
-                    else keepAlive,  # last request should honor keepAlive
+                    keepAlive=(
+                        True
+                        if powermeter["index"] != powermeters[-1]["index"]
+                        else keepAlive
+                    ),  # last request should honor keepAlive
                 )
             )
 
         return outObj
 
     def get_power_settings(self, keepAlive: bool = False):
         """Polls the power settings via rscp protocol.
```

### Comparing `pye3dc-0.9.0/e3dc/_e3dc_rscp_local.py` & `pye3dc-0.9.1/e3dc/_e3dc_rscp_local.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.9.0/e3dc/_e3dc_rscp_web.py` & `pye3dc-0.9.1/e3dc/_e3dc_rscp_web.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import hashlib
 import struct
 import threading
 import time
 from typing import Any, Callable, Tuple
 
 import tzlocal
-from websocket import ABNF, WebSocketApp  # pyright: ignore [reportMissingTypeStubs]
+from websocket import ABNF, WebSocketApp  # pyright: ignore [reportPrivateImportUsage]
 
 from ._rscpLib import (
     rscpDecode,
     rscpEncode,
     rscpFindTag,
     rscpFindTagIndex,
     rscpFrame,
@@ -43,15 +43,15 @@
  Communication is through SERVER_REQ_RSCP_CMD which is a container with:
  virtConId, virtAuthLevel, innerFrame
  
  and the innerframe is an RSCP frame with the appropriate command (HA_REQ_ACTUATOR_STATES for example)
  
 """
 
-REMOTE_ADDRESS = "wss://s10.e3dc.com/ws/"
+REMOTE_ADDRESS = "wss://s10.e3dc.com/ws"
 
 
 class SocketNotReady(Exception):
     """Class for Socket Not Ready Exception."""
 
     pass
 
@@ -116,19 +116,17 @@
             self.password = password
         else:
             self.password = hashlib.md5(bytes(password, "UTF-8")).hexdigest()
 
         self.serialNumberWithPrefix = serialNumberWithPrefix.encode("utf-8")
         self.ws = WebSocketApp(
             REMOTE_ADDRESS,
-            on_message=lambda _, msg: self.on_message(  # pyright: ignore [reportUnknownLambdaType]
-                msg  # pyright: ignore [reportUnknownArgumentType]
-            ),
-            on_close=lambda _: self.reset(),  # pyright: ignore [reportUnknownLambdaType]
-            on_error=lambda _: self.reset(),  # pyright: ignore [reportUnknownLambdaType]
+            on_message=lambda _, msg: self.on_message(msg),
+            on_close=lambda _ws, _, __: self.reset(),
+            on_error=lambda _ws, _: self.reset(),
         )
         self.reset()
 
     def reset(self):
         """Method to reset E3DC rscp web instance."""
         self.ws.close()  # pyright: ignore [reportUnknownMemberType]
         self.conId: int = 0
@@ -159,17 +157,15 @@
                     (RscpTag.SERVER_TYPE, RscpType.Int32, 4),
                     (RscpTag.SERVER_HASH_CODE, RscpType.Int32, 1234567890),
                 ],
             )
         )
 
         # print("--------------------- Sending virtual conn")
-        self.ws.send(
-            virtualConn, ABNF.OPCODE_BINARY  # pyright: ignore [reportGeneralTypeIssues]
-        )
+        self.ws.send(virtualConn, ABNF.OPCODE_BINARY)
 
     def respondToINFORequest(
         self, decoded: Tuple[str | int | RscpTag, str | int | RscpType, Any]
     ):
         """Create Response to INFO request."""
         TIMEZONE_STR, utcDiffS = calcTimeZone()
 
@@ -251,17 +247,15 @@
                 RscpType.Container,
                 [
                     rscpFindTag(decodedMsg, RscpTag.SERVER_CONNECTION_ID),
                     rscpFindTag(decodedMsg, RscpTag.SERVER_AUTH_LEVEL),
                 ],
             )
         )
-        self.ws.send(
-            reply, ABNF.OPCODE_BINARY  # pyright: ignore [reportGeneralTypeIssues]
-        )
+        self.ws.send(reply, ABNF.OPCODE_BINARY)
 
     def on_message(self, message: bytes):
         """Method to handle a received message."""
         # print "Received message", message
         if len(message) == 0:
             return
 
@@ -274,15 +268,15 @@
 
         # print "Decoded received message", decodedMsg
         if tag == RscpTag.SERVER_REQ_PING:
             pingFrame = rscpFrame(
                 rscpEncode(RscpTag.SERVER_PING, RscpType.NoneType, None)
             )
             self.ws.send(
-                pingFrame,  # pyright: ignore [reportGeneralTypeIssues]
+                pingFrame,
                 ABNF.OPCODE_BINARY,
             )
             return
         elif tag == RscpTag.SERVER_REGISTER_CONNECTION:
             self.registerConnectionHandler(decodedMsg)
         elif tag == RscpTag.SERVER_UNREGISTER_CONNECTION:
             # this signifies some error
@@ -324,17 +318,15 @@
                     (RscpTag.SERVER_AUTH_LEVEL, RscpType.UChar8, self.authLevel),
                     (RscpTag.SERVER_RSCP_DATA_LEN, RscpType.Int32, len(innerFrame)),
                     (RscpTag.SERVER_RSCP_DATA, RscpType.ByteArray, innerFrame),
                 ],
             )
 
             self.ws.send(
-                rscpFrame(
-                    responseContainer
-                ),  # pyright: ignore [reportGeneralTypeIssues]
+                rscpFrame(responseContainer),
                 ABNF.OPCODE_BINARY,
             )
 
     def _defaultRequestCallback(
         self, msg: Tuple[str | int | RscpTag, str | int | RscpType, Any]
     ):
         self.requestResult = msg
@@ -358,18 +350,18 @@
     ):
         """Send a command."""
         return self._sendRequest_internal(rscpFrame(rscpEncode(message)))
 
     def _sendRequest_internal(
         self,
         innerFrame: bytes | Tuple[str | int | RscpTag, str | int | RscpType, Any],
-        callback: Callable[
-            [Tuple[str | int | RscpTag, str | int | RscpType, Any]], None
-        ]
-        | None = None,
+        callback: (
+            Callable[[Tuple[str | int | RscpTag, str | int | RscpType, Any]], None]
+            | None
+        ) = None,
     ):
         """Internal send request method.
 
         Args:
             innerFrame (Union[tuple, <RSCP encoded frame>]): inner frame
             callback (str): callback method
             synchronous (bool): If True, the method waits for a response (i.e. exits after calling callback).
@@ -402,17 +394,15 @@
                     ),
                     (RscpTag.SERVER_RSCP_DATA_LEN, RscpType.Int32, len(innerFrame)),
                     (RscpTag.SERVER_RSCP_DATA, RscpType.ByteArray, innerFrame),
                 ],
             )
         )
 
-        self.ws.send(
-            outerFrame, ABNF.OPCODE_BINARY  # pyright: ignore [reportGeneralTypeIssues]
-        )
+        self.ws.send(outerFrame, ABNF.OPCODE_BINARY)
 
     def connect(self):
         """Connect to E3DC system."""
         self.reset()
         self.thread = threading.Thread(
             target=self.ws.run_forever  # pyright: ignore [reportUnknownMemberType, reportUnknownArgumentType]
         )
```

### Comparing `pye3dc-0.9.0/e3dc/_rscpLib.py` & `pye3dc-0.9.1/e3dc/_rscpLib.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,17 @@
         return None
 
     if decodedMsg is None:
         return None
     if decodedMsg[0] == tagStr:
         return decodedMsg
     if isinstance(decodedMsg[2], list):
-        msgList: List[
-            Tuple[str | int | RscpTag, str | int | RscpType, Any]
-        ] = decodedMsg[2]
+        msgList: List[Tuple[str | int | RscpTag, str | int | RscpType, Any]] = (
+            decodedMsg[2]
+        )
         for msg in msgList:
             msgValue = rscpFindTag(msg, tag)
             if msgValue is not None:
                 return msgValue
     return None
```

### Comparing `pye3dc-0.9.0/e3dc/_rscpTags.py` & `pye3dc-0.9.1/e3dc/_rscpTags.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.9.0/pye3dc.egg-info/PKG-INFO` & `pye3dc-0.9.1/pye3dc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pye3dc
-Version: 0.9.0
+Version: 0.9.1
 Summary: E3/DC client for python
 Author-email: Francesco Santini <francesco.santini@gmail.com>, Christopher Banck <christopher@banck.net>
 License: MIT
 Project-URL: Documentation, https://python-e3dc.readthedocs.io
 Project-URL: Repository, https://github.com/fsantini/python-e3dc
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `pye3dc-0.9.0/pyproject.toml` & `pye3dc-0.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 [project.urls]
 Documentation = "https://python-e3dc.readthedocs.io"
 Repository = "https://github.com/fsantini/python-e3dc"
 
 [tool.setuptools]
 packages = ["e3dc"]
 
+[tool.setuptools.package-data]
+"*" = ["py.typed"]
+
 [tool.setuptools.dynamic]
 version = {attr = "e3dc.__version__"}
 
 [tool.black]
 target-version = ['py38','py39','py310','py311','py312']
 include = '\.pyi?$'
 exclude = '''
```

