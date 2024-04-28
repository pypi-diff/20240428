# Comparing `tmp/botnikkk-0.1.2.tar.gz` & `tmp/botnikkk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.1.2.tar", last modified: Tue Apr 16 11:14:46 2024, max compression
+gzip compressed data, was "botnikkk-0.1.3.tar", last modified: Sun Apr 28 11:18:37 2024, max compression
```

## Comparing `botnikkk-0.1.2.tar` & `botnikkk-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 11:14:46.551473 botnikkk-0.1.2/
--rw-rw-rw-   0        0        0     3103 2024-04-16 11:14:46.542996 botnikkk-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2024-04-10 16:40:35.000000 botnikkk-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 11:14:46.537901 botnikkk-0.1.2/botnikkk/
--rw-rw-rw-   0        0        0      212 2024-04-10 15:13:48.000000 botnikkk-0.1.2/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     3208 2024-04-16 11:14:17.000000 botnikkk-0.1.2/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:14:46.542996 botnikkk-0.1.2/botnikkk.egg-info/
--rw-rw-rw-   0        0        0     3103 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 11:14:46.551473 botnikkk-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1000 2024-04-16 11:08:59.000000 botnikkk-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:37.049861 botnikkk-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2024-04-10 17:07:38.000000 botnikkk-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4104 2024-04-28 11:18:37.046463 botnikkk-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3387 2024-04-28 11:14:37.000000 botnikkk-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:37.030437 botnikkk-0.1.3/botnikkk/
+-rw-rw-rw-   0        0        0      212 2024-04-10 17:07:38.000000 botnikkk-0.1.3/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     3681 2024-04-28 11:17:47.000000 botnikkk-0.1.3/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:18:37.044228 botnikkk-0.1.3/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0     4104 2024-04-28 11:18:36.000000 botnikkk-0.1.3/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-04-28 11:18:36.000000 botnikkk-0.1.3/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 11:18:36.000000 botnikkk-0.1.3/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-28 11:18:36.000000 botnikkk-0.1.3/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 11:18:36.000000 botnikkk-0.1.3/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 11:18:37.049861 botnikkk-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-04-28 10:49:49.000000 botnikkk-0.1.3/setup.py
```

### Comparing `botnikkk-0.1.2/botnikkk/formatting.py` & `botnikkk-0.1.3/botnikkk/formatting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 import screeninfo
 import asyncio
 
-
-def get_alignments(string = " "):
+def get_alignments(string= " ", format="auto"):
     screen_width = int((screeninfo.get_monitors()[0].width)/(9.2))
+
     if screen_width < 128 :
         left_align = 0
-        gap = int(screen_width/2)
+        gap = screen_width
+        left_gap = int(screen_width/2) - int(len(string))
+        right_gap = gap - left_gap - len(string)
+
     else :
-        gap = 128
 
-        left_align = (int(screen_width/2) - int(gap/2))
-        left_gap = (int(gap/2) - int(len(string)/2))
-        right_gap = gap - left_gap - len(string)
-    
+        if format == "auto" :
+            gap = 128
+            left_align = (int(screen_width/2) - int(gap/2))
+            left_gap = (int(gap/2) - int(len(string)/2))
+            right_gap = gap - left_gap - len(string)
+
+        elif type(format)  == int :
+            gap = 128
+            left_align = format
+            left_gap = (int(gap/2) - int(len(string)/2))
+            right_gap = gap - left_gap - len(string)
+
+        else :
+            centre("Invalid input")
+            left_align = left_gap = right_gap = gap = None
     return {"left_align" : left_align, "left_gap" : left_gap, "right_gap" : right_gap, "default_gap" : gap }
-
-def centre(title='',symbol=" ",left_alignment=None, str_end="\n") :
+    
+def centre(title='',symbol=" ",format="auto", str_end="\n") :
     #aligns the title in centre with symbols around it
-    alignments = get_alignments(title)
-    left_align = alignments["left_align"]*" "
-    left_gap = alignments["left_gap"]
-    right_gap = alignments["right_gap"]
-    default_gap = alignments["default_gap"]*" "
+    alignments = get_alignments(string=title, format=format)
 
-    if left_alignment != None and type(left_alignment) == int :
-        left_align = left_alignment*" "
+    if None not in alignments.values() :
 
-    if str_end != '\r' :
-        print_string = f"{left_align}|{left_gap*symbol}{title}{right_gap*symbol}|\n{left_align}|{default_gap}|"
+        left_align = alignments["left_align"]*" "
+        left_gap = alignments["left_gap"]
+        right_gap = alignments["right_gap"]
+        default_gap = alignments["default_gap"]*" "
 
-    else :
-        print_string = f"{left_align}|{left_gap*symbol}{title}{right_gap*symbol}|"
+        if str_end != '\r' :
+            print_string = f"{left_align}|{left_gap*symbol}{title}{right_gap*symbol}|\n{left_align}|{default_gap}|"
 
-    print(print_string,end=str_end)
+        else :
+            print_string = f"{left_align}|{left_gap*symbol}{title}{right_gap*symbol}|"
+
+        print(print_string,end=str_end)
 
 def format_input(ques='') : 
     alignments = get_alignments(ques)
-    left_align = alignments["left_align"]*" "
+    left_align = alignments["left_align"]
     left_gap = alignments["left_gap"]*" "
     right_gap = alignments["right_gap"]*" "
 
     string = f"{left_align}|{left_gap}{ques}{right_gap}|\n{left_align}| -"
     output = input(string)
     return output
 
@@ -89,7 +102,8 @@
         gap2 = str(symbol)*(128- len(title) - len(gap))
         centre(title, str_end="\r")
         await asyncio.sleep(1) 
 
 async def redirect(redirect='UNKNOWN'):
     await redirect_function(redirect)
 
+
```

### Comparing `botnikkk-0.1.2/setup.py` & `botnikkk-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'a personal package'
 
 # Setting up
 setup(
     name="botnikkk",
     version=VERSION,
     author="BotNikkk",
```

