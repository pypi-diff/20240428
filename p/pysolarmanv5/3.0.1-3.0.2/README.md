# Comparing `tmp/pysolarmanv5-3.0.1.tar.gz` & `tmp/pysolarmanv5-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolarmanv5-3.0.1.tar", last modified: Wed Oct  4 22:20:05 2023, max compression
+gzip compressed data, was "pysolarmanv5-3.0.2.tar", last modified: Sat Apr 27 22:11:04 2024, max compression
```

## Comparing `pysolarmanv5-3.0.1.tar` & `pysolarmanv5-3.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-10-04 22:20:05.557040 pysolarmanv5-3.0.1/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1083 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/LICENSE
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4385 2023-10-04 22:20:05.557040 pysolarmanv5-3.0.1/PKG-INFO
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     3442 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/README.md
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1038 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/pyproject.toml
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-10-04 22:20:05.557040 pysolarmanv5-3.0.1/pysolarmanv5/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      358 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/pysolarmanv5/__init__.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    26520 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/pysolarmanv5/pysolarmanv5.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    17695 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/pysolarmanv5/pysolarmanv5_async.py
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-10-04 22:20:05.557040 pysolarmanv5-3.0.1/pysolarmanv5.egg-info/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4385 2023-10-04 22:20:05.000000 pysolarmanv5-3.0.1/pysolarmanv5.egg-info/PKG-INFO
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      360 2023-10-04 22:20:05.000000 pysolarmanv5-3.0.1/pysolarmanv5.egg-info/SOURCES.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        1 2023-10-04 22:20:05.000000 pysolarmanv5-3.0.1/pysolarmanv5.egg-info/dependency_links.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       35 2023-10-04 22:20:05.000000 pysolarmanv5-3.0.1/pysolarmanv5.egg-info/requires.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       13 2023-10-04 22:20:05.000000 pysolarmanv5-3.0.1/pysolarmanv5.egg-info/top_level.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       38 2023-10-04 22:20:05.557040 pysolarmanv5-3.0.1/setup.cfg
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-10-04 22:20:05.557040 pysolarmanv5-3.0.1/tests/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1329 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/tests/test_aio_solarman.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1061 2023-10-04 22:18:24.000000 pysolarmanv5-3.0.1/tests/test_solarman.py
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2024-04-27 22:11:04.369397 pysolarmanv5-3.0.2/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1083 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/LICENSE
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4385 2024-04-27 22:11:04.369397 pysolarmanv5-3.0.2/PKG-INFO
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     3442 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/README.md
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1224 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/pyproject.toml
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2024-04-27 22:11:04.365397 pysolarmanv5-3.0.2/pysolarmanv5/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      504 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/pysolarmanv5/__init__.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    28616 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/pysolarmanv5/pysolarmanv5.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    18667 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/pysolarmanv5/pysolarmanv5_async.py
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2024-04-27 22:11:04.365397 pysolarmanv5-3.0.2/pysolarmanv5.egg-info/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4385 2024-04-27 22:11:04.000000 pysolarmanv5-3.0.2/pysolarmanv5.egg-info/PKG-INFO
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      360 2024-04-27 22:11:04.000000 pysolarmanv5-3.0.2/pysolarmanv5.egg-info/SOURCES.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        1 2024-04-27 22:11:04.000000 pysolarmanv5-3.0.2/pysolarmanv5.egg-info/dependency_links.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       35 2024-04-27 22:11:04.000000 pysolarmanv5-3.0.2/pysolarmanv5.egg-info/requires.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       13 2024-04-27 22:11:04.000000 pysolarmanv5-3.0.2/pysolarmanv5.egg-info/top_level.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       38 2024-04-27 22:11:04.369397 pysolarmanv5-3.0.2/setup.cfg
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2024-04-27 22:11:04.365397 pysolarmanv5-3.0.2/tests/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1583 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/tests/test_aio_solarman.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1269 2024-04-27 22:09:52.000000 pysolarmanv5-3.0.2/tests/test_solarman.py
```

### Comparing `pysolarmanv5-3.0.1/LICENSE` & `pysolarmanv5-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-3.0.1/PKG-INFO` & `pysolarmanv5-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolarmanv5
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
 Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
 Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
```

### Comparing `pysolarmanv5-3.0.1/README.md` & `pysolarmanv5-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-3.0.1/pyproject.toml` & `pysolarmanv5-3.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pysolarmanv5"
-version = "3.0.1"
+version = "3.0.2"
 description = "A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 authors = [{name = "Jonathan McCrohan", email = "jmccrohan@gmail.com"}]
 keywords = ["solarman", "igen-tech", "modbus", "solar", "inverter", "solarmanv5"]
 classifiers = [
@@ -31,7 +31,19 @@
 
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["pysolarmanv5"]
+
+[tool.pylint.MAIN]
+ignore-paths='docs,examples,tests' 
+
+[tool.pylint."MESSAGES CONTROL"]
+# Reasons for disabling:
+# format: formatting is handled by black
+
+disable = [
+    "format",
+]
+
```

### Comparing `pysolarmanv5-3.0.1/pysolarmanv5/pysolarmanv5.py` & `pysolarmanv5-3.0.2/pysolarmanv5/pysolarmanv5.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """pysolarmanv5.py"""
+
 import queue
 import struct
 import socket
 import logging
 import selectors
 import platform
 from threading import Thread, Event
 from multiprocessing import Queue
 from typing import Any
 from random import randrange
 
 from umodbus.client.serial import rtu
 
 
-_WIN_PLATFORM = True if platform.system() == 'Windows' else False
+_WIN_PLATFORM = platform.system() == "Windows"
 
 
 class V5FrameError(Exception):
     """V5 Frame Validation Error"""
 
-    pass
-
 
 class NoSocketAvailableError(Exception):
     """No Socket Available Error"""
 
-    pass
-
 
+# pylint: disable-next=too-many-instance-attributes (R0902)
 class PySolarmanV5:
     """
     The PySolarmanV5 class establishes a TCP connection to a Solarman V5 data
     logging stick and exposes methods to send/receive Modbus RTU requests and
     responses.
 
     For more detailed information on the Solarman V5 Protocol, see
@@ -101,41 +99,39 @@
         self.socket_timeout = kwargs.get("socket_timeout", 60)
         self.v5_error_correction = kwargs.get("v5_error_correction", False)
         self.sequence_number = None
 
         if self.verbose:
             self.log.setLevel("DEBUG")
 
-        self._v5_frame_def()
-
-        self.sock: socket.socket = None  # noqa
-        self._poll: selectors.BaseSelector = None  # noqa
-        self._sock_fd: int = None  # noqa
-        self._auto_reconnect = False
-        self._data_queue: Queue = None  # noqa
-        self._data_wanted: Event = None  # noqa
-        self._reader_exit: Event = None  # noqa
-        self._reader_thr: Thread = None  # noqa
-        self._socket_setup(kwargs.get("socket"), kwargs.get("auto_reconnect", False))
-
-    def _v5_frame_def(self):
-        """Define and construct V5 request frame structure."""
+        # Define and construct V5 request frame structure.
         self.v5_start = bytes.fromhex("A5")
         self.v5_length = bytes.fromhex("0000")  # placeholder value
         self.v5_controlcode = struct.pack("<H", 0x4510)
         self.v5_serial = bytes.fromhex("0000")  # placeholder value
         self.v5_loggerserial = struct.pack("<I", self.serial)
         self.v5_frametype = bytes.fromhex("02")
         self.v5_sensortype = bytes.fromhex("0000")
         self.v5_deliverytime = bytes.fromhex("00000000")
         self.v5_powerontime = bytes.fromhex("00000000")
         self.v5_offsettime = bytes.fromhex("00000000")
         self.v5_checksum = bytes.fromhex("00")  # placeholder value
         self.v5_end = bytes.fromhex("15")
 
+        self.sock: socket.socket = None  # noqa
+        self._poll: selectors.BaseSelector = None  # noqa
+        self._sock_fd: int = None  # noqa
+        self._auto_reconnect = False
+        self._data_queue: Queue = None  # noqa
+        self._data_wanted: Event = None  # noqa
+        self._reader_exit: Event = None  # noqa
+        self._reader_thr: Thread = None  # noqa
+        self._last_frame: bytes = b""
+        self._socket_setup(kwargs.get("socket"), kwargs.get("auto_reconnect", False))
+
     @staticmethod
     def _calculate_v5_frame_checksum(frame):
         """Calculate checksum on all frame bytes except head, end and checksum
 
         :param frame: V5 frame
         :type frame: bytes
         :return: Checksum value of V5 frame
@@ -266,106 +262,148 @@
 
         :param data_logging_stick_frame: V5 frame to transmit
         :type data_logging_stick_frame: bytes
         :return: V5 frame received
         :rtype: bytes
 
         """
-        self.log.debug("SENT: " + data_logging_stick_frame.hex(" "))
+        self.log.debug("SENT: %s", data_logging_stick_frame.hex(" "))
         if not self._reader_thr.is_alive():
             raise NoSocketAvailableError("Connection already closed.")
         self.sock.sendall(data_logging_stick_frame)
         self._data_wanted.set()
+        self._last_frame = data_logging_stick_frame
+        v5_response = b""
         try:
             v5_response = self._data_queue.get(timeout=self.socket_timeout)
             if v5_response == b"":
                 raise NoSocketAvailableError("Connection closed on read")
             self._data_wanted.clear()
-        except TimeoutError:
+        except (queue.Empty, TimeoutError):
+            self.log.debug("Got exception when receiving frame", exc_info=True)
             raise
 
-        self.log.debug("RECD: " + v5_response.hex(" "))
+        self.log.debug("RECD: %s", v5_response.hex(" "))
         return v5_response
 
+    def _received_frame_is_valid(self, frame):
+        """Check that the frame is valid and that the serial number of the received
+        frame matches with the last sent one.
+        Ignore also any frames with control code 0x4710 (counter frame).
+        """
+        if not frame.startswith(self.v5_start):
+            self.log.debug("[%s] V5_MISMATCH: %s", self.serial, frame.hex(" "))
+            return False
+        if frame[5] != self.sequence_number:
+            self.log.debug("[%s] V5_SEQ_NO_MISMATCH: %s", self.serial, frame.hex(" "))
+            return False
+        if frame.startswith(self.v5_start + b"\x01\x00\x10\x47"):
+            self.log.debug("[%s] COUNTER: %s", self.serial, frame.hex(" "))
+            return False
+        return True
+
     def _data_receiver(self):
         self._poll.register(self.sock.fileno(), selectors.EVENT_READ)
         while True:
-            events = self._poll.select(.500)
+            events = self._poll.select(0.500)
             if self._reader_exit.is_set():
                 return
+            # pylint: disable-next=unused-variable.
             for event in events:
                 # We are registered only for inbound data on a single socket,
                 # so there is no need to check the (fileno, mask) tuples
                 try:
                     data = self.sock.recv(1024)
-                except ConnectionResetError:
-                    self.log.debug(f'[{self.serial}] Connection RESET by peer.')
+                except Exception:  # pylint: disable=broad-exception-caught
+                    # In the case of errors (peer reset, timeout, ...) set received data to empty to signal receive failure
+                    self.log.debug("[%s] Connection error", self.serial, exc_info=True)
                     data = b""
                 if data == b"":
-                    self.log.debug(f"[POLL] Socket closed. Reader thread exiting.")
+                    self.log.debug("[POLL] Socket closed. Reader thread exiting.")
                     if self._data_wanted.is_set():
+                        self._reconnect()
+                        if self.sock:
+                            self.log.debug(
+                                "[POLL] Data expected. Will retry the last request: %s",
+                                self._last_frame.hex(" "),
+                            )
+                            self.sock.sendall(self._last_frame)
+                            return
                         try:
                             self._data_queue.put_nowait(data)
                         except queue.Full:
                             pass
-                    self._reconnect()
+                    else:
+                        self._reconnect()
                     return
-                elif data.startswith(b"\xa5\x01\x00\x10G"):
-                    # Frame with control code 0x4710 - Counter frame
-                    self.log.debug(f'[{self.serial}] COUNTER: {data.hex(" ")}')
+                if not self._received_frame_is_valid(data):
                     continue
                 if self._data_wanted.is_set():
                     self._data_queue.put(data, timeout=self.socket_timeout)
                 else:
-                    self.log.debug("[POLL-DISCARDED] RECD: " + data.hex(" "))
+                    self.log.debug("[POLL-DISCARDED] RECD: %s", data.hex(" "))
 
     def _reconnect(self):
         """
         Reconnect to the data logger if needed
         """
-        if self._reader_thr.is_alive():
-            try:
-                self.sock.send(b"")
+
+        # Close the old socket. Closing failures can be ignored and just logged.
+        try:
+            if self.sock:
+                self.sock.shutdown(socket.SHUT_RDWR)
                 self.sock.close()
-            except OSError:
-                pass
+        except Exception:  # pylint: disable=broad-exception-caught
+            self.log.debug("Closing socket failed", exc_info=True)
+        finally:
+            self.sock = None
             self._reader_exit.set()
         if self._auto_reconnect:
             self.log.debug(
-                f"Auto-Reconnect enabled. Trying to establish a new connection"
+                "Auto-Reconnect enabled. Trying to establish a new connection"
             )
-            self._poll.unregister(self._sock_fd)
+            if self._sock_fd:
+                self._poll.unregister(self._sock_fd)
+                self._sock_fd = None
             self.sock = self._create_socket()
             if self.sock:
                 self._sock_fd = self.sock.fileno()
                 self._reader_exit.clear()
                 self._reader_thr = Thread(target=self._data_receiver, daemon=True)
                 self._reader_thr.start()
-                self.log.debug(f"Auto-Reconnect successful.")
+                self.log.debug("Auto-Reconnect successful.")
             else:
-                self.log.debug(f"No socket available! Reconnect failed.")
+                self.log.debug("No socket available! Reconnect failed.")
+                self.sock = None
         else:
             self.log.debug("Auto-Reconnect inactive.")
+            self.sock = None
 
     def disconnect(self) -> None:
         """
         Disconnect the socket and set a signal for the reader thread to exit
 
         :return: None
 
         """
         self._data_wanted.clear()
         self._reader_exit.set()
         try:
-            self.sock.send(b"")
-            self.sock.close()
-        except OSError:
-            pass
+            if self.sock:
+                self.sock.shutdown(socket.SHUT_RDWR)
+                self.sock.close()
+        except Exception:  # pylint: disable=broad-exception-caught
+            self.log.debug("Closing socket failed", exc_info=True)
+        finally:
+            self.sock = None
+
         self._reader_thr.join(0.5)
-        self._poll.unregister(self._sock_fd)
+        if self._sock_fd:
+            self._poll.unregister(self._sock_fd)
+            self._sock_fd = None
 
     def _send_receive_modbus_frame(self, mb_request_frame):
         """Encodes mb_frame, sends/receives v5_frame, decodes response
 
         :param mb_request_frame: Modbus RTU frame to transmit
         :type mb_request_frame: bytes
         :return: Modbus RTU frame received
@@ -393,14 +431,15 @@
     def _create_socket(self):
         """Creates and returns a socket"""
         try:
             sock = socket.create_connection(
                 (self.address, self.port), self.socket_timeout
             )
         except OSError:
+            self.log.debug("Socket creation failed", exc_info=True)
             return None
         return sock
 
     def _socket_setup(self, sock: Any, auto_reconnect: bool):
         """Socket setup method"""
         if isinstance(sock, socket.socket) or sock is None:
             self.sock = sock if sock else self._create_socket()
@@ -413,15 +452,15 @@
             self._sock_fd = self.sock.fileno()
             self._auto_reconnect = False if sock else auto_reconnect
             self._data_queue = Queue(maxsize=1)
             self._data_wanted = Event()
             self._reader_exit = Event()
             self._reader_thr = Thread(target=self._data_receiver, daemon=True)
             self._reader_thr.start()
-            self.log.debug(f"Socket setup completed... {self.sock}")
+            self.log.debug("Socket setup completed... %s", self.sock)
 
     @staticmethod
     def twos_complement(val, num_bits):
         """Calculate 2s Complement
 
         :param val: Value to calculate
         :type val: int
```

### Comparing `pysolarmanv5-3.0.1/pysolarmanv5/pysolarmanv5_async.py` & `pysolarmanv5-3.0.2/pysolarmanv5/pysolarmanv5_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """pysolarmanv5_async.py"""
+
 import asyncio
 from multiprocessing import Event
-from typing import Any
 from umodbus.client.serial import rtu
 from .pysolarmanv5 import NoSocketAvailableError, PySolarmanV5
 
+# Disable `invalid-overridden-method` rule. The class `PySolarmanV5Async` overrides
+# (=redefines) non-async methods from `PySolarmanV5`.
+# The override in this case is not a problem in practice.
+
+# This could be avoided by changing the class hierarchy.
+# One way would be to introduce a common base class for async and sync classes
+# that would capture attributes and common (internal) sync methods.
+
 
+# pylint: disable=invalid-overridden-method
 class PySolarmanV5Async(PySolarmanV5):
     """
     The PySolarmanV5Async class establishes a TCP connection to a Solarman V5 data
     logging stick on a call to connect() and exposes methods to send/receive
     Modbus RTU requests and responses asynchronously.
 
     For more detailed information on the Solarman V5 Protocol, see
@@ -62,16 +71,18 @@
         """
         loop = asyncio.get_running_loop()
         try:
             self.reader, self.writer = await asyncio.open_connection(
                 self.address, self.port
             )
             self.reader_task = loop.create_task(self._conn_keeper(), name="ConnKeeper")
-        except:
-            raise NoSocketAvailableError(f"Cannot open connection to {self.address}")
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            raise NoSocketAvailableError(
+                f"Cannot open connection to {self.address}"
+            ) from e
 
     async def reconnect(self) -> None:
         """
         Reconnect to the data logging stick. Called automatically if the auto-reconnect option is enabled
 
         :return: None
         :raises NoSocketAvailableError: When connection cannot be re-established
@@ -81,17 +92,25 @@
             if self.reader_task:
                 self.reader_task.cancel()
             self.reader, self.writer = await asyncio.open_connection(
                 self.address, self.port
             )
             loop = asyncio.get_running_loop()
             self.reader_task = loop.create_task(self._conn_keeper(), name="ConnKeeper")
-            self.log.debug(f"[{self.serial}] Successful reconnect")
-        except:
-            raise NoSocketAvailableError(f"Cannot open connection to {self.address}")
+            self.log.debug("[%s] Successful reconnect", self.serial)
+            if self.data_wanted_ev.is_set():
+                self.log.debug(
+                    "[%s] Data expected. Will retry the last request", self.serial
+                )
+                self.writer.write(self._last_frame)
+                await self.writer.drain()
+        except Exception as e:  # pylint: disable=broad-exception-caught::
+            raise NoSocketAvailableError(
+                f"Cannot open connection to {self.address}"
+            ) from e
 
     async def disconnect(self) -> None:
         """
         Disconnect the socket and set a signal for the reader thread to exit
 
         :return: None
 
@@ -104,15 +123,14 @@
     def _socket_setup(self, *args, **kwargs):
         """Socket setup method
 
         PySolarmanV5Async handles socket creation separately to base
         PySolarmanV5 class
 
         """
-        pass
 
     def _send_data(self, data: bytes):
         """
         Sends the data received from the socket to the receiver.
 
         :param data:
         :return:
@@ -132,36 +150,38 @@
 
         """
         while True:
             try:
                 data = await self.reader.read(1024)
             except ConnectionResetError:
                 self.log.debug(
-                    f"[{self.serial}] Connection reset. Closing the socket reader."
+                    "[%s] Connection reset. Closing the socket reader.",
+                    self.serial,
+                    exc_info=True,
                 )
                 break
             if data == b"":
                 self.log.debug(
-                    f"[{self.serial}] Connection closed by the remote. Closing the socket reader."
+                    "[%s] Connection closed by the remote. Closing the socket reader.",
+                    self.serial,
                 )
                 break
-            elif data.startswith(b"\xa5\x01\x00\x10G"):
-                # Frame with control code 0x4710 - Counter frame
-                self.log.debug(f'[{self.serial}] COUNTER: {data.hex(" ")}')
+            if not self._received_frame_is_valid(data):
                 continue
-            elif self.data_wanted_ev.is_set():
+            if self.data_wanted_ev.is_set():
                 self._send_data(data)
             else:
                 self.log.debug("Data received but nobody waits for it... Discarded")
         self.reader = None
         self.writer = None
-        self._send_data(b"")
+        # self._send_data(b"")
         if self._needs_reconnect:
             self.log.debug(
-                f"[{self.serial}] Auto reconnect enabled. Will try to restart the socket reader"
+                "[%s] Auto reconnect enabled. Will try to restart the socket reader",
+                self.serial,
             )
             loop = asyncio.get_running_loop()
             loop.create_task(self.reconnect())
 
     async def _send_receive_v5_frame(self, data_logging_stick_frame):
         """Send v5 frame to the data logger and receive response
 
@@ -170,35 +190,38 @@
         :return: V5 frame received
         :rtype: bytes
         :raises NoSocketAvailableError: When the connection to data logging stick is closed.
             Can occur even when auto-reconnect is enabled.
 
         """
 
-        self.log.debug("SENT: " + data_logging_stick_frame.hex(" "))
+        self.log.debug("SENT: %s", data_logging_stick_frame.hex(" "))
         self.data_wanted_ev.set()
+        self._last_frame = data_logging_stick_frame
         try:
             self.writer.write(data_logging_stick_frame)
             await self.writer.drain()
-            v5_response = await self.data_queue.get()
+            v5_response = await asyncio.wait_for(
+                self.data_queue.get(), self.socket_timeout
+            )
             if v5_response == b"":
                 raise NoSocketAvailableError(
                     "Connection closed on read. Retry if auto-reconnect is enabled"
                 )
-        except AttributeError:
-            raise NoSocketAvailableError("Connection already closed")
+        except AttributeError as exc:
+            raise NoSocketAvailableError("Connection already closed") from exc
         except NoSocketAvailableError:
             raise
         except Exception as exc:
-            self.log.exception(f"[{self.serial}] Send/Receive error: {exc}")
+            self.log.exception("[%s] Send/Receive error: %s", self.serial, exc)
             raise
         finally:
             self.data_wanted_ev.clear()
 
-        self.log.debug("RECD: " + v5_response.hex(" "))
+        self.log.debug("RECD: %s", v5_response.hex(" "))
         return v5_response
 
     async def _send_receive_modbus_frame(self, mb_request_frame):
         """Encodes mb_frame, sends/receives v5_frame, decodes response
 
         :param mb_request_frame: Modbus RTU frame to transmit
         :type mb_request_frame: bytes
```

### Comparing `pysolarmanv5-3.0.1/pysolarmanv5.egg-info/PKG-INFO` & `pysolarmanv5-3.0.2/pysolarmanv5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolarmanv5
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
 Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
 Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
```

### Comparing `pysolarmanv5-3.0.1/tests/test_solarman.py` & `pysolarmanv5-3.0.2/tests/test_solarman.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     # time.sleep(1)
     res = solarman.read_coils(30, 1)
     log.debug(f"[Sync-COILS] Logger response: {res}")
     assert len(res) > 0
     time.sleep(1)  # wait for auto-reconnect if enabled (see SolarmanServer)
     try:
         res = solarman.read_input_registers(40, 10)
+        res = solarman.read_input_registers(50, 10)
+        res = solarman.read_input_registers(60, 10)
     except NoSocketAvailableError:
         time.sleep(1)
         res = solarman.read_input_registers(40, 10)
+        res = solarman.read_input_registers(50, 10)
+        res = solarman.read_input_registers(60, 10)
     log.debug(f"[Sync-INPUT] Logger response: {res}")
     assert len(res) == 10
     solarman.disconnect()
     log.debug("[Sync] Disconnected!!!")
```

