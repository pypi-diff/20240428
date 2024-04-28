# Comparing `tmp/xiuxian_back-0.13.tar.gz` & `tmp/xiuxian_back-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_back-0.13.tar", last modified: Thu Apr 25 01:54:29 2024, max compression
+gzip compressed data, was "xiuxian_back-0.30.tar", last modified: Sun Apr 28 20:04:38 2024, max compression
```

## Comparing `xiuxian_back-0.13.tar` & `xiuxian_back-0.30.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:54:29.360414 xiuxian_back-0.13/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:54:29.359414 xiuxian_back-0.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:54:29.360414 xiuxian_back-0.13/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 01:54:23.000000 xiuxian_back-0.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:54:29.354414 xiuxian_back-0.13/xiuxian_back/
--rw-rw-rw-   0        0        0    57815 2024-04-25 01:54:06.000000 xiuxian_back-0.13/xiuxian_back/__init__.py
--rw-rw-rw-   0        0        0    20312 2024-04-25 01:10:19.000000 xiuxian_back-0.13/xiuxian_back/back_util.py
--rw-rw-rw-   0        0        0     3053 2024-04-22 01:25:08.000000 xiuxian_back-0.13/xiuxian_back/backconfig.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:54:29.359414 xiuxian_back-0.13/xiuxian_back.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:54:29.000000 xiuxian_back-0.13/xiuxian_back.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-25 01:54:29.000000 xiuxian_back-0.13/xiuxian_back.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:54:29.000000 xiuxian_back-0.13/xiuxian_back.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:54:29.000000 xiuxian_back-0.13/xiuxian_back.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:04:38.102626 xiuxian_back-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:04:38.102626 xiuxian_back-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:04:38.103624 xiuxian_back-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:02:29.000000 xiuxian_back-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:04:38.094664 xiuxian_back-0.30/xiuxian_back/
+-rw-rw-rw-   0        0        0    57965 2024-04-28 19:38:37.000000 xiuxian_back-0.30/xiuxian_back/__init__.py
+-rw-rw-rw-   0        0        0    20437 2024-04-28 19:39:08.000000 xiuxian_back-0.30/xiuxian_back/back_util.py
+-rw-rw-rw-   0        0        0     3053 2024-04-22 01:25:08.000000 xiuxian_back-0.30/xiuxian_back/backconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:04:38.101616 xiuxian_back-0.30/xiuxian_back.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:04:38.000000 xiuxian_back-0.30/xiuxian_back.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-28 20:04:38.000000 xiuxian_back-0.30/xiuxian_back.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:04:38.000000 xiuxian_back-0.30/xiuxian_back.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:04:38.000000 xiuxian_back-0.30/xiuxian_back.egg-info/top_level.txt
```

### Comparing `xiuxian_back-0.13/xiuxian_back/__init__.py` & `xiuxian_back-0.30/xiuxian_back/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     GROUP_ADMIN,
     GROUP_OWNER,
     ActionFailed
 )
 from nonebot.permission import SUPERUSER
 from nonebot.log import logger
 from nonebot.params import CommandArg, RegexGroup
-from xiuxian.utils import data_check_conf, check_user, send_forward_msg, pic_msg_format, get_msg_pic
-from xiuxian.xiuxian2_handle import XiuxianDateManage, OtherSet
-from xiuxian.item_json import Items
-from xiuxian.data_source import jsondata
+from nonebot_plugin_simulator_xiuxian.utils import data_check_conf, check_user, send_forward_msg, pic_msg_format, get_msg_pic
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage, OtherSet
+from nonebot_plugin_simulator_xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.data_source import jsondata
 from .back_util import get_user_back_msg, check_equipment_can_use, get_use_equipment_sql, get_shop_data, save_shop, get_item_msg, check_use_elixir, get_use_jlq_msg, get_item_msg_rank
 from .backconfig import get_config, savef
 import random
 from datetime import datetime
-from xiuxian.read_buff import get_weapon_info_msg, get_armor_info_msg, get_sec_msg, get_main_info_msg, UserBuffDate
-from xiuxian.xiuxian_config import XiuConfig
+from nonebot_plugin_simulator_xiuxian.read_buff import get_weapon_info_msg, get_armor_info_msg, get_sec_msg, get_main_info_msg, UserBuffDate
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import XiuConfig
 
 items = Items()
 config = get_config()
 groups = config['open'] #list，群交流会使用
 auction = {}
 AUCTIONSLEEPTIME = 1200#交友初始等待时间（秒）
```

### Comparing `xiuxian_back-0.13/xiuxian_back/back_util.py` & `xiuxian_back-0.30/xiuxian_back/back_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from xiuxian.item_json import Items
-from xiuxian.xiuxian2_handle import XiuxianDateManage
-from xiuxian.read_buff import UserBuffDate, get_weapon_info_msg, get_armor_info_msg, get_sec_msg, get_main_info_msg
+from nonebot_plugin_simulator_xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.read_buff import UserBuffDate, get_weapon_info_msg, get_armor_info_msg, get_sec_msg, get_main_info_msg
 from datetime import datetime
 import json
 import os
 from pathlib import Path
-from xiuxian.xiuxian_config import USERRANK
-from xiuxian.read_buff import get_player_info, save_player_info
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import USERRANK
+from nonebot_plugin_simulator_xiuxian.read_buff import get_player_info, save_player_info
 
 items = Items()
 sql_message = XiuxianDateManage()
 
 def check_equipment_can_use(user_id, goods_id):
     """
     装备数据库字段：
```

### Comparing `xiuxian_back-0.13/xiuxian_back/backconfig.py` & `xiuxian_back-0.30/xiuxian_back/backconfig.py`

 * *Files identical despite different names*

