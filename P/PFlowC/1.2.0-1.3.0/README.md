# Comparing `tmp/PFlowC-1.2.0.tar.gz` & `tmp/PFlowC-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.2.0.tar", last modified: Sun Apr 28 08:17:28 2024, max compression
+gzip compressed data, was "PFlowC-1.3.0.tar", last modified: Sun Apr 28 08:38:21 2024, max compression
```

## Comparing `PFlowC-1.2.0.tar` & `PFlowC-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:17:28.134248 PFlowC-1.2.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:17:28.133082 PFlowC-1.2.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1088 2024-04-28 08:17:28.000000 PFlowC-1.2.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      213 2024-04-28 08:17:28.000000 PFlowC-1.2.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 08:17:28.000000 PFlowC-1.2.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       69 2024-04-28 08:17:28.000000 PFlowC-1.2.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        4 2024-04-28 08:17:28.000000 PFlowC-1.2.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1088 2024-04-28 08:17:28.134014 PFlowC-1.2.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      173 2024-04-28 08:08:24.000000 PFlowC-1.2.0/README.rst
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:17:28.133520 PFlowC-1.2.0/pfc/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:17:13.000000 PFlowC-1.2.0/pfc/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1471 2024-04-28 08:11:40.000000 PFlowC-1.2.0/pfc/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      725 2024-04-28 08:11:00.000000 PFlowC-1.2.0/pfc/proxy.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:17:28.134291 PFlowC-1.2.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2294 2024-04-28 08:17:19.000000 PFlowC-1.2.0/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.881882 PFlowC-1.3.0/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.879972 PFlowC-1.3.0/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      325 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       71 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        6 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 08:38:21.881671 PFlowC-1.3.0/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.3.0/README.rst
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.880290 PFlowC-1.3.0/pflow/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      111 2024-04-28 08:36:00.000000 PFlowC-1.3.0/pflow/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1523 2024-04-28 08:35:55.000000 PFlowC-1.3.0/pflow/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      725 2024-04-28 08:11:00.000000 PFlowC-1.3.0/pflow/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.880773 PFlowC-1.3.0/pflow/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.3.0/pflow/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3785 2024-04-28 06:00:02.000000 PFlowC-1.3.0/pflow/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.881217 PFlowC-1.3.0/pflow/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.3.0/pflow/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1890 2022-12-03 21:50:12.000000 PFlowC-1.3.0/pflow/utils/logger.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:38:21.881924 PFlowC-1.3.0/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2335 2024-04-28 08:36:46.000000 PFlowC-1.3.0/setup.py
```

### Comparing `PFlowC-1.2.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-1.3.0/PFlowC.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.2.0
+Version: 1.3.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,10 +21,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
+ProxyFlow Control
+------------------------------
+
 A net flow pilot in order to handle some proxy configuration automatically.
```

### Comparing `PFlowC-1.2.0/PKG-INFO` & `PFlowC-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.2.0
+Version: 1.3.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,10 +21,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
+ProxyFlow Control
+------------------------------
+
 A net flow pilot in order to handle some proxy configuration automatically.
```

### Comparing `PFlowC-1.2.0/pfc/main.py` & `PFlowC-1.3.0/pflow/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 @disc:
 ======================================="""
 import json
 import logging
 import os
 
 import click
+from pflow import get_version
+
+from pflow.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
+from pflow.utils import logger
+
+print(get_version())
+
 
-from pfc.utils import logger
-from pfc.utils.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
 
 
 @click.command(help="Command line interface for FlowPilot")
 def main():
     config_fp = os.path.expanduser("~/.flowPilot/config.json")
     if not os.path.isfile(config_fp):
         click.echo("upstream config file: {} does not exist.".format(config_fp))
```

### Comparing `PFlowC-1.2.0/pfc/proxy.py` & `PFlowC-1.3.0/pflow/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.2.0/setup.py` & `PFlowC-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.2.0',
+    version='1.3.0',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
-    packages=["pfc"],
+    packages=["pflow", "pflow.utils", "pflow.proxy_helper"],
     install_requires=install_reqs,
     include_package_data=True,
     python_requires='>=3.7',
     long_description=long_description,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
@@ -63,12 +63,12 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     keywords="proxy flow control",
     entry_points={
         'console_scripts': [
-            'pfc-cli=pfc.main:main',
+            'pflow-cli=pfc.main:main',
             'proxy-cli=pfc.proxy:main',
         ],
     },
 )
```

