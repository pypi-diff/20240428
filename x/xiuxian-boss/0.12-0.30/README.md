# Comparing `tmp/xiuxian_boss-0.12.tar.gz` & `tmp/xiuxian_boss-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_boss-0.12.tar", last modified: Thu Apr 25 01:39:59 2024, max compression
+gzip compressed data, was "xiuxian_boss-0.30.tar", last modified: Sun Apr 28 20:05:51 2024, max compression
```

## Comparing `xiuxian_boss-0.12.tar` & `xiuxian_boss-0.30.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:39:59.522884 xiuxian_boss-0.12/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:39:59.521885 xiuxian_boss-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:39:59.522884 xiuxian_boss-0.12/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 00:05:05.000000 xiuxian_boss-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:39:59.513885 xiuxian_boss-0.12/xiuxian_boss/
--rw-rw-rw-   0        0        0    33990 2024-04-25 01:11:53.000000 xiuxian_boss-0.12/xiuxian_boss/__init__.py
--rw-rw-rw-   0        0        0     4895 2024-04-22 01:25:08.000000 xiuxian_boss-0.12/xiuxian_boss/bossconfig.py
--rw-rw-rw-   0        0        0     1835 2024-04-25 01:11:53.000000 xiuxian_boss-0.12/xiuxian_boss/makeboss.py
--rw-rw-rw-   0        0        0     1269 2024-04-22 01:25:08.000000 xiuxian_boss-0.12/xiuxian_boss/old_boss_info.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:39:59.521885 xiuxian_boss-0.12/xiuxian_boss.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:39:59.000000 xiuxian_boss-0.12/xiuxian_boss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-04-25 01:39:59.000000 xiuxian_boss-0.12/xiuxian_boss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:39:59.000000 xiuxian_boss-0.12/xiuxian_boss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:39:59.000000 xiuxian_boss-0.12/xiuxian_boss.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:51.643138 xiuxian_boss-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:05:51.642138 xiuxian_boss-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:05:51.643138 xiuxian_boss-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:03:33.000000 xiuxian_boss-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:51.635171 xiuxian_boss-0.30/xiuxian_boss/
+-rw-rw-rw-   0        0        0    34165 2024-04-28 19:40:26.000000 xiuxian_boss-0.30/xiuxian_boss/__init__.py
+-rw-rw-rw-   0        0        0     4895 2024-04-22 01:25:08.000000 xiuxian_boss-0.30/xiuxian_boss/bossconfig.py
+-rw-rw-rw-   0        0        0     1860 2024-04-28 19:40:38.000000 xiuxian_boss-0.30/xiuxian_boss/makeboss.py
+-rw-rw-rw-   0        0        0     1269 2024-04-22 01:25:08.000000 xiuxian_boss-0.30/xiuxian_boss/old_boss_info.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:51.642138 xiuxian_boss-0.30/xiuxian_boss.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:05:51.000000 xiuxian_boss-0.30/xiuxian_boss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-04-28 20:05:51.000000 xiuxian_boss-0.30/xiuxian_boss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:05:51.000000 xiuxian_boss-0.30/xiuxian_boss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:05:51.000000 xiuxian_boss-0.30/xiuxian_boss.egg-info/top_level.txt
```

### Comparing `xiuxian_boss-0.12/xiuxian_boss/__init__.py` & `xiuxian_boss-0.30/xiuxian_boss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     GROUP_OWNER,
     ActionFailed,
     MessageSegment
 
 )
 from nonebot.permission import SUPERUSER
 from nonebot.log import logger
-from xiuxian.xiuxian2_handle import XiuxianDateManage
-from xiuxian.xiuxian_config import USERRANK, XiuConfig
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import USERRANK, XiuConfig
 from .makeboss import createboss,createboss_jj
 from .bossconfig import get_config, savef
 from .old_boss_info import old_boss_info
-from xiuxian.player_fight import Boss_fight
-from xiuxian.item_json import Items
-from xiuxian.utils import data_check_conf, send_forward_msg_list, check_user, send_forward_msg, get_msg_pic, pic_msg_format
-from xiuxian.read_buff import UserBuffDate
+from nonebot_plugin_simulator_xiuxian.player_fight import Boss_fight
+from nonebot_plugin_simulator_xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.utils import data_check_conf, send_forward_msg_list, check_user, send_forward_msg, get_msg_pic, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.read_buff import UserBuffDate
 from pathlib import Path
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
 import json
 import os
 from nonebot import get_driver
 
 driver = get_driver()
 
 config = get_config()
```

### Comparing `xiuxian_boss-0.12/xiuxian_boss/bossconfig.py` & `xiuxian_boss-0.30/xiuxian_boss/bossconfig.py`

 * *Files identical despite different names*

### Comparing `xiuxian_boss-0.12/xiuxian_boss/makeboss.py` & `xiuxian_boss-0.30/xiuxian_boss/makeboss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 import json
 import random
-from xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
 from .bossconfig import get_config
 
 config = get_config()
 
 def get_boss_jinjie_dict():
     CONFIGJSONPATH = Path() / "data" / "xiuxian" / "境界.json"
     with open(CONFIGJSONPATH, "r", encoding="UTF-8") as f:
```

### Comparing `xiuxian_boss-0.12/xiuxian_boss/old_boss_info.py` & `xiuxian_boss-0.30/xiuxian_boss/old_boss_info.py`

 * *Files identical despite different names*

