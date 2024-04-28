# Comparing `tmp/mixvideoconcat-1.0.0.tar.gz` & `tmp/mixvideoconcat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixvideoconcat-1.0.0.tar", last modified: Tue Apr 23 22:08:18 2024, max compression
+gzip compressed data, was "mixvideoconcat-1.1.0.tar", last modified: Sun Apr 28 00:06:54 2024, max compression
```

## Comparing `mixvideoconcat-1.0.0.tar` & `mixvideoconcat-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:08:18.255005 mixvideoconcat-1.0.0/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-04-23 19:28:35.000000 mixvideoconcat-1.0.0/LICENSE
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    43618 2024-04-23 22:08:18.255005 mixvideoconcat-1.0.0/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1845 2024-04-23 21:17:06.000000 mixvideoconcat-1.0.0/README.md
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1397 2024-04-23 22:08:13.000000 mixvideoconcat-1.0.0/pyproject.toml
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-04-23 22:08:18.255005 mixvideoconcat-1.0.0/setup.cfg
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:08:18.255005 mixvideoconcat-1.0.0/src/
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:08:18.255005 mixvideoconcat-1.0.0/src/mixvideoconcat/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1728 2024-04-23 21:02:32.000000 mixvideoconcat-1.0.0/src/mixvideoconcat/__init__.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     7391 2024-04-23 21:11:28.000000 mixvideoconcat-1.0.0/src/mixvideoconcat/concat.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-04-23 21:00:36.000000 mixvideoconcat-1.0.0/src/mixvideoconcat/log.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:08:18.255005 mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    43618 2024-04-23 22:08:18.000000 mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      331 2024-04-23 22:08:18.000000 mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/SOURCES.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-04-23 22:08:18.000000 mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/dependency_links.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       55 2024-04-23 22:08:18.000000 mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/entry_points.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       15 2024-04-23 22:08:18.000000 mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/top_level.txt
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-04-23 19:28:35.000000 mixvideoconcat-1.1.0/LICENSE
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    43710 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1845 2024-04-23 21:17:06.000000 mixvideoconcat-1.1.0/README.md
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1481 2024-04-28 00:05:28.000000 mixvideoconcat-1.1.0/pyproject.toml
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/setup.cfg
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.935247 mixvideoconcat-1.1.0/src/
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.983247 mixvideoconcat-1.1.0/src/mixvideoconcat/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     3187 2024-04-26 18:47:18.000000 mixvideoconcat-1.1.0/src/mixvideoconcat/__init__.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     8475 2024-04-26 19:19:15.000000 mixvideoconcat-1.1.0/src/mixvideoconcat/concat.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-04-23 21:00:36.000000 mixvideoconcat-1.1.0/src/mixvideoconcat/log.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-28 00:06:54.991247 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    43710 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      331 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       55 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/entry_points.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       15 2024-04-28 00:06:54.000000 mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/top_level.txt
```

### Comparing `mixvideoconcat-1.0.0/LICENSE` & `mixvideoconcat-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mixvideoconcat-1.0.0/PKG-INFO` & `mixvideoconcat-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixvideoconcat
-Version: 1.0.0
+Version: 1.1.0
 Summary: Mixed videos concatenator
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -678,14 +678,15 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/sashacmc/mixvideoconcat
 Project-URL: Bug Reports, https://github.com/sashacmc/mixvideoconcat/issues
 Project-URL: Source, https://github.com/sashacmc/mixvideoconcat/
+Project-URL: Changelog, https://github.com/sashacmc/mixvideoconcat/blob/master/CHANGELOG.md
 Keywords: video,concatenate,tool,ffmpeg
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mixvideoconcat-1.0.0/README.md` & `mixvideoconcat-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mixvideoconcat-1.0.0/pyproject.toml` & `mixvideoconcat-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mixvideoconcat"
-version = "1.0.0"
+version = "1.1.0"
 description = "Mixed videos concatenator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["video", "concatenate", "tool", "ffmpeg"]
 
 authors = [
@@ -43,10 +43,11 @@
 dependencies = [
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sashacmc/mixvideoconcat"
 "Bug Reports" = "https://github.com/sashacmc/mixvideoconcat/issues"
 "Source" = "https://github.com/sashacmc/mixvideoconcat/"
+"Changelog" = "https://github.com/sashacmc/mixvideoconcat/blob/master/CHANGELOG.md"
 
 [project.scripts]
 mixvideoconcat = "mixvideoconcat:main"
```

### Comparing `mixvideoconcat-1.0.0/src/mixvideoconcat/concat.py` & `mixvideoconcat-1.1.0/src/mixvideoconcat/concat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=line-too-long
+# pylint: disable=line-too-long,too-many-arguments,too-many-locals
 """
 MixVideoConcat Module
 
 This module provides functions for manipulating and concatenating video files.
 """
 
 import os
@@ -23,137 +23,142 @@
 
 
 def get_video_info(filename):
     """
     Retrieve information about a video file.
     """
     command = [
-        'ffprobe',
-        '-v',
-        'error',
-        '-show_format',
-        '-show_streams',
-        '-print_format',
-        'json',
+        "ffprobe",
+        "-v",
+        "error",
+        "-show_format",
+        "-show_streams",
+        "-print_format",
+        "json",
         filename,
     ]
     result = subprocess.run(
         command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False
     )
     if result.returncode != 0:
-        error_msg = result.stderr.decode('utf-8').strip()
+        error_msg = result.stderr.decode("utf-8").strip()
         raise SystemError(error_msg)
 
-    output = result.stdout.decode('utf-8')
+    output = result.stdout.decode("utf-8")
     data = json.loads(output)
 
     video_stream = next(
         (
             stream
-            for stream in data['streams']
-            if stream['codec_type'] == 'video'
+            for stream in data["streams"]
+            if stream["codec_type"] == "video"
         ),
         None,
     )
     if video_stream is None:
         raise RuntimeWarning("File has no video steam")
 
     info = {
-        "width": int(video_stream.get('width', 0)),
-        "height": int(video_stream.get('height', 0)),
-        "duration": float(data['format']['duration']),
+        "width": int(video_stream.get("width", 0)),
+        "height": int(video_stream.get("height", 0)),
+        "duration": float(data["format"]["duration"]),
         "orientation": int(
-            video_stream.get('side_data_list', [{}])[0].get('rotation', 0)
+            video_stream.get("side_data_list", [{}])[0].get("rotation", 0)
         ),
         "interlaced": (
-            video_stream.get('field_order', 'unknown') != "progressive"
+            video_stream.get("field_order", "unknown") != "progressive"
         ),
     }
     logging.info("%s: %s", filename, info)
     return info
 
 
-def apply_video_filters(in_file, out_file, filters, add_params=None):
+def apply_video_filters(
+    in_file, out_file, filters, add_params=None, verbose=False
+):
     """
     Apply filters to a video file.
     """
     cmd = [FFMPEG_BINARY, "-y"]  # overwrite existing
     cmd += ("-i", in_file)  # input file
     cmd += ("-vf", ",".join(filters))  # filters
     if out_file is None:
         cmd += ("-f", "null", "-")
     else:
         cmd += ("-qp", "0")  # lossless
         cmd += ("-preset", "ultrafast")  # maimum speed, big file
-        cmd += ("-acodec", "copy")  # copy audio as is
+        cmd += ("-c:a", "flac")  # copy audio as flac to keep quality
         cmd += ("-c:v", FFMPEG_CODEC)  # video codec
         if add_params is not None:
             cmd += add_params
         cmd += (out_file,)
     logging.debug(cmd)
-    res = subprocess.run(cmd, check=False).returncode
-    if res != 0:
-        raise SystemError(f"apply_video_filters failed: {res}")
+    errout = None if verbose else subprocess.PIPE
+    result = subprocess.run(cmd, stderr=errout, check=False)
+    if result.returncode != 0:
+        if not verbose:
+            logging.error(result.stderr.decode("utf-8"))
+        raise SystemError(f"apply_video_filters failed: {result.returncode}")
 
 
-def deinterlace(in_file, out_file):
+def deinterlace(in_file, out_file, verbose):
     """
     Deinterlace a video file.
     """
     filters = [
         "yadif",
         "format=yuv420p",
     ]
     logging.info("start deinterlace")
-    apply_video_filters(in_file, out_file, filters)
+    apply_video_filters(in_file, out_file, filters, None, verbose)
 
 
-def stabilize(in_file, out_file, tmpdirname):
+def stabilize(in_file, out_file, tmpdirname, verbose):
     """
     Stabilize a video file.
     """
-    trffile = os.path.join(tmpdirname, 'transforms.txt')
+    trffile = os.path.join(tmpdirname, "transforms.txt")
     try:
         filters = [
             f"vidstabdetect=stepsize=32:shakiness=10:accuracy=10:result={trffile}",  # noqa
         ]
         logging.info("start stab prep")
-        apply_video_filters(in_file, None, filters)
+        apply_video_filters(in_file, None, filters, None, verbose)
 
         filters = [
             f"vidstabtransform=input={trffile}:zoom=0:smoothing=10,unsharp=5:5:0.8:3:3:0.4",  # noqa
         ]
         logging.info("start stab")
-        apply_video_filters(in_file, out_file, filters)
+        apply_video_filters(in_file, out_file, filters, None, verbose)
     finally:
         __unlink(trffile)
 
 
-def resize_and_resample(in_file, out_file, w, h):
+def resize_and_resample(in_file, out_file, w, h, verbose):
     """
     Resize and resample a video file.
     """
     filters = [
         "format=yuv420p",
         f"scale=w='if(gt(a,{w}/{h}),{w},trunc(oh*a/2)*2)':h='if(gt(a,{w}/{h}),trunc(ow/a/2)*2,{h})'",  # noqa
         f"pad={w}:{h}:(ow-iw)/2:(oh-ih)/2:black",
     ]
     add_params = ["-r", REENCODE_FPS]
     logging.info("start resize")
-    apply_video_filters(in_file, out_file, filters, add_params)
+    apply_video_filters(in_file, out_file, filters, add_params, verbose)
 
 
-def concat_uniform(filenames, out_file, tmpdirname):
+def concat_uniform(filenames, out_file, tmpdirname, verbose):
     """
     Concatenate video files with uniform properties into a single video file.
     """
     if len(filenames) == 0:
         logging.warning("empty filenames list")
         return
-    listfile = os.path.join(tmpdirname, 'list.txt')
+    listfile = os.path.join(tmpdirname, "list.txt")
     with open(listfile, "w", encoding="utf-8") as f:
         for fname in filenames:
             f.write(f"file '{fname}'\n")
 
     cmd = [FFMPEG_BINARY, "-y"]  # overwrite existing
     cmd += ("-f", "concat")
     cmd += ("-safe", "0")
@@ -169,17 +174,20 @@
     cmd += ("-q:a", "1")  # sets the highest quality for the audio.
     cmd += ("-ac", "2")  # rematrixes audio to stereo.
     cmd += ("-ar", "48000")  # resamples audio to 48000 Hz.
     cmd += (out_file,)
     logging.info("start concatenate")
     logging.debug(cmd)
     try:
-        res = subprocess.run(cmd, check=False).returncode
-        if res != 0:
-            raise SystemError(f"concatenate failed: {res}")
+        errout = None if verbose else subprocess.PIPE
+        result = subprocess.run(cmd, stderr=errout, check=False)
+        if result.returncode != 0:
+            if not verbose:
+                logging.error(result.stderr.decode("utf-8"))
+            raise SystemError(f"concatenate failed: {result.returncode}")
         logging.info("file saved: %s", out_file)
     finally:
         __unlink(listfile)
 
 
 def __get_info_and_size(filenames):
     max_height = 0
@@ -198,22 +206,34 @@
         fileinfos.append(info)
 
     logging.info("Result video: width=%s, height=%s", max_width, max_height)
 
     return fileinfos, max_width, max_height
 
 
-def concat(filenames, outputfile, tmpdirname="/tmp", dry_run=False):
+def concat(
+    filenames,
+    outputfile,
+    tmpdirname="/tmp",
+    deinterlace_mode=None,
+    stabilize_mode=True,
+    verbose=False,
+    dry_run=False,
+):
     """
     Concatenate video files into a single video file.
 
     Args:
         filenames (list of str): List of paths to the input video files.
         outputfile (str): Path to the output concatenated video file.
         tmpdirname (str, optional): Directory for temporary files. Defaults to "/tmp".
+        deinterlace_mode (bool, optional): Enable video deinterlace,
+            if None interlacing will be detected by ffprobe.
+        stabilize_mode (bool, optional): Enable video stabilization.
+        verbose (bool, optional): Enable ffmpeg output.
         dry_run (bool, optional): If True, performs a dry run without actually
             concatenating the videos. Defaults to False.
 
     Returns:
         list: Information about the concatenated video files.
     """
     fileinfos, max_width, max_height = __get_info_and_size(filenames)
@@ -227,27 +247,33 @@
         for i, finfo in enumerate(fileinfos):
             fname = os.path.join(tmpdirname, f"{i}.mp4")
             tfname = os.path.join(tmpdirname, f"{i}_tmp.mp4")
             src_name = finfo["name"]
 
             logging.info("convert '%s' to '%s'", src_name, fname)
 
-            if finfo["interlaced"]:
-                deinterlace(src_name, tfname)
+            if deinterlace_mode is None:
+                deinterlace_mode = finfo["interlaced"]
+            if deinterlace_mode:
+                deinterlace(src_name, tfname, verbose)
                 os.rename(tfname, fname)
                 src_name = fname
 
-            stabilize(src_name, tfname, tmpdirname)
-            os.rename(tfname, fname)
+            if stabilize_mode:
+                stabilize(src_name, tfname, tmpdirname, verbose)
+                os.rename(tfname, fname)
+                src_name = fname
 
-            resize_and_resample(fname, tfname, max_width, max_height)
+            resize_and_resample(
+                src_name, tfname, max_width, max_height, verbose
+            )
             os.rename(tfname, fname)
 
             tmpfilenames.append(fname)
 
-        concat_uniform(tmpfilenames, outputfile, tmpdirname)
+        concat_uniform(tmpfilenames, outputfile, tmpdirname, verbose)
 
     finally:
         for f in tmpfilenames:
             __unlink(f)
 
     return fileinfos
```

### Comparing `mixvideoconcat-1.0.0/src/mixvideoconcat/log.py` & `mixvideoconcat-1.1.0/src/mixvideoconcat/log.py`

 * *Files identical despite different names*

### Comparing `mixvideoconcat-1.0.0/src/mixvideoconcat.egg-info/PKG-INFO` & `mixvideoconcat-1.1.0/src/mixvideoconcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixvideoconcat
-Version: 1.0.0
+Version: 1.1.0
 Summary: Mixed videos concatenator
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -678,14 +678,15 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/sashacmc/mixvideoconcat
 Project-URL: Bug Reports, https://github.com/sashacmc/mixvideoconcat/issues
 Project-URL: Source, https://github.com/sashacmc/mixvideoconcat/
+Project-URL: Changelog, https://github.com/sashacmc/mixvideoconcat/blob/master/CHANGELOG.md
 Keywords: video,concatenate,tool,ffmpeg
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

