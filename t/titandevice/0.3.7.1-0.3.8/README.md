# Comparing `tmp/TitanDevice-0.3.7.1.tar.gz` & `tmp/titandevice-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.7.1.tar", last modified: Fri Apr 26 10:50:31 2024, max compression
+gzip compressed data, was "titandevice-0.3.8.tar", last modified: Sun Apr 28 01:53:26 2024, max compression
```

## Comparing `TitanDevice-0.3.7.1.tar` & `titandevice-0.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:50:31.254362 TitanDevice-0.3.7.1/
--rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-26 10:50:31.254362 TitanDevice-0.3.7.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.7.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:50:31.254362 TitanDevice-0.3.7.1/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-26 10:50:31.000000 TitanDevice-0.3.7.1/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-26 10:50:31.000000 TitanDevice-0.3.7.1/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 10:50:31.000000 TitanDevice-0.3.7.1/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-26 10:50:31.000000 TitanDevice-0.3.7.1/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-26 10:50:31.000000 TitanDevice-0.3.7.1/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 10:50:31.254362 TitanDevice-0.3.7.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      798 2024-04-26 10:50:26.000000 TitanDevice-0.3.7.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 10:50:31.254362 TitanDevice-0.3.7.1/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4205 2024-04-25 06:42:55.000000 TitanDevice-0.3.7.1/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1415 2024-04-26 10:24:31.000000 TitanDevice-0.3.7.1/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7099 2024-04-26 10:50:26.000000 TitanDevice-0.3.7.1/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 TitanDevice-0.3.7.1/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:53:26.565587 titandevice-0.3.8/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 01:53:26.565587 titandevice-0.3.8/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 titandevice-0.3.8/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 01:53:26.565587 titandevice-0.3.8/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-28 01:52:55.000000 titandevice-0.3.8/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:53:26.565587 titandevice-0.3.8/titandevice/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4190 2024-04-28 01:51:38.000000 titandevice-0.3.8/titandevice/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1415 2024-04-26 10:24:31.000000 titandevice-0.3.8/titandevice/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7089 2024-04-28 01:52:55.000000 titandevice-0.3.8/titandevice/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 titandevice-0.3.8/titandevice/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:53:26.565587 titandevice-0.3.8/titandevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      310 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/top_level.txt
```

### Comparing `TitanDevice-0.3.7.1/PKG-INFO` & `titandevice-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TitanDevice
-Version: 0.3.7.1
+Name: titandevice
+Version: 0.3.8
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.7.1/TitanDevice.egg-info/PKG-INFO` & `titandevice-0.3.8/titandevice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TitanDevice
-Version: 0.3.7.1
+Name: titandevice
+Version: 0.3.8
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.7.1/setup.py` & `titandevice-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # Read the content of `README.md`:
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
-    name="TitanDevice",
-    version="0.3.7.1",
+    name="titandevice",
+    version="0.3.8",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.7.1/titan/__init__.py` & `titandevice-0.3.8/titandevice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from titan._device_exception import *
-from titan._device_manager import _DeviceManager
-from titan._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
+from ._device_exception import *
+from ._device_manager import _DeviceManager
+from ._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
 
 device_manager_list: list[_DeviceManager] = _DeviceManager.get_all_device_manager_list()
 
 
 def get_all_devices() -> list[DeviceInfo]:
     global device_manager_list
     device_manager_list = _DeviceManager.get_all_device_manager_list()
```

### Comparing `TitanDevice-0.3.7.1/titan/_device_exception.py` & `titandevice-0.3.8/titandevice/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.7.1/titan/_device_manager.py` & `titandevice-0.3.8/titandevice/_device_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import subprocess
 import time
 from typing import Optional
 
 import apkutils2
 from adbutils import adb, adb_path
 
-from titan._device_exception import *
-from titan._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
+from ._device_exception import *
+from ._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
 
 
 class _DeviceManager(object):
     _device: adb.device
     _serial: str
     _is_root: bool = False
     _device_info: Optional[DeviceInfo] = None
```

### Comparing `TitanDevice-0.3.7.1/titan/_device_models.py` & `titandevice-0.3.8/titandevice/_device_models.py`

 * *Files identical despite different names*

