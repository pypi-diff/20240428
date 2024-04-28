# Comparing `tmp/midiscripter-0.1.1.tar.gz` & `tmp/midiscripter-0.1.2.tar.gz`

## Comparing `midiscripter-0.1.1.tar` & `midiscripter-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/base/__init__.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/base/msg_base.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/base/port_base.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/base/shared.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/cli/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/cli/starters.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/file_event/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/file_event/file_event_msg.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/file_event/file_event_port.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/__init__.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/app.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/log_widget.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/main_window.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/menu_bar.py
--rw-r--r--   0        0        0    13569 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/ports_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/__init__.py
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/button.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/gui_msg.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/gui_widget_base.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/layout.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/list.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/mixins.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/gui/gui_widgets/text.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/keyboard/__init__.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/keyboard/keyboard_msg.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/keyboard/keyboard_port.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/logger/__init__.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/logger/console_sink.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/logger/custom_logger.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/logger/html_sink.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/metronome/__init__.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/metronome/metronome_port.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/midi/__init__.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/midi/midi_msg.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/midi/midi_note_data.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/midi/midi_port.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/midi/midi_ports_update.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/osc/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/osc/osc_msg.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/osc/osc_port.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/osc/osc_query_maker.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/resources/icon.ico
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.1.1/midiscripter/resources/icon.svg
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 midiscripter-0.1.1/.gitignore
--rw-r--r--   0        0        0    35131 2020-02-02 00:00:00.000000 midiscripter-0.1.1/LICENSE
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 midiscripter-0.1.1/README.md
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 midiscripter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    45071 2020-02-02 00:00:00.000000 midiscripter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/__init__.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/msg_base.py
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/port_base.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/shared.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/cli/__init__.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/cli/starters.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/file_event/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/file_event/file_event_msg.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/file_event/file_event_port.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/__init__.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/app.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/log_widget.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/main_window.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/menu_bar.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/ports_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/__init__.py
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/button.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_msg.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_widget_base.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/layout.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/list.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/mixins.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/text.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/keyboard/__init__.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/keyboard/keyboard_msg.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/keyboard/keyboard_port.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/console_sink.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/html_sink.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/log.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/metronome/__init__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/metronome/metronome_port.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/__init__.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_msg.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_note_data.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_port.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_ports_update.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/__init__.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/osc_msg.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/osc_port.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/osc_query_maker.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/resources/icon.ico
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/resources/icon.svg
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 midiscripter-0.1.2/README.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 midiscripter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13761 2020-02-02 00:00:00.000000 midiscripter-0.1.2/PKG-INFO
```

### Comparing `midiscripter-0.1.1/midiscripter/base/port_base.py` & `midiscripter-0.1.2/midiscripter/base/port_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         Args:
             function: Subscribed callable.
             msg: Received message to use as callable only argument.
         """
         try:
             function(msg)
             self._call_statistics[function].append(msg._age_ms)
-        except TypeError:  # TODO TEST
+        except TypeError:
             function()
             self._call_statistics[function].append(msg._age_ms)
         except Exception as exc:
             log.red(''.join(traceback.format_exception(exc)))
 
 
 class Output(Port):
@@ -230,15 +230,15 @@
         with self._check_and_log_sent_message(msg):
             raise NotImplementedError
 
     @contextlib.contextmanager
     def _check_and_log_sent_message(self, msg: 'Msg'):
         if not self.is_enabled:
             log.red('Can\'t send message {msg}. {output} is disabled!', msg=msg, output=self)
-            return  # TODO TEST
+            return
 
         yield 
 
         if msg.source:
             log('{output} sent message {msg} received {age_ms} ms ago', 
                 output=self, msg=msg, age_ms=msg._age_ms)
         else:
```

### Comparing `midiscripter-0.1.1/midiscripter/base/shared.py` & `midiscripter-0.1.2/midiscripter/base/shared.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import os
-import sys
-import time
-import platform
-import __main__
-import concurrent.futures
-from typing import Callable
-
-
-if platform.system() == 'Windows':
-    import win32api
-    import win32con
-    import win32process
-
-
-try:
-    script_path = __main__.__file__
-except AttributeError:  # in subprocess
-    pass
-
-
-thread_executor = concurrent.futures.ThreadPoolExecutor(100)
-
-
-_precise_time_delta = time.time() - time.perf_counter()
-
-def precise_epoch_time():
-    """current time in epoch format with nanosecond precision"""
-    return _precise_time_delta + time.perf_counter()
-
-
-def restart_script():
-    """Exit and restart current script"""
-    os.execv(sys.executable, ['python'] + [script_path])
-    exit(0)
-
-
-def _raise_current_process_cpu_priority() -> None:
-    """Sets HIGH process priority in Windows for current python process"""
-    if platform.system() == 'Windows':
-        pid = win32api.GetCurrentProcessId()
-        handle = win32api.OpenProcess(win32con.PROCESS_ALL_ACCESS, True, pid)
-        win32process.SetPriorityClass(handle, win32process.HIGH_PRIORITY_CLASS)
-
-
-run_after_ports_open_subscribed_calls = []
-
-# A Decorator
-def run_after_ports_opened(function: Callable[[], None]) -> Callable:
-    """Decorator to subscribe a callable to run after all ports are opened at the script start
-
-    Args:
-        function: A callable with no arguments
-
-    Returns:
-        Subscribed callable.
-    """
-    if function not in run_after_ports_open_subscribed_calls:
-        run_after_ports_open_subscribed_calls.append(function)
-    return function
+import os
+import sys
+import time
+import platform
+import __main__
+import concurrent.futures
+from typing import Callable
+
+
+if platform.system() == 'Windows':
+    import win32api
+    import win32con
+    import win32process
+
+
+try:
+    script_path = __main__.__file__
+except AttributeError:  # in subprocess
+    pass
+
+
+thread_executor = concurrent.futures.ThreadPoolExecutor(100)
+
+
+_precise_time_delta = time.time() - time.perf_counter()
+
+def precise_epoch_time():
+    """current time in epoch format with nanosecond precision"""
+    return _precise_time_delta + time.perf_counter()
+
+
+def restart_script():
+    """Exit and restart current script"""
+    os.execv(sys.executable, ['python'] + [script_path])
+    exit(0)
+
+
+def _raise_current_process_cpu_priority() -> None:
+    """Sets HIGH process priority in Windows for current python process"""
+    if platform.system() == 'Windows':
+        pid = win32api.GetCurrentProcessId()
+        handle = win32api.OpenProcess(win32con.PROCESS_ALL_ACCESS, True, pid)
+        win32process.SetPriorityClass(handle, win32process.HIGH_PRIORITY_CLASS)
+
+
+run_after_ports_open_subscribed_calls = []
+
+# A Decorator
+def run_after_ports_opened(function: Callable[[], None]) -> Callable:
+    """Decorator to subscribe a callable to run after all ports are opened at the script start
+
+    Args:
+        function: A callable with no arguments
+
+    Returns:
+        Subscribed callable.
+    """
+    if function not in run_after_ports_open_subscribed_calls:
+        run_after_ports_open_subscribed_calls.append(function)
+    return function
```

### Comparing `midiscripter-0.1.1/midiscripter/cli/starters.py` & `midiscripter-0.1.2/midiscripter/cli/starters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import time
-from typing import NoReturn
-
-import midiscripter.base.shared
-import midiscripter.base.port_base
-import midiscripter.logger.console_sink
-import midiscripter.midi
-import midiscripter.logger.custom_logger
-from midiscripter.logger import log  
-
-
-def start_cli_debug() -> NoReturn:
-    """Starts the script with log output to console.
-    Console prints increase latency and jitter. Use for debugging only.
-    """
-    log._sink = midiscripter.logger.console_sink.ConsoleSink()
-    log('')
-    log('Available MIDI inputs:')
-    [log('{input}', input=port_name) for port_name in midiscripter.midi.MidiIn._available_names]
-    log('')
-    log('Available MIDI outputs:')
-    [log('{output}', output=port_name) for port_name in midiscripter.midi.MidiOut._available_names]
-    log('')
-    _run_cli_loop()
-
-
-def start_silent() -> NoReturn:
-    """Starts the script without logging. The fastest way to run the script.
-        """
-    log.is_enabled = False
-    _run_cli_loop()
-
-
-def _run_cli_loop() -> NoReturn:
-    """Opens the ports and loops until broken by user."""
-    midiscripter.base.shared._raise_current_process_cpu_priority()
-    with midiscripter.base.port_base._all_opened():
-        while True:
-            try:
-                time.sleep(1)
-            except (KeyboardInterrupt, SystemExit):
-                break
+import time
+from typing import NoReturn
+
+import midiscripter.base.shared
+import midiscripter.base.port_base
+import midiscripter.logger.console_sink
+import midiscripter.midi
+import midiscripter.logger.log
+from midiscripter.logger import log  
+
+
+def start_cli_debug() -> NoReturn:
+    """Starts the script with log output to console.
+    Console prints increase latency and jitter. Use for debugging only.
+    """
+    log._sink = midiscripter.logger.console_sink.ConsoleSink()
+    log('')
+    log('Available MIDI inputs:')
+    [log('{input}', input=port_name) for port_name in midiscripter.midi.MidiIn._available_names]
+    log('')
+    log('Available MIDI outputs:')
+    [log('{output}', output=port_name) for port_name in midiscripter.midi.MidiOut._available_names]
+    log('')
+    _run_cli_loop()
+
+
+def start_silent() -> NoReturn:
+    """Starts the script without logging. The fastest way to run the script.
+        """
+    log.is_enabled = False
+    _run_cli_loop()
+
+
+def _run_cli_loop() -> NoReturn:
+    """Opens the ports and loops until broken by user."""
+    midiscripter.base.shared._raise_current_process_cpu_priority()
+    with midiscripter.base.port_base._all_opened():
+        while True:
+            try:
+                time.sleep(1)
+            except (KeyboardInterrupt, SystemExit):
+                break
```

### Comparing `midiscripter-0.1.1/midiscripter/file_event/file_event_msg.py` & `midiscripter-0.1.2/midiscripter/file_event/file_event_msg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,44 @@
-import pathlib
-from typing import TYPE_CHECKING, Union
-
-import midiscripter.base.msg_base
-
-if TYPE_CHECKING:
-    from midiscripter.file_event.file_event_port import FileEventIn
-
-
-class FileEventType(midiscripter.base.msg_base.AttrEnum):
-    # Names are hardcoded, equal watchdog's event types
-    MOVED = 'MOVED'
-    DELETED = 'DELETED'
-    CREATED = 'CREATED'
-    MODIFIED = 'MODIFIED'
-    CLOSED = 'CLOSED'
-    OPENED = 'OPENED'
-
-
-class FileEventMsg(midiscripter.base.msg_base.Msg):
-    ___match_args__ = ('type', 'path')
-
-    def __init__(self, type: Union[FileEventType, str], path: pathlib.Path,
-                 *, source: 'FileEventIn' = None):
-        super().__init__(type, source)
-        self.type = type
-        self.path = path
-
-    def matches(self, type=None, path=None):
-        return super().matches(type, path)
+import pathlib
+from typing import TYPE_CHECKING, Union, Optional
+
+import midiscripter.base.msg_base
+
+if TYPE_CHECKING:
+    from midiscripter.file_event.file_event_port import FileEventIn
+
+
+class FileEventType(midiscripter.base.msg_base.AttrEnum):
+    # Names are hardcoded, equal watchdog's event types
+    MOVED = 'MOVED'
+    DELETED = 'DELETED'
+    CREATED = 'CREATED'
+    MODIFIED = 'MODIFIED'
+    CLOSED = 'CLOSED'
+    OPENED = 'OPENED'
+
+
+class FileEventMsg(midiscripter.base.msg_base.Msg):
+    ___match_args__ = ('type', 'path')
+    
+    type: FileEventType
+    """File event type"""
+    
+    path: pathlib.Path
+    """File path of event"""
+    
+    source: Optional['FileEventIn']
+
+    def __init__(self, type: Union[FileEventType, str], path: pathlib.Path,
+                 *, source: Optional['FileEventIn'] = None):
+        """
+        Args:
+            type: File event type
+            path: File path
+            source (FileEventIn): The [`FileEventIn`][midiscripter.FileEventIn] instance that generated the message
+        """
+        super().__init__(type, source)
+        self.type = type
+        self.path = path
+
+    def matches(self, type=None, path=None):
+        return super().matches(type, path)
```

### Comparing `midiscripter-0.1.1/midiscripter/file_event/file_event_port.py` & `midiscripter-0.1.2/midiscripter/file_event/file_event_port.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import pathlib
-from typing import Union
-
-import watchdog.events
-import watchdog.observers
-
-import midiscripter.base.port_base
-import midiscripter.file_event
-import midiscripter.logger
-
-
-shared_observer = watchdog.observers.Observer()
-shared_observer.daemon = True
-shared_observer.start()
-
-
-class FileEventIn(midiscripter.base.port_base.Input, watchdog.events.FileSystemEventHandler):
-    """File system events input port. Watches file/directory modifications.
-    Produces [`FileEventMsg`][midiscripter.FileEventMsg] objects.
-    """
-    def __init__(self, path: Union[str, pathlib.Path], recursive: bool = False):
-        """
-        Args:
-            path: File/directory path to watch
-            recursive: `True` to watch directory path recursively
-        """
-        if isinstance(path, str):
-            path = pathlib.Path(path)
-
-        midiscripter.base.port_base.Input.__init__(self, path)
-        watchdog.events.FileSystemEventHandler.__init__(self)
-
-        self.__path = path
-
-        if self.__path.is_dir():
-            self.__path_to_watch = self.__path
-            self.__watch_dir_changes = True
-        else:
-            self.__path_to_watch = self.__path.parent  # some editors recreate a file on save
-            self.__watch_dir_changes = False
-
-        self.__recursive = recursive
-        self.__watch = None
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}('{str(self._uid)}')"
-
-    def __str__(self):
-        return f"'{self.__path.relative_to(self.__path.parent.parent)}' watcher"
-
-    def _open(self) -> None:
-        self.__watch = shared_observer.schedule(self, str(self.__path_to_watch),
-                                                self.__recursive)
-        if not shared_observer.is_alive():
-            shared_observer.start()
-        self.is_enabled = True
-        midiscripter.logger.log('Opened {input}', input=self)
-
-    def _close(self) -> None:
-        if self.__watch:
-            shared_observer.unschedule(self.__watch)
-        self.is_enabled = False
-        midiscripter.logger.log('Stopped {input}', input=self)
-
-    def on_any_event(self, event: watchdog.events.FileSystemEvent) -> None:
-        # Override of `watchdog.events.FileSystemEventHandler` method.
-        # Runs on each file system change in `_path`.
-        if not self.is_enabled:
-            return
-
-        event_path = pathlib.Path(event.src_path)
-
-        if self.__watch_dir_changes or event_path == self.__path:
-            msg = midiscripter.file_event.file_event_msg.FileEventMsg(event.event_type.upper(),
-                                                                      self.__path, source=self)
-            self._send_input_msg_to_calls(msg)
+import pathlib
+from typing import Union
+
+import watchdog.events
+import watchdog.observers
+
+import midiscripter.base.port_base
+import midiscripter.file_event
+import midiscripter.logger
+
+
+shared_observer = watchdog.observers.Observer()
+shared_observer.daemon = True
+shared_observer.start()
+
+
+class FileEventIn(midiscripter.base.port_base.Input, watchdog.events.FileSystemEventHandler):
+    """File system events input port. Watches file/directory modifications.
+    Produces [`FileEventMsg`][midiscripter.FileEventMsg] objects.
+    """
+    def __init__(self, path: Union[str, pathlib.Path], recursive: bool = False):
+        """
+        Args:
+            path: File/directory path to watch
+            recursive: `True` to watch directory path recursively
+        """
+        if isinstance(path, str):
+            path = pathlib.Path(path)
+
+        midiscripter.base.port_base.Input.__init__(self, path)
+        watchdog.events.FileSystemEventHandler.__init__(self)
+
+        self.__path = path
+
+        if self.__path.is_dir():
+            self.__path_to_watch = self.__path
+            self.__watch_dir_changes = True
+        else:
+            self.__path_to_watch = self.__path.parent  # some editors recreate a file on save
+            self.__watch_dir_changes = False
+
+        self.__recursive = recursive
+        self.__watch = None
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{str(self._uid)}')"
+
+    def __str__(self):
+        return f"'{self.__path.relative_to(self.__path.parent.parent)}' watcher"
+
+    def _open(self) -> None:
+        self.__watch = shared_observer.schedule(self, str(self.__path_to_watch),
+                                                self.__recursive)
+        if not shared_observer.is_alive():
+            shared_observer.start()
+        self.is_enabled = True
+        midiscripter.logger.log('Opened {input}', input=self)
+
+    def _close(self) -> None:
+        if self.__watch:
+            shared_observer.unschedule(self.__watch)
+        self.is_enabled = False
+        midiscripter.logger.log('Stopped {input}', input=self)
+
+    def on_any_event(self, event: watchdog.events.FileSystemEvent) -> None:
+        # Override of `watchdog.events.FileSystemEventHandler` method.
+        # Runs on each file system change in `_path`.
+        if not self.is_enabled:
+            return
+
+        event_path = pathlib.Path(event.src_path)
+
+        if self.__watch_dir_changes or event_path == self.__path:
+            msg = midiscripter.file_event.file_event_msg.FileEventMsg(event.event_type.upper(),
+                                                                      self.__path, source=self)
+            self._send_input_msg_to_calls(msg)
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/app.py` & `midiscripter-0.1.2/midiscripter/gui/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,109 @@
-import sys
-import time
-import signal
-import pathlib
-import platform
-from typing import NoReturn
-
-from PySide6.QtCore import *
-from PySide6.QtGui import *
-from PySide6.QtWidgets import *
-
-import midiscripter.base.shared
-import midiscripter.base.port_base
-import midiscripter.gui.main_window
-import midiscripter.midi.midi_ports_update
-import midiscripter.file_event.file_event_msg
-
-
-class ScripterGUI(QApplication):
-    request_restart = Signal()
-
-    RESTART_DELAY = 2
-    widgets_to_add = []
-
-    def __init__(self):
-        super().__init__()
-        self.setOrganizationName('MIDI Scripter')
-        self.setApplicationName(pathlib.Path(midiscripter.base.shared.script_path).name)
-        icon_path = pathlib.Path(midiscripter.__file__).parent / 'resources' / 'icon.ico'
-        self.setWindowIcon(QIcon(str(icon_path)))
-
-        self.__time_until_restart_sec = self.RESTART_DELAY
-        self.request_restart.connect(self.restart)
-        self.aboutToQuit.connect(self.__cleanup)
-
-    def prepare_main_window(self, minimized_to_tray: bool = False):
-        self.main_window = midiscripter.gui.main_window.MainWindow(self.widgets_to_add)
-        
-        if not minimized_to_tray:
-            self.main_window.show_from_tray()
-        else:
-            self.main_window.close()  # for always on top windows FIXME
-            
-    def restart_at_file_change(self, msg: 'midiscripter.file_event.file_change_msg.FileEventMsg'):
-        if msg.type not in (midiscripter.file_event.file_event_msg.FileEventType.CREATED,
-                            midiscripter.file_event.file_event_msg.FileEventType.MODIFIED):
-            return
-
-        self.__time_until_restart_sec = self.RESTART_DELAY
-        sleep_step_sec = 0.1
-
-        while self.__time_until_restart_sec > 0:
-            time.sleep(sleep_step_sec)
-            self.__time_until_restart_sec -= sleep_step_sec
-
-        self.request_restart.emit()
-
-    def restart(self):
-        if pathlib.Path(midiscripter.base.shared.script_path).is_file():
-            # These settings saved only for restart
-            self.processEvents()  # update win status to get correct active status
-            QSettings().setValue('restart win active', int(self.main_window.isActiveWindow()))
-            QSettings().setValue('restart win minimized', int(self.main_window.isMinimized()))
-            QSettings().setValue('restart closed to tray', int(not self.main_window.isVisible()))
-            self.exit(1467)
-
-    def __cleanup(self):
-        self.main_window.close()
-        self.main_window.tray.hide()
-
-
-# Creating app at import to allow QWidget instance init in other modules
-app_instance = ScripterGUI()
-
-
-def add_qwidget(qwidget: QWidget):
-    """Add custom pyside6 QWidget to the GUI"""
-    if qwidget not in midiscripter.gui.app.ScripterGUI.widgets_to_add:
-        midiscripter.gui.app.ScripterGUI.widgets_to_add.append(qwidget)
-
-
-def remove_qwidget(qwidget: QWidget):
-    """Remove custom pyside6 QWidget to the GUI"""
-    try:
-        midiscripter.gui.app.ScripterGUI.widgets_to_add.remove(qwidget)
-    except ValueError:
-        pass
-
-
-def start_gui() -> NoReturn:
-    """Starts the script and runs GUI. Logging goes to GUI Log widget."""
-    midiscripter.base.shared._raise_current_process_cpu_priority()
-
-    sigint_exit_code = {'Windows': -1073741510, 'Linux': 130, 'Darwin': 2}[platform.system()]
-    signal.signal(signal.SIGINT, lambda *_: app_instance.exit(sigint_exit_code))
-    
-    signal_checker_dummy_timer = QTimer()  # runs python code from Qt to allow the signal to trigger
-    signal_checker_dummy_timer.start(1000)
-    signal_checker_dummy_timer.timeout.connect(lambda: None)  # dummy python code to run
-
-    start_minimized_to_tray = '--tray' in sys.argv
-
-    with midiscripter.base.port_base._all_opened():
-        app_instance.prepare_main_window(start_minimized_to_tray)
-        exit_status = app_instance.exec()
-
-    if exit_status == 1467:  # exit status for restart request
-        midiscripter.base.shared.restart_script()
-    else:
-        exit(exit_status)
+import sys
+import time
+import signal
+import pathlib
+import platform
+from typing import NoReturn
+
+from PySide6.QtCore import *
+from PySide6.QtGui import *
+from PySide6.QtWidgets import *
+
+import midiscripter.base.shared
+import midiscripter.base.port_base
+import midiscripter.gui.main_window
+import midiscripter.midi.midi_ports_update
+import midiscripter.file_event.file_event_msg
+
+
+class ScripterGUI(QApplication):
+    request_restart = Signal()
+
+    RESTART_DELAY = 2
+    widgets_to_add = []
+
+    def __init__(self):
+        super().__init__()
+        self.setOrganizationName('MIDI Scripter')
+        self.setApplicationName(pathlib.Path(midiscripter.base.shared.script_path).name)
+        icon_path = pathlib.Path(midiscripter.__file__).parent / 'resources' / 'icon.ico'
+        self.setWindowIcon(QIcon(str(icon_path)))
+
+        self.__time_until_restart_sec = self.RESTART_DELAY
+        self.request_restart.connect(self.restart)
+        self.aboutToQuit.connect(self.__cleanup)
+
+    def prepare_main_window(self, minimized_to_tray: bool = False):
+        self.main_window = midiscripter.gui.main_window.MainWindow(self.widgets_to_add)
+        
+        if not minimized_to_tray:
+            self.main_window.show_from_tray()
+        else:
+            self.main_window.close()
+            
+    def restart_at_file_change(self, msg: 'midiscripter.file_event.file_change_msg.FileEventMsg'):
+        if msg.type not in (midiscripter.file_event.file_event_msg.FileEventType.CREATED,
+                            midiscripter.file_event.file_event_msg.FileEventType.MODIFIED):
+            return
+
+        self.__time_until_restart_sec = self.RESTART_DELAY
+        sleep_step_sec = 0.1
+
+        while self.__time_until_restart_sec > 0:
+            time.sleep(sleep_step_sec)
+            self.__time_until_restart_sec -= sleep_step_sec
+
+        self.request_restart.emit()
+
+    def restart(self):
+        if pathlib.Path(midiscripter.base.shared.script_path).is_file():
+            # These settings saved only for restart
+            self.processEvents()  # update win status to get correct status
+            QSettings().setValue('restart win minimized', int(self.main_window.isMinimized()))
+            QSettings().setValue('restart closed to tray', int(not self.main_window.isVisible()))
+            self.exit(1467)
+
+    def __cleanup(self):
+        self.main_window.close()
+        self.main_window.tray.hide()
+
+
+# Creating app at import to allow QWidget instance init in other modules
+app_instance = ScripterGUI()
+
+
+def add_qwidget(qwidget: QWidget):
+    """Add custom pyside6 QWidget to the GUI"""
+    if qwidget not in midiscripter.gui.app.ScripterGUI.widgets_to_add:
+        midiscripter.gui.app.ScripterGUI.widgets_to_add.append(qwidget)
+
+
+def remove_qwidget(qwidget: QWidget):
+    """Remove custom pyside6 QWidget to the GUI"""
+    try:
+        midiscripter.gui.app.ScripterGUI.widgets_to_add.remove(qwidget)
+    except ValueError:
+        pass
+
+
+def start_gui() -> NoReturn:
+    """Starts the script and runs GUI. Logging goes to GUI Log widget."""
+    midiscripter.base.shared._raise_current_process_cpu_priority()
+
+    sigint_exit_code = {'Windows': -1073741510, 'Linux': 130, 'Darwin': 2}[platform.system()]
+    signal.signal(signal.SIGINT, lambda *_: app_instance.exit(sigint_exit_code))
+    
+    signal_checker_dummy_timer = QTimer()  # runs python code from Qt to allow the signal to trigger
+    signal_checker_dummy_timer.start(1000)
+    signal_checker_dummy_timer.timeout.connect(lambda: None)  # dummy python code to run
+
+    start_minimized_to_tray = '--tray' in sys.argv
+
+    with midiscripter.base.port_base._all_opened():
+        app_instance.prepare_main_window(start_minimized_to_tray)
+        exit_status = app_instance.exec()
+
+    if exit_status == 1467:  # exit status for restart request
+        midiscripter.base.shared.restart_script()
+    else:
+        exit(exit_status)
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/log_widget.py` & `midiscripter-0.1.2/midiscripter/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.1/midiscripter/gui/main_window.py` & `midiscripter-0.1.2/midiscripter/gui/main_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,123 @@
-import pathlib
-
-from PySide6.QtCore import *
-from PySide6.QtGui import *
-from PySide6.QtWidgets import *
-
-import midiscripter.base.shared
-import midiscripter.gui.menu_bar
-import midiscripter.gui.log_widget
-import midiscripter.gui.ports_widget
-
-
-class TrayIcon(QSystemTrayIcon):
-    def __init__(self, icon, parent: 'MainWindow' = None):
-        super().__init__(icon, parent)
-        self.setToolTip(QApplication.instance().applicationName())
-        self.activated.connect(self.__activated)
-
-        menu = QMenu(parent)
-        menu.setDefaultAction(menu.addAction('Open GUI', parent.showNormal))
-        self.restart_act = menu.addAction('Restart script', QApplication.instance().restart)
-        menu.addAction('Quit', QApplication.instance().exit)
-        self.setContextMenu(menu)
-
-    def __activated(self, reason: QSystemTrayIcon.ActivationReason):
-        if reason == QSystemTrayIcon.ActivationReason.Trigger:
-            if self.parent().isVisible():
-                self.parent().close()
-            else:
-                self.parent().show_from_tray()
-
-        if reason == QSystemTrayIcon.ActivationReason.MiddleClick:
-            self.restart_act.trigger()
-
-
-class MainWindow(QMainWindow):
-    dock_names: set[str] = set()
-    dock_widgets: list[QDockWidget] = []
-
-    def __init__(self, widgets_to_add: list[QWidget]):
-        super().__init__()
-        self.__normal_flags = self.windowFlags()
-        self.__always_on_top_flags = self.__normal_flags | Qt.WindowStaysOnTopHint
-
-        app_name = QApplication.instance().organizationName()
-        script_name = QApplication.instance().applicationName()
-        self.setWindowTitle(f'{app_name} - {script_name}')
-
-        self.setDockNestingEnabled(True)
-
-        self.add_widget_as_dock(midiscripter.gui.ports_widget.PortsWidget())
-        self.add_widget_as_dock(midiscripter.gui.log_widget.LogWidget())
-
-        for widget in widgets_to_add:
-            self.add_widget_as_dock(widget)
-
-        self.menu_bar = midiscripter.gui.menu_bar.MenuBar(self)
-        self.setMenuBar(self.menu_bar)
-
-        self.tray = TrayIcon(self.windowIcon(), self)
-        self.tray.show()
-
-    def add_widget_as_dock(self, widget: QWidget):
-        dock = QDockWidget(self)
-        dock.setObjectName(widget.objectName())
-        dock.setWindowTitle(widget.objectName())
-        dock.setWidget(widget)
-        dock.setStyleSheet('QDockWidget {border: 1px solid black;}')  # TODO Test
-
-        self.addDockWidget(Qt.DockWidgetArea.TopDockWidgetArea, dock)
-        self.dock_widgets.append(dock)
-
-    def set_dock_titles_visibility(self, are_hidden: bool):
-        # Can't make full lock with setFixedSize due to AdaptiveTextSizeWidgets
-        # that has "Ignore" size policy and always restore at maximum size after that       
-        for dock in self.dock_widgets:
-            if are_hidden:
-                dock.setTitleBarWidget(QWidget())
-            else:
-                dock.setTitleBarWidget(None)
-
-    def show_from_tray(self):
-        self.setWindowState(self.windowState() & ~Qt.WindowMinimized | Qt.WindowActive)
-        self.resize(QSettings().value(f'win size', QSize(1024, 768)))
-        self.move(QSettings().value(f'win position', QPoint(200, 200)))
-        self.restoreState(QSettings().value(f'win state'))
-
-        if QSettings().value('restart win minimized', False):
-            self.showMinimized()
-            # 'win minimized' set by restart request, cleared for the next normal start
-            QSettings().setValue('restart win minimized', 0)
-        elif QSettings().value(f'win maximized', False):
-            self.showMaximized()
-        else:
-            self.show()
-
-        # Using always on top flip to focus on window  TODO
-        # if QSettings().value('win active before restart', 0):
-        #     # QSettings().setValue('win active before restart', 0)
-        #     self.set_always_on_top(True)
-        #     if not self.menu_bar.always_on_top:
-        #         self.set_always_on_top(False)
-
-        # 'win visible' set by restart request, cleared for the next normal start
-        if QSettings().value('restart closed to tray', False):
-            QSettings().setValue('restart closed to tray', 0)
-            self.close()
-        
-    def closeEvent(self, event: QCloseEvent):
-        event.ignore()
-        QSettings().setValue(f'win state', self.saveState())
-        QSettings().setValue(f'win maximized', int(self.isMaximized()))
-
-        if not self.isMaximized():
-            QSettings().setValue(f'win size', self.size())
-            QSettings().setValue(f'win position', self.pos())
-
-        self.hide()
-
-    def set_always_on_top(self, state: bool):
-        if state:
-            self.setWindowFlags(self.__always_on_top_flags)
-        else:
-            self.setWindowFlags(self.__normal_flags)
-        self.show()
+from PySide6.QtCore import *
+from PySide6.QtGui import *
+from PySide6.QtWidgets import *
+
+import midiscripter.base.shared
+import midiscripter.gui.menu_bar
+import midiscripter.gui.log_widget
+import midiscripter.gui.ports_widget
+
+
+class TrayIcon(QSystemTrayIcon):
+    def __init__(self, icon, parent: 'MainWindow' = None):
+        super().__init__(icon, parent)
+        self.setToolTip(QApplication.instance().applicationName())
+        self.activated.connect(self.__activated)
+
+        menu = QMenu(parent)
+        menu.setDefaultAction(menu.addAction('Open GUI', parent.showNormal))
+        self.restart_act = menu.addAction('Restart script', QApplication.instance().restart)
+        menu.addAction('Quit', QApplication.instance().exit)
+        self.setContextMenu(menu)
+
+    def __activated(self, reason: QSystemTrayIcon.ActivationReason):
+        if reason == QSystemTrayIcon.ActivationReason.Trigger:
+            if self.parent().isVisible():
+                self.parent().close()
+            else:
+                self.parent().show_from_tray()
+
+        if reason == QSystemTrayIcon.ActivationReason.MiddleClick:
+            self.restart_act.trigger()
+
+
+class MainWindow(QMainWindow):
+    dock_names: set[str] = set()
+    dock_widgets: list[QDockWidget] = []
+
+    def __init__(self, widgets_to_add: list[QWidget]):
+        super().__init__()
+        self.__normal_flags = self.windowFlags()
+        self.__always_on_top_flags = self.__normal_flags | Qt.WindowStaysOnTopHint
+
+        app_name = QApplication.instance().organizationName()
+        script_name = QApplication.instance().applicationName()
+        self.setWindowTitle(f'{app_name} - {script_name}')
+
+        self.setDockNestingEnabled(True)
+
+        self.add_widget_as_dock(midiscripter.gui.ports_widget.PortsWidget())
+        self.add_widget_as_dock(midiscripter.gui.log_widget.LogWidget())
+
+        for widget in widgets_to_add:
+            self.add_widget_as_dock(widget)
+
+        self.menu_bar = midiscripter.gui.menu_bar.MenuBar(self)
+        self.setMenuBar(self.menu_bar)
+
+        self.tray = TrayIcon(self.windowIcon(), self)
+        self.tray.show()
+
+    def add_widget_as_dock(self, widget: QWidget):
+        dock = QDockWidget(self)
+        dock.setObjectName(widget.objectName())
+        dock.setWindowTitle(widget.objectName())
+        dock.setWidget(widget)
+
+        self.addDockWidget(Qt.DockWidgetArea.TopDockWidgetArea, dock)
+        self.dock_widgets.append(dock)
+
+    def set_dock_titles_visibility(self, are_hidden: bool):
+        # Can't make full lock with setFixedSize due to AdaptiveTextSizeWidgets
+        # that has "Ignore" size policy and always restore at maximum size after that       
+        for dock in self.dock_widgets:
+            if are_hidden:
+                dock.setTitleBarWidget(QWidget())
+            else:
+                dock.setTitleBarWidget(None)
+
+    def show_from_tray(self):
+        self.setWindowState(self.windowState() & ~Qt.WindowMinimized | Qt.WindowActive)
+        self.resize(QSettings().value(f'win size', QSize(800, 500)))
+        self.move(QSettings().value(f'win position', self.__get_screen_center()))
+        self.restoreState(QSettings().value(f'win state'))
+
+        if QSettings().value('restart win minimized', False):
+            self.showMinimized()
+            # 'win minimized' set by restart request, cleared for the next normal start
+            QSettings().setValue('restart win minimized', 0)
+        elif QSettings().value(f'win maximized', False):
+            self.showMaximized()
+        else:
+            self.show()
+
+        # Somewhere in window preparation the window size changes, second resize makes it stick.
+        self.resize(QSettings().value(f'win size', QSize(800, 500)))
+        self.move(QSettings().value(f'win position', self.__get_screen_center()))
+
+        # 'win visible' set by restart request, cleared for the next normal start
+        if QSettings().value('restart closed to tray', False):
+            QSettings().setValue('restart closed to tray', 0)
+            self.close()
+        
+    def closeEvent(self, event: QCloseEvent):
+        event.ignore()
+        QSettings().setValue(f'win state', self.saveState())
+        QSettings().setValue(f'win maximized', int(self.isMaximized()))
+
+        if not self.isMaximized():
+            QSettings().setValue(f'win size', self.size())
+            QSettings().setValue(f'win position', self.pos())
+
+        self.hide()
+
+    def set_always_on_top(self, state: bool):
+        if state:
+            self.setWindowFlags(self.__always_on_top_flags)
+        else:
+            self.setWindowFlags(self.__normal_flags)
+        self.show()
+        
+    def __get_screen_center(self) -> QPoint:
+        return (self.screen().geometry().center() - 
+                QRect(QPoint(), self.frameGeometry().size()).center())
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/menu_bar.py` & `midiscripter-0.1.2/midiscripter/gui/menu_bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,177 +1,171 @@
-import pathlib
-import platform
-import sys
-from typing import Callable, TYPE_CHECKING, Optional
-
-import win32com.client
-from PySide6.QtCore import *
-from PySide6.QtGui import *
-from PySide6.QtWidgets import *
-
-import midiscripter.base.shared
-import midiscripter.file_event
-import midiscripter.midi.midi_ports_update
-
-if TYPE_CHECKING:
-    import midiscripter.gui.main_window
-
-
-class SavedCheckedStateAction(QAction):
-    def __init__(self, name: str,
-                 func_for_state: Optional[Callable] = None,
-                 *, checked_func: Optional[Callable] = None,
-                 unchecked_func: Optional[Callable] = None,
-                 default_state: bool = False,
-                 key_shortcut: Optional[QKeySequence] = None):
-        super().__init__(name)
-        self.__func_for_state = func_for_state
-        self.__checked_func = checked_func
-        self.__unchecked_func = unchecked_func
-        self.__default_state = default_state
-        self.__setting_name = f'action {name}'
-
-        if key_shortcut:
-            self.setShortcut(key_shortcut)
-
-        self.setCheckable(True)
-        self.setChecked(default_state)  # replaces force _state_changed that causes widgets toggled by action to pop up
-        self.toggled.connect(self.__state_changed)
-        self.setChecked(QSettings().value(self.__setting_name, int(default_state)))
-
-    def __bool__(self):
-        return bool(QSettings().value(self.__setting_name, int(self.__default_state)))
-
-    def __state_changed(self, state: bool):
-        QSettings().setValue(self.__setting_name, int(state))
-
-        if self.__func_for_state:
-            self.__func_for_state(state)
-
-        if state is True and self.__checked_func:
-            self.__checked_func()
-        if state is False and self.__unchecked_func:
-            self.__unchecked_func()
-
-
-class MenuBar(QMenuBar):
-    autostart_path = pathlib.Path.home() / 'AppData/Roaming/Microsoft/Windows/' \
-                                           'Start Menu/Programs/Startup'
-    autostart_shortcut_prefix = 'MIDI Scripter - '
-
-    def __init__(self, main_window: 'midiscripter.gui.main_window.MainWindow'):
-        super().__init__(main_window)
-        self.setObjectName('Menu Bar')
-
-        # Script
-        script_menu = self.addMenu('Script')
-        script_menu.addAction('Run another', self._run_another_script)
-        script_menu.addAction('&Restart', QApplication.instance().restart, QKeySequence('Ctrl+R'))
-        script_menu.addAction('&Quit', QApplication.instance().exit, QKeySequence('Ctrl+Q'))
-
-        # Options
-        options_menu = self.addMenu('Options')
-
-        if platform.system() == 'Windows':
-            shortcut_name = f'{self.autostart_shortcut_prefix}' \
-                            f'{pathlib.Path(midiscripter.base.shared.script_path).stem}.lnk'
-            self.__autostart_script_path = self.autostart_path / shortcut_name
-            toggle_autostart = options_menu.addAction('Run at start up')
-            toggle_autostart.setCheckable(True)
-            toggle_autostart.setChecked(self.__autostart_script_path.is_file())  # TODO name beginning
-            toggle_autostart.toggled.connect(self.__set_autostart)
-
-        self.always_on_top = SavedCheckedStateAction('Window always on top',
-                                                     main_window.set_always_on_top,
-                                                     key_shortcut=QKeySequence('Ctrl+Space'))
-        options_menu.insertAction(QAction(), self.always_on_top)
-
-        options_menu.addSeparator()
-
-        self.watch_script_file = SavedCheckedStateAction('Restart on script file change',
-                                                         self.__set_watching_script_file)
-        options_menu.insertAction(QAction(), self.watch_script_file)
-
-        self.watch_midi_ports = SavedCheckedStateAction('Restart on MIDI port changes',
-                                                        self.__set_watching_midi_ports)
-        options_menu.insertAction(QAction(), self.watch_midi_ports)
-
-        # script_path_dir_path = str(pathlib.Path(midiscripter.base.script_path).parent) TODO
-        # self.watch_script_dir = SavedCheckedStateAction('Restart on script parent directory change',
-        #                                                 lambda: QApplication.instance().file_event.addPath(script_path_dir_path),
-        #                                                 lambda: QApplication.instance().file_event.removePath(script_path_dir_path))
-        # options_menu.insertAction(QAction(), self.watch_script_dir)
-
-        # Dock widgets
-        widgets_menu = self.addMenu('Widgets')
-
-        self.lock_dock_widgets = SavedCheckedStateAction('Hide widgets titles',
-                                                         main_window.set_dock_titles_visibility,
-                                                         key_shortcut=QKeySequence('Ctrl+T'))
-        widgets_menu.insertAction(QAction(), self.lock_dock_widgets)
-        widgets_menu.addSeparator()
-        widgets_menu.aboutToShow.connect(lambda: widgets_menu.addActions(main_window.createPopupMenu().actions()))
-        
-        # Help
-        script_menu = self.addMenu('Help')
-        script_menu.addAction('Homepage', lambda: QDesktopServices.openUrl(
-            QUrl('https://github.com/Maboroshy/midi-scripter')))
-        script_menu.addAction('Documentation', lambda: QDesktopServices.openUrl(
-            QUrl('https://maboroshy.github.io/midi-scripter')))
-
-    def _run_another_script(self):
-        file_path_str = QFileDialog.getOpenFileName(self, 'Select python script',
-                                                    str(pathlib.Path(midiscripter.base.shared.script_path).parent),
-                                                    'Python script (*.py)')[0]
-        if file_path_str:
-            midiscripter.base.shared.script_path = file_path_str
-            QApplication.instance().restart()
-
-    @Slot(bool)
-    def __set_autostart(self, state: bool) -> None:
-        other_autostart_shortcuts = []
-        for path in self.autostart_path.iterdir():
-            if (path.name.startswith(self.autostart_shortcut_prefix) and path.is_file() 
-                    and path != self.__autostart_script_path.resolve()):
-                other_autostart_shortcuts.append(path)
-                
-        if other_autostart_shortcuts:
-            remove_other_dialog = QMessageBox()
-            remove_other_dialog.setText('There are other scripts with enabled autostart. Disable them?')
-            remove_other_dialog.setStandardButtons(QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel)
-            remove_other_dialog_pressed_button = remove_other_dialog.exec()
-            
-            if remove_other_dialog_pressed_button == QMessageBox.Cancel:
-                return 
-            elif remove_other_dialog_pressed_button == QMessageBox.Yes:
-                for shortcut_path in other_autostart_shortcuts:
-                    shortcut_path.unlink()
-
-        if state:
-            shell = win32com.client.Dispatch("WScript.Shell")
-            shortcut = shell.CreateShortCut(str(self.__autostart_script_path.resolve()))
-            shortcut.Targetpath = str(pathlib.Path(sys.executable).parent / 'pythonw.exe')
-            shortcut.WorkingDirectory = str(pathlib.Path(midiscripter.base.shared.script_path).parent.resolve())
-            shortcut.Arguments = '"{}" "--tray"'.format(pathlib.Path(midiscripter.base.shared.script_path).resolve())
-            shortcut.save()
-        else:
-            self.__autostart_script_path.resolve().unlink(True)
-        
-    def __set_watching_script_file(self, new_status: bool):
-        if new_status:
-            self.file_watcher_port = midiscripter.file_event.FileEventIn(midiscripter.base.shared.script_path)
-            self.file_watcher_port.subscribe(QApplication.instance().restart_at_file_change)
-            self.file_watcher_port._open()
-        else:
-            self.file_watcher_port.is_enabled = False
-
-    def __set_watching_midi_ports(self, new_status: bool):
-        if new_status:
-            self.midi_port_watcher_port = midiscripter.midi.midi_ports_update.MidiPortsChangedIn()
-
-            @self.midi_port_watcher_port.subscribe
-            def restart_on_midi_port_change(_):
-                QApplication.instance().request_restart.emit()
-
-            self.midi_port_watcher_port._open()
-        else:
-            self.midi_port_watcher_port.is_enabled = False
+import pathlib
+import platform
+import sys
+from typing import Callable, TYPE_CHECKING, Optional
+
+import win32com.client
+from PySide6.QtCore import *
+from PySide6.QtGui import *
+from PySide6.QtWidgets import *
+
+import midiscripter.base.shared
+import midiscripter.file_event
+import midiscripter.midi.midi_ports_update
+
+if TYPE_CHECKING:
+    import midiscripter.gui.main_window
+
+
+class SavedCheckedStateAction(QAction):
+    def __init__(self, name: str,
+                 func_for_state: Optional[Callable] = None,
+                 *, checked_func: Optional[Callable] = None,
+                 unchecked_func: Optional[Callable] = None,
+                 default_state: bool = False,
+                 key_shortcut: Optional[QKeySequence] = None):
+        super().__init__(name)
+        self.__func_for_state = func_for_state
+        self.__checked_func = checked_func
+        self.__unchecked_func = unchecked_func
+        self.__default_state = default_state
+        self.__setting_name = f'action {name}'
+
+        if key_shortcut:
+            self.setShortcut(key_shortcut)
+
+        self.setCheckable(True)
+        self.setChecked(default_state)  # replaces force _state_changed that causes widgets toggled by action to pop up
+        self.toggled.connect(self.__state_changed)
+        self.setChecked(QSettings().value(self.__setting_name, int(default_state)))
+
+    def __bool__(self):
+        return bool(QSettings().value(self.__setting_name, int(self.__default_state)))
+
+    def __state_changed(self, state: bool):
+        QSettings().setValue(self.__setting_name, int(state))
+
+        if self.__func_for_state:
+            self.__func_for_state(state)
+
+        if state is True and self.__checked_func:
+            self.__checked_func()
+        if state is False and self.__unchecked_func:
+            self.__unchecked_func()
+
+
+class MenuBar(QMenuBar):
+    autostart_path = pathlib.Path.home() / 'AppData/Roaming/Microsoft/Windows/' \
+                                           'Start Menu/Programs/Startup'
+    autostart_shortcut_prefix = 'MIDI Scripter - '
+
+    def __init__(self, main_window: 'midiscripter.gui.main_window.MainWindow'):
+        super().__init__(main_window)
+        self.setObjectName('Menu Bar')
+
+        # Script
+        script_menu = self.addMenu('Script')
+        script_menu.addAction('Run another', self._run_another_script)
+        script_menu.addAction('&Restart', QApplication.instance().restart, QKeySequence('Ctrl+R'))
+        script_menu.addAction('&Quit', QApplication.instance().exit, QKeySequence('Ctrl+Q'))
+
+        # Options
+        options_menu = self.addMenu('Options')
+
+        if platform.system() == 'Windows':
+            shortcut_name = f'{self.autostart_shortcut_prefix}' \
+                            f'{pathlib.Path(midiscripter.base.shared.script_path).stem}.lnk'
+            self.__autostart_script_path = self.autostart_path / shortcut_name
+            toggle_autostart = options_menu.addAction('Run at start up')
+            toggle_autostart.setCheckable(True)
+            toggle_autostart.setChecked(self.__autostart_script_path.is_file())
+            toggle_autostart.toggled.connect(self.__set_autostart)
+
+        self.always_on_top = SavedCheckedStateAction('Window always on top',
+                                                     main_window.set_always_on_top,
+                                                     key_shortcut=QKeySequence('Ctrl+Space'))
+        options_menu.insertAction(QAction(), self.always_on_top)
+
+        options_menu.addSeparator()
+
+        self.watch_script_file = SavedCheckedStateAction('Restart on script file change',
+                                                         self.__set_watching_script_file)
+        options_menu.insertAction(QAction(), self.watch_script_file)
+
+        self.watch_midi_ports = SavedCheckedStateAction('Restart on MIDI port changes',
+                                                        self.__set_watching_midi_ports)
+        options_menu.insertAction(QAction(), self.watch_midi_ports)
+
+        # Dock widgets
+        widgets_menu = self.addMenu('Widgets')
+
+        self.lock_dock_widgets = SavedCheckedStateAction('Hide widgets titles',
+                                                         main_window.set_dock_titles_visibility,
+                                                         key_shortcut=QKeySequence('Ctrl+T'))
+        widgets_menu.insertAction(QAction(), self.lock_dock_widgets)
+        widgets_menu.addSeparator()
+        widgets_menu.aboutToShow.connect(lambda: widgets_menu.addActions(main_window.createPopupMenu().actions()))
+        
+        # Help
+        script_menu = self.addMenu('Help')
+        script_menu.addAction('Homepage', lambda: QDesktopServices.openUrl(
+            QUrl('https://github.com/Maboroshy/midi-scripter')))
+        script_menu.addAction('Documentation', lambda: QDesktopServices.openUrl(
+            QUrl('https://maboroshy.github.io/midi-scripter')))
+
+    def _run_another_script(self):
+        file_path_str = QFileDialog.getOpenFileName(self, 'Select python script',
+                                                    str(pathlib.Path(midiscripter.base.shared.script_path).parent),
+                                                    'Python script (*.py)')[0]
+        if file_path_str:
+            midiscripter.base.shared.script_path = file_path_str
+            QApplication.instance().restart()
+
+    @Slot(bool)
+    def __set_autostart(self, state: bool) -> None:
+        other_autostart_shortcuts = []
+        for path in self.autostart_path.iterdir():
+            if (path.name.startswith(self.autostart_shortcut_prefix) and path.is_file() 
+                    and path != self.__autostart_script_path.resolve()):
+                other_autostart_shortcuts.append(path)
+                
+        if other_autostart_shortcuts:
+            remove_other_dialog = QMessageBox()
+            remove_other_dialog.setText('There are other scripts with enabled autostart. Disable them?')
+            remove_other_dialog.setStandardButtons(QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel)
+            remove_other_dialog_pressed_button = remove_other_dialog.exec()
+            
+            if remove_other_dialog_pressed_button == QMessageBox.Cancel:
+                return 
+            elif remove_other_dialog_pressed_button == QMessageBox.Yes:
+                for shortcut_path in other_autostart_shortcuts:
+                    shortcut_path.unlink()
+
+        if state:
+            shell = win32com.client.Dispatch("WScript.Shell")
+            shortcut = shell.CreateShortCut(str(self.__autostart_script_path.resolve()))
+            shortcut.Targetpath = str(pathlib.Path(sys.executable).parent / 'pythonw.exe')
+            shortcut.WorkingDirectory = str(pathlib.Path(midiscripter.base.shared.script_path).parent.resolve())
+            shortcut.Arguments = '"{}" "--tray"'.format(pathlib.Path(midiscripter.base.shared.script_path).resolve())
+            shortcut.save()
+        else:
+            self.__autostart_script_path.resolve().unlink(True)
+        
+    def __set_watching_script_file(self, new_status: bool):
+        if new_status:
+            self.file_watcher_port = midiscripter.file_event.FileEventIn(midiscripter.base.shared.script_path)
+            self.file_watcher_port.subscribe(QApplication.instance().restart_at_file_change)
+            self.file_watcher_port._open()
+        else:
+            self.file_watcher_port.is_enabled = False
+
+    def __set_watching_midi_ports(self, new_status: bool):
+        if new_status:
+            self.midi_port_watcher_port = midiscripter.midi.midi_ports_update.MidiPortsChangedIn()
+
+            @self.midi_port_watcher_port.subscribe
+            def restart_on_midi_port_change(_):
+                QApplication.instance().request_restart.emit()
+
+            self.midi_port_watcher_port._open()
+        else:
+            self.midi_port_watcher_port.is_enabled = False
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/ports_widget.py` & `midiscripter-0.1.2/midiscripter/gui/ports_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-from typing import Callable
-
-from PySide6.QtGui import *
-from PySide6.QtCore import *
-from PySide6.QtWidgets import *
-
-import midiscripter.midi
-import midiscripter.logger.html_sink
-from midiscripter.logger import log  
-from midiscripter.base.port_base import Input, Output
-
-
-class PortsWidget(QTreeWidget):
-    PORT_CLASS_ROLE = 100
-    PORT_UID_ROLE = 101
-    PORT_REPR_ROLE = 103
-    CALLBACK_FUNCTION_ROLE = 104
-    PASSTHROUGH_OUT_PORT_ROLE = 105
-
-    def __init__(self):
-        super().__init__()
-        self.setObjectName('Ports')
-        self.setHeaderHidden(True)
-        self.setMinimumWidth(200)
-        self.setMinimumHeight(200)
-        self.setMouseTracking(True)
-        self.itemEntered.connect(self.__update_item_tooltip)
-        self.__populate()
-    
-    def __add_top_level_item(self, item_text: str):
-        bold_font = self.font()
-        bold_font.setBold(True)
-
-        top_item = QTreeWidgetItem(self, (item_text,))
-        top_item.setData(0, Qt.ItemDataRole.FontRole, bold_font)
-        top_item.setExpanded(True)
-        
-        return top_item
-        
-    def __populate(self):
-        """ Populates the widget with items """
-        self.clear()
-        self.__add_midi_inputs()
-        self.__add_midi_outputs()
-        self.__add_ports_if_declared('OSC Inputs', midiscripter.OscIn)
-        self.__add_ports_if_declared('OSC Outputs', midiscripter.OscOut)
-        self.__add_keyboard_in()
-        self.__add_ports_if_declared('Keyboard Output', midiscripter.KeyOut)
-        self.__add_ports_if_declared('Metronome', midiscripter.MetronomeIn)
-        self.__add_ports_if_declared('File Event Watcher', midiscripter.FileEventIn)
-        self.__add_ports_if_declared('MIDI Port Changes Watcher', midiscripter.MidiPortsChangedIn)
-        
-        self.itemChanged.connect(self.__item_state_changed)
-        self.itemSelectionChanged.connect(self.__item_selected)
-    
-    def __add_midi_inputs(self):
-        inputs_top = self.__add_top_level_item('MIDI Inputs')
-
-        for input_port_name in midiscripter.midi.MidiIn._available_names:
-            port_key = (midiscripter.midi.MidiIn.__name__, input_port_name)
-            port_instance = midiscripter.midi.MidiIn.instance_registry.get(port_key, None)
-            input_item = QTreeWidgetItem(inputs_top, (input_port_name,))
-
-            if not port_instance:
-                input_item.setCheckState(0, Qt.CheckState.Unchecked)
-            elif port_instance.is_enabled:
-                input_item.setCheckState(0, Qt.CheckState.Checked)
-            else:
-                input_item.setCheckState(0, Qt.CheckState.Unchecked)
-                input_item.setData(0, Qt.ItemDataRole.BackgroundRole,
-                                   QBrush(QColor().fromRgb(255, 0, 0, 20)))
-
-            input_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
-            input_item.setData(0, self.PORT_UID_ROLE, input_port_name)
-            
-            port_repr = f"{midiscripter.midi.MidiIn.__name__}('{input_port_name}')"
-            input_item.setData(0, self.PORT_REPR_ROLE, port_repr)
-            
-            input_item.setData(0, Qt.ItemDataRole.ForegroundRole,
-                               QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]))
-
-            if port_instance:
-
-                for passthrough_out_port in port_instance.attached_passthrough_outs:
-                    sub_item = QTreeWidgetItem(input_item, (passthrough_out_port._uid,))
-                    sub_item.setCheckState(0, Qt.CheckState.Checked)
-
-                    sub_item.setData(0, Qt.ItemDataRole.ForegroundRole,
-                                     QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]))
-                    sub_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
-                    sub_item.setData(0, self.PORT_UID_ROLE, input_port_name)
-                    sub_item.setData(0, self.PASSTHROUGH_OUT_PORT_ROLE, passthrough_out_port)
-                    sub_item.setData(0, self.PORT_REPR_ROLE, passthrough_out_port.__repr__())
-
-                self.__add_inputs_subscribed_calls(input_item)
-
-        for port_instance in midiscripter.midi.MidiIn.instance_registry.values():
-            if isinstance(port_instance, midiscripter.midi.MidiIn) and not port_instance._is_available:
-                absent_input_item = QTreeWidgetItem(inputs_top, (str(port_instance),))
-                absent_input_item.setCheckState(0, Qt.CheckState.Unchecked)
-                absent_input_item.setDisabled(True)
-    
-    def __add_inputs_subscribed_calls(self, input_item: QTreeWidgetItem):
-        port_class = input_item.data(0, self.PORT_CLASS_ROLE)
-        port_name = input_item.data(0, self.PORT_UID_ROLE)
-
-        if port_name:
-            port_instance = port_class(port_name)
-        else:
-            port_instance = port_class()
-        
-        for callback_function in port_instance.subscribed_calls:
-            sub_item = QTreeWidgetItem(input_item, (callback_function.__name__,))
-            sub_item.setCheckState(0, Qt.CheckState.Checked)
-
-            sub_item.setData(0, Qt.ItemDataRole.ForegroundRole,
-                             QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Callable]))
-            sub_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
-            sub_item.setData(0, self.PORT_UID_ROLE, port_name)
-            sub_item.setData(0, self.CALLBACK_FUNCTION_ROLE, callback_function)
-    
-    def __add_midi_outputs(self):
-        outputs_top = self.__add_top_level_item('MIDI Outputs')
-
-        for output_port_name in midiscripter.midi.MidiOut._available_names:
-            port_key = (midiscripter.midi.MidiOut.__name__, output_port_name)
-            port_instance = midiscripter.midi.MidiOut.instance_registry.get(port_key, None)
-            output_item = QTreeWidgetItem(outputs_top, (output_port_name,))
-
-            if not port_instance:
-                output_item.setCheckState(0, Qt.CheckState.Unchecked)
-            elif port_instance.is_enabled:
-                output_item.setCheckState(0, Qt.CheckState.Checked)
-            else:
-                output_item.setCheckState(0, Qt.CheckState.Unchecked)
-                output_item.setData(0, Qt.ItemDataRole.BackgroundRole,
-                                    QBrush(QColor().fromRgb(255, 0, 0, 20)))
-
-            output_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
-            output_item.setData(0, self.PORT_UID_ROLE, output_port_name)
-            
-            port_repr = f"{midiscripter.midi.MidiOut.__name__}('{output_port_name}')"
-            output_item.setData(0, self.PORT_REPR_ROLE, port_repr)
-            
-            output_item.setData(0, Qt.ItemDataRole.ForegroundRole,
-                                QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]))
-
-        for port_instance in midiscripter.midi.MidiOut.instance_registry.values():
-            if isinstance(port_instance, midiscripter.midi.MidiOut) and not port_instance._is_available:
-                absent_output_item = QTreeWidgetItem(outputs_top, (port_instance._uid,))
-                absent_output_item.setCheckState(0, Qt.CheckState.Unchecked)
-                absent_output_item.setDisabled(True)
-    
-    def __add_ports_if_declared(self, title: str, port_type: type):
-            port_instances_to_add = []
-            for port_key, port_instance in port_type.instance_registry.items():
-                if port_key[0] is port_type.__name__:
-                    port_instances_to_add.append(port_instance)
-        
-            if not port_instances_to_add:
-                return 
-            
-            port_top = self.__add_top_level_item(title)
-            
-            for port in port_instances_to_add:
-                port_item = QTreeWidgetItem(port_top, (str(port._uid),))
-                port_item.setCheckState(0, Qt.CheckState.Checked)
-
-                port_item.setData(0, self.PORT_CLASS_ROLE, port_type)
-                port_item.setData(0, self.PORT_REPR_ROLE, port.__repr__())
-                
-                if port._force_uid:
-                    port_item.setData(0, self.PORT_UID_ROLE, None)
-                else:
-                    port_item.setData(0, self.PORT_UID_ROLE, port._uid)
-                
-                if issubclass(port_type, Input):
-                    item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]
-                    self.__add_inputs_subscribed_calls(port_item)
-                elif issubclass(port_type, Output):
-                    item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]
-
-                port_item.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
-    
-    def __add_keyboard_in(self):
-        port_top = self.__add_top_level_item('Keyboard Input')
-        port_item = QTreeWidgetItem(port_top, ('Keyboard Input',))
-        if (midiscripter.KeyIn.__name__, midiscripter.KeyIn._force_uid) in midiscripter.KeyIn.instance_registry:
-            port_item.setCheckState(0, Qt.CheckState.Checked)        
-        else:
-            port_item.setCheckState(0, Qt.CheckState.Unchecked)
-            
-        port_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.KeyIn)
-        port_item.setData(0, self.PORT_UID_ROLE, None)
-        port_item.setData(0, self.PORT_REPR_ROLE, f'{midiscripter.KeyIn.__name__}()')
-        port_item.setData(0, Qt.ItemDataRole.ForegroundRole, 
-                          QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]))
-    
-    def __item_selected(self):
-        """ Sends selected item text to the clipboard and shows a "copied" tooltip """
-        if not self.selectedItems():
-            return
-
-        selected_item: QTreeWidgetItem = self.selectedItems()[0]
-        port_repr = selected_item.data(0, self.PORT_REPR_ROLE)
-        if port_repr:
-            QGuiApplication.clipboard().setText(port_repr)
-            QTimer.singleShot(200, lambda: QToolTip().showText(self.cursor().pos(),
-                                                               f'Copied {port_repr}',
-                                                               self, msecShowTime=2000))  # Don't hide on mouse button release
-        selected_item.setSelected(False)
-
-    def __item_state_changed(self, item: QTreeWidgetItem, _):
-        """ Enabled or disables the MIDI port / passthrough out / call according to the checked state change """
-        new_checked_state = item.checkState(0) == Qt.CheckState.Checked
-
-        port_class = item.data(0, self.PORT_CLASS_ROLE)
-        port_name = item.data(0, self.PORT_UID_ROLE)
-
-        callback_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
-        passthrough_out_port: midiscripter.midi.MidiOut = item.data(0, self.PASSTHROUGH_OUT_PORT_ROLE)
-        
-        if port_name:
-            port_instance = port_class(port_name)
-        else:
-            port_instance = port_class()
-
-        if callback_function:
-            if new_checked_state:
-                port_instance.subscribed_calls.append(callback_function)
-            else:
-                port_instance.subscribed_calls.remove(callback_function)
-
-        elif passthrough_out_port:
-            if new_checked_state:
-                port_instance.attached_passthrough_outs.append(passthrough_out_port)
-            else:
-                port_instance.attached_passthrough_outs.remove(passthrough_out_port)
-
-        else:
-            if new_checked_state:
-                if not port_instance.is_enabled:
-                    port_instance._open()
-                    port_instance.is_enabled = True
-                    log('Enabled {port}', port=port_instance)
-
-                if not port_instance.is_enabled:
-                    item.setData(0, Qt.ItemDataRole.BackgroundRole,
-                                 QBrush(QColor().fromRgb(255, 0, 0, 20)))
-                    log.red('Can\'t enable {port}', port=port_instance)
-                else:
-                    item.setData(0, Qt.ItemDataRole.BackgroundRole,
-                                 QBrush(QColor(Qt.GlobalColor.transparent)))
-
-            else:
-                port_instance.is_enabled = False
-                log('Disabled {port}', port=port_instance)
-
-            self.blockSignals(True)
-            item.setCheckState(0, (Qt.CheckState.Unchecked,
-                                   Qt.CheckState.Checked)[port_instance.is_enabled])
-            self.blockSignals(False)
-
-    def __update_item_tooltip(self, item: QTreeWidgetItem):
-        """ Updates items tooltip on hover """
-        call_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
-        if call_function:
-            port_class = item.data(0, self.PORT_CLASS_ROLE)
-            call_statistics = list(port_class._call_statistics[call_function])
-
-            if not call_statistics:
-                tooltip_text = 'No calls made yet'
-            else:
-                call_statistics.sort()
-                tooltip_text = ('Execution time for last 20 calls:\n'
-                                f'Min: {call_statistics[0]} ms; '
-                                f'Med: {call_statistics[int(len(call_statistics) / 2)]} ms; '
-                                f'Max: {call_statistics[-1]} ms')
-                
-            item.setData(0, Qt.ItemDataRole.ToolTipRole, tooltip_text)
+from typing import Callable
+
+from PySide6.QtGui import *
+from PySide6.QtCore import *
+from PySide6.QtWidgets import *
+
+import midiscripter.midi
+import midiscripter.logger.html_sink
+from midiscripter.logger import log  
+from midiscripter.base.port_base import Input, Output
+
+
+class PortsWidget(QTreeWidget):
+    PORT_CLASS_ROLE = 100
+    PORT_UID_ROLE = 101
+    PORT_REPR_ROLE = 103
+    CALLBACK_FUNCTION_ROLE = 104
+    PASSTHROUGH_OUT_PORT_ROLE = 105
+
+    def __init__(self):
+        super().__init__()
+        self.setObjectName('Ports')
+        self.setHeaderHidden(True)
+        self.setMinimumWidth(200)
+        self.setMinimumHeight(200)
+        self.setMouseTracking(True)
+        self.itemEntered.connect(self.__update_item_tooltip)
+        self.__populate()
+    
+    def __add_top_level_item(self, item_text: str):
+        bold_font = self.font()
+        bold_font.setBold(True)
+
+        top_item = QTreeWidgetItem(self, (item_text,))
+        top_item.setData(0, Qt.ItemDataRole.FontRole, bold_font)
+        top_item.setExpanded(True)
+        
+        return top_item
+        
+    def __populate(self):
+        """ Populates the widget with items """
+        self.clear()
+        self.__add_midi_inputs()
+        self.__add_midi_outputs()
+        self.__add_ports_if_declared('OSC Inputs', midiscripter.OscIn)
+        self.__add_ports_if_declared('OSC Outputs', midiscripter.OscOut)
+        self.__add_keyboard_in()
+        self.__add_ports_if_declared('Keyboard Output', midiscripter.KeyOut)
+        self.__add_ports_if_declared('Metronome', midiscripter.MetronomeIn)
+        self.__add_ports_if_declared('File Event Watcher', midiscripter.FileEventIn)
+        self.__add_ports_if_declared('MIDI Port Changes Watcher', midiscripter.MidiPortsChangedIn)
+        
+        self.itemChanged.connect(self.__item_state_changed)
+        self.itemSelectionChanged.connect(self.__item_selected)
+    
+    def __add_midi_inputs(self):
+        inputs_top = self.__add_top_level_item('MIDI Inputs')
+
+        for input_port_name in midiscripter.midi.MidiIn._available_names:
+            port_key = (midiscripter.midi.MidiIn.__name__, input_port_name)
+            port_instance = midiscripter.midi.MidiIn.instance_registry.get(port_key, None)
+            input_item = QTreeWidgetItem(inputs_top, (input_port_name,))
+
+            if not port_instance:
+                input_item.setCheckState(0, Qt.CheckState.Unchecked)
+            elif port_instance.is_enabled:
+                input_item.setCheckState(0, Qt.CheckState.Checked)
+            else:
+                input_item.setCheckState(0, Qt.CheckState.Unchecked)
+                input_item.setData(0, Qt.ItemDataRole.BackgroundRole,
+                                   QBrush(QColor().fromRgb(255, 0, 0, 20)))
+
+            input_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
+            input_item.setData(0, self.PORT_UID_ROLE, input_port_name)
+            
+            port_repr = f"{midiscripter.midi.MidiIn.__name__}('{input_port_name}')"
+            input_item.setData(0, self.PORT_REPR_ROLE, port_repr)
+            
+            input_item.setData(0, Qt.ItemDataRole.ForegroundRole,
+                               QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]))
+
+            if port_instance:
+
+                for passthrough_out_port in port_instance.attached_passthrough_outs:
+                    sub_item = QTreeWidgetItem(input_item, (passthrough_out_port._uid,))
+                    sub_item.setCheckState(0, Qt.CheckState.Checked)
+
+                    sub_item.setData(0, Qt.ItemDataRole.ForegroundRole,
+                                     QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]))
+                    sub_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
+                    sub_item.setData(0, self.PORT_UID_ROLE, input_port_name)
+                    sub_item.setData(0, self.PASSTHROUGH_OUT_PORT_ROLE, passthrough_out_port)
+                    sub_item.setData(0, self.PORT_REPR_ROLE, passthrough_out_port.__repr__())
+
+                self.__add_inputs_subscribed_calls(input_item)
+
+        for port_instance in midiscripter.midi.MidiIn.instance_registry.values():
+            if isinstance(port_instance, midiscripter.midi.MidiIn) and not port_instance._is_available:
+                absent_input_item = QTreeWidgetItem(inputs_top, (str(port_instance),))
+                absent_input_item.setCheckState(0, Qt.CheckState.Unchecked)
+                absent_input_item.setDisabled(True)
+    
+    def __add_inputs_subscribed_calls(self, input_item: QTreeWidgetItem):
+        port_class = input_item.data(0, self.PORT_CLASS_ROLE)
+        port_name = input_item.data(0, self.PORT_UID_ROLE)
+
+        if port_name:
+            port_instance = port_class(port_name)
+        else:
+            port_instance = port_class()
+        
+        for callback_function in port_instance.subscribed_calls:
+            sub_item = QTreeWidgetItem(input_item, (callback_function.__name__,))
+            sub_item.setCheckState(0, Qt.CheckState.Checked)
+
+            sub_item.setData(0, Qt.ItemDataRole.ForegroundRole,
+                             QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Callable]))
+            sub_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiIn)
+            sub_item.setData(0, self.PORT_UID_ROLE, port_name)
+            sub_item.setData(0, self.CALLBACK_FUNCTION_ROLE, callback_function)
+    
+    def __add_midi_outputs(self):
+        outputs_top = self.__add_top_level_item('MIDI Outputs')
+
+        for output_port_name in midiscripter.midi.MidiOut._available_names:
+            port_key = (midiscripter.midi.MidiOut.__name__, output_port_name)
+            port_instance = midiscripter.midi.MidiOut.instance_registry.get(port_key, None)
+            output_item = QTreeWidgetItem(outputs_top, (output_port_name,))
+
+            if not port_instance:
+                output_item.setCheckState(0, Qt.CheckState.Unchecked)
+            elif port_instance.is_enabled:
+                output_item.setCheckState(0, Qt.CheckState.Checked)
+            else:
+                output_item.setCheckState(0, Qt.CheckState.Unchecked)
+                output_item.setData(0, Qt.ItemDataRole.BackgroundRole,
+                                    QBrush(QColor().fromRgb(255, 0, 0, 20)))
+
+            output_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.midi.MidiOut)
+            output_item.setData(0, self.PORT_UID_ROLE, output_port_name)
+            
+            port_repr = f"{midiscripter.midi.MidiOut.__name__}('{output_port_name}')"
+            output_item.setData(0, self.PORT_REPR_ROLE, port_repr)
+            
+            output_item.setData(0, Qt.ItemDataRole.ForegroundRole,
+                                QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]))
+
+        for port_instance in midiscripter.midi.MidiOut.instance_registry.values():
+            if isinstance(port_instance, midiscripter.midi.MidiOut) and not port_instance._is_available:
+                absent_output_item = QTreeWidgetItem(outputs_top, (port_instance._uid,))
+                absent_output_item.setCheckState(0, Qt.CheckState.Unchecked)
+                absent_output_item.setDisabled(True)
+    
+    def __add_ports_if_declared(self, title: str, port_type: type):
+            port_instances_to_add = []
+            for port_key, port_instance in port_type.instance_registry.items():
+                if port_key[0] is port_type.__name__:
+                    port_instances_to_add.append(port_instance)
+        
+            if not port_instances_to_add:
+                return 
+            
+            port_top = self.__add_top_level_item(title)
+            
+            for port in port_instances_to_add:
+                port_item = QTreeWidgetItem(port_top, (str(port._uid),))
+                port_item.setCheckState(0, Qt.CheckState.Checked)
+
+                port_item.setData(0, self.PORT_CLASS_ROLE, port_type)
+                port_item.setData(0, self.PORT_REPR_ROLE, port.__repr__())
+                
+                if port._force_uid:
+                    port_item.setData(0, self.PORT_UID_ROLE, None)
+                else:
+                    port_item.setData(0, self.PORT_UID_ROLE, port._uid)
+                
+                if issubclass(port_type, Input):
+                    item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]
+                    self.__add_inputs_subscribed_calls(port_item)
+                elif issubclass(port_type, Output):
+                    item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]
+
+                port_item.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
+    
+    def __add_keyboard_in(self):
+        port_top = self.__add_top_level_item('Keyboard Input')
+        port_item = QTreeWidgetItem(port_top, ('Keyboard Input',))
+        if (midiscripter.KeyIn.__name__, midiscripter.KeyIn._force_uid) in midiscripter.KeyIn.instance_registry:
+            port_item.setCheckState(0, Qt.CheckState.Checked)        
+        else:
+            port_item.setCheckState(0, Qt.CheckState.Unchecked)
+            
+        port_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.KeyIn)
+        port_item.setData(0, self.PORT_UID_ROLE, None)
+        port_item.setData(0, self.PORT_REPR_ROLE, f'{midiscripter.KeyIn.__name__}()')
+        port_item.setData(0, Qt.ItemDataRole.ForegroundRole, 
+                          QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]))
+    
+    def __item_selected(self):
+        """ Sends selected item text to the clipboard and shows a "copied" tooltip """
+        if not self.selectedItems():
+            return
+
+        selected_item: QTreeWidgetItem = self.selectedItems()[0]
+        port_repr = selected_item.data(0, self.PORT_REPR_ROLE)
+        if port_repr:
+            QGuiApplication.clipboard().setText(port_repr)
+            QTimer.singleShot(200, lambda: QToolTip().showText(self.cursor().pos(),
+                                                               f'Copied {port_repr}',
+                                                               self, msecShowTime=2000))  # Don't hide on mouse button release
+        selected_item.setSelected(False)
+
+    def __item_state_changed(self, item: QTreeWidgetItem, _):
+        """ Enabled or disables the MIDI port / passthrough out / call according to the checked state change """
+        new_checked_state = item.checkState(0) == Qt.CheckState.Checked
+
+        port_class = item.data(0, self.PORT_CLASS_ROLE)
+        port_name = item.data(0, self.PORT_UID_ROLE)
+
+        callback_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
+        passthrough_out_port: midiscripter.midi.MidiOut = item.data(0, self.PASSTHROUGH_OUT_PORT_ROLE)
+        
+        if port_name:
+            port_instance = port_class(port_name)
+        else:
+            port_instance = port_class()
+
+        if callback_function:
+            if new_checked_state:
+                port_instance.subscribed_calls.append(callback_function)
+            else:
+                port_instance.subscribed_calls.remove(callback_function)
+
+        elif passthrough_out_port:
+            if new_checked_state:
+                port_instance.attached_passthrough_outs.append(passthrough_out_port)
+            else:
+                port_instance.attached_passthrough_outs.remove(passthrough_out_port)
+
+        else:
+            if new_checked_state:
+                if not port_instance.is_enabled:
+                    port_instance._open()
+                    port_instance.is_enabled = True
+                    log('Enabled {port}', port=port_instance)
+
+                if not port_instance.is_enabled:
+                    item.setData(0, Qt.ItemDataRole.BackgroundRole,
+                                 QBrush(QColor().fromRgb(255, 0, 0, 20)))
+                    log.red('Can\'t enable {port}', port=port_instance)
+                else:
+                    item.setData(0, Qt.ItemDataRole.BackgroundRole,
+                                 QBrush(QColor(Qt.GlobalColor.transparent)))
+
+            else:
+                port_instance.is_enabled = False
+                log('Disabled {port}', port=port_instance)
+
+            self.blockSignals(True)
+            item.setCheckState(0, (Qt.CheckState.Unchecked,
+                                   Qt.CheckState.Checked)[port_instance.is_enabled])
+            self.blockSignals(False)
+
+    def __update_item_tooltip(self, item: QTreeWidgetItem):
+        """ Updates items tooltip on hover """
+        call_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
+        if call_function:
+            port_class = item.data(0, self.PORT_CLASS_ROLE)
+            call_statistics = list(port_class._call_statistics[call_function])
+
+            if not call_statistics:
+                tooltip_text = 'No calls made yet'
+            else:
+                call_statistics.sort()
+                tooltip_text = ('Execution time for last 20 calls:\n'
+                                f'Min: {call_statistics[0]} ms; '
+                                f'Med: {call_statistics[int(len(call_statistics) / 2)]} ms; '
+                                f'Max: {call_statistics[-1]} ms')
+                
+            item.setData(0, Qt.ItemDataRole.ToolTipRole, tooltip_text)
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/gui_widgets/button.py` & `midiscripter-0.1.2/midiscripter/gui/gui_widgets/button.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from typing import Optional, Union, Sequence
-
-from PySide6.QtWidgets import *
-
-from .gui_widget_base import GuiWidget
-from .mixins import AdaptiveTextSizeMixin, WrappedQWidgetMixin
-
-
-class AdaptablePushButtonWidget(AdaptiveTextSizeMixin, WrappedQWidgetMixin, QPushButton):
-    def __init__(self):
-        QPushButton.__init__(self)
-        WrappedQWidgetMixin.__init__(self)
-        AdaptiveTextSizeMixin.__init__(self)
-
-        self.get_content = self.text
-        self.set_content = self.setText
-
-
-class ButtonWidget(AdaptablePushButtonWidget):
-    def __init__(self):
-        super().__init__()
-        self.clicked.connect(self.triggered_signal)
-
-
-class GuiButton(GuiWidget):
-    """Simple button widget."""
-
-    _qt_widget_class = ButtonWidget
-
-    def __init__(self,
-                 content: str,
-                 title: Optional[str] = None,
-                 color: Optional[Union[str, tuple[int, int, int]]] = None):
-        """
-        Args:
-            content: Button text
-            title: Widget's title, `None` for same as content
-            color: Button text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-        """
-        super().__init__(content, title, color)
-
-
-class ToggleButtonWidget(AdaptablePushButtonWidget):
-    def __init__(self):
-        super().__init__()
-        self.setCheckable(True)
-        self.toggled.connect(self.toggle_state_changed_signal)
-
-        self.get_toggle_state = self.isChecked
-        self.set_toggle_state = self.setChecked
-
-
-class GuiToggleButton(GuiWidget):
-    """Toggleable button."""
-
-    _qt_widget_class = ToggleButtonWidget
-
-    def __init__(self,
-                 content: str,
-                 title: Optional[str] = None,
-                 color: Optional[Union[str, tuple[int, int, int]]] = None,
-                 *,
-                 toggle_state: Optional[bool] = None):
-        """
-        Args:
-            content: Button text
-            title: Widget's title, `None` for same as content
-            color: Button text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-            toggle_state: Button toggle state
-        """
-        super().__init__(content, title, color, toggle_state=toggle_state)
-
-
-class ButtonGroupWidgetHorizontal(WrappedQWidgetMixin, QWidget):
-    layout_class = QHBoxLayout
-
-    def __init__(self):
-        QWidget.__init__(self)
-        WrappedQWidgetMixin.__init__(self)
-        self.qt_button_group = QButtonGroup()
-        self.wrapped_qt_buttons_map = {}
-        self.__content = None
-
-    def get_content(self):
-        return self.__content
-
-    def set_content(self, button_labels: list[str]):
-        self.__content = button_labels
-
-        self.qt_button_group.deleteLater()
-        self.qt_button_group = QButtonGroup()
-        self.wrapped_qt_buttons_map: dict[Union[str, int], AdaptablePushButtonWidget] = {}
-
-        layout = self.layout_class()
-        layout.setContentsMargins(0, 0, 0, 0)
-        self.setLayout(layout)
-
-        for index, text in enumerate(button_labels):
-            qt_button = AdaptablePushButtonWidget()
-            qt_button.setText(text)
-            qt_button.setCheckable(True)
-
-            layout.addWidget(qt_button)
-            self.qt_button_group.addButton(qt_button, index)
-
-            self.wrapped_qt_buttons_map[index] = qt_button
-            self.wrapped_qt_buttons_map[text] = qt_button
-
-        self.qt_button_group.idReleased.connect(self.selection_changed_signal)
-
-    def set_selection(self, selection: Union[int, str]):
-        try:
-            self.wrapped_qt_buttons_map[selection].click()
-        except KeyError:
-            pass
-
-    def get_selected_item_index(self) -> Optional[int]:
-        return self.qt_button_group.checkedId()
-
-    def get_selected_item_text(self) -> Optional[str]:
-        if self.qt_button_group.checkedButton():
-            return self.qt_button_group.checkedButton().text()
-
-
-class GuiButtonSelectorH(GuiWidget):
-    """Button group to select value, horizontal layout."""
-    _qt_widget_class = ButtonGroupWidgetHorizontal
-
-    def __init__(self,
-                 content: Sequence[str],
-                 title: Optional[str] = None,
-                 color: Optional[Union[str, tuple[int, int, int]]] = None,
-                 *,
-                 select: Optional[Union[int, str]] = None):
-        """
-        Args:
-            content: Text for selector's buttons
-            title: Widget's title, `None` for same as content
-            color: Selector button's text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-            select: text or index of button to select initially
-        """
-        super().__init__(content, title, color, select=select)
-
-
-class ButtonGroupWidgetVertical(ButtonGroupWidgetHorizontal):
-    layout_class = QVBoxLayout
-
-
-class GuiButtonSelectorV(GuiWidget):
-    """Button group to select value, vertical layout."""
-    _qt_widget_class = ButtonGroupWidgetVertical
-
-    def __init__(self,
-                 content: Sequence[str],
-                 title: Optional[str] = None,
-                 color: Optional[Union[str, tuple[int, int, int]]] = None,
-                 *,
-                 select: Optional[Union[int, str]] = None):
-        """
-        Args:
-            content: Text for selector's buttons
-            title: Widget's title, `None` for same as content
-            color: Selector button's text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-            select: text or index of button to select initially
-        """
-        super().__init__(content, title, color, select=select)
+from typing import Optional, Union, Sequence
+
+from PySide6.QtWidgets import *
+
+from .gui_widget_base import GuiWidget
+from .mixins import AdaptiveTextSizeMixin, WrappedQWidgetMixin
+
+
+class AdaptablePushButtonWidget(AdaptiveTextSizeMixin, WrappedQWidgetMixin, QPushButton):
+    def __init__(self):
+        QPushButton.__init__(self)
+        WrappedQWidgetMixin.__init__(self)
+        AdaptiveTextSizeMixin.__init__(self)
+
+        self.get_content = self.text
+        self.set_content = self.setText
+
+
+class ButtonWidget(AdaptablePushButtonWidget):
+    def __init__(self):
+        super().__init__()
+        self.clicked.connect(self.triggered_signal)
+
+
+class GuiButton(GuiWidget):
+    """Simple button widget."""
+
+    _qt_widget_class = ButtonWidget
+
+    def __init__(self,
+                 content: str,
+                 title: Optional[str] = None,
+                 color: Optional[Union[str, tuple[int, int, int]]] = None):
+        """
+        Args:
+            content: Button text
+            title: Widget's title, `None` for same as content
+            color: Button text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
+        """
+        super().__init__(content, title, color)
+
+
+class ToggleButtonWidget(AdaptablePushButtonWidget):
+    def __init__(self):
+        super().__init__()
+        self.setCheckable(True)
+        self.toggled.connect(self.toggle_state_changed_signal)
+
+        self.get_toggle_state = self.isChecked
+        self.set_toggle_state = self.setChecked
+
+
+class GuiToggleButton(GuiWidget):
+    """Toggleable button."""
+
+    _qt_widget_class = ToggleButtonWidget
+
+    def __init__(self,
+                 content: str,
+                 title: Optional[str] = None,
+                 color: Optional[Union[str, tuple[int, int, int]]] = None,
+                 *,
+                 toggle_state: Optional[bool] = None):
+        """
+        Args:
+            content: Button text
+            title: Widget's title, `None` for same as content
+            color: Button text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
+            toggle_state: Button toggle state
+        """
+        super().__init__(content, title, color, toggle_state=toggle_state)
+
+
+class ButtonGroupWidgetHorizontal(WrappedQWidgetMixin, QWidget):
+    layout_class = QHBoxLayout
+
+    def __init__(self):
+        QWidget.__init__(self)
+        WrappedQWidgetMixin.__init__(self)
+        self.qt_button_group = QButtonGroup()
+        self.wrapped_qt_buttons_map = {}
+        self.__content = None
+
+    def get_content(self):
+        return self.__content
+
+    def set_content(self, button_labels: list[str]):
+        self.__content = button_labels
+
+        self.qt_button_group.deleteLater()
+        self.qt_button_group = QButtonGroup()
+        self.wrapped_qt_buttons_map: dict[Union[str, int], AdaptablePushButtonWidget] = {}
+
+        layout = self.layout_class()
+        layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(layout)
+
+        for index, text in enumerate(button_labels):
+            qt_button = AdaptablePushButtonWidget()
+            qt_button.setText(text)
+            qt_button.setCheckable(True)
+
+            layout.addWidget(qt_button)
+            self.qt_button_group.addButton(qt_button, index)
+
+            self.wrapped_qt_buttons_map[index] = qt_button
+            self.wrapped_qt_buttons_map[text] = qt_button
+
+        self.qt_button_group.idReleased.connect(self.selection_changed_signal)
+
+    def set_selection(self, selection: Union[int, str]):
+        try:
+            self.wrapped_qt_buttons_map[selection].click()
+        except KeyError:
+            pass
+
+    def get_selected_item_index(self) -> Optional[int]:
+        return self.qt_button_group.checkedId()
+
+    def get_selected_item_text(self) -> Optional[str]:
+        if self.qt_button_group.checkedButton():
+            return self.qt_button_group.checkedButton().text()
+
+
+class GuiButtonSelectorH(GuiWidget):
+    """Button group to select value, horizontal layout."""
+    _qt_widget_class = ButtonGroupWidgetHorizontal
+
+    def __init__(self,
+                 content: Sequence[str],
+                 title: Optional[str] = None,
+                 color: Optional[Union[str, tuple[int, int, int]]] = None,
+                 *,
+                 select: Optional[Union[int, str]] = None):
+        """
+        Args:
+            content: Text for selector's buttons
+            title: Widget's title, `None` for same as content
+            color: Selector button's text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
+            select: text or index of button to select initially
+        """
+        super().__init__(content, title, color, select=select)
+
+
+class ButtonGroupWidgetVertical(ButtonGroupWidgetHorizontal):
+    layout_class = QVBoxLayout
+
+
+class GuiButtonSelectorV(GuiWidget):
+    """Button group to select value, vertical layout."""
+    _qt_widget_class = ButtonGroupWidgetVertical
+
+    def __init__(self,
+                 content: Sequence[str],
+                 title: Optional[str] = None,
+                 color: Optional[Union[str, tuple[int, int, int]]] = None,
+                 *,
+                 select: Optional[Union[int, str]] = None):
+        """
+        Args:
+            content: Text for selector's buttons
+            title: Widget's title, `None` for same as content
+            color: Selector button's text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
+            select: text or index of button to select initially
+        """
+        super().__init__(content, title, color, select=select)
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/gui_widgets/gui_widget_base.py` & `midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_widget_base.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-from typing import Sequence, Optional, Union, TYPE_CHECKING
-
-from PySide6.QtWidgets import *
-
-import midiscripter.base.port_base
-import midiscripter.base.msg_base
-import midiscripter.gui.app
-from .gui_msg import GuiEventType, GuiEventMsg
-
-if TYPE_CHECKING:
-    from.mixins import WrappedQWidgetMixin
-
-
-class GuiWidget(midiscripter.base.port_base.Input):
-    """GUI windows widget which also acts like an input port."""
-    _qt_widget_class: type[QWidget, 'WrappedQWidgetMixin']
-
-    def __init__(self,
-                 content: Union[str, Sequence[str]],
-                 title: Optional[str] = None,
-                 color: Optional[Union[str, tuple[int, int, int]]] = None,
-                 *,
-                 value: Optional[str] = None,
-                 select: Optional[Union[int, str]] = None,
-                 toggle_state: Optional[bool] = None):
-        """
-        Args:
-            content: Widget's text or text for its items
-            title: Widget's title, `None` for same as content
-            color: Preset text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-            value: Preset value
-            select: Preset item text / index to select
-            toggle_state: Preset toggle state
-        """
-        self.title = title or str(content)
-        """Widget's title."""
-        super().__init__(self.title)
-
-        self.qt_widget = self._qt_widget_class()  # workaround for mkdocstrings issue #607
-
-        self.qt_widget: QWidget
-        """Wrapped `PySide6` `QWidget` that can be altered for extra customization."""
-        
-        self.qt_widget.setObjectName(self.title)
-        midiscripter.gui.app.add_qwidget(self.qt_widget)
-
-        self.content = content
-
-        if value:
-            self.value = value
-            
-        if select:
-            self.select(select)
-            
-        if toggle_state:
-            self.toggle_state = toggle_state
-
-        if color:
-            self.color = color
-
-        self.__connect_change_signals()
-
-    def __connect_change_signals(self):
-        self.qt_widget.triggered_signal.connect(
-            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.TRIGGERED)))
-        self.qt_widget.content_changed_signal.connect(
-            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.CONTENT_SET,
-                                                              self.qt_widget.get_content())))
-        self.qt_widget.value_changed_signal.connect(
-            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.VALUE_CHANGED,
-                                                              self.qt_widget.get_value())))
-        self.qt_widget.selection_changed_signal.connect(
-            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.SELECTED,
-                                                              self.qt_widget.get_selected_item_text())))
-        self.qt_widget.toggle_state_changed_signal.connect(
-            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.TOGGLED,
-                                                              self.qt_widget.get_toggle_state())))
-
-    @property
-    def content(self):
-        """Widget's text or text for its items."""
-        return self.qt_widget.get_content()
-
-    @content.setter
-    def content(self, new_content: Union[str, Sequence[str]]):
-        self.qt_widget.set_content_signal.emit(new_content)
-        self.qt_widget.content_changed_signal.emit()
-
-    @property
-    def value(self) -> Optional[str]:
-        """Widget's value / selected item text."""
-        try:
-            return self.qt_widget.get_value()
-        except NotImplementedError:
-            return None
-
-    @value.setter
-    def value(self, new_value):
-        self.qt_widget.set_value_signal.emit(new_value)
-        self.qt_widget.value_changed_signal.emit()
-
-    @property
-    def selected_item_text(self) -> Optional[str]:
-        """Widget's currently selected item's text."""
-        try:
-            return self.qt_widget.get_selected_item_text()
-        except NotImplementedError:
-            return None
-
-    @property
-    def selected_item_index(self) -> Optional[int]:
-        """Widget's currently selected item's index"""
-        try:
-            return self.qt_widget.get_selected_item_index()
-        except NotImplementedError:
-            return None
-
-    def select(self, selection: Union[int, str]):
-        """Select widget's item
-
-        Args:
-            selection: Index or text of item to select
-        """
-        self.qt_widget.set_selection_signal.emit(selection)
-        self.qt_widget.selection_changed_signal.emit()
-
-    @property
-    def toggle_state(self) -> Optional[bool]:
-        """Toggle state."""
-        try:
-            return self.qt_widget.get_toggle_state()
-        except NotImplementedError:
-            return None
-
-    @toggle_state.setter
-    def toggle_state(self, new_state: bool):
-        self.qt_widget.set_toggle_state_signal.emit(new_state)
-        self.qt_widget.toggle_state_changed_signal.emit()
-
-    @property
-    def color(self) -> Optional[Union[str, tuple[int, int, int]]]:
-        """Text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple"""
-        return self.qt_widget.get_color()
-
-    @color.setter
-    def color(self, new_color_value: Union[str, tuple[int, int, int]]):
-        self.qt_widget.set_color_signal.emit(new_color_value)
-        self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.COLOR_SET,
-                                                  new_color_value, source=self))
-
-    @property
-    def is_visible(self) -> bool:
-        """Widget is currently visible."""
-        return self.qt_widget.isVisible()
+from typing import Sequence, Optional, Union, TYPE_CHECKING
+
+from PySide6.QtWidgets import *
+
+import midiscripter.base.port_base
+import midiscripter.base.msg_base
+import midiscripter.gui.app
+from .gui_msg import GuiEventType, GuiEventMsg
+
+if TYPE_CHECKING:
+    from.mixins import WrappedQWidgetMixin
+
+
+class GuiWidget(midiscripter.base.port_base.Input):
+    """GUI windows widget which also acts like an input port."""
+    _qt_widget_class: type[QWidget, 'WrappedQWidgetMixin']
+
+    def __init__(self,
+                 content: Union[str, Sequence[str]],
+                 title: Optional[str] = None,
+                 color: Optional[Union[str, tuple[int, int, int]]] = None,
+                 *,
+                 value: Optional[str] = None,
+                 select: Optional[Union[int, str]] = None,
+                 toggle_state: Optional[bool] = None):
+        """
+        Args:
+            content: Widget's text or text for its items
+            title: Widget's title, `None` for same as content
+            color: Preset text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
+            value: Preset value
+            select: Preset item text / index to select
+            toggle_state: Preset toggle state
+        """
+        self.title = title or str(content)
+        """Widget's title."""
+        super().__init__(self.title)
+
+        self.qt_widget = self._qt_widget_class()  # workaround for mkdocstrings issue #607
+
+        self.qt_widget: QWidget
+        """Wrapped `PySide6` `QWidget` that can be altered for extra customization."""
+        
+        self.qt_widget.setObjectName(self.title)
+        midiscripter.gui.app.add_qwidget(self.qt_widget)
+
+        self.content = content
+
+        if value:
+            self.value = value
+            
+        if select:
+            self.select(select)
+            
+        if toggle_state:
+            self.toggle_state = toggle_state
+
+        if color:
+            self.color = color
+
+        self.__connect_change_signals()
+
+    def __connect_change_signals(self):
+        self.qt_widget.triggered_signal.connect(
+            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.TRIGGERED)))
+        self.qt_widget.content_changed_signal.connect(
+            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.CONTENT_SET,
+                                                              self.qt_widget.get_content())))
+        self.qt_widget.value_changed_signal.connect(
+            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.VALUE_CHANGED,
+                                                              self.qt_widget.get_value())))
+        self.qt_widget.selection_changed_signal.connect(
+            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.SELECTED,
+                                                              self.qt_widget.get_selected_item_text())))
+        self.qt_widget.toggle_state_changed_signal.connect(
+            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.TOGGLED,
+                                                              self.qt_widget.get_toggle_state())))
+
+    @property
+    def content(self):
+        """Widget's text or text for its items."""
+        return self.qt_widget.get_content()
+
+    @content.setter
+    def content(self, new_content: Union[str, Sequence[str]]):
+        self.qt_widget.set_content_signal.emit(new_content)
+        self.qt_widget.content_changed_signal.emit()
+
+    @property
+    def value(self) -> Optional[str]:
+        """Widget's value / selected item text."""
+        try:
+            return self.qt_widget.get_value()
+        except NotImplementedError:
+            return None
+
+    @value.setter
+    def value(self, new_value):
+        self.qt_widget.set_value_signal.emit(new_value)
+        self.qt_widget.value_changed_signal.emit()
+
+    @property
+    def selected_item_text(self) -> Optional[str]:
+        """Widget's currently selected item's text."""
+        try:
+            return self.qt_widget.get_selected_item_text()
+        except NotImplementedError:
+            return None
+
+    @property
+    def selected_item_index(self) -> Optional[int]:
+        """Widget's currently selected item's index"""
+        try:
+            return self.qt_widget.get_selected_item_index()
+        except NotImplementedError:
+            return None
+
+    def select(self, selection: Union[int, str]):
+        """Select widget's item
+
+        Args:
+            selection: Index or text of item to select
+        """
+        self.qt_widget.set_selection_signal.emit(selection)
+        self.qt_widget.selection_changed_signal.emit()
+
+    @property
+    def toggle_state(self) -> Optional[bool]:
+        """Toggle state."""
+        try:
+            return self.qt_widget.get_toggle_state()
+        except NotImplementedError:
+            return None
+
+    @toggle_state.setter
+    def toggle_state(self, new_state: bool):
+        self.qt_widget.set_toggle_state_signal.emit(new_state)
+        self.qt_widget.toggle_state_changed_signal.emit()
+
+    @property
+    def color(self) -> Optional[Union[str, tuple[int, int, int]]]:
+        """Text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple"""
+        return self.qt_widget.get_color()
+
+    @color.setter
+    def color(self, new_color_value: Union[str, tuple[int, int, int]]):
+        self.qt_widget.set_color_signal.emit(new_color_value)
+        self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.COLOR_SET,
+                                                  new_color_value, source=self))
+
+    @property
+    def is_visible(self) -> bool:
+        """Widget is currently visible."""
+        return self.qt_widget.isVisible()
```

### Comparing `midiscripter-0.1.1/midiscripter/gui/gui_widgets/mixins.py` & `midiscripter-0.1.2/midiscripter/gui/gui_widgets/mixins.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from typing import Sequence, Optional, Union
-
-from PySide6.QtCore import *
-from PySide6.QtWidgets import *
-from PySide6.QtGui import *
-
-
-# noinspection PyUnresolvedReferences
-class WrappedQWidgetMixin:
-    # Signals are required to emit them from another thread that is not possible for setter methods below
-    set_content_signal = Signal(object)
-    set_value_signal = Signal(object)
-    set_selection_signal = Signal(object)
-    set_toggle_state_signal = Signal(bool)
-    set_color_signal = Signal(object)
-
-    triggered_signal = Signal()
-    content_changed_signal = Signal()
-    value_changed_signal = Signal()
-    selection_changed_signal = Signal()
-    toggle_state_changed_signal = Signal()
-
-    def __init__(self):
-        self.__color = None
-
-        self.set_content_signal.connect(self.set_content)
-        self.set_value_signal.connect(self.set_value)
-        self.set_selection_signal.connect(self.set_selection)
-        self.set_toggle_state_signal.connect(self.set_toggle_state)
-        self.set_color_signal.connect(self.set_color)
-
-    def get_content(self) -> Union[str, Sequence[str]]:
-        raise NotImplementedError
-
-    def set_content(self, new_content: Union[str, Sequence[str]]):
-        raise NotImplementedError
-
-    def get_value(self) -> Optional[str]:
-        raise NotImplementedError
-
-    def set_value(self, new_value: Union[str, int, bool]):
-        raise NotImplementedError
-
-    def get_selected_item_index(self) -> Optional[int]:
-        raise NotImplementedError
-
-    def get_selected_item_text(self) -> Optional[str]:
-        raise NotImplementedError
-
-    def set_selection(self, selection: Union[int, str]):
-        raise NotImplementedError
-
-    def get_toggle_state(self) -> Optional[bool]:
-        raise NotImplementedError
-
-    def set_toggle_state(self, new_state: bool):
-        raise NotImplementedError
-
-    def get_color(self) -> Optional[str]:
-        return self.__color
-
-    def set_color(self, new_color_value: Union[str, tuple[int, int, int]]):
-        if isinstance(new_color_value, str):
-            color = QColor(new_color_value)
-        else:
-            color = QColor(*new_color_value)
-
-        palette = self.palette()
-        palette.setColor(QPalette.ColorGroup.Active, QPalette.ColorRole.ButtonText, color)
-        palette.setColor(QPalette.ColorGroup.Active, QPalette.ColorRole.WindowText, color)
-        self.setPalette(palette)
-        self.__color = new_color_value
-
-# noinspection PyUnresolvedReferences, PyPep8Naming
-class AdaptiveTextSizeMixin:
-    def __init__(self):
-        self.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Ignored, QSizePolicy.Policy.Ignored))
-        self.setContentsMargins(10, 5, 10, 5)
-        self.__longest_text_rect_size = QFontMetrics(self.font()).boundingRect(self.text()).size()
-
-    def setText(self, text: str) -> None:
-        super().setText(text)
-
-        text_rect = QFontMetrics(self.font()).boundingRect(self.text())
-        if (text_rect.height() > self.__longest_text_rect_size.height() or
-                text_rect.width() > self.__longest_text_rect_size.width()):
-            self.__make_text_size_fit_widget_size()
-            self.__longest_text_rect_size = text_rect
-
-    def resizeEvent(self, event):
-        super().resizeEvent(event)
-        self.__make_text_size_fit_widget_size()
-
-    def __make_text_size_fit_widget_size(self):
-        if not self.text():
-            return
-
-        font = self.font()
-        content_rect = self.contentsRect()
-
-        font_size = 0
-        text_rect = QSize()
-        while (text_rect.height() < content_rect.height()
-               and text_rect.width() < content_rect.width()):
-            font_size += 1
-            font.setPixelSize(font_size)
-            text_rect = QFontMetrics(font).boundingRect(self.text())
-
-        self.setFont(font)
+from typing import Sequence, Optional, Union
+
+from PySide6.QtCore import *
+from PySide6.QtWidgets import *
+from PySide6.QtGui import *
+
+
+# noinspection PyUnresolvedReferences
+class WrappedQWidgetMixin:
+    # Signals are required to emit them from another thread that is not possible for setter methods below
+    set_content_signal = Signal(object)
+    set_value_signal = Signal(object)
+    set_selection_signal = Signal(object)
+    set_toggle_state_signal = Signal(bool)
+    set_color_signal = Signal(object)
+
+    triggered_signal = Signal()
+    content_changed_signal = Signal()
+    value_changed_signal = Signal()
+    selection_changed_signal = Signal()
+    toggle_state_changed_signal = Signal()
+
+    def __init__(self):
+        self.__color = None
+
+        self.set_content_signal.connect(self.set_content)
+        self.set_value_signal.connect(self.set_value)
+        self.set_selection_signal.connect(self.set_selection)
+        self.set_toggle_state_signal.connect(self.set_toggle_state)
+        self.set_color_signal.connect(self.set_color)
+
+    def get_content(self) -> Union[str, Sequence[str]]:
+        raise NotImplementedError
+
+    def set_content(self, new_content: Union[str, Sequence[str]]):
+        raise NotImplementedError
+
+    def get_value(self) -> Optional[str]:
+        raise NotImplementedError
+
+    def set_value(self, new_value: Union[str, int, bool]):
+        raise NotImplementedError
+
+    def get_selected_item_index(self) -> Optional[int]:
+        raise NotImplementedError
+
+    def get_selected_item_text(self) -> Optional[str]:
+        raise NotImplementedError
+
+    def set_selection(self, selection: Union[int, str]):
+        raise NotImplementedError
+
+    def get_toggle_state(self) -> Optional[bool]:
+        raise NotImplementedError
+
+    def set_toggle_state(self, new_state: bool):
+        raise NotImplementedError
+
+    def get_color(self) -> Optional[str]:
+        return self.__color
+
+    def set_color(self, new_color_value: Union[str, tuple[int, int, int]]):
+        if isinstance(new_color_value, str):
+            color = QColor(new_color_value)
+        else:
+            color = QColor(*new_color_value)
+
+        palette = self.palette()
+        palette.setColor(QPalette.ColorGroup.Active, QPalette.ColorRole.ButtonText, color)
+        palette.setColor(QPalette.ColorGroup.Active, QPalette.ColorRole.WindowText, color)
+        self.setPalette(palette)
+        self.__color = new_color_value
+
+# noinspection PyUnresolvedReferences, PyPep8Naming
+class AdaptiveTextSizeMixin:
+    def __init__(self):
+        self.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Ignored, QSizePolicy.Policy.Ignored))
+        self.setContentsMargins(10, 5, 10, 5)
+        self.__longest_text_rect_size = QFontMetrics(self.font()).boundingRect(self.text()).size()
+
+    def setText(self, text: str) -> None:
+        super().setText(text)
+
+        text_rect = QFontMetrics(self.font()).boundingRect(self.text())
+        if (text_rect.height() > self.__longest_text_rect_size.height() or
+                text_rect.width() > self.__longest_text_rect_size.width()):
+            self.__make_text_size_fit_widget_size()
+            self.__longest_text_rect_size = text_rect
+
+    def resizeEvent(self, event):
+        super().resizeEvent(event)
+        self.__make_text_size_fit_widget_size()
+
+    def __make_text_size_fit_widget_size(self):
+        if not self.text():
+            return
+
+        font = self.font()
+        content_rect = self.contentsRect()
+
+        font_size = 0
+        text_rect = QSize()
+        while (text_rect.height() < content_rect.height()
+               and text_rect.width() < content_rect.width()):
+            font_size += 1
+            font.setPixelSize(font_size)
+            text_rect = QFontMetrics(font).boundingRect(self.text())
+
+        self.setFont(font)
```

### Comparing `midiscripter-0.1.1/midiscripter/keyboard/keyboard_port.py` & `midiscripter-0.1.2/midiscripter/keyboard/keyboard_port.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,103 @@
-import pynput.keyboard
-
-import midiscripter.base.port_base
-import midiscripter.osc.osc_msg
-from midiscripter.logger import log
-from midiscripter.keyboard.keyboard_msg import KeyMsg, KeyEventType
-
-
-class KeyIn(midiscripter.base.port_base.Input):
-    """Keyboard input port. Produces [`KeyMsg`][midiscripter.KeyMsg] objects."""
-    
-    _force_uid = 'Keyboard In'
-
-    def __init__(self):
-        super().__init__(self._force_uid)
-        self.pynput_listener = None
-        self.pressed_keys = []
-    
-    def __on_press(self, key: pynput.keyboard.Key):
-        if not self.is_enabled:
-            return 
-        
-        if type(key) is pynput.keyboard.KeyCode:
-            key = self.pynput_listener.canonical(key)
-            
-        if key not in self.pressed_keys:
-            self.pressed_keys.append(key)
-            
-        msg = KeyMsg(KeyEventType.KEY_PRESS, self.pressed_keys.copy(), source=self)
-        self._send_input_msg_to_calls(msg)
-        
-    def __on_release(self, key: pynput.keyboard.Key):    
-        if not self.is_enabled:
-            return 
-        
-        if type(key) is pynput.keyboard.KeyCode:
-            key = self.pynput_listener.canonical(key)
-       
-        try:
-            pressed_keys_for_msg = self.pressed_keys.copy()
-            self.pressed_keys.remove(key)
-            
-            msg = KeyMsg(KeyEventType.KEY_RELEASE, pressed_keys_for_msg, source=self)
-            self._send_input_msg_to_calls(msg)
-        except ValueError:
-            pass
-        
-    def _open(self):
-        if self.pynput_listener:
-            return 
-        
-        self.pynput_listener = pynput.keyboard.Listener(self.__on_press, self.__on_release)
-        self.pynput_listener.start()
-        self.pynput_listener.wait()
-        self.is_enabled = True
-        log(f'Started keyboard input listener')
-
-    def _close(self):
-        self.pynput_listener.stop()
-        self.is_enabled = False
-        log(f'Stopped keyboard input listener')
-
-
-class KeyOut(midiscripter.base.port_base.Output):
-    """Keyboard output port. Sends [`KeyMsg`][midiscripter.KeyMsg] objects."""
-
-    _force_uid = 'Keyboard Output'
-    
-    def __init__(self):
-        super().__init__(self._force_uid)
-        self.pynput_controller = pynput.keyboard.Controller()
-        
-    def send(self, msg: KeyMsg):        
-        """Send the keyboard input.
-
-        Args:
-            msg: object to send
-        """   
-        # Log messages sent before actual sending, so receive messages for sent keys 
-        # won't be displayed before the message
-        with self._check_and_log_sent_message(msg):
-            pass
-            
-        if msg.type is KeyEventType.KEY_PRESS:
-            for keycode in msg.keycodes:
-                self.pynput_controller.press(keycode)
-                
-        elif msg.type is KeyEventType.KEY_RELEASE:
-            for keycode in msg.keycodes:
-                self.pynput_controller.release(keycode)
-                
-        elif msg.type is KeyEventType.KEY_TAP:
-            for keycode in msg.keycodes:
-                self.pynput_controller.press(keycode)
-            for keycode in reversed(msg.keycodes):
-                self.pynput_controller.release(keycode)
-    
-    def type_in(self, string_to_type: str):
-        self.pynput_controller.type(string_to_type)
+import pynput.keyboard
+
+import midiscripter.base.port_base
+import midiscripter.osc.osc_msg
+from midiscripter.logger import log
+from midiscripter.keyboard.keyboard_msg import KeyMsg, KeyEventType
+
+
+class KeyIn(midiscripter.base.port_base.Input):
+    """Keyboard input port. Produces [`KeyMsg`][midiscripter.KeyMsg] objects."""
+
+    pressed_keys: list[pynput.keyboard.Key]
+    """Currently pressed keys"""
+    
+    _force_uid = 'Keyboard In'
+
+    def __init__(self):
+        """ """  # to override Input docstring
+        super().__init__(self._force_uid)
+        self.__pynput_listener = None
+        self.pressed_keys = []
+    
+    def __on_press(self, key: pynput.keyboard.Key):
+        if not self.is_enabled:
+            return 
+        
+        if type(key) is pynput.keyboard.KeyCode:
+            key = self.__pynput_listener.canonical(key)
+            
+        if key not in self.pressed_keys:
+            self.pressed_keys.append(key)
+            
+        msg = KeyMsg(KeyEventType.KEY_PRESS, self.pressed_keys.copy(), source=self)
+        self._send_input_msg_to_calls(msg)
+        
+    def __on_release(self, key: pynput.keyboard.Key):    
+        if not self.is_enabled:
+            return 
+        
+        if type(key) is pynput.keyboard.KeyCode:
+            key = self.__pynput_listener.canonical(key)
+       
+        try:
+            pressed_keys_for_msg = self.pressed_keys.copy()
+            self.pressed_keys.remove(key)
+            
+            msg = KeyMsg(KeyEventType.KEY_RELEASE, pressed_keys_for_msg, source=self)
+            self._send_input_msg_to_calls(msg)
+        except ValueError:
+            pass
+        
+    def _open(self):
+        if self.__pynput_listener:
+            return 
+        
+        self.__pynput_listener = pynput.keyboard.Listener(self.__on_press, self.__on_release)
+        self.__pynput_listener.start()
+        self.__pynput_listener.wait()
+        self.is_enabled = True
+        log(f'Started keyboard input listener')
+
+    def _close(self):
+        self.__pynput_listener.stop()
+        self.is_enabled = False
+        log(f'Stopped keyboard input listener')
+
+
+class KeyOut(midiscripter.base.port_base.Output):
+    """Keyboard output port. Sends [`KeyMsg`][midiscripter.KeyMsg] objects."""
+
+    _force_uid = 'Keyboard Output'
+    
+    def __init__(self):
+        super().__init__(self._force_uid)
+        self.__pynput_controller = pynput.keyboard.Controller()
+        
+    def send(self, msg: KeyMsg):        
+        """Send the keyboard input.
+
+        Args:
+            msg: object to send
+        """   
+        # Log messages sent before actual sending, so receive messages for sent keys 
+        # won't be displayed before the message
+        with self._check_and_log_sent_message(msg):
+            pass
+            
+        if msg.type is KeyEventType.KEY_PRESS:
+            for keycode in msg.keycodes:
+                self.__pynput_controller.press(keycode)
+                
+        elif msg.type is KeyEventType.KEY_RELEASE:
+            for keycode in msg.keycodes:
+                self.__pynput_controller.release(keycode)
+                
+        elif msg.type is KeyEventType.KEY_TAP:
+            for keycode in msg.keycodes:
+                self.__pynput_controller.press(keycode)
+            for keycode in reversed(msg.keycodes):
+                self.__pynput_controller.release(keycode)
+    
+    def type_in(self, string_to_type: str):
+        self.__pynput_controller.type(string_to_type)
```

### Comparing `midiscripter-0.1.1/midiscripter/logger/console_sink.py` & `midiscripter-0.1.2/midiscripter/logger/console_sink.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import sys
-from typing import Callable
-
-import colorama
-
-from midiscripter.base.port_base import Input, Output
-from midiscripter.base.msg_base import Msg
-
-
-class ConsoleSink:
-    COLOR_MAP = {Input: colorama.Fore.GREEN,  # Possible colors for CLI are:
-                 Output: colorama.Fore.MAGENTA,  # black, red, green, yellow,
-                 Msg: colorama.Fore.BLUE,  # blue, magenta, cyan, white
-                 Callable: colorama.Fore.CYAN}
-
-    def __call__(self, log_entries: list[tuple[str, dict]]):
-        entries = []
-        for entry in log_entries:
-            text = entry[0]
-            kwargs = entry[1]
-            
-            if not text:
-                entries.append('\n')
-                continue
-            
-            if '_color' in kwargs and kwargs['_color'].upper() in vars(colorama.Fore):
-                main_color_tag = getattr(colorama.Fore, kwargs['_color'].upper())
-                text = f'{main_color_tag}{text}{colorama.Style.RESET_ALL}'
-            else:
-                main_color_tag = colorama.Style.RESET_ALL
-            
-            for arg_name, arg_object in kwargs.items():
-                for obj_type in (Input, Output, Msg, Callable):
-                    if isinstance(arg_object, obj_type):
-                        kwargs[arg_name] = (self.COLOR_MAP[obj_type] + str(arg_object) 
-                                            + main_color_tag)
-
-            ctime_text = (f'{colorama.Style.DIM}{kwargs["_ctime_str"]}: '
-                          f'{colorama.Style.RESET_ALL}')
-
-            entry_text = ctime_text + text + '\n'
-
-            try:
-                entries.append(entry_text.format(**kwargs))
-            except KeyError:
-                entries.append(entry_text)
-
-        output = ''.join(entries)
-
-        sys.stdout.write(output)
-        sys.stdout.flush()
+import sys
+from typing import Callable
+
+import colorama
+
+from midiscripter.base.port_base import Input, Output
+from midiscripter.base.msg_base import Msg
+
+
+class ConsoleSink:
+    COLOR_MAP = {Input: colorama.Fore.GREEN,  # Possible colors for CLI are:
+                 Output: colorama.Fore.MAGENTA,  # black, red, green, yellow,
+                 Msg: colorama.Fore.BLUE,  # blue, magenta, cyan, white
+                 Callable: colorama.Fore.CYAN}
+
+    def __call__(self, log_entries: list[tuple[str, dict]]):
+        entries = []
+        for entry in log_entries:
+            text = entry[0]
+            kwargs = entry[1]
+            
+            if not text:
+                entries.append('\n')
+                continue
+            
+            if '_color' in kwargs and kwargs['_color'].upper() in vars(colorama.Fore):
+                main_color_tag = getattr(colorama.Fore, kwargs['_color'].upper())
+                text = f'{main_color_tag}{text}{colorama.Style.RESET_ALL}'
+            else:
+                main_color_tag = colorama.Style.RESET_ALL
+            
+            for arg_name, arg_object in kwargs.items():
+                for obj_type in (Input, Output, Msg, Callable):
+                    if isinstance(arg_object, obj_type):
+                        kwargs[arg_name] = (self.COLOR_MAP[obj_type] + str(arg_object) 
+                                            + main_color_tag)
+
+            ctime_text = (f'{colorama.Style.DIM}{kwargs["_ctime_str"]}: '
+                          f'{colorama.Style.RESET_ALL}')
+
+            entry_text = ctime_text + text + '\n'
+
+            try:
+                entries.append(entry_text.format(**kwargs))
+            except KeyError:
+                entries.append(entry_text)
+
+        output = ''.join(entries)
+
+        sys.stdout.write(output)
+        sys.stdout.flush()
```

### Comparing `midiscripter-0.1.1/midiscripter/logger/custom_logger.py` & `midiscripter-0.1.2/midiscripter/logger/log.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,120 +1,127 @@
-import time
-import threading
-import collections
-from typing import Union, TYPE_CHECKING, Callable
-
-import midiscripter.base.shared
-
-if TYPE_CHECKING:
-    from midiscripter.logger.html_sink import HtmlSink
-    from midiscripter.logger.console_sink import ConsoleSink
-
-
-class CustomLogger:
-    """Prints log messages to GUI Log widget or console. 
-    Can print messages in different text colors.
-    
-    Example:
-        `log('message')` for new log entry  
-        `log.red('red message')` for log entry printed in red color
-    """
-    
-    FLUSH_DELAY = 0.1
-    
-    ADD_SPACER_THRESHOLD_SEC = 2
-    """Time in seconds after which an empty line is added to log to separate logged actions"""
-    
-    BUFFER_SIZE = 200
-    """Max size of message buffer to flush to log widget when it becomes visible"""
-
-    def __init__(self):
-        self.__sink = None
-        self.is_enabled = True
-
-        self.__buffer = collections.deque(maxlen=self.BUFFER_SIZE)
-        self.__start_buffer_flush_thread()
-        self.__wait_counter = 0
-    
-    def __call__(self, text, **kwargs):
-        """Print log message.
-
-        Args:
-            text: Log entry to print in f-string format.
-            **kwargs: Optional variables to `.format` text with.
-        """
-        if not self.is_enabled:
-            return
-
-        precise_time = midiscripter.base.shared.precise_epoch_time()
-        time_string = time.strftime('%H:%M:%S', time.localtime(precise_time))
-
-        # >1.5 times faster than datetime
-        after_dot = repr(precise_time).split('.')[1][:6].ljust(6, '0')
-        milisec_part = after_dot[:3]
-        microsec_part = after_dot[3:]
-        kwargs['_ctime_str'] = f'{time_string}.{milisec_part},{microsec_part}'
-
-        self.__buffer.append((str(text), kwargs))
-
-    @property
-    def _sink(self):
-        """A callable that receives a list of log strings to print them for user.
-        Set by starter. Can be altered to customize the logger."""
-        return self.__sink
-
-    @_sink.setter
-    def _sink(self, sink_obj: Union['HtmlSink', 'ConsoleSink', Callable[[list[str]], None]]):
-        self.__sink = sink_obj
-        self._flush()
-        self.__start_buffer_flush_thread()
-
-    def __start_buffer_flush_thread(self):
-        threading.Thread(target=self._buffer_flush_worker, daemon=True).start()
-
-    def _buffer_flush_worker(self):
-        """Thread worker loop that flushes buffered messages"""
-        while self._sink:
-            time.sleep(self.FLUSH_DELAY)
-            self.__wait_counter += self.FLUSH_DELAY
-            if self.__buffer:
-                self._flush()
-
-    def _flush(self):
-        """Sends buffered messages to sink"""
-        output_entries = []
-
-        if self.__wait_counter > self.ADD_SPACER_THRESHOLD_SEC:
-            output_entries.append(('', dict()))
-        self.__wait_counter = 0
-
-        while self.__buffer:
-            output_entries.append(self.__buffer.popleft())  # for thread safety
-
-        try:
-            self._sink(output_entries)
-        except (TypeError, RuntimeError):  # ignore Qt error on widget destruction at app exit
-            pass
-
-    def red(self, text: str, **kwargs):
-        """Print red log message."""
-        self(text, _color='red', **kwargs)
-
-    def blue(self, text: str, **kwargs):
-        """Print blue log message."""
-        self(text, _color='blue', **kwargs)
-
-    def cyan(self, text: str, **kwargs):
-        """Print cyan log message."""
-        self(text, _color='cyan', **kwargs)
-
-    def magenta(self, text: str, **kwargs):
-        """Print magenta log message."""
-        self(text, _color='magenta', **kwargs)
-
-    def green(self, text: str, **kwargs):
-        """Print green log message."""
-        self(text, _color='green', **kwargs)
-
-    def yellow(self, text: str, **kwargs):
-        """Print yellow log message."""
-        self(text, _color='yellow', **kwargs)
+import time
+import threading
+import collections
+from typing import Union, TYPE_CHECKING, Callable
+
+import midiscripter.base.shared
+
+if TYPE_CHECKING:
+    from midiscripter.logger.html_sink import HtmlSink
+    from midiscripter.logger.console_sink import ConsoleSink
+
+
+class Log:
+    """Prints log messages to GUI Log widget or console.  
+    Can print messages in different text colors and highlight object representations.
+    
+    Example:
+        `log('message')` for new log entry  
+        
+        `log.red('red message')` for log entry printed in red color  
+        
+        `log('{call} received {msg}', call=call_function, msg=some_msg)` 
+        for log entry with highlighted object representations.
+    """
+    
+    FLUSH_DELAY = 0.1
+    
+    ADD_SPACER_THRESHOLD_SEC = 2
+    """Time in seconds after which an empty line is added to log to separate logged actions"""
+    
+    BUFFER_SIZE = 200
+    """Max size of message buffer to flush to log widget when it becomes visible"""
+
+    def __init__(self):
+        self.__sink = None
+        self.is_enabled = True
+
+        self.__buffer = collections.deque(maxlen=self.BUFFER_SIZE)
+        self.__start_buffer_flush_thread()
+        self.__wait_counter = 0
+    
+    def __call__(self, text, **kwargs):
+        """Print log message.
+
+        Args:
+            text: Log entry to print. Use `.format` style string to insert kwargs.
+            **kwargs: Optional variables to `.format` text with. 
+                      Passed [inputs][midiscripter.base.port_base.Input], 
+                      [outputs][midiscripter.base.port_base.Output], 
+                      [messages][midiscripter.base.msg_base.Msg] and callables are highlighted.
+        """
+        if not self.is_enabled:
+            return
+
+        precise_time = midiscripter.base.shared.precise_epoch_time()
+        time_string = time.strftime('%H:%M:%S', time.localtime(precise_time))
+
+        # >1.5 times faster than datetime
+        after_dot = repr(precise_time).split('.')[1][:6].ljust(6, '0')
+        milisec_part = after_dot[:3]
+        microsec_part = after_dot[3:]
+        kwargs['_ctime_str'] = f'{time_string}.{milisec_part},{microsec_part}'
+
+        self.__buffer.append((str(text), kwargs))
+
+    @property
+    def _sink(self):
+        """A callable that receives a list of log strings to print them for user.
+        Set by starter. Can be altered to customize the logger."""
+        return self.__sink
+
+    @_sink.setter
+    def _sink(self, sink_obj: Union['HtmlSink', 'ConsoleSink', Callable[[list[str]], None]]):
+        self.__sink = sink_obj
+        self._flush()
+        self.__start_buffer_flush_thread()
+
+    def __start_buffer_flush_thread(self):
+        threading.Thread(target=self._buffer_flush_worker, daemon=True).start()
+
+    def _buffer_flush_worker(self):
+        """Thread worker loop that flushes buffered messages"""
+        while self._sink:
+            time.sleep(self.FLUSH_DELAY)
+            self.__wait_counter += self.FLUSH_DELAY
+            if self.__buffer:
+                self._flush()
+
+    def _flush(self):
+        """Sends buffered messages to sink"""
+        output_entries = []
+
+        if self.__wait_counter > self.ADD_SPACER_THRESHOLD_SEC:
+            output_entries.append(('', dict()))
+        self.__wait_counter = 0
+
+        while self.__buffer:
+            output_entries.append(self.__buffer.popleft())  # for thread safety
+
+        try:
+            self._sink(output_entries)
+        except (TypeError, RuntimeError):  # ignore Qt error on widget destruction at app exit
+            pass
+
+    def red(self, text: str, **kwargs):
+        """Print red log message."""
+        self(text, _color='red', **kwargs)
+
+    def blue(self, text: str, **kwargs):
+        """Print blue log message."""
+        self(text, _color='blue', **kwargs)
+
+    def cyan(self, text: str, **kwargs):
+        """Print cyan log message."""
+        self(text, _color='cyan', **kwargs)
+
+    def magenta(self, text: str, **kwargs):
+        """Print magenta log message."""
+        self(text, _color='magenta', **kwargs)
+
+    def green(self, text: str, **kwargs):
+        """Print green log message."""
+        self(text, _color='green', **kwargs)
+
+    def yellow(self, text: str, **kwargs):
+        """Print yellow log message."""
+        self(text, _color='yellow', **kwargs)
```

### Comparing `midiscripter-0.1.1/midiscripter/logger/html_sink.py` & `midiscripter-0.1.2/midiscripter/logger/html_sink.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from typing import Callable
-
-from midiscripter.base.port_base import Input, Output
-from midiscripter.base.msg_base import Msg
-
-
-def to_html_link(text: str, color: str, link_text: str) -> str:
-    return f'<a href="{link_text}" style="color: {color};">{text}</a>'
-
-
-def to_html_colored_text(text: str, color: str) -> str:
-    return f'<font color="{color}">{text}</font>'
-
-
-class HtmlSink:
-    COLOR_MAP = {Input: 'darkGreen',  # Possible colors for CLI are:
-                 Output: 'darkMagenta',  # black, red, green, yellow,
-                 Msg: 'darkBlue',  # blue, magenta, cyan, white
-                 Callable: 'darkCyan'}
-
-    def __init__(self, sink_function: Callable):
-        self.sink_function = sink_function
-    
-    def __call__(self, log_entries: list[tuple[str, dict]]):
-        html_entries = []
-        for entry in log_entries:
-            text = entry[0]
-            kwargs = entry[1]
-
-            text = text.replace('\n', '<br>')
-            text = text.replace(' ', '&nbsp;')
-
-            if '_color' in kwargs:
-                text = to_html_colored_text(text, f'dark{kwargs["_color"]}')
-            
-            for arg_name, arg_object in kwargs.items():
-                
-                for obj_type in (Input, Output, Msg):
-                    if isinstance(arg_object, obj_type):
-                        kwargs[arg_name] = to_html_link(str(arg_object), self.COLOR_MAP[obj_type],
-                                                        arg_object.__repr__())
-                else:
-                    if isinstance(arg_object, Callable):
-                        kwargs[arg_name] = to_html_colored_text(arg_object.__name__,
-                                                                self.COLOR_MAP[Callable])
-
-            if text:
-                ctime_text = to_html_colored_text(kwargs["_ctime_str"], 'grey')
-                html_entry = f'{ctime_text}: {text}'
-            else:
-                html_entry = ''
-            
-            try:
-                html_entries.append(html_entry.format(**kwargs))
-            except KeyError:
-                html_entries.append(html_entry)
-
-        self.sink_function(html_entries)
+from typing import Callable
+
+from midiscripter.base.port_base import Input, Output
+from midiscripter.base.msg_base import Msg
+
+
+def to_html_link(text: str, color: str, link_text: str) -> str:
+    return f'<a href="{link_text}" style="color: {color};">{text}</a>'
+
+
+def to_html_colored_text(text: str, color: str) -> str:
+    return f'<font color="{color}">{text}</font>'
+
+
+class HtmlSink:
+    COLOR_MAP = {Input: 'darkGreen',  # Possible colors for CLI are:
+                 Output: 'darkMagenta',  # black, red, green, yellow,
+                 Msg: 'darkBlue',  # blue, magenta, cyan, white
+                 Callable: 'darkCyan'}
+
+    def __init__(self, sink_function: Callable):
+        self.sink_function = sink_function
+    
+    def __call__(self, log_entries: list[tuple[str, dict]]):
+        html_entries = []
+        for entry in log_entries:
+            text = entry[0]
+            kwargs = entry[1]
+
+            text = text.replace('\n', '<br>')
+            text = text.replace(' ', '&nbsp;')
+
+            if '_color' in kwargs:
+                text = to_html_colored_text(text, f'dark{kwargs["_color"]}')
+            
+            for arg_name, arg_object in kwargs.items():
+                
+                for obj_type in (Input, Output, Msg):
+                    if isinstance(arg_object, obj_type):
+                        kwargs[arg_name] = to_html_link(str(arg_object), self.COLOR_MAP[obj_type],
+                                                        arg_object.__repr__())
+                else:
+                    if isinstance(arg_object, Callable):
+                        kwargs[arg_name] = to_html_colored_text(arg_object.__name__,
+                                                                self.COLOR_MAP[Callable])
+
+            if text:
+                ctime_text = to_html_colored_text(kwargs["_ctime_str"], 'grey')
+                html_entry = f'{ctime_text}: {text}'
+            else:
+                html_entry = ''
+            
+            try:
+                html_entries.append(html_entry.format(**kwargs))
+            except KeyError:
+                html_entries.append(html_entry)
+
+        self.sink_function(html_entries)
```

### Comparing `midiscripter-0.1.1/midiscripter/midi/midi_msg.py` & `midiscripter-0.1.2/midiscripter/midi/midi_msg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,155 +1,170 @@
-from typing import Sequence, Optional, Union, TYPE_CHECKING
-
-import rtmidi.midiconstants
-
-import midiscripter.base.msg_base
-
-if TYPE_CHECKING:
-    import midiscripter.base.port_base
-    from midiscripter.midi.midi_port import MidiIn
-
-
-class MidiType(midiscripter.base.msg_base.AttrEnum):
-    """MIDI message type enumerator to use as [`MidiMsg`][midiscripter.MidiMsg] `type` attribute."""
-    NOTE_ON = 'NOTE_ON'
-    NOTE_OFF = 'NOTE_OFF'
-    POLYTOUCH = 'POLYTOUCH'
-    AFTERTOUCH = 'AFTERTOUCH'
-    CONTROL_CHANGE = 'CONTROL_CHANGE'
-    PROGRAM_CHANGE = 'PROGRAM_CHANGE'
-    PITCH_BEND = 'PITCH_BEND'
-    SYSEX = 'SYSEX'
-
-
-class MidiMsg(midiscripter.base.msg_base.Msg):
-    """The base class for MIDI message that sets the common attributes
-    for [`ChannelMsg`][midiscripter.ChannelMsg] and [`SysexMsg`][midiscripter.SysexMsg].
-
-    `MidiMsg` class will produce [`ChannelMsg`][midiscripter.ChannelMsg]
-    or [`SysexMsg`][midiscripter.SysexMsg] objects depending on init arguments.
-
-    It is advised to use [`ChannelMsg`][midiscripter.ChannelMsg] 
-    or [`SysexMsg`][midiscripter.SysexMsg] classes 
-    to create MIDI messages in calls for clarity.
-    """
-    __match_args__: tuple[str] = ('type', 'channel', 'data1', 'data2')
-
-    type: MidiType
-    channel: Union[int, tuple[int], tuple[int, int, int]]
-    data1: Union[int, tuple[int, int]]
-    data2: Union[int, tuple[int, ...]]
-    combined_data: Union[int, tuple[int, ...]]
-
-    def __new__(cls, *args, **kwargs):
-        if isinstance(args[0], tuple) or not args and 'combined_data' in kwargs:
-            return SysexMsg.__new__(*args, **kwargs)
-        else:
-            return ChannelMsg.__new__(*args, **kwargs)
-
-    def matches(self, type=None, channel=None, data1=None, data2=None) -> bool:
-        return super(MidiMsg, self).matches(type, channel, data1, data2)
-
-
-class ChannelMsg(MidiMsg):
-    """Channel voice/mode MIDI message. The most common MIDI message."""
-
-    type: MidiType
-    """MIDI message type."""
-
-    channel: int
-    """MIDI message channel (1-16)."""
-
-    data1: int
-    """First data byte: note, control, program or aftertouch value 
-    depending on MIDI message type (0-127)."""
-
-    data2: int
-    """Second data byte: velocity, value depending on MIDI message type (0-127)."""
-
-    def __new__(cls, *args, **kwargs):
-        """Resets base class custom __new__"""
-        return object.__new__(ChannelMsg)
-
-    def __init__(self, type: MidiType, channel: int = 1, data1: int = 0, data2: int = 127,
-                 *, source: Optional['MidiIn'] = None):
-        """
-        Args:
-            type: MIDI message type.
-            channel: MIDI message channel
-            data1: First data byte: note, control, program or aftertouch value
-            depending on MIDI message type
-            data2: Second data byte: velocity, value depending on MIDI message type
-            source (MidiIn): The [`MidiIn`][midiscripter.MidiIn] instance that generated the message
-        """
-        super().__init__(type, source)
-        self.channel = channel
-        self.data1 = data1
-        self.data2 = data2
-
-    @property
-    def combined_data(self) -> Union[int, tuple[int, ...]]:
-        """Both data bytes combined to 14-bit number:
-        pitch value for pitch bend MIDI message (0-16383)."""
-        return self.data1 | (self.data2 << 7)
-
-    @combined_data.setter
-    def combined_data(self, combined_data_value: Union[int, Sequence[int]]):
-        self.data1 = combined_data_value & 0x7f
-        self.data2 = combined_data_value >> 7
-
-
-class SysexMsg(MidiMsg):
-    """System exclusive MIDI message"""
-
-    type = MidiType.SYSEX
-    """MIDI message type."""
-
-    channel: Union[tuple[int], tuple[int, int, int]]
-    """Manufacturer ID (protocol)."""
-
-    data1: Union[tuple[int, int]]
-    """Sub ID (model, device, command, etc.)."""
-
-    data2: Union[tuple[int, ...]]
-    """Message data."""
-
-    def __new__(cls, *args, **kwargs):
-        return object.__new__(SysexMsg)
-
-    def __init__(self, combined_data: tuple[int, ...], *, source: Optional['MidiIn'] = None):
-        """
-        Args:
-            combined_data: Whole sysex message including opening (`240`) and closing (`247`) bytes
-            source (MidiIn): The [`MidiIn`][midiscripter.MidiIn] instance that generated the message
-        """
-        midiscripter.base.msg_base.Msg.__init__(self, MidiType.SYSEX, source)
-        self.combined_data = combined_data
-
-    def __eq__(self, other: MidiMsg):
-        return type(other) is SysexMsg and other.combined_data == self.combined_data
-
-    def __str__(self):
-        return f'{self.type} | {str(self.combined_data)[1:-1]}'
-    
-    def __repr__(self):
-        return f'{self.__class__.__name__}({str(self.combined_data)})'
-    
-    @property
-    def combined_data(self) -> tuple[int, ...]:
-        """Whole sysex message including opening (`240`) and closing (`247`) bytes."""
-        return (rtmidi.midiconstants.SYSTEM_EXCLUSIVE,
-                *self.channel, *self.data1, *self.data2,
-                rtmidi.midiconstants.END_OF_EXCLUSIVE)
-
-    @combined_data.setter
-    def combined_data(self, combined_data: Sequence[int]):
-        # combined_data[0] is sysex status byte
-        if combined_data[1] == 0:
-            manufacturer_id_end_index = 4
-        else:
-            manufacturer_id_end_index = 2
-        sub_id = manufacturer_id_end_index + 2
-
-        self.channel = tuple(combined_data[1:manufacturer_id_end_index])
-        self.data1 = tuple(combined_data[manufacturer_id_end_index:sub_id])
-        self.data2 = tuple(combined_data[sub_id:-1])  # sysex end byte excluded
+from typing import Sequence, Optional, Union, TYPE_CHECKING
+
+import rtmidi.midiconstants
+
+import midiscripter.base.msg_base
+
+if TYPE_CHECKING:
+    import midiscripter.base.port_base
+    from midiscripter.midi.midi_port import MidiIn
+
+
+class MidiType(midiscripter.base.msg_base.AttrEnum):
+    """MIDI message type enumerator to use as [`MidiMsg`][midiscripter.MidiMsg] `type` attribute."""
+    NOTE_ON = 'NOTE_ON'
+    NOTE_OFF = 'NOTE_OFF'
+    POLYTOUCH = 'POLYTOUCH'
+    AFTERTOUCH = 'AFTERTOUCH'
+    CONTROL_CHANGE = 'CONTROL_CHANGE'
+    PROGRAM_CHANGE = 'PROGRAM_CHANGE'
+    PITCH_BEND = 'PITCH_BEND'
+    SYSEX = 'SYSEX'
+
+
+class MidiMsg(midiscripter.base.msg_base.Msg):
+    """The base class for MIDI message that sets the common attributes
+    for [`ChannelMsg`][midiscripter.ChannelMsg] and [`SysexMsg`][midiscripter.SysexMsg].
+
+    `MidiMsg` class will produce [`ChannelMsg`][midiscripter.ChannelMsg]
+    or [`SysexMsg`][midiscripter.SysexMsg] objects depending on init arguments.
+
+    It is advised to use [`ChannelMsg`][midiscripter.ChannelMsg] 
+    or [`SysexMsg`][midiscripter.SysexMsg] classes 
+    to create MIDI messages in calls for clarity.
+    """
+    __match_args__: tuple[str] = ('type', 'channel', 'data1', 'data2')
+
+    type: MidiType
+    channel: Union[int, tuple[int], tuple[int, int, int]]
+    data1: Union[int, tuple[int, int]]
+    data2: Union[int, tuple[int, ...]]
+    combined_data: Union[int, tuple[int, ...]]
+    source: Optional['MidiIn']
+
+    def __new__(cls, *args, **kwargs):
+        if args and isinstance(args[0], tuple) or not args and 'combined_data' in kwargs:
+            return SysexMsg.__new__(SysexMsg, *args, **kwargs)
+        else:
+            return ChannelMsg.__new__(ChannelMsg, *args, **kwargs)
+
+    def matches(self, type=None, channel=None, data1=None, data2=None) -> bool:
+        return super(MidiMsg, self).matches(type, channel, data1, data2)
+
+
+class ChannelMsg(MidiMsg):
+    """Channel voice/mode MIDI message. The most common MIDI message."""
+
+    type: MidiType
+    """MIDI message type."""
+
+    channel: int
+    """MIDI message channel (1-16)."""
+
+    data1: int
+    """First data byte: note, control, program or aftertouch value 
+    depending on MIDI message type (0-127)."""
+
+    data2: int
+    """Second data byte: velocity, value depending on MIDI message type (0-127)."""
+
+    def __new__(cls, *args, **kwargs):
+        """Resets base class custom __new__"""
+        return object.__new__(ChannelMsg)
+
+    def __init__(self, type: MidiType = MidiType.CONTROL_CHANGE, 
+                 channel: int = 1, data1: int = 0, data2: int = 127,
+                 *, source: Optional['MidiIn'] = None):
+        """
+        Args:
+            type: MIDI message type.
+            channel: MIDI message channel
+            data1: First data byte: note, control, program or aftertouch value
+            depending on MIDI message type
+            data2: Second data byte: velocity, value depending on MIDI message type
+            source (MidiIn): The [`MidiIn`][midiscripter.MidiIn] instance that generated the message
+        """
+        super().__init__(type, source)
+        self.channel = channel
+        self.data1 = data1
+        self.data2 = data2
+
+    @property
+    def combined_data(self) -> Union[int, tuple[int, ...]]:
+        """Both data bytes combined to 14-bit number:
+        pitch value for pitch bend MIDI message (0-16383)."""
+        return self.data1 | (self.data2 << 7)
+
+    @combined_data.setter
+    def combined_data(self, combined_data_value: Union[int, Sequence[int]]):
+        self.data1 = combined_data_value & 0x7f
+        self.data2 = combined_data_value >> 7
+
+
+class SysexMsg(MidiMsg):
+    """System exclusive MIDI message"""
+
+    type = MidiType.SYSEX
+    """MIDI message type."""
+
+    channel: Union[tuple[int], tuple[int, int, int]]
+    """Manufacturer ID (protocol)."""
+
+    data1: Union[tuple[int, int]]
+    """Sub ID (model, device, command, etc.)."""
+
+    data2: Union[tuple[int, ...]]
+    """Message data."""
+
+    def __new__(cls, *args, **kwargs):
+        return object.__new__(SysexMsg)
+
+    def __init__(self, combined_data: tuple[int, ...], *, source: Optional['MidiIn'] = None):
+        """
+        Args:
+            combined_data: Whole sysex message including opening (`240`) and closing (`247`) bytes
+            source (MidiIn): The [`MidiIn`][midiscripter.MidiIn] instance that generated the message
+        """            
+        midiscripter.base.msg_base.Msg.__init__(self, MidiType.SYSEX, source)
+        self.combined_data = combined_data
+
+    def __eq__(self, other: MidiMsg):
+        return type(other) is SysexMsg and other.combined_data == self.combined_data
+
+    def __str__(self):
+        return f'{self.type} | {str(self.combined_data)[1:-1]}'
+    
+    def __repr__(self):
+        return f'{self.__class__.__name__}({str(self.combined_data)})'
+    
+    @property
+    def combined_data(self) -> tuple[int, ...]:
+        """Whole sysex message including opening (`240`) and closing (`247`) bytes."""
+        return (rtmidi.midiconstants.SYSTEM_EXCLUSIVE,
+                *self.channel, *self.data1, *self.data2,
+                rtmidi.midiconstants.END_OF_EXCLUSIVE)
+
+    @combined_data.setter
+    def combined_data(self, combined_data: Sequence[int]):
+        if (combined_data[0] != rtmidi.midiconstants.SYSTEM_EXCLUSIVE 
+            or combined_data[-1] != rtmidi.midiconstants.END_OF_EXCLUSIVE):
+            raise AttributeError('Sysex message should start with 240 (0xF0) and end with 247 (0xF7)')
+        
+        # combined_data[0] is sysex status byte
+        if combined_data[1] == 0:
+            sub_id_start_index = 4
+        else:
+            sub_id_start_index = 2
+        
+        data_start_index = sub_id_start_index + 2
+        
+        manufacturer = tuple(combined_data[1:sub_id_start_index])
+        
+        if len(combined_data) < data_start_index + 1:  # +1 for closing 247 byte 
+            raise AttributeError(
+                f'Sysex message for manufacturer {manufacturer} '
+                f'should be at least {data_start_index + 1} ints '
+                f'starting with 240 and ending with 247')
+        
+        self.channel = manufacturer
+        self.data1 = tuple(combined_data[sub_id_start_index:data_start_index])
+        self.data2 = tuple(combined_data[data_start_index:-1])  # sysex end byte excluded
```

### Comparing `midiscripter-0.1.1/midiscripter/midi/midi_port.py` & `midiscripter-0.1.2/midiscripter/midi/midi_port.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,173 +1,167 @@
-from typing import Union, Callable, Optional, TYPE_CHECKING
-
-import rtmidi
-import rtmidi.midiconstants
-
-import midiscripter.base.port_base
-from midiscripter.midi.midi_msg import MidiType
-from midiscripter.logger import log
-
-if TYPE_CHECKING:
-    from midiscripter.midi.midi_msg import MidiMsg
-
-
-BYTE_TO_TYPE_MAP = {rtmidi.midiconstants.NOTE_ON: MidiType.NOTE_ON,
-                    rtmidi.midiconstants.NOTE_OFF: MidiType.NOTE_OFF,
-                    rtmidi.midiconstants.PITCH_BEND: MidiType.PITCH_BEND,
-                    rtmidi.midiconstants.PROGRAM_CHANGE: MidiType.PROGRAM_CHANGE,
-                    rtmidi.midiconstants.CONTROLLER_CHANGE: MidiType.CONTROL_CHANGE,
-                    rtmidi.midiconstants.POLY_PRESSURE: MidiType.POLYTOUCH,
-                    rtmidi.midiconstants.CHANNEL_PRESSURE: MidiType.AFTERTOUCH}
-
-TYPE_TO_BYTE_MAP = {type_: byte_ for byte_, type_ in BYTE_TO_TYPE_MAP.items()}
-
-TYPE_TO_DATA_BYTES_COUNT = {MidiType.NOTE_ON: 3, MidiType.NOTE_OFF: 3,
-                            MidiType.CONTROL_CHANGE: 3,
-                            MidiType.POLYTOUCH: 3, MidiType.PITCH_BEND: 3,
-                            MidiType.AFTERTOUCH: 2, MidiType.PROGRAM_CHANGE: 2}
-
-
-class _MidiPortMixin(midiscripter.base.port_base.Port):
-    # Attrs provided by the class that inherits from MidiPortMixin
-    is_enabled: bool
-    _available_names: list[str]
-
-    # noinspection PyMissingConstructor
-    def __init__(self, port_name: str, input_callback: Optional[Callable] = None):
-        self._port_name = port_name
-
-        if input_callback:
-            self._rtmidi_port = rtmidi.MidiIn()
-            self._rtmidi_port.ignore_types(sysex=False)
-            self._rtmidi_port.set_callback(input_callback)
-            self._log_tag = 'input'
-        else:
-            self._rtmidi_port = rtmidi.MidiOut()
-            self._log_tag = 'output'
-
-    @property
-    def _is_available(self) -> bool:
-        """Port is available and can be opened."""
-        return self._port_name in self._available_names
-
-    def _open(self):
-        if self._rtmidi_port.is_port_open():
-            return
-
-        try:
-            port_index = self._available_names.index(self._port_name)
-            self._rtmidi_port.open_port(port_index)
-            self.is_enabled = True
-            log(f'Opened {self._log_tag} port {{{self._log_tag}}}',
-                **{self._log_tag: self})
-        except ValueError:
-            log.red(f'Can\'t find port {self._log_tag} port {{{self._log_tag}}}. '
-                    f'Check the port name.',
-                    **{self._log_tag: self})
-        except Exception:
-            log.red(f'Failed to open {self._log_tag} port {{{self._log_tag}}}',
-                    **{self._log_tag: self})
-
-    def _close(self):
-        if not self._rtmidi_port.is_port_open():
-            return
-
-        try:
-            self._rtmidi_port.close_port()
-            self._rtmidi_port.delete()
-            self.is_enabled = False
-            log(f'Closed {self._log_tag} port {{{self._log_tag}}}', **{self._log_tag: self})
-        except Exception:
-            log.red(f'Failed to close {self._log_tag} port {{{self._log_tag}}}')
-
-
-class MidiIn(_MidiPortMixin, midiscripter.base.port_base.Input):
-    """MIDI input port. Produces [`MidiMsg`][midiscripter.MidiMsg] objects."""
-    _available_names: list[str] = [port_name[:port_name.rfind(' ')]
-                                   for port_name in rtmidi.MidiIn().get_ports()]
-
-    def __init__(self, port_name: str):
-        """
-        Args:
-            port_name: MIDI input port name
-        """
-        _MidiPortMixin.__init__(self, port_name, self.__callback)
-        midiscripter.base.port_base.Input.__init__(self, port_name)
-
-        self.attached_passthrough_outs: list['MidiOut'] = []
-        """[`MidiOut`][midiscripter.MidiOut] ports attached as pass-through ports 
-        which will send all incoming messages as soon as they arrive before sending them to calls"""
-
-    def passthrough_out(self, midi_output: 'MidiOut'):
-        """Attach [`MidiOut`][midiscripter.MidiOut] as a pass-through port to send all incoming messages
-        as soon as they arrive, before sending them to calls. This can greatly reduce latency.
-
-        Args:
-            midi_output: [`MidiOut`][midiscripter.MidiOut] port to use for pass-through
-        """
-        if midi_output not in self.attached_passthrough_outs:
-            self.attached_passthrough_outs.append(midi_output)
-            log('{input} input will pass through {output}',
-                input= self, output=midi_output)
-
-    def __callback(self, rt_midi_input: tuple[tuple[hex, ...], float], _):
-        if not self.is_enabled:
-            return
-
-        rt_midi_data, _ = rt_midi_input
-        [output._passthrough_send(rt_midi_data) for output in self.attached_passthrough_outs]
-        self._send_input_msg_to_calls(self.__convert_to_msg(rt_midi_data))
-
-    def __convert_to_msg(self, rt_midi_data: tuple[hex, ...]) -> (
-            Union['midiscripter.midi.midi_msg.ChannelMsg', 'midiscripter.midi.midi_msg.SysexMsg']):
-
-        if (rt_midi_data[0] == rtmidi.midiconstants.SYSTEM_EXCLUSIVE and
-                rt_midi_data[-1] == rtmidi.midiconstants.END_OF_EXCLUSIVE):
-            return midiscripter.midi.midi_msg.SysexMsg(rt_midi_data, source=self)
-
-        elif rt_midi_data[0] < rtmidi.midiconstants.SYSTEM_EXCLUSIVE:
-            midi_type_byte = rt_midi_data[0] & 0xF0
-            midi_type = BYTE_TO_TYPE_MAP[midi_type_byte]
-            channel = (rt_midi_data[0] & 0xF) + 1
-
-            msg_atts = (midi_type, channel, *rt_midi_data[1:])
-            return midiscripter.midi.midi_msg.ChannelMsg(*msg_atts, source=self)
-
-        else:
-            log.red(f'Unsupported MIDI msg type byte: {rt_midi_data[0]}')
-
-
-class MidiOut(_MidiPortMixin, midiscripter.base.port_base.Output):
-    """MIDI output port. Sends [`MidiMsg`][midiscripter.MidiMsg] objects."""
-    _available_names: list[str] = [port_name[:port_name.rfind(' ')]
-                                   for port_name in rtmidi.MidiOut().get_ports()]
-
-    def __init__(self, port_name: str):
-        """
-        Args:
-            port_name: MIDI output port name
-        """
-        _MidiPortMixin.__init__(self, port_name)
-        midiscripter.base.port_base.Output.__init__(self, port_name)
-
-    def send(self, msg: 'MidiMsg') -> None:
-        """Send the MIDI message.
-
-        Args:
-            msg: object to send
-        """        
-        with self._check_and_log_sent_message(msg):
-            if msg.type == MidiType.SYSEX:
-                rt_midi_output = msg.combined_data  # FIXME Sequence have no attrs
-            else:
-                status_byte = (TYPE_TO_BYTE_MAP[msg.type] & 0xF0) | (msg.channel - 1 & 0xF)
-                rt_midi_output = [status_byte, msg.data1, msg.data2][:TYPE_TO_DATA_BYTES_COUNT[msg.type]]
-    
-            self._rtmidi_port.send_message(rt_midi_output)
-
-    def _passthrough_send(self, rt_midi_data: tuple[hex, hex, hex]):
-        if self.is_enabled:
-            try:
-                self._rtmidi_port.send_message(rt_midi_data)
-            except Exception:  # _rtmidi.SystemError: MidiOutWinMM::sendMessage: error sending MIDI message.
-                log.red(f'Failed to send message data: {rt_midi_data}')
+from typing import Union, Callable, Optional, TYPE_CHECKING
+
+import rtmidi
+import rtmidi.midiconstants
+
+import midiscripter.base.port_base
+from midiscripter.midi.midi_msg import MidiType
+from midiscripter.logger import log
+
+if TYPE_CHECKING:
+    from midiscripter.midi.midi_msg import MidiMsg
+
+
+BYTE_TO_TYPE_MAP = {rtmidi.midiconstants.NOTE_ON: MidiType.NOTE_ON,
+                    rtmidi.midiconstants.NOTE_OFF: MidiType.NOTE_OFF,
+                    rtmidi.midiconstants.PITCH_BEND: MidiType.PITCH_BEND,
+                    rtmidi.midiconstants.PROGRAM_CHANGE: MidiType.PROGRAM_CHANGE,
+                    rtmidi.midiconstants.CONTROLLER_CHANGE: MidiType.CONTROL_CHANGE,
+                    rtmidi.midiconstants.POLY_PRESSURE: MidiType.POLYTOUCH,
+                    rtmidi.midiconstants.CHANNEL_PRESSURE: MidiType.AFTERTOUCH}
+
+TYPE_TO_BYTE_MAP = {type_: byte_ for byte_, type_ in BYTE_TO_TYPE_MAP.items()}
+
+TYPE_TO_DATA_BYTES_COUNT = {MidiType.NOTE_ON: 3, MidiType.NOTE_OFF: 3,
+                            MidiType.CONTROL_CHANGE: 3,
+                            MidiType.POLYTOUCH: 3, MidiType.PITCH_BEND: 3,
+                            MidiType.AFTERTOUCH: 2, MidiType.PROGRAM_CHANGE: 2}
+
+
+class _MidiPortMixin(midiscripter.base.port_base.Port):
+    # Attrs provided by the class that inherits from MidiPortMixin
+    is_enabled: bool
+    _available_names: list[str]
+
+    # noinspection PyMissingConstructor
+    def __init__(self, port_name: str, input_callback: Optional[Callable] = None):
+        self.__port_name = port_name
+
+        if input_callback:
+            self.__rtmidi_port = rtmidi.MidiIn()
+            self.__rtmidi_port.ignore_types(sysex=False)
+            self.__rtmidi_port.set_callback(input_callback)
+        else:
+            self.__rtmidi_port = rtmidi.MidiOut()
+
+    @property
+    def _is_available(self) -> bool:
+        """Port is available and can be opened."""
+        return self.__port_name in self._available_names
+
+    def _open(self):
+        if self.__rtmidi_port.is_port_open():
+            return
+
+        try:
+            port_index = self._available_names.index(self.__port_name)
+            self.__rtmidi_port.open_port(port_index)
+            self.is_enabled = True
+            log('Opened {port}', port=self)
+        except ValueError:
+            log.red('Can\'t find port {port}. Check the port name.', port=self)
+        except Exception:
+            log.red('Failed to open {port}', port=self)
+
+    def _close(self):
+        if not self.__rtmidi_port.is_port_open():
+            return
+
+        try:
+            self.__rtmidi_port.close_port()
+            self.__rtmidi_port.delete()
+            self.is_enabled = False
+            log('Closed {port}', port=self)
+        except Exception:
+            log.red('Failed to close {port}', port=self)
+
+
+class MidiIn(_MidiPortMixin, midiscripter.base.port_base.Input):
+    """MIDI input port. Produces [`MidiMsg`][midiscripter.MidiMsg] objects."""
+    _available_names: list[str] = [port_name[:port_name.rfind(' ')]
+                                   for port_name in rtmidi.MidiIn().get_ports()]
+
+    def __init__(self, port_name: str):
+        """
+        Args:
+            port_name: MIDI input port name
+        """
+        _MidiPortMixin.__init__(self, port_name, self.__callback)
+        midiscripter.base.port_base.Input.__init__(self, port_name)
+
+        self.attached_passthrough_outs: list['MidiOut'] = []
+        """[`MidiOut`][midiscripter.MidiOut] ports attached as pass-through ports 
+        which will send all incoming messages as soon as they arrive before sending them to calls"""
+
+    def passthrough_out(self, midi_output: 'MidiOut'):
+        """Attach [`MidiOut`][midiscripter.MidiOut] as a pass-through port to send all incoming messages
+        as soon as they arrive, before sending them to calls. This can greatly reduce latency.
+
+        Args:
+            midi_output: [`MidiOut`][midiscripter.MidiOut] port to use for pass-through
+        """
+        if midi_output not in self.attached_passthrough_outs:
+            self.attached_passthrough_outs.append(midi_output)
+            log('{input} input will pass through {output}',
+                input=self, output=midi_output)
+
+    def __callback(self, rt_midi_input: tuple[tuple[hex, ...], float], _):
+        if not self.is_enabled:
+            return
+
+        rt_midi_data, _ = rt_midi_input
+        [output._passthrough_send(rt_midi_data) for output in self.attached_passthrough_outs]
+        self._send_input_msg_to_calls(self.__convert_to_msg(rt_midi_data))
+
+    def __convert_to_msg(self, rt_midi_data: tuple[hex, ...]) -> (
+            Union['midiscripter.midi.midi_msg.ChannelMsg', 'midiscripter.midi.midi_msg.SysexMsg']):
+
+        if (rt_midi_data[0] == rtmidi.midiconstants.SYSTEM_EXCLUSIVE and
+                rt_midi_data[-1] == rtmidi.midiconstants.END_OF_EXCLUSIVE):
+            return midiscripter.midi.midi_msg.SysexMsg(rt_midi_data, source=self)
+
+        elif rt_midi_data[0] < rtmidi.midiconstants.SYSTEM_EXCLUSIVE:
+            midi_type_byte = rt_midi_data[0] & 0xF0
+            midi_type = BYTE_TO_TYPE_MAP[midi_type_byte]
+            channel = (rt_midi_data[0] & 0xF) + 1
+
+            msg_atts = (midi_type, channel, *rt_midi_data[1:])
+            return midiscripter.midi.midi_msg.ChannelMsg(*msg_atts, source=self)
+
+        else:
+            log.red(f'Unsupported MIDI msg type byte: {rt_midi_data[0]}')
+
+
+class MidiOut(_MidiPortMixin, midiscripter.base.port_base.Output):
+    """MIDI output port. Sends [`MidiMsg`][midiscripter.MidiMsg] objects."""
+    _available_names: list[str] = [port_name[:port_name.rfind(' ')]
+                                   for port_name in rtmidi.MidiOut().get_ports()]
+
+    def __init__(self, port_name: str):
+        """
+        Args:
+            port_name: MIDI output port name
+        """
+        _MidiPortMixin.__init__(self, port_name)
+        midiscripter.base.port_base.Output.__init__(self, port_name)
+
+    def send(self, msg: 'MidiMsg') -> None:
+        """Send the MIDI message.
+
+        Args:
+            msg: object to send
+        """        
+        with self._check_and_log_sent_message(msg):
+            if msg.type == MidiType.SYSEX:
+                rt_midi_output = msg.combined_data
+            else:
+                status_byte = (TYPE_TO_BYTE_MAP[msg.type] & 0xF0) | (msg.channel - 1 & 0xF)
+                rt_midi_output = [status_byte, msg.data1, msg.data2][:TYPE_TO_DATA_BYTES_COUNT[msg.type]]
+    
+            self.__rtmidi_port.send_message(rt_midi_output)
+
+    def _passthrough_send(self, rt_midi_data: tuple[hex, hex, hex]):
+        if self.is_enabled:
+            try:
+                self.__rtmidi_port.send_message(rt_midi_data)
+            except Exception:  # _rtmidi.SystemError: MidiOutWinMM::sendMessage: error sending MIDI message.
+                log.red(f'Failed to send message data: {rt_midi_data}')
```

### Comparing `midiscripter-0.1.1/midiscripter/midi/midi_ports_update.py` & `midiscripter-0.1.2/midiscripter/midi/midi_ports_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import time
-
-import rtmidi
-
-import midiscripter.base.shared
-import midiscripter.base.port_base
-import midiscripter.base.msg_base
-import midiscripter.logger
-
-
-class MidiPortsChangedIn(midiscripter.base.port_base.Input):
-    """MIDI ports change watcher. Produces [`Msg`][midiscripter.base.msg_base.Msg] objects
-    with `MIDI Ports Changed` as `type` on any MIDI port connection or disconnection.
-
-    Used as a service port for `Restart on new MIDI port found` GUI option.
-
-    Notes:
-        Can be used to restart CLI scripts on ports change by:
-        `MidiPortsChangedIn().subscribe(restart_script)`.
-    """
-
-    REFRESH_RATE_SEC = 1
-    """MIDI ports polling rate."""
-    
-    _force_uid = 'MIDI Ports Change'
-    
-    def __init__(self):
-        super().__init__(self._force_uid)
-        self.__dummy_midi_input = rtmidi.MidiIn()
-        self.__dummy_midi_output = rtmidi.MidiOut()
-
-        self.__last_check_inputs = self.__dummy_midi_input.get_ports()
-        self.__last_check_outputs = self.__dummy_midi_output.get_ports()
-
-    def _open(self) -> None:
-        self.is_enabled = True
-        midiscripter.base.shared.thread_executor.submit(self.updater_worker)
-        midiscripter.logger.log(f'Started MIDI ports change watcher')
-
-    def _close(self) -> None:
-        self.is_enabled = False
-
-    def updater_worker(self):
-        while self.is_enabled:
-            time.sleep(self.REFRESH_RATE_SEC)
-
-            current_inputs = self.__dummy_midi_input.get_ports()
-            current_outputs = self.__dummy_midi_output.get_ports()
-
-            if (self.__last_check_inputs != current_inputs
-                    or self.__last_check_outputs != current_outputs):
-                self.__last_check_inputs = current_inputs
-                self.__last_check_outputs = current_outputs
-                self._send_input_msg_to_calls(midiscripter.base.msg_base.Msg('MIDI Ports Changed'))
+import time
+
+import rtmidi
+
+import midiscripter.base.shared
+import midiscripter.base.port_base
+import midiscripter.base.msg_base
+import midiscripter.logger
+
+
+class MidiPortsChangedIn(midiscripter.base.port_base.Input):
+    """MIDI ports change watcher. Produces [`Msg`][midiscripter.base.msg_base.Msg] objects
+    with `MIDI Ports Changed` as `type` on any MIDI port connection or disconnection.
+
+    Used as a service port for `Restart on new MIDI port found` GUI option.
+
+    Notes:
+        Can be used to restart CLI scripts on ports change by:
+        `MidiPortsChangedIn().subscribe(restart_script)`.
+    """
+
+    REFRESH_RATE_SEC = 1
+    """MIDI ports polling rate."""
+    
+    _force_uid = 'MIDI Ports Change'
+    
+    def __init__(self):
+        super().__init__(self._force_uid)
+        self.__dummy_midi_input = rtmidi.MidiIn()
+        self.__dummy_midi_output = rtmidi.MidiOut()
+
+        self.__last_check_inputs = self.__dummy_midi_input.get_ports()
+        self.__last_check_outputs = self.__dummy_midi_output.get_ports()
+
+    def _open(self) -> None:
+        self.is_enabled = True
+        midiscripter.base.shared.thread_executor.submit(self.__updater_worker)
+        midiscripter.logger.log(f'Started MIDI ports change watcher')
+
+    def _close(self) -> None:
+        self.is_enabled = False
+
+    def __updater_worker(self):
+        while self.is_enabled:
+            time.sleep(self.REFRESH_RATE_SEC)
+
+            current_inputs = self.__dummy_midi_input.get_ports()
+            current_outputs = self.__dummy_midi_output.get_ports()
+
+            if (self.__last_check_inputs != current_inputs
+                    or self.__last_check_outputs != current_outputs):
+                self.__last_check_inputs = current_inputs
+                self.__last_check_outputs = current_outputs
+                self._send_input_msg_to_calls(midiscripter.base.msg_base.Msg('MIDI Ports Changed'))
```

### Comparing `midiscripter-0.1.1/midiscripter/osc/osc_msg.py` & `midiscripter-0.1.2/midiscripter/osc/osc_msg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from typing import TYPE_CHECKING, Union
-
-import midiscripter.base.msg_base
-
-if TYPE_CHECKING:
-    from midiscripter.osc.osc_port import OscIn
-
-
-class OscMsg(midiscripter.base.msg_base.Msg):
-    """Open Sound Control message"""
-    
-    __match_args__ = ('type', 'address', 'data')
-    type: str = 'OSC'
-    
-    address: str
-    """Message address"""
-    
-    data: Union[str, bytes, bool, int, float, list, tuple]
-    """Message data"""
-
-    def __init__(self, address: str,
-                 data: Union[str, bytes, bool, int, float, list, tuple] = None,
-                 *, source: 'OscIn' = None):
-        """
-        Args:
-            address: Open Sound Control message address
-            data: Open Sound Control message data
-            source (OscIn): The [`OscIn`][midiscripter.OscIn] instance 
-                            that generated the message
-        """
-        super().__init__(self.type, source)
-        self.address = address
-        self.data = data
-    
-    def matches(self, address=None, data=None):
-        return super().matches(self.type, address, data)
+from typing import TYPE_CHECKING, Union, Optional
+
+import midiscripter.base.msg_base
+
+if TYPE_CHECKING:
+    from midiscripter.osc.osc_port import OscIn
+
+
+class OscMsg(midiscripter.base.msg_base.Msg):
+    """Open Sound Control message"""
+    
+    __match_args__ = ('type', 'address', 'data')
+    type: str = 'OSC'
+    
+    address: str
+    """Message address"""
+    
+    data: Union[str, bytes, bool, int, float, list, tuple]
+    """Message data"""
+
+    source: Optional['OscIn']
+
+    def __init__(self, address: str,
+                 data: Union[str, bytes, bool, int, float, list, tuple] = None,
+                 *, source: Optional['OscIn'] = None):
+        """
+        Args:
+            address: Open Sound Control message address
+            data: Open Sound Control message data
+            source (OscIn): The [`OscIn`][midiscripter.OscIn] instance 
+                            that generated the message
+        """
+        super().__init__(self.type, source)
+        self.address = address
+        self.data = data
+    
+    def matches(self, address=None, data=None):
+        return super().matches(self.type, address, data)
```

### Comparing `midiscripter-0.1.1/midiscripter/osc/osc_port.py` & `midiscripter-0.1.2/midiscripter/osc/osc_port.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from typing import Union
-
-import pythonosc.osc_server
-import pythonosc.udp_client
-
-import midiscripter.base.port_base
-import midiscripter.base.shared
-import midiscripter.osc.osc_msg
-from midiscripter.logger import log
-from midiscripter.osc.osc_msg import OscMsg
-
-
-def _parse_ip_port(ip_port: Union[str, int]) -> (str, int):
-    """ Parses 'ip:port' or local port to get ip and port
-
-    Args:
-        ip_port: 'ip:port' or local port
-    Returns:
-        ip, port number
-    """
-    if isinstance(ip_port, int) or ip_port.isdigit():
-        ip_address = '127.0.0.1'
-        port = int(ip_port)
-    elif ':' in ip_port:
-        ip_address, port = ip_port.split(':')
-        port = int(port)
-    else:
-        raise AttributeError(f'Invalid OSC port address: {ip_port}')
-    
-    return ip_address, port
-
-
-class OscIn(midiscripter.base.port_base.Input):
-    """Open Sound Control input port. Produces [`OscMsg`][midiscripter.OscMsg] objects."""
-
-    def __init__(self, listener_ip_port: Union[str, int]):
-        """
-            Args:
-                listener_ip_port: 'ip:port' or local port to listen for incoming OSC messages
-        """
-        super().__init__(listener_ip_port)
-        self.listener_ip_address, self.listener_port = _parse_ip_port(listener_ip_port)
-        self.__dispatcher = None
-    
-    def __osc_server_msg_handler(self, address: str, *data):
-        if not self.is_enabled:
-            return 
-        
-        if len(data) == 1:
-            data = data[0]
-        input_msg = OscMsg(address, data, source=self)
-        self._send_input_msg_to_calls(input_msg)
-    
-    def _open(self):
-        if self.__dispatcher:
-            return 
-            
-        self.__dispatcher = pythonosc.osc_server.Dispatcher()
-        self.__dispatcher.set_default_handler(self.__osc_server_msg_handler)
-        self._osc_server = pythonosc.osc_server.BlockingOSCUDPServer(
-            (self.listener_ip_address, self.listener_port), self.__dispatcher)
-        
-        midiscripter.base.shared.thread_executor.submit(self._osc_server.serve_forever)
-        self.is_enabled = True
-        log('Opened {input}', input=self)
-
-    def _close(self):
-        self._osc_server.shutdown()
-        self.is_enabled = False
-        log('Stopped {input}', input=self)
-
-
-class OscOut(midiscripter.base.port_base.Output):
-    """Open Sound Control output port. Sends [`OscMsg`][midiscripter.OscMsg] objects."""
-    
-    def __init__(self, target_ip_port: Union[str, int]):
-        """
-            Args:
-                target_ip_port: 'ip:port' or local port to send output OSC messages to
-        """
-        super().__init__(target_ip_port)
-        target_ip_address, target_port = _parse_ip_port(target_ip_port)
-        self._osc_client = pythonosc.udp_client.SimpleUDPClient(target_ip_address, target_port)
-        self.is_enabled = True
-        
-    def send(self, msg: OscMsg):
-        """Send the OSC message
-
-        Args:
-            msg: object to send
-        """   
-        with self._check_and_log_sent_message(msg):
-            data = list(msg.data) if isinstance(msg.data, tuple) else msg.data
-            self._osc_client.send_message(msg.address, data)
+from typing import Union
+
+import pythonosc.osc_server
+import pythonosc.udp_client
+
+import midiscripter.base.port_base
+import midiscripter.base.shared
+import midiscripter.osc.osc_msg
+from midiscripter.logger import log
+from midiscripter.osc.osc_msg import OscMsg
+
+
+def _parse_ip_port(ip_port: Union[str, int]) -> (str, int):
+    """ Parses 'ip:port' or local port to get ip and port
+
+    Args:
+        ip_port: 'ip:port' or local port
+    Returns:
+        ip, port number
+    """
+    if isinstance(ip_port, int) or ip_port.isdigit():
+        ip_address = '127.0.0.1'
+        port = int(ip_port)
+    elif ':' in ip_port:
+        ip_address, port = ip_port.split(':')
+        port = int(port)
+    else:
+        raise AttributeError(f'Invalid OSC port address: {ip_port}')
+    
+    return ip_address, port
+
+
+class OscIn(midiscripter.base.port_base.Input):
+    """Open Sound Control input port. Produces [`OscMsg`][midiscripter.OscMsg] objects."""
+
+    def __init__(self, listener_ip_port: Union[str, int]):
+        """
+            Args:
+                listener_ip_port: 'ip:port' or local port to listen for incoming OSC messages
+        """
+        super().__init__(listener_ip_port)
+        self.listener_ip_address, self.listener_port = _parse_ip_port(listener_ip_port)
+        self.__dispatcher = None
+    
+    def __osc_server_msg_handler(self, address: str, *data):
+        if not self.is_enabled:
+            return 
+        
+        if len(data) == 1:
+            data = data[0]
+        input_msg = OscMsg(address, data, source=self)
+        self._send_input_msg_to_calls(input_msg)
+    
+    def _open(self):
+        if self.__dispatcher:
+            return 
+            
+        self.__dispatcher = pythonosc.osc_server.Dispatcher()
+        self.__dispatcher.set_default_handler(self.__osc_server_msg_handler)
+        self._osc_server = pythonosc.osc_server.BlockingOSCUDPServer(
+            (self.listener_ip_address, self.listener_port), self.__dispatcher)
+        
+        midiscripter.base.shared.thread_executor.submit(self._osc_server.serve_forever)
+        self.is_enabled = True
+        log('Opened {input}', input=self)
+
+    def _close(self):
+        self._osc_server.shutdown()
+        self.is_enabled = False
+        log('Stopped {input}', input=self)
+
+
+class OscOut(midiscripter.base.port_base.Output):
+    """Open Sound Control output port. Sends [`OscMsg`][midiscripter.OscMsg] objects."""
+    
+    def __init__(self, target_ip_port: Union[str, int]):
+        """
+            Args:
+                target_ip_port: 'ip:port' or local port to send output OSC messages to
+        """
+        super().__init__(target_ip_port)
+        target_ip_address, target_port = _parse_ip_port(target_ip_port)
+        self._osc_client = pythonosc.udp_client.SimpleUDPClient(target_ip_address, target_port)
+        self.is_enabled = True
+        
+    def send(self, msg: OscMsg):
+        """Send the OSC message
+
+        Args:
+            msg: object to send
+        """   
+        with self._check_and_log_sent_message(msg):
+            data = list(msg.data) if isinstance(msg.data, tuple) else msg.data
+            self._osc_client.send_message(msg.address, data)
```

### Comparing `midiscripter-0.1.1/midiscripter/osc/osc_query_maker.py` & `midiscripter-0.1.2/midiscripter/osc/osc_query_maker.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import queue
-from typing import Union
-
-from midiscripter.osc.osc_msg import OscMsg
-from midiscripter.osc.osc_port import OscIn, OscOut
-from midiscripter.logger import log
-
-
-class OscQueryMaker:
-    """The helper class to handle OSC request - response queries"""
-
-    def __init__(self, osc_in: OscIn, osc_out: OscOut):
-        """
-        Args:
-            osc_in: OscIn port for incoming responses
-            osc_out: OscOut port to send requests to
-        """
-        self.__osc_in = osc_in
-        self.__osc_out = osc_out
-        self.__query_register: dict[str, queue.SimpleQueue] = {}
-        osc_in.subscribe(self.__osc_query_maker_in)
-
-    def __osc_query_maker_in(self, msg: OscMsg):
-        try:
-            self.__query_register[msg.address].put(msg.data)
-        except KeyError:
-            pass
-
-    def query(self, address: str, timeout_sec: float = 2) -> Union[
-        str, bytes, bool, int, float, list, tuple]:
-        """Query data by sending the request to OSC address 
-           and returning the response from that address
-
-        Args:
-            address: OSC address to send request to
-            timeout_sec: time for response until raising TimeoutError
-
-        Returns:
-            Response OSC message data
-        """
-        result_queue = queue.SimpleQueue()
-        self.__query_register[address] = result_queue
-        log("Requesting '{address}' data from {input}", address=address, input=self.__osc_in)
-        self.__osc_out.send(OscMsg(address))
-        
-        try:
-            result = result_queue.get(timeout=timeout_sec)
-            self.__query_register.pop(address)
-            return result
-        except queue.Empty:
-            self.__query_register.pop(address)
-            raise TimeoutError from None
+import queue
+from typing import Union
+
+from midiscripter.osc.osc_msg import OscMsg
+from midiscripter.osc.osc_port import OscIn, OscOut
+from midiscripter.logger import log
+
+
+class OscQueryMaker:
+    """The helper class to handle OSC request - response queries"""
+
+    def __init__(self, osc_in: OscIn, osc_out: OscOut):
+        """
+        Args:
+            osc_in: OscIn port for incoming responses
+            osc_out: OscOut port to send requests to
+        """
+        self.__osc_in = osc_in
+        self.__osc_out = osc_out
+        self.__query_register: dict[str, queue.SimpleQueue] = {}
+        osc_in.subscribe(self.__osc_query_maker_in)
+
+    def __osc_query_maker_in(self, msg: OscMsg):
+        try:
+            self.__query_register[msg.address].put(msg.data)
+        except KeyError:
+            pass
+
+    def query(self, address: str, timeout_sec: float = 2) -> Union[
+        str, bytes, bool, int, float, list, tuple]:
+        """Query data by sending the request to OSC address 
+           and returning the response from that address
+
+        Args:
+            address: OSC address to send request to
+            timeout_sec: time for response until raising TimeoutError
+
+        Returns:
+            Response OSC message data
+        """
+        result_queue = queue.SimpleQueue()
+        self.__query_register[address] = result_queue
+        log("Requesting '{address}' data from {input}", address=address, input=self.__osc_in)
+        self.__osc_out.send(OscMsg(address))
+        
+        try:
+            result = result_queue.get(timeout=timeout_sec)
+            self.__query_register.pop(address)
+            return result
+        except queue.Empty:
+            self.__query_register.pop(address)
+            raise TimeoutError from None
```

### Comparing `midiscripter-0.1.1/midiscripter/resources/icon.ico` & `midiscripter-0.1.2/midiscripter/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.1/midiscripter/resources/icon.svg` & `midiscripter-0.1.2/midiscripter/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.1/README.md` & `midiscripter-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # MIDI Scripter
 
 MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound Control (OSC) input and output with a few lines of Python code.
 
-MIDI Scripter is intended for digital audio workstation (DAW) controls scripting. It fits where controller mappings are not enough but rewriting DAW controller integration is too much. 
+MIDI Scripter is intended for digital audio workstation (DAW) controls scripting but can also be used for general input conversion and automation. It fits where controller mappings are not enough but rewriting DAW controller integration is too much. 
 
-MIDI Scripter can also be used for general input conversion and automation.
-
-An octave transposer with GUI controls in 11 lines of code:
+An octave transposer with GUI controls in 10 lines of code:
 
 ``` python
 from midiscripter import *  # safe * import with no bloat
 
 midi_keyboard = MidiIn('Port name')  # GUI will provide you with port names
 proxy_output = MidiOut('loopMIDI Port') # using loopMIDI virtual port for output
 
@@ -23,15 +21,17 @@
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
 		proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
-![](/examples/octave_transposer/screenshot.png)
+![Screenshot](/examples/octave_transposer/screenshot.png)
+
+[Scripting guide and API documentation available](https://maboroshy.github.io/midi-scripter)
 
 Easy tasks for MIDI Scripter:  
 1. Filter, modify and route MIDI, OSC and keyboard messages in any way.  
 2. Map MIDI, OSC and keyboard to each other.  
 3. Map any Python code to input message.  
 4. Make extra "shift" keys to multiply MIDI controls.  
 5. Organize mappings into sets / scenes with GUI controls.  
@@ -43,21 +43,21 @@
 3. Make music education ot trainer GUI application based on MIDI input.
 
 Currently MIDI Scripter is at "beta" development stage. It's fully functional but needs some more testing. It targets only Windows for now but Linux and macOS support will follow.
 
 ## Installation
 1. [Python 3.11+](https://www.python.org/downloads/).
 2. [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) for virtual MIDI output ports on Windows.
-3. `pip3 install midiscripter` in console.
+3. `pip install midiscripter` in console.
 
 ## Setup
 Run loopMIDI and add virtual ports you want to send MIDI messages. You can enable its autostart option.
 
 Enable virtual MIDI output ports as MIDI inputs in DAW. 
 
 ## Quick Start
-1. Download [script template](examples/script_template.py) and open it in Python IDE or plain text editor.  
-2. Run unchanged template script to open GUI for more info on available MIDI ports and input.
+1. Paste [script template](examples/script_template.py) to Python IDE or plain text editor. IDE is greatly recommended.
+2. Run unchanged template script from IDE or by `python .\script_template.py` to open GUI for more info on available ports and their input.
 3. Turn on the ports' checkboxes to enable them and watch the log for input messages.
-4. Click on available ports names and messages to copy their declarations to the clipboard. Paste the declarations to your script.
+4. Click on port names and messages to copy their declarations to the clipboard. Paste the declarations to your script.
 5. Write the functions you need. Subscribe them to messages with `@input_port.subscribe` decorator. Use `log('messages')` for debugging. Use `output_port.send(msg)` to send modified or created messages from a function.
-6. Restart the script from GUI or enable TODO option.
+6. Restart the script from GUI.
```

### Comparing `midiscripter-0.1.1/pyproject.toml` & `midiscripter-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-[build-system]
-requires = ['hatchling']
-build-backend = 'hatchling.build'
-
-[project]
-name = 'midiscripter'
-version = '0.1.1'
-description = 'Framework for scripting MIDI, keyboard and Open Sound Control input and output'
-readme = 'README.md'
-requires-python = '>=3.11'
-license = {file = "LICENSE"}
-keywords = ['MIDI', 'OSC', 'scripting', 'automation', 'input']
-authors = [
-  {name = 'Maboroshy'},
-]
-classifiers = [
-  'Development Status :: 4 - Beta',
-  'Programming Language :: Python',
-  'Programming Language :: Python :: 3.11',
-  'Programming Language :: Python :: 3.12',
-  'Programming Language :: Python :: Implementation :: CPython',
-  'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-  'Operating System :: Microsoft :: Windows',
-  'Topic :: Multimedia :: Sound/Audio',
-  'Topic :: Multimedia :: Sound/Audio :: MIDI',
-  'Topic :: Software Development :: Libraries :: Python Modules',
-]
-dependencies = [ 
-  'colorama ~=0.4.6',
-  'python-rtmidi ~=1.5.0',
-  'python-osc ~=1.7.6',
-  'pynput ~=1.7.5',
-  'watchdog ~=4.0',
-  'PySide6 ~=6.4',
-]
-
-[tool.hatch.build.targets.sdist]
-only-include = ['midiscripter']
-
-#[tool.hatch.build.targets.wheel]
-#only-include = ['midiscripter']
-
-[project.urls]
-Documentation = 'https://github.com/Maboroshy/midi-scripter#readme'
-Issues = 'https://github.com/Maboroshy/midi-scripter/issues'
-Source = 'https://github.com/Maboroshy/midi-scripter'
+[build-system]
+requires = ['hatchling']
+build-backend = 'hatchling.build'
+
+[project]
+name = 'midiscripter'
+version = '0.1.2'
+description = 'Framework for scripting MIDI, keyboard and Open Sound Control input and output'
+readme = 'README.md'
+requires-python = '>=3.11'
+license = {file = "LICENSE"}
+keywords = ['MIDI', 'OSC', 'script', 'automation', 'input']
+authors = [
+  {name = 'Maboroshy'},
+]
+classifiers = [
+  'Development Status :: 4 - Beta',
+  'Programming Language :: Python',
+  'Programming Language :: Python :: 3.11',
+  'Programming Language :: Python :: 3.12',
+  'Programming Language :: Python :: Implementation :: CPython',
+  'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
+  'Operating System :: Microsoft :: Windows',
+  'Topic :: Multimedia :: Sound/Audio',
+  'Topic :: Multimedia :: Sound/Audio :: MIDI',
+  'Topic :: Software Development :: Libraries :: Python Modules',
+]
+dependencies = [
+  'colorama ~=0.4',  # BSD
+  'python-rtmidi ~=1.5',  # MIT
+  'python-osc ~=1.7',  # Unlicense
+  'pynput ~=1.7',  # LGPL
+  'watchdog ~=4.0',  # Apache
+  'PySide6-Essentials ~=6.4',  # LGPL
+]
+
+[project.optional-dependencies]
+doc = [
+  'mkdocs-material',
+  'griffe-inherited-docstrings',
+]
+
+[tool.hatch.build.targets.sdist]
+only-include = ['midiscripter']
+
+[project.gui-scripts]
+midiscripter = 'midiscripter:start_gui'
+
+[project.urls]
+Documentation = 'https://maboroshy.github.io/midi-scripter'
+Issues = 'https://github.com/Maboroshy/midi-scripter/issues'
+Source = 'https://github.com/Maboroshy/midi-scripter'
```

