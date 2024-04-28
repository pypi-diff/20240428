# Comparing `tmp/nonebot_plugin_simulator_xiuxian-0.5.31.tar.gz` & `tmp/nonebot_plugin_simulator_xiuxian-0.5.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.31.tar", last modified: Thu Apr 25 06:27:19 2024, max compression
+gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.34.tar", last modified: Sun Apr 28 20:00:47 2024, max compression
```

## Comparing `nonebot_plugin_simulator_xiuxian-0.5.31.tar` & `nonebot_plugin_simulator_xiuxian-0.5.34.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 06:27:19.617009 nonebot_plugin_simulator_xiuxian-0.5.31/
--rw-rw-rw-   0        0        0     1089 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.31/LICENSE
--rw-rw-rw-   0        0        0     6851 2024-04-25 06:27:19.617009 nonebot_plugin_simulator_xiuxian-0.5.31/PKG-INFO
--rw-rw-rw-   0        0        0     5846 2024-04-25 06:26:15.000000 nonebot_plugin_simulator_xiuxian-0.5.31/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 06:27:19.602010 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian/
--rw-rw-rw-   0        0        0      381 2024-04-25 01:04:12.000000 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:27:19.616001 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/
--rw-rw-rw-   0        0        0     6851 2024-04-25 06:27:19.000000 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-25 06:27:19.000000 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 06:27:19.000000 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      243 2024-04-25 06:27:19.000000 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-04-25 06:27:19.000000 nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-25 06:27:19.618000 nonebot_plugin_simulator_xiuxian-0.5.31/setup.cfg
--rw-rw-rw-   0        0        0     1407 2024-04-25 06:27:14.000000 nonebot_plugin_simulator_xiuxian-0.5.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:00:47.253222 nonebot_plugin_simulator_xiuxian-0.5.34/
+-rw-rw-rw-   0        0        0     1089 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/LICENSE
+-rw-rw-rw-   0        0        0     6672 2024-04-28 20:00:47.252226 nonebot_plugin_simulator_xiuxian-0.5.34/PKG-INFO
+-rw-rw-rw-   0        0        0     5676 2024-04-27 18:59:32.000000 nonebot_plugin_simulator_xiuxian-0.5.34/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 20:00:47.243206 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/
+-rw-rw-rw-   0        0        0     1352 2024-04-28 19:32:56.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/__init__.py
+-rw-rw-rw-   0        0        0     1960 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/cd_manager.py
+-rw-rw-rw-   0        0        0      361 2024-04-25 00:35:49.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/config.py
+-rw-rw-rw-   0        0        0     2849 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/data_source.py
+-rw-rw-rw-   0        0        0     1787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/exp_util.py
+-rw-rw-rw-   0        0        0     1354 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/help.py
+-rw-rw-rw-   0        0        0     4430 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/item_json.py
+-rw-rw-rw-   0        0        0    50728 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/player_fight.py
+-rw-rw-rw-   0        0        0     8141 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/read_buff.py
+-rw-rw-rw-   0        0        0     8555 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/utils.py
+-rw-rw-rw-   0        0        0    54293 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
+-rw-rw-rw-   0        0        0     5784 2024-04-25 00:26:19.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
+-rw-rw-rw-   0        0        0      787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
+-rw-rw-rw-   0        0        0     2199 2024-04-25 14:18:36.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:00:47.252226 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/
+-rw-rw-rw-   0        0        0     6672 2024-04-28 20:00:47.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      979 2024-04-28 20:00:47.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:00:47.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2024-04-28 20:00:47.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-28 20:00:47.000000 nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-28 20:00:47.254230 nonebot_plugin_simulator_xiuxian-0.5.34/setup.cfg
+-rw-rw-rw-   0        0        0     1374 2024-04-28 20:00:01.000000 nonebot_plugin_simulator_xiuxian-0.5.34/setup.py
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.31/LICENSE` & `nonebot_plugin_simulator_xiuxian-0.5.34/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.31/PKG-INFO` & `nonebot_plugin_simulator_xiuxian-0.5.34/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_simulator_xiuxian
-Version: 0.5.31
+Version: 0.5.34
 Summary: 修仙
 Home-page: https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian
 Author: 甘城菜月
 Author-email: 2859385794@qq.com
 License: MIT license
 Platform: all
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: wget
 Requires-Dist: nonebot_plugin_apscheduler
 Requires-Dist: Pillow==9.5.0
 Requires-Dist: pydantic
 Requires-Dist: wcwidth
 Requires-Dist: ujson
-Requires-Dist: xiuxianxiuxian_base
+Requires-Dist: xiuxian_base
 Requires-Dist: xiuxian_bank
 Requires-Dist: xiuxian_base
 Requires-Dist: xiuxian_boss
 Requires-Dist: xiuxian_buff
 Requires-Dist: xiuxian_info
 Requires-Dist: xiuxian_mixelixir
 Requires-Dist: xiuxian_rift
@@ -52,19 +52,17 @@
 </div>
 
 ## 简介
 
 本插件主要为实现群聊修仙功能,最近经常封号，请自行判断后再使用，已默认转成图片模式，如需关闭，可在config.py处调整img字段为false<br>
 推荐使用[修仙2.0](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2)
 
-## 设定征集中，有好的想法可以推送给群主,只要你敢想群主都能干~~~
-
-
-# 除 git clone 和 zip 下载其余方式需要先下载 data 修仙包<br> xiuxian-main.zip 解压改成 xiuxian 放入 data<br>[[点击下载data修仙包]](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)
+# 设定征集中，有好的想法可以推送给群主,只要你敢想群主都能干~~~
 
+# 启动时会自动下载需要的压缩包到 data <br>需自行解压并命名为 xiuxian 才可正常使用修仙1.0<br>
 
 ## 计划
 
 1、移除认为与修仙无关功能，简化修仙命令。<br>
 2、新功能开发 /完成度-50%。<br>
 
 ## 特色功能
@@ -96,26 +94,30 @@
 ```
 git clone https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian.git
 ```
 
 2、下载数据文件
 
 使用git clone的方法的，进入插件目录，把data文件夹中的全部内容移动到bot的数据文件夹中<br>
-使用pip的，在GitHub处下载data文件夹，把data文件夹中的全部内容移动到bot的数据文件夹中<br>
-bot的数据文件夹一般为bot.py同级目录下的data文件夹
+使用pip，首次启动会在 data 下载压缩包 (xiuxian_XXX.zip) 解压并命名为 xiuxian 重新启动即可使用<br>
+bot的数据文件夹一般为 .env 同级目录下的data文件夹
 
 3、加载插件
 
-- 然后在bot.py文件中添加
+- 然后在pyproject.toml文件中添加
 
 ```
-nonebot.load_plugin('nonebot_plugin_simulator_xiuxian')
+plugins = ['nonebot_plugin_simulator_xiuxian']
 ```
 
-4、如果遇到问题，请先百度和查看下方的 【一些问题】
+4、如果遇到问题
+
+- 当前首次使用，未自动创建json文件及sql文<br>在[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)处下载，目录data -> xiuxian
+处下载的文件，放置于bot目录，data -> xiuxian文件夹处<br>
+- 当为放置为src/plugins目录使用时<br>修改xiuxian目录下__init__.py文件中的42行：src=''中的内容<br>填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
 
 5、如解决不了进交流群：760517008 提问，提问请贴上完整的日志,群里回的快！（疯狂暗示）<br> 
    修仙体验群: 766929439
 
 ## 配置文件
 1、配置文件一般在data/xiuxian文件夹下，自行按照json格式修改即可，一些字段的含义可以进群交流<br>
 2、子插件的配置会在插件运行后在子插件文件中生成config.json文件，该文件字段含义在同级目录的xxxconfig.py有备注。注意：修改配置只需要修改json即可，修改.py文件的话需要删除json文件才会生效，任何修改都需要重启bot。
@@ -139,19 +141,15 @@
 
 - 使用 `我要修仙` 指令触发机器人，机器人创建用户信息，生成灵根，境界等信息。
 - 发送突破，当修为足够时，可突破境界。
 - 发送修仙签到，获取每日初始化的灵石及修为。
 
 ![image](https://user-images.githubusercontent.com/44226600/187607785-3ea934f4-2b5c-418e-9b99-e8a8e5562125.png)
 ![屏幕截图 2024-04-19 033714](https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian/assets/127736993/8519dca7-6a49-409a-a386-0a64e1faa500)
-## 一些问题
 
-- 当前首次使用，未自动创建json文件及sql文件，请在[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)处下载，目录data -> xiuxian
-处下载的文件，放置于bot目录，data -> xiuxian文件夹处
-- 当为放置为plugins目录使用时，请修改xiuxian目录下__init__.py文件中的42行：src=''中的内容，填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
 ## 特别感谢
 
 - [NoneBot2](https://github.com/nonebot/nonebot2)：本插件实装的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
 - [xiuxian](https://github.com/s52047qwas/nonebot_plugin_xiuxian) 原版修仙
 - [xiuxian2](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2) 修仙2
 ## 插件依赖
@@ -166,8 +164,7 @@
 大家喜欢的话可以给这个项目点个star
 
 有bug、意见和建议都欢迎提交 [Issues](https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian/issues) <br>或者联系进入QQ交流群：760517008<br>修仙1.0体验群：766929439<br>(注：提交bug时加上你的地址)<br>修复bug X<br>干掉发现bug的 √<br>
 
 
 ## 许可证
 本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
-
```

#### html2text {}

```diff
@@ -1,34 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.31
+Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.34
 Summary: ä¿®ä» Home-page: https://github.com/luoyefufeng/
 nonebot_plugin_simulator_xiuxian Author: çåèæ Author-email:
 2859385794@qq.com License: MIT license Platform: all Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-Dist:
 nonebot-adapter-onebot Requires-Dist: wget Requires-Dist:
 nonebot_plugin_apscheduler Requires-Dist: Pillow==9.5.0 Requires-Dist: pydantic
-Requires-Dist: wcwidth Requires-Dist: ujson Requires-Dist: xiuxianxiuxian_base
+Requires-Dist: wcwidth Requires-Dist: ujson Requires-Dist: xiuxian_base
 Requires-Dist: xiuxian_bank Requires-Dist: xiuxian_base Requires-Dist:
 xiuxian_boss Requires-Dist: xiuxian_buff Requires-Dist: xiuxian_info Requires-
 Dist: xiuxian_mixelixir Requires-Dist: xiuxian_rift Requires-Dist: xiuxian_sect
 Requires-Dist: xiuxian_work
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»1.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
                             [Python][NoneBot]_[_p_y_p_i_]
 ## ç®ä»
 æ¬æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½,æè¿ç»å¸¸å°å·ï¼è¯·èªè¡å¤æ­ååä½¿ç¨ï¼å·²é»è®¤è½¬æå¾çæ¨¡å¼ï¼å¦éå³é­ï¼å¯å¨config.pyå¤è°æ´imgå­æ®µä¸ºfalse
 æ¨èä½¿ç¨[ä¿®ä»2.0](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2)
-##
+#
 è®¾å®å¾éä¸­ï¼æå¥½çæ³æ³å¯ä»¥æ¨éç»ç¾¤ä¸»,åªè¦ä½ æ¢æ³ç¾¤ä¸»é½è½å¹²~~~
-# é¤ git clone å zip ä¸è½½å¶ä½æ¹å¼éè¦åä¸è½½ data ä¿®ä»å
-xiuxian-main.zip è§£åæ¹æ xiuxian æ¾å¥ data
-[[ç¹å»ä¸è½½dataä¿®ä»å]](https://codeload.github.com/luoyefufeng/xiuxian/
-zip/refs/heads/main) ## è®¡å
-1ãç§»é¤è®¤ä¸ºä¸ä¿®ä»æ å³åè½ï¼ç®åä¿®ä»å½ä»¤ã
+# å¯å¨æ¶ä¼èªå¨ä¸è½½éè¦çåç¼©åå° data
+éèªè¡è§£åå¹¶å½åä¸º xiuxian æå¯æ­£å¸¸ä½¿ç¨ä¿®ä»1.0
+## è®¡å 1ãç§»é¤è®¤ä¸ºä¸ä¿®ä»æ å³åè½ï¼ç®åä¿®ä»å½ä»¤ã
 2ãæ°åè½å¼å /å®æåº¦-50%ã
 ## ç¹è²åè½ æä»¤è¾å¤ï¼å·ä½æ¥çæä»¤ ä¿®ä»å¸®å©
 1ãæ¬èµä»¤ç³»ç»ï¼åéæä»¤ æ¬èµä»¤å¸®å© è·åä¿¡æ¯
 2ãå®é¨ç³»ç»ï¼åéæä»¤ å®é¨å¸®å© è·åä¿¡æ¯
 3ãä¸çbossç³»ç»ï¼åé ä¸çbosså¸®å© è·åä¿¡æ¯
 4ãåå¸ï¼æ¥è¯¢ååºä¿¡æ¯ï¼å½åååä¸ºç¨æ·èªè¡ä¸æ¶æåï¼åéæä»¤
 èåå¸®å© è·åä¿¡æ¯
@@ -42,20 +40,27 @@
 ## å®è£ 1ãä¸è½½æä»¶æä»¶ - ä½¿ç¨èææ¶å®è£
 (æ¨ègithubå¤æåæºç ä½¿ç¨) ``` pip install
 nonebot_plugin_simulator_xiuxian nb plugin install
 nonebot_plugin_simulator_xiuxian ``` - ä½¿ç¨githubå¤æåæºç ä½¿ç¨ ```
 git clone https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian.git
 ``` 2ãä¸è½½æ°æ®æä»¶ ä½¿ç¨git
 cloneçæ¹æ³çï¼è¿å¥æä»¶ç®å½ï¼ædataæä»¶å¤¹ä¸­çå¨é¨åå®¹ç§»å¨å°botçæ°æ®æä»¶å¤¹ä¸­
-ä½¿ç¨pipçï¼å¨GitHubå¤ä¸è½½dataæä»¶å¤¹ï¼ædataæä»¶å¤¹ä¸­çå¨é¨åå®¹ç§»å¨å°botçæ°æ®æä»¶å¤¹ä¸­
-botçæ°æ®æä»¶å¤¹ä¸è¬ä¸ºbot.pyåçº§ç®å½ä¸çdataæä»¶å¤¹
-3ãå è½½æä»¶ - ç¶åå¨bot.pyæä»¶ä¸­æ·»å  ``` nonebot.load_plugin
-('nonebot_plugin_simulator_xiuxian') ```
-4ãå¦æéå°é®é¢ï¼è¯·åç¾åº¦åæ¥çä¸æ¹ç ãä¸äºé®é¢ã
-5ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
+ä½¿ç¨pipï¼é¦æ¬¡å¯å¨ä¼å¨ data ä¸è½½åç¼©å (xiuxian_XXX.zip)
+è§£åå¹¶å½åä¸º xiuxian éæ°å¯å¨å³å¯ä½¿ç¨
+botçæ°æ®æä»¶å¤¹ä¸è¬ä¸º .env åçº§ç®å½ä¸çdataæä»¶å¤¹
+3ãå è½½æä»¶ - ç¶åå¨pyproject.tomlæä»¶ä¸­æ·»å  ``` plugins =
+['nonebot_plugin_simulator_xiuxian'] ``` 4ãå¦æéå°é®é¢ -
+å½åé¦æ¬¡ä½¿ç¨ï¼æªèªå¨åå»ºjsonæä»¶åsqlæ
+å¨[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/
+main)å¤ä¸è½½ï¼ç®å½data -> xiuxian
+å¤ä¸è½½çæä»¶ï¼æ¾ç½®äºbotç®å½ï¼data -> xiuxianæä»¶å¤¹å¤
+- å½ä¸ºæ¾ç½®ä¸ºsrc/pluginsç®å½ä½¿ç¨æ¶
+ä¿®æ¹xiuxianç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹
+å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸ src='src.plugins.'
+å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ 5ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
 æé®ï¼æé®è¯·è´´ä¸å®æ´çæ¥å¿,ç¾¤éåçå¿«ï¼ï¼ç¯çæç¤ºï¼
 ä¿®ä»ä½éªç¾¤: 766929439 ## éç½®æä»¶ 1ãéç½®æä»¶ä¸è¬å¨data/
 xiuxianæä»¶å¤¹ä¸ï¼èªè¡æç§jsonæ ¼å¼ä¿®æ¹å³å¯ï¼ä¸äºå­æ®µçå«ä¹å¯ä»¥è¿ç¾¤äº¤æµ
 2ãå­æä»¶çéç½®ä¼å¨æä»¶è¿è¡åå¨å­æä»¶æä»¶ä¸­çæconfig.jsonæä»¶ï¼è¯¥æä»¶å­æ®µå«ä¹å¨åçº§ç®å½çxxxconfig.pyæå¤æ³¨ãæ³¨æï¼ä¿®æ¹éç½®åªéè¦ä¿®æ¹jsonå³å¯ï¼ä¿®æ¹.pyæä»¶çè¯éè¦å é¤jsonæä»¶æä¼çæï¼ä»»ä½ä¿®æ¹é½éè¦éå¯botã
 ## æ´æ° - ä½¿ç¨èææ¶å®è£ç ``` pip install
 nonebot_plugin_simulator_xiuxian -U ``` ``` pip install
 nonebot_plugin_simulator_xiuxian --upgrade ``` -
@@ -63,27 +68,20 @@
 pull ``` ## åè½å±ç¤º - ä½¿ç¨ `æè¦ä¿®ä»`
 æä»¤è§¦åæºå¨äººï¼æºå¨äººåå»ºç¨æ·ä¿¡æ¯ï¼çæçµæ ¹ï¼å¢çç­ä¿¡æ¯ã
 - åéçªç ´ï¼å½ä¿®ä¸ºè¶³å¤æ¶ï¼å¯çªç ´å¢çã -
 åéä¿®ä»ç­¾å°ï¼è·åæ¯æ¥åå§åççµç³åä¿®ä¸ºã ![image](https:
 //user-images.githubusercontent.com/44226600/187607785-3ea934f4-2b5c-418e-9b99-
 e8a8e5562125.png) ![å±å¹æªå¾ 2024-04-19 033714](https://github.com/
 luoyefufeng/nonebot_plugin_simulator_xiuxian/assets/127736993/8519dca7-6a49-
-409a-a386-0a64e1faa500) ## ä¸äºé®é¢ -
-å½åé¦æ¬¡ä½¿ç¨ï¼æªèªå¨åå»ºjsonæä»¶åsqlæä»¶ï¼è¯·å¨[GitHub]
-(https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/
-main)å¤ä¸è½½ï¼ç®å½data -> xiuxian
-å¤ä¸è½½çæä»¶ï¼æ¾ç½®äºbotç®å½ï¼data -> xiuxianæä»¶å¤¹å¤ -
-å½ä¸ºæ¾ç½®ä¸ºpluginsç®å½ä½¿ç¨æ¶ï¼è¯·ä¿®æ¹xiuxianç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹ï¼å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸
-src='src.plugins.' å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ ## ç¹å«æè°¢ -
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ã - [go-cqhttp](https://github.com/
-Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã - [xiuxian](https://
-github.com/s52047qwas/nonebot_plugin_xiuxian) åçä¿®ä» - [xiuxian2](https:/
-/github.com/QingMuCat/nonebot_plugin_xiuxian_2) ä¿®ä»2 ## æä»¶ä¾èµ -
-nonebot2 - nonebot-adapter-onebot - go-cqhttp ## æ¯æ
+409a-a386-0a64e1faa500) ## ç¹å«æè°¢ - [NoneBot2](https://github.com/
+nonebot/nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ã - [go-cqhttp](https://
+github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã - [xiuxian]
+(https://github.com/s52047qwas/nonebot_plugin_xiuxian) åçä¿®ä» -
+[xiuxian2](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2) ä¿®ä»2 ##
+æä»¶ä¾èµ - nonebot2 - nonebot-adapter-onebot - go-cqhttp ## æ¯æ
 å¤§å®¶åæ¬¢çè¯å¯ä»¥ç»è¿ä¸ªé¡¹ç®ç¹ä¸ªstar
 æbugãæè§åå»ºè®®é½æ¬¢è¿æäº¤ [Issues](https://github.com/
 luoyefufeng/nonebot_plugin_simulator_xiuxian/issues)
 æèèç³»è¿å¥QQäº¤æµç¾¤ï¼760517008
 ä¿®ä»1.0ä½éªç¾¤ï¼766929439
 (æ³¨ï¼æäº¤bugæ¶å ä¸ä½ çå°å)
 ä¿®å¤bug X
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.31/README.md` & `nonebot_plugin_simulator_xiuxian-0.5.34/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,17 @@
 </div>
 
 ## 简介
 
 本插件主要为实现群聊修仙功能,最近经常封号，请自行判断后再使用，已默认转成图片模式，如需关闭，可在config.py处调整img字段为false<br>
 推荐使用[修仙2.0](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2)
 
-## 设定征集中，有好的想法可以推送给群主,只要你敢想群主都能干~~~
-
-
-# 除 git clone 和 zip 下载其余方式需要先下载 data 修仙包<br> xiuxian-main.zip 解压改成 xiuxian 放入 data<br>[[点击下载data修仙包]](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)
+# 设定征集中，有好的想法可以推送给群主,只要你敢想群主都能干~~~
 
+# 启动时会自动下载需要的压缩包到 data <br>需自行解压并命名为 xiuxian 才可正常使用修仙1.0<br>
 
 ## 计划
 
 1、移除认为与修仙无关功能，简化修仙命令。<br>
 2、新功能开发 /完成度-50%。<br>
 
 ## 特色功能
@@ -66,26 +64,30 @@
 ```
 git clone https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian.git
 ```
 
 2、下载数据文件
 
 使用git clone的方法的，进入插件目录，把data文件夹中的全部内容移动到bot的数据文件夹中<br>
-使用pip的，在GitHub处下载data文件夹，把data文件夹中的全部内容移动到bot的数据文件夹中<br>
-bot的数据文件夹一般为bot.py同级目录下的data文件夹
+使用pip，首次启动会在 data 下载压缩包 (xiuxian_XXX.zip) 解压并命名为 xiuxian 重新启动即可使用<br>
+bot的数据文件夹一般为 .env 同级目录下的data文件夹
 
 3、加载插件
 
-- 然后在bot.py文件中添加
+- 然后在pyproject.toml文件中添加
 
 ```
-nonebot.load_plugin('nonebot_plugin_simulator_xiuxian')
+plugins = ['nonebot_plugin_simulator_xiuxian']
 ```
 
-4、如果遇到问题，请先百度和查看下方的 【一些问题】
+4、如果遇到问题
+
+- 当前首次使用，未自动创建json文件及sql文<br>在[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)处下载，目录data -> xiuxian
+处下载的文件，放置于bot目录，data -> xiuxian文件夹处<br>
+- 当为放置为src/plugins目录使用时<br>修改xiuxian目录下__init__.py文件中的42行：src=''中的内容<br>填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
 
 5、如解决不了进交流群：760517008 提问，提问请贴上完整的日志,群里回的快！（疯狂暗示）<br> 
    修仙体验群: 766929439
 
 ## 配置文件
 1、配置文件一般在data/xiuxian文件夹下，自行按照json格式修改即可，一些字段的含义可以进群交流<br>
 2、子插件的配置会在插件运行后在子插件文件中生成config.json文件，该文件字段含义在同级目录的xxxconfig.py有备注。注意：修改配置只需要修改json即可，修改.py文件的话需要删除json文件才会生效，任何修改都需要重启bot。
@@ -109,19 +111,15 @@
 
 - 使用 `我要修仙` 指令触发机器人，机器人创建用户信息，生成灵根，境界等信息。
 - 发送突破，当修为足够时，可突破境界。
 - 发送修仙签到，获取每日初始化的灵石及修为。
 
 ![image](https://user-images.githubusercontent.com/44226600/187607785-3ea934f4-2b5c-418e-9b99-e8a8e5562125.png)
 ![屏幕截图 2024-04-19 033714](https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian/assets/127736993/8519dca7-6a49-409a-a386-0a64e1faa500)
-## 一些问题
 
-- 当前首次使用，未自动创建json文件及sql文件，请在[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)处下载，目录data -> xiuxian
-处下载的文件，放置于bot目录，data -> xiuxian文件夹处
-- 当为放置为plugins目录使用时，请修改xiuxian目录下__init__.py文件中的42行：src=''中的内容，填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
 ## 特别感谢
 
 - [NoneBot2](https://github.com/nonebot/nonebot2)：本插件实装的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
 - [xiuxian](https://github.com/s52047qwas/nonebot_plugin_xiuxian) 原版修仙
 - [xiuxian2](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2) 修仙2
 ## 插件依赖
@@ -135,9 +133,8 @@
 
 大家喜欢的话可以给这个项目点个star
 
 有bug、意见和建议都欢迎提交 [Issues](https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian/issues) <br>或者联系进入QQ交流群：760517008<br>修仙1.0体验群：766929439<br>(注：提交bug时加上你的地址)<br>修复bug X<br>干掉发现bug的 √<br>
 
 
 ## 许可证
-本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
-
+本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
```

#### html2text {}

```diff
@@ -2,21 +2,19 @@
                               [NoneBotPluginText]
              # ä¿®ä»1.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
                             [Python][NoneBot]_[_p_y_p_i_]
 ## ç®ä»
 æ¬æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½,æè¿ç»å¸¸å°å·ï¼è¯·èªè¡å¤æ­ååä½¿ç¨ï¼å·²é»è®¤è½¬æå¾çæ¨¡å¼ï¼å¦éå³é­ï¼å¯å¨config.pyå¤è°æ´imgå­æ®µä¸ºfalse
 æ¨èä½¿ç¨[ä¿®ä»2.0](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2)
-##
+#
 è®¾å®å¾éä¸­ï¼æå¥½çæ³æ³å¯ä»¥æ¨éç»ç¾¤ä¸»,åªè¦ä½ æ¢æ³ç¾¤ä¸»é½è½å¹²~~~
-# é¤ git clone å zip ä¸è½½å¶ä½æ¹å¼éè¦åä¸è½½ data ä¿®ä»å
-xiuxian-main.zip è§£åæ¹æ xiuxian æ¾å¥ data
-[[ç¹å»ä¸è½½dataä¿®ä»å]](https://codeload.github.com/luoyefufeng/xiuxian/
-zip/refs/heads/main) ## è®¡å
-1ãç§»é¤è®¤ä¸ºä¸ä¿®ä»æ å³åè½ï¼ç®åä¿®ä»å½ä»¤ã
+# å¯å¨æ¶ä¼èªå¨ä¸è½½éè¦çåç¼©åå° data
+éèªè¡è§£åå¹¶å½åä¸º xiuxian æå¯æ­£å¸¸ä½¿ç¨ä¿®ä»1.0
+## è®¡å 1ãç§»é¤è®¤ä¸ºä¸ä¿®ä»æ å³åè½ï¼ç®åä¿®ä»å½ä»¤ã
 2ãæ°åè½å¼å /å®æåº¦-50%ã
 ## ç¹è²åè½ æä»¤è¾å¤ï¼å·ä½æ¥çæä»¤ ä¿®ä»å¸®å©
 1ãæ¬èµä»¤ç³»ç»ï¼åéæä»¤ æ¬èµä»¤å¸®å© è·åä¿¡æ¯
 2ãå®é¨ç³»ç»ï¼åéæä»¤ å®é¨å¸®å© è·åä¿¡æ¯
 3ãä¸çbossç³»ç»ï¼åé ä¸çbosså¸®å© è·åä¿¡æ¯
 4ãåå¸ï¼æ¥è¯¢ååºä¿¡æ¯ï¼å½åååä¸ºç¨æ·èªè¡ä¸æ¶æåï¼åéæä»¤
 èåå¸®å© è·åä¿¡æ¯
@@ -30,20 +28,27 @@
 ## å®è£ 1ãä¸è½½æä»¶æä»¶ - ä½¿ç¨èææ¶å®è£
 (æ¨ègithubå¤æåæºç ä½¿ç¨) ``` pip install
 nonebot_plugin_simulator_xiuxian nb plugin install
 nonebot_plugin_simulator_xiuxian ``` - ä½¿ç¨githubå¤æåæºç ä½¿ç¨ ```
 git clone https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian.git
 ``` 2ãä¸è½½æ°æ®æä»¶ ä½¿ç¨git
 cloneçæ¹æ³çï¼è¿å¥æä»¶ç®å½ï¼ædataæä»¶å¤¹ä¸­çå¨é¨åå®¹ç§»å¨å°botçæ°æ®æä»¶å¤¹ä¸­
-ä½¿ç¨pipçï¼å¨GitHubå¤ä¸è½½dataæä»¶å¤¹ï¼ædataæä»¶å¤¹ä¸­çå¨é¨åå®¹ç§»å¨å°botçæ°æ®æä»¶å¤¹ä¸­
-botçæ°æ®æä»¶å¤¹ä¸è¬ä¸ºbot.pyåçº§ç®å½ä¸çdataæä»¶å¤¹
-3ãå è½½æä»¶ - ç¶åå¨bot.pyæä»¶ä¸­æ·»å  ``` nonebot.load_plugin
-('nonebot_plugin_simulator_xiuxian') ```
-4ãå¦æéå°é®é¢ï¼è¯·åç¾åº¦åæ¥çä¸æ¹ç ãä¸äºé®é¢ã
-5ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
+ä½¿ç¨pipï¼é¦æ¬¡å¯å¨ä¼å¨ data ä¸è½½åç¼©å (xiuxian_XXX.zip)
+è§£åå¹¶å½åä¸º xiuxian éæ°å¯å¨å³å¯ä½¿ç¨
+botçæ°æ®æä»¶å¤¹ä¸è¬ä¸º .env åçº§ç®å½ä¸çdataæä»¶å¤¹
+3ãå è½½æä»¶ - ç¶åå¨pyproject.tomlæä»¶ä¸­æ·»å  ``` plugins =
+['nonebot_plugin_simulator_xiuxian'] ``` 4ãå¦æéå°é®é¢ -
+å½åé¦æ¬¡ä½¿ç¨ï¼æªèªå¨åå»ºjsonæä»¶åsqlæ
+å¨[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/
+main)å¤ä¸è½½ï¼ç®å½data -> xiuxian
+å¤ä¸è½½çæä»¶ï¼æ¾ç½®äºbotç®å½ï¼data -> xiuxianæä»¶å¤¹å¤
+- å½ä¸ºæ¾ç½®ä¸ºsrc/pluginsç®å½ä½¿ç¨æ¶
+ä¿®æ¹xiuxianç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹
+å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸ src='src.plugins.'
+å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ 5ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
 æé®ï¼æé®è¯·è´´ä¸å®æ´çæ¥å¿,ç¾¤éåçå¿«ï¼ï¼ç¯çæç¤ºï¼
 ä¿®ä»ä½éªç¾¤: 766929439 ## éç½®æä»¶ 1ãéç½®æä»¶ä¸è¬å¨data/
 xiuxianæä»¶å¤¹ä¸ï¼èªè¡æç§jsonæ ¼å¼ä¿®æ¹å³å¯ï¼ä¸äºå­æ®µçå«ä¹å¯ä»¥è¿ç¾¤äº¤æµ
 2ãå­æä»¶çéç½®ä¼å¨æä»¶è¿è¡åå¨å­æä»¶æä»¶ä¸­çæconfig.jsonæä»¶ï¼è¯¥æä»¶å­æ®µå«ä¹å¨åçº§ç®å½çxxxconfig.pyæå¤æ³¨ãæ³¨æï¼ä¿®æ¹éç½®åªéè¦ä¿®æ¹jsonå³å¯ï¼ä¿®æ¹.pyæä»¶çè¯éè¦å é¤jsonæä»¶æä¼çæï¼ä»»ä½ä¿®æ¹é½éè¦éå¯botã
 ## æ´æ° - ä½¿ç¨èææ¶å®è£ç ``` pip install
 nonebot_plugin_simulator_xiuxian -U ``` ``` pip install
 nonebot_plugin_simulator_xiuxian --upgrade ``` -
@@ -51,27 +56,20 @@
 pull ``` ## åè½å±ç¤º - ä½¿ç¨ `æè¦ä¿®ä»`
 æä»¤è§¦åæºå¨äººï¼æºå¨äººåå»ºç¨æ·ä¿¡æ¯ï¼çæçµæ ¹ï¼å¢çç­ä¿¡æ¯ã
 - åéçªç ´ï¼å½ä¿®ä¸ºè¶³å¤æ¶ï¼å¯çªç ´å¢çã -
 åéä¿®ä»ç­¾å°ï¼è·åæ¯æ¥åå§åççµç³åä¿®ä¸ºã ![image](https:
 //user-images.githubusercontent.com/44226600/187607785-3ea934f4-2b5c-418e-9b99-
 e8a8e5562125.png) ![å±å¹æªå¾ 2024-04-19 033714](https://github.com/
 luoyefufeng/nonebot_plugin_simulator_xiuxian/assets/127736993/8519dca7-6a49-
-409a-a386-0a64e1faa500) ## ä¸äºé®é¢ -
-å½åé¦æ¬¡ä½¿ç¨ï¼æªèªå¨åå»ºjsonæä»¶åsqlæä»¶ï¼è¯·å¨[GitHub]
-(https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/
-main)å¤ä¸è½½ï¼ç®å½data -> xiuxian
-å¤ä¸è½½çæä»¶ï¼æ¾ç½®äºbotç®å½ï¼data -> xiuxianæä»¶å¤¹å¤ -
-å½ä¸ºæ¾ç½®ä¸ºpluginsç®å½ä½¿ç¨æ¶ï¼è¯·ä¿®æ¹xiuxianç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹ï¼å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸
-src='src.plugins.' å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ ## ç¹å«æè°¢ -
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ã - [go-cqhttp](https://github.com/
-Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã - [xiuxian](https://
-github.com/s52047qwas/nonebot_plugin_xiuxian) åçä¿®ä» - [xiuxian2](https:/
-/github.com/QingMuCat/nonebot_plugin_xiuxian_2) ä¿®ä»2 ## æä»¶ä¾èµ -
-nonebot2 - nonebot-adapter-onebot - go-cqhttp ## æ¯æ
+409a-a386-0a64e1faa500) ## ç¹å«æè°¢ - [NoneBot2](https://github.com/
+nonebot/nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ã - [go-cqhttp](https://
+github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã - [xiuxian]
+(https://github.com/s52047qwas/nonebot_plugin_xiuxian) åçä¿®ä» -
+[xiuxian2](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2) ä¿®ä»2 ##
+æä»¶ä¾èµ - nonebot2 - nonebot-adapter-onebot - go-cqhttp ## æ¯æ
 å¤§å®¶åæ¬¢çè¯å¯ä»¥ç»è¿ä¸ªé¡¹ç®ç¹ä¸ªstar
 æbugãæè§åå»ºè®®é½æ¬¢è¿æäº¤ [Issues](https://github.com/
 luoyefufeng/nonebot_plugin_simulator_xiuxian/issues)
 æèèç³»è¿å¥QQäº¤æµç¾¤ï¼760517008
 ä¿®ä»1.0ä½éªç¾¤ï¼766929439
 (æ³¨ï¼æäº¤bugæ¶å ä¸ä½ çå°å)
 ä¿®å¤bug X
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.31/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO` & `nonebot_plugin_simulator_xiuxian-0.5.34/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_simulator_xiuxian
-Version: 0.5.31
+Version: 0.5.34
 Summary: 修仙
 Home-page: https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian
 Author: 甘城菜月
 Author-email: 2859385794@qq.com
 License: MIT license
 Platform: all
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: wget
 Requires-Dist: nonebot_plugin_apscheduler
 Requires-Dist: Pillow==9.5.0
 Requires-Dist: pydantic
 Requires-Dist: wcwidth
 Requires-Dist: ujson
-Requires-Dist: xiuxianxiuxian_base
+Requires-Dist: xiuxian_base
 Requires-Dist: xiuxian_bank
 Requires-Dist: xiuxian_base
 Requires-Dist: xiuxian_boss
 Requires-Dist: xiuxian_buff
 Requires-Dist: xiuxian_info
 Requires-Dist: xiuxian_mixelixir
 Requires-Dist: xiuxian_rift
@@ -52,19 +52,17 @@
 </div>
 
 ## 简介
 
 本插件主要为实现群聊修仙功能,最近经常封号，请自行判断后再使用，已默认转成图片模式，如需关闭，可在config.py处调整img字段为false<br>
 推荐使用[修仙2.0](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2)
 
-## 设定征集中，有好的想法可以推送给群主,只要你敢想群主都能干~~~
-
-
-# 除 git clone 和 zip 下载其余方式需要先下载 data 修仙包<br> xiuxian-main.zip 解压改成 xiuxian 放入 data<br>[[点击下载data修仙包]](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)
+# 设定征集中，有好的想法可以推送给群主,只要你敢想群主都能干~~~
 
+# 启动时会自动下载需要的压缩包到 data <br>需自行解压并命名为 xiuxian 才可正常使用修仙1.0<br>
 
 ## 计划
 
 1、移除认为与修仙无关功能，简化修仙命令。<br>
 2、新功能开发 /完成度-50%。<br>
 
 ## 特色功能
@@ -96,26 +94,30 @@
 ```
 git clone https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian.git
 ```
 
 2、下载数据文件
 
 使用git clone的方法的，进入插件目录，把data文件夹中的全部内容移动到bot的数据文件夹中<br>
-使用pip的，在GitHub处下载data文件夹，把data文件夹中的全部内容移动到bot的数据文件夹中<br>
-bot的数据文件夹一般为bot.py同级目录下的data文件夹
+使用pip，首次启动会在 data 下载压缩包 (xiuxian_XXX.zip) 解压并命名为 xiuxian 重新启动即可使用<br>
+bot的数据文件夹一般为 .env 同级目录下的data文件夹
 
 3、加载插件
 
-- 然后在bot.py文件中添加
+- 然后在pyproject.toml文件中添加
 
 ```
-nonebot.load_plugin('nonebot_plugin_simulator_xiuxian')
+plugins = ['nonebot_plugin_simulator_xiuxian']
 ```
 
-4、如果遇到问题，请先百度和查看下方的 【一些问题】
+4、如果遇到问题
+
+- 当前首次使用，未自动创建json文件及sql文<br>在[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)处下载，目录data -> xiuxian
+处下载的文件，放置于bot目录，data -> xiuxian文件夹处<br>
+- 当为放置为src/plugins目录使用时<br>修改xiuxian目录下__init__.py文件中的42行：src=''中的内容<br>填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
 
 5、如解决不了进交流群：760517008 提问，提问请贴上完整的日志,群里回的快！（疯狂暗示）<br> 
    修仙体验群: 766929439
 
 ## 配置文件
 1、配置文件一般在data/xiuxian文件夹下，自行按照json格式修改即可，一些字段的含义可以进群交流<br>
 2、子插件的配置会在插件运行后在子插件文件中生成config.json文件，该文件字段含义在同级目录的xxxconfig.py有备注。注意：修改配置只需要修改json即可，修改.py文件的话需要删除json文件才会生效，任何修改都需要重启bot。
@@ -139,19 +141,15 @@
 
 - 使用 `我要修仙` 指令触发机器人，机器人创建用户信息，生成灵根，境界等信息。
 - 发送突破，当修为足够时，可突破境界。
 - 发送修仙签到，获取每日初始化的灵石及修为。
 
 ![image](https://user-images.githubusercontent.com/44226600/187607785-3ea934f4-2b5c-418e-9b99-e8a8e5562125.png)
 ![屏幕截图 2024-04-19 033714](https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian/assets/127736993/8519dca7-6a49-409a-a386-0a64e1faa500)
-## 一些问题
 
-- 当前首次使用，未自动创建json文件及sql文件，请在[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main)处下载，目录data -> xiuxian
-处下载的文件，放置于bot目录，data -> xiuxian文件夹处
-- 当为放置为plugins目录使用时，请修改xiuxian目录下__init__.py文件中的42行：src=''中的内容，填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
 ## 特别感谢
 
 - [NoneBot2](https://github.com/nonebot/nonebot2)：本插件实装的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
 - [xiuxian](https://github.com/s52047qwas/nonebot_plugin_xiuxian) 原版修仙
 - [xiuxian2](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2) 修仙2
 ## 插件依赖
@@ -166,8 +164,7 @@
 大家喜欢的话可以给这个项目点个star
 
 有bug、意见和建议都欢迎提交 [Issues](https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian/issues) <br>或者联系进入QQ交流群：760517008<br>修仙1.0体验群：766929439<br>(注：提交bug时加上你的地址)<br>修复bug X<br>干掉发现bug的 √<br>
 
 
 ## 许可证
 本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
-
```

#### html2text {}

```diff
@@ -1,34 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.31
+Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.34
 Summary: ä¿®ä» Home-page: https://github.com/luoyefufeng/
 nonebot_plugin_simulator_xiuxian Author: çåèæ Author-email:
 2859385794@qq.com License: MIT license Platform: all Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-Dist:
 nonebot-adapter-onebot Requires-Dist: wget Requires-Dist:
 nonebot_plugin_apscheduler Requires-Dist: Pillow==9.5.0 Requires-Dist: pydantic
-Requires-Dist: wcwidth Requires-Dist: ujson Requires-Dist: xiuxianxiuxian_base
+Requires-Dist: wcwidth Requires-Dist: ujson Requires-Dist: xiuxian_base
 Requires-Dist: xiuxian_bank Requires-Dist: xiuxian_base Requires-Dist:
 xiuxian_boss Requires-Dist: xiuxian_buff Requires-Dist: xiuxian_info Requires-
 Dist: xiuxian_mixelixir Requires-Dist: xiuxian_rift Requires-Dist: xiuxian_sect
 Requires-Dist: xiuxian_work
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»1.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
                             [Python][NoneBot]_[_p_y_p_i_]
 ## ç®ä»
 æ¬æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½,æè¿ç»å¸¸å°å·ï¼è¯·èªè¡å¤æ­ååä½¿ç¨ï¼å·²é»è®¤è½¬æå¾çæ¨¡å¼ï¼å¦éå³é­ï¼å¯å¨config.pyå¤è°æ´imgå­æ®µä¸ºfalse
 æ¨èä½¿ç¨[ä¿®ä»2.0](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2)
-##
+#
 è®¾å®å¾éä¸­ï¼æå¥½çæ³æ³å¯ä»¥æ¨éç»ç¾¤ä¸»,åªè¦ä½ æ¢æ³ç¾¤ä¸»é½è½å¹²~~~
-# é¤ git clone å zip ä¸è½½å¶ä½æ¹å¼éè¦åä¸è½½ data ä¿®ä»å
-xiuxian-main.zip è§£åæ¹æ xiuxian æ¾å¥ data
-[[ç¹å»ä¸è½½dataä¿®ä»å]](https://codeload.github.com/luoyefufeng/xiuxian/
-zip/refs/heads/main) ## è®¡å
-1ãç§»é¤è®¤ä¸ºä¸ä¿®ä»æ å³åè½ï¼ç®åä¿®ä»å½ä»¤ã
+# å¯å¨æ¶ä¼èªå¨ä¸è½½éè¦çåç¼©åå° data
+éèªè¡è§£åå¹¶å½åä¸º xiuxian æå¯æ­£å¸¸ä½¿ç¨ä¿®ä»1.0
+## è®¡å 1ãç§»é¤è®¤ä¸ºä¸ä¿®ä»æ å³åè½ï¼ç®åä¿®ä»å½ä»¤ã
 2ãæ°åè½å¼å /å®æåº¦-50%ã
 ## ç¹è²åè½ æä»¤è¾å¤ï¼å·ä½æ¥çæä»¤ ä¿®ä»å¸®å©
 1ãæ¬èµä»¤ç³»ç»ï¼åéæä»¤ æ¬èµä»¤å¸®å© è·åä¿¡æ¯
 2ãå®é¨ç³»ç»ï¼åéæä»¤ å®é¨å¸®å© è·åä¿¡æ¯
 3ãä¸çbossç³»ç»ï¼åé ä¸çbosså¸®å© è·åä¿¡æ¯
 4ãåå¸ï¼æ¥è¯¢ååºä¿¡æ¯ï¼å½åååä¸ºç¨æ·èªè¡ä¸æ¶æåï¼åéæä»¤
 èåå¸®å© è·åä¿¡æ¯
@@ -42,20 +40,27 @@
 ## å®è£ 1ãä¸è½½æä»¶æä»¶ - ä½¿ç¨èææ¶å®è£
 (æ¨ègithubå¤æåæºç ä½¿ç¨) ``` pip install
 nonebot_plugin_simulator_xiuxian nb plugin install
 nonebot_plugin_simulator_xiuxian ``` - ä½¿ç¨githubå¤æåæºç ä½¿ç¨ ```
 git clone https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian.git
 ``` 2ãä¸è½½æ°æ®æä»¶ ä½¿ç¨git
 cloneçæ¹æ³çï¼è¿å¥æä»¶ç®å½ï¼ædataæä»¶å¤¹ä¸­çå¨é¨åå®¹ç§»å¨å°botçæ°æ®æä»¶å¤¹ä¸­
-ä½¿ç¨pipçï¼å¨GitHubå¤ä¸è½½dataæä»¶å¤¹ï¼ædataæä»¶å¤¹ä¸­çå¨é¨åå®¹ç§»å¨å°botçæ°æ®æä»¶å¤¹ä¸­
-botçæ°æ®æä»¶å¤¹ä¸è¬ä¸ºbot.pyåçº§ç®å½ä¸çdataæä»¶å¤¹
-3ãå è½½æä»¶ - ç¶åå¨bot.pyæä»¶ä¸­æ·»å  ``` nonebot.load_plugin
-('nonebot_plugin_simulator_xiuxian') ```
-4ãå¦æéå°é®é¢ï¼è¯·åç¾åº¦åæ¥çä¸æ¹ç ãä¸äºé®é¢ã
-5ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
+ä½¿ç¨pipï¼é¦æ¬¡å¯å¨ä¼å¨ data ä¸è½½åç¼©å (xiuxian_XXX.zip)
+è§£åå¹¶å½åä¸º xiuxian éæ°å¯å¨å³å¯ä½¿ç¨
+botçæ°æ®æä»¶å¤¹ä¸è¬ä¸º .env åçº§ç®å½ä¸çdataæä»¶å¤¹
+3ãå è½½æä»¶ - ç¶åå¨pyproject.tomlæä»¶ä¸­æ·»å  ``` plugins =
+['nonebot_plugin_simulator_xiuxian'] ``` 4ãå¦æéå°é®é¢ -
+å½åé¦æ¬¡ä½¿ç¨ï¼æªèªå¨åå»ºjsonæä»¶åsqlæ
+å¨[GitHub](https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/
+main)å¤ä¸è½½ï¼ç®å½data -> xiuxian
+å¤ä¸è½½çæä»¶ï¼æ¾ç½®äºbotç®å½ï¼data -> xiuxianæä»¶å¤¹å¤
+- å½ä¸ºæ¾ç½®ä¸ºsrc/pluginsç®å½ä½¿ç¨æ¶
+ä¿®æ¹xiuxianç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹
+å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸ src='src.plugins.'
+å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ 5ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
 æé®ï¼æé®è¯·è´´ä¸å®æ´çæ¥å¿,ç¾¤éåçå¿«ï¼ï¼ç¯çæç¤ºï¼
 ä¿®ä»ä½éªç¾¤: 766929439 ## éç½®æä»¶ 1ãéç½®æä»¶ä¸è¬å¨data/
 xiuxianæä»¶å¤¹ä¸ï¼èªè¡æç§jsonæ ¼å¼ä¿®æ¹å³å¯ï¼ä¸äºå­æ®µçå«ä¹å¯ä»¥è¿ç¾¤äº¤æµ
 2ãå­æä»¶çéç½®ä¼å¨æä»¶è¿è¡åå¨å­æä»¶æä»¶ä¸­çæconfig.jsonæä»¶ï¼è¯¥æä»¶å­æ®µå«ä¹å¨åçº§ç®å½çxxxconfig.pyæå¤æ³¨ãæ³¨æï¼ä¿®æ¹éç½®åªéè¦ä¿®æ¹jsonå³å¯ï¼ä¿®æ¹.pyæä»¶çè¯éè¦å é¤jsonæä»¶æä¼çæï¼ä»»ä½ä¿®æ¹é½éè¦éå¯botã
 ## æ´æ° - ä½¿ç¨èææ¶å®è£ç ``` pip install
 nonebot_plugin_simulator_xiuxian -U ``` ``` pip install
 nonebot_plugin_simulator_xiuxian --upgrade ``` -
@@ -63,27 +68,20 @@
 pull ``` ## åè½å±ç¤º - ä½¿ç¨ `æè¦ä¿®ä»`
 æä»¤è§¦åæºå¨äººï¼æºå¨äººåå»ºç¨æ·ä¿¡æ¯ï¼çæçµæ ¹ï¼å¢çç­ä¿¡æ¯ã
 - åéçªç ´ï¼å½ä¿®ä¸ºè¶³å¤æ¶ï¼å¯çªç ´å¢çã -
 åéä¿®ä»ç­¾å°ï¼è·åæ¯æ¥åå§åççµç³åä¿®ä¸ºã ![image](https:
 //user-images.githubusercontent.com/44226600/187607785-3ea934f4-2b5c-418e-9b99-
 e8a8e5562125.png) ![å±å¹æªå¾ 2024-04-19 033714](https://github.com/
 luoyefufeng/nonebot_plugin_simulator_xiuxian/assets/127736993/8519dca7-6a49-
-409a-a386-0a64e1faa500) ## ä¸äºé®é¢ -
-å½åé¦æ¬¡ä½¿ç¨ï¼æªèªå¨åå»ºjsonæä»¶åsqlæä»¶ï¼è¯·å¨[GitHub]
-(https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/
-main)å¤ä¸è½½ï¼ç®å½data -> xiuxian
-å¤ä¸è½½çæä»¶ï¼æ¾ç½®äºbotç®å½ï¼data -> xiuxianæä»¶å¤¹å¤ -
-å½ä¸ºæ¾ç½®ä¸ºpluginsç®å½ä½¿ç¨æ¶ï¼è¯·ä¿®æ¹xiuxianç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹ï¼å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸
-src='src.plugins.' å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ ## ç¹å«æè°¢ -
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ã - [go-cqhttp](https://github.com/
-Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã - [xiuxian](https://
-github.com/s52047qwas/nonebot_plugin_xiuxian) åçä¿®ä» - [xiuxian2](https:/
-/github.com/QingMuCat/nonebot_plugin_xiuxian_2) ä¿®ä»2 ## æä»¶ä¾èµ -
-nonebot2 - nonebot-adapter-onebot - go-cqhttp ## æ¯æ
+409a-a386-0a64e1faa500) ## ç¹å«æè°¢ - [NoneBot2](https://github.com/
+nonebot/nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ã - [go-cqhttp](https://
+github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã - [xiuxian]
+(https://github.com/s52047qwas/nonebot_plugin_xiuxian) åçä¿®ä» -
+[xiuxian2](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2) ä¿®ä»2 ##
+æä»¶ä¾èµ - nonebot2 - nonebot-adapter-onebot - go-cqhttp ## æ¯æ
 å¤§å®¶åæ¬¢çè¯å¯ä»¥ç»è¿ä¸ªé¡¹ç®ç¹ä¸ªstar
 æbugãæè§åå»ºè®®é½æ¬¢è¿æäº¤ [Issues](https://github.com/
 luoyefufeng/nonebot_plugin_simulator_xiuxian/issues)
 æèèç³»è¿å¥QQäº¤æµç¾¤ï¼760517008
 ä¿®ä»1.0ä½éªç¾¤ï¼766929439
 (æ³¨ï¼æäº¤bugæ¶å ä¸ä½ çå°å)
 ä¿®å¤bug X
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.31/setup.py` & `nonebot_plugin_simulator_xiuxian-0.5.34/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_namespace_packages,find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='nonebot_plugin_simulator_xiuxian',
-    version='0.5.31',
+    version='0.5.34',
     description='修仙',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='甘城菜月',
     author_email='2859385794@qq.com',
     license='MIT license',
     include_package_data=True,
@@ -17,15 +17,14 @@
                       "nonebot-adapter-onebot",
                       'wget',
                       "nonebot_plugin_apscheduler",
                       "Pillow==9.5.0",
                       "pydantic",
                       "wcwidth",
                       "ujson",
-                      "xiuxian"
                       "xiuxian_base",
                       "xiuxian_bank",
                       "xiuxian_base",
                       "xiuxian_boss",
                       "xiuxian_buff",
                       "xiuxian_info",
                       "xiuxian_mixelixir",
```

