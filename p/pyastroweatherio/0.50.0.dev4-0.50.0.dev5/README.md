# Comparing `tmp/pyastroweatherio-0.50.0.dev4.tar.gz` & `tmp/pyastroweatherio-0.50.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.0.dev4.tar", last modified: Sat Apr 27 11:42:08 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.0.dev5.tar", last modified: Sun Apr 28 14:49:35 2024, max compression
```

## Comparing `pyastroweatherio-0.50.0.dev4.tar` & `pyastroweatherio-0.50.0.dev5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev4/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev4/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 11:42:08.099517 pyastroweatherio-0.50.0.dev4/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    37537 2024-04-27 11:42:03.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3968 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20099 2024-04-27 09:24:39.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    42008 2024-04-27 10:59:55.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-04-27 11:41:15.000000 pyastroweatherio-0.50.0.dev4/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-28 14:49:35.270906 pyastroweatherio-0.50.0.dev5/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev5/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-28 14:49:35.270906 pyastroweatherio-0.50.0.dev5/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev5/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-28 14:49:35.262906 pyastroweatherio-0.50.0.dev5/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    40224 2024-04-28 14:49:17.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4031 2024-04-28 09:17:08.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20104 2024-04-28 12:53:36.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    46495 2024-04-28 14:40:54.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-28 14:49:35.270906 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-28 14:49:35.274906 pyastroweatherio-0.50.0.dev5/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-04-28 14:49:04.000000 pyastroweatherio-0.50.0.dev5/setup.py
```

### Comparing `pyastroweatherio-0.50.0.dev4/LICENSE` & `pyastroweatherio-0.50.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev4/PKG-INFO` & `pyastroweatherio-0.50.0.dev5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev4
+Version: 0.50.0.dev5
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev4/README.md` & `pyastroweatherio-0.50.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev4/pyastroweatherio/client.py` & `pyastroweatherio-0.50.0.dev5/pyastroweatherio/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,23 +34,24 @@
     WIND10M_VALUE,
     WIND10M_RANGE,
     HOME_LATITUDE,
     HOME_LONGITUDE,
     STIMER_OUTPUT,
     FORECAST_TYPE_HOURLY,
     SEEING,
+    TRANSPARENCY,
 )
 from pyastroweatherio.dataclasses import (
     ForecastData,
     LocationData,
     NightlyConditionsData,
     DSOUpTonight,
 )
 from pyastroweatherio.errors import RequestError
-from pyastroweatherio.helper_functions import ConversionFunctions, AstronomicalRoutines, AstronomicalSeeing
+from pyastroweatherio.helper_functions import ConversionFunctions, AstronomicalRoutines, AstronomicalSeeing, AstronomicalTransparency, AstronomicalLiftedIndex
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AstroWeather:
     """AstroWeather Communication Client."""
 
@@ -66,14 +67,15 @@
         cloudcover_medium_weakening=DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING,
         cloudcover_low_weakening=DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING,
         seeing_weight=DEFAULT_CONDITION_SEEING_WEIGHT,
         transparency_weight=DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
         calm_weight=DEFAULT_CONDITION_CALM_WEIGHT,
         uptonight_path="/conf/www",
         test_datetime=None,
+        seven_timer=True,
     ):
         self._session: ClientSession = session
         self._latitude = latitude
         self._longitude = longitude
         self._elevation = elevation
         self._timezone_info = timezone_info
         self._weather_data_seventimer = []
@@ -89,14 +91,15 @@
         self._cloudcover_medium_weakening = cloudcover_medium_weakening
         self._cloudcover_low_weakening = cloudcover_low_weakening
         self._seeing_weight = seeing_weight
         self._transparency_weight = transparency_weight
         self._calm_weight = calm_weight
         self._uptonight_path = uptonight_path
         self._test_datetime = test_datetime
+        self._seven_timer = seven_timer
 
         self._forecast_data = None
 
         self.req = session
 
         # Astro Routines
         self._astro_routines = AstronomicalRoutines(
@@ -104,14 +107,16 @@
             self._longitude,
             self._elevation,
             self._timezone_info,
             self._test_datetime,
         )
 
         self._astro_seeing = AstronomicalSeeing()
+        self._astro_transparency = AstronomicalTransparency()
+        self._astro_lifted_index = AstronomicalLiftedIndex()
 
         # Testing
         self._test_mode = False
         if self._test_datetime is not None:
             self._test_mode = True
 
     # Public functions
@@ -182,14 +187,34 @@
                 cloud_cover=details_metno.get("cloud_area_fraction", -1),
                 altitude=self._elevation,
                 air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
             )
         else:
             seeing = SEEING[details_seventimer["seeing"] - 1]
 
+        transparency = 0
+        if details_seventimer["transparency"] == -1 or details_seventimer["transparency"] == -9999:
+            transparency = await self._astro_transparency.calculate_transparency_model(
+                temperature=details_metno.get("air_temperature", -1),
+                humidity=details_metno.get("relative_humidity", -1),
+                dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                wind_speed=details_metno.get("wind_speed", -1),
+                cloud_cover=details_metno.get("cloud_area_fraction", -1),
+                altitude=self._elevation,
+                air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
+            )
+        else:
+            transparency = TRANSPARENCY[details_seventimer["transparency"] - 1]
+
+        await self._astro_lifted_index.calculate_lifted_index(
+            temperature=details_metno.get("air_temperature", -1),
+            dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+            altitude=self._elevation,
+        )
+     
         item = {
             # seventimer_init is "init" of 7timer astro data
             "seventimer_init": seventimer_init,  # init
             # seventimer_timepoint is "timepoint" of 7timer astro data and defines the data for init + timepoint
             "seventimer_timepoint": details_seventimer["timepoint"],  # timepoint
             # Forecast_time is the actual datetime for the forecast data onwards in UTC
             # Corresponds to "time" in met data
@@ -199,15 +224,15 @@
             # Remaining forecast data point in met.no data
             "forecast_length": (len(self._weather_data_metno) - metno_index),
             # Location
             "latitude": self._latitude,
             "longitude": self._longitude,
             "elevation": self._elevation,
             "seeing": seeing,
-            "transparency": details_seventimer["transparency"],
+            "transparency": transparency,
             "lifted_index": details_seventimer["lifted_index"],
             # Calculate
             "sun_next_rising": await self._astro_routines.sun_next_rising_civil(),
             "sun_next_rising_nautical": await self._astro_routines.sun_next_rising_nautical(),
             "sun_next_rising_astro": await self._astro_routines.sun_next_rising_astro(),
             "sun_next_setting": await self._astro_routines.sun_next_setting_civil(),
             "sun_next_setting_nautical": await self._astro_routines.sun_next_setting_nautical(),
@@ -349,22 +374,21 @@
                 _LOGGER.error("Missing Met.no data")
                 break
 
             details_seventimer = self._get_data_seventimer_timer(
                 seventimer_init, datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ")
             )
 
-            transparency = details_seventimer["transparency"]
             item = {
                 "seventimer_init": init_ts,
                 "seventimer_timepoint": details_seventimer["timepoint"],
                 "forecast_time": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"),
                 "hour": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ").hour,  # forecast_time.hour % 24,
                 "seeing": details_seventimer["seeing"],
-                "transparency": transparency,
+                "transparency": details_seventimer["transparency"],
                 "lifted_index": details_seventimer["lifted_index"],
             }
 
             seeing = 0
             if details_seventimer["seeing"] == -1 or details_seventimer["seeing"] == -9999:
                 seeing = await self._astro_seeing.calculate_seeing_model6(
                     temperature=details_metno.get("air_temperature", -1),
@@ -374,30 +398,50 @@
                     cloud_cover=details_metno.get("cloud_area_fraction", -1),
                     altitude=self._elevation,
                     air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
                 )
             else:
                 seeing = SEEING[details_seventimer["seeing"] - 1]
 
-            item["cloudcover"] = details_metno.get("cloud_area_fraction", -1)
+            transparency = 0
+            if details_seventimer["transparency"] == -1 or details_seventimer["transparency"] == -9999:
+                transparency = await self._astro_transparency.calculate_transparency_model(
+                    temperature=details_metno.get("air_temperature", -1),
+                    humidity=details_metno.get("relative_humidity", -1),
+                    dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                    wind_speed=details_metno.get("wind_speed", -1),
+                    cloud_cover=details_metno.get("cloud_area_fraction", -1),
+                    altitude=self._elevation,
+                    air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
+                )
+            else:
+                transparency = TRANSPARENCY[details_seventimer["transparency"] - 1]
 
+            await self._astro_lifted_index.calculate_lifted_index(
+                temperature=details_metno.get("air_temperature", -1),
+                dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                altitude=self._elevation,
+            )
+            
+            item["cloudcover"] = details_metno.get("cloud_area_fraction", -1)
             item["cloud_area_fraction"] = details_metno.get("cloud_area_fraction", -1)
             item["cloud_area_fraction_high"] = details_metno.get("cloud_area_fraction_high", -1)
             item["cloud_area_fraction_medium"] = details_metno.get("cloud_area_fraction_medium", -1)
             item["cloud_area_fraction_low"] = details_metno.get("cloud_area_fraction_low", -1)
             item["fog_area_fraction"] = details_metno.get("fog_area_fraction", -1)
             item["rh2m"] = details_metno.get("relative_humidity", -1)
             item["wind_speed"] = details_metno.get("wind_speed", -1)
             item["seeing"] = seeing
+            item["transparency"] = transparency
             item["condition_percentage"] = await self.calc_condition_percentage(
                 item["cloud_area_fraction_high"],
                 item["cloud_area_fraction_medium"],
                 item["cloud_area_fraction_low"],
                 seeing,
-                details_seventimer["transparency"],
+                transparency,
                 item["wind_speed"],
             )
 
             item["wind_from_direction"] = details_metno.get("wind_from_direction", -1)
             item["temp2m"] = details_metno.get("air_temperature", -1)
             item["dewpoint2m"] = details_metno.get("dew_point_temperature", -1)
             if self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}) == {}:
@@ -495,33 +539,33 @@
                 details_forecast = self._forecast_data[index]
 
                 if len(interval_points) == 0:
                     forecast_dayname = details_forecast.forecast_time.strftime("%A")
                     start_forecast_hour = details_forecast.forecast_time.hour
                     start_weather = details_forecast.weather6
 
-                _LOGGER.debug(
-                    "Idex: %d, Hour of day: %d, cloud_area_fraction: %s %s %s, seeing: %s, transparency: %s, wind_speed: %s, condition: %s",
-                    index,
-                    details_forecast.forecast_time.hour,
-                    str(details_forecast.cloud_area_fraction_high_percentage),
-                    str(details_forecast.cloud_area_fraction_medium_percentage),
-                    str(details_forecast.cloud_area_fraction_low_percentage),
-                    str(details_forecast.seeing),
-                    str(details_forecast.transparency),
-                    str(details_forecast.wind10m_speed),
-                    await self.calc_condition_percentage(
-                        details_forecast.cloud_area_fraction_high_percentage,
-                        details_forecast.cloud_area_fraction_medium_percentage,
-                        details_forecast.cloud_area_fraction_low_percentage,
-                        details_forecast.seeing,
-                        details_forecast.transparency,
-                        details_forecast.wind10m_speed,
-                    ),
-                )
+                # _LOGGER.debug(
+                #     "Idex: %d, Hour of day: %d, cloud_area_fraction: %s %s %s, seeing: %s, transparency: %s, wind_speed: %s, condition: %s",
+                #     index,
+                #     details_forecast.forecast_time.hour,
+                #     str(details_forecast.cloud_area_fraction_high_percentage),
+                #     str(details_forecast.cloud_area_fraction_medium_percentage),
+                #     str(details_forecast.cloud_area_fraction_low_percentage),
+                #     str(details_forecast.seeing),
+                #     str(details_forecast.transparency),
+                #     str(details_forecast.wind10m_speed),
+                #     await self.calc_condition_percentage(
+                #         details_forecast.cloud_area_fraction_high_percentage,
+                #         details_forecast.cloud_area_fraction_medium_percentage,
+                #         details_forecast.cloud_area_fraction_low_percentage,
+                #         details_forecast.seeing,
+                #         details_forecast.transparency,
+                #         details_forecast.wind10m_speed,
+                #     ),
+                # )
 
                 # Calculate Condition
                 if len(interval_points) <= int(math.floor(night_duration_astronomical / 3600)):
                     interval_points.append(
                         await self.calc_condition_percentage(
                             details_forecast.cloud_area_fraction_high_percentage,
                             details_forecast.cloud_area_fraction_medium_percentage,
@@ -564,15 +608,16 @@
     async def calc_condition_percentage(
         self, cloudcover_high, cloudcover_medium, cloudcover_low, seeing, transparency, wind_speed
     ):
         """Return condition based on cloud cover, seeing, transparency, and wind speed"""
 
         # Seeing is something in between 0 and 2.5 arcsecs
         seeing = int(seeing * 40)  # arcsecs up to 2.5
-        transparency = int((transparency - 1) * (100 / 7))  # 1-8, 8 is bad
+        # transparency = int(transparency * 40)  # mag degration up to 2.5
+        transparency = int(transparency * 100)  # mag degration up to 1
         # Wind speed is something in between 0 and 16.5 m/s
         if wind_speed > 16.5:
             wind_speed = 16.5
         wind_speed_value = int(wind_speed * (100 / 16.5))  # m/s up to 16.5
 
         cloudcover = []
         cloudcover.append(cloudcover_high * self._cloudcover_high_weakening)
@@ -654,32 +699,33 @@
     async def retrieve_data_seventimer(self):
         """Retrieves current data from 7timer"""
 
         if ((datetime.now() - self._weather_data_seventimer_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
             self._weather_data_seventimer_timestamp = datetime.now()
             _LOGGER.debug("Updating data from 7Timer")
 
-            astro_dataseries = None
+            astro_dataseries = {}
 
             # Testing
-            if self._test_mode:
-                if os.path.isfile("debug/astro.json"):
-                    _LOGGER.debug("Reading 7Timer from file")
-                    with open("debug/astro.json") as json_file:
-                        astro_dataseries_json = json.load(json_file)
-                        astro_dataseries = astro_dataseries_json.get("dataseries", {})
-                        json_data_astro = {"init": astro_dataseries_json.get("init")}
+            if self._seven_timer:
+                if self._test_mode:
+                    if os.path.isfile("debug/astro.json"):
+                        _LOGGER.debug("Reading 7Timer from file")
+                        with open("debug/astro.json") as json_file:
+                            astro_dataseries_json = json.load(json_file)
+                            astro_dataseries = astro_dataseries_json.get("dataseries", {})
+                            json_data_astro = {"init": astro_dataseries_json.get("init")}
+                    else:
+                        json_data_astro = await self.async_request_seventimer("astro", "get")
+                        astro_dataseries = json_data_astro.get("dataseries", {})
                 else:
                     json_data_astro = await self.async_request_seventimer("astro", "get")
                     astro_dataseries = json_data_astro.get("dataseries", {})
-            else:
-                json_data_astro = await self.async_request_seventimer("astro", "get")
-                astro_dataseries = json_data_astro.get("dataseries", {})
 
-            if astro_dataseries != {}:
+            if astro_dataseries != {} and self._seven_timer:
                 self._weather_data_seventimer = astro_dataseries
                 self._weather_data_seventimer_init = json_data_astro.get("init")
             else:
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
                 # TODO: Think about a complete redesign of the calculations and potentially
                 #       make met.no the leading source instead of 7timer
```

### Comparing `pyastroweatherio-0.50.0.dev4/pyastroweatherio/const.py` & `pyastroweatherio-0.50.0.dev5/pyastroweatherio/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 #     '1.25 to 1.5"',
 #     '1.5 to 2"',
 #     '2 to 2.5"',
 #     'Over 2.5"',
 # ]
 
 SEEING = [0.25, 0.625, 0.875, 1.125, 1.375, 1.75, 2.25, 2.5]
+TRANSPARENCY = [0.15, 0.35, 0.45, 0.55, 0.65, 0.775, 0.925, 1]
 
 TRANSPARENCY_PLAIN = [
     "Below 0.3 mag",
     "0.3 to 0.4 mag",
     "0.4 to 0.5 mag",
     "0.5 to 0.6 mag",
     "0.6 to 0.7 mag",
```

### Comparing `pyastroweatherio-0.50.0.dev4/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.0.dev5/pyastroweatherio/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,22 +112,22 @@
 
     @property
     def seeing_percentage(self) -> int:
         """Return Seeing."""
         return int(100 - self._seeing * 40)
 
     @property
-    def transparency(self) -> int:
+    def transparency(self) -> float:
         """Return Transparency."""
-        return int(self._transparency)
+        return round(self._transparency, 2)
 
     @property
     def transparency_percentage(self) -> int:
         """Return Transparency."""
-        return int((100 + 100 / 7 - self._transparency * 100 / 7))
+        return int(100 - self._transparency * 100)
 
     @property
     def lifted_index(self) -> int:
         """Return Lifted Index."""
         return int(self._lifted_index)
 
     @property
@@ -252,21 +252,21 @@
         """Return Seeing."""
         return "Deprecated. Use seeing instead."
         seeing = self._seeing
         if seeing >= 1 and seeing <= 8:
             return SEEING_PLAIN[seeing - 1]
         return None
 
-    @property
-    def transparency_plain(self) -> str:
-        """Return Transparency."""
-        transparency = self._transparency
-        if transparency >= 1 and transparency <= 8:
-            return TRANSPARENCY_PLAIN[self._transparency - 1]
-        return None
+    # @property
+    # def transparency_plain(self) -> str:
+    #     """Return Transparency."""
+    #     transparency = self._transparency
+    #     if transparency >= 1 and transparency <= 8:
+    #         return TRANSPARENCY_PLAIN[self._transparency - 1]
+    #     return None
 
     @property
     def wind10m_speed_plain(self) -> str:
         """Return Transparency."""
         wind10m_speed = self._wind_speed
 
         wind_speed_value = 0
```

### Comparing `pyastroweatherio-0.50.0.dev4/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.0.dev5/pyastroweatherio/helper_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,16 +42,118 @@
 
     async def anchor_timestamp(self, value) -> datetime:
         """Converts the datetime string from 7Timer to DateTime."""
         _LOGGER.debug("7timer anchor timestamp: %s", str(datetime.strptime(value, "%Y%m%d%H")))
         return datetime.strptime(value, "%Y%m%d%H")
 
 
+class AstronomicalLiftedIndex:
+    """Calculate astronomical lifted index"""
+
+    # Write a python3 program to calculate atmospheric lifted index based on humidity, temperature, clouds, wind, altitude, dew_point_temperature, transparency, and air_pressure_at_sea_level and convert the transparency to magnitude degradation
+
+    def __init__(
+        self,
+    ):
+        _LOGGER.debug("AstronomicalTransparency calculation mode active")
+        # Temperature in Celsius
+        # Altitude in meters
+        # Dew point temperature in Celsius
+
+    async def calculate_lifted_index(self, temperature, altitude, dew_point_temperature):
+        # Constants
+        lapse_rate = 0.0098  # Standard lapse rate (temperature decrease with altitude)
+
+        # Calculate temperature at lifting condensation level (LCL)
+        temperature_LCL = dew_point_temperature - ((altitude / 1000) * lapse_rate)
+
+        # Calculate lifted index
+        lifted_index = temperature - temperature_LCL
+
+        print("Estimated Atmospheric Lifted Index: {:.2f}".format(lifted_index))
+        return lifted_index
+
+
+class AstronomicalTransparency:
+    """Calculate astronomical transparency"""
+
+    # Write a python3 program to calculate atmospheric transparence based on humidity, temperature, clouds, wind, altitude, dew_point_temperature, and air_pressure_at_sea_level and convert the transparency to magnitude degradation
+
+    def __init__(
+        self,
+    ):
+        _LOGGER.debug("AstronomicalTransparency calculation mode active")
+        # Relative humidity (0.0 to 1.0)
+        # Temperature in Celsius
+        # Cloud cover fraction (0.0 to 1.0)
+        # Wind speed in meters per second
+        # Altitude in meters
+        # Dew point temperature in Celsius
+        # Air pressure at sea level in hPa
+
+    def calculate_transparency(self, humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level):
+        # Coefficients for the linear model (you can adjust these based on your requirements)
+        humidity_coefficient = 0.02
+        temperature_coefficient = 0.03
+        cloud_cover_coefficient = -0.1
+        wind_speed_coefficient = -0.05
+        altitude_coefficient = -0.01
+        dew_point_temperature_coefficient = 0.02
+        air_pressure_coefficient = 0.01
+
+        # Calculate transparency using the linear model
+        transparency = (1 - (humidity * humidity_coefficient) +
+                        (temperature * temperature_coefficient) +
+                        (cloud_cover * cloud_cover_coefficient / 100) +
+                        (wind_speed * wind_speed_coefficient) +
+                        # (altitude * altitude_coefficient) +
+                        # (air_pressure_at_sea_level * air_pressure_coefficient) +
+                        (dew_point_temperature * dew_point_temperature_coefficient))
+
+        print(humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level, ":", transparency)
+        # Ensure transparency is within the valid range [0, 1]
+        transparency = max(0, min(1, transparency))
+
+        return transparency
+
+    def transparency_to_magnitude_degradation(self, transparency):
+
+        # if transparency == 0:
+        #     return float(2.5)  #float('inf')
+        # else:
+        #     magnitude_degradation = -2.5 * math.log10(transparency)
+        #     magnitude_degradation = max(0, min(2.5, magnitude_degradation))
+
+        #     return magnitude_degradation
+
+        # 7Timer
+        if transparency == 0:
+            return float(1)  #float('inf')
+        else:
+            magnitude_degradation = -1 * math.log10(transparency)
+            magnitude_degradation = max(0, min(1, magnitude_degradation))
+
+            return magnitude_degradation
+
+    async def calculate_transparency_model(self, humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level):
+
+        # Calculate transparency
+        transparency = self.calculate_transparency(humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level)
+
+        # Convert transparency to magnitude degradation
+        magnitude_degradation = self.transparency_to_magnitude_degradation(transparency)
+
+        print("Estimated Atmospheric Transparency: {:.2f}".format(transparency))
+        print("Magnitude Degradation: {:.2f}".format(magnitude_degradation))
+        
+        return magnitude_degradation
+
+
 class AstronomicalSeeing:
-    """Calculate different astronomical objects"""
+    """Calculate astronomical seeing"""
 
     def __init__(
         self,
     ):
         _LOGGER.debug("AstronomicalSeeing calculation mode active")
         # temperature = 15  # in Celsius
         # wind_speed = 5  # in m/s
```

### Comparing `pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev4
+Version: 0.50.0.dev5
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev4/setup.py` & `pyastroweatherio-0.50.0.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.0.dev4",
+    version="0.50.0.dev5",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

