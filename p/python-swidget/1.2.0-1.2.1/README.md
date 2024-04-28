# Comparing `tmp/python_swidget-1.2.0.tar.gz` & `tmp/python_swidget-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_swidget-1.2.0.tar", max compression
+gzip compressed data, was "python_swidget-1.2.1.tar", max compression
```

## Comparing `python_swidget-1.2.0.tar` & `python_swidget-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      539 2024-04-10 14:24:43.925014 python_swidget-1.2.0/README.md
--rw-r--r--   0        0        0     2179 2024-04-26 14:40:32.968055 python_swidget-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1330 2024-04-10 14:24:43.935014 python_swidget-1.2.0/swidget/__init__.py
--rw-r--r--   0        0        0     8951 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/cli.py
--rw-r--r--   0        0        0     3865 2024-04-14 18:19:53.397240 python_swidget-1.2.0/swidget/discovery.py
--rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.2.0/swidget/exceptions.py
--rw-r--r--   0        0        0     4591 2024-04-10 14:24:43.935014 python_swidget-1.2.0/swidget/provision.py
--rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.2.0/swidget/py.typed
--rw-r--r--   0        0        0    22143 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/swidgetdevice.py
--rw-r--r--   0        0        0     1969 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/swidgetdimmer.py
--rw-r--r--   0        0        0      402 2024-04-10 14:24:43.935014 python_swidget-1.2.0/swidget/swidgetoutlet.py
--rw-r--r--   0        0        0      402 2024-04-14 18:19:53.397240 python_swidget-1.2.0/swidget/swidgetswitch.py
--rw-r--r--   0        0        0      820 2024-04-14 18:19:53.397240 python_swidget-1.2.0/swidget/swidgettimerswitch.py
--rw-r--r--   0        0        0     5774 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/websocket.py
--rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 python_swidget-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      539 2024-04-10 14:24:43.925014 python_swidget-1.2.1/README.md
+-rw-r--r--   0        0        0     2179 2024-04-28 21:51:16.110837 python_swidget-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1330 2024-04-10 14:24:43.935014 python_swidget-1.2.1/swidget/__init__.py
+-rw-r--r--   0        0        0     8951 2024-04-26 14:40:11.998055 python_swidget-1.2.1/swidget/cli.py
+-rw-r--r--   0        0        0     3865 2024-04-14 18:19:53.397240 python_swidget-1.2.1/swidget/discovery.py
+-rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.2.1/swidget/exceptions.py
+-rw-r--r--   0        0        0     4591 2024-04-10 14:24:43.935014 python_swidget-1.2.1/swidget/provision.py
+-rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.2.1/swidget/py.typed
+-rw-r--r--   0        0        0    21885 2024-04-28 21:51:16.110837 python_swidget-1.2.1/swidget/swidgetdevice.py
+-rw-r--r--   0        0        0     1969 2024-04-26 14:40:11.998055 python_swidget-1.2.1/swidget/swidgetdimmer.py
+-rw-r--r--   0        0        0      402 2024-04-10 14:24:43.935014 python_swidget-1.2.1/swidget/swidgetoutlet.py
+-rw-r--r--   0        0        0      402 2024-04-14 18:19:53.397240 python_swidget-1.2.1/swidget/swidgetswitch.py
+-rw-r--r--   0        0        0      820 2024-04-14 18:19:53.397240 python_swidget-1.2.1/swidget/swidgettimerswitch.py
+-rw-r--r--   0        0        0     5768 2024-04-28 21:51:16.110837 python_swidget-1.2.1/swidget/websocket.py
+-rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 python_swidget-1.2.1/PKG-INFO
```

### Comparing `python_swidget-1.2.0/README.md` & `python_swidget-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/pyproject.toml` & `python_swidget-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-swidget"
-version = "1.2.0"
+version = "1.2.1"
 description = "Python API for Swidget smart devices"
 license = "GPL-3.0-or-later"
 authors = ["Swidget"]
 repository = "https://github.com/swidget/python-swidget"
 readme = "README.md"
 packages = [
   { include = "swidget" }
```

### Comparing `python_swidget-1.2.0/swidget/__init__.py` & `python_swidget-1.2.1/swidget/__init__.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/swidget/cli.py` & `python_swidget-1.2.1/swidget/cli.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/swidget/discovery.py` & `python_swidget-1.2.1/swidget/discovery.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/swidget/provision.py` & `python_swidget-1.2.1/swidget/provision.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/swidget/swidgetdevice.py` & `python_swidget-1.2.1/swidget/swidgetdevice.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.use_https = use_https
         self.uri_scheme = 'https' if self.use_https is True else 'http'
         self.secret_key = secret_key
         self.use_websockets = use_websockets
         self.device_type = DeviceType.Unknown
         self._friendly_name = "Unknown Swidget Device"
         self.assemblies: Dict[Any, Any] = dict()
-        self._subscribers: Callable[[Dict[str, Any]], Any] = list()
+        self._subscribers: List[Any] = list()
         headers = {self.token_name: self.secret_key,
                    'Connection': 'keep-alive'}
         connector = TCPConnector(verify_ssl=False, force_close=True)
         self._session = ClientSession(headers=headers, connector=connector)
         self._last_update: int = 0
         if self.use_websockets:
             self._websocket = SwidgetWebsocket(
@@ -109,23 +109,26 @@
         if hasattr(self, '_websocket'):
             await self._websocket.close()
         await self._session.close()
 
     async def close(self) -> None:
         await self.stop()
 
-    async def add_event_callback(self, callback: Callable[[Dict, Any], None],) -> bool:
+    async def disconnect(self) -> None:
+        await self.stop()
+
+    def add_event_callback(self, callback: Callable[[Dict, Any], None],) -> bool:
         for c in self._subscribers:
             if c == callback:
                 _LOGGER.warn(f"Callback has already been added, not adding the same callback function again")
                 return False
         self._subscribers.append(callback)
         return True
 
-    async def remove_event_callback(self, callback: Callable[[Dict, Any], None],) -> bool:
+    def remove_event_callback(self, callback: Callable[[Dict, Any], None],) -> bool:
         if callback in self._subscribers:
             self._subscribers.remove(callback)
             return True
         return False
 
     async def message_callback(self, message) -> None:
         """Entrypoint for a websocket callback"""
@@ -359,15 +362,15 @@
                 "version": version
             }
             async with self._session.post(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update/version",
                 ssl=False,
                 data=json.dumps(data)
             ) as response:
-                result = await response.status
+                result = response.status
                 if result == 200:
                     return True
                 return False
         except:
             raise SwidgetException
 
     @property
@@ -385,45 +388,45 @@
             "model": self.model,
             "insert_type": self.insert_type,
             "insert_features": self.insert_features,
             "host_features": self.host_features,
             "rssi": self.rssi
         }
 
-    async def get_child_consumption(self, plug_id=0) -> Any:
+    def get_child_consumption(self, plug_id=0) -> Any:
         """Get the power consumption of a plug in watts."""
         if plug_id == "all":
             return_dict = {}
             for id, properties in self.assemblies['host'].components.items():
                 try:
                     return_dict[f"power_{id}"] = properties.functions['power']['current']
                 except KeyError: # Hits this when there is no power metering
                     return None
             return return_dict
         return self.assemblies['host'].components[str(plug_id)].functions['power']['current']
 
-    async def total_consumption(self) -> float:
+    def total_consumption(self) -> float:
         """Get the total power consumption in watts."""
         total_consumption = 0
         for id, properties in self.assemblies['host'].components.items():
             total_consumption += properties.functions['power']['current']
         return total_consumption
 
     @property
-    async def realtime_values(self) -> Dict:
+    def realtime_values(self) -> Dict:
         """Get a dict of realtime value attributes from the insert and host
 
         :return: A dictionary of insert sensor values and power consumption values
         :rtype: dict
         """
         return_dict = {}
         for feature in self.insert_features:
             return_dict.update(self.get_function_values(feature))
         return_dict.update({'rssi': self.rssi})
-        power_values = await self.get_child_consumption("all")
+        power_values =self.get_child_consumption("all")
         if power_values:
             return_dict.update(power_values)
         return return_dict
 
     @property
     def host_features(self) -> List[str]:
         """Return a set of features that the host supports."""
@@ -547,20 +550,14 @@
     async def __aexit__(
         self, exc_type: Exception, exc_value: str, traceback: TracebackType
     ) -> None:
         """Disconnect from the websocket."""
         await self.disconnect()
 
     def __repr__(self) -> str:
-        """Return the representation."""
-        url = self.connection.ws_server_url
-        prefix = "" if self.connection.connected else "not "
-        return f"{type(self).__name__}(ws_server_url={url!r}, {prefix}connected)"
-
-    def __repr__(self) -> str:
         if self._last_update == 0:
             return f"<{self.device_type} at {self.ip_address} - update() needed>"
         return f"<{self.device_type} model {self.model} at {self.ip_address}>"
 
 
 class SwidgetAssembly:
     def __init__(self, summary: dict):
```

### Comparing `python_swidget-1.2.0/swidget/swidgetdimmer.py` & `python_swidget-1.2.1/swidget/swidgetdimmer.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/swidget/swidgettimerswitch.py` & `python_swidget-1.2.1/swidget/swidgettimerswitch.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.2.0/swidget/websocket.py` & `python_swidget-1.2.1/swidget/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,16 @@
                 aiohttp.WSMsgType.CLOSED,
                 aiohttp.WSMsgType.CLOSING,
             ):
                 _LOGGER.error("Connection to the Swidget WebSocket on has been closed")
 
     async def receive_message_or_raise(self) -> Any:
         """Receive ONE (raw) message or raise."""
-        assert self._ws_client
-        ws_msg = await self._ws_client.receive()
+        assert self._client
+        ws_msg = await self._client.receive()
 
         if ws_msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSED, WSMsgType.CLOSING):
             raise ConnectionError("Connection was closed.")
 
         if ws_msg.type == WSMsgType.ERROR:
             raise ConnectionError
```

### Comparing `python_swidget-1.2.0/PKG-INFO` & `python_swidget-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-swidget
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python API for Swidget smart devices
 Home-page: https://github.com/swidget/python-swidget
 License: GPL-3.0-or-later
 Author: Swidget
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

