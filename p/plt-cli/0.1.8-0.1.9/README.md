# Comparing `tmp/plt_cli-0.1.8-py3-none-any.whl.zip` & `tmp/plt_cli-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12752 bytes, number of entries: 19
+Zip file size: 12735 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-Feb-09 12:48 plt/__init__.py
--rwxr-xr-x  2.0 unx     4846 b- defN 24-Apr-28 19:53 plt/plt
+-rwxr-xr-x  2.0 unx     4877 b- defN 24-Apr-28 20:15 plt/plt
 -rw-r--r--  2.0 unx      894 b- defN 24-Apr-28 20:01 plt/templates/python/matplotlib/density.py
 -rw-r--r--  2.0 unx      957 b- defN 24-Apr-28 20:01 plt/templates/python/matplotlib/histogram.py
 -rw-r--r--  2.0 unx      650 b- defN 24-Apr-28 19:35 plt/templates/python/matplotlib/line.py
 -rw-r--r--  2.0 unx      794 b- defN 24-Apr-28 20:01 plt/templates/python/matplotlib/line_2d.py
 -rw-r--r--  2.0 unx      848 b- defN 24-Apr-28 20:01 plt/templates/python/matplotlib/normalized_histogram.py
 -rw-r--r--  2.0 unx      832 b- defN 24-Apr-28 20:01 plt/templates/python/matplotlib/scatter.py
 -rw-r--r--  2.0 unx      583 b- defN 22-Feb-09 12:48 plt/templates/python/plotext/density.py
 -rw-r--r--  2.0 unx      570 b- defN 22-Dec-21 15:53 plt/templates/python/plotext/histogram.py
 -rw-r--r--  2.0 unx      456 b- defN 22-Feb-09 12:48 plt/templates/python/plotext/line.py
 -rw-r--r--  2.0 unx      590 b- defN 24-Feb-18 17:33 plt/templates/python/plotext/line_2d.py
 -rw-r--r--  2.0 unx      596 b- defN 22-Sep-16 18:58 plt/templates/python/plotext/scatter.py
--rwxr-xr-x  2.0 unx     4832 b- defN 24-Apr-28 20:07 plt_cli-0.1.8.data/scripts/plt
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-28 20:07 plt_cli-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1111 b- defN 24-Apr-28 20:07 plt_cli-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 20:07 plt_cli-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-28 20:07 plt_cli-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1679 b- defN 24-Apr-28 20:07 plt_cli-0.1.8.dist-info/RECORD
-19 files, 21395 bytes uncompressed, 9948 bytes compressed:  53.5%
+-rwxr-xr-x  2.0 unx     4863 b- defN 24-Apr-28 20:21 plt_cli-0.1.9.data/scripts/plt
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-28 20:21 plt_cli-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1111 b- defN 24-Apr-28 20:21 plt_cli-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 20:21 plt_cli-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-28 20:21 plt_cli-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1679 b- defN 24-Apr-28 20:21 plt_cli-0.1.9.dist-info/RECORD
+19 files, 21457 bytes uncompressed, 9931 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: plt/templates/python/plotext/line_2d.py
 Comment: 
 
 Filename: plt/templates/python/plotext/scatter.py
 Comment: 
 
-Filename: plt_cli-0.1.8.data/scripts/plt
+Filename: plt_cli-0.1.9.data/scripts/plt
 Comment: 
 
-Filename: plt_cli-0.1.8.dist-info/LICENSE
+Filename: plt_cli-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: plt_cli-0.1.8.dist-info/METADATA
+Filename: plt_cli-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: plt_cli-0.1.8.dist-info/WHEEL
+Filename: plt_cli-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: plt_cli-0.1.8.dist-info/top_level.txt
+Filename: plt_cli-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: plt_cli-0.1.8.dist-info/RECORD
+Filename: plt_cli-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plt/plt

```diff
@@ -141,18 +141,21 @@
 # substitute remaining by default values
 template = re.sub('<<[^:]*:', '', template)
 template = re.sub('>>', '', template)
 
 if args.py:
     print(template)
 else:
-    f = BytesIO()
-    old_stdout = sys.stdout
-    sys.stdout = f
-    exec(template, {})
-    sys.stdout = old_stdout
 
     if args.icat:
+        f = BytesIO()
+        old_stdout = sys.stdout
+        sys.stdout = f
+        exec(template, {})
+        sys.stdout = old_stdout
+
         process = Popen(['kitty', 'icat'], stdin=PIPE, bufsize=-1)
         process.communicate(input=f.getvalue())
+        print(f.getvalue())
+
     else:
-        sys.stdout.buffer.write(f.getvalue())
+        exec(template, {})
```

## Comparing `plt_cli-0.1.8.data/scripts/plt` & `plt_cli-0.1.9.data/scripts/plt`

 * *Files 4% similar despite different names*

```diff
@@ -141,18 +141,21 @@
 # substitute remaining by default values
 template = re.sub('<<[^:]*:', '', template)
 template = re.sub('>>', '', template)
 
 if args.py:
     print(template)
 else:
-    f = BytesIO()
-    old_stdout = sys.stdout
-    sys.stdout = f
-    exec(template, {})
-    sys.stdout = old_stdout
 
     if args.icat:
+        f = BytesIO()
+        old_stdout = sys.stdout
+        sys.stdout = f
+        exec(template, {})
+        sys.stdout = old_stdout
+
         process = Popen(['kitty', 'icat'], stdin=PIPE, bufsize=-1)
         process.communicate(input=f.getvalue())
+        print(f.getvalue())
+
     else:
-        sys.stdout.buffer.write(f.getvalue())
+        exec(template, {})
```

## Comparing `plt_cli-0.1.8.dist-info/LICENSE` & `plt_cli-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plt_cli-0.1.8.dist-info/METADATA` & `plt_cli-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plt-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI plotting utility
 Home-page: https://github.com/rlschuller/plt
 Author: Rodrigo Loro Schuller
 Author-email: rloroschuller@gmail.com
 Project-URL: Bug Tracker, https://github.com/rlschuller/plt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `plt_cli-0.1.8.dist-info/RECORD` & `plt_cli-0.1.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 plt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-plt/plt,sha256=LFZKT32CjonrKdOj5RX4lc64YJOhHQ-KTxeLCw4uafs,4846
+plt/plt,sha256=aEmn9q1lU8Auz62fxjGVeA1vtAeQntp4r10Glo_uPeE,4877
 plt/templates/python/matplotlib/density.py,sha256=Q-VLrXCwINZMjWG7lWkwGfG1xXy8FapVh2dbOly0JCA,894
 plt/templates/python/matplotlib/histogram.py,sha256=49cTLdeEIq__Ep0EQusYB9sdtG6p6ZICi2DDU9TKYvI,957
 plt/templates/python/matplotlib/line.py,sha256=YOsfJ1J3tTzvSJk46C87MtngCFhzUL5zR9xpU8eDs8Y,650
 plt/templates/python/matplotlib/line_2d.py,sha256=n5aWLAgUY8NIIY4WBaRdPHwspXQ4B3buJm_dZOH2tlI,794
 plt/templates/python/matplotlib/normalized_histogram.py,sha256=UadTTihNAXLAwhkeEy-1XcQWk2fZAbubOTIg3LO5yzI,848
 plt/templates/python/matplotlib/scatter.py,sha256=Dho9_04MBZGqma5taE9WDAvnrQzSaLk5lmGGGyNwsSE,832
 plt/templates/python/plotext/density.py,sha256=Upv8Bvve0I00X---hydFHt5Im23h5yvWLhlh1LPlB9k,583
 plt/templates/python/plotext/histogram.py,sha256=o5JHZezDkVJ4l0ZMrXnswbtnPlNQ3-Pl17pGtyO35t8,570
 plt/templates/python/plotext/line.py,sha256=ejbpMeYjD45oIrANt0LSGR76TT4ggCtnC3dBVvbedeI,456
 plt/templates/python/plotext/line_2d.py,sha256=QlQ0k-rmoOC6AkYbONAIOmnDQAEZwCjJNltXMvPHkpU,590
 plt/templates/python/plotext/scatter.py,sha256=P-oW-6gc352se2QqMSaWqk9s8XdzP0sDcHCngau3Zu0,596
-plt_cli-0.1.8.data/scripts/plt,sha256=pz51WpeniqXY3im4hv3f4n19rcRX85jnPb7yUWfSAmM,4832
-plt_cli-0.1.8.dist-info/LICENSE,sha256=LzFoEOoP6Ft-CaRnffscO7BhQWVyJmy0xIU-YL_Y5tA,1061
-plt_cli-0.1.8.dist-info/METADATA,sha256=KTTM2rVYaq8frtyo-Ao5nRwl52Yvad2YF_WDUIUVIZ4,1111
-plt_cli-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-plt_cli-0.1.8.dist-info/top_level.txt,sha256=BOa_6dnl1Sm1TASq1nK3PKkTWtMOQK9X6ogMxIEUw-w,4
-plt_cli-0.1.8.dist-info/RECORD,,
+plt_cli-0.1.9.data/scripts/plt,sha256=vJIBBZAMraSU6iX_z3OqdDMNuSsG9P5zgdQFZugtoN0,4863
+plt_cli-0.1.9.dist-info/LICENSE,sha256=LzFoEOoP6Ft-CaRnffscO7BhQWVyJmy0xIU-YL_Y5tA,1061
+plt_cli-0.1.9.dist-info/METADATA,sha256=YcYVULKEWnaheVOY_yI8oYoWOCv1b3MokSLkygnPby8,1111
+plt_cli-0.1.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+plt_cli-0.1.9.dist-info/top_level.txt,sha256=BOa_6dnl1Sm1TASq1nK3PKkTWtMOQK9X6ogMxIEUw-w,4
+plt_cli-0.1.9.dist-info/RECORD,,
```

