# Comparing `tmp/ch9329-1.0.6.tar.gz` & `tmp/ch9329-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.0.6.tar", last modified: Fri Mar 22 07:06:09 2024, max compression
+gzip compressed data, was "ch9329-1.0.7.tar", last modified: Sun Apr 28 13:40:57 2024, max compression
```

## Comparing `ch9329-1.0.6.tar` & `ch9329-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:06:09.358806 ch9329-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-22 07:06:00.000000 ch9329-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 07:06:00.000000 ch9329-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-22 07:06:09.358806 ch9329-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-22 07:06:00.000000 ch9329-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:06:09.354806 ch9329-1.0.6/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-22 07:06:00.000000 ch9329-1.0.6/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 07:06:09.358806 ch9329-1.0.6/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-22 07:06:09.000000 ch9329-1.0.6/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-22 07:06:09.000000 ch9329-1.0.6/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 07:06:09.000000 ch9329-1.0.6/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 07:06:09.000000 ch9329-1.0.6/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 07:06:09.000000 ch9329-1.0.6/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-22 07:06:00.000000 ch9329-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 07:06:09.358806 ch9329-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:57.037489 ch9329-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 13:40:49.000000 ch9329-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 13:40:49.000000 ch9329-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-28 13:40:57.037489 ch9329-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-28 13:40:49.000000 ch9329-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:57.033489 ch9329-1.0.7/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:57.033489 ch9329-1.0.7/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 13:40:49.000000 ch9329-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:40:57.037489 ch9329-1.0.7/setup.cfg
```

### Comparing `ch9329-1.0.6/LICENSE` & `ch9329-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.6/PKG-INFO` & `ch9329-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.0.6/README.md` & `ch9329-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.6/ch9329/config.py` & `ch9329-1.0.7/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.6/ch9329/hid.py` & `ch9329-1.0.7/ch9329/hid.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,15 @@
     "ctrl_right": (HID_KEY_CONTROL_RIGHT, None),
     "shift": (HID_KEY_SHIFT_LEFT, None),
     "shift_left": (HID_KEY_SHIFT_LEFT, None),
     "shift_right": (HID_KEY_SHIFT_RIGHT, None),
     "alt": (HID_KEY_ALT_LEFT, None),
     "alt_left": (HID_KEY_ALT_LEFT, None),
     "alt_right": (HID_KEY_ALT_RIGHT, None),
+    "win": (HID_KEY_GUI_LEFT, None),
     "gui": (HID_KEY_GUI_LEFT, None),
     "gui_left": (HID_KEY_GUI_LEFT, None),
     "gui_right": (HID_KEY_GUI_RIGHT, None),
     # white spaces
     " ": (HID_KEY_SPACE, None),
     "\t": (HID_KEY_TAB, None),
     "\n": (HID_KEY_ENTER, None),
```

### Comparing `ch9329-1.0.6/ch9329/keyboard.py` & `ch9329-1.0.7/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.6/ch9329/mouse.py` & `ch9329-1.0.7/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.6/ch9329/utils.py` & `ch9329-1.0.7/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.6/ch9329.egg-info/PKG-INFO` & `ch9329-1.0.7/ch9329.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.0.6/pyproject.toml` & `ch9329-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.0.6"
+version = "1.0.7"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

