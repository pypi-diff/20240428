# Comparing `tmp/colormap-1.0.6.tar.gz` & `tmp/colormap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colormap-1.0.6.tar", last modified: Tue Oct 10 12:50:01 2023, max compression
+gzip compressed data, was "colormap-1.1.0.tar", max compression
```

## Comparing `colormap-1.0.6.tar` & `colormap-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:50:01.000000 colormap-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-10 12:49:55.000000 colormap-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-10 12:49:55.000000 colormap-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-10-10 12:50:01.000000 colormap-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2023-10-10 12:49:55.000000 colormap-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-10 12:49:55.000000 colormap-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-10 12:50:01.000000 colormap-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-10 12:49:55.000000 colormap-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:50:01.000000 colormap-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-10-10 12:49:55.000000 colormap-1.0.6/src/colormap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33326 2023-10-10 12:49:55.000000 colormap-1.0.6/src/colormap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-10-10 12:49:55.000000 colormap-1.0.6/src/colormap/get_cmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2023-10-10 12:49:55.000000 colormap-1.0.6/src/colormap/xfree86.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-10 12:50:01.000000 colormap-1.0.6/src/colormap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 12:50:01.000000 colormap-1.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2023-10-10 12:49:55.000000 colormap-1.0.6/test/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-10-10 12:49:55.000000 colormap-1.0.6/test/test_get_cmap.py
+-rw-r--r--   0        0        0     1482 2021-09-07 22:57:02.000000 colormap-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2860 2024-04-28 15:53:47.221288 colormap-1.1.0/README.rst
+-rw-r--r--   0        0        0     1711 2024-04-28 15:39:16.151288 colormap-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1056 2024-04-28 15:23:36.571977 colormap-1.1.0/src/colormap/__init__.py
+-rw-r--r--   0        0        0    34590 2024-04-28 15:53:47.222288 colormap-1.1.0/src/colormap/colors.py
+-rw-r--r--   0        0        0     2029 2022-04-04 17:11:34.000000 colormap-1.1.0/src/colormap/get_cmap.py
+-rw-r--r--   0        0        0     4810 2022-04-04 17:11:34.000000 colormap-1.1.0/src/colormap/xfree86.py
+-rw-r--r--   0        0        0     4010 1970-01-01 00:00:00.000000 colormap-1.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `colormap-1.0.6/LICENSE` & `colormap-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `colormap-1.0.6/README.rst` & `colormap-1.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 .. image:: https://github.com/cokelaer/colormap/actions/workflows/ci.yml/badge.svg?branch=master
     :target: https://github.com/cokelaer/colormap/actions/workflows/ci.yml
 
 .. image:: https://coveralls.io/repos/cokelaer/colormap/badge.png?branch=master
     :target: https://coveralls.io/r/cokelaer/colormap?branch=master
 
 
-:version: Python 3.8, 3.9, 3.10, 3.11
+:version: Python 3.8, 3.9, 3.10, 3.11, 3.12
 :contributions: Please join https://github.com/cokelaer/colormap
 :issues: Please use https://github.com/cokelaer/colormap/issues
 :notebook: Please see https://github.com/cokelaer/colormap/tree/master/notebooks
 
 
 
 What is it ?
@@ -72,14 +72,16 @@
 
 changelog
 #########
 
 ========= ================================================================================
 Version   Description
 ========= ================================================================================
+1.1.0     * switch to pyproject. remove easydev dependency. compat for python 3.11 and
+            3.12
 1.0.6     * Fix a matplotlib deprecation
           * Fix RTD documentation
 1.0.5     * remove Python3.6 and added Python3.10 to CI action
           * Fix issue in setup reported in https://github.com/cokelaer/colormap/pull/14
           * add requirements in MANIFEST
           * applied black on all files
 ========= ================================================================================
```

### Comparing `colormap-1.0.6/src/colormap/__init__.py` & `colormap-1.1.0/src/colormap/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 # http://www.gnu.org/licenses/gpl-3.0.html
 #
 # Website: https://www.github.com/cokelaer/colormap
 # Documentation: http://packages.python.org/colormap
 #
 ##############################################################################
 """main colormap module"""
-from __future__ import print_function
-from __future__ import division
+from importlib import metadata
 
-import pkg_resources
 
-try:
-    version = pkg_resources.require("colormap")[0].version
-    __version__ = version
-except Exception:
-    version = ""
+def get_package_version(package_name):
+    try:
+        version = metadata.version(package_name)
+        return version
+    except metadata.PackageNotFoundError:
+        return f"{package_name} not found"
+
+
+version = get_package_version("colormap")
 
 
-from .xfree86 import *
 from . import colors
 from .colors import *
 from .get_cmap import *
+from .xfree86 import *
 
 c = Colormap()
 colormap_names = c.colormaps + c.diverging_black
 # create an alias to test_colormap methiod
 test_colormap = c.test_colormap
 test_cmap = c.test_colormap
```

### Comparing `colormap-1.0.6/src/colormap/colors.py` & `colormap-1.1.0/src/colormap/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 standard Python module called :mod:`colorsys` or in matplotlib.colors
 (e.g rgb2hex) or are original to this module (e.g., rgb2huv)
 
 
 """
 # matplotlib dependence is only inside Colormap class
 import colorsys
-from easydev.tools import check_param_in_list, swapdict, check_range
-from colormap.xfree86 import XFree86_colors
 
+from colormap.xfree86 import XFree86_colors
 
 __all__ = [
     "HEX",
     "Color",
     "hex2web",
     "web2hex",
     "hex2rgb",
@@ -44,14 +43,61 @@
     "to_intensity",
     "yuv2rgb_int",
     "rgb2yuv_int",
     "Colormap",
 ]
 
 
+def check_range(data, dmin, dmax):
+    if data < dmin or data > dmax:
+        raise ValueError(f"Value must be in the range [{dmin}-{dmax}]. You provided {data}")
+
+
+def swapdict(dic, check_ambiguity=True):
+    """Swap keys for values in a dictionary
+
+    ::
+
+        >>> d = {'a':1}
+        >>> swapdict(d)
+        {1:'a'}
+
+    """
+    # this version is more elegant but slightly slower : return {v:k for k,v in dic.items()}
+    if check_ambiguity:
+        assert len(set(dic.keys())) == len(set(dic.values())), "values is not a set. ambiguities for keys."
+    return dict(zip(dic.values(), dic.keys()))
+
+
+def check_param_in_list(param, valid_values, name=None):
+    """Checks that the value of param is amongst valid
+
+    :param param: a parameter to be checked
+    :param list valid_values: a list of values
+
+    ::
+
+        check_param_in_list(1, [1,2,3])
+        check_param_in_list(mode, ["on", "off"])
+    """
+    if isinstance(valid_values, list) is False:
+
+        raise TypeError(
+            "the valid_values second argument must be a list of valid values. {0} was provided.".format(valid_values)
+        )
+
+    if param not in valid_values:
+        if name:
+            msg = "Incorrect value provided for {} ({})".format(name, param)
+        else:
+            msg = "Incorrect value provided (%s)" % param
+        msg += "    Correct values are %s" % valid_values
+        raise ValueError(msg)
+
+
 def hex2web(hexa):
     """Convert hexadecimal string (6 digits) into *web* version (3 digits)
 
     .. doctest::
 
         >>> from colormap.colors import hex2web
         >>> hex2web("#FFAA11")
@@ -132,17 +178,19 @@
 
     """
     if normalised:
         r, g, b = _denormalise(r, g, b, mode="rgb")
         r = int(r)
         g = int(g)
         b = int(b)
+
     check_range(r, 0, 255)
     check_range(g, 0, 255)
     check_range(b, 0, 255)
+
     return "#%02X%02X%02X" % (r, g, b)
 
 
 def rgb2hls(r, g, b, normalised=True):
     """Convert an RGB value to an HLS value.
 
     :param bool normalised: if *normalised* is True, the input RGB triplet
@@ -284,15 +332,15 @@
     return colorsys.hls_to_rgb(h, l, s)
 
 
 def hex2dec(data):
     """convert hexadecimal string (data) into a float in the [0-65536] inclusive range"""
     if data[0] == "#":
         data.replace("#", "")
-    return int(data, 16) / 255.0
+    return int(data, 16) / 255
 
 
 def rgb2yuv(r, g, b):
     """Convert RGB triplet into YUV
 
     :return: YUV triplet with values between 0 and 1
 
@@ -306,31 +354,31 @@
     check_range(b, 0, 1)
 
     # y = int(0.299 * r + 0.587 * g + 0.114 * b)
     # u = int(-0.14713 * r + -0.28886 * g + 0.436 * b)
     # v = int(0.615 * r + -0.51499 * g + -0.10001 * b)
 
     y = 0.299 * r + 0.587 * g + 0.114 * b
-    u = -32591.0 / 221500.0 * r + -63983.0 / 221500.0 * g + 0.436 * b
-    v = 0.615 * r + -72201.0 / 140200 * g + -7011 / 70100.0 * b
+    u = -32591 / 221500 * r + -63983 / 221500 * g + 0.436 * b
+    v = 0.615 * r + -72201 / 140200 * g + -7011 / 70100 * b
     return (y, u, v)
 
 
 def yuv2rgb(y, u, v):
     """Convert YUV triplet into RGB
 
     `YUV <http://en.wikipedia.org/wiki/YUV>`_
 
     .. warning:: expected input must be between 0 and 255 (not normalised)
 
     """
     check_range(y, 0, 1)
     check_range(u, 0, 1)
     check_range(v, 0, 1)
-    A, B, C, D = 701.0 / 615.0, 25251.0 / 63983.0, 209599.0 / 361005.0, 443.0 / 218.0
+    A, B, C, D = 701 / 615, 25251 / 63983, 209599 / 361005, 443 / 218
     r = y + A * v
     g = y - B * u - C * v
     b = y + D * u
     return (r, g, b)
 
 
 def rgb2yuv_int(r, g, b):
@@ -342,16 +390,16 @@
 
     """
     check_range(r, 0, 255)
     check_range(g, 0, 255)
     check_range(b, 0, 255)
 
     y = int(0.299 * r + 0.587 * g + 0.114 * b)
-    u = int(-32591.0 / 221500.0 * r + -63983.0 / 221500.0 * g + 0.436 * b)
-    v = int(0.615 * r + -72201.0 / 140200 * g + -7011 / 70100.0 * b)
+    u = int(-32591 / 221500 * r + -63983 / 221500 * g + 0.436 * b)
+    v = int(0.615 * r + -72201 / 140200 * g + -7011 / 70100 * b)
 
     return (y, u, v)
 
 
 def yuv2rgb_int(y, u, v):
     """Convert YUV triplet into RGB
 
@@ -368,35 +416,35 @@
     b = int(y + 2.03211 * u)
     return (r, g, b)
 
 
 def _denormalise(r, g, b, mode="rgb"):
     check_param_in_list(mode, ["rgb", "hls", "hsv"])
     if mode == "rgb":
-        return r * 255.0, g * 255.0, b * 255.0
+        return r * 255, g * 255, b * 255
     elif mode in ["hls", "hsv"]:
-        return r * 360.0, g * 100.0, b * 100.0
+        return r * 360, g * 100, b * 100
 
 
 def _normalise(r, g, b, mode="rgb"):
     check_param_in_list(mode, ["rgb", "hls", "hsv"])
     if mode == "rgb":
-        return r / 255.0, g / 255.0, b / 255.0
+        return r / 255, g / 255, b / 255
     elif mode in ["hls", "hsv"]:
-        return r / 360.0, g / 100.0, b / 100.0
+        return r / 360, g / 100, b / 100
 
 
 def to_intensity(n):
     """Return intensity
 
     :param n: value between 0 and 1
     :return: value between 0 and 255; round(n*127.5+127.5)
     """
     check_range(n, 0, 1)
-    return int(round(n * 127.5 + 127.5))
+    return round(n * 127.5 + 127.5)
 
 
 class HEX(object):
     """Class to check the validity of an hexadecimal string and get standard string
 
     By standard, we mean #FFFFFF (6 digits)
 
@@ -880,17 +928,17 @@
                  '#0066FFFF', '#001AFFFF', '#3300FFFF', '#7F00FFFF',
                  '#CC00FFFF','#FF00E6FF','#FF0099FF', '#FF004DFF']
             c.plot_rgb_from_hex_list(t)
 
         """
         import pylab
 
-        red = [hex2rgb(x)[0] / 255.0 for x in cols]
-        blue = [hex2rgb(x)[2] / 255.0 for x in cols]
-        green = [hex2rgb(x)[1] / 255.0 for x in cols]
+        red = [hex2rgb(x)[0] / 255 for x in cols]
+        blue = [hex2rgb(x)[2] / 255 for x in cols]
+        green = [hex2rgb(x)[1] / 255 for x in cols]
         x = pylab.linspace(0, 1, len(cols))
         pylab.clf()
         pylab.plot(x, red, "ro-", alpha=0.5)
         pylab.plot(x, green, "gs-", alpha=0.5, markersize=15)
         pylab.plot(x, blue, "bx-", alpha=0.5, markersize=15)
         pylab.ylim([-0.1, 1.1])
 
@@ -939,14 +987,15 @@
 
         """
         # matplotlib colormaps
         if colors in self.colormaps:
             if reverse and colors.endswith("_r") is False:
                 colors += "_r"
             from matplotlib import colormaps
+
             return colormaps[colors]
         # custom ones
         elif colors in self.diverging_black:
             c1, c2, c3 = colors.split("_")
             # special case of sky, which does not exists
             c3 = c3.replace("sky", "deep sky blue")
             return self.cmap_linear(c1, c2, c3)
@@ -1034,21 +1083,21 @@
 
         By default, test the :meth:`get_cmap_heat`
 
         """
         if cmap is None:
             cmap = self.get_cmap_heat()
         import numpy as np
-        from pylab import clf, pcolor, colorbar, show, linspace, axis
+        from pylab import axis, clf, colorbar, linspace, pcolor, show
 
         A, B = np.meshgrid(linspace(0, 10, 100), linspace(0, 10, 100))
         clf()
         pcolor((A - 5) ** 2 + (B - 5) ** 2, cmap=cmap)
         colorbar()
-        show()
+        # show()
         axis("off")
 
     def plot_colormap(self, cmap_list=None):
         """cmap_list list of valid cmap or name of a set (sequential,
         diverging,)
 
         if none, plot all known colors
@@ -1076,24 +1125,24 @@
             )
         for this in cmap_list:
             if this not in self.colormaps and this not in self.diverging_black:
                 raise ValueError("unknown colormap name. Please check valid names in colormaps attribute")
 
         nrows = len(cmap_list)
 
-        gradient = [x / 255.0 for x in range(0, 256)]
+        gradient = [x / 255 for x in range(0, 256)]
         gradient = [gradient, gradient]
         # np.vstack((gradient, gradient))
 
         fig, axes = subplots(nrows=nrows)
         fig.subplots_adjust(top=0.95, bottom=0.05, left=0.05, right=0.8)
 
         for ax, name in zip(axes, cmap_list):
             ax.imshow(gradient, aspect="auto", cmap=self.cmap(name))
             pos = list(ax.get_position().bounds)
             x_text = pos[2] + 0.08
-            y_text = pos[1] + pos[3] / 2.0
+            y_text = pos[1] + pos[3] / 2
             fig.text(x_text, y_text, name, va="center", ha="left", fontsize=10)
 
         # Turn off *all* ticks & spines, not just the ones with colormaps.
         for ax in axes:
             ax.set_axis_off()
```

### Comparing `colormap-1.0.6/src/colormap/get_cmap.py` & `colormap-1.1.0/src/colormap/get_cmap.py`

 * *Files identical despite different names*

### Comparing `colormap-1.0.6/src/colormap/xfree86.py` & `colormap-1.1.0/src/colormap/xfree86.py`

 * *Files identical despite different names*

