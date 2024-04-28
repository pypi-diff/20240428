# Comparing `tmp/nonebot-plugin-steam-game-status-0.1.7.tar.gz` & `tmp/nonebot-plugin-steam-game-status-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-steam-game-status-0.1.7.tar", last modified: Wed Feb 28 18:39:53 2024, max compression
+gzip compressed data, was "nonebot-plugin-steam-game-status-0.1.8.tar", last modified: Sun Apr 28 02:44:47 2024, max compression
```

## Comparing `nonebot-plugin-steam-game-status-0.1.7.tar` & `nonebot-plugin-steam-game-status-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-02-28 18:39:41.180110 nonebot-plugin-steam-game-status-0.1.7/LICENSE
--rw-r--r--   0        0        0     4825 2024-02-28 18:39:41.180110 nonebot-plugin-steam-game-status-0.1.7/README.md
--rw-r--r--   0        0        0    19480 2024-02-28 18:39:41.180110 nonebot-plugin-steam-game-status-0.1.7/nonebot_plugin_steam_game_status/__init__.py
--rw-r--r--   0        0        0     1273 2024-02-28 18:39:41.180110 nonebot-plugin-steam-game-status-0.1.7/nonebot_plugin_steam_game_status/config.py
--rw-r--r--   0        0        0     2265 2024-02-28 18:39:41.180110 nonebot-plugin-steam-game-status-0.1.7/nonebot_plugin_steam_game_status/source.py
--rw-r--r--   0        0        0      755 2024-02-28 18:39:41.180110 nonebot-plugin-steam-game-status-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 nonebot-plugin-steam-game-status-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-28 02:44:44.490741 nonebot-plugin-steam-game-status-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4872 2024-04-28 02:44:44.490741 nonebot-plugin-steam-game-status-0.1.8/README.md
+-rw-r--r--   0        0        0    19769 2024-04-28 02:44:44.490741 nonebot-plugin-steam-game-status-0.1.8/nonebot_plugin_steam_game_status/__init__.py
+-rw-r--r--   0        0        0     1273 2024-04-28 02:44:44.490741 nonebot-plugin-steam-game-status-0.1.8/nonebot_plugin_steam_game_status/config.py
+-rw-r--r--   0        0        0     2265 2024-04-28 02:44:44.490741 nonebot-plugin-steam-game-status-0.1.8/nonebot_plugin_steam_game_status/source.py
+-rw-r--r--   0        0        0      755 2024-04-28 02:44:44.490741 nonebot-plugin-steam-game-status-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5274 1970-01-01 00:00:00.000000 nonebot-plugin-steam-game-status-0.1.8/PKG-INFO
```

### Comparing `nonebot-plugin-steam-game-status-0.1.7/LICENSE` & `nonebot-plugin-steam-game-status-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-steam-game-status-0.1.7/README.md` & `nonebot-plugin-steam-game-status-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -139,12 +139,16 @@
 ## 注意事项
 
 1.不支持播报非 Steam 游戏
 
 2.不支持播报 Steam 隐身状态下进行的游戏
 
 ## 更新记录
+2024.04.28
+1. steam列表 合并消息优化
+
+
 2024.02.29
 1. 新增游戏中文名播报，感谢 [6DDUU6](https://github.com/6DDUU6) 的 [PR](https://github.com/nek0us/nonebot_plugin_steam_game_status/pull/18)
 2. 顺应 Nonebot 规范，缓存文件迁移至用户目录下，详见 [plugin-localstore](https://github.com/nonebot/plugin-localstore)
 3. 调整数据结构，节省 key 
 4. 变更原缓存记录从 每次读取文件 更改为 持续在内存中
```

#### html2text {}

```diff
@@ -40,14 +40,14 @@
 åå ä¸ªäººSteamID64æå¥½åä»£ç  | | steamè§£ç»/steamå é¤/steam.del |
 å¦ | ç¾¤è | ç¾¤å | åå ä¸ªäººSteamID64 | | steamåè¡¨/steamç»å®åè¡¨
 | å¦ | ç¾¤è | è¶ç®¡/ç¾¤ç®¡ | ç®¡çåå½ä»¤ | | steamæ­æ¥å¼å¯/
 steamæ­æ¥æå¼ | å¦ | ç¾¤è | è¶ç®¡/ç¾¤ç®¡ | ç®¡çåå½ä»¤ | |
 steamæ­æ¥å³é­/steamæ­æ¥åæ­¢ | å¦ | ç¾¤è | è¶ç®¡/ç¾¤ç®¡ |
 ç®¡çåå½ä»¤ | ## åææ¥æº ç¾¤åç koishi bot çè¯¥æææä»¶ ##
 æ³¨æäºé¡¹ 1.ä¸æ¯ææ­æ¥é Steam æ¸¸æ 2.ä¸æ¯ææ­æ¥ Steam
-éèº«ç¶æä¸è¿è¡çæ¸¸æ ## æ´æ°è®°å½ 2024.02.29 1.
-æ°å¢æ¸¸æä¸­æåæ­æ¥ï¼æè°¢ [6DDUU6](https://github.com/6DDUU6) ç
-[PR](https://github.com/nek0us/nonebot_plugin_steam_game_status/pull/18) 2.
-é¡ºåº Nonebot è§èï¼ç¼å­æä»¶è¿ç§»è³ç¨æ·ç®å½ä¸ï¼è¯¦è§ [plugin-
-localstore](https://github.com/nonebot/plugin-localstore) 3.
-è°æ´æ°æ®ç»æï¼èç key 4. åæ´åç¼å­è®°å½ä» æ¯æ¬¡è¯»åæä»¶
-æ´æ¹ä¸º æç»­å¨åå­ä¸­
+éèº«ç¶æä¸è¿è¡çæ¸¸æ ## æ´æ°è®°å½ 2024.04.28 1. steamåè¡¨
+åå¹¶æ¶æ¯ä¼å 2024.02.29 1. æ°å¢æ¸¸æä¸­æåæ­æ¥ï¼æè°¢ [6DDUU6]
+(https://github.com/6DDUU6) ç [PR](https://github.com/nek0us/
+nonebot_plugin_steam_game_status/pull/18) 2. é¡ºåº Nonebot
+è§èï¼ç¼å­æä»¶è¿ç§»è³ç¨æ·ç®å½ä¸ï¼è¯¦è§ [plugin-localstore]
+(https://github.com/nonebot/plugin-localstore) 3. è°æ´æ°æ®ç»æï¼èç
+key 4. åæ´åç¼å­è®°å½ä» æ¯æ¬¡è¯»åæä»¶ æ´æ¹ä¸º æç»­å¨åå­ä¸­
```

### Comparing `nonebot-plugin-steam-game-status-0.1.7/nonebot_plugin_steam_game_status/__init__.py` & `nonebot-plugin-steam-game-status-0.1.8/nonebot_plugin_steam_game_status/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from nonebot.plugin import PluginMetadata
 from nonebot.exception import MatcherException
 from nonebot import require,get_driver,on_command
 from nonebot_plugin_sendmsg_by_bots import tools
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN,GROUP_OWNER
-from nonebot.adapters.onebot.v11 import Message,MessageEvent,Bot,GroupMessageEvent
+from nonebot.adapters.onebot.v11 import Message,MessageEvent,Bot,GroupMessageEvent,MessageSegment
 
 config_dev = Config.parse_obj(get_driver().config)
 bot_name = list(get_driver().config.nickname)
 if not config_dev.steam_web_key:
     logger.warning("steam_web_key 未配置")
     
 group_list = json.loads(new_file_group.read_text("utf8"))  # noqa: F405
@@ -280,15 +280,20 @@
 steam_bind_list = on_command("steam列表", aliases={"steam绑定列表","steam播报列表","Steam列表","Steam绑定列表","Steam播报列表"}, priority=config_dev.steam_command_priority, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
 @steam_bind_list.handle()
 async def steam_bind_list_handle(bot: Bot, event: MessageEvent):
     if isinstance(event,GroupMessageEvent):
         try:
             msg = []
             for steam_id in group_list[str(event.group_id)]["user_list"]:
-                msg += await node_msg(event.user_id,f"Steam ID：{steam_id}\nName：{steam_list[steam_id][2]}")
+                # msg += await node_msg(event.user_id,f"Steam ID：{steam_id}\nName：{steam_list[steam_id][2]}")
+                msg += MessageSegment.node_custom(
+                    user_id=event.user_id,
+                    nickname=str(index+1),
+                    content=Message(MessageSegment.text(f"Steam ID：{steam_id}\nName：{steam_list[steam_id][2]}"))
+                )
             await bot.send_group_forward_msg(group_id=event.group_id,messages=msg)
         except Exception as e:
             logger.debug(f"Steam 列表合并消息发送出错，错误：{e}")
             await steam_bind_list.finish("本群尚未绑定任何 Steam ID，请先绑定。")
 
 
 steam_on = on_command("steam播报开启", aliases={"steam播报打开","Steam播报开启","Steam播报打开"}, priority=config_dev.steam_command_priority, permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
```

### Comparing `nonebot-plugin-steam-game-status-0.1.7/nonebot_plugin_steam_game_status/config.py` & `nonebot-plugin-steam-game-status-0.1.8/nonebot_plugin_steam_game_status/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-steam-game-status-0.1.7/nonebot_plugin_steam_game_status/source.py` & `nonebot-plugin-steam-game-status-0.1.8/nonebot_plugin_steam_game_status/source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-steam-game-status-0.1.7/pyproject.toml` & `nonebot-plugin-steam-game-status-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-steam-game-status"
-version = "0.1.7"
+version = "0.1.8"
 description = "播报群友 Steam 游戏状态"
 authors = [
     { name = "nek0us", email = "nekouss@mail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-steam-game-status-0.1.7/PKG-INFO` & `nonebot-plugin-steam-game-status-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-steam-game-status
-Version: 0.1.7
+Version: 0.1.8
 Summary: 播报群友 Steam 游戏状态
 License: GPL3
 Author-email: nek0us <nekouss@mail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot_plugin_steam_game_status
 Project-URL: Repository, https://github.com/nek0us/nonebot_plugin_steam_game_status
 Description-Content-Type: text/markdown
@@ -150,12 +150,16 @@
 ## 注意事项
 
 1.不支持播报非 Steam 游戏
 
 2.不支持播报 Steam 隐身状态下进行的游戏
 
 ## 更新记录
+2024.04.28
+1. steam列表 合并消息优化
+
+
 2024.02.29
 1. 新增游戏中文名播报，感谢 [6DDUU6](https://github.com/6DDUU6) 的 [PR](https://github.com/nek0us/nonebot_plugin_steam_game_status/pull/18)
 2. 顺应 Nonebot 规范，缓存文件迁移至用户目录下，详见 [plugin-localstore](https://github.com/nonebot/plugin-localstore)
 3. 调整数据结构，节省 key 
 4. 变更原缓存记录从 每次读取文件 更改为 持续在内存中
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-steam-game-status Version: 0.1.7
+Metadata-Version: 2.1 Name: nonebot-plugin-steam-game-status Version: 0.1.8
 Summary: æ­æ¥ç¾¤å Steam æ¸¸æç¶æ License: GPL3 Author-email: nek0us
 mail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot_plugin_steam_game_status Project-URL: Repository, https://
 github.com/nek0us/nonebot_plugin_steam_game_status Description-Content-Type:
 text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
@@ -46,14 +46,14 @@
 åå ä¸ªäººSteamID64æå¥½åä»£ç  | | steamè§£ç»/steamå é¤/steam.del |
 å¦ | ç¾¤è | ç¾¤å | åå ä¸ªäººSteamID64 | | steamåè¡¨/steamç»å®åè¡¨
 | å¦ | ç¾¤è | è¶ç®¡/ç¾¤ç®¡ | ç®¡çåå½ä»¤ | | steamæ­æ¥å¼å¯/
 steamæ­æ¥æå¼ | å¦ | ç¾¤è | è¶ç®¡/ç¾¤ç®¡ | ç®¡çåå½ä»¤ | |
 steamæ­æ¥å³é­/steamæ­æ¥åæ­¢ | å¦ | ç¾¤è | è¶ç®¡/ç¾¤ç®¡ |
 ç®¡çåå½ä»¤ | ## åææ¥æº ç¾¤åç koishi bot çè¯¥æææä»¶ ##
 æ³¨æäºé¡¹ 1.ä¸æ¯ææ­æ¥é Steam æ¸¸æ 2.ä¸æ¯ææ­æ¥ Steam
-éèº«ç¶æä¸è¿è¡çæ¸¸æ ## æ´æ°è®°å½ 2024.02.29 1.
-æ°å¢æ¸¸æä¸­æåæ­æ¥ï¼æè°¢ [6DDUU6](https://github.com/6DDUU6) ç
-[PR](https://github.com/nek0us/nonebot_plugin_steam_game_status/pull/18) 2.
-é¡ºåº Nonebot è§èï¼ç¼å­æä»¶è¿ç§»è³ç¨æ·ç®å½ä¸ï¼è¯¦è§ [plugin-
-localstore](https://github.com/nonebot/plugin-localstore) 3.
-è°æ´æ°æ®ç»æï¼èç key 4. åæ´åç¼å­è®°å½ä» æ¯æ¬¡è¯»åæä»¶
-æ´æ¹ä¸º æç»­å¨åå­ä¸­
+éèº«ç¶æä¸è¿è¡çæ¸¸æ ## æ´æ°è®°å½ 2024.04.28 1. steamåè¡¨
+åå¹¶æ¶æ¯ä¼å 2024.02.29 1. æ°å¢æ¸¸æä¸­æåæ­æ¥ï¼æè°¢ [6DDUU6]
+(https://github.com/6DDUU6) ç [PR](https://github.com/nek0us/
+nonebot_plugin_steam_game_status/pull/18) 2. é¡ºåº Nonebot
+è§èï¼ç¼å­æä»¶è¿ç§»è³ç¨æ·ç®å½ä¸ï¼è¯¦è§ [plugin-localstore]
+(https://github.com/nonebot/plugin-localstore) 3. è°æ´æ°æ®ç»æï¼èç
+key 4. åæ´åç¼å­è®°å½ä» æ¯æ¬¡è¯»åæä»¶ æ´æ¹ä¸º æç»­å¨åå­ä¸­
```

