# Comparing `tmp/updrytwist-UpDryTwist-0.0.8.tar.gz` & `tmp/updrytwist-UpDryTwist-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "updrytwist-UpDryTwist-0.0.8.tar", last modified: Sat May  8 21:15:40 2021, max compression
+gzip compressed data, was "updrytwist-UpDryTwist-0.0.9.tar", last modified: Mon May 24 03:24:40 2021, max compression
```

## Comparing `updrytwist-UpDryTwist-0.0.8.tar` & `updrytwist-UpDryTwist-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2021-05-08 21:15:40.236934 updrytwist-UpDryTwist-0.0.8/
--rw-rw-rw-   0        0        0    35801 2021-05-02 19:31:13.000000 updrytwist-UpDryTwist-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1172 2021-05-08 21:15:40.236934 updrytwist-UpDryTwist-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      470 2021-05-03 01:45:59.000000 updrytwist-UpDryTwist-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2021-04-26 04:15:01.000000 updrytwist-UpDryTwist-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      642 2021-05-08 21:15:40.238935 updrytwist-UpDryTwist-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       73 2021-05-02 22:41:14.000000 updrytwist-UpDryTwist-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-08 21:15:40.225932 updrytwist-UpDryTwist-0.0.8/updrytwist/
--rw-rw-rw-   0        0        0       82 2021-05-08 21:10:53.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/__init__.py
--rw-rw-rw-   0        0        0     4231 2021-05-08 21:15:22.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/config.py
--rw-rw-rw-   0        0        0     5558 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/geolocate.py
--rw-rw-rw-   0        0        0     2296 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/mailer.py
--rw-rw-rw-   0        0        0     5950 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/mqttdriver.py
--rw-rw-rw-   0        0        0     1278 2021-05-07 19:31:51.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/music-test.py
--rw-rw-rw-   0        0        0     2917 2021-05-07 19:31:51.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/music.py
--rw-rw-rw-   0        0        0     9699 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.8/updrytwist/piwigo.py
-drwxrwxrwx   0        0        0        0 2021-05-08 21:15:40.234934 updrytwist-UpDryTwist-0.0.8/updrytwist_UpDryTwist.egg-info/
--rw-rw-rw-   0        0        0     1172 2021-05-08 21:15:40.000000 updrytwist-UpDryTwist-0.0.8/updrytwist_UpDryTwist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2021-05-08 21:15:40.000000 updrytwist-UpDryTwist-0.0.8/updrytwist_UpDryTwist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-08 21:15:40.000000 updrytwist-UpDryTwist-0.0.8/updrytwist_UpDryTwist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-05-08 21:15:40.000000 updrytwist-UpDryTwist-0.0.8/updrytwist_UpDryTwist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-05-24 03:24:40.672539 updrytwist-UpDryTwist-0.0.9/
+-rw-rw-rw-   0        0        0    35801 2021-05-02 19:31:13.000000 updrytwist-UpDryTwist-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1050 2021-05-24 03:24:40.672539 updrytwist-UpDryTwist-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2021-05-03 01:45:59.000000 updrytwist-UpDryTwist-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-04-26 04:15:01.000000 updrytwist-UpDryTwist-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      642 2021-05-24 03:24:40.674540 updrytwist-UpDryTwist-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       73 2021-05-02 22:41:14.000000 updrytwist-UpDryTwist-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-24 03:24:40.659536 updrytwist-UpDryTwist-0.0.9/updrytwist/
+-rw-rw-rw-   0        0        0       82 2021-05-24 03:24:18.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/__init__.py
+-rw-rw-rw-   0        0        0     4231 2021-05-08 21:15:22.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/config.py
+-rw-rw-rw-   0        0        0     6682 2021-05-23 18:24:38.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/filerotator.py
+-rw-rw-rw-   0        0        0     5558 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/geolocate.py
+-rw-rw-rw-   0        0        0     2296 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/mailer.py
+-rw-rw-rw-   0        0        0     6002 2021-05-23 21:26:01.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/mqttdriver.py
+-rw-rw-rw-   0        0        0     1278 2021-05-07 19:31:51.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/music-test.py
+-rw-rw-rw-   0        0        0     2917 2021-05-07 19:31:51.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/music.py
+-rw-rw-rw-   0        0        0     9699 2021-05-07 22:51:09.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/piwigo.py
+-rw-rw-rw-   0        0        0     4357 2021-05-23 21:33:09.000000 updrytwist-UpDryTwist-0.0.9/updrytwist/tkasync.py
+drwxrwxrwx   0        0        0        0 2021-05-24 03:24:40.670539 updrytwist-UpDryTwist-0.0.9/updrytwist_UpDryTwist.egg-info/
+-rw-rw-rw-   0        0        0     1050 2021-05-24 03:24:40.000000 updrytwist-UpDryTwist-0.0.9/updrytwist_UpDryTwist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2021-05-24 03:24:40.000000 updrytwist-UpDryTwist-0.0.9/updrytwist_UpDryTwist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-24 03:24:40.000000 updrytwist-UpDryTwist-0.0.9/updrytwist_UpDryTwist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2021-05-24 03:24:40.000000 updrytwist-UpDryTwist-0.0.9/updrytwist_UpDryTwist.egg-info/top_level.txt
```

### Comparing `updrytwist-UpDryTwist-0.0.8/LICENSE` & `updrytwist-UpDryTwist-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/PKG-INFO` & `updrytwist-UpDryTwist-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: updrytwist-UpDryTwist
-Version: 0.0.8
+Version: 0.0.9
 Summary: My common utilities
 Home-page: https://github.com/tathamg/updrytwist
 Author: Greg Tatham
 Author-email: tathamg@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/tathamg/updrytwist/issues
-Description: 
-        This project is a collection of the utilities that I use all the time in different projects,
-        most of which are around home automation-type activities, or kiosk screens, or tinkering
-        with a Raspberry Pi.  
-        
-        How to Install
-        --------------
-            pip install updrytwist
-        
-        How to Use
-        ----------
-        
-        Maybe at some point this will be filled in.  But for now, just read the source.
-        
-        Contact Information
-        -------------------
-        
-        Please contact through github (UpDryTwist).
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+This project is a collection of the utilities that I use all the time in different projects,
+most of which are around home automation-type activities, or kiosk screens, or tinkering
+with a Raspberry Pi.  
+
+How to Install
+--------------
+    pip install updrytwist
+
+How to Use
+----------
+
+Maybe at some point this will be filled in.  But for now, just read the source.
+
+Contact Information
+-------------------
+
+Please contact through github (UpDryTwist).
+
```

### Comparing `updrytwist-UpDryTwist-0.0.8/setup.cfg` & `updrytwist-UpDryTwist-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/config.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/config.py`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/geolocate.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/geolocate.py`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/mailer.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/mailer.py`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/mqttdriver.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/mqttdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,27 +144,28 @@
 
     def quitLoop ( self ) :
         self.keepLooping = False
         asyncio.run(MqttDriver.cancelTasks(self.tasks))
 
     async def messageLoop( self ):
 
+        self.keepLooping = True
         self.loop = asyncio.get_event_loop()
         while self.keepLooping:
             try:
                 await self.runListen()
             except asyncio.CancelledError:
                 self.keepLooping = False
+                await self.cancelTasks(self.tasks)
                 _LOGGER.info( f'Run loop was cancelled.  Exiting loop.')
             except MqttError as error:
                 _LOGGER.info( f'Error "{error}". Reconnecting in {self.reconnectSeconds} seconds.')
             finally:
                 if self.keepLooping:
                     await asyncio.sleep( self.reconnectSeconds )
         _LOGGER.info( f'Exiting the mqttdriver message loop')
 
     def getMessageLoop ( self ) :
         return self.loop
 
     def runMessageLoop ( self ) :
-        self.keepLooping = True
         asyncio.run( self.messageLoop(), debug=DEBUG_ASYNCIO )
```

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/music-test.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/music-test.py`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/music.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/music.py`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist/piwigo.py` & `updrytwist-UpDryTwist-0.0.9/updrytwist/piwigo.py`

 * *Files identical despite different names*

### Comparing `updrytwist-UpDryTwist-0.0.8/updrytwist_UpDryTwist.egg-info/PKG-INFO` & `updrytwist-UpDryTwist-0.0.9/updrytwist_UpDryTwist.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: updrytwist-UpDryTwist
-Version: 0.0.8
+Version: 0.0.9
 Summary: My common utilities
 Home-page: https://github.com/tathamg/updrytwist
 Author: Greg Tatham
 Author-email: tathamg@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/tathamg/updrytwist/issues
-Description: 
-        This project is a collection of the utilities that I use all the time in different projects,
-        most of which are around home automation-type activities, or kiosk screens, or tinkering
-        with a Raspberry Pi.  
-        
-        How to Install
-        --------------
-            pip install updrytwist
-        
-        How to Use
-        ----------
-        
-        Maybe at some point this will be filled in.  But for now, just read the source.
-        
-        Contact Information
-        -------------------
-        
-        Please contact through github (UpDryTwist).
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+This project is a collection of the utilities that I use all the time in different projects,
+most of which are around home automation-type activities, or kiosk screens, or tinkering
+with a Raspberry Pi.  
+
+How to Install
+--------------
+    pip install updrytwist
+
+How to Use
+----------
+
+Maybe at some point this will be filled in.  But for now, just read the source.
+
+Contact Information
+-------------------
+
+Please contact through github (UpDryTwist).
+
```

