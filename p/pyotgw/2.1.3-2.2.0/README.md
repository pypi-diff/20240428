# Comparing `tmp/pyotgw-2.1.3.tar.gz` & `tmp/pyotgw-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyotgw-2.1.3.tar", last modified: Sun Nov 20 20:28:47 2022, max compression
+gzip compressed data, was "pyotgw-2.2.0.tar", last modified: Sun Apr 28 19:12:15 2024, max compression
```

## Comparing `pyotgw-2.1.3.tar` & `pyotgw-2.2.0.tar`

### file list

```diff
@@ -1,42 +1,30 @@
-drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2022-11-20 20:28:47.214355 pyotgw-2.1.3/
--rw-r--r--   0 milan     (1000) milan     (1000)       22 2022-07-28 18:15:15.000000 pyotgw-2.1.3/.coveragerc
-drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2022-11-20 20:28:47.207688 pyotgw-2.1.3/.github/
-drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2022-11-20 20:28:47.207688 pyotgw-2.1.3/.github/workflows/
--rw-r--r--   0 milan     (1000) milan     (1000)      965 2022-07-28 18:15:15.000000 pyotgw-2.1.3/.github/workflows/ci.yml
--rw-r--r--   0 milan     (1000) milan     (1000)       35 2022-07-28 18:15:15.000000 pyotgw-2.1.3/.gitignore
--rw-r--r--   0 milan     (1000) milan     (1000)      907 2022-11-20 15:58:25.000000 pyotgw-2.1.3/.pre-commit-config.yaml
--rw-r--r--   0 milan     (1000) milan     (1000)      256 2022-07-28 18:15:15.000000 pyotgw-2.1.3/.travis.yml
--rw-r--r--   0 milan     (1000) milan     (1000)    35149 2017-09-30 07:16:26.000000 pyotgw-2.1.3/LICENSE
--rw-r--r--   0 milan     (1000) milan     (1000)    28917 2022-11-20 20:28:47.214355 pyotgw-2.1.3/PKG-INFO
--rw-r--r--   0 milan     (1000) milan     (1000)    28334 2022-10-14 19:28:06.000000 pyotgw-2.1.3/README.md
-drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2022-11-20 20:28:47.211021 pyotgw-2.1.3/pyotgw/
--rw-r--r--   0 milan     (1000) milan     (1000)      112 2022-07-28 18:15:15.000000 pyotgw-2.1.3/pyotgw/__init__.py
--rw-r--r--   0 milan     (1000) milan     (1000)     4869 2022-07-28 18:15:15.000000 pyotgw-2.1.3/pyotgw/commandprocessor.py
--rw-r--r--   0 milan     (1000) milan     (1000)     7933 2022-08-20 15:03:47.000000 pyotgw-2.1.3/pyotgw/connection.py
--rw-r--r--   0 milan     (1000) milan     (1000)     7688 2022-11-20 16:09:52.000000 pyotgw-2.1.3/pyotgw/messageprocessor.py
--rw-r--r--   0 milan     (1000) milan     (1000)    15934 2022-11-20 20:22:22.000000 pyotgw-2.1.3/pyotgw/messages.py
--rw-r--r--   0 milan     (1000) milan     (1000)     4455 2022-07-29 01:25:41.000000 pyotgw-2.1.3/pyotgw/protocol.py
--rw-r--r--   0 milan     (1000) milan     (1000)    35961 2022-10-14 19:28:06.000000 pyotgw-2.1.3/pyotgw/pyotgw.py
--rw-r--r--   0 milan     (1000) milan     (1000)     3755 2022-08-03 10:34:23.000000 pyotgw-2.1.3/pyotgw/status.py
--rw-r--r--   0 milan     (1000) milan     (1000)    10905 2022-07-28 18:15:15.000000 pyotgw-2.1.3/pyotgw/vars.py
-drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2022-11-20 20:28:47.211021 pyotgw-2.1.3/pyotgw.egg-info/
--rw-r--r--   0 milan     (1000) milan     (1000)    28917 2022-11-20 20:28:47.000000 pyotgw-2.1.3/pyotgw.egg-info/PKG-INFO
--rw-r--r--   0 milan     (1000) milan     (1000)      681 2022-11-20 20:28:47.000000 pyotgw-2.1.3/pyotgw.egg-info/SOURCES.txt
--rw-r--r--   0 milan     (1000) milan     (1000)        1 2022-11-20 20:28:47.000000 pyotgw-2.1.3/pyotgw.egg-info/dependency_links.txt
--rw-r--r--   0 milan     (1000) milan     (1000)       17 2022-11-20 20:28:47.000000 pyotgw-2.1.3/pyotgw.egg-info/requires.txt
--rw-r--r--   0 milan     (1000) milan     (1000)        7 2022-11-20 20:28:47.000000 pyotgw-2.1.3/pyotgw.egg-info/top_level.txt
--rw-r--r--   0 milan     (1000) milan     (1000)       88 2022-07-28 18:15:15.000000 pyotgw-2.1.3/requirements_test.txt
--rw-r--r--   0 milan     (1000) milan     (1000)       38 2022-11-20 20:28:47.214355 pyotgw-2.1.3/setup.cfg
--rw-r--r--   0 milan     (1000) milan     (1000)     1123 2022-11-20 20:27:57.000000 pyotgw-2.1.3/setup.py
-drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2022-11-20 20:28:47.214355 pyotgw-2.1.3/tests/
--rw-r--r--   0 milan     (1000) milan     (1000)       19 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/__init__.py
--rw-r--r--   0 milan     (1000) milan     (1000)     2098 2022-08-20 14:13:19.000000 pyotgw-2.1.3/tests/conftest.py
--rw-r--r--   0 milan     (1000) milan     (1000)    14289 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/data.py
--rw-r--r--   0 milan     (1000) milan     (1000)      696 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/helpers.py
--rw-r--r--   0 milan     (1000) milan     (1000)    14487 2022-08-20 16:02:18.000000 pyotgw-2.1.3/tests/test_connection.py
--rw-r--r--   0 milan     (1000) milan     (1000)    11424 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/test_messageprocessor.py
--rw-r--r--   0 milan     (1000) milan     (1000)      629 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/test_messages.py
--rw-r--r--   0 milan     (1000) milan     (1000)     5367 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/test_protocol.py
--rw-r--r--   0 milan     (1000) milan     (1000)    29737 2022-10-14 14:18:21.000000 pyotgw-2.1.3/tests/test_pyotgw.py
--rw-r--r--   0 milan     (1000) milan     (1000)     6732 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tests/test_status.py
--rw-r--r--   0 milan     (1000) milan     (1000)      909 2022-07-28 18:15:15.000000 pyotgw-2.1.3/tox.ini
+drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2024-04-28 19:12:15.696239 pyotgw-2.2.0/
+-rw-r--r--   0 milan     (1000) milan     (1000)    35149 2024-01-07 11:33:09.000000 pyotgw-2.2.0/LICENSE
+-rw-r--r--   0 milan     (1000) milan     (1000)    29440 2024-04-28 19:12:15.696239 pyotgw-2.2.0/PKG-INFO
+-rw-r--r--   0 milan     (1000) milan     (1000)    28857 2024-04-27 14:06:35.000000 pyotgw-2.2.0/README.md
+drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2024-04-28 19:12:15.692906 pyotgw-2.2.0/pyotgw/
+-rw-r--r--   0 milan     (1000) milan     (1000)      112 2024-01-07 11:33:09.000000 pyotgw-2.2.0/pyotgw/__init__.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     4869 2024-01-07 11:33:09.000000 pyotgw-2.2.0/pyotgw/commandprocessor.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     8364 2024-04-28 14:28:53.000000 pyotgw-2.2.0/pyotgw/connection.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     7688 2024-01-07 11:33:09.000000 pyotgw-2.2.0/pyotgw/messageprocessor.py
+-rw-r--r--   0 milan     (1000) milan     (1000)    15934 2024-01-07 11:33:09.000000 pyotgw-2.2.0/pyotgw/messages.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     4455 2024-04-27 14:30:12.000000 pyotgw-2.2.0/pyotgw/protocol.py
+-rw-r--r--   0 milan     (1000) milan     (1000)    36889 2024-04-28 19:06:19.000000 pyotgw-2.2.0/pyotgw/pyotgw.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     3755 2024-01-07 11:33:09.000000 pyotgw-2.2.0/pyotgw/status.py
+-rw-r--r--   0 milan     (1000) milan     (1000)    10905 2024-01-07 11:33:09.000000 pyotgw-2.2.0/pyotgw/vars.py
+drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2024-04-28 19:12:15.692906 pyotgw-2.2.0/pyotgw.egg-info/
+-rw-r--r--   0 milan     (1000) milan     (1000)    29440 2024-04-28 19:12:15.000000 pyotgw-2.2.0/pyotgw.egg-info/PKG-INFO
+-rw-r--r--   0 milan     (1000) milan     (1000)      531 2024-04-28 19:12:15.000000 pyotgw-2.2.0/pyotgw.egg-info/SOURCES.txt
+-rw-r--r--   0 milan     (1000) milan     (1000)        1 2024-04-28 19:12:15.000000 pyotgw-2.2.0/pyotgw.egg-info/dependency_links.txt
+-rw-r--r--   0 milan     (1000) milan     (1000)       22 2024-04-28 19:12:15.000000 pyotgw-2.2.0/pyotgw.egg-info/requires.txt
+-rw-r--r--   0 milan     (1000) milan     (1000)        7 2024-04-28 19:12:15.000000 pyotgw-2.2.0/pyotgw.egg-info/top_level.txt
+-rw-r--r--   0 milan     (1000) milan     (1000)       38 2024-04-28 19:12:15.696239 pyotgw-2.2.0/setup.cfg
+-rw-r--r--   0 milan     (1000) milan     (1000)     1128 2024-04-28 19:09:03.000000 pyotgw-2.2.0/setup.py
+drwxr-xr-x   0 milan     (1000) milan     (1000)        0 2024-04-28 19:12:15.696239 pyotgw-2.2.0/tests/
+-rw-r--r--   0 milan     (1000) milan     (1000)     6743 2024-01-07 11:33:09.000000 pyotgw-2.2.0/tests/test_commandprocessor.py
+-rw-r--r--   0 milan     (1000) milan     (1000)    15519 2024-04-28 11:24:41.000000 pyotgw-2.2.0/tests/test_connection.py
+-rw-r--r--   0 milan     (1000) milan     (1000)    12102 2024-04-28 11:28:43.000000 pyotgw-2.2.0/tests/test_messageprocessor.py
+-rw-r--r--   0 milan     (1000) milan     (1000)      629 2024-01-07 11:33:09.000000 pyotgw-2.2.0/tests/test_messages.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     5367 2024-01-07 11:33:09.000000 pyotgw-2.2.0/tests/test_protocol.py
+-rw-r--r--   0 milan     (1000) milan     (1000)    30228 2024-04-27 14:34:29.000000 pyotgw-2.2.0/tests/test_pyotgw.py
+-rw-r--r--   0 milan     (1000) milan     (1000)     6732 2024-01-07 11:33:09.000000 pyotgw-2.2.0/tests/test_status.py
```

### Comparing `pyotgw-2.1.3/LICENSE` & `pyotgw-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/PKG-INFO` & `pyotgw-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyotgw
-Version: 2.1.3
+Version: 2.2.0
 Summary: A library to interface with the opentherm gateway through serial or network connection.
 Home-page: https://github.com/mvn23/pyotgw
 Author: Milan van Nugteren
 Author-email: milan@network23.nl
 License: GPLv3+
 Keywords: opentherm gateway otgw
 Classifier: Development Status :: 5 - Production/Stable
@@ -370,14 +370,27 @@
 - __timeout__ The timeout for the request. Defaults to OTGW_DEFAULT_TIMEOUT (3 seconds).
 
 Return the newly accepted value, or `None` on failure.
 
 This method is a coroutine.
 
 ---
+##### OpenThermGateway.send_transparent_command(_self_, cmd, state, timeout=OTGW_DEFAULT_TIMEOUT)
+Send a transparent command.
+Sends custom commands through a transparent interface.
+Check https://otgw.tclcode.com/firmware.html for supported commands.
+This method supports the following arguments:
+- __cmd__ The supported command e.g. `SC` (set time/day).
+- __state__ The command argument e.g. `23:59/4` (the current time/day)
+
+Returns the gateway response, which should be equal __state__.
+
+This method is a coroutine.
+
+---
 ##### OpenThermGateway.subscribe(_self_, coro)
 Subscribe to status updates from the Opentherm Gateway.
 The subscribed coroutine must have the following signature:
 ```
 async def coro(status)
 ```
 Where `status` will be the full status dict containing the last known information from the OpenTherm Gateway.
```

### Comparing `pyotgw-2.1.3/README.md` & `pyotgw-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,27 @@
 - __timeout__ The timeout for the request. Defaults to OTGW_DEFAULT_TIMEOUT (3 seconds).
 
 Return the newly accepted value, or `None` on failure.
 
 This method is a coroutine.
 
 ---
+##### OpenThermGateway.send_transparent_command(_self_, cmd, state, timeout=OTGW_DEFAULT_TIMEOUT)
+Send a transparent command.
+Sends custom commands through a transparent interface.
+Check https://otgw.tclcode.com/firmware.html for supported commands.
+This method supports the following arguments:
+- __cmd__ The supported command e.g. `SC` (set time/day).
+- __state__ The command argument e.g. `23:59/4` (the current time/day)
+
+Returns the gateway response, which should be equal __state__.
+
+This method is a coroutine.
+
+---
 ##### OpenThermGateway.subscribe(_self_, coro)
 Subscribe to status updates from the Opentherm Gateway.
 The subscribed coroutine must have the following signature:
 ```
 async def coro(status)
 ```
 Where `status` will be the full status dict containing the last known information from the OpenTherm Gateway.
```

### Comparing `pyotgw-2.1.3/pyotgw/commandprocessor.py` & `pyotgw-2.2.0/pyotgw/commandprocessor.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/pyotgw/connection.py` & `pyotgw-2.2.0/pyotgw/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import asyncio
 import logging
 from functools import partial
 
 import serial
-import serial_asyncio
+import serial_asyncio_fast
 
 from pyotgw.protocol import OpenThermProtocol
 
 CONNECTION_TIMEOUT = 5
 
 MAX_RETRY_TIMEOUT = 60
 MIN_RETRY_TIMEOUT = 5
@@ -108,24 +108,26 @@
         """Try to connect to the OpenTherm Gateway."""
         loop = asyncio.get_running_loop()
         transport = None
         protocol = None
         self._retry_timeout = MIN_RETRY_TIMEOUT
         while transport is None:
             try:
-                transport, protocol = await serial_asyncio.create_serial_connection(
-                    loop,
-                    partial(
-                        OpenThermProtocol,
-                        self._otgw.status,
-                        self.watchdog.inform,
-                    ),
-                    self._port,
-                    write_timeout=0,
-                    **self._config,
+                transport, protocol = await (
+                    serial_asyncio_fast.create_serial_connection(
+                        loop,
+                        partial(
+                            OpenThermProtocol,
+                            self._otgw.status,
+                            self.watchdog.inform,
+                        ),
+                        self._port,
+                        write_timeout=0,
+                        **self._config,
+                    )
                 )
                 await asyncio.wait_for(
                     protocol.init_and_wait_for_activity(),
                     CONNECTION_TIMEOUT,
                 )
                 return transport, protocol
 
@@ -144,15 +146,24 @@
                     _LOGGER.error(
                         "The serial device on %s is not responding. "
                         "Will keep trying.",
                         self._port,
                     )
                     self._error = err
                 if protocol:
-                    protocol.disconnect()
+                    await protocol.cleanup()
+
+            except SyntaxError as err:
+                # The gateway may throw a SyntaxError on the first initialization
+                # attempt.
+                if protocol:
+                    await protocol.cleanup()
+                if isinstance(err, type(self._error)):
+                    raise
+                self._error = err
 
             transport = None
             await asyncio.sleep(self._get_retry_timeout())
 
     async def _cleanup(self):
         """Cleanup possible leftovers from old connections"""
         await self.watchdog.stop()
```

### Comparing `pyotgw-2.1.3/pyotgw/messageprocessor.py` & `pyotgw-2.2.0/pyotgw/messageprocessor.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/pyotgw/messages.py` & `pyotgw-2.2.0/pyotgw/messages.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/pyotgw/protocol.py` & `pyotgw-2.2.0/pyotgw/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,10 +127,10 @@
     @property
     def active(self):
         """Indicate that we have seen activity on the serial line."""
         return self._received_lines > 0
 
     async def init_and_wait_for_activity(self):
         """Wait for activity on the serial connection."""
-        await self.command_processor.issue_cmd(v.OTGW_CMD_SUMMARY, 0, retry=0)
+        await self.command_processor.issue_cmd(v.OTGW_CMD_SUMMARY, 0, retry=1)
         while not self.active:
             await asyncio.sleep(0)
```

### Comparing `pyotgw-2.1.3/pyotgw/pyotgw.py` & `pyotgw-2.2.0/pyotgw/pyotgw.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,139 +261,21 @@
         # Return to 'reporting' mode
         if ret is None:
             return
         asyncio.get_running_loop().create_task(self._wait_for_cmd(cmd, 0))
         fields = ret[1].split(",")
         if len(fields) == 34:
             # OpenTherm Gateway 5.0
-            device_status = fields[0].split("/")
-            master_status = device_status[0]
-            slave_status = device_status[1]
-            remote_params = fields[2].split("/")
-            capmodlimits = fields[6].split("/")
-            dhw_setp_bounds = fields[19].split("/")
-            ch_setp_bounds = fields[20].split("/")
-            vh_device_status = fields[23].split("/")
-            vh_master_status = vh_device_status[0]
-            vh_slave_status = vh_device_status[1]
-            status = {
-                v.DATA_MASTER_CH_ENABLED: int(master_status[7]),
-                v.DATA_MASTER_DHW_ENABLED: int(master_status[6]),
-                v.DATA_MASTER_COOLING_ENABLED: int(master_status[5]),
-                v.DATA_MASTER_OTC_ENABLED: int(master_status[4]),
-                v.DATA_MASTER_CH2_ENABLED: int(master_status[3]),
-                v.DATA_SLAVE_FAULT_IND: int(slave_status[7]),
-                v.DATA_SLAVE_CH_ACTIVE: int(slave_status[6]),
-                v.DATA_SLAVE_DHW_ACTIVE: int(slave_status[5]),
-                v.DATA_SLAVE_FLAME_ON: int(slave_status[4]),
-                v.DATA_SLAVE_COOLING_ACTIVE: int(slave_status[3]),
-                v.DATA_SLAVE_CH2_ACTIVE: int(slave_status[2]),
-                v.DATA_SLAVE_DIAG_IND: int(slave_status[1]),
-                v.DATA_CONTROL_SETPOINT: float(fields[1]),
-                v.DATA_REMOTE_TRANSFER_DHW: int(remote_params[0][7]),
-                v.DATA_REMOTE_TRANSFER_MAX_CH: int(remote_params[0][6]),
-                v.DATA_REMOTE_RW_DHW: int(remote_params[1][7]),
-                v.DATA_REMOTE_RW_MAX_CH: int(remote_params[1][6]),
-                v.DATA_COOLING_CONTROL: float(fields[3]),
-                v.DATA_CONTROL_SETPOINT_2: float(fields[4]),
-                v.DATA_SLAVE_MAX_RELATIVE_MOD: float(fields[5]),
-                v.DATA_SLAVE_MAX_CAPACITY: int(capmodlimits[0]),
-                v.DATA_SLAVE_MIN_MOD_LEVEL: int(capmodlimits[1]),
-                v.DATA_ROOM_SETPOINT: float(fields[7]),
-                v.DATA_REL_MOD_LEVEL: float(fields[8]),
-                v.DATA_CH_WATER_PRESS: float(fields[9]),
-                v.DATA_DHW_FLOW_RATE: float(fields[10]),
-                v.DATA_ROOM_SETPOINT_2: float(fields[11]),
-                v.DATA_ROOM_TEMP: float(fields[12]),
-                v.DATA_CH_WATER_TEMP: float(fields[13]),
-                v.DATA_DHW_TEMP: float(fields[14]),
-                v.DATA_OUTSIDE_TEMP: float(fields[15]),
-                v.DATA_RETURN_WATER_TEMP: float(fields[16]),
-                v.DATA_CH_WATER_TEMP_2: float(fields[17]),
-                v.DATA_EXHAUST_TEMP: int(fields[18]),
-                v.DATA_SLAVE_DHW_MAX_SETP: int(dhw_setp_bounds[0]),
-                v.DATA_SLAVE_DHW_MIN_SETP: int(dhw_setp_bounds[1]),
-                v.DATA_SLAVE_CH_MAX_SETP: int(ch_setp_bounds[0]),
-                v.DATA_SLAVE_CH_MIN_SETP: int(ch_setp_bounds[1]),
-                v.DATA_DHW_SETPOINT: float(fields[21]),
-                v.DATA_MAX_CH_SETPOINT: float(fields[22]),
-                v.DATA_VH_MASTER_VENT_ENABLED: int(vh_master_status[7]),
-                v.DATA_VH_MASTER_BYPASS_POS: int(vh_master_status[6]),
-                v.DATA_VH_MASTER_BYPASS_MODE: int(vh_master_status[5]),
-                v.DATA_VH_MASTER_FREE_VENT_MODE: int(vh_master_status[4]),
-                v.DATA_VH_SLAVE_FAULT_INDICATE: int(vh_slave_status[7]),
-                v.DATA_VH_SLAVE_VENT_MODE: int(vh_slave_status[6]),
-                v.DATA_VH_SLAVE_BYPASS_STATUS: int(vh_slave_status[5]),
-                v.DATA_VH_SLAVE_BYPASS_AUTO_STATUS: int(vh_slave_status[4]),
-                v.DATA_VH_SLAVE_FREE_VENT_STATUS: int(vh_slave_status[3]),
-                v.DATA_VH_SLAVE_DIAG_INDICATE: int(vh_slave_status[1]),
-                v.DATA_VH_CONTROL_SETPOINT: int(fields[24]),
-                v.DATA_VH_RELATIVE_VENT: int(fields[25]),
-                v.DATA_TOTAL_BURNER_STARTS: int(fields[26]),
-                v.DATA_CH_PUMP_STARTS: int(fields[27]),
-                v.DATA_DHW_PUMP_STARTS: int(fields[28]),
-                v.DATA_DHW_BURNER_STARTS: int(fields[29]),
-                v.DATA_TOTAL_BURNER_HOURS: int(fields[30]),
-                v.DATA_CH_PUMP_HOURS: int(fields[31]),
-                v.DATA_DHW_PUMP_HOURS: int(fields[32]),
-                v.DATA_DHW_BURNER_HOURS: int(fields[33]),
-            }
+            boiler_status, thermostat_status = process_statusfields_v5(fields)
         else:
-            device_status = fields[0].split("/")
-            master_status = device_status[0]
-            slave_status = device_status[1]
-            remote_params = fields[2].split("/")
-            capmodlimits = fields[4].split("/")
-            dhw_setp_bounds = fields[13].split("/")
-            ch_setp_bounds = fields[14].split("/")
-            status = {
-                v.DATA_MASTER_CH_ENABLED: int(master_status[7]),
-                v.DATA_MASTER_DHW_ENABLED: int(master_status[6]),
-                v.DATA_MASTER_COOLING_ENABLED: int(master_status[5]),
-                v.DATA_MASTER_OTC_ENABLED: int(master_status[4]),
-                v.DATA_MASTER_CH2_ENABLED: int(master_status[3]),
-                v.DATA_SLAVE_FAULT_IND: int(slave_status[7]),
-                v.DATA_SLAVE_CH_ACTIVE: int(slave_status[6]),
-                v.DATA_SLAVE_DHW_ACTIVE: int(slave_status[5]),
-                v.DATA_SLAVE_FLAME_ON: int(slave_status[4]),
-                v.DATA_SLAVE_COOLING_ACTIVE: int(slave_status[3]),
-                v.DATA_SLAVE_CH2_ACTIVE: int(slave_status[2]),
-                v.DATA_SLAVE_DIAG_IND: int(slave_status[1]),
-                v.DATA_CONTROL_SETPOINT: float(fields[1]),
-                v.DATA_REMOTE_TRANSFER_DHW: int(remote_params[0][7]),
-                v.DATA_REMOTE_TRANSFER_MAX_CH: int(remote_params[0][6]),
-                v.DATA_REMOTE_RW_DHW: int(remote_params[1][7]),
-                v.DATA_REMOTE_RW_MAX_CH: int(remote_params[1][6]),
-                v.DATA_SLAVE_MAX_RELATIVE_MOD: float(fields[3]),
-                v.DATA_SLAVE_MAX_CAPACITY: int(capmodlimits[0]),
-                v.DATA_SLAVE_MIN_MOD_LEVEL: int(capmodlimits[1]),
-                v.DATA_ROOM_SETPOINT: float(fields[5]),
-                v.DATA_REL_MOD_LEVEL: float(fields[6]),
-                v.DATA_CH_WATER_PRESS: float(fields[7]),
-                v.DATA_ROOM_TEMP: float(fields[8]),
-                v.DATA_CH_WATER_TEMP: float(fields[9]),
-                v.DATA_DHW_TEMP: float(fields[10]),
-                v.DATA_OUTSIDE_TEMP: float(fields[11]),
-                v.DATA_RETURN_WATER_TEMP: float(fields[12]),
-                v.DATA_SLAVE_DHW_MAX_SETP: int(dhw_setp_bounds[0]),
-                v.DATA_SLAVE_DHW_MIN_SETP: int(dhw_setp_bounds[1]),
-                v.DATA_SLAVE_CH_MAX_SETP: int(ch_setp_bounds[0]),
-                v.DATA_SLAVE_CH_MIN_SETP: int(ch_setp_bounds[1]),
-                v.DATA_DHW_SETPOINT: float(fields[15]),
-                v.DATA_MAX_CH_SETPOINT: float(fields[16]),
-                v.DATA_TOTAL_BURNER_STARTS: int(fields[17]),
-                v.DATA_CH_PUMP_STARTS: int(fields[18]),
-                v.DATA_DHW_PUMP_STARTS: int(fields[19]),
-                v.DATA_DHW_BURNER_STARTS: int(fields[20]),
-                v.DATA_TOTAL_BURNER_HOURS: int(fields[21]),
-                v.DATA_CH_PUMP_HOURS: int(fields[22]),
-                v.DATA_DHW_PUMP_HOURS: int(fields[23]),
-                v.DATA_DHW_BURNER_HOURS: int(fields[24]),
-            }
-        self.status.submit_full_update({v.BOILER: status, v.THERMOSTAT: status})
+            boiler_status, thermostat_status = process_statusfields_v4(fields)
+        self.status.submit_full_update({
+            v.BOILER: boiler_status,
+            v.THERMOSTAT: thermostat_status
+        })
         return self.status.status
 
     async def set_hot_water_ovrd(self, state, timeout=v.OTGW_DEFAULT_TIMEOUT):
         """
         Control the domestic hot water enable option. If the boiler has
         been configured to let the room unit control when to keep a
         small amount of water preheated, this command can influence
@@ -777,14 +659,31 @@
         if ret is None:
             return
         ret = int(ret)
         status_boiler[v.DATA_COOLING_CONTROL] = ret
         self.status.submit_partial_update(v.BOILER, status_boiler)
         return ret
 
+    async def send_transparent_command(
+        self, cmd, state, timeout=v.OTGW_DEFAULT_TIMEOUT
+    ):
+        """
+        Sends custom otgw commands throug a transparent interface.
+        Check https://otgw.tclcode.com/firmware.html for supported commands.
+        @cmd the supported command e.g. 'SC' (set time/day)
+        @state the command argument e.g. '23:59/4' (the current time/day)
+        Returns the gateway response, which should be equal to @state.
+
+        Note that unlike the set_* methods, this does not update the status object.
+
+        This method is a coroutine
+        """
+        ret = await self._wait_for_cmd(cmd, state, timeout)
+        return ret
+
     def subscribe(self, coro):
         """
         Subscribe to status updates from the Opentherm Gateway.
         Can only be used after connect()
         @coro is a coroutine which will be called with a single
         argument (status) when a status change occurs.
         Return True on success, False if not connected or already
@@ -861,7 +760,154 @@
                     _LOGGER.debug("GPIO polling routine stopped")
 
             _LOGGER.debug("Starting GPIO polling routine")
             self._gpio_task = asyncio.get_running_loop().create_task(polling_routine())
         elif not poll and self._gpio_task is not None:
             _LOGGER.debug("Stopping GPIO polling routine")
             self._gpio_task.cancel()
+
+
+def process_statusfields_v4(status_fields):
+    """
+    Process the fields of a split status line for OpenTherm Gateway firmware
+    version <5.0.
+    
+    Return a tuple of (boiler_status, thermostat_status).
+    """
+    device_status = status_fields[0].split("/")
+    master_status = device_status[0]
+    slave_status = device_status[1]
+    remote_params = status_fields[2].split("/")
+    capmodlimits = status_fields[4].split("/")
+    dhw_setp_bounds = status_fields[13].split("/")
+    ch_setp_bounds = status_fields[14].split("/")
+    thermostat_status = {
+        v.DATA_MASTER_CH_ENABLED: int(master_status[7]),
+        v.DATA_MASTER_DHW_ENABLED: int(master_status[6]),
+        v.DATA_MASTER_COOLING_ENABLED: int(master_status[5]),
+        v.DATA_MASTER_OTC_ENABLED: int(master_status[4]),
+        v.DATA_MASTER_CH2_ENABLED: int(master_status[3]),
+        v.DATA_CONTROL_SETPOINT: float(status_fields[1]),
+        v.DATA_ROOM_SETPOINT: float(status_fields[5]),
+        v.DATA_ROOM_TEMP: float(status_fields[8]),
+    }
+    boiler_status = {
+        v.DATA_SLAVE_FAULT_IND: int(slave_status[7]),
+        v.DATA_SLAVE_CH_ACTIVE: int(slave_status[6]),
+        v.DATA_SLAVE_DHW_ACTIVE: int(slave_status[5]),
+        v.DATA_SLAVE_FLAME_ON: int(slave_status[4]),
+        v.DATA_SLAVE_COOLING_ACTIVE: int(slave_status[3]),
+        v.DATA_SLAVE_CH2_ACTIVE: int(slave_status[2]),
+        v.DATA_SLAVE_DIAG_IND: int(slave_status[1]),
+        v.DATA_REMOTE_TRANSFER_DHW: int(remote_params[0][7]),
+        v.DATA_REMOTE_TRANSFER_MAX_CH: int(remote_params[0][6]),
+        v.DATA_REMOTE_RW_DHW: int(remote_params[1][7]),
+        v.DATA_REMOTE_RW_MAX_CH: int(remote_params[1][6]),
+        v.DATA_SLAVE_MAX_RELATIVE_MOD: float(status_fields[3]),
+        v.DATA_SLAVE_MAX_CAPACITY: int(capmodlimits[0]),
+        v.DATA_SLAVE_MIN_MOD_LEVEL: int(capmodlimits[1]),
+        v.DATA_REL_MOD_LEVEL: float(status_fields[6]),
+        v.DATA_CH_WATER_PRESS: float(status_fields[7]),
+        v.DATA_CH_WATER_TEMP: float(status_fields[9]),
+        v.DATA_DHW_TEMP: float(status_fields[10]),
+        v.DATA_OUTSIDE_TEMP: float(status_fields[11]),
+        v.DATA_RETURN_WATER_TEMP: float(status_fields[12]),
+        v.DATA_SLAVE_DHW_MAX_SETP: int(dhw_setp_bounds[0]),
+        v.DATA_SLAVE_DHW_MIN_SETP: int(dhw_setp_bounds[1]),
+        v.DATA_SLAVE_CH_MAX_SETP: int(ch_setp_bounds[0]),
+        v.DATA_SLAVE_CH_MIN_SETP: int(ch_setp_bounds[1]),
+        v.DATA_DHW_SETPOINT: float(status_fields[15]),
+        v.DATA_MAX_CH_SETPOINT: float(status_fields[16]),
+        v.DATA_TOTAL_BURNER_STARTS: int(status_fields[17]),
+        v.DATA_CH_PUMP_STARTS: int(status_fields[18]),
+        v.DATA_DHW_PUMP_STARTS: int(status_fields[19]),
+        v.DATA_DHW_BURNER_STARTS: int(status_fields[20]),
+        v.DATA_TOTAL_BURNER_HOURS: int(status_fields[21]),
+        v.DATA_CH_PUMP_HOURS: int(status_fields[22]),
+        v.DATA_DHW_PUMP_HOURS: int(status_fields[23]),
+        v.DATA_DHW_BURNER_HOURS: int(status_fields[24]),
+    }
+    return (boiler_status, thermostat_status)
+
+
+def process_statusfields_v5(status_fields):
+    """
+    Process the fields of a split status line for OpenTherm Gateway firmware
+    version >=5.0.
+    
+    Return a tuple of (boiler_status, thermostat_status).
+    """
+    device_status = status_fields[0].split("/")
+    master_status = device_status[0]
+    slave_status = device_status[1]
+    remote_params = status_fields[2].split("/")
+    capmodlimits = status_fields[6].split("/")
+    dhw_setp_bounds = status_fields[19].split("/")
+    ch_setp_bounds = status_fields[20].split("/")
+    vh_device_status = status_fields[23].split("/")
+    vh_master_status = vh_device_status[0]
+    vh_slave_status = vh_device_status[1]
+    thermostat_status = {
+        v.DATA_MASTER_CH_ENABLED: int(master_status[7]),
+        v.DATA_MASTER_DHW_ENABLED: int(master_status[6]),
+        v.DATA_MASTER_COOLING_ENABLED: int(master_status[5]),
+        v.DATA_MASTER_OTC_ENABLED: int(master_status[4]),
+        v.DATA_MASTER_CH2_ENABLED: int(master_status[3]),
+        v.DATA_CONTROL_SETPOINT: float(status_fields[1]),
+        v.DATA_ROOM_SETPOINT: float(status_fields[7]),
+        v.DATA_COOLING_CONTROL: float(status_fields[3]),
+        v.DATA_CONTROL_SETPOINT_2: float(status_fields[4]),
+        v.DATA_ROOM_SETPOINT_2: float(status_fields[11]),
+        v.DATA_ROOM_TEMP: float(status_fields[12]),
+        v.DATA_VH_MASTER_VENT_ENABLED: int(vh_master_status[7]),
+        v.DATA_VH_MASTER_BYPASS_POS: int(vh_master_status[6]),
+        v.DATA_VH_MASTER_BYPASS_MODE: int(vh_master_status[5]),
+        v.DATA_VH_MASTER_FREE_VENT_MODE: int(vh_master_status[4]),
+        v.DATA_VH_CONTROL_SETPOINT: int(status_fields[24]),
+    }
+    boiler_status = {
+        v.DATA_SLAVE_FAULT_IND: int(slave_status[7]),
+        v.DATA_SLAVE_CH_ACTIVE: int(slave_status[6]),
+        v.DATA_SLAVE_DHW_ACTIVE: int(slave_status[5]),
+        v.DATA_SLAVE_FLAME_ON: int(slave_status[4]),
+        v.DATA_SLAVE_COOLING_ACTIVE: int(slave_status[3]),
+        v.DATA_SLAVE_CH2_ACTIVE: int(slave_status[2]),
+        v.DATA_SLAVE_DIAG_IND: int(slave_status[1]),
+        v.DATA_REMOTE_TRANSFER_DHW: int(remote_params[0][7]),
+        v.DATA_REMOTE_TRANSFER_MAX_CH: int(remote_params[0][6]),
+        v.DATA_REMOTE_RW_DHW: int(remote_params[1][7]),
+        v.DATA_REMOTE_RW_MAX_CH: int(remote_params[1][6]),
+        v.DATA_SLAVE_MAX_RELATIVE_MOD: float(status_fields[5]),
+        v.DATA_SLAVE_MAX_CAPACITY: int(capmodlimits[0]),
+        v.DATA_SLAVE_MIN_MOD_LEVEL: int(capmodlimits[1]),
+        v.DATA_REL_MOD_LEVEL: float(status_fields[8]),
+        v.DATA_CH_WATER_PRESS: float(status_fields[9]),
+        v.DATA_DHW_FLOW_RATE: float(status_fields[10]),
+        v.DATA_CH_WATER_TEMP: float(status_fields[13]),
+        v.DATA_DHW_TEMP: float(status_fields[14]),
+        v.DATA_OUTSIDE_TEMP: float(status_fields[15]),
+        v.DATA_RETURN_WATER_TEMP: float(status_fields[16]),
+        v.DATA_CH_WATER_TEMP_2: float(status_fields[17]),
+        v.DATA_EXHAUST_TEMP: int(status_fields[18]),
+        v.DATA_SLAVE_DHW_MAX_SETP: int(dhw_setp_bounds[0]),
+        v.DATA_SLAVE_DHW_MIN_SETP: int(dhw_setp_bounds[1]),
+        v.DATA_SLAVE_CH_MAX_SETP: int(ch_setp_bounds[0]),
+        v.DATA_SLAVE_CH_MIN_SETP: int(ch_setp_bounds[1]),
+        v.DATA_DHW_SETPOINT: float(status_fields[21]),
+        v.DATA_MAX_CH_SETPOINT: float(status_fields[22]),
+        v.DATA_VH_SLAVE_FAULT_INDICATE: int(vh_slave_status[7]),
+        v.DATA_VH_SLAVE_VENT_MODE: int(vh_slave_status[6]),
+        v.DATA_VH_SLAVE_BYPASS_STATUS: int(vh_slave_status[5]),
+        v.DATA_VH_SLAVE_BYPASS_AUTO_STATUS: int(vh_slave_status[4]),
+        v.DATA_VH_SLAVE_FREE_VENT_STATUS: int(vh_slave_status[3]),
+        v.DATA_VH_SLAVE_DIAG_INDICATE: int(vh_slave_status[1]),
+        v.DATA_TOTAL_BURNER_STARTS: int(status_fields[26]),
+        v.DATA_CH_PUMP_STARTS: int(status_fields[27]),
+        v.DATA_DHW_PUMP_STARTS: int(status_fields[28]),
+        v.DATA_DHW_BURNER_STARTS: int(status_fields[29]),
+        v.DATA_TOTAL_BURNER_HOURS: int(status_fields[30]),
+        v.DATA_CH_PUMP_HOURS: int(status_fields[31]),
+        v.DATA_DHW_PUMP_HOURS: int(status_fields[32]),
+        v.DATA_DHW_BURNER_HOURS: int(status_fields[33]),
+        v.DATA_VH_RELATIVE_VENT: int(status_fields[25]),
+    }
+    return (boiler_status, thermostat_status)
```

### Comparing `pyotgw-2.1.3/pyotgw/status.py` & `pyotgw-2.2.0/pyotgw/status.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/pyotgw/vars.py` & `pyotgw-2.2.0/pyotgw/vars.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/pyotgw.egg-info/PKG-INFO` & `pyotgw-2.2.0/pyotgw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyotgw
-Version: 2.1.3
+Version: 2.2.0
 Summary: A library to interface with the opentherm gateway through serial or network connection.
 Home-page: https://github.com/mvn23/pyotgw
 Author: Milan van Nugteren
 Author-email: milan@network23.nl
 License: GPLv3+
 Keywords: opentherm gateway otgw
 Classifier: Development Status :: 5 - Production/Stable
@@ -370,14 +370,27 @@
 - __timeout__ The timeout for the request. Defaults to OTGW_DEFAULT_TIMEOUT (3 seconds).
 
 Return the newly accepted value, or `None` on failure.
 
 This method is a coroutine.
 
 ---
+##### OpenThermGateway.send_transparent_command(_self_, cmd, state, timeout=OTGW_DEFAULT_TIMEOUT)
+Send a transparent command.
+Sends custom commands through a transparent interface.
+Check https://otgw.tclcode.com/firmware.html for supported commands.
+This method supports the following arguments:
+- __cmd__ The supported command e.g. `SC` (set time/day).
+- __state__ The command argument e.g. `23:59/4` (the current time/day)
+
+Returns the gateway response, which should be equal __state__.
+
+This method is a coroutine.
+
+---
 ##### OpenThermGateway.subscribe(_self_, coro)
 Subscribe to status updates from the Opentherm Gateway.
 The subscribed coroutine must have the following signature:
 ```
 async def coro(status)
 ```
 Where `status` will be the full status dict containing the last known information from the OpenTherm Gateway.
```

### Comparing `pyotgw-2.1.3/setup.py` & `pyotgw-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyotgw",
-    version="2.1.3",
+    version="2.2.0",
     author="Milan van Nugteren",
     author_email="milan@network23.nl",
     description=(
         "A library to interface with the opentherm gateway through "
         "serial or network connection."
     ),
     license="GPLv3+",
     keywords="opentherm gateway otgw",
     url="https://github.com/mvn23/pyotgw",
     packages=["pyotgw"],
     python_requires=">=3.8",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
-    install_requires=["pyserial-asyncio"],
+    install_requires=["pyserial-asyncio-fast"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     ],
 )
```

### Comparing `pyotgw-2.1.3/tests/test_connection.py` & `pyotgw-2.2.0/tests/test_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         """Store args and kwargs each time we're called"""
         saved_args_list.append({"args": used_args, "kwargs": used_kwargs})
         return DEFAULT
 
     with patch(
         "pyotgw.protocol.OpenThermProtocol.init_and_wait_for_activity",
     ) as init_and_wait, patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         return_value=(pygw_proto.transport, pygw_proto),
         side_effect=save_args,
     ) as create_serial_connection:
         assert await pygw_conn._attempt_connect() == (pygw_proto.transport, pygw_proto)
 
     create_serial_connection.assert_called_once()
     assert len(saved_args_list) == 1
@@ -293,15 +293,15 @@
 @pytest.mark.asyncio
 async def test_attempt_connect_serialexception(caplog, pygw_conn):
     """Test ConnectionManager._attempt_connect() with SerialException"""
     loop = asyncio.get_running_loop()
     pygw_conn._port = "loop://"
 
     with patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         side_effect=serial.SerialException,
     ) as create_serial_connection, patch.object(
         pygw_conn,
         "_get_retry_timeout",
         return_value=0,
     ) as retry_timeout, caplog.at_level(
         logging.ERROR
@@ -330,15 +330,15 @@
     loop = asyncio.get_running_loop()
     pygw_conn._port = "loop://"
 
     pygw_proto.init_and_wait_for_activity = MagicMock(side_effect=asyncio.TimeoutError)
     pygw_proto.disconnect = MagicMock()
 
     with patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         return_value=(pygw_proto.transport, pygw_proto),
     ) as create_serial_connection, patch.object(
         pygw_conn,
         "_get_retry_timeout",
         return_value=0,
     ) as retry_timeout, caplog.at_level(
         logging.ERROR
@@ -358,14 +358,43 @@
 
         task.cancel()
         with pytest.raises(asyncio.CancelledError):
             await task
 
 
 @pytest.mark.asyncio
+async def test_attempt_connect_syntaxerror(caplog, pygw_conn, pygw_proto):
+    """Test ConnectionManager._attempt_connect() with SyntaxError"""
+    loop = asyncio.get_running_loop()
+    pygw_conn._port = "loop://"
+
+    pygw_proto.init_and_wait_for_activity = MagicMock(side_effect=SyntaxError)
+    pygw_proto.disconnect = MagicMock()
+
+    with patch(
+        "serial_asyncio_fast.create_serial_connection",
+        return_value=(pygw_proto.transport, pygw_proto),
+    ) as create_serial_connection, patch.object(
+        pygw_conn,
+        "_get_retry_timeout",
+        return_value=0,
+    ) as retry_timeout, caplog.at_level(
+        logging.ERROR
+    ):
+        task = loop.create_task(pygw_conn._attempt_connect())
+        with pytest.raises(SyntaxError):
+            await task
+
+        assert retry_timeout.call_count == 1
+        assert create_serial_connection.call_count >= 2
+        assert pygw_proto.disconnect.call_count >= 2
+        assert isinstance(pygw_conn._error, SyntaxError)
+
+
+@pytest.mark.asyncio
 async def test_cleanup(pygw_conn):
     """Test ConnectionManager._cleanup()"""
     pass  # with patch.object()
 
 
 def test_get_retry_timeout(pygw):
     """Test pyotgw._get_retry_timeout()"""
```

### Comparing `pyotgw-2.1.3/tests/test_messageprocessor.py` & `pyotgw-2.2.0/tests/test_messageprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -292,14 +292,42 @@
             v.BOILER: {},
             v.OTGW: {v.OTGW_THRM_DETECT: "I"},
             v.THERMOSTAT: {},
         }
     )
 
 
+@pytest.mark.asyncio
+async def test_quirk_trset_s2m(pygw_message_processor):
+    """Test MessageProcessor._quirk_trset_s2m()"""
+
+    async def empty_coroutine(stat):
+        return
+
+    with patch.object(
+        pygw_message_processor.status_manager,
+        "submit_partial_update"
+    ) as partial_update:
+        await pygw_message_processor._quirk_trset_s2m(
+            v.THERMOSTAT,
+            b"\x01",
+            b"\x02",
+        )
+        await pygw_message_processor._quirk_trset_s2m(
+            v.BOILER,
+            b"\x14",
+            b"\x80"
+        )
+
+    partial_update.assert_called_once_with(
+        v.BOILER,
+        {v.DATA_ROOM_SETPOINT: 20.5}
+    )
+
+
 def test_get_flag8(pygw_message_processor):
     """Test pygw._get_flag8()"""
     test_cases = (
         (
             int("00000001", 2).to_bytes(1, "big"),
             [1, 0, 0, 0, 0, 0, 0, 0],
         ),
```

### Comparing `pyotgw-2.1.3/tests/test_messages.py` & `pyotgw-2.2.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/tests/test_protocol.py` & `pyotgw-2.2.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `pyotgw-2.1.3/tests/test_pyotgw.py` & `pyotgw-2.2.0/tests/test_pyotgw.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         pygw,
         "get_status",
         return_value={},
     ), patch.object(pygw, "_poll_gpio") as poll_gpio, patch.object(
         pygw_proto,
         "init_and_wait_for_activity",
     ) as init_and_wait, patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         return_value=(pygw_proto.transport, pygw_proto),
     ), caplog.at_level(
         logging.DEBUG
     ):
         status = await pygw.connect("loop://")
 
         assert status == v.DEFAULT_STATUS
@@ -71,15 +71,15 @@
         return_value={},
     ) as get_status, patch.object(
         pygw, "_poll_gpio"
     ) as poll_gpio, patch.object(
         pygw_proto,
         "init_and_wait_for_activity",
     ) as init_and_wait, patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         return_value=(pygw_proto.transport, pygw_proto),
     ), caplog.at_level(
         logging.DEBUG
     ):
         status = await pygw.connect("loop://", skip_init=True)
 
         assert status == v.DEFAULT_STATUS
@@ -102,15 +102,15 @@
 
 @pytest.mark.asyncio
 async def test_connect_serialexception(caplog, pygw):
     """Test pyotgw.connect() with SerialException"""
     loop = asyncio.get_running_loop()
 
     with patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         side_effect=serial.serialutil.SerialException,
     ) as create_serial_connection, patch.object(
         pygw.connection,
         "_get_retry_timeout",
         return_value=0,
     ) as loops_done:
         task = loop.create_task(pygw.connect("loop://"))
@@ -133,15 +133,15 @@
         assert await task is False
 
 
 @pytest.mark.asyncio
 async def test_connect_cancel(pygw):
     """Test pyotgw.connect() with CancelledError"""
     with patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         side_effect=asyncio.CancelledError,
     ) as create_serial_connection:
         status = await pygw.connect("loop://")
 
     assert status is False
     create_serial_connection.assert_called_once()
 
@@ -157,15 +157,15 @@
     pygw_proto.disconnect = MagicMock()
 
     with patch.object(
         pygw.connection,
         "_get_retry_timeout",
         return_value=0,
     ) as loops_done, patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         return_value=(pygw_proto.transport, pygw_proto),
     ), caplog.at_level(
         logging.DEBUG
     ):
         task = loop.create_task(pygw.connect("loop://"))
         await called_x_times(loops_done, 2)
 
@@ -187,15 +187,15 @@
 
 @pytest.mark.asyncio
 async def test_disconnect_while_connecting(pygw):
     """Test pyotgw.disconnect()"""
     loop = asyncio.get_running_loop()
 
     with patch(
-        "serial_asyncio.create_serial_connection",
+        "serial_asyncio_fast.create_serial_connection",
         side_effect=serial.SerialException,
     ):
         task = loop.create_task(pygw.connect("loop://"))
 
         with patch(
             "pyotgw.protocol.OpenThermProtocol.disconnect"
         ) as protocol_disconnect:
@@ -847,14 +847,32 @@
         ],
         any_order=False,
     )
 
     update_status.assert_called_once_with(v.BOILER, {v.DATA_COOLING_CONTROL: 75})
 
 
+@pytest.mark.asyncio
+async def test_send_transparent_command(pygw):
+    """Test pyotgw.send_transparent_command()"""
+    with patch.object(
+        pygw,
+        "_wait_for_cmd",
+        side_effect=["CD"],
+    ) as wait_for_cmd:
+        assert await pygw.send_transparent_command("AB", "CD") == "CD"
+
+    assert wait_for_cmd.call_count == 1
+    wait_for_cmd.assert_has_awaits(
+        [
+            call("AB", "CD", v.OTGW_DEFAULT_TIMEOUT),
+        ],
+    )
+
+
 def test_subscribe_and_unsubscribe(pygw):
     """Test pyotgw.subscribe() and pyotgw.unsubscribe()"""
 
     async def empty_coroutine(status):
         return
 
     async def empty_coroutine_2(status):
```

### Comparing `pyotgw-2.1.3/tests/test_status.py` & `pyotgw-2.2.0/tests/test_status.py`

 * *Files identical despite different names*

