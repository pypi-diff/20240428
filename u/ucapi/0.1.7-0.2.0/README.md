# Comparing `tmp/ucapi-0.1.7.tar.gz` & `tmp/ucapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucapi-0.1.7.tar", last modified: Wed Mar 13 15:56:32 2024, max compression
+gzip compressed data, was "ucapi-0.2.0.tar", last modified: Sun Apr 28 20:52:11 2024, max compression
```

## Comparing `ucapi-0.1.7.tar` & `ucapi-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:56:32.821004 ucapi-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-13 15:56:27.000000 ucapi-0.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-13 15:56:27.000000 ucapi-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-13 15:56:27.000000 ucapi-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-13 15:56:32.821004 ucapi-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-13 15:56:27.000000 ucapi-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:56:32.817003 ucapi-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-13 15:56:27.000000 ucapi-0.1.7/docs/code_guidelines.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-13 15:56:27.000000 ucapi-0.1.7/docs/setup.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:56:32.817003 ucapi-0.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-13 15:56:27.000000 ucapi-0.1.7/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-13 15:56:27.000000 ucapi-0.1.7/examples/hello_integration.json
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-13 15:56:27.000000 ucapi-0.1.7/examples/hello_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-13 15:56:27.000000 ucapi-0.1.7/examples/setup_flow.json
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-03-13 15:56:27.000000 ucapi-0.1.7/examples/setup_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-13 15:56:27.000000 ucapi-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-13 15:56:27.000000 ucapi-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-13 15:56:32.821004 ucapi-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 15:56:27.000000 ucapi-0.1.7/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:56:32.821004 ucapi-0.1.7/ucapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-13 15:56:32.000000 ucapi-0.1.7/ucapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    31239 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/api_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/media_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-13 15:56:27.000000 ucapi-0.1.7/ucapi/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:56:32.821004 ucapi-0.1.7/ucapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-13 15:56:32.000000 ucapi-0.1.7/ucapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-13 15:56:32.000000 ucapi-0.1.7/ucapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:56:32.000000 ucapi-0.1.7/ucapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-13 15:56:32.000000 ucapi-0.1.7/ucapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 15:56:32.000000 ucapi-0.1.7/ucapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:52:11.251019 ucapi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-28 20:52:05.000000 ucapi-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-28 20:52:05.000000 ucapi-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-28 20:52:05.000000 ucapi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-28 20:52:11.251019 ucapi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-28 20:52:05.000000 ucapi-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:52:11.243019 ucapi-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-28 20:52:05.000000 ucapi-0.2.0/docs/code_guidelines.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-28 20:52:05.000000 ucapi-0.2.0/docs/setup.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:52:11.247019 ucapi-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/hello_integration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/hello_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/remote_ui_page.json
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/setup_flow.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-28 20:52:05.000000 ucapi-0.2.0/examples/setup_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-28 20:52:05.000000 ucapi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-28 20:52:05.000000 ucapi-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 20:52:11.251019 ucapi-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-28 20:52:05.000000 ucapi-0.2.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:52:11.247019 ucapi-0.2.0/ucapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:52:11.000000 ucapi-0.2.0/ucapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31239 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/api_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/media_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-28 20:52:05.000000 ucapi-0.2.0/ucapi/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:52:11.251019 ucapi-0.2.0/ucapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-28 20:52:11.000000 ucapi-0.2.0/ucapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-28 20:52:11.000000 ucapi-0.2.0/ucapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:52:11.000000 ucapi-0.2.0/ucapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 20:52:11.000000 ucapi-0.2.0/ucapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 20:52:11.000000 ucapi-0.2.0/ucapi.egg-info/top_level.txt
```

### Comparing `ucapi-0.1.7/CHANGELOG.md` & `ucapi-0.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 ## Unreleased
 
 _Changes in the next release_
 
 ---
 
+## v0.2.0 - 2024-04-28
+### Added
+- New remote-entity type. Requires remote-core / Core Simulator version 0.43.0 or newer.
+
 ## v0.1.7 - 2024-03-13
 ### Changed
 - Filter out base64 encoded media-player image fields in log messages ([#17](https://github.com/unfoldedcircle/integration-python-library/issues/17)).
 
 ## v0.1.6 - 2024-03-04
 ### Added
 - Media-player RepeatMode enum and new features: context_menu, settings
```

### Comparing `ucapi-0.1.7/CONTRIBUTING.md` & `ucapi-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/LICENSE` & `ucapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/PKG-INFO` & `ucapi-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucapi
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python wrapper for the Unfolded Circle Integration API
 Author-email: Unfolded Circle ApS <hello@unfoldedcircle.com>
 License: MPL-2.0
 Project-URL: Homepage, https://www.unfoldedcircle.com/
 Project-URL: Source Code, https://github.com/unfoldedcircle/integration-python-library
 Project-URL: Bug Reports, https://github.com/unfoldedcircle/integration-python-library/issues
 Project-URL: Discord, http://unfolded.chat/
```

### Comparing `ucapi-0.1.7/README.md` & `ucapi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/docs/code_guidelines.md` & `ucapi-0.2.0/docs/code_guidelines.md`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/examples/README.md` & `ucapi-0.2.0/examples/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 ## hello_integration
 
 The [hello_integration.py](hello_integration.py) example is a "hello world" example showing the bare minimum required
 to start with an integration driver for the Remote Two.
 
 It defines a single push button with a callback handler. When pushed, it just prints a message in the console.
 
+## remote
+
+The [remote.py](remote.py) example shows how to use the [remote-entity](https://github.com/unfoldedcircle/core-api/blob/main/doc/entities/entity_remote.md).
+
+It defines some simple commands, a custom button mapping and user interface pages for the available commands. 
+
 ## setup_flow
 
 The [setup_flow](setup_flow.py) example shows how to define a dynamic setup flow for the driver setup.
 
 If the user selects the _expert_ option in the main setup screen:
 1. An input screen is shown asking to select an item from a dropdown list.
 2. The chosen option will be shown in the next input screen with another setting, on how many button entities to create.
```

### Comparing `ucapi-0.1.7/examples/hello_integration.py` & `ucapi-0.2.0/examples/hello_integration.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/examples/setup_flow.json` & `ucapi-0.2.0/examples/setup_flow.json`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/examples/setup_flow.py` & `ucapi-0.2.0/examples/setup_flow.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/pyproject.toml` & `ucapi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/__init__.py` & `ucapi-0.2.0/ucapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 # Entity types
 from .button import Button  # noqa: F401
 from .climate import Climate  # noqa: F401
 from .cover import Cover  # noqa: F401
 from .light import Light  # noqa: F401
 from .media_player import MediaPlayer  # noqa: F401
+from .remote import Remote  # noqa: F401
 from .sensor import Sensor  # noqa: F401
 from .switch import Switch  # noqa: F401
 
 try:
     from ._version import version as __version__
     from ._version import version_tuple
 except ImportError:
```

### Comparing `ucapi-0.1.7/ucapi/api.py` & `ucapi-0.2.0/ucapi/api.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/api_definitions.py` & `ucapi-0.2.0/ucapi/api_definitions.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/button.py` & `ucapi-0.2.0/ucapi/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,12 +55,10 @@
         """
         super().__init__(
             identifier,
             name,
             EntityTypes.BUTTON,
             ["press"],
             {Attributes.STATE: States.AVAILABLE},
-            None,
-            None,
-            area,
-            cmd_handler,
+            area=area,
+            cmd_handler=cmd_handler,
         )
```

### Comparing `ucapi-0.1.7/ucapi/climate.py` & `ucapi-0.2.0/ucapi/climate.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/cover.py` & `ucapi-0.2.0/ucapi/cover.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/entities.py` & `ucapi-0.2.0/ucapi/entities.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/entity.py` & `ucapi-0.2.0/ucapi/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     """Entity types."""
 
     COVER = "cover"
     BUTTON = "button"
     CLIMATE = "climate"
     LIGHT = "light"
     MEDIA_PLAYER = "media_player"
+    REMOTE = "remote"
     SENSOR = "sensor"
     SWITCH = "switch"
 
 
 class Entity:
     """
     Entity base class.
@@ -38,16 +39,16 @@
     def __init__(
         self,
         identifier: str,
         name: str | dict[str, str],
         entity_type: EntityTypes,
         features: list[str],
         attributes: dict[str, Any],
-        device_class: str | None,
-        options: dict[str, Any] | None,
+        device_class: str | None = None,
+        options: dict[str, Any] | None = None,
         area: str | None = None,
         cmd_handler: CommandHandler = None,
     ):
         """
         Initialize entity.
 
         :param identifier: entity identifier
```

### Comparing `ucapi-0.1.7/ucapi/light.py` & `ucapi-0.2.0/ucapi/light.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/media_player.py` & `ucapi-0.2.0/ucapi/media_player.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/sensor.py` & `ucapi-0.2.0/ucapi/sensor.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi/switch.py` & `ucapi-0.2.0/ucapi/switch.py`

 * *Files identical despite different names*

### Comparing `ucapi-0.1.7/ucapi.egg-info/PKG-INFO` & `ucapi-0.2.0/ucapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucapi
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python wrapper for the Unfolded Circle Integration API
 Author-email: Unfolded Circle ApS <hello@unfoldedcircle.com>
 License: MPL-2.0
 Project-URL: Homepage, https://www.unfoldedcircle.com/
 Project-URL: Source Code, https://github.com/unfoldedcircle/integration-python-library
 Project-URL: Bug Reports, https://github.com/unfoldedcircle/integration-python-library/issues
 Project-URL: Discord, http://unfolded.chat/
```

