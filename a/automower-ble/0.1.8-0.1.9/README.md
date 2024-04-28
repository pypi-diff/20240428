# Comparing `tmp/automower_ble-0.1.8.tar.gz` & `tmp/automower_ble-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automower_ble-0.1.8.tar", last modified: Sun Jan 14 02:59:23 2024, max compression
+gzip compressed data, was "automower_ble-0.1.9.tar", last modified: Sun Jan 14 10:12:59 2024, max compression
```

## Comparing `automower_ble-0.1.8.tar` & `automower_ble-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alistair  (1000) alistair  (1000)        0 2024-01-14 02:59:23.639451 automower_ble-0.1.8/
--rw-r--r--   0 alistair  (1000) alistair  (1000)    35149 2024-01-09 11:34:27.000000 automower_ble-0.1.8/LICENSE
--rw-r--r--   0 alistair  (1000) alistair  (1000)     1570 2024-01-14 02:59:23.639451 automower_ble-0.1.8/PKG-INFO
--rw-r--r--   0 alistair  (1000) alistair  (1000)     1205 2024-01-09 12:05:14.000000 automower_ble-0.1.8/README.md
-drwxr-xr-x   0 alistair  (1000) alistair  (1000)        0 2024-01-14 02:59:23.638451 automower_ble-0.1.8/automower_ble/
--rw-r--r--   0 alistair  (1000) alistair  (1000)        0 2024-01-10 11:01:04.000000 automower_ble-0.1.8/automower_ble/__init__.py
--rw-r--r--   0 alistair  (1000) alistair  (1000)     1506 2024-01-09 11:47:18.000000 automower_ble-0.1.8/automower_ble/helpers.py
--rw-r--r--   0 alistair  (1000) alistair  (1000)     1434 2024-01-09 11:47:22.000000 automower_ble-0.1.8/automower_ble/models.py
--rw-r--r--   0 alistair  (1000) alistair  (1000)    11409 2024-01-14 02:58:01.000000 automower_ble-0.1.8/automower_ble/mower.py
--rw-r--r--   0 alistair  (1000) alistair  (1000)    10543 2024-01-14 01:09:13.000000 automower_ble-0.1.8/automower_ble/request.py
--rw-r--r--   0 alistair  (1000) alistair  (1000)     5413 2024-01-14 01:09:13.000000 automower_ble-0.1.8/automower_ble/response.py
-drwxr-xr-x   0 alistair  (1000) alistair  (1000)        0 2024-01-14 02:59:23.639451 automower_ble-0.1.8/automower_ble.egg-info/
--rw-r--r--   0 alistair  (1000) alistair  (1000)     1570 2024-01-14 02:59:23.000000 automower_ble-0.1.8/automower_ble.egg-info/PKG-INFO
--rw-r--r--   0 alistair  (1000) alistair  (1000)      329 2024-01-14 02:59:23.000000 automower_ble-0.1.8/automower_ble.egg-info/SOURCES.txt
--rw-r--r--   0 alistair  (1000) alistair  (1000)        1 2024-01-14 02:59:23.000000 automower_ble-0.1.8/automower_ble.egg-info/dependency_links.txt
--rw-r--r--   0 alistair  (1000) alistair  (1000)       14 2024-01-14 02:59:23.000000 automower_ble-0.1.8/automower_ble.egg-info/top_level.txt
--rw-r--r--   0 alistair  (1000) alistair  (1000)      447 2024-01-14 02:58:08.000000 automower_ble-0.1.8/pyproject.toml
--rw-r--r--   0 alistair  (1000) alistair  (1000)       38 2024-01-14 02:59:23.639451 automower_ble-0.1.8/setup.cfg
+drwxr-xr-x   0 alistair  (1000) alistair  (1000)        0 2024-01-14 10:12:59.792869 automower_ble-0.1.9/
+-rw-r--r--   0 alistair  (1000) alistair  (1000)    35149 2024-01-09 11:34:27.000000 automower_ble-0.1.9/LICENSE
+-rw-r--r--   0 alistair  (1000) alistair  (1000)     1570 2024-01-14 10:12:59.792869 automower_ble-0.1.9/PKG-INFO
+-rw-r--r--   0 alistair  (1000) alistair  (1000)     1205 2024-01-09 12:05:14.000000 automower_ble-0.1.9/README.md
+drwxr-xr-x   0 alistair  (1000) alistair  (1000)        0 2024-01-14 10:12:59.790869 automower_ble-0.1.9/automower_ble/
+-rw-r--r--   0 alistair  (1000) alistair  (1000)        0 2024-01-10 11:01:04.000000 automower_ble-0.1.9/automower_ble/__init__.py
+-rw-r--r--   0 alistair  (1000) alistair  (1000)     1506 2024-01-09 11:47:18.000000 automower_ble-0.1.9/automower_ble/helpers.py
+-rw-r--r--   0 alistair  (1000) alistair  (1000)     1434 2024-01-09 11:47:22.000000 automower_ble-0.1.9/automower_ble/models.py
+-rw-r--r--   0 alistair  (1000) alistair  (1000)    11308 2024-01-14 10:11:27.000000 automower_ble-0.1.9/automower_ble/mower.py
+-rw-r--r--   0 alistair  (1000) alistair  (1000)    10543 2024-01-14 10:09:38.000000 automower_ble-0.1.9/automower_ble/request.py
+-rw-r--r--   0 alistair  (1000) alistair  (1000)     5413 2024-01-14 10:09:38.000000 automower_ble-0.1.9/automower_ble/response.py
+drwxr-xr-x   0 alistair  (1000) alistair  (1000)        0 2024-01-14 10:12:59.791869 automower_ble-0.1.9/automower_ble.egg-info/
+-rw-r--r--   0 alistair  (1000) alistair  (1000)     1570 2024-01-14 10:12:59.000000 automower_ble-0.1.9/automower_ble.egg-info/PKG-INFO
+-rw-r--r--   0 alistair  (1000) alistair  (1000)      329 2024-01-14 10:12:59.000000 automower_ble-0.1.9/automower_ble.egg-info/SOURCES.txt
+-rw-r--r--   0 alistair  (1000) alistair  (1000)        1 2024-01-14 10:12:59.000000 automower_ble-0.1.9/automower_ble.egg-info/dependency_links.txt
+-rw-r--r--   0 alistair  (1000) alistair  (1000)       14 2024-01-14 10:12:59.000000 automower_ble-0.1.9/automower_ble.egg-info/top_level.txt
+-rw-r--r--   0 alistair  (1000) alistair  (1000)      447 2024-01-14 10:11:32.000000 automower_ble-0.1.9/pyproject.toml
+-rw-r--r--   0 alistair  (1000) alistair  (1000)       38 2024-01-14 10:12:59.792869 automower_ble-0.1.9/setup.cfg
```

### Comparing `automower_ble-0.1.8/LICENSE` & `automower_ble-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automower_ble-0.1.8/PKG-INFO` & `automower_ble-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automower_ble
-Version: 0.1.8
+Version: 0.1.9
 Summary: An unofficial reverse engineered Husqvarna Automower Connect BLE library
 Author-email: Alistair Francis <alistair@alistair23.me>
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: automower_ble Version: 0.1.8 Summary: An unofficial
+Metadata-Version: 2.1 Name: automower_ble Version: 0.1.9 Summary: An unofficial
 reverse engineered Husqvarna Automower Connect BLE library Author-email:
 Alistair Francis
 alistair23.me> Classifier: Environment :: Console Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # AutoMower-BLE This is an unofficial reverse
 engineered Husqvarna Automower Connect BLE library. This allows connecting and
 controlling an Automower without any accounts, cloud or network connection.
```

### Comparing `automower_ble-0.1.8/README.md` & `automower_ble-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `automower_ble-0.1.8/automower_ble/helpers.py` & `automower_ble-0.1.9/automower_ble/helpers.py`

 * *Files identical despite different names*

### Comparing `automower_ble-0.1.8/automower_ble/models.py` & `automower_ble-0.1.9/automower_ble/models.py`

 * *Files identical despite different names*

### Comparing `automower_ble-0.1.8/automower_ble/mower.py` & `automower_ble-0.1.9/automower_ble/mower.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .response import MowerResponse
 
 from bleak import BleakClient, BleakScanner
 from bleak.backends.characteristic import BleakGATTCharacteristic
 
 logger = logging.getLogger(__name__)
 
+MTU_SIZE = 20
 
 class Mower:
     def __init__(self, channel_id: int, address):
         self.channel_id = channel_id
         self.address = address
 
         self.request = MowerRequest(channel_id)
@@ -51,15 +52,15 @@
         await self.client.connect()
         logger.info("connected")
 
         logger.info("pairing device...")
         await self.client.pair()
         logger.info("paired")
 
-        self.client._backend._mtu_size = 20
+        self.client._backend._mtu_size = MTU_SIZE
 
         for service in self.client.services:
             logger.info("[Service] %s", service)
 
             for char in service.characteristics:
                 if "read" in char.properties:
                     try:
@@ -93,118 +94,118 @@
             await self.queue.put(data)
 
         await self.client.start_notify(self.read_char, notification_handler)
 
         data = self.request.generate_request_setup_channel_id()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         logger.debug("chunk_size: " + str(chunk_size))
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
 
         data = self.request.generate_request_handshake()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
 
     async def get_model(self):
         """
             Get the mower model
         """
         data = self.request.generate_request_device_type()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
         return self.response.decode_response_device_type(data)
 
     async def is_charging(self):
         data = self.request.generate_request_is_charging()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
     async def battery_level(self):
         """
             Query the mower battery level
         """
         data = self.request.generate_request_battery_level()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
         return self.response.decode_response_battery_level(data)
 
     async def mower_state(self):
         data = self.request.generate_request_mower_state()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
         return self.response.decode_response_mower_state(data)
 
     async def mower_activity(self):
         data = self.request.generate_request_mower_activity()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
         return self.response.decode_response_mower_activity(data)
 
@@ -212,64 +213,64 @@
         """
             Force the mower to run 3 hours
         """
 
         data = self.request.generate_request_mode_of_operation("manual")
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
         data = self.request.generate_request_override_duration("3hours")
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
     async def mower_pause(self):
         data = self.request.generate_request_pause()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
     async def mower_resume(self):
         data = self.request.generate_request_resume()
         logger.info("Writing: " + str(binascii.hexlify(data)))
 
-        chunk_size = self.client.mtu_size - 3
+        chunk_size = MTU_SIZE - 3
         for chunk in (
             data[i: i + chunk_size] for i in range(0, len(data), chunk_size)
         ):
             logger.info(chunk)
-            await self.client.write_gatt_char(self.write_char, chunk, response=True)
+            await self.client.write_gatt_char(self.write_char, chunk, response=False)
 
         data = await self.queue.get()
         if data[len(data) - 1] != 0x03:
             data = data + await self.queue.get()
 
     async def disconnect(self):
         """
```

### Comparing `automower_ble-0.1.8/automower_ble/request.py` & `automower_ble-0.1.9/automower_ble/request.py`

 * *Files identical despite different names*

### Comparing `automower_ble-0.1.8/automower_ble/response.py` & `automower_ble-0.1.9/automower_ble/response.py`

 * *Files identical despite different names*

### Comparing `automower_ble-0.1.8/automower_ble.egg-info/PKG-INFO` & `automower_ble-0.1.9/automower_ble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automower_ble
-Version: 0.1.8
+Version: 0.1.9
 Summary: An unofficial reverse engineered Husqvarna Automower Connect BLE library
 Author-email: Alistair Francis <alistair@alistair23.me>
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: automower_ble Version: 0.1.8 Summary: An unofficial
+Metadata-Version: 2.1 Name: automower_ble Version: 0.1.9 Summary: An unofficial
 reverse engineered Husqvarna Automower Connect BLE library Author-email:
 Alistair Francis
 alistair23.me> Classifier: Environment :: Console Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # AutoMower-BLE This is an unofficial reverse
 engineered Husqvarna Automower Connect BLE library. This allows connecting and
 controlling an Automower without any accounts, cloud or network connection.
```

