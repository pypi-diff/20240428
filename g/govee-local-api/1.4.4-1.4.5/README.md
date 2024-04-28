# Comparing `tmp/govee_local_api-1.4.4.tar.gz` & `tmp/govee_local_api-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govee_local_api-1.4.4.tar", max compression
+gzip compressed data, was "govee_local_api-1.4.5.tar", max compression
```

## Comparing `govee_local_api-1.4.4.tar` & `govee_local_api-1.4.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-12-14 23:25:14.641450 govee_local_api-1.4.4/LICENSE
--rw-r--r--   0        0        0      464 2023-12-14 23:25:14.641450 govee_local_api-1.4.4/README.md
--rw-r--r--   0        0        0     1286 2024-02-18 12:56:02.424195 govee_local_api-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      219 2024-02-18 11:45:29.275820 govee_local_api-1.4.4/src/govee_local_api/__init__.py
--rw-r--r--   0        0        0    12813 2024-02-13 20:48:51.658758 govee_local_api-1.4.4/src/govee_local_api/controller.py
--rw-r--r--   0        0        0     4062 2024-02-13 20:48:51.658758 govee_local_api-1.4.4/src/govee_local_api/device.py
--rw-r--r--   0        0        0    10208 2024-02-18 11:40:12.431814 govee_local_api-1.4.4/src/govee_local_api/light_capabilities.py
--rw-r--r--   0        0        0     3755 2024-02-08 21:11:28.576514 govee_local_api-1.4.4/src/govee_local_api/message.py
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 govee_local_api-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/LICENSE
+-rw-r--r--   0        0        0      464 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/README.md
+-rw-r--r--   0        0        0     1252 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/src/govee_local_api/__init__.py
+-rw-r--r--   0        0        0    13573 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/controller.py
+-rw-r--r--   0        0        0     4062 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/device.py
+-rw-r--r--   0        0        0    11156 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/light_capabilities.py
+-rw-r--r--   0        0        0     3755 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/message.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 govee_local_api-1.4.5/PKG-INFO
```

### Comparing `govee_local_api-1.4.4/LICENSE` & `govee_local_api-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `govee_local_api-1.4.4/pyproject.toml` & `govee_local_api-1.4.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "govee-local-api"
-version = "1.4.4"
+version = "1.4.5"
 description = "Library to communicate with Govee local API"
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/Galorhallen/govee-local-api"
 
 authors = ["Galorhallen <andrea.ponte1987@gmail.com>"]
 
@@ -18,17 +18,16 @@
 packages = [
     { include = "govee_local_api", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Galorhallen/govee-local-api/issues"
 
-
-[tool.poetry-dynamic-versioning]
-enable = false
+[tool.poetry_bumpversion.file."src/govee_local_api/__init__.py"]
+# Duplicate the line above to add more files
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 
@@ -47,9 +46,8 @@
 pythonpath = "src"
 addopts = [
     "--import-mode=importlib",
     "-v",
 ]
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
-build-backend = "poetry_dynamic_versioning.backend"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `govee_local_api-1.4.4/src/govee_local_api/controller.py` & `govee_local_api-1.4.5/src/govee_local_api/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,20 +236,41 @@
 
     @property
     def devices(self) -> list[GoveeDevice]:
         return list(self._devices.values())
 
     def connection_made(self, transport):
         self._transport = transport
-
         sock = self._transport.get_extra_info("socket")
+
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+        sock.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, 2)
+
+        sock.setsockopt(
+            socket.SOL_IP,
+            socket.IP_MULTICAST_IF,
+            socket.inet_aton(self._listening_address),
+        )
+        sock.setsockopt(
+            socket.SOL_IP,
+            socket.IP_ADD_MEMBERSHIP,
+            socket.inet_aton(self._broadcast_address)
+            + socket.inet_aton(self._listening_address),
+        )
 
     def connection_lost(self, *args, **kwargs):
+        if self._transport:
+            sock = self._transport.get_extra_info("socket")
+            sock.setsockopt(
+                socket.SOL_IP,
+                socket.IP_DROP_MEMBERSHIP,
+                socket.inet_aton(self._broadcast_address)
+                + socket.inet_aton(self._listening_address),
+            )
         self._logger.debug("Disconnected")
 
     def datagram_received(self, data: bytes, addr: tuple):
         if not data:
             return
         message = self._message_factory.create_message(data)
         if not message:
```

### Comparing `govee_local_api-1.4.4/src/govee_local_api/device.py` & `govee_local_api-1.4.5/src/govee_local_api/device.py`

 * *Files identical despite different names*

### Comparing `govee_local_api-1.4.4/src/govee_local_api/light_capabilities.py` & `govee_local_api-1.4.5/src/govee_local_api/light_capabilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,8 +323,38 @@
         GoveeLightCapability.BRIGHTNESS,
     },
     "H608A": {
         GoveeLightCapability.COLOR_RGB,
         GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
         GoveeLightCapability.BRIGHTNESS,
     },
+    "H606A": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
+    "H61C5": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
+    "H7020": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
+    "H61BE": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
+    "H61B5": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
+    "H61C3": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
 }
```

### Comparing `govee_local_api-1.4.4/src/govee_local_api/message.py` & `govee_local_api-1.4.5/src/govee_local_api/message.py`

 * *Files identical despite different names*

### Comparing `govee_local_api-1.4.4/PKG-INFO` & `govee_local_api-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govee-local-api
-Version: 1.4.4
+Version: 1.4.5
 Summary: Library to communicate with Govee local API
 Home-page: https://github.com/Galorhallen/govee-local-api
 License: Apache Software License 2.0
 Author: Galorhallen
 Author-email: andrea.ponte1987@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

