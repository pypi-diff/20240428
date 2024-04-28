# Comparing `tmp/pyviewer-1.4.0.tar.gz` & `tmp/pyviewer-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.4.0.tar", last modified: Tue Apr 23 16:50:55 2024, max compression
+gzip compressed data, was "pyviewer-1.4.1.tar", last modified: Sun Apr 28 19:40:40 2024, max compression
```

## Comparing `pyviewer-1.4.0.tar` & `pyviewer-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-04-23 16:50:41.000000 pyviewer-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-23 16:50:55.364974 pyviewer-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-23 16:50:41.000000 pyviewer-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (127)  3423528 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/MPLUSRounded1c-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/pyviewer/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/custom_ops/cuda_gl_interop.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    25971 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    71936 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/roboto_mono.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:50:55.364974 pyviewer-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-23 16:50:42.000000 pyviewer-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.604717 pyviewer-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-04-28 19:40:34.000000 pyviewer-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-28 19:40:40.600717 pyviewer-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-28 19:40:34.000000 pyviewer-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.600717 pyviewer-1.4.1/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)  3423528 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/MPLUSRounded1c-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.600717 pyviewer-1.4.1/pyviewer/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/custom_ops/cuda_gl_interop.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25971 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71936 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/roboto_mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.600717 pyviewer-1.4.1/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:40:40.604717 pyviewer-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-28 19:40:34.000000 pyviewer-1.4.1/setup.py
```

### Comparing `pyviewer-1.4.0/LICENSE` & `pyviewer-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/PKG-INFO` & `pyviewer-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.4.0
+Version: 1.4.1
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.4.0/README.md` & `pyviewer-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/MPLUSRounded1c-Medium.ttf` & `pyviewer-1.4.1/pyviewer/MPLUSRounded1c-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/custom_ops/cuda_gl_interop.cpp` & `pyviewer-1.4.1/pyviewer/custom_ops/cuda_gl_interop.cpp`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/custom_ops.py` & `pyviewer-1.4.1/pyviewer/custom_ops.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/gl_viewer.py` & `pyviewer-1.4.1/pyviewer/gl_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/imgui_themes.py` & `pyviewer-1.4.1/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/params.py` & `pyviewer-1.4.1/pyviewer/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import imgui
 from pyviewer.utils import enum_slider, combo_box_vals, slider_range_int, slider_range_float, strict_dataclass
-from typing import Tuple
+from typing import Tuple, Callable
 
 """ Small param wrappers for automatically creating UI widgets """
 
 class Param:
     def __init__(self, type, label: str, default_val, tooltip: str = None) -> None:
         self.type = type
         self.label = label
@@ -44,20 +44,21 @@
         super().__init__(type(default_val), label, default_val, tooltip)
         self.opts = list(valid_vals)
 
     def draw_widget(self):
         return combo_box_vals(self.label, self.opts, self.value)
 
 class EnumSliderParam(Param):
-    def __init__(self, label, default_val, valid_vals=(), tooltip: str = None) -> None:
+    def __init__(self, label, default_val, valid_vals=(), to_str: Callable[..., str] = str, tooltip: str = None) -> None:
         super().__init__(type(default_val), label, default_val, tooltip)
         self.opts = list(valid_vals)
+        self.to_str = to_str
 
     def draw_widget(self):
-        return enum_slider(self.label, self.opts, self.value)
+        return enum_slider(self.label, self.opts, self.value, self.to_str)
 
 class BoolParam(Param):
     def __init__(self, label, default_val: bool, tooltip: str = None) -> None:
         super().__init__(bool, label, default_val, tooltip)
     
     def draw_widget(self):
         return imgui.checkbox(self.label, self.value)
```

### Comparing `pyviewer-1.4.0/pyviewer/roboto_mono.ttf` & `pyviewer-1.4.1/pyviewer/roboto_mono.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/single_image_viewer.py` & `pyviewer-1.4.1/pyviewer/single_image_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/toolbar_viewer.py` & `pyviewer-1.4.1/pyviewer/toolbar_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer/utils.py` & `pyviewer-1.4.1/pyviewer/utils.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.0/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.4.1/pyviewer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.4.0
+Version: 1.4.1
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.4.0/setup.py` & `pyviewer-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # git push --delete origin tagname
 
 # Test package_data changes by manually starting
 # the publish workflow and checking the "Print whl contents" step,
 # or with: `rm -r build\ && pip wheel . && unzip -l pyviewer-*.whl`
 # (not same environment, but good first step)
 setup(name='pyviewer',
-    version='1.4.0',
+    version='1.4.1',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
```

