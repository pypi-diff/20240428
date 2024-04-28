# Comparing `tmp/kbinxml-2.0.tar.gz` & `tmp/kbinxml-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbinxml-2.0.tar", last modified: Thu Oct 26 08:03:11 2023, max compression
+gzip compressed data, was "kbinxml-2.1.tar", last modified: Sun Apr 28 00:54:32 2024, max compression
```

## Comparing `kbinxml-2.0.tar` & `kbinxml-2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-10-26 08:03:11.046638 kbinxml-2.0/
--rw-rw-rw-   0        0        0     1060 2020-07-09 23:24:57.000000 kbinxml-2.0/LICENSE
--rw-rw-rw-   0        0        0      322 2023-10-26 08:03:11.046638 kbinxml-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      639 2020-07-09 23:25:03.000000 kbinxml-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-26 08:03:11.036639 kbinxml-2.0/kbinxml/
--rw-rw-rw-   0        0        0       35 2017-12-11 17:21:32.000000 kbinxml-2.0/kbinxml/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-10-26 07:42:28.000000 kbinxml-2.0/kbinxml/bytebuffer.py
--rw-rw-rw-   0        0        0     4636 2023-10-26 07:08:34.000000 kbinxml-2.0/kbinxml/format_ids.py
--rw-rw-rw-   0        0        0    17400 2023-10-26 07:59:13.000000 kbinxml-2.0/kbinxml/kbinxml.py
--rw-rw-rw-   0        0        0     1057 2023-10-26 06:41:09.000000 kbinxml-2.0/kbinxml/sixbit.py
--rw-rw-rw-   0        0        0      794 2023-10-26 07:03:32.000000 kbinxml-2.0/kbinxml/test.py
-drwxrwxrwx   0        0        0        0 2023-10-26 08:03:11.045638 kbinxml-2.0/kbinxml.egg-info/
--rw-rw-rw-   0        0        0      322 2023-10-26 08:03:10.000000 kbinxml-2.0/kbinxml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-10-26 08:03:11.000000 kbinxml-2.0/kbinxml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-26 08:03:10.000000 kbinxml-2.0/kbinxml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-10-26 08:03:10.000000 kbinxml-2.0/kbinxml.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-10-26 08:03:10.000000 kbinxml-2.0/kbinxml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-26 08:03:10.000000 kbinxml-2.0/kbinxml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-10-26 08:03:11.048639 kbinxml-2.0/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-10-26 07:33:29.000000 kbinxml-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:54:32.876220 kbinxml-2.1/
+-rw-rw-rw-   0        0        0     1060 2020-07-09 23:24:57.000000 kbinxml-2.1/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-28 00:54:32.876220 kbinxml-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2020-07-09 23:25:03.000000 kbinxml-2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 00:54:32.864221 kbinxml-2.1/kbinxml/
+-rw-rw-rw-   0        0        0       35 2017-12-11 17:21:32.000000 kbinxml-2.1/kbinxml/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-10-26 07:42:28.000000 kbinxml-2.1/kbinxml/bytebuffer.py
+-rw-rw-rw-   0        0        0     4636 2023-10-26 07:08:34.000000 kbinxml-2.1/kbinxml/format_ids.py
+-rw-rw-rw-   0        0        0    17533 2024-04-28 00:52:38.000000 kbinxml-2.1/kbinxml/kbinxml.py
+-rw-rw-rw-   0        0        0     1057 2023-10-26 06:41:09.000000 kbinxml-2.1/kbinxml/sixbit.py
+-rw-rw-rw-   0        0        0      794 2023-10-26 07:03:32.000000 kbinxml-2.1/kbinxml/test.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:54:32.875222 kbinxml-2.1/kbinxml.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-28 00:54:32.000000 kbinxml-2.1/kbinxml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-28 00:54:32.000000 kbinxml-2.1/kbinxml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 00:54:32.000000 kbinxml-2.1/kbinxml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-28 00:54:32.000000 kbinxml-2.1/kbinxml.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 00:54:32.000000 kbinxml-2.1/kbinxml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 00:54:32.000000 kbinxml-2.1/kbinxml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-28 00:54:32.878222 kbinxml-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      594 2024-04-28 00:53:41.000000 kbinxml-2.1/setup.py
```

### Comparing `kbinxml-2.0/LICENSE` & `kbinxml-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kbinxml-2.0/README.md` & `kbinxml-2.1/README.md`

 * *Files identical despite different names*

### Comparing `kbinxml-2.0/kbinxml/bytebuffer.py` & `kbinxml-2.1/kbinxml/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `kbinxml-2.0/kbinxml/format_ids.py` & `kbinxml-2.1/kbinxml/format_ids.py`

 * *Files identical despite different names*

### Comparing `kbinxml-2.0/kbinxml/kbinxml.py` & `kbinxml-2.1/kbinxml/kbinxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
-from struct import calcsize
-import sys
 import operator
+import sys
 from io import BytesIO
+from struct import calcsize
 
 import lxml.etree as etree
 
 from .bytebuffer import ByteBuffer
-from .sixbit import pack_sixbit, unpack_sixbit
 from .format_ids import xml_formats, xml_types
+from .sixbit import pack_sixbit, unpack_sixbit
 
 DEBUG_OFFSETS = False
 DEBUG = False
 
 SIGNATURE = 0xA0
 
 SIG_COMPRESSED = 0x42
@@ -475,15 +475,19 @@
     args = parser.parse_args()
 
     with open(args.filename, "rb") as f:
         input = f.read()
 
     xml = KBinXML(input, convert_illegal_things=args.convert_illegal)
     stdout = getattr(sys.stdout, "buffer", sys.stdout)
-    if KBinXML.is_binary_xml(input):
-        stdout.write(xml.to_text().encode("utf-8"))
-    else:
-        stdout.write(xml.to_binary())
+    try:
+        if KBinXML.is_binary_xml(input):
+            stdout.write(xml.to_text().encode("utf-8"))
+        else:
+            stdout.write(xml.to_binary())
+    except BrokenPipeError:
+        # allows kbinxml to be piped to `head` or similar
+        sys.exit(141)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `kbinxml-2.0/kbinxml/sixbit.py` & `kbinxml-2.1/kbinxml/sixbit.py`

 * *Files identical despite different names*

### Comparing `kbinxml-2.0/kbinxml/test.py` & `kbinxml-2.1/kbinxml/test.py`

 * *Files identical despite different names*

### Comparing `kbinxml-2.0/setup.py` & `kbinxml-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup
 
-
 requires = [
     "lxml",
 ]
 
 python_requires = ">=3.10"
 
-version = "2.0"
+version = "2.1"
 setup(
     name="kbinxml",
     description="Decoder/encoder for Konami's binary XML format",
     long_description="See Github for up to date documentation",
     version=version,
     entry_points={
         "console_scripts": ["kbinxml=kbinxml:main"],
```

