# Comparing `tmp/xiuxian_sect-0.12.tar.gz` & `tmp/xiuxian_sect-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_sect-0.12.tar", last modified: Thu Apr 25 01:41:31 2024, max compression
+gzip compressed data, was "xiuxian_sect-0.30.tar", last modified: Sun Apr 28 20:24:15 2024, max compression
```

## Comparing `xiuxian_sect-0.12.tar` & `xiuxian_sect-0.30.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:41:31.283669 xiuxian_sect-0.12/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:41:31.282665 xiuxian_sect-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:41:31.283669 xiuxian_sect-0.12/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 00:11:34.000000 xiuxian_sect-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:41:31.275505 xiuxian_sect-0.12/xiuxian_sect/
--rw-rw-rw-   0        0        0    84573 2024-04-25 01:13:48.000000 xiuxian_sect-0.12/xiuxian_sect/__init__.py
--rw-rw-rw-   0        0        0     6120 2024-04-22 01:25:08.000000 xiuxian_sect-0.12/xiuxian_sect/sectconfig.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:41:31.281662 xiuxian_sect-0.12/xiuxian_sect.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:41:31.000000 xiuxian_sect-0.12/xiuxian_sect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-25 01:41:31.000000 xiuxian_sect-0.12/xiuxian_sect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:41:31.000000 xiuxian_sect-0.12/xiuxian_sect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:41:31.000000 xiuxian_sect-0.12/xiuxian_sect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:24:15.393769 xiuxian_sect-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:24:15.393769 xiuxian_sect-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:24:15.393769 xiuxian_sect-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:03:33.000000 xiuxian_sect-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:24:15.385769 xiuxian_sect-0.30/xiuxian_sect/
+-rw-rw-rw-   0        0        0    84773 2024-04-28 19:43:30.000000 xiuxian_sect-0.30/xiuxian_sect/__init__.py
+-rw-rw-rw-   0        0        0     6120 2024-04-22 01:25:08.000000 xiuxian_sect-0.30/xiuxian_sect/sectconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:24:15.392770 xiuxian_sect-0.30/xiuxian_sect.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:24:15.000000 xiuxian_sect-0.30/xiuxian_sect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-28 20:24:15.000000 xiuxian_sect-0.30/xiuxian_sect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:24:15.000000 xiuxian_sect-0.30/xiuxian_sect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:24:15.000000 xiuxian_sect-0.30/xiuxian_sect.egg-info/top_level.txt
```

### Comparing `xiuxian_sect-0.12/xiuxian_sect/__init__.py` & `xiuxian_sect-0.30/xiuxian_sect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
 from nonebot import get_bot, on_command, on_regex, require
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import (
     PRIVATE_FRIEND,
     Bot,
     GROUP,
     Message,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment,
 )
 from nonebot.params import CommandArg, RegexGroup
-from xiuxian.data_source import jsondata
-from xiuxian.xiuxian_config import XiuConfig, USERRANK
-from xiuxian.utils import Txt2Img
+from nonebot_plugin_simulator_xiuxian.data_source import jsondata
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import XiuConfig, USERRANK
+from nonebot_plugin_simulator_xiuxian.utils import Txt2Img
 import re
 from .sectconfig import get_config
 import random
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
-from xiuxian.utils import check_user,send_forward_msg, data_check_conf, get_msg_pic, pic_msg_format
-from xiuxian.read_buff import BuffJsonDate, get_main_info_msg, UserBuffDate, get_sec_msg
-from xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.utils import check_user,send_forward_msg, data_check_conf, get_msg_pic, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.read_buff import BuffJsonDate, get_main_info_msg, UserBuffDate, get_sec_msg
+from nonebot_plugin_simulator_xiuxian.item_json import Items
 
 items = Items()
 config = get_config()
 LEVLECOST = config["LEVLECOST"]
 
 # 定时任务
 materialsupdate = require("nonebot_plugin_apscheduler").scheduler
```

### Comparing `xiuxian_sect-0.12/xiuxian_sect/sectconfig.py` & `xiuxian_sect-0.30/xiuxian_sect/sectconfig.py`

 * *Files identical despite different names*

