# Comparing `tmp/nonebot_plugin_analysis_bilibili-2.6.9.tar.gz` & `tmp/nonebot_plugin_analysis_bilibili-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.6.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.7.0.tar", max compression
```

## Comparing `nonebot_plugin_analysis_bilibili-2.6.9.tar` & `nonebot_plugin_analysis_bilibili-2.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2738 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/README.md
--rw-r--r--   0        0        0     4932 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/__init__.py
--rw-r--r--   0        0        0    16850 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
--rw-r--r--   0        0        0     2284 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/wbi.py
--rw-r--r--   0        0        0      575 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/pyproject.toml
--rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.6.9/PKG-INFO
+-rw-r--r--   0        0        0     2851 2024-04-28 07:16:01.020735 nonebot_plugin_analysis_bilibili-2.7.0/README.md
+-rw-r--r--   0        0        0     4990 2024-04-28 07:16:01.020735 nonebot_plugin_analysis_bilibili-2.7.0/nonebot_plugin_analysis_bilibili/__init__.py
+-rw-r--r--   0        0        0    17419 2024-04-28 07:16:01.020735 nonebot_plugin_analysis_bilibili-2.7.0/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
+-rw-r--r--   0        0        0     2284 2024-04-28 07:16:01.020735 nonebot_plugin_analysis_bilibili-2.7.0/nonebot_plugin_analysis_bilibili/wbi.py
+-rw-r--r--   0        0        0      573 2024-04-28 07:16:01.020735 nonebot_plugin_analysis_bilibili-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.7.0/PKG-INFO
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.9/README.md` & `nonebot_plugin_analysis_bilibili-2.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 ```
 # 当图片大小超过下值时，修改图片大小，不填则发送原图，example: 100h / 100w / 100h_100w
 analysis_images_size = ""
 analysis_cover_images_size = "" # 封面图大小，和上面相同，视频、直播、番剧 封面图使用这个大小
 analysis_blacklist = [123456789] # 不解析里面填写的QQ号发的链接 List[int | str]
 analysis_group_blacklist = [123456789] # 不解析里面填写的QQ群号发的链接 List[int | str]
 analysis_desc_blacklist = [123456789] # 里面填写的群号，发送的解析内容不包含简介 List[int | str]
+analysis_reanalysis_time = 0 # 同一个视频重新解析时间，单位秒，0为不重新解析，example: 60
 analysis_display_image = true # 是否显示封面 true/false
 # 哪种类型需要显示封面，与上一项相冲突，上一项为true则全开 List[str]
 analysis_display_image_list = ["video", "bangumi", "live", "article", "dynamic"]
 analysis_enable_search = false # 是否开启搜视频功能 true/false  example: "搜视频 123456"
 
 
 analysis_trust_env = false # 是否使用环境变量或者当前系统正在使用中的代理设置 true/false
```

#### html2text {}

```diff
@@ -11,15 +11,17 @@
 "" # å°é¢å¾å¤§å°ï¼åä¸é¢ç¸åï¼è§é¢ãç´æ­ãçªå§
 å°é¢å¾ä½¿ç¨è¿ä¸ªå¤§å° analysis_blacklist = [123456789] #
 ä¸è§£æéé¢å¡«åçQQå·åçé¾æ¥ List[int | str]
 analysis_group_blacklist = [123456789] #
 ä¸è§£æéé¢å¡«åçQQç¾¤å·åçé¾æ¥ List[int | str]
 analysis_desc_blacklist = [123456789] #
 éé¢å¡«åçç¾¤å·ï¼åéçè§£æåå®¹ä¸åå«ç®ä» List[int | str]
-analysis_display_image = true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
+analysis_reanalysis_time = 0 #
+åä¸ä¸ªè§é¢éæ°è§£ææ¶é´ï¼åä½ç§ï¼0ä¸ºä¸éæ°è§£æï¼example:
+60 analysis_display_image = true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
 åªç§ç±»åéè¦æ¾ç¤ºå°é¢ï¼ä¸ä¸ä¸é¡¹ç¸å²çªï¼ä¸ä¸é¡¹ä¸ºtrueåå¨å¼
 List[str] analysis_display_image_list = ["video", "bangumi", "live", "article",
 "dynamic"] analysis_enable_search = false # æ¯å¦å¼å¯æè§é¢åè½ true/
 false example: "æè§é¢ 123456" analysis_trust_env = false #
 æ¯å¦ä½¿ç¨ç¯å¢åéæèå½åç³»ç»æ­£å¨ä½¿ç¨ä¸­çä»£çè®¾ç½® true/
 false ``` ## å®è£ 1. ä½¿ç¨ nb-cli
 å®è£ï¼ä¸éè¦æå¨æ·»å å¥å£ï¼æ´æ°ä½¿ç¨ pip (æ¨è) ``` nb plugin
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/__init__.py` & `nonebot_plugin_analysis_bilibili-2.7.0/nonebot_plugin_analysis_bilibili/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,29 +95,31 @@
         elif is_image(i):
             msg.append(Image(i))
         else:
             msg.append(Text(i))
     return msg
 
 
-async def send_msg(msg_list: List[Union[List[str], str]]) -> None:
+async def send_msg(msg_list: List[Union[List[str], str, bool]]) -> None:
+    if msg_list is False:
+        return
     if msg_list is None:
         logger.warning("此次解析的内容为空，接口可能被修改，需要更新！")
         return
 
     try:
         await MessageFactory(format_msg(msg_list)).send()
     except RuntimeError:
         await analysis_bili.send(format_msg(msg_list, is_plain_text=True))
     except Exception as e:
         logger.exception(e)
         logger.warning(f"{msg_list}\n此次解析的内容可能被风控！")
 
 
-async def get_msg(event: Event, text: str, search: bool = False) -> List[str]:
+async def get_msg(event: Event, text: str, search: bool = False) -> Union[List[str], bool]:
     group_id = str(
         event.group_id
         if hasattr(event, "group_id")
         else event.channel_id
         if hasattr(event, "channel_id")
         else None
     )
@@ -137,15 +139,15 @@
             # 说明是错误信息
             await analysis_bili.finish(msg)
 
         if group_id in desc_blacklist:
             if msg[-1].startswith("简介"):
                 msg[-1] = ""
 
-        return msg
+    return msg
 
 
 @analysis_bili.handle()
 async def handle_analysis(event: Event) -> None:
     text = str(event.message).strip()
     msg = await get_msg(event, text)
     await send_msg(msg)
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py` & `nonebot_plugin_analysis_bilibili-2.7.0/nonebot_plugin_analysis_bilibili/analysis_bilibili.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import re
-import json
 import nonebot
 
-from time import localtime, strftime
+from time import time, localtime, strftime
 from typing import Dict, List, Optional, Tuple, Union
 from aiohttp import ClientSession
 
 from .wbi import get_query
 
 
-# group_id : last_vurl
-analysis_stat: Dict[int, str] = {}
+# group_id : [last_vurl, last_analysis_time]
+analysis_stat: Dict[int, List] = {}
 
 config = nonebot.get_driver().config
 analysis_display_image = getattr(config, "analysis_display_image", False)
 analysis_display_image_list = getattr(config, "analysis_display_image_list", [])
 images_size = getattr(config, "analysis_images_size", "")
 cover_images_size = getattr(config, "analysis_cover_images_size", "")
+reanalysis_time = getattr(config, "analysis_reanalysis_time", 0)
 
 
 def resize_image(src: str, is_cover=False) -> str:
     img_type = src[-3:]
     if cover_images_size and is_cover:
         return f"{src}@{cover_images_size}.{img_type}"
     if images_size:
         return f"{src}@{images_size}.{img_type}"
     return src
 
 
 async def bili_keyword(
     group_id: Optional[int], text: str, session: ClientSession
-) -> Union[List[Union[List[str], str]], str]:
+) -> Union[List[Union[List[str], str]], str, bool]:
     try:
         # 提取url
         url, page, time_location = extract(text)
         # 如果是小程序就去搜索标题
         if not url:
             if title := re.search(r'"desc":("[^"哔哩]+")', text):
                 vurl = await search_bili_by_title(title[1], session)
@@ -43,28 +43,29 @@
 
         # 获取视频详细信息
         msg, vurl = "", ""
         if "view?" in url:
             msg, vurl = await video_detail(
                 url, page=page, time_location=time_location, session=session
             )
-        elif "bangumi" in url:
+        elif "pgc" in url:
             msg, vurl = await bangumi_detail(url, time_location, session)
         elif "xlive" in url:
             msg, vurl = await live_detail(url, session)
         elif "article" in url:
             msg, vurl = await article_detail(url, page, session)
         elif "dynamic" in url:
             msg, vurl = await dynamic_detail(url, session)
 
         # 避免多个机器人解析重复推送
         if group_id:
-            if group_id in analysis_stat and analysis_stat[group_id] == vurl:
-                return ""
-            analysis_stat[group_id] = vurl
+            if group_id in analysis_stat and analysis_stat[group_id][0] == vurl:
+                if not reanalysis_time or analysis_stat[group_id][1] + int(reanalysis_time) > int(time()):
+                    return False
+            analysis_stat[group_id] = [vurl, int(time())]
     except Exception as e:
         msg = "bili_keyword Error: {}".format(type(e))
     return msg
 
 
 async def b23_extract(text: str, session: ClientSession) -> str:
     b23 = re.compile(r"b23.tv/(\w+)|(bili(22|23|33|2233).cn)/(\w+)", re.I).search(
@@ -107,20 +108,20 @@
         dynamic_id = re.compile(r"(t|m).bilibili.com/(\d+)", re.I).search(text)
         if bvid:
             url = f"https://api.bilibili.com/x/web-interface/view?bvid={bvid[0]}"
         elif aid:
             url = f"https://api.bilibili.com/x/web-interface/view?aid={aid[0][2:]}"
         elif epid:
             url = (
-                f"https://bangumi.bilibili.com/view/web_api/season?ep_id={epid[0][2:]}"
+                f"https://api.bilibili.com/pgc/view/web/season?ep_id={epid[0][2:]}"
             )
         elif ssid:
-            url = f"https://bangumi.bilibili.com/view/web_api/season?season_id={ssid[0][2:]}"
+            url = f"https://api.bilibili.com/pgc/view/web/season?season_id={ssid[0][2:]}"
         elif mdid:
-            url = f"https://bangumi.bilibili.com/view/web_api/season?media_id={mdid[0][2:]}"
+            url = f"https://api.bilibili.com/pgc/review/user?media_id={mdid[0][2:]}"
         elif room_id:
             url = f"https://api.live.bilibili.com/xlive/web-room/v1/index/getInfoByRoom?room_id={room_id[2]}"
         elif cvid:
             page = cvid[4]
             url = f"https://api.bilibili.com/x/article/viewinfo?id={page}&mobi_app=pc&from=web"
         elif dynamic_id_type2:
             url = f"https://api.bilibili.com/x/polymer/web-dynamic/v1/detail?rid={dynamic_id_type2[2]}&type=2"
@@ -209,46 +210,55 @@
         return msg, None
 
 
 async def bangumi_detail(
     url: str, time_location: str, session: ClientSession
 ) -> Tuple[List[str], str]:
     try:
+        is_media = False
+        if "media_id" in url:
+            is_media = True
+            async with session.get(url) as resp:
+                ssid = (await resp.json()).get("result").get("media").get("season_id")
+                if not ssid:
+                    return None, None
+            url = f"https://api.bilibili.com/pgc/view/web/season?season_id={ssid}"
+
         async with session.get(url) as resp:
             res = (await resp.json()).get("result")
             if not res:
                 return None, None
 
         has_image = False
         if analysis_display_image or "bangumi" in analysis_display_image_list:
             has_image = True
 
         cover = resize_image(res["cover"], is_cover=True) if has_image else ""
         title = f"番剧：{res['title']}\n"
-        desc = f"{res['newest_ep']['desc']}\n"
-        index_title = ""
-        style = "".join(f"{i}," for i in res["style"])
-        style = f"类型：{style[:-1]}\n"
+        desc = f"{res['new_ep']['desc']}\n"
+        long_title = ""
+        styles = "".join(f"{i}," for i in res["styles"])
+        styles = f"类型：{styles[:-1]}\n"
         evaluate = f"简介：{res['evaluate']}\n"
-        if "season_id" in url:
-            vurl = f"https://www.bilibili.com/bangumi/play/ss{res['season_id']}"
-        elif "media_id" in url:
+        if is_media:
             vurl = f"https://www.bilibili.com/bangumi/media/md{res['media_id']}"
+        elif "season_id" in url:
+            vurl = f"https://www.bilibili.com/bangumi/play/ss{res['season_id']}"
         else:
             epid = re.compile(r"ep_id=\d+").search(url)[0][len("ep_id=") :]
             for i in res["episodes"]:
                 if str(i["ep_id"]) == epid:
-                    index_title = f"标题：{i['index_title']}\n"
+                    long_title = f"标题：{i['long_title']}\n"
                     break
             vurl = f"https://www.bilibili.com/bangumi/play/ep{epid}"
         if time_location:
             time_location = time_location[0].replace("&amp;", "&")[3:]
             vurl += f"?t={time_location}"
         vurl = "\n" + vurl if cover else vurl
-        msg = [cover, f"{vurl}\n", title, index_title, desc, style, evaluate]
+        msg = [cover, f"{vurl}\n", title, long_title, desc, styles, evaluate]
         return msg, vurl
     except Exception as e:
         msg = "番剧解析出错--Error: {}".format(type(e))
         msg += f"\n{url}"
         return msg, None
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/wbi.py` & `nonebot_plugin_analysis_bilibili-2.7.0/nonebot_plugin_analysis_bilibili/wbi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_analysis_bilibili-2.6.9/pyproject.toml` & `nonebot_plugin_analysis_bilibili-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-analysis-bilibili"
-version = "2.6.9"
+version = "2.7.0"
 description = "nonebot2解析bilibili插件"
 authors = ["mengshouer"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/mengshouer/nonebot_plugin_analysis_bilibili"
 keywords = ["nonebot", "nonebot2", "bilibili"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.7"
 nonebot2 = "^2.1.1"
-nonebot-plugin-send-anything-anywhere = "^0.3"
+nonebot-plugin-send-anything-anywhere = "^0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.9/PKG-INFO` & `nonebot_plugin_analysis_bilibili-2.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-analysis-bilibili
-Version: 2.6.9
+Version: 2.7.0
 Summary: nonebot2解析bilibili插件
 Home-page: https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
 License: MIT
 Keywords: nonebot,nonebot2,bilibili
 Author: mengshouer
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.7,<4.0)
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.3,<0.4)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0,<1)
 Requires-Dist: nonebot2 (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
 Description-Content-Type: text/markdown
 
 <!--
  * @Author         : mengshouer
  * @Date           : 2021-03-16 00:00:00
@@ -62,14 +62,15 @@
 ```
 # 当图片大小超过下值时，修改图片大小，不填则发送原图，example: 100h / 100w / 100h_100w
 analysis_images_size = ""
 analysis_cover_images_size = "" # 封面图大小，和上面相同，视频、直播、番剧 封面图使用这个大小
 analysis_blacklist = [123456789] # 不解析里面填写的QQ号发的链接 List[int | str]
 analysis_group_blacklist = [123456789] # 不解析里面填写的QQ群号发的链接 List[int | str]
 analysis_desc_blacklist = [123456789] # 里面填写的群号，发送的解析内容不包含简介 List[int | str]
+analysis_reanalysis_time = 0 # 同一个视频重新解析时间，单位秒，0为不重新解析，example: 60
 analysis_display_image = true # 是否显示封面 true/false
 # 哪种类型需要显示封面，与上一项相冲突，上一项为true则全开 List[str]
 analysis_display_image_list = ["video", "bangumi", "live", "article", "dynamic"]
 analysis_enable_search = false # 是否开启搜视频功能 true/false  example: "搜视频 123456"
 
 
 analysis_trust_env = false # 是否使用环境变量或者当前系统正在使用中的代理设置 true/false
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.6.9
+Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.7.0
 Summary: nonebot2è§£æbilibiliæä»¶ Home-page: https://github.com/mengshouer/
 nonebot_plugin_analysis_bilibili License: MIT Keywords:
 nonebot,nonebot2,bilibili Author: mengshouer Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: aiohttp
-(>=3.7,<4.0) Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.3,<0.4)
+(>=3.7,<4.0) Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0,<1)
 Requires-Dist: nonebot2 (>=2.1.1,<3.0.0) Project-URL: Repository, https://
 github.com/mengshouer/nonebot_plugin_analysis_bilibili Description-Content-
 Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
            # nonebot_plugin_analysis_bilibili _â¨ NoneBot bilibili
                        è§é¢ãçªå§è§£ææä»¶ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -24,15 +24,17 @@
 "" # å°é¢å¾å¤§å°ï¼åä¸é¢ç¸åï¼è§é¢ãç´æ­ãçªå§
 å°é¢å¾ä½¿ç¨è¿ä¸ªå¤§å° analysis_blacklist = [123456789] #
 ä¸è§£æéé¢å¡«åçQQå·åçé¾æ¥ List[int | str]
 analysis_group_blacklist = [123456789] #
 ä¸è§£æéé¢å¡«åçQQç¾¤å·åçé¾æ¥ List[int | str]
 analysis_desc_blacklist = [123456789] #
 éé¢å¡«åçç¾¤å·ï¼åéçè§£æåå®¹ä¸åå«ç®ä» List[int | str]
-analysis_display_image = true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
+analysis_reanalysis_time = 0 #
+åä¸ä¸ªè§é¢éæ°è§£ææ¶é´ï¼åä½ç§ï¼0ä¸ºä¸éæ°è§£æï¼example:
+60 analysis_display_image = true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
 åªç§ç±»åéè¦æ¾ç¤ºå°é¢ï¼ä¸ä¸ä¸é¡¹ç¸å²çªï¼ä¸ä¸é¡¹ä¸ºtrueåå¨å¼
 List[str] analysis_display_image_list = ["video", "bangumi", "live", "article",
 "dynamic"] analysis_enable_search = false # æ¯å¦å¼å¯æè§é¢åè½ true/
 false example: "æè§é¢ 123456" analysis_trust_env = false #
 æ¯å¦ä½¿ç¨ç¯å¢åéæèå½åç³»ç»æ­£å¨ä½¿ç¨ä¸­çä»£çè®¾ç½® true/
 false ``` ## å®è£ 1. ä½¿ç¨ nb-cli
 å®è£ï¼ä¸éè¦æå¨æ·»å å¥å£ï¼æ´æ°ä½¿ç¨ pip (æ¨è) ``` nb plugin
```

