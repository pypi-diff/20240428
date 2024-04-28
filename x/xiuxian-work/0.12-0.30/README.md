# Comparing `tmp/xiuxian_work-0.12.tar.gz` & `tmp/xiuxian_work-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_work-0.12.tar", last modified: Thu Apr 25 01:41:53 2024, max compression
+gzip compressed data, was "xiuxian_work-0.30.tar", last modified: Sun Apr 28 20:24:40 2024, max compression
```

## Comparing `xiuxian_work-0.12.tar` & `xiuxian_work-0.30.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:41:53.610939 xiuxian_work-0.12/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:41:53.609932 xiuxian_work-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:41:53.610939 xiuxian_work-0.12/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 00:12:06.000000 xiuxian_work-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:41:53.602398 xiuxian_work-0.12/xiuxian_work/
--rw-rw-rw-   0        0        0    20766 2024-04-25 01:25:35.000000 xiuxian_work-0.12/xiuxian_work/__init__.py
--rw-rw-rw-   0        0        0     2144 2024-04-25 01:14:10.000000 xiuxian_work-0.12/xiuxian_work/reward_data_source.py
--rw-rw-rw-   0        0        0     2241 2024-04-25 01:14:09.000000 xiuxian_work-0.12/xiuxian_work/work_handle.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 01:25:09.000000 xiuxian_work-0.12/xiuxian_work/workmake.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:41:53.609932 xiuxian_work-0.12/xiuxian_work.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:41:53.000000 xiuxian_work-0.12/xiuxian_work.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-25 01:41:53.000000 xiuxian_work-0.12/xiuxian_work.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:41:53.000000 xiuxian_work-0.12/xiuxian_work.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:41:53.000000 xiuxian_work-0.12/xiuxian_work.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:24:40.513049 xiuxian_work-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:24:40.513049 xiuxian_work-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:24:40.513049 xiuxian_work-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:03:33.000000 xiuxian_work-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:24:40.504097 xiuxian_work-0.30/xiuxian_work/
+-rw-rw-rw-   0        0        0    20941 2024-04-28 19:43:57.000000 xiuxian_work-0.30/xiuxian_work/__init__.py
+-rw-rw-rw-   0        0        0     2169 2024-04-28 19:44:05.000000 xiuxian_work-0.30/xiuxian_work/reward_data_source.py
+-rw-rw-rw-   0        0        0     2291 2024-04-28 19:44:12.000000 xiuxian_work-0.30/xiuxian_work/work_handle.py
+-rw-rw-rw-   0        0        0     2694 2024-04-28 19:44:21.000000 xiuxian_work-0.30/xiuxian_work/workmake.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:24:40.512049 xiuxian_work-0.30/xiuxian_work.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:24:40.000000 xiuxian_work-0.30/xiuxian_work.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-28 20:24:40.000000 xiuxian_work-0.30/xiuxian_work.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:24:40.000000 xiuxian_work-0.30/xiuxian_work.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:24:40.000000 xiuxian_work-0.30/xiuxian_work.egg-info/top_level.txt
```

### Comparing `xiuxian_work-0.12/xiuxian_work/__init__.py` & `xiuxian_work-0.30/xiuxian_work/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     MessageEvent,
     PRIVATE_FRIEND,
     GROUP,
     GroupMessageEvent,
     MessageSegment,
     Message
 )
-from xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
 from .work_handle import workhandle
 from datetime import datetime
-from xiuxian.xiuxian_opertion import do_is_work
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
-from xiuxian.utils import data_check_conf, check_user, send_forward_msg, check_user_type, send_forward_msg_list, get_msg_pic, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.xiuxian_opertion import do_is_work
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.utils import data_check_conf, check_user, send_forward_msg, check_user_type, send_forward_msg_list, get_msg_pic, pic_msg_format
 from nonebot.log import logger
 from .reward_data_source import PLAYERSDATA
 import os
-from xiuxian.item_json import Items
-from xiuxian.xiuxian_config import USERRANK, XiuConfig
-from xiuxian.exp_util import get_exp_rate, user_get_exp_max
+from nonebot_plugin_simulator_xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import USERRANK, XiuConfig
+from nonebot_plugin_simulator_xiuxian.exp_util import get_exp_rate, user_get_exp_max
 # 定时任务
 resetrefreshnum = require("nonebot_plugin_apscheduler").scheduler
 
 
 work = {}  # 悬赏令信息记录
 refreshnum : Dict[str, int] = {} #用户悬赏令刷新次数记录
 sql_message = XiuxianDateManage()  # sql类
```

### Comparing `xiuxian_work-0.12/xiuxian_work/reward_data_source.py` & `xiuxian_work-0.30/xiuxian_work/reward_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xiuxian.data_source import *
+from nonebot_plugin_simulator_xiuxian.data_source import *
 import os
 
 
 
 WORKDATA = Path() / "data" / "xiuxian" / "work"
 
 class reward(JsonDate):
```

### Comparing `xiuxian_work-0.12/xiuxian_work/work_handle.py` & `xiuxian_work-0.30/xiuxian_work/work_handle.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
-from xiuxian.xiuxian2_handle import *
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import *
 from .reward_data_source import *
 import json
 from .workmake import *
-from xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.item_json import Items
 
 class workhandle(XiuxianJsonDate):
     
     
     def do_work(self,key,work_list=None,name=None,level="江湖好手", exp=None, user_id=None):
         """悬赏令获取"""
         if key == 0:   # 如果没有获取过，则返回悬赏令
```

### Comparing `xiuxian_work-0.12/xiuxian_work/workmake.py` & `xiuxian_work-0.30/xiuxian_work/workmake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .reward_data_source import *
 import random
-from xiuxian.item_json import Items
-from xiuxian.xiuxian_config import USERRANK
-from xiuxian.xiuxian2_handle import OtherSet
+from nonebot_plugin_simulator_xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import USERRANK
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import OtherSet
 
 def workmake(work_level, exp, user_level):
     if work_level == '江湖好手':
         work_level = '江湖好手'
     else:
         work_level = work_level[:3]#取境界前3位，补全初期、中期、圆满任务可不取
```

