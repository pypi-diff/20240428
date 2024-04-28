# Comparing `tmp/better-ffmpeg-progress-2.1.3.tar.gz` & `tmp/better-ffmpeg-progress-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\better-ffmpeg-progress-2.1.3.tar", last modified: Mon Apr 22 18:25:26 2024, max compression
+gzip compressed data, was "dist\better-ffmpeg-progress-2.1.4.tar", last modified: Sun Apr 28 16:12:35 2024, max compression
```

## Comparing `better-ffmpeg-progress-2.1.3.tar` & `better-ffmpeg-progress-2.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 18:25:26.000000 better-ffmpeg-progress-2.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-22 18:25:26.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress/
--rw-rw-rw-   0        0        0     6102 2024-04-22 18:09:02.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress/better_ffmpeg_progress.py
--rw-rw-rw-   0        0        0       50 2024-04-22 18:00:24.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 18:25:26.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-22 18:25:25.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     6168 2024-04-22 18:25:25.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-04-22 18:25:25.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/requires.txt
--rw-rw-rw-   0        0        0      339 2024-04-22 18:25:25.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       23 2024-04-22 18:25:25.000000 better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-08-29 21:18:31.000000 better-ffmpeg-progress-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     6168 2024-04-22 18:25:26.000000 better-ffmpeg-progress-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4583 2024-04-22 17:58:07.000000 better-ffmpeg-progress-2.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 18:25:26.000000 better-ffmpeg-progress-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-04-22 18:24:12.000000 better-ffmpeg-progress-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/
+-rw-rw-rw-   0        0        0     6098 2024-04-28 15:59:22.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/better_ffmpeg_progress.py
+-rw-rw-rw-   0        0        0       50 2024-04-22 18:00:24.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     6458 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      339 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       23 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-08-29 21:18:31.000000 better-ffmpeg-progress-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6458 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4801 2024-04-28 16:01:33.000000 better-ffmpeg-progress-2.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      808 2024-04-28 16:00:20.000000 better-ffmpeg-progress-2.1.4/setup.py
```

### Comparing `better-ffmpeg-progress-2.1.3/better_ffmpeg_progress/better_ffmpeg_progress.py` & `better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/better_ffmpeg_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                             self._estimated_size = self._current_size * (
                                 100 / self._percentage_progress
                             )
 
                 elif "speed" in ffmpeg_output:
                     speed_str = value[:-1]
 
-                    if speed_str != "0" and "N/A" not in speed_str:
+                    if speed_str != "0" and "N/A" not in value:
                         self._speed = float(speed_str)
 
                         if self._can_get_duration:
                             self._eta = (
                                 self._duration_secs - self._seconds_processed
                             ) / self._speed
```

### Comparing `better-ffmpeg-progress-2.1.3/better_ffmpeg_progress.egg-info/PKG-INFO` & `better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-ffmpeg-progress
-Version: 2.1.3
+Version: 2.1.4
 Summary: Run FFmpeg & see percentage progress + ETA.
 Home-page: https://github.com/CrypticSignal/better-ffmpeg-progress
 Author: GitHub.com/CrypticSignal
 Author-email: theaudiophile@outlook.com
 License: UNKNOWN
 Description: <div align="center">
         
@@ -117,14 +117,22 @@
         
         - [v2.1.0] [Update function name](https://github.com/CrypticSignal/better-ffmpeg-progress/commit/572fe8a0d71957d00b833134a4d35170630203fa) to fix `'process_complete_handler' is not defined` error.
         
         [05/11/2023]
         
         - [v2.1.2] [Do not exit the Python interpreter after the FFmpeg process is complete](https://github.com/CrypticSignal/better-ffmpeg-progress/commit/0a358810773835297faae688689c6e0d8a5859ae)
         
+        [22/04/2024]
+        
+        - [v2.1.3] Fix issue [#20](https://github.com/CrypticSignal/better-ffmpeg-progress/issues/20)
+        
+        [28/04/2024]
+        
+        - [v2.1.4] Fix issue [#21](https://github.com/CrypticSignal/better-ffmpeg-progress/issues/21)
+        
 Keywords: ffmpeg,progress
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `better-ffmpeg-progress-2.1.3/LICENSE` & `better-ffmpeg-progress-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `better-ffmpeg-progress-2.1.3/PKG-INFO` & `better-ffmpeg-progress-2.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-ffmpeg-progress
-Version: 2.1.3
+Version: 2.1.4
 Summary: Run FFmpeg & see percentage progress + ETA.
 Home-page: https://github.com/CrypticSignal/better-ffmpeg-progress
 Author: GitHub.com/CrypticSignal
 Author-email: theaudiophile@outlook.com
 License: UNKNOWN
 Description: <div align="center">
         
@@ -117,14 +117,22 @@
         
         - [v2.1.0] [Update function name](https://github.com/CrypticSignal/better-ffmpeg-progress/commit/572fe8a0d71957d00b833134a4d35170630203fa) to fix `'process_complete_handler' is not defined` error.
         
         [05/11/2023]
         
         - [v2.1.2] [Do not exit the Python interpreter after the FFmpeg process is complete](https://github.com/CrypticSignal/better-ffmpeg-progress/commit/0a358810773835297faae688689c6e0d8a5859ae)
         
+        [22/04/2024]
+        
+        - [v2.1.3] Fix issue [#20](https://github.com/CrypticSignal/better-ffmpeg-progress/issues/20)
+        
+        [28/04/2024]
+        
+        - [v2.1.4] Fix issue [#21](https://github.com/CrypticSignal/better-ffmpeg-progress/issues/21)
+        
 Keywords: ffmpeg,progress
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `better-ffmpeg-progress-2.1.3/README.md` & `better-ffmpeg-progress-2.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -108,7 +108,15 @@
 [07/02/2022]
 
 - [v2.1.0] [Update function name](https://github.com/CrypticSignal/better-ffmpeg-progress/commit/572fe8a0d71957d00b833134a4d35170630203fa) to fix `'process_complete_handler' is not defined` error.
 
 [05/11/2023]
 
 - [v2.1.2] [Do not exit the Python interpreter after the FFmpeg process is complete](https://github.com/CrypticSignal/better-ffmpeg-progress/commit/0a358810773835297faae688689c6e0d8a5859ae)
+
+[22/04/2024]
+
+- [v2.1.3] Fix issue [#20](https://github.com/CrypticSignal/better-ffmpeg-progress/issues/20)
+
+[28/04/2024]
+
+- [v2.1.4] Fix issue [#21](https://github.com/CrypticSignal/better-ffmpeg-progress/issues/21)
```

### Comparing `better-ffmpeg-progress-2.1.3/setup.py` & `better-ffmpeg-progress-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="better-ffmpeg-progress",
-    version="2.1.3",
+    version="2.1.4",
     author="GitHub.com/CrypticSignal",
     author_email="theaudiophile@outlook.com",
     description="Run FFmpeg & see percentage progress + ETA.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CrypticSignal/better-ffmpeg-progress",
     packages=["better_ffmpeg_progress"],
```

