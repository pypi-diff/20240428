# Comparing `tmp/pgpyui-0.0.5.tar.gz` & `tmp/pgpyui-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpyui-0.0.5.tar", last modified: Sun Apr 28 11:39:58 2024, max compression
+gzip compressed data, was "pgpyui-0.0.6.tar", last modified: Sun Apr 28 13:06:37 2024, max compression
```

## Comparing `pgpyui-0.0.5.tar` & `pgpyui-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 11:39:58.377900 pgpyui-0.0.5/
--rw-rw-rw-   0        0        0     3609 2024-04-28 11:39:58.376917 pgpyui-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3023 2024-04-28 11:35:37.000000 pgpyui-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 11:39:58.370874 pgpyui-0.0.5/pgpyui/
--rw-rw-rw-   0        0        0      149 2024-04-28 11:37:14.000000 pgpyui-0.0.5/pgpyui/__init__.py
--rw-rw-rw-   0        0        0     2284 2024-04-25 14:17:42.000000 pgpyui-0.0.5/pgpyui/button.py
--rw-rw-rw-   0        0        0     2451 2024-04-28 11:31:24.000000 pgpyui-0.0.5/pgpyui/checkbox.py
--rw-rw-rw-   0        0        0     2608 2024-04-28 11:21:59.000000 pgpyui-0.0.5/pgpyui/slider.py
--rw-rw-rw-   0        0        0     6072 2024-04-28 11:21:52.000000 pgpyui-0.0.5/pgpyui/textarea.py
-drwxrwxrwx   0        0        0        0 2024-04-28 11:39:58.375886 pgpyui-0.0.5/pgpyui.egg-info/
--rw-rw-rw-   0        0        0     3609 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 11:39:58.000000 pgpyui-0.0.5/pgpyui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 11:39:58.378885 pgpyui-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-04-26 13:50:08.000000 pgpyui-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:06:37.004277 pgpyui-0.0.6/
+-rw-rw-rw-   0        0        0     4214 2024-04-28 13:06:37.003276 pgpyui-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3636 2024-04-28 13:04:55.000000 pgpyui-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 13:06:36.996280 pgpyui-0.0.6/pgpyui/
+-rw-rw-rw-   0        0        0      149 2024-04-28 11:37:14.000000 pgpyui-0.0.6/pgpyui/__init__.py
+-rw-rw-rw-   0        0        0     2284 2024-04-25 14:17:42.000000 pgpyui-0.0.6/pgpyui/button.py
+-rw-rw-rw-   0        0        0     2451 2024-04-28 11:31:24.000000 pgpyui-0.0.6/pgpyui/checkbox.py
+-rw-rw-rw-   0        0        0     2608 2024-04-28 11:21:59.000000 pgpyui-0.0.6/pgpyui/slider.py
+-rw-rw-rw-   0        0        0     6072 2024-04-28 11:21:52.000000 pgpyui-0.0.6/pgpyui/textarea.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:06:37.002275 pgpyui-0.0.6/pgpyui.egg-info/
+-rw-rw-rw-   0        0        0     4214 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:06:37.004277 pgpyui-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-04-28 12:58:58.000000 pgpyui-0.0.6/setup.py
```

### Comparing `pgpyui-0.0.5/PKG-INFO` & `pgpyui-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.5
+Version: 0.0.6
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
 
-# pgpyui 0.0.5
+# pgpyui 0.0.6
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -30,15 +30,15 @@
 
 Imports
 ```python
 from pgpyui import button
 import pygame
 ```
 
-РЎreating a button
+Creating a button
 ```python
 button = button.Button((100, 100), (200, 100), "Some text", func, sprite="sprites/sprite.png")
 ```
 
 Event handling
 ```python
 button.check_events(event)
@@ -53,15 +53,15 @@
 
 Imports
 ```python
 from pgpyui import textarea
 import pygame
 ```
 
-РЎreating a text area
+Creating a text area
 ```python
 textarea = textarea.TextArea((200, 100), (100, 100), 20, 15, is_enter=False, font="Arial")
 ```
 
 Event handling
 ```python
 textarea.check_events(event)
@@ -82,15 +82,15 @@
 
 Imports
 ```python
 from pgpyui import slider
 import pygame
 ```
 
-РЎreating a slider
+Creating a slider
 ```python
 slider = slider.Slider((200, 100), (100, 100), 100, orientation="True")
 ```
 
 Event handling
 ```python
 slider.check_events(event)
@@ -107,19 +107,19 @@
 ```
 
 #
 ### CheckBox
 
 Imports
 ```python
-from pgpyui import slider
+from pgpyui import checkbox
 import pygame
 ```
 
-РЎreating a checkbox
+Creating a checkbox
 ```python
 chkbox = checkbox.CheckBox((100, 100), (50, 50), 3, 75, color=(0, 0, 0), ["passive.png", "active.png"])
 ```
 
 Event handling
 ```python
 chkbox.check_events(event)
@@ -131,14 +131,43 @@
 ```
 
 Information output
 ```python
 prgrs: list = chkbox.data_return()
 ```
 
+#
+### Radio-button
+
+Imports
+```python
+from pgpyui import radio
+import pygame
+```
+
+Creating a radio-button
+```python
+radiob = radio.Radio((100, 100), 25, 10, 100)
+```
+
+Event handling
+```python
+radiob.check_events(event)
+```
+
+Drawing
+```python
+radiob.draw(window)
+```
+
+Information output
+```python
+rt: list = radiob.data_return()
+```
+
 ## Documentation
 
 ### Button
 
 **Parameters:**
 
 * `position`: The position of the button.
@@ -169,20 +198,31 @@
 * `orientation`: Horisontal or vertical slider. (optional)
 
 ### CheckBox
 
 **Parameters:**
 
 * `position`: The position of the CheckBox.
-* `size`: The size of the block Check_box.
+* `size`: The size of the block Checkbox.
 * `num_boxes`: The num of CheckBoxes.
 * `step`: The distance between the boxes.
 * `color`: Color of the box. (optional)
 * `sprites`: Two sprites - the first without a check mark, the second with a check mark. (optional)
 
+### Radio-button
+
+**Parameters:**
+
+* `position`: The position of the radio-button.
+* `radius`: Radius of radio-button.
+* `num_rb`: The num of radio-buttons.
+* `step`: The distance between the buttons.
+* `color`: Color of the box. (optional)
+
+
 ## License
 
 MIT
 
 ## Author mail
 
 mixail.vilyukov@icloud.com
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pgpyui-0.0.5/README.md` & `pgpyui-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pgpyui 0.0.5
+# pgpyui 0.0.6
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -14,15 +14,15 @@
 
 Imports
 ```python
 from pgpyui import button
 import pygame
 ```
 
-Сreating a button
+Creating a button
 ```python
 button = button.Button((100, 100), (200, 100), "Some text", func, sprite="sprites/sprite.png")
 ```
 
 Event handling
 ```python
 button.check_events(event)
@@ -37,15 +37,15 @@
 
 Imports
 ```python
 from pgpyui import textarea
 import pygame
 ```
 
-Сreating a text area
+Creating a text area
 ```python
 textarea = textarea.TextArea((200, 100), (100, 100), 20, 15, is_enter=False, font="Arial")
 ```
 
 Event handling
 ```python
 textarea.check_events(event)
@@ -66,15 +66,15 @@
 
 Imports
 ```python
 from pgpyui import slider
 import pygame
 ```
 
-Сreating a slider
+Creating a slider
 ```python
 slider = slider.Slider((200, 100), (100, 100), 100, orientation="True")
 ```
 
 Event handling
 ```python
 slider.check_events(event)
@@ -91,19 +91,19 @@
 ```
 
 #
 ### CheckBox
 
 Imports
 ```python
-from pgpyui import slider
+from pgpyui import checkbox
 import pygame
 ```
 
-Сreating a checkbox
+Creating a checkbox
 ```python
 chkbox = checkbox.CheckBox((100, 100), (50, 50), 3, 75, color=(0, 0, 0), ["passive.png", "active.png"])
 ```
 
 Event handling
 ```python
 chkbox.check_events(event)
@@ -115,14 +115,43 @@
 ```
 
 Information output
 ```python
 prgrs: list = chkbox.data_return()
 ```
 
+#
+### Radio-button
+
+Imports
+```python
+from pgpyui import radio
+import pygame
+```
+
+Creating a radio-button
+```python
+radiob = radio.Radio((100, 100), 25, 10, 100)
+```
+
+Event handling
+```python
+radiob.check_events(event)
+```
+
+Drawing
+```python
+radiob.draw(window)
+```
+
+Information output
+```python
+rt: list = radiob.data_return()
+```
+
 ## Documentation
 
 ### Button
 
 **Parameters:**
 
 * `position`: The position of the button.
@@ -153,20 +182,31 @@
 * `orientation`: Horisontal or vertical slider. (optional)
 
 ### CheckBox
 
 **Parameters:**
 
 * `position`: The position of the CheckBox.
-* `size`: The size of the block Check_box.
+* `size`: The size of the block Checkbox.
 * `num_boxes`: The num of CheckBoxes.
 * `step`: The distance between the boxes.
 * `color`: Color of the box. (optional)
 * `sprites`: Two sprites - the first without a check mark, the second with a check mark. (optional)
 
+### Radio-button
+
+**Parameters:**
+
+* `position`: The position of the radio-button.
+* `radius`: Radius of radio-button.
+* `num_rb`: The num of radio-buttons.
+* `step`: The distance between the buttons.
+* `color`: Color of the box. (optional)
+
+
 ## License
 
 MIT
 
 ## Author mail
 
 mixail.vilyukov@icloud.com
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pgpyui-0.0.5/pgpyui/button.py` & `pgpyui-0.0.6/pgpyui/button.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.5/pgpyui/checkbox.py` & `pgpyui-0.0.6/pgpyui/checkbox.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.5/pgpyui/slider.py` & `pgpyui-0.0.6/pgpyui/slider.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.5/pgpyui/textarea.py` & `pgpyui-0.0.6/pgpyui/textarea.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.5/pgpyui.egg-info/PKG-INFO` & `pgpyui-0.0.6/pgpyui.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.5
+Version: 0.0.6
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
 
-# pgpyui 0.0.5
+# pgpyui 0.0.6
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -30,15 +30,15 @@
 
 Imports
 ```python
 from pgpyui import button
 import pygame
 ```
 
-РЎreating a button
+Creating a button
 ```python
 button = button.Button((100, 100), (200, 100), "Some text", func, sprite="sprites/sprite.png")
 ```
 
 Event handling
 ```python
 button.check_events(event)
@@ -53,15 +53,15 @@
 
 Imports
 ```python
 from pgpyui import textarea
 import pygame
 ```
 
-РЎreating a text area
+Creating a text area
 ```python
 textarea = textarea.TextArea((200, 100), (100, 100), 20, 15, is_enter=False, font="Arial")
 ```
 
 Event handling
 ```python
 textarea.check_events(event)
@@ -82,15 +82,15 @@
 
 Imports
 ```python
 from pgpyui import slider
 import pygame
 ```
 
-РЎreating a slider
+Creating a slider
 ```python
 slider = slider.Slider((200, 100), (100, 100), 100, orientation="True")
 ```
 
 Event handling
 ```python
 slider.check_events(event)
@@ -107,19 +107,19 @@
 ```
 
 #
 ### CheckBox
 
 Imports
 ```python
-from pgpyui import slider
+from pgpyui import checkbox
 import pygame
 ```
 
-РЎreating a checkbox
+Creating a checkbox
 ```python
 chkbox = checkbox.CheckBox((100, 100), (50, 50), 3, 75, color=(0, 0, 0), ["passive.png", "active.png"])
 ```
 
 Event handling
 ```python
 chkbox.check_events(event)
@@ -131,14 +131,43 @@
 ```
 
 Information output
 ```python
 prgrs: list = chkbox.data_return()
 ```
 
+#
+### Radio-button
+
+Imports
+```python
+from pgpyui import radio
+import pygame
+```
+
+Creating a radio-button
+```python
+radiob = radio.Radio((100, 100), 25, 10, 100)
+```
+
+Event handling
+```python
+radiob.check_events(event)
+```
+
+Drawing
+```python
+radiob.draw(window)
+```
+
+Information output
+```python
+rt: list = radiob.data_return()
+```
+
 ## Documentation
 
 ### Button
 
 **Parameters:**
 
 * `position`: The position of the button.
@@ -169,20 +198,31 @@
 * `orientation`: Horisontal or vertical slider. (optional)
 
 ### CheckBox
 
 **Parameters:**
 
 * `position`: The position of the CheckBox.
-* `size`: The size of the block Check_box.
+* `size`: The size of the block Checkbox.
 * `num_boxes`: The num of CheckBoxes.
 * `step`: The distance between the boxes.
 * `color`: Color of the box. (optional)
 * `sprites`: Two sprites - the first without a check mark, the second with a check mark. (optional)
 
+### Radio-button
+
+**Parameters:**
+
+* `position`: The position of the radio-button.
+* `radius`: Radius of radio-button.
+* `num_rb`: The num of radio-buttons.
+* `step`: The distance between the buttons.
+* `color`: Color of the box. (optional)
+
+
 ## License
 
 MIT
 
 ## Author mail
 
 mixail.vilyukov@icloud.com
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pgpyui-0.0.5/setup.py` & `pgpyui-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='pgpyui',
-  version='0.0.5',
+  version='0.0.6',
   author='Memdved',
   author_email='mixail.vilyukov@icloud.com',
   description='The package is an add-on for Pygame to create a user interface on the screen.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://pypi.org/project/pgpyui/',
   packages=find_packages(),
```

