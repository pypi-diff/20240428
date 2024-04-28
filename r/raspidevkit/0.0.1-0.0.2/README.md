# Comparing `tmp/raspidevkit-0.0.1.tar.gz` & `tmp/raspidevkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspidevkit-0.0.1.tar", last modified: Sun Apr 14 10:12:24 2024, max compression
+gzip compressed data, was "raspidevkit-0.0.2.tar", last modified: Sun Apr 28 13:13:08 2024, max compression
```

## Comparing `raspidevkit-0.0.1.tar` & `raspidevkit-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:12:24.349725 raspidevkit-0.0.1/
--rw-rw-rw-   0        0        0     1087 2024-04-09 10:52:40.000000 raspidevkit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       48 2024-04-09 10:52:40.000000 raspidevkit-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11087 2024-04-14 10:12:24.346225 raspidevkit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8933 2024-04-09 10:52:40.000000 raspidevkit-0.0.1/README.md
--rw-rw-rw-   0        0        0      838 2024-04-14 09:46:13.000000 raspidevkit-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-14 10:12:24.345225 raspidevkit-0.0.1/raspidevkit.egg-info/
--rw-rw-rw-   0        0        0    11087 2024-04-14 10:12:24.000000 raspidevkit-0.0.1/raspidevkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-14 10:12:24.000000 raspidevkit-0.0.1/raspidevkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:12:24.000000 raspidevkit-0.0.1/raspidevkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-14 10:12:24.000000 raspidevkit-0.0.1/raspidevkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:12:24.000000 raspidevkit-0.0.1/raspidevkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 10:12:24.349725 raspidevkit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2024-04-09 10:52:40.000000 raspidevkit-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:12:24.339603 raspidevkit-0.0.1/tests/
--rw-rw-rw-   0        0        0      335 2024-04-10 11:58:25.000000 raspidevkit-0.0.1/tests/test_arduino.py
--rw-rw-rw-   0        0        0     3094 2024-04-09 10:52:40.000000 raspidevkit-0.0.1/tests/test_drivers.py
--rw-rw-rw-   0        0        0     2553 2024-04-09 10:52:40.000000 raspidevkit-0.0.1/tests/test_gpio_devices.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.818787 raspidevkit-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       48 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11846 2024-04-28 13:13:08.816790 raspidevkit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9692 2024-04-14 10:33:57.000000 raspidevkit-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.723140 raspidevkit-0.0.2/docs/
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.743977 raspidevkit-0.0.2/docs/source/
+-rw-rw-rw-   0        0        0     1124 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0      838 2024-04-28 13:12:56.000000 raspidevkit-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.755688 raspidevkit-0.0.2/raspidevkit/
+-rw-rw-rw-   0        0        0      279 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/__init__.py
+-rw-rw-rw-   0        0        0    18195 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/__interface.py
+-rw-rw-rw-   0        0        0     1291 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/__logger.py
+-rw-rw-rw-   0        0        0      487 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.771684 raspidevkit-0.0.2/raspidevkit/devices/
+-rw-rw-rw-   0        0        0      571 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.775808 raspidevkit-0.0.2/raspidevkit/devices/arduino/
+-rw-rw-rw-   0        0        0     2994 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/arduino/led.py
+-rw-rw-rw-   0        0        0     2606 2024-04-09 10:57:32.000000 raspidevkit-0.0.2/raspidevkit/devices/arduino/servo_motor.py
+-rw-rw-rw-   0        0        0    17228 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/base.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.728200 raspidevkit-0.0.2/raspidevkit/devices/drivers/
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.782334 raspidevkit-0.0.2/raspidevkit/devices/drivers/dc_motor/
+-rw-rw-rw-   0        0        0     6543 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/drivers/dc_motor/base.py
+-rw-rw-rw-   0        0        0     2366 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/drivers/dc_motor/l293d.py
+-rw-rw-rw-   0        0        0     2366 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/drivers/dc_motor/l298n.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.801909 raspidevkit-0.0.2/raspidevkit/devices/gpio/
+-rw-rw-rw-   0        0        0      786 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/button.py
+-rw-rw-rw-   0        0        0     2693 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/buzzer.py
+-rw-rw-rw-   0        0        0     1946 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/led.py
+-rw-rw-rw-   0        0        0     1016 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/light_sensor.py
+-rw-rw-rw-   0        0        0      813 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/pir_motion_sensor.py
+-rw-rw-rw-   0        0        0     1539 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/relay.py
+-rw-rw-rw-   0        0        0     3713 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/rgb_led.py
+-rw-rw-rw-   0        0        0     2810 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/servo_motor.py
+-rw-rw-rw-   0        0        0     1743 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/gpio/ultrasonic_sensor.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.804920 raspidevkit-0.0.2/raspidevkit/devices/serial/
+-rw-rw-rw-   0        0        0    10023 2024-04-09 12:44:52.000000 raspidevkit-0.0.2/raspidevkit/devices/serial/arduino.py
+-rw-rw-rw-   0        0        0     3449 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/devices/serial/sim808.py
+-rw-rw-rw-   0        0        0    10652 2024-04-09 11:40:54.000000 raspidevkit-0.0.2/raspidevkit/machine.py
+-rw-rw-rw-   0        0        0     9103 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/raspidevkit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.814265 raspidevkit-0.0.2/raspidevkit.egg-info/
+-rw-rw-rw-   0        0        0    11846 2024-04-28 13:13:08.000000 raspidevkit-0.0.2/raspidevkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2024-04-28 13:13:08.000000 raspidevkit-0.0.2/raspidevkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:13:08.000000 raspidevkit-0.0.2/raspidevkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-28 13:13:08.000000 raspidevkit-0.0.2/raspidevkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-04-28 13:13:08.000000 raspidevkit-0.0.2/raspidevkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:13:08.818787 raspidevkit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2024-04-28 13:12:42.000000 raspidevkit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:13:08.810850 raspidevkit-0.0.2/tests/
+-rw-rw-rw-   0        0        0      335 2024-04-10 11:58:25.000000 raspidevkit-0.0.2/tests/test_arduino.py
+-rw-rw-rw-   0        0        0     3094 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/tests/test_drivers.py
+-rw-rw-rw-   0        0        0     2553 2024-04-09 10:52:40.000000 raspidevkit-0.0.2/tests/test_gpio_devices.py
```

### Comparing `raspidevkit-0.0.1/LICENSE` & `raspidevkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspidevkit-0.0.1/PKG-INFO` & `raspidevkit-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspidevkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Easily control devices with Raspberry Pi
 Home-page: https://github.com/raspidevkit/raspidevkit
 Author: DailyLollipops
 Author-email: DailyLollipops <clarencemadrigal84@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Raspidevkit
@@ -44,14 +44,15 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # Raspidevkit
 Easily control devices with Raspberry Pi
 
 ## Building
+### Using setuptools
 First, ensure that the `setuptools` and `wheel` packages as installed with
 
 ```bash
 pip install setuptools 
 pip install wheel
 ```
 
@@ -59,14 +60,23 @@
 
 ```bash
 python setup.py sdist bdist_wheel
 ```
 
 After creating the package, we can now install the package with `pip install dist/raspidevkit-{version}.tar.gz`
 
+### Using build (project.toml)
+```bash
+pip install piptools build
+pip-compile --extra dev pyproject.toml
+python -m build
+```
+
+After creating the package, we can now install the package with `pip install dist/raspidevkit-{version}.tar.gz`
+
 ## Running Test
 First ensure that `pytest` is installed on your machine by running
 
 ```bash
 pip install pytest
 ```
 
@@ -99,14 +109,43 @@
 
 After installing the documentation dependencies navigate to the `docs` folder. Inside the docs folder, run:
 
 ```bash
 sphinx-build -M html source/ build/
 ```
 
+## Uploading to PyPi
+Install dependencies
+
+```bash
+pip install twine
+```
+
+Then build the projevt either by using setuptools or by build. After generating the wheel and source file, test it with twine
+
+```bash
+twine check dist/*
+```
+
+To upload to testpypi use:
+
+```bash
+twine upload-r testpypi dist/*
+```
+
+To upload to PyPi use:
+
+```bash
+twine upload dist/*
+```
+
+Enter your API key which should be in the .env file. 
+
+Install it with `pip install raspidevkit`
+
 ## Usage
 
 For all devices coverage, you can read the documentation [here](https://raspidevkit.readthedocs.io/en/latest/)
 
 ### Blinking an LED
 ```python
 import raspidevkit
@@ -244,11 +283,11 @@
 - [pyserial](https://pypi.org/project/pyserial/): Fundamental package for the serial interface of the library.
 - [arduino-cli](https://arduino.github.io/arduino-cli/latest/): For the great solutions for automating development with Arduino Boards.
 - and others...
 
 These libraries have been instrumental in achieving various functionalities within our project. We express our gratitude to the developers for their hard work and dedication in creating and maintaining these essential tools.
 
 ## TODO
-- [ ] Launch to PyPi
-- [ ] Create documentation
+- [x] Launch to PyPi
+- [x] Create documentation
 - [ ] Add support for SPI devices
 - [ ] Add more supported devices
```

### Comparing `raspidevkit-0.0.1/README.md` & `raspidevkit-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Raspidevkit
 Easily control devices with Raspberry Pi
 
 ## Building
+### Using setuptools
 First, ensure that the `setuptools` and `wheel` packages as installed with
 
 ```bash
 pip install setuptools 
 pip install wheel
 ```
 
@@ -13,14 +14,23 @@
 
 ```bash
 python setup.py sdist bdist_wheel
 ```
 
 After creating the package, we can now install the package with `pip install dist/raspidevkit-{version}.tar.gz`
 
+### Using build (project.toml)
+```bash
+pip install piptools build
+pip-compile --extra dev pyproject.toml
+python -m build
+```
+
+After creating the package, we can now install the package with `pip install dist/raspidevkit-{version}.tar.gz`
+
 ## Running Test
 First ensure that `pytest` is installed on your machine by running
 
 ```bash
 pip install pytest
 ```
 
@@ -53,14 +63,43 @@
 
 After installing the documentation dependencies navigate to the `docs` folder. Inside the docs folder, run:
 
 ```bash
 sphinx-build -M html source/ build/
 ```
 
+## Uploading to PyPi
+Install dependencies
+
+```bash
+pip install twine
+```
+
+Then build the projevt either by using setuptools or by build. After generating the wheel and source file, test it with twine
+
+```bash
+twine check dist/*
+```
+
+To upload to testpypi use:
+
+```bash
+twine upload-r testpypi dist/*
+```
+
+To upload to PyPi use:
+
+```bash
+twine upload dist/*
+```
+
+Enter your API key which should be in the .env file. 
+
+Install it with `pip install raspidevkit`
+
 ## Usage
 
 For all devices coverage, you can read the documentation [here](https://raspidevkit.readthedocs.io/en/latest/)
 
 ### Blinking an LED
 ```python
 import raspidevkit
@@ -198,11 +237,11 @@
 - [pyserial](https://pypi.org/project/pyserial/): Fundamental package for the serial interface of the library.
 - [arduino-cli](https://arduino.github.io/arduino-cli/latest/): For the great solutions for automating development with Arduino Boards.
 - and others...
 
 These libraries have been instrumental in achieving various functionalities within our project. We express our gratitude to the developers for their hard work and dedication in creating and maintaining these essential tools.
 
 ## TODO
-- [ ] Launch to PyPi
-- [ ] Create documentation
+- [x] Launch to PyPi
+- [x] Create documentation
 - [ ] Add support for SPI devices
 - [ ] Add more supported devices
```

### Comparing `raspidevkit-0.0.1/pyproject.toml` & `raspidevkit-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raspidevkit"
-version = "0.0.1"
+version = "0.0.2"
 description = "Easily control devices with Raspberry Pi"
 readme = "README.md"
 authors = [{ name = "DailyLollipops", email = "clarencemadrigal84@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `raspidevkit-0.0.1/raspidevkit.egg-info/PKG-INFO` & `raspidevkit-0.0.2/raspidevkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspidevkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Easily control devices with Raspberry Pi
 Home-page: https://github.com/raspidevkit/raspidevkit
 Author: DailyLollipops
 Author-email: DailyLollipops <clarencemadrigal84@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Raspidevkit
@@ -44,14 +44,15 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # Raspidevkit
 Easily control devices with Raspberry Pi
 
 ## Building
+### Using setuptools
 First, ensure that the `setuptools` and `wheel` packages as installed with
 
 ```bash
 pip install setuptools 
 pip install wheel
 ```
 
@@ -59,14 +60,23 @@
 
 ```bash
 python setup.py sdist bdist_wheel
 ```
 
 After creating the package, we can now install the package with `pip install dist/raspidevkit-{version}.tar.gz`
 
+### Using build (project.toml)
+```bash
+pip install piptools build
+pip-compile --extra dev pyproject.toml
+python -m build
+```
+
+After creating the package, we can now install the package with `pip install dist/raspidevkit-{version}.tar.gz`
+
 ## Running Test
 First ensure that `pytest` is installed on your machine by running
 
 ```bash
 pip install pytest
 ```
 
@@ -99,14 +109,43 @@
 
 After installing the documentation dependencies navigate to the `docs` folder. Inside the docs folder, run:
 
 ```bash
 sphinx-build -M html source/ build/
 ```
 
+## Uploading to PyPi
+Install dependencies
+
+```bash
+pip install twine
+```
+
+Then build the projevt either by using setuptools or by build. After generating the wheel and source file, test it with twine
+
+```bash
+twine check dist/*
+```
+
+To upload to testpypi use:
+
+```bash
+twine upload-r testpypi dist/*
+```
+
+To upload to PyPi use:
+
+```bash
+twine upload dist/*
+```
+
+Enter your API key which should be in the .env file. 
+
+Install it with `pip install raspidevkit`
+
 ## Usage
 
 For all devices coverage, you can read the documentation [here](https://raspidevkit.readthedocs.io/en/latest/)
 
 ### Blinking an LED
 ```python
 import raspidevkit
@@ -244,11 +283,11 @@
 - [pyserial](https://pypi.org/project/pyserial/): Fundamental package for the serial interface of the library.
 - [arduino-cli](https://arduino.github.io/arduino-cli/latest/): For the great solutions for automating development with Arduino Boards.
 - and others...
 
 These libraries have been instrumental in achieving various functionalities within our project. We express our gratitude to the developers for their hard work and dedication in creating and maintaining these essential tools.
 
 ## TODO
-- [ ] Launch to PyPi
-- [ ] Create documentation
+- [x] Launch to PyPi
+- [x] Create documentation
 - [ ] Add support for SPI devices
 - [ ] Add more supported devices
```

### Comparing `raspidevkit-0.0.1/tests/test_drivers.py` & `raspidevkit-0.0.2/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `raspidevkit-0.0.1/tests/test_gpio_devices.py` & `raspidevkit-0.0.2/tests/test_gpio_devices.py`

 * *Files identical despite different names*

