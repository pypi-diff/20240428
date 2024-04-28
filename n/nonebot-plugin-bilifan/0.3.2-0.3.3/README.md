# Comparing `tmp/nonebot_plugin_bilifan-0.3.2.tar.gz` & `tmp/nonebot_plugin_bilifan-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.3.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.3.3.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.3.2.tar` & `nonebot_plugin_bilifan-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/LICENSE
--rw-r--r--   0        0        0     2246 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/README.md
--rw-r--r--   0        0        0     7335 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4879 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     6387 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       80 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17637 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    18385 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2197 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     2745 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/utils.py
--rw-r--r--   0        0        0     1876 2024-01-25 10:09:51.368909 nonebot_plugin_bilifan-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2246 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/README.md
+-rw-r--r--   0        0        0     8034 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     6064 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     6616 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       80 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    17653 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    19425 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2197 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     3020 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/utils.py
+-rw-r--r--   0        0        0     2061 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.3.2/LICENSE` & `nonebot_plugin_bilifan-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.2/README.md` & `nonebot_plugin_bilifan-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/__init__.py` & `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import shutil
 from pathlib import Path
+from typing import List
 
 # import aiohttp
 from nonebot import get_driver, on_command, require
 from nonebot.adapters import Event
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
@@ -19,22 +20,24 @@
     from nonebot_plugin_apscheduler import scheduler
 except BaseException:
     scheduler = None
 require("nonebot_plugin_saa")
 from nonebot_plugin_saa import Image, MessageFactory  # noqa: E402
 
 logger.opt(colors=True).info(
-    "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
-    if scheduler
-    else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>",
+    (
+        "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
+        if scheduler
+        else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
+    ),
 )
 
 
 driver = get_driver()
-__version__ = "0.3.0"
+__version__ = "0.3.3"
 __plugin_meta__ = PluginMetadata(
     name="bilifan",
     description="b站粉丝牌~",
     usage="发送 开始刷牌子 即可",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_bilifan",
     supported_adapters=inherit_supported_adapters("nonebot_plugin_saa"),
@@ -43,41 +46,54 @@
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 login_in = on_command("blogin", aliases={"b站登录"}, block=False)
 login_del = on_command("blogin_del", aliases={"删除登录信息"}, block=False)
 fan_once = on_command("bfan", aliases={"开始刷牌子", "开始粉丝牌"}, block=False)
-fan_auto = on_command("addfan", aliases={"自动刷牌子", "自动粉丝牌"}, priority=40, block=False)
+fan_auto = on_command(
+    "addfan",
+    aliases={"自动刷牌子", "自动粉丝牌"},
+    priority=40,
+    block=False,
+)
 del_only = on_command("bdel", aliases={"取消自动刷牌子", "取消自动粉丝牌"}, block=False)
-del_all = on_command("bdel_all", aliases={"删除全部定时任务"}, block=False, permission=SUPERUSER)
+del_all = on_command(
+    "bdel_all",
+    aliases={"删除全部定时任务"},
+    block=False,
+    permission=SUPERUSER,
+)
 
 
 @login_in.handle()
 async def _(matcher: Matcher, event: Event):
-    # try:
-    login_url, auth_code = await get_tv_qrcode_url_and_auth_code()
-    # except Exception as e:
-    #     print(e)
-    #     await matcher.finish("已超时，请稍后重试！")
+    try:
+        login_url, auth_code = await get_tv_qrcode_url_and_auth_code()
+    except Exception as e:
+        print(e)
+        await matcher.finish("已超时，请稍后重试！")
     data_path = Path().joinpath(f"data/bilifan/{event.get_user_id()}")
     data_path.mkdir(parents=True, exist_ok=True)
     data = await draw_QR(login_url)
-    forward_msg: list = ["本功能会调用并保存b站登录信息的cookie,请确保你在信任本机器人主人的情况下登录,如果出现财产损失,本作者对此不负责任"]
+    forward_msg: list = [
+        "本功能会调用并保存b站登录信息的cookie,请确保你在信任本机器人主人的情况下登录,如果出现财产损失,本作者对此不负责任",
+    ]
     forward_msg.append(Image(data))
     try:
         # if isinstance(event, GroupEvent):
         #     await bot.call_api(
         #         "send_group_forward_msg", group_id=event.group_id, messages=forward_msg
         #     )
         # else:
         await MessageFactory(forward_msg).send()
+        await matcher.send("或将此链接复制到手机B站打开:" + login_url)
     except Exception:
         logger.warning("二维码可能被风控，发送链接")
-        await matcher.send("或将此链接复制到手机B站打开:" + login_url)
+        await matcher.send("将此链接复制到手机B站打开:" + login_url)
     while True:
         a = await verify_login(auth_code, data_path)
         if a:
             await matcher.send(f"登录成功！\nqq:{event.get_user_id()}\n{a}")
             break
         await matcher.finish("登录失败！")
 
@@ -108,30 +124,38 @@
             logger.info(msg_path)
             users = await read_yaml(Path().joinpath("data/bilifan"))
             watchinglive = users.get("WATCHINGLIVE", None)
             await matcher.send(f"开始执行，预计将在{watchinglive}分钟后完成~")
         else:
             logger.info(msg_path)
             await matcher.finish("你尚未登录，请输入【b站登录】")
-        messageList = await mains(msg_path.parent)
+        messageList: List[str] = await mains(msg_path.parent)
         message_str = "\n".join(messageList)
         await matcher.finish(message_str)
     except (FileNotFoundError, SystemExit):
         await matcher.finish("你尚未登录，请输入【b站登录】")
 
 
 @fan_auto.handle()
 async def _(matcher: Matcher, event: Event):
     config = load_config()
     group_id = event.get_session_id()
 
     msg_path = Path().joinpath(f"data/bilifan/{event.get_user_id()}/login_info.txt")
     if msg_path.is_file():
         if event.get_user_id() in config:
-            await matcher.finish(f"{event.get_user_id()}的定时任务已存在")
+            users = await read_yaml(Path().joinpath("data/bilifan"))
+            cron = users.get("CRON", None)
+            try:
+                fields = cron.split(" ")
+                await matcher.finish(
+                    f"{event.get_user_id()}的定时任务已存在，将在每天{fields[0]}时{fields[1]}分开始执行~",
+                )
+            except AttributeError:
+                await matcher.finish("定时格式不正确，请删除定时任务后重新设置")
         else:
             config[event.get_user_id()] = group_id
             save_config(config)
             users = await read_yaml(Path().joinpath("data/bilifan"))
             cron = users.get("CRON", None)
             try:
                 fields = cron.split(" ")
@@ -173,14 +197,15 @@
     except AttributeError:
         logger.error("定时格式不正确，不启用定时功能")
         return
     if scheduler is None:
         logger.error("定时格式不正确，不启用定时功能")
         return
     try:
+        logger.info(f"定时任务已配置，将在每天{fields[0]}时{fields[1]}分后自动执行~")
         scheduler.add_job(
             auto_cup,
             "cron",
             hour=fields[0],
             minute=fields[1],
             id="auto_cup",
         )
```

### Comparing `nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/login/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,102 +3,123 @@
 import shutil
 import time
 import urllib.parse as urlparse
 from io import BytesIO
 from pathlib import Path
 
 import aiohttp
-
-# import qrcode_terminal
+import anyio
 import qrcode
 import yaml
 from nonebot.log import logger
 
-# Cookies = cookiejar.CookieJar()
-# session = requests.Session()
-# session.cookies = Cookies
-
 csrf = ""
 access_key = ""
 base_path = Path().joinpath("data/bilifan")
-headers = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
-}
 
 
 async def is_login(session, cookies):
     api = "https://api.bilibili.com/x/web-interface/nav"
-
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.99 Safari/537.36 Edg/97.0.1072.69",
+    }
     async with session.get(api, headers=headers, cookies=cookies) as resp:
         data = await resp.json()
         return data["code"] == 0, data["data"]["uname"]
 
 
 async def get_tv_qrcode_url_and_auth_code():
-    api = "https://passport.bilibili.com/x/passport-login/web/qrcode/generate"
+    api = "https://passport.bilibili.com/x/passport-tv-login/qrcode/auth_code"
     data = {
         "local_id": "0",
         "ts": str(int(time.time())),
     }
     await signature(data)
     async with aiohttp.ClientSession() as session:
-        async with session.get(
+        async with session.post(
             api,
             data=await map_to_string(data),
-            headers=headers,
-            # headers={"Content-Type": "application/x-www-form-urlencoded"},
+            cookies={},
+            headers={
+                "Host": "passport.bilibili.com",
+                "Content-Type": "application/x-www-form-urlencoded",
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.99 Safari/537.36 Edg/97.0.1072.69",
+            },
         ) as resp:
-            print(resp)
+            if resp.status != 200:
+                raise Exception("Failed to connect to server")
             resp_data = await resp.json()
             code = resp_data["code"]
             if code == 0:
                 login_url = resp_data["data"]["url"]
                 login_key = resp_data["data"]["qrcode_key"]
                 return login_url, login_key
             raise Exception("get_tv_qrcode_url_and_auth_code error")
 
 
-async def verify_login(auth_code, data_path):
-    api = "https://passport.bilibili.com/x/passport-login/web/qrcode/poll"
+async def verify_login(login_key: str, data_path: Path):
+    api = "https://passport.bilibili.com/x/passport-tv-login/qrcode/poll"
     data = {
-        "auth_code": auth_code,
+        "auth_code": login_key,
         "local_id": "0",
         "ts": str(int(time.time())),
     }
     await signature(data)
-    data_string = await map_to_string(data)
     while True:
         async with aiohttp.ClientSession() as session:
-            async with session.get(api, headers=headers) as resp:
+            async with session.post(
+                api,
+                data=await map_to_string(data),
+                cookies={},
+                headers={
+                    "Host": "passport.bilibili.com",
+                    "Content-Type": "application/x-www-form-urlencoded",
+                    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.99 Safari/537.36 Edg/97.0.1072.69",
+                },
+            ) as resp:
                 if resp.status != 200:
-                    print(resp)
                     raise Exception("Failed to connect to server")
                 response_dict = await resp.json()
                 code = response_dict["code"]
                 try:
                     access_key = response_dict["data"]["access_token"]
                 except Exception:
                     access_key = ""
                     await asyncio.sleep(3)
 
             if code == 0:
                 logger.success("登录成功")
-                with Path(data_path / "login_info.txt").open("w") as f:
+                filename = "login_info.txt"
+                data_path.mkdir(parents=True, exist_ok=True)
+                with (data_path / filename).open(mode="w", encoding="utf-8") as f:
                     f.write(access_key)
                 if not Path(data_path / "users.yaml").is_file():
                     logger.info("初始化配置文件")
                     shutil.copy2(
                         Path().joinpath("data/bilifan/users.yaml"),
                         data_path / "users.yaml",
                     )
-                with Path(data_path / "users.yaml").open("r", encoding="utf-8") as f:
-                    config = yaml.safe_load(f)
+                config = yaml.safe_load(
+                    await anyio.Path(data_path / "users.yaml").read_text("u8")
+                )
+                # with Path(data_path / "users.yaml").open(
+                #     "r", encoding="utf-8"
+                # ) as f:
+                #     config = yaml.safe_load(f)
+
                 config["USERS"][0]["access_key"] = access_key
-                with Path(data_path / "users.yaml").open("w", encoding="utf-8") as f:
-                    yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
+                config = yaml.dump(
+                    await anyio.Path(data_path / "users.yaml").write_text("u8"),
+                    allow_unicode=True,
+                    default_flow_style=False,
+                )
+                # with Path(data_path / "users.yaml").open(
+                #     "w", encoding="utf-8"
+                # ) as f:  # noqa: ASYNC101
+                #     yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
                 return "access_key已保存"
             await asyncio.sleep(3)
 
 
 appkey = "4409e2ce8ffd12b8"
 appsec = "59b43e04ad6965f34319062b478f83dd"
```

### Comparing `nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import itertools
 import json
 import os
 import warnings
 from pathlib import Path
 
 from nonebot.log import logger
-from nonebot.log import logger as log
 
 from .src import BiliUser
 
 local_path = Path(__file__).parent
 
 
 warnings.filterwarnings(
@@ -29,18 +28,26 @@
 
 async def read_yaml(msg_path: Path):
     global config, users
     try:
         if os.environ.get("USERS"):
             users = json.loads(os.environ.get("USERS"))  # type: ignore
         else:
+            import anyio
             import yaml
 
-            with Path(msg_path / "users.yaml").open("r", encoding="utf-8") as f:
-                users = yaml.load(f, Loader=yaml.FullLoader)
+            users = yaml.load(
+                await anyio.Path(msg_path / "users.yaml").read_text("u8"),
+                Loader=yaml.FullLoader,
+            )
+            # with Path(msg_path / "users.yaml").open(
+            #     "r", encoding="utf-8",
+            # ) as f:
+            #     users = yaml.load(f, Loader=yaml.FullLoader)
+
         assert users["ASYNC"] in [0, 1], "ASYNC参数错误"
         assert users["LIKE_CD"] >= 0, "LIKE_CD参数错误"
         assert users["ASYNC"] in [0, 1], "ASYNC参数错误"
         assert users["LIKE_CD"] >= 0, "LIKE_CD参数错误"
         # assert users['SHARE_CD'] >= 0, "SHARE_CD参数错误"
         assert users["DANMAKU_CD"] >= 0, "DANMAKU_CD参数错误"
         assert users["WATCHINGLIVE"] >= 0, "WATCHINGLIVE参数错误"
@@ -60,20 +67,20 @@
             "SIGNINGROUP": users.get("SIGNINGROUP", 2),
             "DANMAKU_CD": users["DANMAKU_CD"],
             "WATCHINGLIVE": users["WATCHINGLIVE"],
             "WEARMEDAL": users["WEARMEDAL"],
             "SIGNINGROUP": users.get("SIGNINGROUP", 2),
         }
     except Exception as e:
-        log.error(f"读取配置文件失败,请检查配置文件格式是否正确: {e}")
+        logger.error(f"读取配置文件失败,请检查配置文件格式是否正确: {e}")
         exit(1)
     return users
 
 
-@log.catch
+@logger.catch
 async def mains(msg_path):
     await read_yaml(msg_path)
     init_tasks = []
     start_tasks = []
     catch_msg = []
 
     for user in users["USERS"]:
@@ -96,89 +103,89 @@
             start_tasks.append(bili_user.start())
             catch_msg.append(bili_user.sendmsg())
 
     try:
         await asyncio.gather(*init_tasks)
         await asyncio.gather(*start_tasks)
     except Exception as e:
-        log.exception(e)
+        logger.exception(e)
         message_list = [f"任务执行失败: {e}"]
     else:
         message_list = []
 
     try:
         catch_msg_results = await asyncio.gather(*catch_msg)
     except Exception as e:
-        log.exception(e)
+        logger.exception(e)
         message_list.append(f"发送消息失败: {e}")
     else:
         message_list += list(itertools.chain.from_iterable(catch_msg_results))
 
-    [log.info(message) for message in message_list]
+    [logger.info(message) for message in message_list]
     return message_list
 
 
 def run(*args, **kwargs):  # noqa: ARG001
     loop = asyncio.new_event_loop()
     loop.run_until_complete(mains(Path().joinpath("data/bilifan")))
-    log.info("任务结束，等待下一次执行。")
+    logger.info("任务结束，等待下一次执行。")
 
 
 # if __name__ == '__main__':
 # cron = users.get('CRON', None)
 # cron = users.get('CRON', None)
 
 # if cron:
 #     from apscheduler.schedulers.blocking import BlockingScheduler
 #     from apscheduler.triggers.cron import CronTrigger
 # if cron:
 #     from apscheduler.schedulers.blocking import BlockingScheduler
 #     from apscheduler.triggers.cron import CronTrigger
 
-#     log.info(f'使用内置定时器 {cron}，开启定时任务，等待时间到达后执行。')
+#     logger.info(f'使用内置定时器 {cron}，开启定时任务，等待时间到达后执行。')
 #     schedulers = BlockingScheduler()
 #     schedulers.add_job(run, CronTrigger.from_crontab(cron), misfire_grace_time=3600)
 #     schedulers.start()
 # elif "--auto" in sys.argv:
 #     from apscheduler.schedulers.blocking import BlockingScheduler
 #     from apscheduler.triggers.interval import IntervalTrigger
 #     import datetime
-#     log.info(f'使用内置定时器 {cron}，开启定时任务，等待时间到达后执行。')
+#     logger.info(f'使用内置定时器 {cron}，开启定时任务，等待时间到达后执行。')
 #     schedulers = BlockingScheduler()
 #     schedulers.add_job(run, CronTrigger.from_crontab(cron), misfire_grace_time=3600)
 #     schedulers.start()
 # elif "--auto" in sys.argv:
 #     from apscheduler.schedulers.blocking import BlockingScheduler
 #     from apscheduler.triggers.interval import IntervalTrigger
 #     import datetime
 
-#     log.info('使用自动守护模式，每隔 24 小时运行一次。')
+#     logger.info('使用自动守护模式，每隔 24 小时运行一次。')
 #     scheduler = BlockingScheduler(timezone='Asia/Shanghai')
 #     scheduler.add_job(
 #         run,
 #         IntervalTrigger(hours=24),
 #         next_run_time=datetime.datetime.now(),
 #         misfire_grace_time=3600,
 #     )
 #     scheduler.start()
 # else:
-#     log.info('未配置定时器，开启单次任务。')
+#     logger.info('未配置定时器，开启单次任务。')
 #     loop = asyncio.new_event_loop()
 #     asyncio.set_event_loop(loop)
 #     loop.run_until_complete(main())
-#     log.info("任务结束")
+#     logger.info("任务结束")
 
-#     log.info('使用自动守护模式，每隔 24 小时运行一次。')
+#     logger.info('使用自动守护模式，每隔 24 小时运行一次。')
 #     scheduler = BlockingScheduler(timezone='Asia/Shanghai')
 #     scheduler.add_job(
 #         run,
 #         IntervalTrigger(hours=24),
 #         next_run_time=datetime.datetime.now(),
 #         misfire_grace_time=3600,
 #     )
 #     scheduler.start()
 # else:
-#     log.info('未配置定时器，开启单次任务。')
+#     logger.info('未配置定时器，开启单次任务。')
 #     loop = asyncio.new_event_loop()
 #     asyncio.set_event_loop(loop)
 #     loop.run_until_complete(main())
-#     log.info("任务结束")
+#     logger.info("任务结束")
```

### Comparing `nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         data = {
             "access_key": self.u.access_key,
             "actionKey": "appkey",
             "appkey": Crypto.APPKEY,
             "click_time": 1,
             "room_id": room_id,
             "anchor_id": up_id,
-            "uid": up_id,
+            "uid": self_uid,
         }
         self.headers.update(
             {
                 "Content-Type": "application/x-www-form-urlencoded",
             },
         )
         # for _ in range(3):
@@ -422,27 +422,27 @@
             "platform": "android",
             "uuid": self.u.uuids[0],
             "buvid": randomString(37).upper(),
             "seq_id": "1",
             "room_id": f"{room_id}",
             "parent_id": "6",
             "area_id": "283",
-            "timestamp": f"{int(time.time())-60}",
+            "timestamp": f"{int(time.time()) - 60}",
             "secret_key": "axoaadsffcazxksectbbb",
             "watch_time": "60",
             "up_id": f"{up_id}",
             "up_level": "40",
             "jump_from": "30000",
             "gu_id": randomString(43).lower(),
             "play_type": "0",
             "play_url": "",
             "s_time": "0",
             "data_behavior_id": "",
             "data_source_id": "",
-            "up_session": f"l:one:live:record:{room_id}:{int(time.time())-88888}",
+            "up_session": f"l:one:live:record:{room_id}:{int(time.time()) - 88888}",
             "visit_id": randomString(32).lower(),
             "watch_status": "%7B%22pk_id%22%3A0%2C%22screen_status%22%3A1%7D",
             "click_id": self.u.uuids[1],
             "session_id": "",
             "player_type": "0",
             "client_ts": f"{int(time.time())}",
         }
@@ -501,18 +501,18 @@
             "ts": int(time.time()),
         }
         list_msg = await self.__get(
             url,
             params=SingableDict(params).signed,
             headers=self.headers,
         )
-        print(list_msg)
-        list_m = list_msg["list"]
-        for group in list_m:
-            yield group
+        if list_msg:
+            list_m = list_msg["list"]
+            for group in list_m:
+                yield group
 
     async def signInGroups(self, group_id: int, owner_id: int):
         url = "https://api.vc.bilibili.com/link_setting/v1/link_setting/sign_in"
         params = {
             "access_key": self.u.access_key,
             "actionKey": "appkey",
             "appkey": Crypto.APPKEY,
```

### Comparing `nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,23 +106,29 @@
         获取用户勋章
         """
         self.medals.clear()
         self.medalsNeedDo.clear()
         async for medal in self.api.getFansMedalandRoomID():  # type: ignore
             if self.whiteList == [0]:
                 if medal["medal"]["target_id"] in self.bannedList:
-                    log.warning(f"{medal['anchor_info']['nick_name']} 在黑名单中，已过滤")
+                    log.warning(
+                        f"{medal['anchor_info']['nick_name']} 在黑名单中，已过滤"
+                    )
                     continue
                 self.medals.append(medal) if medal["room_info"]["room_id"] != 0 else ...
             else:
                 if medal["medal"]["target_id"] in self.whiteList:
-                    self.medals.append(medal) if medal["room_info"][
-                        "room_id"
-                    ] != 0 else ...
-                    log.success(f"{medal['anchor_info']['nick_name']} 在白名单中，加入任务")
+                    (
+                        self.medals.append(medal)
+                        if medal["room_info"]["room_id"] != 0
+                        else ...
+                    )
+                    log.success(
+                        f"{medal['anchor_info']['nick_name']} 在白名单中，加入任务"
+                    )
         [
             self.medalsNeedDo.append(medal)
             for medal in self.medals
             if medal["medal"]["level"] < 20 and medal["medal"]["today_feed"] < 1500
         ]
 
     async def asynclikeandShare(self, failedMedals: list = []):  # noqa: B006
@@ -138,37 +144,53 @@
         try:
             if not failedMedals:
                 failedMedals = self.medalsNeedDo
             if not self.config["ASYNC"]:
                 log.info("同步点赞、分享任务开始....")
                 for index, medal in enumerate(failedMedals):
                     tasks = []
-                    tasks.append(
-                        self.api.likeInteract(medal["room_info"]["room_id"]),
-                    ) if self.config["LIKE_CD"] else ...
-                    tasks.append(
-                        self.api.shareRoom(medal["room_info"]["room_id"]),
-                    ) if self.config["SHARE_CD"] else ...
+                    (
+                        tasks.append(
+                            self.api.likeInteract(medal["room_info"]["room_id"]),
+                        )
+                        if self.config["LIKE_CD"]
+                        else ...
+                    )
+                    (
+                        tasks.append(
+                            self.api.shareRoom(medal["room_info"]["room_id"]),
+                        )
+                        if self.config["SHARE_CD"]
+                        else ...
+                    )
                     await asyncio.gather(*tasks)
                     log.success(
-                        f"{medal['anchor_info']['nick_name']} 点赞,分享成功 {index+1}/{len(self.medalsNeedDo)}",
+                        f"{medal['anchor_info']['nick_name']} 点赞,分享成功 {index + 1}/{len(self.medalsNeedDo)}",
                     )
                     await asyncio.sleep(
                         max(self.config["LIKE_CD"], self.config["SHARE_CD"]),
                     )
             else:
                 log.info("异步点赞、分享任务开始....")
                 allTasks = []
                 for medal in failedMedals:
-                    allTasks.append(
-                        self.api.likeInteract(medal["room_info"]["room_id"]),
-                    ) if self.config["LIKE_CD"] else ...
-                    allTasks.append(
-                        self.api.shareRoom(medal["room_info"]["room_id"]),
-                    ) if self.config["SHARE_CD"] else ...
+                    (
+                        allTasks.append(
+                            self.api.likeInteract(medal["room_info"]["room_id"]),
+                        )
+                        if self.config["LIKE_CD"]
+                        else ...
+                    )
+                    (
+                        allTasks.append(
+                            self.api.shareRoom(medal["room_info"]["room_id"]),
+                        )
+                        if self.config["SHARE_CD"]
+                        else ...
+                    )
                 await asyncio.gather(*allTasks)
             await asyncio.sleep(10)
             await self.getMedals()  # 刷新勋章
             log.success("点赞、分享任务完成")
             finallyMedals = [
                 medal
                 for medal in self.medalsNeedDo
@@ -197,15 +219,17 @@
             )
             if self.retryTimes > self.maxRetryTimes:
                 log.error("任务重试次数过多,停止任务")
                 return
             if len(finallyMedals) / len(self.medalsNeedDo) <= 0.9:
                 log.warning("成功率过低,重新执行任务")
                 self.retryTimes += 1
-                log.warning("重试次数: {}/{}".format(self.retryTimes, self.maxRetryTimes))
+                log.warning(
+                    "重试次数: {}/{}".format(self.retryTimes, self.maxRetryTimes)
+                )
                 await self.asynclikeandShare(failedMedals)
         except Exception:
             log.exception("点赞、分享任务异常")
             self.errmsg.append(f"【{self.name}】 点赞、分享任务异常,请检查日志")
 
     async def like_v3(self, failedMedals: Optional[list] = None):
         if failedMedals is None:
@@ -216,37 +240,45 @@
         try:
             if not failedMedals:
                 failedMedals = self.medalsNeedDo
             if not self.config["ASYNC"]:
                 log.info("同步点赞任务开始....")
                 for index, medal in enumerate(failedMedals):
                     tasks = []
-                    tasks.append(
-                        self.api.likeInteractV3(
-                            medal["room_info"]["room_id"],
-                            medal["medal"]["target_id"],
-                            self.mid,
-                        ),
-                    ) if self.config["LIKE_CD"] else ...
+                    (
+                        tasks.append(
+                            self.api.likeInteractV3(
+                                medal["room_info"]["room_id"],
+                                medal["medal"]["target_id"],
+                                self.mid,
+                            ),
+                        )
+                        if self.config["LIKE_CD"]
+                        else ...
+                    )
                     await asyncio.gather(*tasks)
                     log.success(
-                        f"{medal['anchor_info']['nick_name']} 点赞成功 {index+1}/{len(self.medalsNeedDo)}",
+                        f"{medal['anchor_info']['nick_name']} 点赞成功 {index + 1}/{len(self.medalsNeedDo)}",
                     )
                     await asyncio.sleep(self.config["LIKE_CD"])
             else:
                 log.info("异步点赞任务开始....")
                 allTasks = []
                 for medal in failedMedals:
-                    allTasks.append(
-                        self.api.likeInteractV3(
-                            medal["room_info"]["room_id"],
-                            medal["medal"]["target_id"],
-                            self.mid,
-                        ),
-                    ) if self.config["LIKE_CD"] else ...
+                    (
+                        allTasks.append(
+                            self.api.likeInteractV3(
+                                medal["room_info"]["room_id"],
+                                medal["medal"]["target_id"],
+                                self.mid,
+                            ),
+                        )
+                        if self.config["LIKE_CD"]
+                        else ...
+                    )
                 await asyncio.gather(*allTasks)
             await asyncio.sleep(10)
             log.success("点赞任务完成")
             finallyMedals = [
                 medal
                 for medal in self.medalsNeedDo
                 if medal["medal"]["today_feed"] >= 100
@@ -271,53 +303,61 @@
             "弹幕打卡任务开始....(预计 {} 秒完成)".format(
                 len(self.medals) * self.config["DANMAKU_CD"],
             ),
         )
         n = 0
         for medal in self.medals:
             try:
-                (await self.api.wearMedal(medal["medal"]["medal_id"])) if self.config[
-                    "WEARMEDAL"
-                ] else ...
+                (
+                    (await self.api.wearMedal(medal["medal"]["medal_id"]))
+                    if self.config["WEARMEDAL"]
+                    else ...
+                )
                 danmaku = await self.api.sendDanmaku(medal["room_info"]["room_id"])
                 n += 1
                 log.success(
                     "{} 房间弹幕打卡成功: {} ({}/{})".format(
                         medal["anchor_info"]["nick_name"],
                         danmaku,
                         n,
                         len(self.medals),
                     ),
                 )
             except Exception as e:
-                log.error("{} 房间弹幕打卡失败: {}".format(medal["anchor_info"]["nick_name"], e))
+                log.error(
+                    "{} 房间弹幕打卡失败: {}".format(
+                        medal["anchor_info"]["nick_name"], e
+                    )
+                )
                 self.errmsg.append(
                     f"【{self.name}】 {medal['anchor_info']['nick_name']} 房间弹幕打卡失败: {e!s}",
                 )
             finally:
                 await asyncio.sleep(self.config["DANMAKU_CD"])
         if hasattr(self, "initialMedal"):
-            (await self.api.wearMedal(self.initialMedal["medal_id"])) if self.config[
-                "WEARMEDAL"
-            ] else ...
+            (
+                (await self.api.wearMedal(self.initialMedal["medal_id"]))
+                if self.config["WEARMEDAL"]
+                else ...
+            )
         log.success("弹幕打卡任务完成")
         self.message.append(f"【{self.name}】 弹幕打卡任务完成 {n}/{len(self.medals)}")
         if n >= 5:
             try:
                 await self.api.getOneBattery()
                 log.success("领取电池成功")
                 self.message.append(f"【{self.name}】 领取电池成功")
             except Exception as e:
                 log.error("领取电池失败: {}".format(e))
                 self.errmsg.append(f"【{self.name}】 领取电池失败: {e!s}")
 
     async def init(self):
         if not await self.loginVerify():
-            log.error("登录失败 可能是 access_key 过期 , 请重新获取")
-            self.errmsg.append("登录失败 可能是 access_key 过期 , 请重新获取")
+            log.error(f"登录失败 可能是 access_key：{self.access_key} 过期 , 请重新获取")
+            self.errmsg.append("登录失败 可能是登录已过期 , 请发送【b站登录】重新登录")
             await self.session.close()
         else:
             await self.doSign()
             await self.getMedals()
 
     async def start(self):
         if self.isLogin:
```

### Comparing `nonebot_plugin_bilifan-0.3.2/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/users.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.2/pyproject.toml` & `nonebot_plugin_bilifan-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.3.2"
+version = "0.3.3"
 description = "刷站粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 repository = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 keywords = ["bilibili", "nonebot2", "plugin"]
@@ -35,22 +35,30 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 89
-target-version = ["py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311","py312"]
 include = '\.pyi?$'
 # skip-string-normalization = true
 
-[tool.ruff.isort]
+[tool.ruff.format]
+docstring-code-format = true
+line-ending = "lf"
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
+detect-same-package = true
 extra-standard-library = ["typing_extensions"]
+split-on-trailing-comma = true
 
-[tool.ruff]
+[tool.ruff.lint]
+preview = true
 ignore = [
     "B008",
     "B905",
     "N803",
     "E402",
     "F601",
     "E501",
```

### Comparing `nonebot_plugin_bilifan-0.3.2/PKG-INFO` & `nonebot_plugin_bilifan-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_bilifan
-Version: 0.3.2
+Version: 0.3.3
 Summary: 刷站粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_bilifan
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_bilifan Version: 0.3.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_bilifan Version: 0.3.3 Summary:
 å·ç«ç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_bilifan License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

