# Comparing `tmp/asyncTwitterClient-0.4.0.tar.gz` & `tmp/asyncTwitterClient-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncTwitterClient-0.4.0.tar", last modified: Thu Apr 25 21:44:49 2024, max compression
+gzip compressed data, was "asyncTwitterClient-0.5.0.tar", last modified: Sun Apr 28 21:44:53 2024, max compression
```

## Comparing `asyncTwitterClient-0.4.0.tar` & `asyncTwitterClient-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 21:44:49.673070 asyncTwitterClient-0.4.0/
--rw-rw-rw-   0        0        0    35149 2023-12-12 23:43:05.000000 asyncTwitterClient-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     2291 2024-04-25 21:44:49.671069 asyncTwitterClient-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1260 2024-04-25 06:04:42.000000 asyncTwitterClient-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 21:44:49.641031 asyncTwitterClient-0.4.0/asyncTwitter/
--rw-rw-rw-   0        0        0        0 2023-11-01 20:45:28.000000 asyncTwitterClient-0.4.0/asyncTwitter/__init__.py
--rw-rw-rw-   0        0        0      185 2024-04-25 20:38:29.000000 asyncTwitterClient-0.4.0/asyncTwitter/__version__.py
--rw-rw-rw-   0        0        0    35054 2023-12-12 23:38:01.000000 asyncTwitterClient-0.4.0/asyncTwitter/account.py
--rw-rw-rw-   0        0        0    39688 2024-04-25 20:34:04.000000 asyncTwitterClient-0.4.0/asyncTwitter/asyncAccount.py
--rw-rw-rw-   0        0        0     8622 2024-04-25 05:00:23.000000 asyncTwitterClient-0.4.0/asyncTwitter/asyncLogin.py
--rw-rw-rw-   0        0        0    39924 2024-04-24 23:41:30.000000 asyncTwitterClient-0.4.0/asyncTwitter/asyncScraper.py
--rw-rw-rw-   0        0        0     8960 2024-04-25 02:06:24.000000 asyncTwitterClient-0.4.0/asyncTwitter/asyncSearch.py
--rw-rw-rw-   0        0        0     8507 2024-04-24 23:41:30.000000 asyncTwitterClient-0.4.0/asyncTwitter/asyncUtil.py
--rw-rw-rw-   0        0        0    33499 2024-04-24 23:41:30.000000 asyncTwitterClient-0.4.0/asyncTwitter/constants.py
--rw-rw-rw-   0        0        0     7022 2023-12-12 23:07:50.000000 asyncTwitterClient-0.4.0/asyncTwitter/login.py
--rw-rw-rw-   0        0        0    34714 2024-04-24 23:41:30.000000 asyncTwitterClient-0.4.0/asyncTwitter/scraper.py
--rw-rw-rw-   0        0        0     6511 2024-04-24 23:43:14.000000 asyncTwitterClient-0.4.0/asyncTwitter/search.py
--rw-rw-rw-   0        0        0     5406 2024-04-25 20:57:34.000000 asyncTwitterClient-0.4.0/asyncTwitter/twoCaptcha.py
--rw-rw-rw-   0        0        0     8440 2023-12-12 23:07:53.000000 asyncTwitterClient-0.4.0/asyncTwitter/util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 21:44:49.670069 asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/
--rw-rw-rw-   0        0        0     2291 2024-04-25 21:44:49.000000 asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2024-04-25 21:44:49.000000 asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 21:44:49.000000 asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-25 21:44:49.000000 asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 21:44:49.000000 asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 21:44:49.673070 asyncTwitterClient-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1268 2024-04-25 21:44:38.000000 asyncTwitterClient-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 21:44:53.331807 asyncTwitterClient-0.5.0/
+-rw-rw-rw-   0        0        0    35149 2023-12-12 23:43:05.000000 asyncTwitterClient-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2475 2024-04-28 21:44:53.330803 asyncTwitterClient-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1441 2024-04-28 20:04:59.000000 asyncTwitterClient-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 21:44:53.322805 asyncTwitterClient-0.5.0/asyncTwitter/
+-rw-rw-rw-   0        0        0        0 2023-11-01 20:45:28.000000 asyncTwitterClient-0.5.0/asyncTwitter/__init__.py
+-rw-rw-rw-   0        0        0      185 2024-04-25 20:38:29.000000 asyncTwitterClient-0.5.0/asyncTwitter/__version__.py
+-rw-rw-rw-   0        0        0    35054 2023-12-12 23:38:01.000000 asyncTwitterClient-0.5.0/asyncTwitter/account.py
+-rw-rw-rw-   0        0        0    43543 2024-04-28 21:44:06.000000 asyncTwitterClient-0.5.0/asyncTwitter/asyncAccount.py
+-rw-rw-rw-   0        0        0     8597 2024-04-28 20:10:34.000000 asyncTwitterClient-0.5.0/asyncTwitter/asyncLogin.py
+-rw-rw-rw-   0        0        0    39924 2024-04-24 23:41:30.000000 asyncTwitterClient-0.5.0/asyncTwitter/asyncScraper.py
+-rw-rw-rw-   0        0        0     8960 2024-04-25 02:06:24.000000 asyncTwitterClient-0.5.0/asyncTwitter/asyncSearch.py
+-rw-rw-rw-   0        0        0     8507 2024-04-24 23:41:30.000000 asyncTwitterClient-0.5.0/asyncTwitter/asyncUtil.py
+-rw-rw-rw-   0        0        0    33499 2024-04-24 23:41:30.000000 asyncTwitterClient-0.5.0/asyncTwitter/constants.py
+-rw-rw-rw-   0        0        0     7022 2023-12-12 23:07:50.000000 asyncTwitterClient-0.5.0/asyncTwitter/login.py
+-rw-rw-rw-   0        0        0    34714 2024-04-24 23:41:30.000000 asyncTwitterClient-0.5.0/asyncTwitter/scraper.py
+-rw-rw-rw-   0        0        0     6511 2024-04-24 23:43:14.000000 asyncTwitterClient-0.5.0/asyncTwitter/search.py
+-rw-rw-rw-   0        0        0     4862 2024-04-28 20:50:03.000000 asyncTwitterClient-0.5.0/asyncTwitter/twoCaptcha.py
+-rw-rw-rw-   0        0        0     8440 2023-12-12 23:07:53.000000 asyncTwitterClient-0.5.0/asyncTwitter/util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 21:44:53.329803 asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/
+-rw-rw-rw-   0        0        0     2475 2024-04-28 21:44:53.000000 asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2024-04-28 21:44:53.000000 asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 21:44:53.000000 asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-28 21:44:53.000000 asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 21:44:53.000000 asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 21:44:53.331807 asyncTwitterClient-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1268 2024-04-28 21:44:24.000000 asyncTwitterClient-0.5.0/setup.py
```

### Comparing `asyncTwitterClient-0.4.0/LICENSE` & `asyncTwitterClient-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/PKG-INFO` & `asyncTwitterClient-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncTwitterClient
-Version: 0.4.0
+Version: 0.5.0
 Summary: A async port of twitter-api-client with extra features
 Home-page: https://github.com/obnoxiousish/async_twitter_api_client
 Author: obnoxious
 Author-email: obnoxious@dongcorp.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -40,21 +40,24 @@
 supports unlocking account via account.unlockViaArkoseCaptcha()
 linted by ruff
 renames tweet and other functions to asyncTweet asyncReply etc
 all functions must be awaited
 uses httpx asyncclient instead of Client so it supports anyio, trio, curio, asyncio
 natively supports proxies, http(s)+socks5
 reply & quote support uploading images
+save_cookies takes toFile arg instead of always making a file and rets a dict
 
 Original search.py uses asyncio.gather(), i switched to use anyio.create_task_group() with a results list that the tasks append to, might not be a 1:1 behaviour
 ```
 
 # Todo
 ```
 Add more captchas providers to solve arkose challenge
+Find a way to provide real ui_metrics for unlocker
+Find a way to use original AsyncClient for unlocker
 Maybe fix searching somehwat?
 Add signup
 ```
```

### Comparing `asyncTwitterClient-0.4.0/README.md` & `asyncTwitterClient-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 supports unlocking account via account.unlockViaArkoseCaptcha()
 linted by ruff
 renames tweet and other functions to asyncTweet asyncReply etc
 all functions must be awaited
 uses httpx asyncclient instead of Client so it supports anyio, trio, curio, asyncio
 natively supports proxies, http(s)+socks5
 reply & quote support uploading images
+save_cookies takes toFile arg instead of always making a file and rets a dict
 
 Original search.py uses asyncio.gather(), i switched to use anyio.create_task_group() with a results list that the tasks append to, might not be a 1:1 behaviour
 ```
 
 # Todo
 ```
 Add more captchas providers to solve arkose challenge
+Find a way to provide real ui_metrics for unlocker
+Find a way to use original AsyncClient for unlocker
 Maybe fix searching somehwat?
 Add signup
 ```
```

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/account.py` & `asyncTwitterClient-0.5.0/asyncTwitter/account.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/asyncAccount.py` & `asyncTwitterClient-0.5.0/asyncTwitter/asyncAccount.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import orjson
 import mimetypes
 import random
 import hashlib
 import time
 import logging
 import math
+import sys
 
 from logging import Logger
 from copy import deepcopy
 from tqdm import tqdm
 from datetime import datetime
 from httpx import AsyncClient, Response
 from .constants import (
@@ -19,109 +20,177 @@
     UPLOAD_CHUNK_SIZE,
     MEDIA_UPLOAD_SUCCEED,
     MEDIA_UPLOAD_FAIL,
     LOG_CONFIG,
     follow_settings,
     follower_notification_settings,
 )
-from .util import get_headers, log, urlencode, find_key, RED, RESET, Path, get_cursor, GREEN
+from .util import (
+    get_headers,
+    log,
+    urlencode,
+    find_key,
+    RED,
+    RESET,
+    Path,
+    get_cursor,
+    GREEN,
+)
 from uuid import uuid1, getnode
 from string import ascii_letters
 from asyncTwitter.twoCaptcha import TwoCaptcha
 
 from .asyncLogin import asyncLogin
+from httpx_socks import AsyncProxyTransport
+from urllib import parse
 
 
 class AsyncAccount:
     def __init__(
         self,
-        *args,
+        save: bool = True,
+        debug: bool = False,
+        twid: bool = False,
+        twoCaptchaApiKey: str = None,
+        proxies: str = None,
+        httpxSocks: bool = False,
         **kwargs,
     ):
-        self.save = kwargs.get("save", True)
-        self.debug = kwargs.get("debug", False)
-        self.twid = kwargs.get("twid", False)
+        """Initailize the AsyncAccount class.
+
+        Args:
+            save (bool, optional): Enable or disable saving files. Defaults to True.
+            debug (bool, optional): Enable or disable debug logging. Defaults to False.
+            twid (bool, optional): Provide the accounts Rest_Id. Defaults to False.
+            twoCaptchaApiKey (str, optional): Provide a TwoCaptcha API key. Defaults to None.
+
+            Do not confuse save with save_cookies. Save is used to save files like images and videos.
+
+            twoCaptchaAPIKey is used to solve captchas for unlocking the account.
+
+            **kwargs: Additional arguments to pass to the logger.
+        """
+        self.save = save
+        self.debug = debug
+        self.twid = twid
         self.gql_api = "https://twitter.com/i/api/graphql"
         self.v1_api = "https://api.twitter.com/1.1"
         self.v2_api = "https://twitter.com/i/api/2"
         self.logger = self._init_logger(**kwargs)
         self.rate_limits = {}
-        self.twoCaptcha = TwoCaptcha(
-            main=self, apiKey=kwargs.get("twoCaptchaApiKey", "")
-        )
+        self.twoCaptcha = TwoCaptcha(main=self, apiKey=twoCaptchaApiKey)
+
+        if httpxSocks:
+            self.transport = AsyncProxyTransport.from_url(proxies)
+            self.proxies = None
+            self.proxyString = proxies
+        else:
+            self.proxies = proxies
+            self.transport = None
+            self.proxyString = proxies
 
         # print(f'AsyncAcc Logger: {self.logger}')
 
     async def unlockViaArkoseCaptcha(self) -> dict:
         """
         This method is used to unlock the account via Arkose Captcha.
+        Provide the TwoCaptcha API key in the constructor/__init__ to use this method.
+
+        This function really needs someone to find a way to find real ui_metrics values.
+        Theyre just static currently, could be getting accounts banned.
+
+        Also needs a way to use the authenticated session instead of copying it,
+        not sure why it wont just werk for me.
         """
 
-        unlockHeaders = {
-            # "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0",
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
-            "Accept-Language": "en-CA,en-US;q=0.7,en;q=0.3",
-            "DNT": "1",
-            "Sec-GPC": "1",
-            "Connection": "keep-alive",
-            "Referer": "https://twitter.com/",
-            "Upgrade-Insecure-Requests": "1",
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "same-origin",
-            "Priority": "u=1",
-            "Pragma": "no-cache",
-            "Cache-Control": "no-cache",
-        }
+        copyOfHeaders = dict(self.session.headers.copy())
+        copyOfHeaders.pop("authorization", None)
+
+        copyOfHeaders["accept"] = (
+            "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8"
+        )
+        copyOfHeaders["referer"] = "https://twitter.com/account/access"
+        copyOfHeaders["content-type"] = "application/x-www-form-urlencoded"
+        # Authorization is removed cuz it causes a 403? Not sure why...
 
-        # new client because it wouldnt work on the self.session idk why
         newClient = AsyncClient(
-            headers=unlockHeaders,
-            cookies=self.session.cookies,
+            headers=copyOfHeaders,
+            cookies=dict(self.session.cookies),
+            transport=self.transport,
             proxies=self.proxies,
             verify=False,
             timeout=30,
             http2=True,
         )
+
+        if self.debug:
+            print(
+                dict(newClient.headers),
+                file=open("newClientHeaders.json", "w", encoding="utf-8"),
+            )
+
         endpointUrl = "https://twitter.com/account/access"
         params = {"lang": "en"}
 
         getRespForData = await newClient.get(endpointUrl, params=params)
 
         authenticityToken = getRespForData.text.split(
             '<input type="hidden" name="authenticity_token" value="'
         )[1].split('"')[0]
         assignmentToken = getRespForData.text.split(
             '<input type="hidden" name="assignment_token" value="'
         )[1].split('"')[0]
 
         if self.debug:
-            self.logger.debug(
+            self.logger.info(
                 f"Authenticity Token Found, getting solved Captcha...: {authenticityToken}"
             )
 
+        if self.proxyString:
+            parsedProxy = parse.urlparse(self.proxyString)
+
+            kwargs = {
+                "proxyType": parsedProxy.scheme,
+                "proxyAddress": parsedProxy.hostname,
+                "proxyPort": parsedProxy.port,
+                "proxyLogin": parsedProxy.username,
+                "proxyPassword": parsedProxy.password,
+                "userAgent": dict(self.session.headers).get(
+                    "user-agent",
+                    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.3",
+                ),
+            }
+        else:
+            kwargs = {
+                "userAgent": dict(self.session.headers).get(
+                    "user-agent",
+                    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.3",
+                ),
+            }
+
         submitCaptchaTask = await self.twoCaptcha.createTask(
             websiteUrl="https://twitter.com/account/access",
             websiteKey="0152B4EB-D2DC-460A-89A1-629838B529C9",
+            **kwargs,
         )
 
         captchaTaskId = submitCaptchaTask.get("taskId")
 
         if self.debug:
             self.logger.debug(f"Captcha Task ID: {captchaTaskId}")
 
         captchaResults = await self.twoCaptcha.checkTaskUntilFinished(
             captchaTaskId, sleepTime=15, maxRetries=20
         )
 
+        solutionToken = captchaResults.get("solution", {}).get("token")
+
         if self.debug:
-            self.logger.debug(f"Captcha Results: {captchaResults}")
+            self.logger.debug(f"Captcha Solution Token: {solutionToken}")
 
-        solutionToken = captchaResults.get("solution", {}).get("token")
-        
         if not solutionToken:
             if self.debug:
                 self.logger.debug("Failed to solve Captcha.")
                 return {"success": False, "error": "Failed to solve Captcha."}
 
         payload = {
             "authenticity_token": authenticityToken,
@@ -129,75 +198,110 @@
             "lang": "en",
             "flow": "",
             "verification_string": solutionToken,  # Captcha solve
             "language_code": "en",
         }
 
         unlockResponse = await newClient.post(
-            endpointUrl, params=params, data=payload, headers=unlockHeaders
+            endpointUrl, params=params, data=payload, follow_redirects=True
         )
-        
-        if 'Your account is now available for use.' in unlockResponse.text:
+
+        if "Your account is now available for use." in unlockResponse.text:
             unlocked = True
         else:
             unlocked = False
 
         if self.debug:
-            self.logger.debug(f"Captcha Unlock: {unlocked} | Checking final stage...")
+            self.logger.debug(
+                f"Captcha Unlock: {unlocked} | Unlock Response status_code: {unlockResponse.status_code}"
+            )
             print(unlockResponse.text, file=open("unlock.html", "w", encoding="utf-8"))
 
         if unlocked:
             authenticityToken = unlockResponse.text.split(
                 '<input type="hidden" name="authenticity_token" value="'
             )[1].split('"')[0]
             assignmentToken = unlockResponse.text.split(
                 '<input type="hidden" name="assignment_token" value="'
             )[1].split('"')[0]
             finishPayload = {
-                'authenticity_token': authenticityToken,
-                'assignment_token': assignmentToken,
-                'lang': 'en',
-                'flow': '',
-                'ui_metrics': '{"rf":{"a164b41fad0433b3eb8ef1474015a1c192606f211d5cab98860739135a6f57d2":-111,"a846abda2338f92a076af6e5f40e8171ddfa1f5f802abc62f1fb39cfd0138301":-1,"ace36e17c04cb2475c443874a57310e469013dbecf948d84137d12b6ad71e025":0,"a25211b004a8e34850978eeb17bab27bca8653a820c1c58442766f317ce2f965":-128},"s":"s0TtDv7i3G_2y2Dx1m-IOiI6st_0zRgRrfYDgKHX7jpHDp0q0bm2Bj7youdKVhxivyJTOpD0t6QrhVGbeUwN3rGreAE2p06HTYtVT_iWDmwdHTmbrOoFM4ws3pNLHb7AGB6ceguzlW8J51qGwY1DrCLFxMFm3_rQ6T0Cu7gp1CsVutURjyEdzecozhS57mEaryVBaxImglAON7SbByk-cOj5FMki6pH3SxFvaOaA3A1Y7CiOU7pQ07KdFhCUcyfM1xkWY3kdH9-lw9sOPBaTrjX15d0L6RTnEcsqtINE8NNZJ5QFaXLNbrlEtSGW29ugUlZphX5Z24iM1-Zn6g6uBgAAAY8W4QwM"}',
+                "authenticity_token": authenticityToken,
+                "assignment_token": assignmentToken,
+                "lang": "en",
+                "flow": "",
+                "ui_metrics": {  # What the fuck is this? Thinking of just making it random
+                    "rf": {
+                        "a164b41fad0433b3eb8ef1474015a1c192606f211d5cab98860739135a6f57d2": -111,
+                        "a846abda2338f92a076af6e5f40e8171ddfa1f5f802abc62f1fb39cfd0138301": -1,
+                        "ace36e17c04cb2475c443874a57310e469013dbecf948d84137d12b6ad71e025": 0,
+                        "a25211b004a8e34850978eeb17bab27bca8653a820c1c58442766f317ce2f965": -128,
+                    },
+                    "s": "s0TtDv7i3G_2y2Dx1m-IOiI6st_0zRgRrfYDgKHX7jpHDp0q0bm2Bj7youdKVhxivyJTOpD0t6QrhVGbeUwN3rGreAE2p06HTYtVT_iWDmwdHTmbrOoFM4ws3pNLHb7AGB6ceguzlW8J51qGwY1DrCLFxMFm3_rQ6T0Cu7gp1CsVutURjyEdzecozhS57mEaryVBaxImglAON7SbByk-cOj5FMki6pH3SxFvaOaA3A1Y7CiOU7pQ07KdFhCUcyfM1xkWY3kdH9-lw9sOPBaTrjX15d0L6RTnEcsqtINE8NNZJ5QFaXLNbrlEtSGW29ugUlZphX5Z24iM1-Zn6g6uBgAAAY8W4QwM",
+                },
             }
-            finishUnlockResp = await newClient.post(endpointUrl, data=finishPayload, follow_redirects=True)
-            
-            if str(finishUnlockResp.url) == "https://twitter.com/?lang=en":
+            finishUnlockResp = await newClient.post(
+                endpointUrl, data=finishPayload, follow_redirects=True
+            )
+
+            if "https://twitter.com/?lang" in str(finishUnlockResp.url):
                 unlocked = True
                 if self.debug:
                     self.logger.debug(f"{GREEN}Account Unlocked Successfully!!!{RESET}")
             else:
                 unlocked = False
                 if self.debug:
                     self.logger.debug(f"{RED}Failed to unlock account.{RESET}")
-                    
 
         return {"success": unlocked}
 
     async def asyncAuthenticate(
         self,
         email: str = None,
         username: str = None,
         password: str = None,
         session: AsyncClient = None,
+        proxies: str = None,
+        httpxSocks: bool = False,
+        cookies: dict = None,
         **kwargs,
-    ):
+    ) -> AsyncClient:
         """
         This is used to authenticate the account.
 
-        This used to be in __init__ but we can't await in __init__ so we have to do it here.
+        If email:username:pass is provided will attempt to login
+        If cookies ct0&auth_token are provided will attempt to validate the session using cookies.
+
+        Args:
+            email (str): Email of the account.
+            username (str): Username of the account.
+            password (str): Password of the account.
+            session (AsyncClient): Session to use.
+            proxies (str): Proxies to use.
+            cookies (dict): Cookies to use.
+            **kwargs: Additional arguments to pass to the logger.
+
+        Returns:
+            AsyncClient: The session authenticated session
         """
 
         self.email = email
         self.username = username
         self.password = password
         self.twitterId = False
         self.twitterRestId = False
-        self.cookies = kwargs.get("cookies")
-        self.proxies = kwargs.get("proxies")
+        self.cookies = cookies
+
+        if httpxSocks:
+            self.transport = AsyncProxyTransport.from_url(proxies)
+            self.proxies = None
+            self.proxyString = proxies
+        else:
+            self.proxies = proxies
+            self.transport = None
+            self.proxyString = proxies
 
         # print(f'AsyncAcc Got: {email}, {username}, {password}, {session}, {self.cookies}, {self.proxies}')
 
         self.session = await self._async_validate_session(
             self.email, self.username, self.password, session, **kwargs
         )
 
@@ -948,26 +1052,30 @@
         addAltTextResponse = await self.session.post(
             url, headers=get_headers(self.session), json=params
         )
         return addAltTextResponse
 
     def _init_logger(self, **kwargs) -> Logger:
         if self.debug:
-            cfg = kwargs.get("log_config")
-            logging.config.dictConfig(cfg or LOG_CONFIG)
+            self.logger = logging.getLogger("asyncTwitter")
+            self.logger.setLevel(logging.DEBUG)  # Set the logging level for this logger
 
-            # only support one logger
-            logger_name = list(LOG_CONFIG["loggers"].keys())[0]
-
-            # set level of all other loggers to ERROR
-            for name in logging.root.manager.loggerDict:
-                if name != logger_name:
-                    logging.getLogger(name).setLevel(logging.ERROR)
+            # Create a StreamHandler that sends log messages to stdout
+            handler = logging.StreamHandler(sys.stdout)
+            handler.setLevel(logging.DEBUG)  # Set the logging level for this handler
+
+            # Create a formatter and add it to the handler
+            formatter = logging.Formatter(
+                "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+            )
+            handler.setFormatter(formatter)
 
-            return logging.getLogger(logger_name)
+            # Add the handler to the logger
+            self.logger.addHandler(handler)
+            return self.logger
 
     def id(self) -> int:
         """Get User ID"""
         if not self.twid:
             potentialTwid = self.session.cookies.get("twid")
 
             if not potentialTwid:
```

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/asyncLogin.py` & `asyncTwitterClient-0.5.0/asyncTwitter/asyncLogin.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,9 +250,9 @@
         http2=True,
         timeout=30,
         verify=False
     )
 
     client = await asyncExecuteLoginFlow(client, **kwargs)
     if not client or client.cookies.get("flow_errors") == "true":
-        raise Exception(f"[{RED}error{RESET}] {BOLD}{username}{RESET} login failed")
+        raise Exception(f"[error] {username} login failed")
     return client
```

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/asyncScraper.py` & `asyncTwitterClient-0.5.0/asyncTwitter/asyncScraper.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/asyncSearch.py` & `asyncTwitterClient-0.5.0/asyncTwitter/asyncSearch.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/asyncUtil.py` & `asyncTwitterClient-0.5.0/asyncTwitter/asyncUtil.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/constants.py` & `asyncTwitterClient-0.5.0/asyncTwitter/constants.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/login.py` & `asyncTwitterClient-0.5.0/asyncTwitter/login.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/scraper.py` & `asyncTwitterClient-0.5.0/asyncTwitter/scraper.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/search.py` & `asyncTwitterClient-0.5.0/asyncTwitter/search.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/twoCaptcha.py` & `asyncTwitterClient-0.5.0/asyncTwitter/twoCaptcha.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
         self.baseUrl = "https://api.2captcha.com"
 
         self.client = AsyncClient(
             http2=False,
             verify=False,
             # proxies=self.main.general.config.get("proxy", 'http://127.0.0.1:8866'),
-            proxies="http://127.0.0.1:8866",
+            #proxies="http://127.0.0.1:8866",
             headers={"Content-Type": "application/json"},
         )
 
     async def checkBalance(self):
         resp = await self.client.post(
             f"{self.baseUrl}/getBalance",
             json={
@@ -72,32 +72,22 @@
         }
 
     async def createTask(
         self,
         websiteUrl: str,
         websiteKey: str,
         method="FunCaptchaTaskProxyless",
-        isInvisible: bool = False,
-        isEnterprise: bool = False,
         cookies: dict = None,
+        **kwargs,
     ):
         taskObject = {
             "type": method,
             "websiteURL": websiteUrl,
             "websitePublicKey": websiteKey,
-            #"isInvisible": isInvisible,
-            #"isEnterprise": isEnterprise,
-            #"userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0",
-            #"apiDomain": "recaptcha.net",
-            #"proxyType": 'socks5',
-            #"proxyAddress": "212.83.142.158",
-            #"proxyPort": "10554",
-            #"pageAction": "login"
-            #"proxyLogin": "user-default_geo-ca_session-RuWtjl6c",
-            #"proxyPassword": "O4A2GhpNjgOw",
+            **kwargs
         }
 
         def convert_cookies_to_string(cookie_dict):
             cookies = [f"{key}={value}" for key, value in cookie_dict.items()]
             return '; '.join(cookies)
         
         if cookies:
```

### Comparing `asyncTwitterClient-0.4.0/asyncTwitter/util.py` & `asyncTwitterClient-0.5.0/asyncTwitter/util.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/PKG-INFO` & `asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncTwitterClient
-Version: 0.4.0
+Version: 0.5.0
 Summary: A async port of twitter-api-client with extra features
 Home-page: https://github.com/obnoxiousish/async_twitter_api_client
 Author: obnoxious
 Author-email: obnoxious@dongcorp.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -40,21 +40,24 @@
 supports unlocking account via account.unlockViaArkoseCaptcha()
 linted by ruff
 renames tweet and other functions to asyncTweet asyncReply etc
 all functions must be awaited
 uses httpx asyncclient instead of Client so it supports anyio, trio, curio, asyncio
 natively supports proxies, http(s)+socks5
 reply & quote support uploading images
+save_cookies takes toFile arg instead of always making a file and rets a dict
 
 Original search.py uses asyncio.gather(), i switched to use anyio.create_task_group() with a results list that the tasks append to, might not be a 1:1 behaviour
 ```
 
 # Todo
 ```
 Add more captchas providers to solve arkose challenge
+Find a way to provide real ui_metrics for unlocker
+Find a way to use original AsyncClient for unlocker
 Maybe fix searching somehwat?
 Add signup
 ```
```

### Comparing `asyncTwitterClient-0.4.0/asyncTwitterClient.egg-info/SOURCES.txt` & `asyncTwitterClient-0.5.0/asyncTwitterClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.4.0/setup.py` & `asyncTwitterClient-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt', 'r', encoding='utf-8') as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name='asyncTwitterClient',
-    version='0.4.0',
+    version='0.5.0',
     author='obnoxious',
     author_email='obnoxious@dongcorp.org',
     description='A async port of twitter-api-client with extra features',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/obnoxiousish/async_twitter_api_client',
     packages=find_packages(),
```

