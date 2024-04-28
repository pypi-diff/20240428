# Comparing `tmp/pgpyui-0.0.4.tar.gz` & `tmp/pgpyui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpyui-0.0.4.tar", last modified: Thu Apr 25 17:14:01 2024, max compression
+gzip compressed data, was "pgpyui-0.0.5.tar", last modified: Sun Apr 28 11:39:58 2024, max compression
```

## Comparing `pgpyui-0.0.4.tar` & `pgpyui-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 17:14:01.662493 pgpyui-0.0.4/
--rw-rw-rw-   0        0        0     2847 2024-04-25 17:14:01.662493 pgpyui-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2263 2024-04-25 17:01:35.000000 pgpyui-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 17:14:01.654494 pgpyui-0.0.4/pgpyui/
--rw-rw-rw-   0        0        0      149 2024-04-25 13:54:47.000000 pgpyui-0.0.4/pgpyui/__init__.py
--rw-rw-rw-   0        0        0     2284 2024-04-25 14:17:42.000000 pgpyui-0.0.4/pgpyui/button.py
--rw-rw-rw-   0        0        0     2612 2024-04-25 17:12:21.000000 pgpyui-0.0.4/pgpyui/slider.py
--rw-rw-rw-   0        0        0     6073 2024-04-25 13:19:16.000000 pgpyui-0.0.4/pgpyui/textarea.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:14:01.661502 pgpyui-0.0.4/pgpyui.egg-info/
--rw-rw-rw-   0        0        0     2847 2024-04-25 17:14:01.000000 pgpyui-0.0.4/pgpyui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-25 17:14:01.000000 pgpyui-0.0.4/pgpyui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 17:14:01.000000 pgpyui-0.0.4/pgpyui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-25 17:14:01.000000 pgpyui-0.0.4/pgpyui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 17:14:01.000000 pgpyui-0.0.4/pgpyui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 17:14:01.663498 pgpyui-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-04-25 13:46:21.000000 pgpyui-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:39:58.377900 pgpyui-0.0.5/
+-rw-rw-rw-   0        0        0     3609 2024-04-28 11:39:58.376917 pgpyui-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3023 2024-04-28 11:35:37.000000 pgpyui-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 11:39:58.370874 pgpyui-0.0.5/pgpyui/
+-rw-rw-rw-   0        0        0      149 2024-04-28 11:37:14.000000 pgpyui-0.0.5/pgpyui/__init__.py
+-rw-rw-rw-   0        0        0     2284 2024-04-25 14:17:42.000000 pgpyui-0.0.5/pgpyui/button.py
+-rw-rw-rw-   0        0        0     2451 2024-04-28 11:31:24.000000 pgpyui-0.0.5/pgpyui/checkbox.py
+-rw-rw-rw-   0        0        0     2608 2024-04-28 11:21:59.000000 pgpyui-0.0.5/pgpyui/slider.py
+-rw-rw-rw-   0        0        0     6072 2024-04-28 11:21:52.000000 pgpyui-0.0.5/pgpyui/textarea.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:39:58.375886 pgpyui-0.0.5/pgpyui.egg-info/
+-rw-rw-rw-   0        0        0     3609 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 11:39:58.378885 pgpyui-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-04-26 13:50:08.000000 pgpyui-0.0.5/setup.py
```

### Comparing `pgpyui-0.0.4/PKG-INFO` & `pgpyui-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1
-Name: pgpyui
-Version: 0.0.4
-Summary: The package is an add-on for Pygame to create a user interface on the screen.
-Home-page: https://pypi.org/project/pgpyui/
-Author: Memdved
-Author-email: mixail.vilyukov@icloud.com
-Project-URL: GitHub, https://github.com/Memdved
-Keywords: ui gui pgpyui pygame
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: requests>=2.25.1
-
-# pgpyui 0.0.4
+# pgpyui 0.0.5
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -30,15 +14,15 @@
 
 Imports
 ```python
 from pgpyui import button
 import pygame
 ```
 
-РЎreating a button
+Сreating a button
 ```python
 button = button.Button((100, 100), (200, 100), "Some text", func, sprite="sprites/sprite.png")
 ```
 
 Event handling
 ```python
 button.check_events(event)
@@ -53,15 +37,15 @@
 
 Imports
 ```python
 from pgpyui import textarea
 import pygame
 ```
 
-РЎreating a text area
+Сreating a text area
 ```python
 textarea = textarea.TextArea((200, 100), (100, 100), 20, 15, is_enter=False, font="Arial")
 ```
 
 Event handling
 ```python
 textarea.check_events(event)
@@ -70,27 +54,27 @@
 Drawing
 ```python
 textarea.draw(window)
 ```
 
 Information output
 ```python
-text: list[str] = textarea.return_texts()
+text: list[str] = textarea.data_return()
 ```
 
 #
 ### Slider
 
 Imports
 ```python
 from pgpyui import slider
 import pygame
 ```
 
-РЎreating a slider
+Сreating a slider
 ```python
 slider = slider.Slider((200, 100), (100, 100), 100, orientation="True")
 ```
 
 Event handling
 ```python
 slider.check_events(event)
@@ -99,15 +83,44 @@
 Drawing
 ```python
 slider.draw(window)
 ```
 
 Information output
 ```python
-prgrs: int = slider.return_progress()
+prgrs: int = slider.data_return()
+```
+
+#
+### CheckBox
+
+Imports
+```python
+from pgpyui import slider
+import pygame
+```
+
+Сreating a checkbox
+```python
+chkbox = checkbox.CheckBox((100, 100), (50, 50), 3, 75, color=(0, 0, 0), ["passive.png", "active.png"])
+```
+
+Event handling
+```python
+chkbox.check_events(event)
+```
+
+Drawing
+```python
+chkbox.draw(window)
+```
+
+Information output
+```python
+prgrs: list = chkbox.data_return()
 ```
 
 ## Documentation
 
 ### Button
 
 **Parameters:**
@@ -135,14 +148,24 @@
 
 * `position`: The position of the slider.
 * `size_block`: The size of the block slider.
 * `len`: Length of slide.
 * `max_symbols`: The maximum number of symbols that can be entered.
 * `orientation`: Horisontal or vertical slider. (optional)
 
+### CheckBox
+
+**Parameters:**
+
+* `position`: The position of the CheckBox.
+* `size`: The size of the block Check_box.
+* `num_boxes`: The num of CheckBoxes.
+* `step`: The distance between the boxes.
+* `color`: Color of the box. (optional)
+* `sprites`: Two sprites - the first without a check mark, the second with a check mark. (optional)
 
 ## License
 
 MIT
 
 ## Author mail
```

### Comparing `pgpyui-0.0.4/pgpyui/button.py` & `pgpyui-0.0.5/pgpyui/button.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.4/pgpyui/slider.py` & `pgpyui-0.0.5/pgpyui/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 self.__is_push = True
         if event.type == pygame.MOUSEBUTTONUP:
             if event.button == 1:
                 self.__is_push = False
         
         self.__move()
 
-    def return_progress(self):
+    def data_return(self):
         progress: int
         if not self.__orientation:
             progress = int(round(self.__rectangle.centerx / self.__finish[0], 2) * 100)
         else:
             progress = int(round(self.__rectangle.centery / self.__finish[1], 2) * 100)
 
         return progress
```

### Comparing `pgpyui-0.0.4/pgpyui/textarea.py` & `pgpyui-0.0.5/pgpyui/textarea.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,14 @@
             elif keys[pygame.K_SLASH]:
                 self.__add_symbol('backspace')
                 self.__add_symbol("?")
         else:
             self.__register = False
         
 
-    def return_texts(self) -> list:
+    def data_return(self) -> list:
         """
         Function for return all text in text area.
 
         :return: Text in text area.
         """
         return self.__texts
```

### Comparing `pgpyui-0.0.4/pgpyui.egg-info/PKG-INFO` & `pgpyui-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.4
+Version: 0.0.5
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
-# pgpyui 0.0.4
+# pgpyui 0.0.5
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -70,15 +70,15 @@
 Drawing
 ```python
 textarea.draw(window)
 ```
 
 Information output
 ```python
-text: list[str] = textarea.return_texts()
+text: list[str] = textarea.data_return()
 ```
 
 #
 ### Slider
 
 Imports
 ```python
@@ -99,15 +99,44 @@
 Drawing
 ```python
 slider.draw(window)
 ```
 
 Information output
 ```python
-prgrs: int = slider.return_progress()
+prgrs: int = slider.data_return()
+```
+
+#
+### CheckBox
+
+Imports
+```python
+from pgpyui import slider
+import pygame
+```
+
+РЎreating a checkbox
+```python
+chkbox = checkbox.CheckBox((100, 100), (50, 50), 3, 75, color=(0, 0, 0), ["passive.png", "active.png"])
+```
+
+Event handling
+```python
+chkbox.check_events(event)
+```
+
+Drawing
+```python
+chkbox.draw(window)
+```
+
+Information output
+```python
+prgrs: list = chkbox.data_return()
 ```
 
 ## Documentation
 
 ### Button
 
 **Parameters:**
@@ -135,14 +164,24 @@
 
 * `position`: The position of the slider.
 * `size_block`: The size of the block slider.
 * `len`: Length of slide.
 * `max_symbols`: The maximum number of symbols that can be entered.
 * `orientation`: Horisontal or vertical slider. (optional)
 
+### CheckBox
+
+**Parameters:**
+
+* `position`: The position of the CheckBox.
+* `size`: The size of the block Check_box.
+* `num_boxes`: The num of CheckBoxes.
+* `step`: The distance between the boxes.
+* `color`: Color of the box. (optional)
+* `sprites`: Two sprites - the first without a check mark, the second with a check mark. (optional)
 
 ## License
 
 MIT
 
 ## Author mail
```

### Comparing `pgpyui-0.0.4/setup.py` & `pgpyui-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='pgpyui',
-  version='0.0.4',
+  version='0.0.5',
   author='Memdved',
   author_email='mixail.vilyukov@icloud.com',
   description='The package is an add-on for Pygame to create a user interface on the screen.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://pypi.org/project/pgpyui/',
   packages=find_packages(),
```

