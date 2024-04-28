# Comparing `tmp/xiuxian_mixelixir-0.12.tar.gz` & `tmp/xiuxian_mixelixir-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_mixelixir-0.12.tar", last modified: Thu Apr 25 01:40:56 2024, max compression
+gzip compressed data, was "xiuxian_mixelixir-0.30.tar", last modified: Sun Apr 28 20:23:14 2024, max compression
```

## Comparing `xiuxian_mixelixir-0.12.tar` & `xiuxian_mixelixir-0.30.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:40:56.058388 xiuxian_mixelixir-0.12/
--rw-rw-rw-   0        0        0      256 2024-04-25 01:40:56.057236 xiuxian_mixelixir-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:40:56.058388 xiuxian_mixelixir-0.12/setup.cfg
--rw-rw-rw-   0        0        0      500 2024-04-25 00:08:27.000000 xiuxian_mixelixir-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:40:56.049229 xiuxian_mixelixir-0.12/xiuxian_mixelixir/
--rw-rw-rw-   0        0        0    27185 2024-04-25 01:13:16.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir/__init__.py
--rw-rw-rw-   0        0        0      480 2024-04-22 01:25:08.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir/mix_elixir_config.py
--rw-rw-rw-   0        0        0     6933 2024-04-25 01:13:16.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir/mixelixirutil.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:40:56.057236 xiuxian_mixelixir-0.12/xiuxian_mixelixir.egg-info/
--rw-rw-rw-   0        0        0      256 2024-04-25 01:40:56.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-25 01:40:56.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:40:56.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-25 01:40:56.000000 xiuxian_mixelixir-0.12/xiuxian_mixelixir.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:23:14.762327 xiuxian_mixelixir-0.30/
+-rw-rw-rw-   0        0        0      257 2024-04-28 20:23:14.762327 xiuxian_mixelixir-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:23:14.762327 xiuxian_mixelixir-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      501 2024-04-28 20:03:33.000000 xiuxian_mixelixir-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:23:14.754327 xiuxian_mixelixir-0.30/xiuxian_mixelixir/
+-rw-rw-rw-   0        0        0    27360 2024-04-28 19:42:08.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir/__init__.py
+-rw-rw-rw-   0        0        0      480 2024-04-22 01:25:08.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir/mix_elixir_config.py
+-rw-rw-rw-   0        0        0     6958 2024-04-28 19:42:19.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir/mixelixirutil.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:23:14.761326 xiuxian_mixelixir-0.30/xiuxian_mixelixir.egg-info/
+-rw-rw-rw-   0        0        0      257 2024-04-28 20:23:14.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-28 20:23:14.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:23:14.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 20:23:14.000000 xiuxian_mixelixir-0.30/xiuxian_mixelixir.egg-info/top_level.txt
```

### Comparing `xiuxian_mixelixir-0.12/xiuxian_mixelixir/__init__.py` & `xiuxian_mixelixir-0.30/xiuxian_mixelixir/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     PRIVATE_FRIEND,
     GROUP,
     Message,
     GroupMessageEvent,
     MessageSegment
 )
 from nonebot.permission import SUPERUSER
-from xiuxian.xiuxian2_handle import XiuxianDateManage
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage
 from datetime import datetime
-from xiuxian.xiuxian_opertion import do_is_work
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.xiuxian_opertion import do_is_work
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
 from nonebot.log import logger
-from xiuxian.utils import data_check_conf, check_user, send_forward_msg, get_msg_pic, pic_msg_format
-from xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.utils import data_check_conf, check_user, send_forward_msg, get_msg_pic, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.item_json import Items
 from .mixelixirutil import get_mix_elixir_msg, tiaohe, check_mix
-from xiuxian.read_buff import get_player_info, save_player_info
-from xiuxian.xiuxian_config import USERRANK, XiuConfig
+from nonebot_plugin_simulator_xiuxian.read_buff import get_player_info, save_player_info
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import USERRANK, XiuConfig
 from datetime import datetime
 import random
 import re
 
 sql_message = XiuxianDateManage()  # sql类
 items = Items()
 from .mix_elixir_config import MIXELIXIRCONFIG
```

### Comparing `xiuxian_mixelixir-0.12/xiuxian_mixelixir/mixelixirutil.py` & `xiuxian_mixelixir-0.30/xiuxian_mixelixir/mixelixirutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.item_json import Items
 import json
 import os
 from pathlib import Path
 
 
 mix_config = Items().get_data_by_item_type(['合成丹药'])
 mix_configs = {}
```

