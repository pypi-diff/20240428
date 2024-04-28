# Comparing `tmp/pyweatherfr-5.3.4.tar.gz` & `tmp/pyweatherfr-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.3.4.tar", last modified: Mon Apr 22 18:14:30 2024, max compression
+gzip compressed data, was "pyweatherfr-5.3.5.tar", last modified: Sun Apr 28 07:49:57 2024, max compression
```

## Comparing `pyweatherfr-5.3.4.tar` & `pyweatherfr-5.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:14:30.486690 pyweatherfr-5.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 18:14:30.486690 pyweatherfr-5.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:14:30.486690 pyweatherfr-5.3.4/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34641 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/meteofrance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/openstreetmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:14:30.486690 pyweatherfr-5.3.4/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 18:14:30.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 18:14:30.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:14:30.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 18:14:30.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:13:40.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-22 18:14:30.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 18:14:30.000000 pyweatherfr-5.3.4/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:14:30.486690 pyweatherfr-5.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-22 18:13:33.000000 pyweatherfr-5.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36086 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/meteofrance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/openstreetmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:49:09.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 07:49:57.000000 pyweatherfr-5.3.5/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:49:57.309765 pyweatherfr-5.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-28 07:49:04.000000 pyweatherfr-5.3.5/setup.py
```

### Comparing `pyweatherfr-5.3.4/LICENSE.txt` & `pyweatherfr-5.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.4/PKG-INFO` & `pyweatherfr-5.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.3.4
+Version: 5.3.5
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.3.4/README.md` & `pyweatherfr-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.4/pyweatherfr/__init__.py` & `pyweatherfr-5.3.5/pyweatherfr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.4/pyweatherfr/app.py` & `pyweatherfr-5.3.5/pyweatherfr/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import pytz
 import tzlocal
 import numpy
 
 
 SUN = "\U0001F31E"
 MI_SUN = "\U0001F324"
-CLOUD = "\U0001F325"
+CLOUD = "\U0001F325" + " "
 NIGHT_CLOUD = "\U0001f319"
 MI_CLOUD_RAIN = "\U0001F326"
-RAIN = "\U0001F327"
+RAIN = "\U0001F327" + " "
 SNOW = "\U0001F328"
 NIGHT_CLEAR = "\U0001f319"
 ORAGE = "\U0001F329"
 ORAGE_PLUIE = "\U0001F329" + " " + "\U0001F327"
 FOG = "\U0001F32B"
 DROPLET = "\U0001F4A7"
 FLOCON = "\U00002744"
@@ -60,14 +60,15 @@
 WARNING_SNOW = 0.1
 WARNING_RAIN = 0.1
 WARNING_WIND = 30
 WARNING_WIND_GUST = 50
 WARNING_HP = 1030
 WARNING_BP = 995
 WARNING_HUMIDITY = 90
+WARNING_WATTS = 1000
 
 
 def app():
     if pyweatherfr.args.compute_args().town:
         ville, dpt, lat, long, country = obtain_city_data()
     elif pyweatherfr.args.compute_args().gps:
         ville, dpt, lat, long, country = obtain_city_data_from_gps()
@@ -91,22 +92,22 @@
         previsions_detaillees(ville, dpt, lat, long, tz)
     if (
         not pyweatherfr.args.compute_args().town
         and not pyweatherfr.args.compute_args().gps
     ):
         print(
             pyweatherfr.log.my_colored(
-                "warning : si vous utilisez un proxy ou un VPN, la localisation peut être incorrecte",
+                "warning : si vous utilisez un proxy ou un VPN, la localisation peut être incorrecte.",
                 "yellow",
             )
         )
     if country is None:
         print(
             pyweatherfr.log.my_colored(
-                "warning : ville potentiellement hors de France, les prévisions et données peuvent être moins précises",
+                "warning : ville potentiellement hors de France, les prévisions et données peuvent être moins précises.",
                 "yellow",
             )
         )
     elif country != "France":
         print(
             pyweatherfr.log.my_colored(
                 "warning : ville hors de France, les prévisions et données peuvent être moins précises",
@@ -150,71 +151,87 @@
     print_generic_data_town(ville, dpt, lat, long, alt, recap)
     data = []
     new_var = diff_jour(long, lat)
     for h in range(0, 24):
         if numpy.isnan(hourly_temperature_2m[h]):
             print(
                 pyweatherfr.log.my_colored(
-                    "warning : pas de données pour ce jour", "yellow"
+                    "warning : pas de données pour ce jour.", "yellow"
                 )
             )
             exit(1)
+        nbw=0    
         warning = ""
         if (
             datetime.datetime.now(tz=pytz.timezone(tz))
             + datetime.timedelta(days=new_var)
         ).strftime("%Y-%m-%d") == datetime.datetime.now(tz=pytz.timezone(tz)).strftime(
             "%Y-%m-%d"
         ) and 0 < h - int(
             datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%H")
         ) <= 1:
-            warning = warning + " " + CLOCK
+            warning = warning + "  " + CLOCK
+            nbw=nbw+1
         if isFullWidth():
             temp = f"{hourly_temperature_2m[h]:.1f}°C ({hourly_apparent_temperature[h]:.1f}°C)"
         else:
             temp = f"{hourly_temperature_2m[h]:.0f}°C"
         if (
             hourly_temperature_2m[h] <= WARNING_FROID
             or hourly_apparent_temperature[h] <= WARNING_FROID
         ):
-            warning = warning + " " + COLD
+            warning = warning + "  " + COLD
+            nbw=nbw+1
         if (
             hourly_temperature_2m[h] >= WARNING_WARM
             or hourly_apparent_temperature[h] >= WARNING_WARM
         ):
-            warning = warning + " " + WARM
+            warning = warning + "  " + WARM
+            nbw=nbw+1
         pluie = f"{hourly_precipitation[h]:.1f}mm"
         if snowfall[h] >= WARNING_SNOW:
-            warning = warning + " " + SNOW
+            warning = warning + "  " + SNOW
+            nbw=nbw+1
         elif hourly_precipitation[h] >= WARNING_RAIN:
-            warning = warning + " " + RAIN
+            warning = warning + "  " + RAIN
+            nbw=nbw+1
 
         vent = (
             f"{hourly_wind_speed_10m[h]:.0f}km/h ({hourly_wind_gusts_10m[h]:.0f}km/h)"
         )
         direction = calculer_direction(hourly_wind_direction_10m[h])
 
         vent = vent
         if (
             hourly_wind_speed_10m[h] >= WARNING_WIND
             or hourly_wind_gusts_10m[h] >= WARNING_WIND_GUST
         ):
-            warning = warning + " " + WIND
+            warning = warning + "  " + WIND
+            nbw=nbw+1
 
         pression = f"{surface_pressure[h]:.0f}Hpa"
         if surface_pressure[h] >= WARNING_HP:
-            warning = warning + " " + ELEPHANT
+            warning = warning + "  " + ELEPHANT
+            nbw=nbw+1     
         if surface_pressure[h] <= WARNING_BP:
-            warning = warning + " " + PLUME
+            warning = warning + "  " + PLUME 
+            nbw=nbw+1                         
         weather, emojiweather = traduction(current_weather_code[h], isday[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
+        if relative_humidity_2m[h] >= WARNING_HUMIDITY:
+            warning = warning + "  " + DROPLET
+            nbw=nbw+1           
         duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
         rayonnement = f" {shortwave_radiation[h]:.0f}W/m\u00B2"
-        if shortwave_radiation[h] > 1000:
-            warning = warning + " " + LUNETTES
+        if shortwave_radiation[h] >= WARNING_WATTS:
+            warning = warning + "  " + LUNETTES
+            nbw=nbw+1
+        for i in range(nbw):  
+            warning = warning + " "
+        warning = warning + " "    
         if pyweatherfr.args.compute_args().nocolor:
             if isFullWidth():
                 data.append(
                     [
                         datetime.datetime.strftime(
                             datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                                 hour=0, minute=0, second=0, microsecond=0
@@ -338,20 +355,20 @@
                 "pluie",
                 "vent (rafales)",
                 "dir.",
                 "/!\\",
             ]
     if data != []:
         print("")
-        table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
+        table = columnar.columnar(data, headers, no_borders=pyweatherfr.args.compute_args().condensate, wrap_max=0, justify= 'l' if pyweatherfr.args.compute_args().nocolor else 'c')
         print(table)
         if not isFullWidth():
             print(
                 pyweatherfr.log.my_colored(
-                    "warning : pour + d'affichage, élargissez votre terminal", "yellow"
+                    "warning : pour plus de données, élargissez votre terminal et relancez la commande, ou utilisez l'option --f (affiche dégradé possible).", "yellow"
                 )
             )
 
 
 def previsions_courantes(ville, dpt, lat, long, tz):
     (
         current_temperature_2m,
@@ -456,21 +473,21 @@
                 [
                     "vent",
                     f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "
                     + direction,
                     "",
                 ]
             )
-        if w_soleil > 1000:
+        if w_soleil >= WARNING_WATTS:
             data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2", LUNETTES])
         else:
             data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2", ""])
         data.append(["temps", emojiweather + " " + current_weather, ""])
     print("")
-    table = columnar.columnar(data, no_borders=False, wrap_max=0)
+    table = columnar.columnar(data, no_borders=pyweatherfr.args.compute_args().condensate, wrap_max=0, justify= 'l' if pyweatherfr.args.compute_args().nocolor else 'c')
     print(table)
 
 
 def previsions_generiques(ville, dpt, lat, long, tz):
     (
         daily_temperature_2m_min,
         daily_temperature_2m_max,
@@ -522,49 +539,58 @@
     data = []
     fin = 3
     if pyweatherfr.args.compute_args().past != 0:
         fin = -1
     tronque = False
     for i in range(0, len(daily_precipitation_sum)):
         if not numpy.isnan(daily_precipitation_sum[i]):
+            nbw=0
             warning = ""
             pluie = f"{daily_precipitation_sum[i]:.1f}mm"
             if snowfall[i] >= WARNING_SNOW:
-                warning = warning + " " + SNOW
+                warning = warning + "  " + SNOW
+                nbw=nbw+1
             elif daily_precipitation_sum[i] >= WARNING_RAIN:
-                warning = warning + " " + RAIN
+                warning = warning + "  " + RAIN
+                nbw=nbw+1
             if isFullWidth():
                 temp = f"{daily_temperature_2m_min[i]:.1f}°C ({daily_apparent_temperature_min[i]:.1f}°C) -> {daily_temperature_2m_max[i]:.1f}°C ({daily_apparent_temperature_max[i]:.1f}°C)"
             else:
                 temp = f"{daily_temperature_2m_min[i]:.0f}°C -> {daily_temperature_2m_max[i]:.0f}°C"
             if (
                 daily_temperature_2m_min[i] <= WARNING_FROID
                 or daily_apparent_temperature_min[i] <= WARNING_FROID
                 or daily_temperature_2m_max[i] <= WARNING_FROID
                 or daily_apparent_temperature_max[i] <= WARNING_FROID
             ):
-                warning = warning + " " + COLD
+                warning = warning + "  " + COLD
+                nbw=nbw+1
             if (
                 daily_temperature_2m_min[i] >= WARNING_WARM
                 or daily_apparent_temperature_min[i] >= WARNING_WARM
                 or daily_temperature_2m_max[i] >= WARNING_WARM
                 or daily_apparent_temperature_max[i] >= WARNING_WARM
             ):
-                warning = warning + " " + WARM
+                warning = warning + "  " + WARM
+                nbw=nbw+1
             weather, emojiweather = traduction(weather_code[i], 1)
 
             vent = f"{daily_wind_speed_10m_max[i]:.0f}km/h ({daily_wind_gusts_10m_max[i]:.0f}km/h)"
             direction = calculer_direction(daily_wind_direction_10m_dominant[i])
 
             vent = vent
             if (
                 daily_wind_speed_10m_max[i] >= WARNING_WIND
                 or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST
             ):
-                warning = warning + " " + WIND
+                warning = warning + "  " + WIND
+                nbw=nbw+1
+            for i in range(nbw):  
+                warning = warning + " " 
+            warning = warning + " "    
             duree_pluie = f"{precipitation_hours[i]:.0f}h"
             duree_soleil = f"{sunshine_duration[i]/3600:.0f}h"
             if pyweatherfr.args.compute_args().nocolor:
                 if isFullWidth():
                     data.append(
                         [
                             datetime.datetime.strftime(
@@ -679,39 +705,39 @@
                     "temps",
                     "température (ressentie)",
                     "pluie",
                     "vent (rafales)",
                     "dir.",
                     "tps pluie",
                     "tps soleil",
-                    "",
+                    "/!\\",
                 ]
             else:
                 headers = [
                     "date",
                     "temps",
                     "température",
                     "pluie",
                     "vent (rafales)",
                     "dir.",
-                    "",
+                    "/!\\",
                 ]
 
         print("")
-        table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
+        table = columnar.columnar(data, headers, no_borders=pyweatherfr.args.compute_args().condensate, wrap_max=0, justify= 'l' if pyweatherfr.args.compute_args().nocolor else 'c')
         print(table)
         if not isFullWidth():
             print(
                 pyweatherfr.log.my_colored(
-                    "warning : pour + d'affichage, élargissez votre terminal", "yellow"
+                    "warning : pour plus de données, élargissez votre terminal et relancez la commande, ou utilisez l'option --f (affiche dégradé possible).", "yellow"
                 )
             )
 
     if tronque:
-        print(pyweatherfr.log.my_colored("warning : données tronquées", "yellow"))
+        print(pyweatherfr.log.my_colored("warning : données partiellement indisponibles.", "yellow"))
 
 
 def print_generic_data_town(ville, dpt, lat, long, alt, recap):
     print("")
     data = []
     if pyweatherfr.args.compute_args().nocolor:
         if (ville is None or ville == "") and (dpt is None or dpt == ""):
@@ -743,15 +769,15 @@
             [
                 BOUSSOLE,
                 f"lat.:  {float(lat):.4f}°  / long.: {float(long):.4f}° / alt.: {float(alt):.0f}m ",
             ]
         )
         data.append([PC, recap])
 
-    table = columnar.columnar(data, no_borders=False, wrap_max=0)
+    table = columnar.columnar(data, no_borders=pyweatherfr.args.compute_args().condensate, wrap_max=0, justify= 'l' if pyweatherfr.args.compute_args().nocolor else 'c')
 
     print(table)
     if ville=="Springfield" and "Oregon" in dpt and not pyweatherfr.args.compute_args().serious:
         art_ascii = "\
             |\/\/\/|\n\
             |      |\n\
             |      |\n\
@@ -778,62 +804,62 @@
 
 
 def obtain_city_data():
     parties = pyweatherfr.args.compute_args().town.split(",")
     if len(parties) > 2:
         print(
             pyweatherfr.log.my_colored(
-                "erreur : format incorrect : attendu 'ville, pays' ou 'ville'", "red"
+                "erreur : format incorrect : attendu 'ville, pays' ou 'ville'.", "red"
             )
         )
         exit(1)
     if len(parties) == 1 and pyweatherfr.args.compute_args().world == True:
         print(
             pyweatherfr.log.my_colored(
-                "warning : si la ville souhaitée ne s'affiche pas vous pouvez utiliser le format 'ville, pays' pour la recherche",
+                "warning : si la ville souhaitée ne s'affiche pas vous pouvez utiliser le format 'ville, pays' pour la recherche.",
                 "yellow",
             )
         )
     town = parties[0]
     others = ",".join(parties[1:])
     pyweatherfr.log.print_debug(town)
     pyweatherfr.log.print_debug(others)
     choix, world = pyweatherfr.openstreetmap.findcitybyopenstreetmap(town, others)
     if not pyweatherfr.args.compute_args().world and world:
         print("")
         print(
             pyweatherfr.log.my_colored(
-                "warning : il existe des villes hors France disponibles pour wotre recherche. Relancez la avec -w pour y acceder",
+                "warning : il existe des villes hors de France disponibles pour votre recherche. Relancez la commande avec -w pour y accéder.",
                 "yellow",
             )
         )
     if len(choix) == 1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
         country = choice[3]
         lat = choice[4]
         long = choice[5]
         return ville, dpt, lat, long, country
     elif len(choix) == 0:
-        print(pyweatherfr.log.my_colored("erreur : aucune ville trouvée", "red"))
+        print(pyweatherfr.log.my_colored("erreur : aucune ville trouvée.", "red"))
         exit(1)
     else:
         while True:
             i = 0
             for choice in choix:
                 i = i + 1
                 print("[" + str(i) + "] " + choice[1] + " (" + choice[2] + ")")
             print("[0] pour quitter")
             answer = input("Quelle ville? ")
             if answer.isnumeric() and int(answer) == 0:
                 exit(0)
             if answer.isnumeric() and 1 <= int(answer) <= len(choix):
                 break
-            print(pyweatherfr.log.my_colored("erreur : choix incorrect", "red"))
+            print(pyweatherfr.log.my_colored("erreur : choix incorrect.", "red"))
         choice = choix[int(answer) - 1]
         ville = choice[1]
         dpt = choice[2]
         country = choice[3]
         lat = choice[4]
         long = choice[5]
     return ville, dpt, lat, long, country
@@ -841,15 +867,15 @@
 
 def diff_jour(long, lat):
     tz = timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
     if not pyweatherfr.args.compute_args().date is None:
         if not est_format_date(pyweatherfr.args.compute_args().date):
             print(
                 pyweatherfr.log.my_colored(
-                    "erreur : format date invalide, format attendu yyyy-mm-dd", "red"
+                    "erreur : format date invalide, format attendu yyyy-mm-dd.", "red"
                 )
             )
             exit(1)
         diff = (
             pytz.timezone(tz).localize(
                 datetime.datetime.strptime(
                     pyweatherfr.args.compute_args().date, "%Y-%m-%d"
@@ -857,24 +883,24 @@
             )
             - datetime.datetime.now(tz=pytz.timezone(tz))
         ).days + 1
         pyweatherfr.log.print_debug(str(diff) + " jours")
         if diff >= 15:
             print(
                 pyweatherfr.log.my_colored(
-                    "erreur : date invalide (limitée à +14 jour de la date actuelle)",
+                    "erreur : date invalide (limitée à +14 jour de la date actuelle).",
                     "red",
                 )
             )
             exit(1)
         return diff
     if pyweatherfr.args.compute_args().jour >= 15:
         print(
             pyweatherfr.log.my_colored(
-                "erreur : date invalide (limitée à +14 jour de la date actuelle)", "red"
+                "erreur : date invalide (limitée à +14 jour de la date actuelle).", "red"
             )
         )
         exit(1)
     return pyweatherfr.args.compute_args().jour
 
 
 def est_format_date(chaine):
```

### Comparing `pyweatherfr-5.3.4/pyweatherfr/args.py` & `pyweatherfr-5.3.5/pyweatherfr/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,20 @@
     )
     my_parser.add_argument(
         "--serious",
         action="store_true",
         help="retire les easters eggs (dommage)",
     )
     my_parser.add_argument(
+        "-c",
+        "--condensate",
+        action="store_true",
+        help="condense la sortie",
+    )    
+    my_parser.add_argument(
         "-f",
         "--fullwidth",
         action="store_true",
         help="force l'affichage de toutes les données",
     )
     my_parser.add_argument(
         "-l",
```

### Comparing `pyweatherfr-5.3.4/pyweatherfr/meteofrance.py` & `pyweatherfr-5.3.5/pyweatherfr/meteofrance.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.4/pyweatherfr/openstreetmap.py` & `pyweatherfr-5.3.5/pyweatherfr/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.3.4/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.3.5/pyweatherfr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.3.4
+Version: 5.3.5
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.3.4/setup.py` & `pyweatherfr-5.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.3.4",
+    version="5.3.5",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

