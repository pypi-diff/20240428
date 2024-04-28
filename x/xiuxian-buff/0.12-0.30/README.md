# Comparing `tmp/xiuxian_buff-0.12.tar.gz` & `tmp/xiuxian_buff-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_buff-0.12.tar", last modified: Thu Apr 25 01:40:20 2024, max compression
+gzip compressed data, was "xiuxian_buff-0.30.tar", last modified: Sun Apr 28 20:08:40 2024, max compression
```

## Comparing `xiuxian_buff-0.12.tar` & `xiuxian_buff-0.30.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:40:20.639273 xiuxian_buff-0.12/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:40:20.639273 xiuxian_buff-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:40:20.639273 xiuxian_buff-0.12/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 00:05:33.000000 xiuxian_buff-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:40:20.631350 xiuxian_buff-0.12/xiuxian_buff/
--rw-rw-rw-   0        0        0    33297 2024-04-25 01:12:06.000000 xiuxian_buff-0.12/xiuxian_buff/__init__.py
--rw-rw-rw-   0        0        0     1933 2024-04-22 01:25:08.000000 xiuxian_buff-0.12/xiuxian_buff/two_exp_cd.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:40:20.638265 xiuxian_buff-0.12/xiuxian_buff.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:40:20.000000 xiuxian_buff-0.12/xiuxian_buff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-25 01:40:20.000000 xiuxian_buff-0.12/xiuxian_buff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:40:20.000000 xiuxian_buff-0.12/xiuxian_buff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:40:20.000000 xiuxian_buff-0.12/xiuxian_buff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:08:40.827555 xiuxian_buff-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:08:40.826554 xiuxian_buff-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:08:40.827555 xiuxian_buff-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:03:33.000000 xiuxian_buff-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:08:40.819563 xiuxian_buff-0.30/xiuxian_buff/
+-rw-rw-rw-   0        0        0    33522 2024-04-28 19:41:03.000000 xiuxian_buff-0.30/xiuxian_buff/__init__.py
+-rw-rw-rw-   0        0        0     1933 2024-04-22 01:25:08.000000 xiuxian_buff-0.30/xiuxian_buff/two_exp_cd.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:08:40.826554 xiuxian_buff-0.30/xiuxian_buff.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:08:40.000000 xiuxian_buff-0.30/xiuxian_buff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-28 20:08:40.000000 xiuxian_buff-0.30/xiuxian_buff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:08:40.000000 xiuxian_buff-0.30/xiuxian_buff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:08:40.000000 xiuxian_buff-0.30/xiuxian_buff.egg-info/top_level.txt
```

### Comparing `xiuxian_buff-0.12/xiuxian_buff/__init__.py` & `xiuxian_buff-0.30/xiuxian_buff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     MessageEvent,
     GroupMessageEvent,
     MessageSegment
 )
 from nonebot.log import logger
 from datetime import datetime
 from nonebot import get_bot, on_command, on_regex, require
-from xiuxian.xiuxian2_handle import XiuxianDateManage, XiuxianJsonDate, OtherSet
-from xiuxian.xiuxian_config import XiuConfig, JsonConfig
-from xiuxian.utils import check_user
-from xiuxian.data_source import jsondata
-from xiuxian.read_buff import UserBuffDate, get_main_info_msg, get_user_buff, get_sec_msg
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage, XiuxianJsonDate, OtherSet
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import XiuConfig, JsonConfig
+from nonebot_plugin_simulator_xiuxian.utils import check_user
+from nonebot_plugin_simulator_xiuxian.data_source import jsondata
+from nonebot_plugin_simulator_xiuxian.read_buff import UserBuffDate, get_main_info_msg, get_user_buff, get_sec_msg
 from nonebot.permission import SUPERUSER
 from nonebot.params import CommandArg, RegexGroup
-from xiuxian.player_fight import Player_fight
+from nonebot_plugin_simulator_xiuxian.player_fight import Player_fight
 from .two_exp_cd import two_exp_cd
-from xiuxian.utils import send_forward_msg_list, data_check_conf, check_user_type, get_msg_pic, pic_msg_format
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
-from xiuxian.read_buff import get_player_info, save_player_info
+from nonebot_plugin_simulator_xiuxian.utils import send_forward_msg_list, data_check_conf, check_user_type, get_msg_pic, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.read_buff import get_player_info, save_player_info
 import random
 
 two_exp_cd_up = require("nonebot_plugin_apscheduler").scheduler
 
 buffinfo = on_command("我的功法", priority=5)
 out_closing = on_command("出关", aliases={"灵石出关"}, priority=5)
 mind_state = on_command("我的状态", priority=5)
```

### Comparing `xiuxian_buff-0.12/xiuxian_buff/two_exp_cd.py` & `xiuxian_buff-0.30/xiuxian_buff/two_exp_cd.py`

 * *Files identical despite different names*

