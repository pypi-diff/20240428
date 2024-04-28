# Comparing `tmp/input_devices-0.1.1.tar.gz` & `tmp/input_devices-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "input_devices-0.1.1.tar", last modified: Fri Apr 26 20:50:45 2024, max compression
+gzip compressed data, was "input_devices-0.1.2.tar", last modified: Sun Apr 28 07:10:56 2024, max compression
```

## Comparing `input_devices-0.1.1.tar` & `input_devices-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 20:50:45.034027 input_devices-0.1.1/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1070 2024-04-19 22:25:44.000000 input_devices-0.1.1/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     3176 2024-04-26 20:50:45.034027 input_devices-0.1.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     2604 2024-04-20 04:46:30.000000 input_devices-0.1.1/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 20:50:45.034027 input_devices-0.1.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      865 2024-04-26 20:50:44.000000 input_devices-0.1.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 20:50:45.034027 input_devices-0.1.1/src/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 20:50:45.034027 input_devices-0.1.1/src/input_devices.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     3176 2024-04-26 20:50:45.000000 input_devices-0.1.1/src/input_devices.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      472 2024-04-26 20:50:45.000000 input_devices-0.1.1/src/input_devices.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 20:50:45.000000 input_devices-0.1.1/src/input_devices.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 20:50:45.000000 input_devices-0.1.1/src/input_devices.egg-info/not-zip-safe
--rw-rw-r--   0 mark      (1000) mark      (1000)        7 2024-04-26 20:50:45.000000 input_devices-0.1.1/src/input_devices.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       23 2024-04-26 20:50:45.000000 input_devices-0.1.1/src/input_devices.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 20:50:45.034027 input_devices-0.1.1/src/shared/
--rw-rw-r--   0 mark      (1000) mark      (1000)      134 2024-04-19 22:28:04.000000 input_devices-0.1.1/src/shared/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6904 2024-04-20 03:59:37.000000 input_devices-0.1.1/src/shared/axis_input.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1697 2024-04-20 03:59:37.000000 input_devices-0.1.1/src/shared/axis_trigger.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3685 2024-04-19 22:26:53.000000 input_devices-0.1.1/src/shared/button.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      605 2024-04-19 22:26:53.000000 input_devices-0.1.1/src/shared/directional_pad.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 20:50:45.034027 input_devices-0.1.1/src/xbox_controller/
--rw-rw-r--   0 mark      (1000) mark      (1000)       52 2024-04-19 23:46:00.000000 input_devices-0.1.1/src/xbox_controller/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4305 2024-04-20 04:00:54.000000 input_devices-0.1.1/src/xbox_controller/xbox_controller_gen4.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 07:10:56.182688 input_devices-0.1.2/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1070 2024-04-19 22:25:44.000000 input_devices-0.1.2/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3177 2024-04-28 07:10:56.182688 input_devices-0.1.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2605 2024-04-28 07:09:26.000000 input_devices-0.1.2/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 07:10:56.182688 input_devices-0.1.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      894 2024-04-28 07:10:55.000000 input_devices-0.1.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 07:10:56.182688 input_devices-0.1.2/src/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 07:10:56.182688 input_devices-0.1.2/src/input_devices/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       30 2024-04-28 07:05:44.000000 input_devices-0.1.2/src/input_devices/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 07:10:56.182688 input_devices-0.1.2/src/input_devices.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3177 2024-04-28 07:10:56.000000 input_devices-0.1.2/src/input_devices.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      300 2024-04-28 07:10:56.000000 input_devices-0.1.2/src/input_devices.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 07:10:56.000000 input_devices-0.1.2/src/input_devices.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 07:10:56.000000 input_devices-0.1.2/src/input_devices.egg-info/not-zip-safe
+-rw-rw-r--   0 mark      (1000) mark      (1000)        7 2024-04-28 07:10:56.000000 input_devices-0.1.2/src/input_devices.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-28 07:10:56.000000 input_devices-0.1.2/src/input_devices.egg-info/top_level.txt
```

### Comparing `input_devices-0.1.1/LICENSE` & `input_devices-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `input_devices-0.1.1/PKG-INFO` & `input_devices-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: input_devices
-Version: 0.1.1
-Summary: high level API wrapper around inputs library for working with input devices like gamepads, joysticks, etc.
+Version: 0.1.2
+Summary: High level API wrapper around inputs library for working with input devices like gamepads, joysticks, etc.
 Home-page: https://github.com/MarikTik/input_devices
 Author: Mark Tikhonov
 Author-email: mtik.philosopher@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,18 @@
 
 # input_devices
 
 `input_devices` is a Python library designed to provide a high-level API for interacting with various electronic input devices. This includes game controllers (such as Xbox and PlayStation controllers), joysticks, remote controllers, as well as computer peripherals like keyboards and mice. The goal of `input_devices` is to simplify the process of integrating these devices into Python projects by offering a straightforward and unified interface.
 
 ## Features
 
-- **Game Controllers**: Support for Xbox and PlayStation controllers.
+- **Game Controllers**: Support for Xbox Gen4 controllers.
+
+## Future
+
 - **Joysticks**: Compatibility with various models of joysticks.
 - **Remote Controllers**: Integration with different types of remote control devices.
 - **Computer Peripherals**: Support for keyboards and mice, facilitating complex input handling.
 - **Extensible**: Designed to be easily extendable for more types of devices.
 
 ## Installation
```

### Comparing `input_devices-0.1.1/README.md` & `input_devices-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # input_devices
 
 `input_devices` is a Python library designed to provide a high-level API for interacting with various electronic input devices. This includes game controllers (such as Xbox and PlayStation controllers), joysticks, remote controllers, as well as computer peripherals like keyboards and mice. The goal of `input_devices` is to simplify the process of integrating these devices into Python projects by offering a straightforward and unified interface.
 
 ## Features
 
-- **Game Controllers**: Support for Xbox and PlayStation controllers.
+- **Game Controllers**: Support for Xbox Gen4 controllers.
+
+## Future
+
 - **Joysticks**: Compatibility with various models of joysticks.
 - **Remote Controllers**: Integration with different types of remote control devices.
 - **Computer Peripherals**: Support for keyboards and mice, facilitating complex input handling.
 - **Extensible**: Designed to be easily extendable for more types of devices.
 
 ## Installation
```

### Comparing `input_devices-0.1.1/setup.py` & `input_devices-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 from setuptools import setup, find_packages
 
-
-with open('README.md') as f:
-    long_description = f.read()
-
 setup(
     name='input_devices',
-    version='0.1.1',
-    description='high level API wrapper around inputs library for working with input devices like gamepads, joysticks, etc.',
-    long_description=long_description,
+    version='0.1.2',
+    description='High level API wrapper around inputs library for working with input devices like gamepads, joysticks, etc.',
+    long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MarikTik/input_devices',
     author='Mark Tikhonov',
     author_email='mtik.philosopher@gmail.com',
     license='MIT',
-    packages=find_packages('src'),
-    install_requires=[
-        'inputs'
-    ],
+    package_dir={'': 'src'},  # Set 'src' as the root directory for packages
+    packages=['input_devices'],  # Find all packages in 'src'
+    install_requires=['inputs'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
-    zip_safe=False,
-    package_dir={'': 'src'}
+    zip_safe=False
 )
```

### Comparing `input_devices-0.1.1/src/input_devices.egg-info/PKG-INFO` & `input_devices-0.1.2/src/input_devices.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: input-devices
-Version: 0.1.1
-Summary: high level API wrapper around inputs library for working with input devices like gamepads, joysticks, etc.
+Version: 0.1.2
+Summary: High level API wrapper around inputs library for working with input devices like gamepads, joysticks, etc.
 Home-page: https://github.com/MarikTik/input_devices
 Author: Mark Tikhonov
 Author-email: mtik.philosopher@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,18 @@
 
 # input_devices
 
 `input_devices` is a Python library designed to provide a high-level API for interacting with various electronic input devices. This includes game controllers (such as Xbox and PlayStation controllers), joysticks, remote controllers, as well as computer peripherals like keyboards and mice. The goal of `input_devices` is to simplify the process of integrating these devices into Python projects by offering a straightforward and unified interface.
 
 ## Features
 
-- **Game Controllers**: Support for Xbox and PlayStation controllers.
+- **Game Controllers**: Support for Xbox Gen4 controllers.
+
+## Future
+
 - **Joysticks**: Compatibility with various models of joysticks.
 - **Remote Controllers**: Integration with different types of remote control devices.
 - **Computer Peripherals**: Support for keyboards and mice, facilitating complex input handling.
 - **Extensible**: Designed to be easily extendable for more types of devices.
 
 ## Installation
```

