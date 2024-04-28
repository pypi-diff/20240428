# Comparing `tmp/textalloc-0.1.1.tar.gz` & `tmp/textalloc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-0.1.1.tar", last modified: Sat Apr  6 15:46:30 2024, max compression
+gzip compressed data, was "textalloc-0.1.2.tar", last modified: Sun Apr 28 19:33:23 2024, max compression
```

## Comparing `textalloc-0.1.1.tar` & `textalloc-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:30.292714 textalloc-0.1.1/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.1.1/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8270 2024-04-06 15:46:30.282715 textalloc-0.1.1/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7607 2024-04-06 15:42:17.000000 textalloc-0.1.1/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-06 15:45:24.000000 textalloc-0.1.1/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-06 15:46:30.293716 textalloc-0.1.1/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:29.985719 textalloc-0.1.1/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:30.129719 textalloc-0.1.1/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    16415 2024-04-06 15:42:38.000000 textalloc-0.1.1/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-0.1.1/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-05 17:35:17.000000 textalloc-0.1.1/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-0.1.1/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-06 15:46:30.272716 textalloc-0.1.1/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8270 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-06 15:46:29.000000 textalloc-0.1.1/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:33:23.406339 textalloc-0.1.2/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.1.2/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8360 2024-04-28 19:33:23.396342 textalloc-0.1.2/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7697 2024-04-28 19:24:07.000000 textalloc-0.1.2/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-28 19:33:03.000000 textalloc-0.1.2/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-28 19:33:23.407338 textalloc-0.1.2/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:33:23.029106 textalloc-0.1.2/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:33:23.214106 textalloc-0.1.2/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    16607 2024-04-28 19:24:07.000000 textalloc-0.1.2/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-0.1.2/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-28 19:23:40.000000 textalloc-0.1.2/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-0.1.2/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:33:23.386336 textalloc-0.1.2/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8360 2024-04-28 19:33:22.000000 textalloc-0.1.2/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-28 19:33:23.000000 textalloc-0.1.2/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-28 19:33:22.000000 textalloc-0.1.2/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-28 19:33:22.000000 textalloc-0.1.2/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-28 19:33:22.000000 textalloc-0.1.2/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-0.1.1/LICENSE` & `textalloc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.1/PKG-INFO` & `textalloc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -128,14 +128,15 @@
     Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
 src_crs: (object), default None
     Default crs of data, required when using transform in kwargs.
     For example one can set src_crs=cartopy.crs.TransverseMercator() which is
     default in matplotlib if using transform=cartopy.crs.PlateCarree().
+plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

### Comparing `textalloc-0.1.1/README.md` & `textalloc-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
 src_crs: (object), default None
     Default crs of data, required when using transform in kwargs.
     For example one can set src_crs=cartopy.crs.TransverseMercator() which is
     default in matplotlib if using transform=cartopy.crs.PlateCarree().
+plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

### Comparing `textalloc-0.1.1/pyproject.toml` & `textalloc-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textalloc"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Christoffer Kjellson", email="c.kjellson@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Efficient Text Allocation in matplotlib using NumPy Broadcasting"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `textalloc-0.1.1/src/textalloc/__init__.py` & `textalloc-0.1.2/src/textalloc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from matplotlib.path import get_path_collection_extents
 from textalloc.non_overlapping_boxes import (
     get_non_overlapping_boxes,
     find_nearest_point_on_box,
 )
 import numpy as np
 import time
-from typing import List, Union
+from typing import Any, Dict, List, Union
 
 try:
     from tqdm import tqdm
 except ImportError:
 
     def tqdm(iterator, *args, **kwargs):
         return iterator
@@ -41,15 +41,16 @@
     textcolor: Union[str, List[str]] = "k",
     seed: int = 0,
     direction: str = None,
     x_logscale_base: float = None,
     y_logscale_base: float = None,
     avoid_label_lines_overlap: bool = False,
     src_crs: object = None,
-    **kwargs,
+    plot_kwargs: Dict[str, Any] = None,
+    ** kwargs,
 ):
     """Main function of allocating text-boxes in matplotlib plot
 
     Args:
         fig (_type_): matplotlib figure used for rendering textbox-sizes.
         ax (_type_): matplotlib axes used for plotting.
         x (Union[np.ndarray, List[float]]): x-coordinates of texts 1d array/list.
@@ -75,14 +76,15 @@
         textcolor (Union[str, List[str]], optional): color code of the text. Defaults to "k".
         seed (int, optional): seeds order of text allocations. Defaults to 0.
         direction (str, optional): set preferred location of the boxes (south, north, east, west, northeast, northwest, southeast, southwest). Defaults to None.
         x_logscale_base (int, optional): base of x-axis log-scale, required if the scaling of the x-axis is "log".
         y_logscale_base (int, optional): base of y-axis log-scale, required if the scaling of the y-axis is "log".
         avoid_label_lines_overlap (bool, optional): If True, avoids overlap with lines drawn between text labels and locations. Defaults to False.
         src_crs (object, optional): Default crs of data, required when using transform in kwargs. For example one can set src_crs=cartopy.crs.TransverseMercator() which is default in matplotlib if using transform=cartopy.crs.PlateCarree(). Defaults to None.
+        plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
         **kwargs (): kwargs for the plt.text() call.
     """
     t0 = time.time()
     aspect_ratio = fig.get_size_inches()[0] / fig.get_size_inches()[1]
     aspect_ratio2 = ax.get_aspect()
     xlims = ax.get_xlim()
     ylims = ax.get_ylim()
@@ -321,15 +323,15 @@
             )
             if x_near is not None:
                 ax.plot(
                     [x[ind], x_near],
                     [y[ind], y_near],
                     linewidth=linewidth,
                     c=linecolor[ind],
-                    **kwargs,
+                    **(plot_kwargs if plot_kwargs is not None else {}),
                 )
     for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
         ax.text(x_coord, y_coord, s, size=textsize[ind], c=textcolor[ind], **kwargs)
 
     if draw_all:
         for ind in overlapping_boxes_inds:
             ax.text(
```

### Comparing `textalloc-0.1.1/src/textalloc/candidates.py` & `textalloc-0.1.2/src/textalloc/candidates.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.1/src/textalloc/non_overlapping_boxes.py` & `textalloc-0.1.2/src/textalloc/non_overlapping_boxes.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.1/src/textalloc/overlap_functions.py` & `textalloc-0.1.2/src/textalloc/overlap_functions.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.1/src/textalloc.egg-info/PKG-INFO` & `textalloc-0.1.2/src/textalloc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -128,14 +128,15 @@
     Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
 src_crs: (object), default None
     Default crs of data, required when using transform in kwargs.
     For example one can set src_crs=cartopy.crs.TransverseMercator() which is
     default in matplotlib if using transform=cartopy.crs.PlateCarree().
+plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

