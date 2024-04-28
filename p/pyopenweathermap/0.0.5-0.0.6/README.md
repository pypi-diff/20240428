# Comparing `tmp/pyopenweathermap-0.0.5.tar.gz` & `tmp/pyopenweathermap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenweathermap-0.0.5.tar", max compression
+gzip compressed data, was "pyopenweathermap-0.0.6.tar", max compression
```

## Comparing `pyopenweathermap-0.0.5.tar` & `pyopenweathermap-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.5/LICENSE
--rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.5/README.md
--rw-r--r--   0        0        0      568 2024-04-26 18:16:57.650541 pyopenweathermap-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.5/src/pyopenweathermap/__init__.py
--rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.5/src/pyopenweathermap/exception.py
--rw-r--r--   0        0        0     2721 2024-04-26 14:38:45.810524 pyopenweathermap-0.0.5/src/pyopenweathermap/owm_client.py
--rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.5/src/pyopenweathermap/weather.py
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.6/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.6/README.md
+-rw-r--r--   0        0        0      568 2024-04-28 14:45:56.155941 pyopenweathermap-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.6/src/pyopenweathermap/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.6/src/pyopenweathermap/exception.py
+-rw-r--r--   0        0        0     2783 2024-04-28 14:46:26.536085 pyopenweathermap-0.0.6/src/pyopenweathermap/owm_client.py
+-rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.6/src/pyopenweathermap/weather.py
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.6/PKG-INFO
```

### Comparing `pyopenweathermap-0.0.5/LICENSE` & `pyopenweathermap-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.5/pyproject.toml` & `pyopenweathermap-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyopenweathermap"
-version = "0.0.5"
+version = "0.0.6"
 description = "lib for OpenWeatherMap for Home Assistant"
 authors = ["Evgeny <iam@freekode.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["homeassistant", "owm", "openweathermap"]
 packages = [
     { include = "pyopenweathermap", from = "src" },
```

### Comparing `pyopenweathermap-0.0.5/src/pyopenweathermap/owm_client.py` & `pyopenweathermap-0.0.6/src/pyopenweathermap/owm_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 API_URL = 'https://api.openweathermap.org/data/3.0/onecall'
 WEATHER_TYPES = {'current', 'minutely', 'hourly', 'daily', 'alerts'}
 
 
 class OWMClient:
     session: ClientSession | None = None
-    request_timeout: int = 10
+    request_timeout: int
 
-    def __init__(self, api_key, units="metric", lang='en'):
+    def __init__(self, api_key, units="metric", lang='en', request_timeout=20):
         self.api_key = api_key
         self.units = units
         self.lang = lang
+        self.request_timeout = request_timeout
 
     async def get_weather(self, lat, lon, weather_types=None) -> WeatherReport:
         if weather_types is None:
             exclude_weather_types = {}
         else:
             exclude_weather_types = WEATHER_TYPES - set(weather_types)
```

### Comparing `pyopenweathermap-0.0.5/src/pyopenweathermap/weather.py` & `pyopenweathermap-0.0.6/src/pyopenweathermap/weather.py`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.5/PKG-INFO` & `pyopenweathermap-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenweathermap
-Version: 0.0.5
+Version: 0.0.6
 Summary: lib for OpenWeatherMap for Home Assistant
 License: MIT
 Keywords: homeassistant,owm,openweathermap
 Author: Evgeny
 Author-email: iam@freekode.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

