# Comparing `tmp/elegantt-0.0.2.tar.gz` & `tmp/elegantt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantt-0.0.2.tar", last modified: Sun Feb 26 00:31:53 2023, max compression
+gzip compressed data, was "elegantt-0.0.3.tar", last modified: Sun Apr 28 14:36:40 2024, max compression
```

## Comparing `elegantt-0.0.2.tar` & `elegantt-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2023-02-26 00:31:53.796542 elegantt-0.0.2/
--rw-rw-r--   0 palau     (1000) palau     (1000)     1065 2023-02-23 05:08:13.000000 elegantt-0.0.2/LICENSE
--rw-rw-r--   0 palau     (1000) palau     (1000)       68 2023-02-25 08:35:15.000000 elegantt-0.0.2/MANIFEST.in
--rw-rw-r--   0 palau     (1000) palau     (1000)     1653 2023-02-26 00:31:53.795542 elegantt-0.0.2/PKG-INFO
--rw-rw-r--   0 palau     (1000) palau     (1000)      801 2023-02-25 13:31:13.000000 elegantt-0.0.2/README.md
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2023-02-26 00:31:53.790542 elegantt-0.0.2/elegantt/
--rw-rw-r--   0 palau     (1000) palau     (1000)       91 2023-02-25 13:16:30.000000 elegantt-0.0.2/elegantt/__init__.py
--rw-rw-r--   0 palau     (1000) palau     (1000)      692 2023-02-25 13:50:25.000000 elegantt-0.0.2/elegantt/command.py
--rw-rw-r--   0 palau     (1000) palau     (1000)     7323 2023-02-25 13:42:41.000000 elegantt-0.0.2/elegantt/elegantt.py
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2023-02-26 00:31:53.789542 elegantt-0.0.2/elegantt/tests/
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2023-02-26 00:31:53.790542 elegantt-0.0.2/elegantt/tests/ipaexg/
--rw-rw-r--   0 palau     (1000) palau     (1000)    20564 2023-02-23 02:32:09.000000 elegantt-0.0.2/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)     1710 2023-02-23 02:32:14.000000 elegantt-0.0.2/elegantt/tests/ipaexg/Readme_ipaexg00401.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)  6099900 2023-02-23 02:32:13.000000 elegantt-0.0.2/elegantt/tests/ipaexg/ipaexg.ttf
--rw-rw-r--   0 palau     (1000) palau     (1000)      701 2023-02-25 12:47:33.000000 elegantt-0.0.2/elegantt/utils.py
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2023-02-26 00:31:53.790542 elegantt-0.0.2/elegantt.egg-info/
--rw-rw-r--   0 palau     (1000) palau     (1000)     1653 2023-02-26 00:31:53.000000 elegantt-0.0.2/elegantt.egg-info/PKG-INFO
--rw-rw-r--   0 palau     (1000) palau     (1000)      448 2023-02-26 00:31:53.000000 elegantt-0.0.2/elegantt.egg-info/SOURCES.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)        1 2023-02-26 00:31:53.000000 elegantt-0.0.2/elegantt.egg-info/dependency_links.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)       70 2023-02-26 00:31:53.000000 elegantt-0.0.2/elegantt.egg-info/entry_points.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)       14 2023-02-26 00:31:53.000000 elegantt-0.0.2/elegantt.egg-info/requires.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)        9 2023-02-26 00:31:53.000000 elegantt-0.0.2/elegantt.egg-info/top_level.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)       38 2023-02-26 00:31:53.796542 elegantt-0.0.2/setup.cfg
--rw-rw-r--   0 palau     (1000) palau     (1000)      797 2023-02-26 00:26:08.000000 elegantt-0.0.2/setup.py
+drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.653662 elegantt-0.0.3/
+-rw-rw-r--   0 palau     (1000) palau     (1000)     1065 2023-02-23 05:08:13.000000 elegantt-0.0.3/LICENSE
+-rw-rw-r--   0 palau     (1000) palau     (1000)       68 2023-02-25 08:35:15.000000 elegantt-0.0.3/MANIFEST.in
+-rw-rw-r--   0 palau     (1000) palau     (1000)     1653 2024-04-28 14:36:40.653662 elegantt-0.0.3/PKG-INFO
+-rw-rw-r--   0 palau     (1000) palau     (1000)      801 2023-02-25 13:31:13.000000 elegantt-0.0.3/README.md
+drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.645662 elegantt-0.0.3/elegantt/
+-rw-rw-r--   0 palau     (1000) palau     (1000)       91 2023-02-25 13:16:30.000000 elegantt-0.0.3/elegantt/__init__.py
+-rw-rw-r--   0 palau     (1000) palau     (1000)      692 2023-02-25 13:50:25.000000 elegantt-0.0.3/elegantt/command.py
+-rw-rw-r--   0 palau     (1000) palau     (1000)     7388 2024-04-28 13:53:18.000000 elegantt-0.0.3/elegantt/elegantt.py
+drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.644662 elegantt-0.0.3/elegantt/tests/
+drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.645662 elegantt-0.0.3/elegantt/tests/ipaexg/
+-rw-rw-r--   0 palau     (1000) palau     (1000)    20564 2023-02-23 02:32:09.000000 elegantt-0.0.3/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)     1710 2023-02-23 02:32:14.000000 elegantt-0.0.3/elegantt/tests/ipaexg/Readme_ipaexg00401.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)  6099900 2023-02-23 02:32:13.000000 elegantt-0.0.3/elegantt/tests/ipaexg/ipaexg.ttf
+-rw-rw-r--   0 palau     (1000) palau     (1000)      701 2023-02-25 12:47:33.000000 elegantt-0.0.3/elegantt/utils.py
+drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.645662 elegantt-0.0.3/elegantt.egg-info/
+-rw-rw-r--   0 palau     (1000) palau     (1000)     1653 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/PKG-INFO
+-rw-rw-r--   0 palau     (1000) palau     (1000)      448 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/SOURCES.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)        1 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/dependency_links.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)       70 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/entry_points.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)       14 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/requires.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)        9 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/top_level.txt
+-rw-rw-r--   0 palau     (1000) palau     (1000)       38 2024-04-28 14:36:40.653662 elegantt-0.0.3/setup.cfg
+-rw-rw-r--   0 palau     (1000) palau     (1000)      798 2024-04-28 14:31:28.000000 elegantt-0.0.3/setup.py
```

### Comparing `elegantt-0.0.2/LICENSE` & `elegantt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/PKG-INFO` & `elegantt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegantt
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a gantt chart drawing library
 Home-page: http://github.com/usop4/elegantt
 Author: Takayuki Uehara
 Author-email: t.uehara@gmail.com
 License: UNKNOWN
 Description: # elegantt
```

### Comparing `elegantt-0.0.2/README.md` & `elegantt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/elegantt/command.py` & `elegantt-0.0.3/elegantt/command.py`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/elegantt/elegantt.py` & `elegantt-0.0.3/elegantt/elegantt.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,16 @@
             fill = self.font_color, 
             font = ImageFont.truetype(self.font_regular, self.font_size)
         )
         self.num = self.num + 1
 
     def draw_calendar(self):
 
-        week_str = ['月','火','水','木','金','土','日']
+        week_str = ['Mon ','Tue','Wed','Thu','Fri','Sat','Sun']
+        #week_str = ['月','火','水','木','金','土','日']
 
         for i in range(self.max_day):
             
             d = self.monday+datetime.timedelta(days=i)
 
             if d.weekday() in [5,6]: #土日は背景を灰色にする
                 self.draw.rectangle(
```

### Comparing `elegantt-0.0.2/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt` & `elegantt-0.0.3/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/elegantt/tests/ipaexg/Readme_ipaexg00401.txt` & `elegantt-0.0.3/elegantt/tests/ipaexg/Readme_ipaexg00401.txt`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/elegantt/tests/ipaexg/ipaexg.ttf` & `elegantt-0.0.3/elegantt/tests/ipaexg/ipaexg.ttf`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/elegantt/utils.py` & `elegantt-0.0.3/elegantt/utils.py`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.2/elegantt.egg-info/PKG-INFO` & `elegantt-0.0.3/elegantt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegantt
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a gantt chart drawing library
 Home-page: http://github.com/usop4/elegantt
 Author: Takayuki Uehara
 Author-email: t.uehara@gmail.com
 License: UNKNOWN
 Description: # elegantt
```

### Comparing `elegantt-0.0.2/setup.py` & `elegantt-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='elegantt',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
 
     author='Takayuki Uehara',
     author_email='t.uehara@gmail.com',
 
     url='http://github.com/usop4/elegantt',
 
@@ -28,8 +28,8 @@
     ],
 
     entry_points="""
        [console_scripts]
        elegantt = elegantt.command:main
     """,
 
-)
+)
```

