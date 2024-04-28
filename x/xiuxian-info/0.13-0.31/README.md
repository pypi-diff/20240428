# Comparing `tmp/xiuxian_info-0.13.tar.gz` & `tmp/xiuxian_info-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_info-0.13.tar", last modified: Thu Apr 25 01:47:10 2024, max compression
+gzip compressed data, was "xiuxian_info-0.31.tar", last modified: Sun Apr 28 20:22:51 2024, max compression
```

## Comparing `xiuxian_info-0.13.tar` & `xiuxian_info-0.31.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:47:10.232824 xiuxian_info-0.13/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:47:10.232824 xiuxian_info-0.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:47:10.233824 xiuxian_info-0.13/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 01:47:05.000000 xiuxian_info-0.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:47:10.226824 xiuxian_info-0.13/xiuxian_info/
--rw-rw-rw-   0        0        0     7295 2024-04-25 01:46:40.000000 xiuxian_info-0.13/xiuxian_info/__init__.py
--rw-rw-rw-   0        0        0     1814 2024-04-22 01:25:08.000000 xiuxian_info-0.13/xiuxian_info/download.py
--rw-rw-rw-   0        0        0     6260 2024-04-25 01:17:51.000000 xiuxian_info-0.13/xiuxian_info/draw_user_info.py
--rw-rw-rw-   0        0        0      890 2024-04-22 01:25:08.000000 xiuxian_info-0.13/xiuxian_info/infoconfig.py
--rw-rw-rw-   0        0        0      963 2024-04-22 01:25:08.000000 xiuxian_info-0.13/xiuxian_info/send_image_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:47:10.231825 xiuxian_info-0.13/xiuxian_info.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:47:10.000000 xiuxian_info-0.13/xiuxian_info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-25 01:47:10.000000 xiuxian_info-0.13/xiuxian_info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:47:10.000000 xiuxian_info-0.13/xiuxian_info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 01:47:10.000000 xiuxian_info-0.13/xiuxian_info.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:22:51.411345 xiuxian_info-0.31/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:22:51.410345 xiuxian_info-0.31/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:22:51.411345 xiuxian_info-0.31/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:22:44.000000 xiuxian_info-0.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:22:51.405345 xiuxian_info-0.31/xiuxian_info/
+-rw-rw-rw-   0        0        0     7420 2024-04-28 19:41:24.000000 xiuxian_info-0.31/xiuxian_info/__init__.py
+-rw-rw-rw-   0        0        0     1814 2024-04-22 01:25:08.000000 xiuxian_info-0.31/xiuxian_info/download.py
+-rw-rw-rw-   0        0        0     6213 2024-04-28 20:21:08.000000 xiuxian_info-0.31/xiuxian_info/draw_user_info.py
+-rw-rw-rw-   0        0        0      890 2024-04-22 01:25:08.000000 xiuxian_info-0.31/xiuxian_info/infoconfig.py
+-rw-rw-rw-   0        0        0      963 2024-04-22 01:25:08.000000 xiuxian_info-0.31/xiuxian_info/send_image_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:22:51.410345 xiuxian_info-0.31/xiuxian_info.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:22:51.000000 xiuxian_info-0.31/xiuxian_info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-28 20:22:51.000000 xiuxian_info-0.31/xiuxian_info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:22:51.000000 xiuxian_info-0.31/xiuxian_info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:22:51.000000 xiuxian_info-0.31/xiuxian_info.egg-info/top_level.txt
```

### Comparing `xiuxian_info-0.13/xiuxian_info/__init__.py` & `xiuxian_info-0.31/xiuxian_info/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     GROUP_OWNER,
     Message,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment,
 )
 
-from xiuxian.xiuxian2_handle import XiuxianDateManage, OtherSet
-from xiuxian.data_source import jsondata
+from nonebot_plugin_simulator_xiuxian.xiuxian2_handle import XiuxianDateManage, OtherSet
+from nonebot_plugin_simulator_xiuxian.data_source import jsondata
 from .draw_user_info import draw_user_info_img
-from xiuxian.cd_manager import add_cd, check_cd, cd_msg
+from nonebot_plugin_simulator_xiuxian.cd_manager import add_cd, check_cd, cd_msg
 from .infoconfig import get_config
-from xiuxian.utils import data_check_conf
-from xiuxian.read_buff import UserBuffDate
+from nonebot_plugin_simulator_xiuxian.utils import data_check_conf
+from nonebot_plugin_simulator_xiuxian.read_buff import UserBuffDate
 
 config = get_config()
 
 def format_number(number: int) -> str:
     if number >= 1000000000000:
         return str(round(number / 1000000000000, 1)) + "万亿"
     elif number >= 100000000:
```

### Comparing `xiuxian_info-0.13/xiuxian_info/download.py` & `xiuxian_info-0.31/xiuxian_info/download.py`

 * *Files identical despite different names*

### Comparing `xiuxian_info-0.13/xiuxian_info/draw_user_info.py` & `xiuxian_info-0.31/xiuxian_info/draw_user_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from PIL import Image, ImageDraw, ImageFont
 import asyncio
 from pathlib import Path
 
 from .download import get_avatar_by_user_id_and_save
 
 from .send_image_tool import convert_img
-
-back = Path(__file__).parent / 'back.png'
-line2 = Path(__file__).parent / 'line2.png'
-line3 = Path(__file__).parent / 'line3.png'
-line4 = Path(__file__).parent / 'line4.png'
-user_state = Path(__file__).parent / 'user_state.png'
+DATSA = Path() / 'data' / 'xiuxian' / 'texture2d'
+back = DATSA / 'back.png'
+line2 = DATSA / 'line2.png'
+line3 = DATSA / 'line3.png'
+line4 = DATSA / 'line4.png'
+user_state = DATSA / 'user_state.png'
 
 first_color = (242, 250, 242)
 second_color = (57, 57, 57)
 
-FONT_ORIGIN_PATH = Path(__file__).parent / 'font.ttf'
+FONT_ORIGIN_PATH = DATSA / 'font.ttf'
 
 def font_origin(size: int) -> ImageFont.FreeTypeFont:
     return ImageFont.truetype(str(FONT_ORIGIN_PATH), size=size)
 
 
 font_36 = font_origin(36)
 font_40 = font_origin(40)
```

### Comparing `xiuxian_info-0.13/xiuxian_info/infoconfig.py` & `xiuxian_info-0.31/xiuxian_info/infoconfig.py`

 * *Files identical despite different names*

### Comparing `xiuxian_info-0.13/xiuxian_info/send_image_tool.py` & `xiuxian_info-0.31/xiuxian_info/send_image_tool.py`

 * *Files identical despite different names*

