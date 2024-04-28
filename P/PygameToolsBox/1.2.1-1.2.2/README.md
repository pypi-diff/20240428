# Comparing `tmp/pygametoolsbox-1.2.1.tar.gz` & `tmp/pygametoolsbox-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygametoolsbox-1.2.1.tar", last modified: Sun Apr 14 23:28:00 2024, max compression
+gzip compressed data, was "pygametoolsbox-1.2.2.tar", last modified: Sun Apr 28 20:42:45 2024, max compression
```

## Comparing `pygametoolsbox-1.2.1.tar` & `pygametoolsbox-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 23:28:00.965778 pygametoolsbox-1.2.1/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 pygametoolsbox-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3717 2024-04-14 23:28:00.965778 pygametoolsbox-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 23:28:00.934502 pygametoolsbox-1.2.1/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-14 23:27:49.000000 pygametoolsbox-1.2.1/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     4513 2024-04-11 01:18:52.000000 pygametoolsbox-1.2.1/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      327 2024-04-08 02:08:23.000000 pygametoolsbox-1.2.1/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 pygametoolsbox-1.2.1/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3891 2024-04-11 00:36:46.000000 pygametoolsbox-1.2.1/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-14 23:28:00.950246 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3717 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3111 2024-04-08 02:33:17.000000 pygametoolsbox-1.2.1/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 pygametoolsbox-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 23:28:00.965778 pygametoolsbox-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 20:42:45.970580 pygametoolsbox-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 pygametoolsbox-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3717 2024-04-28 20:42:45.969580 pygametoolsbox-1.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 20:42:45.941967 pygametoolsbox-1.2.2/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-28 20:42:37.000000 pygametoolsbox-1.2.2/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     4513 2024-04-11 01:18:52.000000 pygametoolsbox-1.2.2/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0     1647 2024-04-28 20:40:28.000000 pygametoolsbox-1.2.2/PygameToolsBox/button.py
+-rw-rw-rw-   0        0        0      327 2024-04-08 02:08:23.000000 pygametoolsbox-1.2.2/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 pygametoolsbox-1.2.2/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3891 2024-04-11 00:36:46.000000 pygametoolsbox-1.2.2/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:42:45.968621 pygametoolsbox-1.2.2/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3717 2024-04-28 20:42:45.000000 pygametoolsbox-1.2.2/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-28 20:42:45.000000 pygametoolsbox-1.2.2/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:42:45.000000 pygametoolsbox-1.2.2/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-28 20:42:45.000000 pygametoolsbox-1.2.2/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-28 20:42:45.000000 pygametoolsbox-1.2.2/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3111 2024-04-08 02:33:17.000000 pygametoolsbox-1.2.2/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 pygametoolsbox-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:42:45.970580 pygametoolsbox-1.2.2/setup.cfg
```

### Comparing `pygametoolsbox-1.2.1/LICENSE` & `pygametoolsbox-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygametoolsbox-1.2.1/PKG-INFO` & `pygametoolsbox-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygametoolsbox-1.2.1/PygameToolsBox/animated_object.py` & `pygametoolsbox-1.2.2/PygameToolsBox/animated_object.py`

 * *Files identical despite different names*

### Comparing `pygametoolsbox-1.2.1/PygameToolsBox/parallax_bg.py` & `pygametoolsbox-1.2.2/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `pygametoolsbox-1.2.1/PygameToolsBox/spritesheet.py` & `pygametoolsbox-1.2.2/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `pygametoolsbox-1.2.1/PygameToolsBox.egg-info/PKG-INFO` & `pygametoolsbox-1.2.2/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygametoolsbox-1.2.1/README.md` & `pygametoolsbox-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pygametoolsbox-1.2.1/pyproject.toml` & `pygametoolsbox-1.2.2/pyproject.toml`

 * *Files identical despite different names*

