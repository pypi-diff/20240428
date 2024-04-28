# Comparing `tmp/PFlowC-1.0.0.tar.gz` & `tmp/PFlowC-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.0.0.tar", last modified: Sun Apr 28 08:07:17 2024, max compression
+gzip compressed data, was "PFlowC-1.1.0.tar", last modified: Sun Apr 28 08:13:11 2024, max compression
```

## Comparing `PFlowC-1.0.0.tar` & `PFlowC-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:07:17.549586 PFlowC-1.0.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:07:17.548497 PFlowC-1.0.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1078 2024-04-28 08:07:17.000000 PFlowC-1.0.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-28 08:07:17.000000 PFlowC-1.0.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 08:07:17.000000 PFlowC-1.0.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       69 2024-04-28 08:07:17.000000 PFlowC-1.0.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        4 2024-04-28 08:07:17.000000 PFlowC-1.0.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1078 2024-04-28 08:07:17.549306 PFlowC-1.0.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      173 2024-04-28 08:03:27.000000 PFlowC-1.0.0/README.rst
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:07:17.548920 PFlowC-1.0.0/pfc/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1463 2024-04-28 07:39:01.000000 PFlowC-1.0.0/pfc/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      718 2024-04-26 04:54:59.000000 PFlowC-1.0.0/pfc/proxy.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:07:17.549650 PFlowC-1.0.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2284 2024-04-28 08:06:51.000000 PFlowC-1.0.0/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:13:11.335396 PFlowC-1.1.0/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:13:11.330375 PFlowC-1.1.0/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1088 2024-04-28 08:13:11.000000 PFlowC-1.1.0/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-28 08:13:11.000000 PFlowC-1.1.0/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 08:13:11.000000 PFlowC-1.1.0/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       69 2024-04-28 08:13:11.000000 PFlowC-1.1.0/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        4 2024-04-28 08:13:11.000000 PFlowC-1.1.0/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1088 2024-04-28 08:13:11.335130 PFlowC-1.1.0/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      173 2024-04-28 08:08:24.000000 PFlowC-1.1.0/README.rst
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:13:11.332883 PFlowC-1.1.0/pfc/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1471 2024-04-28 08:11:40.000000 PFlowC-1.1.0/pfc/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      725 2024-04-28 08:11:00.000000 PFlowC-1.1.0/pfc/proxy.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:13:11.336003 PFlowC-1.1.0/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2294 2024-04-28 08:13:03.000000 PFlowC-1.1.0/setup.py
```

### Comparing `PFlowC-1.0.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-1.1.0/PFlowC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.0.0
+Version: 1.1.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
-Author-email: ouzheng1993@gmail.com
+Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Education
```

### Comparing `PFlowC-1.0.0/PKG-INFO` & `PFlowC-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.0.0
+Version: 1.1.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
-Author-email: ouzheng1993@gmail.com
+Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Education
```

### Comparing `PFlowC-1.0.0/pfc/main.py` & `PFlowC-1.1.0/pfc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 ======================================="""
 import json
 import logging
 import os
 
 import click
 
-from utils import logger
-from utils.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
+from pfc.utils import logger
+from pfc.utils.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
 
 
 @click.command(help="Command line interface for FlowPilot")
 def main():
     config_fp = os.path.expanduser("~/.flowPilot/config.json")
     if not os.path.isfile(config_fp):
         click.echo("upstream config file: {} does not exist.".format(config_fp))
```

### Comparing `PFlowC-1.0.0/pfc/proxy.py` & `PFlowC-1.1.0/pfc/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import click
 
-from utils.proxy_helper import set_web_proxy
-
-VERSION = "0.1.0"
+from pfc.utils.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
 
 
 @click.command
 @click.option("--host", "-h", default="127.0.0.1", help="The host address of the proxy")
 @click.option("--port", "-p", default=8080, help="The port of the proxy")
 @click.option("--socks_port", "-s", default=8090, help="The port of the socks server")
 @click.option("--bypass-domains", type=list, default=['127.0.0.1', "192.168.0.0/16"],
```

### Comparing `PFlowC-1.0.0/setup.py` & `PFlowC-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,18 +34,18 @@
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.0.0',
+    version='1.1.0',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
-    author_email='ouzheng1993@gmail.com',
+    author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["pfc"],
     install_requires=install_reqs,
     include_package_data=True,
     python_requires='>=3.7',
     long_description=long_description,
```

