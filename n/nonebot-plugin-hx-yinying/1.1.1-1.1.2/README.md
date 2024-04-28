# Comparing `tmp/nonebot-plugin-hx-yinying-1.1.1.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.1.tar", last modified: Sat Apr 27 19:46:47 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.2.tar", last modified: Sat Apr 27 20:21:26 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.1.1.tar` & `nonebot-plugin-hx-yinying-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 19:46:47.305420 nonebot-plugin-hx-yinying-1.1.1/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5087 2024-04-27 19:46:47.306568 nonebot-plugin-hx-yinying-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 19:46:47.084036 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    56840 2024-04-27 19:45:25.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    95553 2024-04-27 18:12:21.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      396 2024-04-27 19:46:39.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     4060 2024-04-27 18:25:28.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/report.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:46:47.289339 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     5087 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-27 19:46:46.000000 nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-27 19:46:47.354296 nonebot-plugin-hx-yinying-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      961 2024-04-27 18:26:26.000000 nonebot-plugin-hx-yinying-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:21:26.136652 nonebot-plugin-hx-yinying-1.1.2/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5087 2024-04-27 20:21:26.136652 nonebot-plugin-hx-yinying-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 20:21:25.719780 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    56840 2024-04-27 19:45:25.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    95553 2024-04-27 18:12:21.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      618 2024-04-27 20:20:17.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     1864 2024-04-27 20:19:31.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     4106 2024-04-27 20:04:45.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/report.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:21:26.123476 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     5087 2024-04-27 20:21:24.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-27 20:21:25.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 20:21:24.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-04-27 20:21:24.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-27 20:21:24.000000 nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-27 20:21:26.170184 nonebot-plugin-hx-yinying-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2024-04-27 20:19:53.000000 nonebot-plugin-hx-yinying-1.1.2/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.1.1/LICENSE` & `nonebot-plugin-hx-yinying-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.1/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.1
+Version: 1.1.2
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.2 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.1/README.md` & `nonebot-plugin-hx-yinying-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/chat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import traceback,requests,zipfile,sys,os
 from PIL import Image,ImageFilter
 from .chat import(
     file_get,
     path_in,
     create_dir_usr,
 )
-from nonebot import get_plugin_config
+from nonebot import get_plugin_config,require
+require("nonebot_plugin_htmlrender")
 from nonebot_plugin_htmlrender import template_to_pic
 from loguru import logger
 from tqdm import tqdm
 from nonebot.message import run_postprocessor
 from nonebot.adapters.onebot.v11 import (
    Bot,  MessageEvent ,MessageSegment
 )
```

### Comparing `nonebot-plugin-hx-yinying-1.1.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.2/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.1
+Version: 1.1.2
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.2 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.1/setup.py` & `nonebot-plugin-hx-yinying-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.1.1",
+    version="1.1.2",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
-    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0','nonebot_plugin_htmlrender>=0.3.0','pillow>=9.3.0','tqdm>=4.65.0'],
+    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0','nonebot_plugin_htmlrender>=0.3.0','pillow>=9.3.0','tqdm>=4.65.0','alibabacloud_imageaudit20191230>=2.0.5'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

