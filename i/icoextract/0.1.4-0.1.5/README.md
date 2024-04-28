# Comparing `tmp/icoextract-0.1.4.tar.gz` & `tmp/icoextract-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icoextract-0.1.4.tar", last modified: Mon Aug  8 08:05:01 2022, max compression
+gzip compressed data, was "icoextract-0.1.5.tar", last modified: Sun Apr 28 20:07:21 2024, max compression
```

## Comparing `icoextract-0.1.4.tar` & `icoextract-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 08:05:01.207731 icoextract-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     1144 2022-08-08 08:04:11.000000 icoextract-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4008 2022-08-08 08:05:01.207731 icoextract-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2469 2022-08-08 08:04:11.000000 icoextract-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 08:05:01.203731 icoextract-0.1.4/icoextract/
--rw-r--r--   0 root         (0) root         (0)     6290 2022-08-08 08:04:11.000000 icoextract-0.1.4/icoextract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 08:05:01.207731 icoextract-0.1.4/icoextract/scripts/
--rw-r--r--   0 root         (0) root         (0)       48 2022-08-08 08:04:11.000000 icoextract-0.1.4/icoextract/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      810 2022-08-08 08:04:11.000000 icoextract-0.1.4/icoextract/scripts/extract.py
--rwxr-xr-x   0 root         (0) root         (0)      823 2022-08-08 08:04:11.000000 icoextract-0.1.4/icoextract/scripts/icolist.py
--rwxr-xr-x   0 root         (0) root         (0)     2352 2022-08-08 08:04:11.000000 icoextract-0.1.4/icoextract/scripts/thumbnailer.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-08 08:04:11.000000 icoextract-0.1.4/icoextract/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 08:05:01.207731 icoextract-0.1.4/icoextract.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2022-08-08 08:05:01.000000 icoextract-0.1.4/icoextract.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2022-08-08 08:05:01.000000 icoextract-0.1.4/icoextract.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-08 08:05:01.000000 icoextract-0.1.4/icoextract.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      174 2022-08-08 08:05:01.000000 icoextract-0.1.4/icoextract.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-08 08:05:01.000000 icoextract-0.1.4/icoextract.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-08-08 08:05:01.000000 icoextract-0.1.4/icoextract.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      190 2022-08-08 08:05:01.207731 icoextract-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1523 2022-08-08 08:04:11.000000 icoextract-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:07:21.215237 icoextract-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-28 20:06:45.000000 icoextract-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-04-28 20:07:21.215237 icoextract-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-28 20:06:45.000000 icoextract-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:07:21.215237 icoextract-0.1.5/icoextract/
+-rw-r--r--   0 root         (0) root         (0)     6712 2024-04-28 20:06:45.000000 icoextract-0.1.5/icoextract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:07:21.215237 icoextract-0.1.5/icoextract/scripts/
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-28 20:06:45.000000 icoextract-0.1.5/icoextract/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      834 2024-04-28 20:06:45.000000 icoextract-0.1.5/icoextract/scripts/extract.py
+-rwxr-xr-x   0 root         (0) root         (0)      823 2024-04-28 20:06:45.000000 icoextract-0.1.5/icoextract/scripts/icolist.py
+-rwxr-xr-x   0 root         (0) root         (0)     2376 2024-04-28 20:06:45.000000 icoextract-0.1.5/icoextract/scripts/thumbnailer.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-28 20:06:45.000000 icoextract-0.1.5/icoextract/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:07:21.215237 icoextract-0.1.5/icoextract.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-04-28 20:07:21.000000 icoextract-0.1.5/icoextract.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-28 20:07:21.000000 icoextract-0.1.5/icoextract.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 20:07:21.000000 icoextract-0.1.5/icoextract.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      173 2024-04-28 20:07:21.000000 icoextract-0.1.5/icoextract.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-28 20:07:21.000000 icoextract-0.1.5/icoextract.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-28 20:07:21.000000 icoextract-0.1.5/icoextract.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      190 2024-04-28 20:07:21.215237 icoextract-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-04-28 20:06:45.000000 icoextract-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:07:21.215237 icoextract-0.1.5/tests/
+-rwxr-xr-x   0 root         (0) root         (0)     2167 2024-04-28 20:06:45.000000 icoextract-0.1.5/tests/test_extract.py
+-rwxr-xr-x   0 root         (0) root         (0)     2559 2024-04-28 20:06:45.000000 icoextract-0.1.5/tests/test_thumbnailer.py
```

### Comparing `icoextract-0.1.4/LICENSE` & `icoextract-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `icoextract-0.1.4/README.md` & `icoextract-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # icoextract
 
 [![Build Status](https://drone.overdrivenetworks.com/api/badges/jlu5/icoextract/status.svg)](https://drone.overdrivenetworks.com/jlu5/icoextract)
 
-**icoextract** is an icon extractor for Windows PE files (.exe/.dll), written in Python. It also includes a thumbnailer script (`exe-thumbnailer`) for Linux desktops.
+**icoextract** is an icon extractor for Windows PE files (.exe/.dll/.mun), written in Python. It also includes a thumbnailer script (`exe-thumbnailer`) for Linux desktops.
 
 This project is inspired by [extract-icon-py](https://github.com/firodj/extract-icon-py), [icoutils](https://www.nongnu.org/icoutils/), and others.
 
 icoextract aims to be:
 
 - Lightweight
 - Portable (cross-platform)
@@ -19,50 +19,52 @@
 You can install the project via pip: `pip3 install icoextract[thumbnailer]`
 
 On Linux, you can activate the thumbnailer by copying [`exe-thumbnailer.thumbnailer`](/exe-thumbnailer.thumbnailer) into the thumbnailers directory:
 
 - `/usr/local/share/thumbnailers/` if you installed `icoextract` globally
 - `~/.local/share/thumbnailers` if you installed `icoextract` for your user only
 
-The thumbnailer should work with any file manager that implements the [Freedesktop Thumbnails Standard](https://specifications.freedesktop.org/thumbnail-spec/thumbnail-spec-latest.html): this includes Nautilus, Caja, Nemo, Thunar (when Tumbler is installed), and PCManFM. KDE / Dolphin uses a different architecture and is not supported here.
+The thumbnailer should work with any file manager that implements the [Freedesktop Thumbnails Standard](https://specifications.freedesktop.org/thumbnail-spec/thumbnail-spec-latest.html): this includes Nautilus, Caja, Nemo, Thunar (when Tumbler is installed), and PCManFM. KDE / Dolphin uses a different architecture and is *not* supported here.
 
 ### Distribution packages
 
-icoextract is packaged in these repositories:
+You can install icoextract from any of these distribution repositories:
 
-- Arch Linux AUR: [icoextract](https://aur.archlinux.org/packages/icoextract)
-- Debian (11+): [icoextract](https://packages.debian.org/icoextract)
-- Ubuntu (21.10+): [icoextract](https://packages.ubuntu.com/icoextract)
+[![Packaging status](https://repology.org/badge/vertical-allrepos/icoextract.svg)](https://repology.org/project/icoextract/versions)
 
 ## Usage
 
-icoextract ships `icoextract` and `icolist` scripts to extract and list icon resources in an executable:
+icoextract ships `icoextract` and `icolist` scripts to extract and list icon resources inside a file.
+
+**Note**: recent versions of Windows (Windows 10 1903+) have moved icons from system libraries (`shell32.dll`, etc.) into a new [`C:\Windows\SystemResources`](https://superuser.com/questions/1480268/) folder. icoextract can extract these `.mun` files natively, but the `.dll`s themselves no longer contain icons.
+
+For API docs, see https://projects.jlu5.com/icoextract.html
 
 ```
 usage: icoextract [-h] [-V] [-n NUM] [-v] input output
 
 Windows PE EXE icon extractor.
 
 positional arguments:
-  input              input filename
-  output             output filename
+  input              input filename (.exe/.dll/.mun)
+  output             output filename (.ico)
 
-optional arguments:
+options:
   -h, --help         show this help message and exit
   -V, --version      show program's version number and exit
   -n NUM, --num NUM  index of icon to extract
   -v, --verbose      enables debug logging
 ```
 
 ```
 usage: icolist [-h] [-V] [-v] input
 
 Lists group icons present in a program.
 
 positional arguments:
   input          input filename
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -V, --version  show program's version number and exit
   -v, --verbose  enables debug logging
 ```
```

### Comparing `icoextract-0.1.4/icoextract/__init__.py` & `icoextract-0.1.5/icoextract/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python3
 """
-Windows PE EXE icon extractor.
+Windows Portable Executable (PE) icon extractor.
+
+.. include:: ../LIB-USAGE.md
 """
 
 import io
 import logging
 import sys
 import struct
 
@@ -21,27 +23,29 @@
 try:
     from .version import __version__
 except ImportError:
     __version__ = 'unknown'
     logger.info('icoextract: failed to read program version')
 
 class IconExtractorError(Exception):
-    pass
+    """Superclass for exceptions raised by IconExtractor."""
+
 class NoIconsAvailableError(IconExtractorError):
-    pass
+    """Exception raised when the input program has no icon resources."""
+
 class InvalidIconDefinitionError(IconExtractorError):
-    pass
+    """Exception raised when the input program has an invalid icon resource."""
 
 class IconExtractor():
     def __init__(self, filename=None, data=None):
         """
-        Loads an executable from the given filename or data (raw bytes).
-        As with pefile, if both filename and data are given, filename takes precedence.
+        Loads an executable from the given `filename` or `data` (raw bytes).
+        As with pefile, if both `filename` and `data` are given, `filename` takes precedence.
 
-        If the executable has contains no icons, this will raise NoIconsAvailableError.
+        If the executable has contains no icons, this will raise `NoIconsAvailableError`.
         """
         # Use fast loading and explicitly load the RESOURCE directory entry. This saves a LOT of time
         # on larger files
         self._pe = pefile.PE(name=filename, data=data, fast_load=True)
         self._pe.parse_data_directories(pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE'])
 
         if not hasattr(self._pe, 'DIRECTORY_ENTRY_RESOURCE'):
@@ -136,23 +140,33 @@
             dataoffset += len(icon_data)  # Increase offset for next image
 
         # Second pass: write the icon data
         for datapair in icons:
             group_icon, icon_data = datapair
             fd.write(icon_data)
 
-    def export_icon(self, fname, num=0):
+    def export_icon(self, filename, num=0):
         """
-        Writes ICO data of the requested group icon ID to fname.
+        Exports ICO data for the requested group icon (`num`) to `filename`.
         """
-        with open(fname, 'wb') as f:
+        with open(filename, 'wb') as f:
             self._write_ico(f, num=num)
 
     def get_icon(self, num=0):
         """
-        Returns ICO data as a BytesIO() instance, containing the requested group icon ID.
+        Exports ICO data for the requested group icon (`num`) as a `io.BytesIO` instance.
         """
         f = io.BytesIO()
         self._write_ico(f, num=num)
         return f
 
-__all__ = ['IconExtractor']
+__all__ = [
+    'IconExtractor',
+    'IconExtractorError',
+    'NoIconsAvailableError',
+    'InvalidIconDefinitionError'
+]
+
+__pdoc__ = {
+    'scripts': False,
+    'version': False,
+}
```

### Comparing `icoextract-0.1.4/icoextract/scripts/extract.py` & `icoextract-0.1.5/icoextract/scripts/extract.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from icoextract import IconExtractor, logger, __version__
 
 def main():
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("-V", "--version", action='version', version=f'icoextract {__version__}')
     parser.add_argument("-n", "--num", type=int, help="index of icon to extract", default=0)
     parser.add_argument("-v", "--verbose", action="store_true", help="enables debug logging")
-    parser.add_argument("input", help="input filename")
-    parser.add_argument("output", help="output filename")
+    parser.add_argument("input", help="input filename (.exe/.dll/.mun)")
+    parser.add_argument("output", help="output filename (.ico)")
     args = parser.parse_args()
 
     if args.verbose:
         logger.setLevel(logging.DEBUG)
 
     extractor = IconExtractor(args.input)
     extractor.export_icon(args.output, num=args.num)
```

### Comparing `icoextract-0.1.4/icoextract/scripts/icolist.py` & `icoextract-0.1.5/icoextract/scripts/icolist.py`

 * *Files identical despite different names*

### Comparing `icoextract-0.1.4/icoextract/scripts/thumbnailer.py` & `icoextract-0.1.5/icoextract/scripts/thumbnailer.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
 
 def main():
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("-V", "--version", action='version', version=f'exe-thumbnailer, part of icoextract {__version__}')
     parser.add_argument("-s", "--size", type=int, help="size of desired thumbnail", default=256)
     parser.add_argument("-v", "--verbose", action="store_true", help="enables debug logging")
-    parser.add_argument("inputfile", help="input file name")
-    parser.add_argument("outfile", help="output file name", nargs='?')
+    parser.add_argument("inputfile", help="input file name (.exe/.dll/.mun)")
+    parser.add_argument("outfile", help="output file name (.png)", nargs='?')
     args = parser.parse_args()
 
     if args.verbose:
         logger.setLevel(logging.DEBUG)
 
     large_size = (args.size >= 256)
     generate_thumbnail(args.inputfile, args.outfile, large_size)
```

### Comparing `icoextract-0.1.4/setup.py` & `icoextract-0.1.5/setup.py`

 * *Files identical despite different names*

