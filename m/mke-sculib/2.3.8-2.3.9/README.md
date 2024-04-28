# Comparing `tmp/mke_sculib-2.3.8.tar.gz` & `tmp/mke_sculib-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.3.8.tar", last modified: Thu Oct 19 14:16:10 2023, max compression
+gzip compressed data, was "mke_sculib-2.3.9.tar", last modified: Thu Oct 19 14:37:28 2023, max compression
```

## Comparing `mke_sculib-2.3.8.tar` & `mke_sculib-2.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-10-19 14:16:10.618616 mke_sculib-2.3.8/
--rw-rw-rw-   0        0        0     4120 2023-10-19 14:16:10.619617 mke_sculib-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-10-12 09:31:00.000000 mke_sculib-2.3.8/README.rst
--rw-rw-rw-   0        0        0      921 2023-10-19 14:16:10.620782 mke_sculib-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0      359 2023-10-12 09:31:00.000000 mke_sculib-2.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-19 14:16:10.537080 mke_sculib-2.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-10-19 14:16:10.576988 mke_sculib-2.3.8/src/mke_sculib/
--rw-rw-rw-   0        0        0       21 2023-10-19 14:15:23.000000 mke_sculib-2.3.8/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1532 2023-10-12 09:31:00.000000 mke_sculib-2.3.8/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-10-12 09:31:00.000000 mke_sculib-2.3.8/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-10-12 09:31:00.000000 mke_sculib-2.3.8/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    28063 2023-10-19 14:14:27.000000 mke_sculib-2.3.8/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    87923 2023-10-14 18:20:15.000000 mke_sculib-2.3.8/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19534 2023-10-12 09:31:00.000000 mke_sculib-2.3.8/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9892 2023-10-17 06:37:38.000000 mke_sculib-2.3.8/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2023-10-19 14:16:10.604289 mke_sculib-2.3.8/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2023-10-19 14:16:10.000000 mke_sculib-2.3.8/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-10-19 14:16:10.000000 mke_sculib-2.3.8/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-19 14:16:10.000000 mke_sculib-2.3.8/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-10-19 14:16:10.000000 mke_sculib-2.3.8/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-19 14:16:10.604289 mke_sculib-2.3.8/tests/
--rw-rw-rw-   0        0        0    10521 2023-10-19 14:10:42.000000 mke_sculib-2.3.8/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2486 2023-10-19 12:08:52.000000 mke_sculib-2.3.8/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2023-10-19 14:37:28.255164 mke_sculib-2.3.9/
+-rw-rw-rw-   0        0        0     4120 2023-10-19 14:37:28.255164 mke_sculib-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-10-12 09:31:00.000000 mke_sculib-2.3.9/README.rst
+-rw-rw-rw-   0        0        0      921 2023-10-19 14:37:28.260629 mke_sculib-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      359 2023-10-12 09:31:00.000000 mke_sculib-2.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-19 14:37:28.188380 mke_sculib-2.3.9/src/
+drwxrwxrwx   0        0        0        0 2023-10-19 14:37:28.220889 mke_sculib-2.3.9/src/mke_sculib/
+-rw-rw-rw-   0        0        0       21 2023-10-19 14:37:09.000000 mke_sculib-2.3.9/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1532 2023-10-12 09:31:00.000000 mke_sculib-2.3.9/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-10-12 09:31:00.000000 mke_sculib-2.3.9/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-10-12 09:31:00.000000 mke_sculib-2.3.9/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    28063 2023-10-19 14:14:27.000000 mke_sculib-2.3.9/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    88067 2023-10-19 14:36:59.000000 mke_sculib-2.3.9/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19534 2023-10-12 09:31:00.000000 mke_sculib-2.3.9/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9892 2023-10-17 06:37:38.000000 mke_sculib-2.3.9/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2023-10-19 14:37:28.248032 mke_sculib-2.3.9/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2023-10-19 14:37:27.000000 mke_sculib-2.3.9/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-10-19 14:37:27.000000 mke_sculib-2.3.9/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-19 14:37:27.000000 mke_sculib-2.3.9/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-10-19 14:37:27.000000 mke_sculib-2.3.9/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-19 14:37:28.253160 mke_sculib-2.3.9/tests/
+-rw-rw-rw-   0        0        0    10521 2023-10-19 14:10:42.000000 mke_sculib-2.3.9/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2486 2023-10-19 12:08:52.000000 mke_sculib-2.3.9/tests/test_scu.py
```

### Comparing `mke_sculib-2.3.8/PKG-INFO` & `mke_sculib-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.3.8
+Version: 2.3.9
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.3.8/README.rst` & `mke_sculib-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/setup.cfg` & `mke_sculib-2.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.3.9/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.3.9/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib/helpers.py` & `mke_sculib-2.3.9/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.3.9/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib/scu.py` & `mke_sculib-2.3.9/src/mke_sculib/scu.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,29 +285,33 @@
 
         angle_min, angle_max, speed_max = self.lims_el
         el_pos = limit('el_pos', el_pos, angle_min, angle_max)
         el_speed = limit('el_speed', el_speed, 1e-10, speed_max)
         return az_pos, el_pos, az_speed, el_speed
 
 
+    def _limit_len(self, s):
+        return s[:97].replace('\n', '') + '...' if len(s) > 100 else s
     #Direct SCU webapi functions based on urllib PUT/GET
     def _feedback(self, r):
         if self.debug == True:
-            log('***Feedback:' +  str(r.request.url) + ' ' + str(r.request.body))
+
+            log('***Feedback:' +  str(r.request.url))# + ' ' + str(r.request.body))
             log(f'{r.status_code}: {r.reason}')
             log("***Text returned:")
-            log(r.text)
+            log(self._limit_len(r.text))
         elif r.status_code != 200:
-            log('***Feedback:' +  str(r.request.url) + ' ' + str(r.request.body), color=colors.WARNING)
+            log('***Feedback:' +  str(r.request.url))# + ' ' + str(r.request.body), color=colors.WARNING)
             log(f'{r.status_code}: {r.reason}', color=colors.WARNING)
             log("***Text returned:", color=colors.WARNING)
-            log(r.text, color=colors.WARNING)
+            log(self._limit_len(r.text), color=colors.WARNING)
             #log(r.reason, r.status_code)
             #log()
 
+
     #	def scu_get(device, params = {}, r_ip = self.ip, r_port = port):
     def scu_get(self, device, params = {}):
         '''This is a generic GET command into http: scu port + folder 
         with params=payload'''
         URL = 'http://' + self.ip + ':' + self.port + device
         if device != '/devices/statusValue':
             self.event_log[datetime.datetime.utcnow()] = 'GET | ' + device
```

### Comparing `mke_sculib-2.3.8/src/mke_sculib/sim.py` & `mke_sculib-2.3.9/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.3.9/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.3.9/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.3.8
+Version: 2.3.9
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.3.8/tests/test_acu_sim.py` & `mke_sculib-2.3.9/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.3.8/tests/test_scu.py` & `mke_sculib-2.3.9/tests/test_scu.py`

 * *Files identical despite different names*

