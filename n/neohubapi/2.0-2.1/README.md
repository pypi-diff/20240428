# Comparing `tmp/neohubapi-2.0.tar.gz` & `tmp/neohubapi-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neohubapi-2.0.tar", last modified: Tue Nov 21 23:21:02 2023, max compression
+gzip compressed data, was "neohubapi-2.1.tar", last modified: Sat Apr 27 22:40:24 2024, max compression
```

## Comparing `neohubapi-2.0.tar` & `neohubapi-2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-11-21 23:21:02.519477 neohubapi-2.0/
--rw-r--r--   0 andrius   (1000) andrius   (1000)      135 2020-12-27 20:17:35.000000 neohubapi-2.0/.gitignore
--rw-r--r--   0 andrius   (1000) andrius   (1000)      330 2022-12-01 20:33:25.000000 neohubapi-2.0/.gitlab-ci.yml
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-11-21 23:21:02.519477 neohubapi-2.0/LICENSES/
--rw-r--r--   0 andrius   (1000) andrius   (1000)    16814 2020-10-16 22:01:40.000000 neohubapi-2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     6916 2020-11-20 18:38:22.000000 neohubapi-2.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     7431 2020-10-16 15:56:35.000000 neohubapi-2.0/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     1108 2020-10-16 22:01:40.000000 neohubapi-2.0/LICENSES/MIT.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     2677 2023-11-21 23:21:02.519477 neohubapi-2.0/PKG-INFO
--rw-r--r--   0 andrius   (1000) andrius   (1000)     2134 2023-10-25 00:36:21.000000 neohubapi-2.0/README.md
--rwxr-xr-x   0 andrius   (1000) andrius   (1000)      938 2021-01-19 21:53:09.000000 neohubapi-2.0/example.py
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-11-21 23:21:02.519477 neohubapi-2.0/neohubapi/
--rw-r--r--   0 andrius   (1000) andrius   (1000)      181 2021-02-06 14:30:21.000000 neohubapi-2.0/neohubapi/__init__.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)     1229 2021-06-23 10:58:50.000000 neohubapi-2.0/neohubapi/enums.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)    22819 2023-11-21 19:48:32.000000 neohubapi-2.0/neohubapi/neohub.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)     6823 2023-11-21 19:48:32.000000 neohubapi-2.0/neohubapi/neostat.py
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-11-21 23:21:02.519477 neohubapi-2.0/neohubapi.egg-info/
--rw-r--r--   0 andrius   (1000) andrius   (1000)     2677 2023-11-21 23:21:02.000000 neohubapi-2.0/neohubapi.egg-info/PKG-INFO
--rw-r--r--   0 andrius   (1000) andrius   (1000)      475 2023-11-21 23:21:02.000000 neohubapi-2.0/neohubapi.egg-info/SOURCES.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2023-11-21 23:21:02.000000 neohubapi-2.0/neohubapi.egg-info/dependency_links.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)       26 2023-11-21 23:21:02.000000 neohubapi-2.0/neohubapi.egg-info/requires.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)       10 2023-11-21 23:21:02.000000 neohubapi-2.0/neohubapi.egg-info/top_level.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2020-12-27 19:07:42.000000 neohubapi-2.0/neohubapi.egg-info/zip-safe
--rw-r--r--   0 andrius   (1000) andrius   (1000)       29 2022-12-01 20:29:12.000000 neohubapi-2.0/pytest.ini
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-11-21 23:21:02.519477 neohubapi-2.0/scripts/
--rwxr-xr-x   0 andrius   (1000) andrius   (1000)    11329 2023-11-21 19:48:32.000000 neohubapi-2.0/scripts/neohub_cli.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)       38 2023-11-21 23:21:02.519477 neohubapi-2.0/setup.cfg
--rwxr-xr-x   0 andrius   (1000) andrius   (1000)     1012 2023-11-21 19:48:32.000000 neohubapi-2.0/setup.py
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-11-21 23:21:02.519477 neohubapi-2.0/tests/
--rw-r--r--   0 andrius   (1000) andrius   (1000)     3279 2022-12-01 20:29:03.000000 neohubapi-2.0/tests/test_neohub.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2024-04-27 22:40:24.911866 neohubapi-2.1/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      135 2020-12-27 20:17:35.000000 neohubapi-2.1/.gitignore
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      330 2022-12-01 20:33:25.000000 neohubapi-2.1/.gitlab-ci.yml
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2024-04-27 22:40:24.908533 neohubapi-2.1/LICENSES/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)    16814 2020-10-16 22:01:40.000000 neohubapi-2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     6916 2020-11-20 18:38:22.000000 neohubapi-2.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     7431 2020-10-16 15:56:35.000000 neohubapi-2.1/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     1108 2020-10-16 22:01:40.000000 neohubapi-2.1/LICENSES/MIT.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     2694 2024-04-27 22:40:24.911866 neohubapi-2.1/PKG-INFO
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     2151 2024-01-21 17:03:32.000000 neohubapi-2.1/README.md
+-rwxr-xr-x   0 andrius   (1000) andrius   (1000)      938 2021-01-19 21:53:09.000000 neohubapi-2.1/example.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2024-04-27 22:40:24.908533 neohubapi-2.1/neohubapi/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      181 2021-02-06 14:30:21.000000 neohubapi-2.1/neohubapi/__init__.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     1229 2021-06-23 10:58:50.000000 neohubapi-2.1/neohubapi/enums.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)    22819 2023-11-21 19:48:32.000000 neohubapi-2.1/neohubapi/neohub.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     7200 2024-04-27 22:34:02.000000 neohubapi-2.1/neohubapi/neostat.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2024-04-27 22:40:24.911866 neohubapi-2.1/neohubapi.egg-info/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     2694 2024-04-27 22:40:24.000000 neohubapi-2.1/neohubapi.egg-info/PKG-INFO
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      475 2024-04-27 22:40:24.000000 neohubapi-2.1/neohubapi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2024-04-27 22:40:24.000000 neohubapi-2.1/neohubapi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       26 2024-04-27 22:40:24.000000 neohubapi-2.1/neohubapi.egg-info/requires.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       10 2024-04-27 22:40:24.000000 neohubapi-2.1/neohubapi.egg-info/top_level.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2020-12-27 19:07:42.000000 neohubapi-2.1/neohubapi.egg-info/zip-safe
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       29 2022-12-01 20:29:12.000000 neohubapi-2.1/pytest.ini
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2024-04-27 22:40:24.911866 neohubapi-2.1/scripts/
+-rwxr-xr-x   0 andrius   (1000) andrius   (1000)    11329 2023-11-21 19:48:32.000000 neohubapi-2.1/scripts/neohub_cli.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       38 2024-04-27 22:40:24.911866 neohubapi-2.1/setup.cfg
+-rwxr-xr-x   0 andrius   (1000) andrius   (1000)     1012 2024-04-27 22:37:33.000000 neohubapi-2.1/setup.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2024-04-27 22:40:24.911866 neohubapi-2.1/tests/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     3279 2022-12-01 20:29:03.000000 neohubapi-2.1/tests/test_neohub.py
```

### Comparing `neohubapi-2.0/LICENSES/CC-BY-4.0.txt` & `neohubapi-2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/LICENSES/CC0-1.0.txt` & `neohubapi-2.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/LICENSES/LGPL-3.0-or-later.txt` & `neohubapi-2.1/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/LICENSES/MIT.txt` & `neohubapi-2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/PKG-INFO` & `neohubapi-2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neohubapi
-Version: 2.0
+Version: 2.1
 Summary: Async library to communicate with Heatmiser NeoHub 2 API.
 Home-page: https://gitlab.com/neohubapi/neohubapi/
 Author: Andrius Štikonas
 Author-email: andrius@stikonas.eu
 Keywords: neohub,heatmiser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -45,16 +45,17 @@
 
 async def run():
     # Legacy connection
     hub = neohub.NeoHub()
     # Or, for a websocket connection:
     # hub = neohub.Neohub(port=4243, token='xxx-xxxxxxx')
     system = await hub.get_system()
-    hub_data, devices = await hub.get_live_data()
-    for device in devices['thermostats']:
+    hub_data = await hub.get_devices_data()
+    devices = hub_data['neo_devices']
+    for device in devices:
         print(f"Temperature in zone {device.name}: {device.temperature}")
         await device.identify()
 
 
 asyncio.run(run())
 ```
```

### Comparing `neohubapi-2.0/README.md` & `neohubapi-2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 
 async def run():
     # Legacy connection
     hub = neohub.NeoHub()
     # Or, for a websocket connection:
     # hub = neohub.Neohub(port=4243, token='xxx-xxxxxxx')
     system = await hub.get_system()
-    hub_data, devices = await hub.get_live_data()
-    for device in devices['thermostats']:
+    hub_data = await hub.get_devices_data()
+    devices = hub_data['neo_devices']
+    for device in devices:
         print(f"Temperature in zone {device.name}: {device.temperature}")
         await device.identify()
 
 
 asyncio.run(run())
 ```
```

### Comparing `neohubapi-2.0/example.py` & `neohubapi-2.1/example.py`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/neohubapi/enums.py` & `neohubapi-2.1/neohubapi/enums.py`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/neohubapi/neohub.py` & `neohubapi-2.1/neohubapi/neohub.py`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/neohubapi/neostat.py` & `neohubapi-2.1/neohubapi/neostat.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,21 @@
 
         self.weekday = Weekday(self.date)
 
         _switch_delay_left = datetime.strptime(self.switch_delay_left, "%H:%M")
         self.switch_delay_left = timedelta(
             hours=_switch_delay_left.hour,
             minutes=_switch_delay_left.minute)
+
+        # The API Sometimes returns 24:XX, see https://gitlab.com/neohubapi/neohubapi/-/issues/8
+        time_fragments = self.time.split(':')
+        if time_fragments[0] == "24":
+            corrected_time = f"00:{time_fragments[1]}"
+            self._logger.debug(f"API returned {self.time} for time, correcting to {corrected_time}")
+            self.time = corrected_time
         _time = datetime.strptime(self.time, "%H:%M")
         self.time = timedelta(hours=_time.hour, minutes=_time.minute)
 
         # 35 Degrees appears to be the hard limit in app, 5 degrees appears to be the hard lower limit.
         self.max_temperature_limit = 35
         self.min_temperature_limit = 5
```

### Comparing `neohubapi-2.0/neohubapi.egg-info/PKG-INFO` & `neohubapi-2.1/neohubapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neohubapi
-Version: 2.0
+Version: 2.1
 Summary: Async library to communicate with Heatmiser NeoHub 2 API.
 Home-page: https://gitlab.com/neohubapi/neohubapi/
 Author: Andrius Štikonas
 Author-email: andrius@stikonas.eu
 Keywords: neohub,heatmiser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -45,16 +45,17 @@
 
 async def run():
     # Legacy connection
     hub = neohub.NeoHub()
     # Or, for a websocket connection:
     # hub = neohub.Neohub(port=4243, token='xxx-xxxxxxx')
     system = await hub.get_system()
-    hub_data, devices = await hub.get_live_data()
-    for device in devices['thermostats']:
+    hub_data = await hub.get_devices_data()
+    devices = hub_data['neo_devices']
+    for device in devices:
         print(f"Temperature in zone {device.name}: {device.temperature}")
         await device.identify()
 
 
 asyncio.run(run())
 ```
```

### Comparing `neohubapi-2.0/scripts/neohub_cli.py` & `neohubapi-2.1/scripts/neohub_cli.py`

 * *Files identical despite different names*

### Comparing `neohubapi-2.0/setup.py` & `neohubapi-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="neohubapi",
-    version="2.0",
+    version="2.1",
     description="Async library to communicate with Heatmiser NeoHub 2 API.",
     url="https://gitlab.com/neohubapi/neohubapi/",
     author="Andrius Štikonas",
     author_email="andrius@stikonas.eu",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
```

### Comparing `neohubapi-2.0/tests/test_neohub.py` & `neohubapi-2.1/tests/test_neohub.py`

 * *Files identical despite different names*

