# Comparing `tmp/nonebot-plugin-hx-yinying-1.1.3.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.3.tar", last modified: Sun Apr 28 11:47:04 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.4.tar", last modified: Sun Apr 28 13:01:19 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.1.3.tar` & `nonebot-plugin-hx-yinying-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 11:47:04.713273 nonebot-plugin-hx-yinying-1.1.3/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     5087 2024-04-28 11:47:04.714275 nonebot-plugin-hx-yinying-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 11:47:04.632235 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    56854 2024-04-28 11:08:06.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    92065 2024-04-28 11:39:35.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1532 2024-04-28 09:04:32.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2405 2024-04-28 11:45:02.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     4111 2024-04-28 11:42:05.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5038 2024-04-28 10:07:11.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-04-28 11:47:04.708277 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     5087 2024-04-28 11:47:03.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-28 11:47:04.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 11:47:03.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-04-28 11:47:03.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-28 11:47:03.000000 nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-28 11:47:04.733160 nonebot-plugin-hx-yinying-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1002 2024-04-28 11:46:41.000000 nonebot-plugin-hx-yinying-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:01:19.413522 nonebot-plugin-hx-yinying-1.1.4/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5087 2024-04-28 13:01:19.413522 nonebot-plugin-hx-yinying-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 13:01:19.305421 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    56854 2024-04-28 11:08:06.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    91353 2024-04-28 12:53:22.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1532 2024-04-28 12:57:10.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2364 2024-04-28 12:09:24.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     4111 2024-04-28 11:42:05.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5038 2024-04-28 10:07:11.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:01:19.402468 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     5087 2024-04-28 13:01:18.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-28 13:01:18.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:01:18.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-04-28 13:01:18.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-28 13:01:18.000000 nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-28 13:01:19.423679 nonebot-plugin-hx-yinying-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2024-04-28 13:00:45.000000 nonebot-plugin-hx-yinying-1.1.4/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.1.3/LICENSE` & `nonebot-plugin-hx-yinying-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.3/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.3
+Version: 1.1.4
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.4 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.3/README.md` & `nonebot-plugin-hx-yinying-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import operator,nonebot
 from nonebot import get_plugin_config, logger, require,get_driver
 from pathlib import Path
 require("nonebot_plugin_localstore")
 import nonebot_plugin_localstore as store
 from .image_check import image_check
 
+
 hx_config = get_plugin_config(Config)
 
 #判断主要配置文件夹是否存在！
 if hx_config.hx_path == None:
     logger.warning("找不到配置里的路径，将使用默认配置")
     lg.opt(colors=True).success( f"""
     <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
@@ -1510,51 +1511,35 @@
         if text == "！d" or text == "/！d":
             return
         else:
             msg = "诶唔，你叫我是有什么事嘛？"
             await send_msg(matcher,event,msg)
     elif img != []:
         in_img = await image_check(img[0])
-        try:
-            back_msg = str(await yinying(groupid,id,text,nick,in_img))
-            msg = back_msg.replace("/n","\n")
-            await send_msg(matcher,event,msg)
-        except Exception as e:
-            back_msg = f"请求接口报错！\n返回结果：{e}"
-            await send_msg(matcher, event, back_msg)
+        back_msg = str(await yinying(groupid,id,text,nick,in_img))
+        msg = back_msg.replace("/n","\n")
+        await send_msg(matcher,event,msg)
     else:
-        try:
-            back_msg = str(await yinying(groupid,id,text,nick))
-            msg = back_msg.replace("/n","\n")
-            await send_msg(matcher,event,msg)
-        except Exception as e:
-            back_msg = f"请求接口报错！\n返回结果：{e}"
-            await send_msg(matcher, event, back_msg)
+        back_msg = str(await yinying(groupid,id,text,nick,False))
+        msg = back_msg.replace("/n","\n")
+        await send_msg(matcher,event,msg)
 
 #获取回复（指令触发）
 async def get_answer_ml(matcher, event ,bot ,msg):
     text = msg.extract_plain_text()
     img = await get_img_urls(event)
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     user_in(id,json_replace(text))
-    if not text == "" or text == None:
-        try:
-            back_msg = str(await yinying(groupid,id,text,nick))
-            msg = back_msg.replace("/n","\n")
-            await send_msg(matcher,event,msg)
-        except Exception as e:
-            back_msg = f"请求接口报错！\n返回结果：{e}"
-            await send_msg(matcher, event, back_msg)
-    elif img == "" or img == []:
+    if  text == "" or text == None and img == []:
         msg = "诶唔，你叫我是有什么事嘛？"
         await send_msg(matcher,event,msg)
-    else:
+    elif img != []:
         in_img = await image_check(img[0])
-        try:
-            back_msg = str(await yinying(groupid,id,text,nick,in_img))
-            msg = back_msg.replace("/n","\n")
-            await send_msg(matcher,event,msg)
-        except Exception as e:
-            back_msg = f"请求接口报错！\n返回结果：{e}"
-            await send_msg(matcher, event, back_msg)
+        back_msg = str(await yinying(groupid,id,text,nick,in_img))
+        msg = back_msg.replace("/n","\n")
+        await send_msg(matcher,event,msg)
+    else:
+        back_msg = str(await yinying(groupid,id,text,nick,False))
+        msg = back_msg.replace("/n","\n")
+        await send_msg(matcher,event,msg)
```

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional, Union
 import nonebot
 from pydantic import BaseModel,AnyHttpUrl,Field
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.1.3"
+    hx_version: Optional[str] = "1.1.4"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
     # 秩乱给你的token
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
```

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/image_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,18 +48,17 @@
         scan_image_request = ScanImageAdvanceRequest(
         task=[task1],
         scene=['porn']
         )
         try:
             client = Client(config)
             response = client.scan_image_advance(scan_image_request, runtime_option)
-            logger.debug(response.body)
             back = response.body.to_map()
             msg0 = back["Data"]["Results"][0]["SubResults"][0]["Rate"]
-            if msg0 >= 0.6:
+            if msg0 <= 0.6:
                 logger.warning(f"[Hx]图片违规，请重新上传")
                 msg = False
             else:
                 msg = img0
             return msg
         except Exception as e:
             return False
```

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/report.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying/smms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.1.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.3
+Version: 1.1.4
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.4 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.3/setup.py` & `nonebot-plugin-hx-yinying-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.1.3",
+    version="1.1.4",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

