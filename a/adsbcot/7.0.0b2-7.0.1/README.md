# Comparing `tmp/adsbcot-7.0.0b2.tar.gz` & `tmp/adsbcot-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsbcot-7.0.0b2.tar", last modified: Wed Jan 17 23:07:19 2024, max compression
+gzip compressed data, was "adsbcot-7.0.1.tar", last modified: Sun Apr 28 21:08:16 2024, max compression
```

## Comparing `adsbcot-7.0.0b2.tar` & `adsbcot-7.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:07:19.709254 adsbcot-7.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-01-17 23:07:19.709254 adsbcot-7.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:07:19.709254 adsbcot-7.0.0b2/adsbcot/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/adsbcot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/adsbcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/adsbcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/adsbcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/adsbcot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:07:19.709254 adsbcot-7.0.0b2/adsbcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-01-17 23:07:19.000000 adsbcot-7.0.0b2/adsbcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-17 23:07:19.000000 adsbcot-7.0.0b2/adsbcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 23:07:19.000000 adsbcot-7.0.0b2/adsbcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-17 23:07:19.000000 adsbcot-7.0.0b2/adsbcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-17 23:07:19.000000 adsbcot-7.0.0b2/adsbcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-17 23:07:19.000000 adsbcot-7.0.0b2/adsbcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-17 23:07:19.713254 adsbcot-7.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:07:19.709254 adsbcot-7.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-01-17 23:07:10.000000 adsbcot-7.0.0b2/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:08:16.704174 adsbcot-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-28 21:08:05.000000 adsbcot-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 21:08:05.000000 adsbcot-7.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-28 21:08:16.704174 adsbcot-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-28 21:08:05.000000 adsbcot-7.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:08:16.700174 adsbcot-7.0.1/adsbcot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-28 21:08:05.000000 adsbcot-7.0.1/adsbcot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-04-28 21:08:05.000000 adsbcot-7.0.1/adsbcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-28 21:08:05.000000 adsbcot-7.0.1/adsbcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-28 21:08:05.000000 adsbcot-7.0.1/adsbcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-28 21:08:05.000000 adsbcot-7.0.1/adsbcot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:08:16.704174 adsbcot-7.0.1/adsbcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-28 21:08:16.000000 adsbcot-7.0.1/adsbcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-28 21:08:16.000000 adsbcot-7.0.1/adsbcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:08:16.000000 adsbcot-7.0.1/adsbcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 21:08:16.000000 adsbcot-7.0.1/adsbcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-28 21:08:16.000000 adsbcot-7.0.1/adsbcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 21:08:16.000000 adsbcot-7.0.1/adsbcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-28 21:08:16.704174 adsbcot-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-28 21:08:05.000000 adsbcot-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:08:16.704174 adsbcot-7.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-28 21:08:05.000000 adsbcot-7.0.1/tests/test_functions.py
```

### Comparing `adsbcot-7.0.0b2/LICENSE` & `adsbcot-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adsbcot-7.0.0b2/PKG-INFO` & `adsbcot-7.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 7.0.0b2
-Summary: ADSBCOT: ADS-B to TAK Gateway
+Version: 7.0.1
+Summary: Software for monitoring and analyzing aviation surveillance data (ADS-B) via the Team Awareness Kit (TAK) ecosystem of products.
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
 Project-URL: GitHub: repo, https://github.com/snstac/adsbcot
@@ -59,14 +59,16 @@
 
 ADSBCOT is in active use today in a variety of missions.
 
 `Documentation is available here. <https://adsbcot.rtfd.io>`_
 
    Use ADS-B Aggregators? Check out my sister software `ADSBXCOT <https://adsbxcot.rtfd.io>`_.
 
+   Want a turn-key ADS-B to TAK Gateway? Check out `AirTAK <https://www.snstac.com/store/p/airtak-v1>`_.
+
 License
 =======
 
 Copyright Sensors & Signals LLC https://www.snstac.com
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `adsbcot-7.0.0b2/README.rst` & `adsbcot-7.0.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 ADSBCOT is in active use today in a variety of missions.
 
 `Documentation is available here. <https://adsbcot.rtfd.io>`_
 
    Use ADS-B Aggregators? Check out my sister software `ADSBXCOT <https://adsbxcot.rtfd.io>`_.
 
+   Want a turn-key ADS-B to TAK Gateway? Check out `AirTAK <https://www.snstac.com/store/p/airtak-v1>`_.
+
 License
 =======
 
 Copyright Sensors & Signals LLC https://www.snstac.com
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `adsbcot-7.0.0b2/adsbcot/__init__.py` & `adsbcot-7.0.1/adsbcot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #
 
 """ADS-B to TAK Gateway.
 
 :source: <https://github.com/snstac/adsbcot>
 """
 
-__version__ = "7.0.0-beta2"
+__version__ = "7.0.1"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright Sensors & Signals LLC https://www.snstac.com"
 __license__ = "Apache License, Version 2.0"
 
 # Python 3.6 test/build work-around:
 try:
     from .constants import (  # NOQA
```

### Comparing `adsbcot-7.0.0b2/adsbcot/classes.py` & `adsbcot-7.0.1/adsbcot/classes.py`

 * *Files identical despite different names*

### Comparing `adsbcot-7.0.0b2/adsbcot/commands.py` & `adsbcot-7.0.1/adsbcot/commands.py`

 * *Files identical despite different names*

### Comparing `adsbcot-7.0.0b2/adsbcot/constants.py` & `adsbcot-7.0.1/adsbcot/constants.py`

 * *Files identical despite different names*

### Comparing `adsbcot-7.0.0b2/adsbcot/functions.py` & `adsbcot-7.0.1/adsbcot/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,36 +221,40 @@
     contact.set("callsign", callsign)
 
     track: ET.Element = ET.Element("track")
     track.set("course", str(craft.get("trk", craft.get("track", "9999999.0"))))
     track.set("speed", aircot.functions.get_speed(craft.get("gs")))
 
     detail = ET.Element("detail")
+
+    # Remarks should always be the first sub-entity within the Detail entity.
+    remarks = ET.Element("remarks")
+    remarks_fields.append(f"{cot_host_id}")
+    _remarks = " ".join(list(filter(None, remarks_fields)))
+    remarks.text = _remarks
+    detail.append(remarks)
+
     detail.append(contact)
     detail.append(track)
     detail.append(aircotx)
 
     icon = known_craft.get("ICON")
     if icon:
         usericon = ET.Element("usericon")
         usericon.set("iconsetpath", icon)
         detail.append(usericon)
 
-    remarks = ET.Element("remarks")
-    remarks_fields.append(f"{cot_host_id}")
-    _remarks = " ".join(list(filter(None, remarks_fields)))
-    remarks.text = _remarks
-    detail.append(remarks)
-
     cot_d = {
         "lat": str(lat),
         "lon": str(lon),
         "ce": str(craft.get("nac_p", "9999999.0")),
         "le": str(craft.get("nac_v", "9999999.0")),
-        "hae": aircot.functions.get_hae(craft.get("alt_geom")),  # Multiply alt_geom by "Clarke 1880 (international foot)"
+        "hae": aircot.functions.get_hae(
+            craft.get("alt_geom")
+        ),  # Multiply alt_geom by "Clarke 1880 (international foot)"
         "uid": cot_uid,
         "cot_type": cot_type,
         "stale": cot_stale,
     }
     cot = pytak.gen_cot_xml(**cot_d)
     cot.set("access", config.get("COT_ACCESS", pytak.DEFAULT_COT_ACCESS))
 
@@ -267,11 +271,9 @@
     craft: dict,
     config: Union[SectionProxy, dict, None] = None,
     known_craft: Optional[dict] = None,
 ) -> Optional[bytes]:
     """Return CoT XML object as an XML string."""
     cot: Optional[ET.Element] = adsb_to_cot_xml(craft, config, known_craft)
     return (
-        b"\n".join([pytak.DEFAULT_XML_DECLARATION, ET.tostring(cot)])
-        if cot
-        else None
+        b"\n".join([pytak.DEFAULT_XML_DECLARATION, ET.tostring(cot)]) if cot else None
     )
```

### Comparing `adsbcot-7.0.0b2/adsbcot.egg-info/PKG-INFO` & `adsbcot-7.0.1/adsbcot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 7.0.0b2
-Summary: ADSBCOT: ADS-B to TAK Gateway
+Version: 7.0.1
+Summary: Software for monitoring and analyzing aviation surveillance data (ADS-B) via the Team Awareness Kit (TAK) ecosystem of products.
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
 Project-URL: GitHub: repo, https://github.com/snstac/adsbcot
@@ -59,14 +59,16 @@
 
 ADSBCOT is in active use today in a variety of missions.
 
 `Documentation is available here. <https://adsbcot.rtfd.io>`_
 
    Use ADS-B Aggregators? Check out my sister software `ADSBXCOT <https://adsbxcot.rtfd.io>`_.
 
+   Want a turn-key ADS-B to TAK Gateway? Check out `AirTAK <https://www.snstac.com/store/p/airtak-v1>`_.
+
 License
 =======
 
 Copyright Sensors & Signals LLC https://www.snstac.com
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `adsbcot-7.0.0b2/setup.cfg` & `adsbcot-7.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = adsbcot
 version = attr: adsbcot.__version__
 url = https://github.com/snstac/adsbcot
 project_urls = 
 	CI: GitHub Actions = https://github.com/snstac/adsbcot/actions
 	GitHub: issues = https://github.com/snstac/adsbcot/issues
 	GitHub: repo = https://github.com/snstac/adsbcot
-description = ADSBCOT: ADS-B to TAK Gateway
+description = Software for monitoring and analyzing aviation surveillance data (ADS-B) via the Team Awareness Kit (TAK) ecosystem of products.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 maintainer = Greg Albrecht <oss@undef.net>
 maintainer_email = oss@undef.net
 license = Apache 2.0
 license_files = LICENSE
 classifiers = 
@@ -68,11 +68,25 @@
 test = 
 	pytest-asyncio
 	pytest-cov
 	pylint
 	flake8
 	black
 
+[isort]
+profile = black
+
+[flake8]
+max-line-length = 88
+extend-ignore = E203, E704
+
+[pylint]
+max-line-length = 88
+
+[pycodestyle]
+ignore = E203
+max_line_length = 88
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `adsbcot-7.0.0b2/setup.py` & `adsbcot-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `adsbcot-7.0.0b2/tests/test_functions.py` & `adsbcot-7.0.1/tests/test_functions.py`

 * *Files identical despite different names*

