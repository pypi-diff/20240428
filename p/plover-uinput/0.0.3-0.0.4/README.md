# Comparing `tmp/plover-uinput-0.0.3.tar.gz` & `tmp/plover-uinput-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-uinput-0.0.3.tar", last modified: Sat Apr 13 13:56:26 2024, max compression
+gzip compressed data, was "plover-uinput-0.0.4.tar", last modified: Sun Apr 28 13:54:15 2024, max compression
```

## Comparing `plover-uinput-0.0.3.tar` & `plover-uinput-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/
--rw-r--r--   0 olai      (1000) users      (100)     1053 2024-04-11 16:08:24.000000 plover-uinput-0.0.3/LICENSE
--rw-r--r--   0 olai      (1000) users      (100)     2090 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/PKG-INFO
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-13 13:56:26.686653 plover-uinput-0.0.3/plover_uinput/
--rw-r--r--   0 olai      (1000) users      (100)     9283 2024-04-13 13:54:59.000000 plover-uinput-0.0.3/plover_uinput/__init__.py
--rw-r--r--   0 olai      (1000) users      (100)      130 2024-04-09 10:35:53.000000 plover-uinput-0.0.3/plover_uinput/all_keys.py
--rw-r--r--   0 olai      (1000) users      (100)    10000 2024-04-09 10:31:51.000000 plover-uinput-0.0.3/plover_uinput/keys.py
--rw-r--r--   0 olai      (1000) users      (100)     2019 2024-04-11 13:38:12.000000 plover-uinput-0.0.3/plover_uinput/symbols.py
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/plover_uinput.egg-info/
--rw-r--r--   0 olai      (1000) users      (100)     2090 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/PKG-INFO
--rw-r--r--   0 olai      (1000) users      (100)      374 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/SOURCES.txt
--rw-r--r--   0 olai      (1000) users      (100)        1 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/dependency_links.txt
--rw-r--r--   0 olai      (1000) users      (100)      119 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/entry_points.txt
--rw-r--r--   0 olai      (1000) users      (100)       45 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/requires.txt
--rw-r--r--   0 olai      (1000) users      (100)       14 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/top_level.txt
--rw-r--r--   0 olai      (1000) users      (100)       89 2024-04-11 16:18:33.000000 plover-uinput-0.0.3/pyproject.toml
--rw-r--r--   0 olai      (1000) users      (100)      625 2024-04-11 16:10:12.000000 plover-uinput-0.0.3/readme.md
--rw-r--r--   0 olai      (1000) users      (100)      670 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/setup.cfg
--rw-r--r--   0 olai      (1000) users      (100)       62 2024-04-09 17:27:40.000000 plover-uinput-0.0.3/setup.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/
+-rw-r--r--   0 olai      (1000) users      (100)     1053 2024-04-11 16:08:24.000000 plover-uinput-0.0.4/LICENSE
+-rw-r--r--   0 olai      (1000) users      (100)     2208 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/PKG-INFO
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-28 13:54:15.345328 plover-uinput-0.0.4/plover_uinput/
+-rw-r--r--   0 olai      (1000) users      (100)     9403 2024-04-28 13:53:32.000000 plover-uinput-0.0.4/plover_uinput/__init__.py
+-rw-r--r--   0 olai      (1000) users      (100)      130 2024-04-09 10:35:53.000000 plover-uinput-0.0.4/plover_uinput/all_keys.py
+-rw-r--r--   0 olai      (1000) users      (100)    10000 2024-04-09 10:31:51.000000 plover-uinput-0.0.4/plover_uinput/keys.py
+-rw-r--r--   0 olai      (1000) users      (100)     2019 2024-04-11 13:38:12.000000 plover-uinput-0.0.4/plover_uinput/symbols.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/plover_uinput.egg-info/
+-rw-r--r--   0 olai      (1000) users      (100)     2208 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/PKG-INFO
+-rw-r--r--   0 olai      (1000) users      (100)      374 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/SOURCES.txt
+-rw-r--r--   0 olai      (1000) users      (100)        1 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/dependency_links.txt
+-rw-r--r--   0 olai      (1000) users      (100)      119 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/entry_points.txt
+-rw-r--r--   0 olai      (1000) users      (100)       45 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/requires.txt
+-rw-r--r--   0 olai      (1000) users      (100)       14 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/top_level.txt
+-rw-r--r--   0 olai      (1000) users      (100)       89 2024-04-11 16:18:33.000000 plover-uinput-0.0.4/pyproject.toml
+-rw-r--r--   0 olai      (1000) users      (100)      743 2024-04-16 14:42:09.000000 plover-uinput-0.0.4/readme.md
+-rw-r--r--   0 olai      (1000) users      (100)      670 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/setup.cfg
+-rw-r--r--   0 olai      (1000) users      (100)       62 2024-04-09 17:27:40.000000 plover-uinput-0.0.4/setup.py
```

### Comparing `plover-uinput-0.0.3/LICENSE` & `plover-uinput-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.3/PKG-INFO` & `plover-uinput-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover>=4.0.0rc2
 Requires-Dist: evdev>=1.7.0
 Requires-Dist: xkbcommon>=0.8
 
 # Plover output plugin for linux using uinput
 
+If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)!
+
 ## Setup
 Add your user to the `input` group, and add this `udev` rule:
 ```
 KERNEL=="uinput", GROUP="input", MODE="0660", OPTIONS+="static_node=uinput"
 ```
 Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`.
```

### Comparing `plover-uinput-0.0.3/plover_uinput/__init__.py` & `plover-uinput-0.0.4/plover_uinput/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,50 +222,54 @@
     def set_key_press_delay(self, ms):
         if self._ms != ms:
             self._ms = ms
             self._delay = self._ms / 1000
 
     def _press_key(self, key, state):
         self._ui.write(e.EV_KEY, key, 1 if state else 0)
+        self._ui.syn()
 
     def _send_key(self, key):
         self._press_key(key, True)
         self._press_key(key, False)
+        self._ui.syn()
 
     # Send unicode character (through iBus)
     def _send_unicode(self, hex):
         self._press_key(modifiers["control_l"], True)
         self._press_key(modifiers["shift_l"], False)
+        sleep(self._delay)
         self._send_key(keys["u"])
+        sleep(self._delay)
         self._press_key(modifiers["control_l"], False)
         self._press_key(modifiers["shift_l"], False)
-        self._ui.syn()
+        sleep(self._delay)
         self._send_string(hex)
         self._send_key(keys["\n"])
-        self._ui.syn()
 
     def _send_char(self, char):
         # === Key can be sent with a key combination ===
         if char in self._symbols:
             (base, mods) = self._symbols[char]
             for mod in mods.split():
                 self._press_key(modifiers[mods], True)
+            sleep(self._delay)
             self._send_key(keys[base])
             for mod in mods.split():
                 self._press_key(modifiers[mods], False)
+            sleep(self._delay)
         # === Key can not be typed - send unicode symbol ===
         # It would be better if it was possible to modify the layout to a custom one
         # including all the needed symbols
         else:
             # Convert to hex and remove leading "0x"
             unicode_hex = hex(ord(char))[2:]
             self._send_unicode(unicode_hex)
 
         # === Delay before next ===
-        self._ui.syn()
         sleep(self._delay)
 
     def send_string(self, string):
         # key_presses = [keys[i] for i in list(string)]
         # for key in key_presses:
         for key in list(string):
             self._send_char(key)
```

### Comparing `plover-uinput-0.0.3/plover_uinput/keys.py` & `plover-uinput-0.0.4/plover_uinput/keys.py`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.3/plover_uinput/symbols.py` & `plover-uinput-0.0.4/plover_uinput/symbols.py`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.3/plover_uinput.egg-info/PKG-INFO` & `plover-uinput-0.0.4/plover_uinput.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover>=4.0.0rc2
 Requires-Dist: evdev>=1.7.0
 Requires-Dist: xkbcommon>=0.8
 
 # Plover output plugin for linux using uinput
 
+If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)!
+
 ## Setup
 Add your user to the `input` group, and add this `udev` rule:
 ```
 KERNEL=="uinput", GROUP="input", MODE="0660", OPTIONS+="static_node=uinput"
 ```
 Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`.
```

### Comparing `plover-uinput-0.0.3/setup.cfg` & `plover-uinput-0.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-uinput
-version = 0.0.3
+version = 0.0.4
 author = LilleAila
 description = Plover output plugin for linux using evdev / uinput
 long_description = file: readme.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/LilleAila/plover-uinput
 keywords = plover plover_plugin
```

