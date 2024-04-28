# Comparing `tmp/robotframework_pyserial-1.0.0.tar.gz` & `tmp/robotframework_pyserial-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_pyserial-1.0.0.tar", last modified: Thu Apr 25 19:18:48 2024, max compression
+gzip compressed data, was "robotframework_pyserial-1.1.0.tar", last modified: Sun Apr 28 16:42:04 2024, max compression
```

## Comparing `robotframework_pyserial-1.0.0.tar` & `robotframework_pyserial-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:18:48.325291 robotframework_pyserial-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 19:18:43.000000 robotframework_pyserial-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-25 19:18:48.325291 robotframework_pyserial-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-25 19:18:43.000000 robotframework_pyserial-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-25 19:18:43.000000 robotframework_pyserial-1.0.0/Serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:18:48.325291 robotframework_pyserial-1.0.0/robotframework_pyserial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-25 19:18:48.000000 robotframework_pyserial-1.0.0/robotframework_pyserial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 19:18:48.000000 robotframework_pyserial-1.0.0/robotframework_pyserial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:18:48.000000 robotframework_pyserial-1.0.0/robotframework_pyserial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 19:18:48.000000 robotframework_pyserial-1.0.0/robotframework_pyserial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 19:18:48.000000 robotframework_pyserial-1.0.0/robotframework_pyserial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:18:48.325291 robotframework_pyserial-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-25 19:18:43.000000 robotframework_pyserial-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:42:04.863811 robotframework_pyserial-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 16:41:58.000000 robotframework_pyserial-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-28 16:42:04.863811 robotframework_pyserial-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-28 16:41:58.000000 robotframework_pyserial-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-28 16:41:58.000000 robotframework_pyserial-1.1.0/SerialLibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:42:04.863811 robotframework_pyserial-1.1.0/robotframework_pyserial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-28 16:42:04.000000 robotframework_pyserial-1.1.0/robotframework_pyserial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-28 16:42:04.000000 robotframework_pyserial-1.1.0/robotframework_pyserial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:42:04.000000 robotframework_pyserial-1.1.0/robotframework_pyserial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 16:42:04.000000 robotframework_pyserial-1.1.0/robotframework_pyserial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 16:42:04.000000 robotframework_pyserial-1.1.0/robotframework_pyserial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:42:04.863811 robotframework_pyserial-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-28 16:41:58.000000 robotframework_pyserial-1.1.0/setup.py
```

### Comparing `robotframework_pyserial-1.0.0/LICENSE` & `robotframework_pyserial-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_pyserial-1.0.0/Serial.py` & `robotframework_pyserial-1.1.0/SerialLibrary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=C0103
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,182 +14,256 @@
 #
 
 """
 Author: reharish@github
 Requirements: robotframework, pyserial
 """
 
-import serial
-
 from io import BytesIO
 
+import serial
+
 from serial import SerialException
 from robot.api.deco import keyword
 
 class PySerialError(Exception):
     """Represents the Serial exceptions"""
 
-class Serial:
+class SerialLibrary:
     """
     Library for interacting with serial devices.
 
     == Example ==
 
     | Serial.Connect | /dev/ttyUSB0 | 115200
     | Serial.Write   | Hello
     | ${DATA}=       | Serial.Read
+    | ${DATA}=       | Serial.Read All
     | Serial.Save Buffer to file |  /path/to/serial.log
 
     == Another Example ==
 
     | Connect     | /dev/ttyUSB1 | 115200
     | Set Timeout | 2
+    | Reset Input Buffer
+    | Reset Output Buffer
     | Write       | Hello
     | Write       | Hello
     | Read until  | World
+    | Read All
 
     """
 
+    ROBOT_LIBRARY_SCOPE = "GLOBAL"
     ROBOT_AUTO_KEYWORDS = False
 
     def __init__(self, unicode='utf-8'):
         """
         Initializes the Serial Library.
 
-        Arguments
-        - unicode - Unicode encoding for data communication.
+        ``unicode`` - Unicode encoding for data communication.
         """
         self.device = None
         self.timeout = 10
         self.unicode = unicode
         self.buffer = BytesIO()
 
     @keyword("Connect")
     def connect_to_serial(self, device: str, baudrate: int) -> serial.Serial:
         """
         Connects to a serial device.
 
-        Arguments:
-        - device: The device name or a device number.
-        - baudrate: The baud rate to use for communication.
+        ``device`` - The device name or a device number.
+
+        ``baudrate`` -  The baud rate to use for communication.
 
-        Returns:
-        - The connected serial device object.
+        === Example ===
+        | Connect  |   <device>   | <baudrate>
+        | Connect  | /dev/ttyUSB0 | 115200
+
+        === Returns ===
+        The connected serial device object.
         """
         try:
             self.device = serial.Serial(device, baudrate=baudrate)
         except SerialException as exc:
-            raise PySerialError(f"Failed to connect {device}: {exc}")
+            raise PySerialError(f"Failed to connect {device}: {exc}") from exc
         return self.device
 
     @keyword("Disconnect")
     def disconnect_from_serial(self):
         """
         Disconnects from the serial device.
+
+        === Example ===
+        | Disconnect
         """
         self.device.close()
 
     @keyword("Set Timeout")
     def set_timeout(self, seconds: int):
         """
         Sets the read timeout for the serial device.
 
-        Arguments:
-        - seconds: The timeout value in seconds.
+        ``seconds`` - The timeout value in seconds.
+
+        === Example ===
+        | Set Timeout  | <seconds>
+        | Set Timeout  |  10
         """
         if not self.device:
             raise PySerialError("Device not initialized to set timeout")
         self.device.timeout = seconds
 
     @keyword("Set Write Timeout")
-    def set_timeout_write(self, seconds: int):
+    def set_write_timeout(self, seconds: int):
         """
         Sets the write timeout for the serial device.
 
-        Arguments:
-        - seconds: The timeout value in seconds.
+        ``seconds`` - The timeout value in seconds.
+
+        === Example ===
+        | Set Write Timeout  | <seconds>
+        | Set Write Timeout  |  10
         """
         if not self.device:
             raise PySerialError("Device not connected to set write timeout")
         self.device.write_timeout = seconds
 
     @keyword("Set Unicode")
     def set_unicode(self, unicode: str):
         """
         Sets the Unicode encoding for data communication.
 
-        Arguments:
-        - unicode: The Unicode encoding to use.
+        ``unicode`` - The Unicode encoding to use.
+
+        === Example ===
+        | Set Unicode  | <unicode>
+        | Set Unicode  | utf-8
         """
         self.unicode = unicode
 
     @keyword("Read")
     def read(self) -> str:
         """
         Reads data from the serial device.
 
-        Returns:
-        - The read data as a string.
+        === Example ===
+        | Read
+
+        === Returns ===
+        The read data as a string.
         """
         if not self.device:
             raise PySerialError("Device not connected to start read")
         buff = self.device.read()
         self.buffer.write(buff)
         buff = buff.decode(self.unicode)
         return buff
 
     @keyword("Write")
     def write(self, data: str):
         """
         Writes data to the serial device.
 
-        Arguments:
-        - data: The data to write.
+        ``data`` - The data to write.
+
+        === Example ===
+        | Write
         """
         if not self.device:
             raise PySerialError("Device not connected to start write")
         try:
             self.device.write(data.encode())
         except SerialException as exc:
-            raise PySerialError(f"Failed to write to device: {exc}")
+            raise PySerialError(f"Failed to write to device: {exc}") from exc
 
     @keyword("Read until")
     def read_until(self, expected: str) -> str:
         """
         Reads data from the serial device until a specified string is encountered.
 
-        Arguments:
-        - expected: The string to read until.
+        ``expected`` - The string to read until.
 
-        Returns:
-        - The read data as a string.
+        === Example ===
+        | Read until  | <expected>
+        | Read until  | string
+
+        === Returns ===
+        The read data as a string.
         """
         if not self.device:
             raise PySerialError("Device not connected to start read")
         expected = expected.encode()
         buff = self.device.read_until(expected)
         self.buffer.write(buff)
         return buff.decode(self.unicode)
 
+    @keyword("Read all")
+    def read_all(self) -> str:
+        """
+        Reads all the data available in the buffer
+
+        === Example ===
+        | Read All
+
+        === Returns ===
+        The read data as a string.
+        """
+        if not self.device:
+            raise PySerialError("Device not connected to start read")
+        buff = self.device.read_all()
+        self.buffer.write(buff)
+        return buff.decode(self.unicode)
+
+    @keyword("Reset Input Buffer")
+    def reset_input_buffer(self):
+        """
+        Clear the input buffer for the serial device
+
+        === Example ===
+        | Reset Input Buffer
+        """
+        if not self.device:
+            raise PySerialError("Device not connected to reset buffer")
+        self.device.reset_input_buffer()
+
+    @keyword("Reset Output Buffer")
+    def reset_output_buffer(self):
+        """
+        Clear the output buffer for the serial device
+
+        === Example ===
+        | Reset Output Buffer
+        """
+        if not self.device:
+            raise PySerialError("Device not connected to reset buffer")
+        self.device.reset_output_buffer()
+
     @keyword("Close")
     def close_connection(self):
         """
         Closes the connection to the serial device.
+
+        === Example ===
+        | Close
         """
         if self.device:
             self.device.close()
             self.device = None
 
     @keyword("Save buffer to file")
     def save_into_file(self, outputfile: str):
         """
         Saves the data buffer into a file.
 
-        Arguments:
-        - outputfile: The path to the output file.
+        ``outputfile`` - The path to the output file.
+
+        === Example ===
+        | Save buffer to file  | <outputfile>
+        | Save buffer to file  | test.log
         """
         self.set_timeout(10)
-        buff = self.device.read()
-        self.buffer.write(buff)
+        self.read_all()
         with open(outputfile, 'wb+') as outf:
             outf.write(self.buffer.getvalue())
         print(f"File saved: {outputfile}")
```

### Comparing `robotframework_pyserial-1.0.0/setup.py` & `robotframework_pyserial-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), "r") as fd:
     long_description = fd.read()
 
 setup(
     name='robotframework-pyserial',
-    version='1.0.0',
+    version='1.1.0',
     description='Robotframework implementation of beloved pyserial module',
     license="Apache License 2.0",
     url="https://reharish.github.io/cv",
     author='reharish',
     author_email='rengarajharish@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(),
-    py_modules=['Serial'],
+    py_modules=['SerialLibrary'],
     install_requires=["robotframework", "pyserial"],
 )
```

