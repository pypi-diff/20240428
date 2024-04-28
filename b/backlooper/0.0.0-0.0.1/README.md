# Comparing `tmp/backlooper-0.0.0.tar.gz` & `tmp/backlooper-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backlooper-0.0.0.tar", last modified: Fri Apr 26 18:25:01 2024, max compression
+gzip compressed data, was "backlooper-0.0.1.tar", last modified: Sun Apr 28 11:18:34 2024, max compression
```

## Comparing `backlooper-0.0.0.tar` & `backlooper-0.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:25:00.992414 backlooper-0.0.0/
--rw-rw-rw-   0        0        0     1093 2024-04-26 18:23:12.000000 backlooper-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       43 2024-04-26 18:23:12.000000 backlooper-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1396 2024-04-26 18:25:00.992414 backlooper-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      877 2024-04-26 18:23:12.000000 backlooper-0.0.0/README.md
--rw-rw-rw-   0        0        0      110 2024-04-26 18:23:12.000000 backlooper-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      635 2024-04-26 18:25:00.992414 backlooper-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-26 18:23:12.000000 backlooper-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:25:00.820541 backlooper-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:25:00.929912 backlooper-0.0.0/src/backlooper/
--rw-rw-rw-   0        0        0        0 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/__init__.py
--rw-rw-rw-   0        0        0     5235 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/__main__.py
--rw-rw-rw-   0        0        0      634 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/_clicktrack.py
--rw-rw-rw-   0        0        0    14112 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/audio.py
--rw-rw-rw-   0        0        0      958 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/config.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:25:00.961163 backlooper-0.0.0/src/backlooper/samples/
--rw-rw-rw-   0        0        0    35440 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/samples/hi_hat.wav
--rw-rw-rw-   0        0        0    17986 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/session.py
--rw-rw-rw-   0        0        0     7544 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/striped_storage.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:25:00.976786 backlooper-0.0.0/src/backlooper/tests/
--rw-rw-rw-   0        0        0        0 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/tests/__init__.py
--rw-rw-rw-   0        0        0     7458 2024-04-26 18:23:12.000000 backlooper-0.0.0/src/backlooper/tests/test_striped_storage.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:25:00.992414 backlooper-0.0.0/src/backlooper.egg-info/
--rw-rw-rw-   0        0        0     1396 2024-04-26 18:25:00.000000 backlooper-0.0.0/src/backlooper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2024-04-26 18:25:00.000000 backlooper-0.0.0/src/backlooper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:25:00.000000 backlooper-0.0.0/src/backlooper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-26 18:25:00.000000 backlooper-0.0.0/src/backlooper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 18:25:00.000000 backlooper-0.0.0/src/backlooper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:33.995291 backlooper-0.0.1/
+-rw-rw-rw-   0        0        0     1093 2024-04-28 11:17:21.000000 backlooper-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-04-28 11:17:21.000000 backlooper-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1453 2024-04-28 11:18:33.993297 backlooper-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2024-04-28 11:17:21.000000 backlooper-0.0.1/README.md
+-rw-rw-rw-   0        0        0      110 2024-04-28 11:17:21.000000 backlooper-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      635 2024-04-28 11:18:33.998289 backlooper-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-28 11:17:21.000000 backlooper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:33.860571 backlooper-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:33.944831 backlooper-0.0.1/src/backlooper/
+-rw-rw-rw-   0        0        0        0 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/__init__.py
+-rw-rw-rw-   0        0        0     5235 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/__main__.py
+-rw-rw-rw-   0        0        0      634 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/_clicktrack.py
+-rw-rw-rw-   0        0        0    14112 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/audio.py
+-rw-rw-rw-   0        0        0      958 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/config.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:33.975693 backlooper-0.0.1/src/backlooper/samples/
+-rw-rw-rw-   0        0        0    35440 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/samples/hi_hat.wav
+-rw-rw-rw-   0        0        0    17986 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/session.py
+-rw-rw-rw-   0        0        0     7544 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/striped_storage.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:33.986726 backlooper-0.0.1/src/backlooper/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/tests/__init__.py
+-rw-rw-rw-   0        0        0     7458 2024-04-28 11:17:21.000000 backlooper-0.0.1/src/backlooper/tests/test_striped_storage.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:33.991287 backlooper-0.0.1/src/backlooper.egg-info/
+-rw-rw-rw-   0        0        0     1453 2024-04-28 11:18:33.000000 backlooper-0.0.1/src/backlooper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-04-28 11:18:33.000000 backlooper-0.0.1/src/backlooper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 11:18:33.000000 backlooper-0.0.1/src/backlooper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-28 11:18:33.000000 backlooper-0.0.1/src/backlooper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-28 11:18:33.000000 backlooper-0.0.1/src/backlooper.egg-info/top_level.txt
```

### Comparing `backlooper-0.0.0/LICENSE` & `backlooper-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/PKG-INFO` & `backlooper-0.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backlooper
-Version: 0.0.0
+Version: 0.0.1
 Summary: Backlooper.app is a looper that allows you to decide to loop a few bars after you played them
 Home-page: https://github.com/spmvg/backlooper_backend
 Author: Steven van Gemert
 Author-email: steven@vangemert.dev
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,18 +21,17 @@
 It is not necessary to hit "record" before playing a loop.
 Audio is always being recorded.
 The last few bars will be looped if you select a track at approximately the first beat of the next bar.
 
 For user documentation, please see [here](https://backlooper.app/docs/general).
 
 For developer documentation, please continue reading.
-More developer documentation is provided [here](TODO sphinx).
+More developer documentation is provided [here](https://backlooper.readthedocs.io/en/latest/).
 
-
-The frontend code is provided [here](TODO frontend code).
+The frontend code is provided [here](https://github.com/spmvg/backlooper_frontend).
 
 ## Development setup
 Install the backend locally:
 
 ```commandline
 python -m pip install -e .
 ```
```

### Comparing `backlooper-0.0.0/README.md` & `backlooper-0.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 It is not necessary to hit "record" before playing a loop.
 Audio is always being recorded.
 The last few bars will be looped if you select a track at approximately the first beat of the next bar.
 
 For user documentation, please see [here](https://backlooper.app/docs/general).
 
 For developer documentation, please continue reading.
-More developer documentation is provided [here](TODO sphinx).
+More developer documentation is provided [here](https://backlooper.readthedocs.io/en/latest/).
 
-
-The frontend code is provided [here](TODO frontend code).
+The frontend code is provided [here](https://github.com/spmvg/backlooper_frontend).
 
 ## Development setup
 Install the backend locally:
 
 ```commandline
 python -m pip install -e .
 ```
```

### Comparing `backlooper-0.0.0/setup.cfg` & `backlooper-0.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6163 6b6c 6f6f 7065 720d 0a76   = backlooper..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e30 0d0a  ersion = 0.0.0..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e31 0d0a  ersion = 0.0.1..
 00000030: 6175 7468 6f72 203d 2053 7465 7665 6e20  author = Steven 
 00000040: 7661 6e20 4765 6d65 7274 0d0a 6175 7468  van Gemert..auth
 00000050: 6f72 5f65 6d61 696c 203d 2073 7465 7665  or_email = steve
 00000060: 6e40 7661 6e67 656d 6572 742e 6465 760d  n@vangemert.dev.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2042  .description = B
 00000080: 6163 6b6c 6f6f 7065 722e 6170 7020 6973  acklooper.app is
 00000090: 2061 206c 6f6f 7065 7220 7468 6174 2061   a looper that a
```

### Comparing `backlooper-0.0.0/src/backlooper/__main__.py` & `backlooper-0.0.1/src/backlooper/__main__.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/_clicktrack.py` & `backlooper-0.0.1/src/backlooper/_clicktrack.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/audio.py` & `backlooper-0.0.1/src/backlooper/audio.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/config.py` & `backlooper-0.0.1/src/backlooper/config.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/samples/hi_hat.wav` & `backlooper-0.0.1/src/backlooper/samples/hi_hat.wav`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/session.py` & `backlooper-0.0.1/src/backlooper/session.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/striped_storage.py` & `backlooper-0.0.1/src/backlooper/striped_storage.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper/tests/test_striped_storage.py` & `backlooper-0.0.1/src/backlooper/tests/test_striped_storage.py`

 * *Files identical despite different names*

### Comparing `backlooper-0.0.0/src/backlooper.egg-info/PKG-INFO` & `backlooper-0.0.1/src/backlooper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backlooper
-Version: 0.0.0
+Version: 0.0.1
 Summary: Backlooper.app is a looper that allows you to decide to loop a few bars after you played them
 Home-page: https://github.com/spmvg/backlooper_backend
 Author: Steven van Gemert
 Author-email: steven@vangemert.dev
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,18 +21,17 @@
 It is not necessary to hit "record" before playing a loop.
 Audio is always being recorded.
 The last few bars will be looped if you select a track at approximately the first beat of the next bar.
 
 For user documentation, please see [here](https://backlooper.app/docs/general).
 
 For developer documentation, please continue reading.
-More developer documentation is provided [here](TODO sphinx).
+More developer documentation is provided [here](https://backlooper.readthedocs.io/en/latest/).
 
-
-The frontend code is provided [here](TODO frontend code).
+The frontend code is provided [here](https://github.com/spmvg/backlooper_frontend).
 
 ## Development setup
 Install the backend locally:
 
 ```commandline
 python -m pip install -e .
 ```
```

### Comparing `backlooper-0.0.0/src/backlooper.egg-info/SOURCES.txt` & `backlooper-0.0.1/src/backlooper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

