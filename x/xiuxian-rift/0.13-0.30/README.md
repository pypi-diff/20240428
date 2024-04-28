# Comparing `tmp/xiuxian_rift-0.13.tar.gz` & `tmp/xiuxian_rift-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_rift-0.13.tar", last modified: Thu Apr 25 01:44:18 2024, max compression
+gzip compressed data, was "xiuxian_rift-0.30.tar", last modified: Sun Apr 28 20:23:52 2024, max compression
```

## Comparing `xiuxian_rift-0.13.tar` & `xiuxian_rift-0.30.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:44:18.015687 xiuxian_rift-0.13/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:44:18.014686 xiuxian_rift-0.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:44:18.015687 xiuxian_rift-0.13/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 01:44:10.000000 xiuxian_rift-0.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:44:18.009686 xiuxian_rift-0.13/xiuxian_rift/
--rw-rw-rw-   0        0        0    17832 2024-04-25 01:13:31.000000 xiuxian_rift-0.13/xiuxian_rift/__init__.py
--rw-rw-rw-   0        0        0     1010 2024-04-22 01:25:08.000000 xiuxian_rift-0.13/xiuxian_rift/jsondata.py
--rw-rw-rw-   0        0        0     2553 2024-04-22 01:25:08.000000 xiuxian_rift-0.13/xiuxian_rift/old_rift_info.py
--rw-rw-rw-   0        0        0     2079 2024-04-25 01:44:00.000000 xiuxian_rift-0.13/xiuxian_rift/riftconfig.py
--rw-rw-rw-   0        0        0    15096 2024-04-25 01:13:31.000000 xiuxian_rift-0.13/xiuxian_rift/riftmake.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:44:18.014686 xiuxian_rift-0.13/xiuxian_rift.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:44:17.000000 xiuxian_rift-0.13/xiuxian_rift.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-25 01:44:17.000000 xiuxian_rift-0.13/xiuxian_rift.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:44:17.000000 xiuxian_rift-0.13/xiuxian_rift.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:44:17.000000 xiuxian_rift-0.13/xiuxian_rift.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:23:52.395651 xiuxian_rift-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:23:52.395651 xiuxian_rift-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:23:52.395651 xiuxian_rift-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:04:03.000000 xiuxian_rift-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:23:52.387634 xiuxian_rift-0.30/xiuxian_rift/
+-rw-rw-rw-   0        0        0    17907 2024-04-28 19:42:36.000000 xiuxian_rift-0.30/xiuxian_rift/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-04-22 01:25:08.000000 xiuxian_rift-0.30/xiuxian_rift/jsondata.py
+-rw-rw-rw-   0        0        0     2553 2024-04-22 01:25:08.000000 xiuxian_rift-0.30/xiuxian_rift/old_rift_info.py
+-rw-rw-rw-   0        0        0     2079 2024-04-25 01:44:00.000000 xiuxian_rift-0.30/xiuxian_rift/riftconfig.py
+-rw-rw-rw-   0        0        0    15246 2024-04-28 19:43:00.000000 xiuxian_rift-0.30/xiuxian_rift/riftmake.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:23:52.394651 xiuxian_rift-0.30/xiuxian_rift.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:23:52.000000 xiuxian_rift-0.30/xiuxian_rift.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-28 20:23:52.000000 xiuxian_rift-0.30/xiuxian_rift.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:23:52.000000 xiuxian_rift-0.30/xiuxian_rift.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:23:52.000000 xiuxian_rift-0.30/xiuxian_rift.egg-info/top_level.txt
```

### Comparing `xiuxian_rift-0.13/xiuxian_rift/__init__.py` & `xiuxian_rift-0.30/xiuxian_rift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     GROUP_ADMIN,
     GROUP_OWNER,
     MessageSegment
 )
 from .old_rift_info import old_rift_info
 from nonebot.permission import SUPERUSER
 from nonebot.log import logger
-from xiuxian.xiuxian2_handle import XiuxianDateManage
-from xiuxian.utils import data_check_conf, check_user, send_forward_msg, check_user_type, send_forward_msg_list, get_msg_pic, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.utils import data_check_conf, check_user, send_forward_msg, check_user_type, send_forward_msg_list, get_msg_pic, pic_msg_format
 from .riftconfig import get_config, savef
 from .jsondata import save_rift_data, read_rift_data
 from .riftmake import Rift, get_rift_type, get_story_type, NONEMSG, get_battle_type, get_dxsj_info, get_boss_battle_info, get_treasure_info
 import random
 from datetime import datetime
-from xiuxian.xiuxian_config import XiuConfig
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import XiuConfig
 from nonebot import get_driver
 
 driver = get_driver()
 config = get_config()
 sql_message = XiuxianDateManage()  # sql类
 
 # 定时任务
```

### Comparing `xiuxian_rift-0.13/xiuxian_rift/jsondata.py` & `xiuxian_rift-0.30/xiuxian_rift/jsondata.py`

 * *Files identical despite different names*

### Comparing `xiuxian_rift-0.13/xiuxian_rift/old_rift_info.py` & `xiuxian_rift-0.30/xiuxian_rift/old_rift_info.py`

 * *Files identical despite different names*

### Comparing `xiuxian_rift-0.13/xiuxian_rift/riftconfig.py` & `xiuxian_rift-0.30/xiuxian_rift/riftconfig.py`

 * *Files identical despite different names*

### Comparing `xiuxian_rift-0.13/xiuxian_rift/riftmake.py` & `xiuxian_rift-0.30/xiuxian_rift/riftmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import random
 from .riftconfig import get_config
-from xiuxian.xiuxian2_handle import OtherSet
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import OtherSet
 from .jsondata import read_f
-from xiuxian.read_buff import UserBuffDate, get_main_info_msg, get_sec_msg
-from xiuxian.xiuxian2_handle import XiuxianDateManage
-from xiuxian.player_fight import Boss_fight
-from xiuxian.item_json import Items
-from xiuxian.xiuxian_config import USERRANK
+from nonebot_plugin_simulator_xiuxian.read_buff import UserBuffDate, get_main_info_msg, get_sec_msg
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.player_fight import Boss_fight
+from nonebot_plugin_simulator_xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import USERRANK
 
 sql_message = XiuxianDateManage()
 items = Items()
 skill_data = read_f()
 
 NONEMSG = [
     "道友在秘境中晕头转向，等到清醒时竟然发现已被秘境踢出，毫无所获！",
```

