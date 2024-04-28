# Comparing `tmp/xiuxian_base-0.12.tar.gz` & `tmp/xiuxian_base-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_base-0.12.tar", last modified: Thu Apr 25 01:39:43 2024, max compression
+gzip compressed data, was "xiuxian_base-0.30.tar", last modified: Sun Apr 28 20:05:28 2024, max compression
```

## Comparing `xiuxian_base-0.12.tar` & `xiuxian_base-0.30.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:39:43.778948 xiuxian_base-0.12/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:39:43.778948 xiuxian_base-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:39:43.779972 xiuxian_base-0.12/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 00:04:31.000000 xiuxian_base-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:39:43.770706 xiuxian_base-0.12/xiuxian_base/
--rw-rw-rw-   0        0        0    51818 2024-04-25 01:11:19.000000 xiuxian_base-0.12/xiuxian_base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:39:43.777945 xiuxian_base-0.12/xiuxian_base.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:39:43.000000 xiuxian_base-0.12/xiuxian_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-25 01:39:43.000000 xiuxian_base-0.12/xiuxian_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:39:43.000000 xiuxian_base-0.12/xiuxian_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:39:43.000000 xiuxian_base-0.12/xiuxian_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:28.896187 xiuxian_base-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:05:28.895173 xiuxian_base-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:05:28.896187 xiuxian_base-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:03:20.000000 xiuxian_base-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:28.887648 xiuxian_base-0.30/xiuxian_base/
+-rw-rw-rw-   0        0        0    52018 2024-04-28 19:58:19.000000 xiuxian_base-0.30/xiuxian_base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:28.895173 xiuxian_base-0.30/xiuxian_base.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:05:28.000000 xiuxian_base-0.30/xiuxian_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-28 20:05:28.000000 xiuxian_base-0.30/xiuxian_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:05:28.000000 xiuxian_base-0.30/xiuxian_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:05:28.000000 xiuxian_base-0.30/xiuxian_base.egg-info/top_level.txt
```

### Comparing `xiuxian_base-0.12/xiuxian_base/__init__.py` & `xiuxian_base-0.30/xiuxian_base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     GroupMessageEvent,
     MessageSegment,
 )
 from nonebot.log import logger
 from typing import Any, Tuple
 from nonebot.params import CommandArg, RegexGroup, EventPlainText
 from nonebot.permission import SUPERUSER
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
-from xiuxian.data_source import jsondata
-from xiuxian.xiuxian2_handle import XiuxianDateManage, XiuxianJsonDate, OtherSet
-from xiuxian.xiuxian_config import XiuConfig, JsonConfig
-from xiuxian.xiuxian_opertion import do_is_work
-from xiuxian.read_buff import UserBuffDate
-from xiuxian.utils import Txt2Img, data_check_conf, check_user_type, get_msg_pic, check_user, pic_msg_format
-from xiuxian.item_json import Items
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.data_source import jsondata
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage, XiuxianJsonDate, OtherSet
+from nonebot_plugin_simulator_xiuxian.xiuxian_config import XiuConfig, JsonConfig
+from nonebot_plugin_simulator_xiuxian.xiuxian_opertion import do_is_work
+from nonebot_plugin_simulator_xiuxian.read_buff import UserBuffDate
+from nonebot_plugin_simulator_xiuxian.utils import Txt2Img, data_check_conf, check_user_type, get_msg_pic, check_user, pic_msg_format
+from nonebot_plugin_simulator_xiuxian.item_json import Items
 
 
 run_xiuxian = on_command("我要修仙", priority=5)
 restart = on_command("再入仙途", aliases={"重新修仙", "重入仙途"}, priority=5)
 package = on_command("我的纳戒", aliases={"升级纳戒"}, priority=5)
 sign_in = on_command("修仙签到", priority=5)
 help_in = on_command("修仙帮助", priority=5)
```

