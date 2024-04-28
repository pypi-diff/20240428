# Comparing `tmp/misspy-2023.9.17rc1.tar.gz` & `tmp/misspy-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misspy-2023.9.17rc1.tar", max compression
+gzip compressed data, was "misspy-2024.4.0.tar", max compression
```

## Comparing `misspy-2023.9.17rc1.tar` & `misspy-2024.4.0.tar`

### file list

```diff
@@ -1,22 +1,39 @@
--rw-r--r--   0        0        0     1065 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/LICENSE
--rw-r--r--   0        0        0     2501 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/README.md
--rw-r--r--   0        0        0      218 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/__init__.py
--rw-r--r--   0        0        0     2453 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/auth.py
--rw-r--r--   0        0        0    39841 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/client.py
--rw-r--r--   0        0        0      794 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/exception.py
--rw-r--r--   0        0        0     1865 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/ext/MiAuth.py
--rw-r--r--   0        0        0       27 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/ext/admin/__init__.py
--rw-r--r--   0        0        0     2343 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/ext/admin/ad.py
--rw-r--r--   0        0        0     1351 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/ext/admin/admin.py
--rw-r--r--   0        0        0     1242 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/ext/admin/raw.txt
--rw-r--r--   0        0        0      916 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/hook.py
--rw-r--r--   0        0        0     3709 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/http.py
--rw-r--r--   0        0        0      875 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/log.py
--rw-r--r--   0        0        0      369 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/not_recommended.py
--rw-r--r--   0        0        0    11224 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/notes.py
--rw-r--r--   0        0        0      861 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/reaction.py
--rw-r--r--   0        0        0      347 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/types.py
--rw-r--r--   0        0        0      349 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/misspy/util.py
--rw-r--r--   0        0        0      845 2023-09-30 10:54:49.324373 misspy-2023.9.17rc1/pyproject.toml
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 misspy-2023.9.17rc1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 10:55:32.351343 misspy-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     2821 2024-04-04 10:55:32.355343 misspy-2024.4.0/README.md
+-rw-r--r--   0        0        0     1075 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/MiWeb.py
+-rw-r--r--   0        0        0      432 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/__init__.py
+-rw-r--r--   0        0        0     2285 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/auth.py
+-rw-r--r--   0        0        0     2515 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/channels.py
+-rw-r--r--   0        0        0     3456 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/client.py
+-rw-r--r--   0        0        0     1385 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/clips.py
+-rw-r--r--   0        0        0       35 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/core/__init__.py
+-rw-r--r--   0        0        0      887 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/core/exception.py
+-rw-r--r--   0        0        0     3277 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/core/http.py
+-rw-r--r--   0        0        0     4265 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/core/ws.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/data.py
+-rw-r--r--   0        0        0     5969 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/drive.py
+-rw-r--r--   0        0        0     1783 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/MiAuth.py
+-rw-r--r--   0        0        0       27 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/admin/__init__.py
+-rw-r--r--   0        0        0     2343 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/admin/ad.py
+-rw-r--r--   0        0        0     1351 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/admin/admin.py
+-rw-r--r--   0        0        0     1242 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/admin/raw.txt
+-rw-r--r--   0        0        0       20 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/commands/__init__.py
+-rw-r--r--   0        0        0     3364 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/commands/bot.py
+-rw-r--r--   0        0        0      949 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/commands/hook.py
+-rw-r--r--   0        0        0     8159 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/ext/commands/ws.py
+-rw-r--r--   0        0        0     2748 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/federation.py
+-rw-r--r--   0        0        0     1890 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/hashtags.py
+-rw-r--r--   0        0        0      916 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/hook.py
+-rw-r--r--   0        0        0      875 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/log.py
+-rw-r--r--   0        0        0      369 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/not_recommended.py
+-rw-r--r--   0        0        0    21008 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/notes.py
+-rw-r--r--   0        0        0     1544 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/pages.py
+-rw-r--r--   0        0        0     4619 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/permissions.py
+-rw-r--r--   0        0        0     1527 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/reaction.py
+-rw-r--r--   0        0        0     1325 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/server.py
+-rw-r--r--   0        0        0     7095 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/types.py
+-rw-r--r--   0        0        0    15798 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/user.py
+-rw-r--r--   0        0        0      476 2024-04-04 10:55:32.355343 misspy-2024.4.0/misspy/util.py
+-rw-r--r--   0        0        0     2222 2024-04-04 10:55:32.355343 misspy-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 misspy-2024.4.0/PKG-INFO
```

### Comparing `misspy-2023.9.17rc1/LICENSE` & `misspy-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `misspy-2023.9.17rc1/README.md` & `misspy-2024.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,80 @@
 # misspy
-![Supported Python Version](https://img.shields.io/pypi/pyversions/misspy) [![PyPI version](https://badge.fury.io/py/misspy.svg)](https://badge.fury.io/py/misspy) [![PyPI Downloads](https://img.shields.io/pypi/dm/misspy.svg)](https://badge.fury.io/py/misspy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=sonyakun_misspy&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=sonyakun_misspy) [![Upload Python Package](https://github.com/sonyakun/misspy/actions/workflows/main.yml/badge.svg)](https://github.com/sonyakun/misspy/actions/workflows/main.yml)
+![Supported Python Version](https://img.shields.io/pypi/pyversions/misspy?style=flat-square) [![PyPI version](https://badge.fury.io/py/misspy.svg?style=flat-square)](https://badge.fury.io/py/misspy) [![PyPI Downloads](https://img.shields.io/pypi/dm/misspy.svg?style=flat-square)](https://badge.fury.io/py/misspy) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black) 
+[![Misskey-API](https://img.shields.io/badge/Misskey-555555.svg?logo=Misskey&style=flat-square)](https://misskey-hub.net)
 
 Misskey API library for Python with StreamingAPI support.
 
 # supported software
 Misskey forks not listed below are supported only in the latest version **__provided they are API compatible__**.
 * [misskey](https://github.com/misskey-dev/misskey)
 * [misskey (misskey.io)](https://github.com/misskeyIO/misskey)
-* [firefish (calckey)](https://codeberg.org/firefish/firefish) (Some APIs may not be compatible with some APIs due to missing documentation regarding firefish API specifications.)
-
-
-## supported misskey versions
-This library is developed based on the API specification for Misskey v13 or later, so v12 and earlier are not supported (but you may still be able to use this library).
-
+* ~~[firefish (calckey)](https://codeberg.org/firefish/firefish) (Some APIs may not be compatible with some APIs due to missing documentation regarding firefish API specifications.)~~
 
 # example
 **Other examples can be found in the examples directory.**
 
 ## send note
 ```python
 import misspy
 
 mi = misspy.Bot(address, i=token)
 ```
 
 ## Output notes text to the console
 ```python
 import misspy
-from misspy.ext import MiAuth
-from misspy.hook import hook
 
-bot = misspy.Bot("misskey.io", i=token)
+bot = commands.Bot("misskey.example", "token")
 
 async def on_ready():
-    bot.connect("localTimeline")
-    print("running")
+    print("loggedin: ")
+    print("id: "+ bot.id)
+    print("name: "+ bot.name)
+    print("username: "+ bot.username)
+    await bot.connect(misspy.localTimeline) # supported args: misspy.homeTimeline, misspy.localTimeline, misspy.socialTimeline or misspy.hybridTimeline, misspy.globalTimeline and Conventional Method
+
 
-async def on_note(message):
+async def on_note(ctx, message):
+    if message["text"] == "test":
+        await ctx.add_reaction(":test:")
     print("------------")
-    print(message.text)
+    print(message)
     print("------------")
 
+bot.add_hook("ready", on_ready)
+bot.add_hook("note", on_note)
 
-hook.add("note", on_note)
-hook.add("ready", on_ready)
 bot.run()
 ```
 
 ## MiAuth
 ```python
-from misspy.ext import MiAuth
+from misspy import MiAuth
 
 mia = MiAuth("misskey.io")
 print(mia.generate_url("example app"))
 while True:
     input("enter to continue...")
     try:
         token = mia.check()
         break
     except misspy.MiAuthFailed:
         pass
 print(token)
 ```
 
+# Other
 
-# docs
-Document is Multi-Language supported. (English, 日本語)
-
+## docs
 Documentation can be found at:
-https://misspy.sonyakun.com/docs
+https://docs.misspy.xyz/
+
+## supported python version
+|                          | below 3.7 | 3.8 ~ 3.11          | 3.12             | 
+| ------------------------ | --------- | ------------------- | ---------------- | 
+| supported                | ❌        | ⭕                  | ⭕        | 
+| supported misspy version | ❌        | 2023.8.24rc1~latest | latest | 
+
+## supported misskey versions
+This library is developed based on the API specification for Misskey v13 or later, so v12 and earlier are not supported (but you may still be able to use this library).
```

### Comparing `misspy-2023.9.17rc1/misspy/exception.py` & `misspy-2024.4.0/misspy/core/exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
     pass
 
 
 class ClientException(MisskeyException):
     """Parent class of error classes such as login failure."""
 
+class RateLimitError(ClientException):
+    """RateLimitError trigger: RATE_LIMIT_EXCEEDED"""
 
 class AuthenticationFailed(ClientException):
     """Class called if MisskeyAPI authentication fails."""
 
 
 class MiAuthFailed(AuthenticationFailed):
     """Class called if MiAuth fails."""
```

### Comparing `misspy-2023.9.17rc1/misspy/ext/admin/ad.py` & `misspy-2024.4.0/misspy/ext/admin/ad.py`

 * *Files identical despite different names*

### Comparing `misspy-2023.9.17rc1/misspy/ext/admin/admin.py` & `misspy-2024.4.0/misspy/ext/admin/admin.py`

 * *Files identical despite different names*

### Comparing `misspy-2023.9.17rc1/misspy/ext/admin/raw.txt` & `misspy-2024.4.0/misspy/ext/admin/raw.txt`

 * *Files identical despite different names*

### Comparing `misspy-2023.9.17rc1/misspy/hook.py` & `misspy-2024.4.0/misspy/hook.py`

 * *Files identical despite different names*

### Comparing `misspy-2023.9.17rc1/misspy/http.py` & `misspy-2024.4.0/misspy/core/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,123 +1,111 @@
-import json
 import requests
 
 import aiohttp
 import httpx
 
-from .exception import HTTPException, ClientException
+try:
+    import orjson as json
+except ModuleNotFoundError:
+    import json
+
+from misspy.core.exception import HTTPException, ClientException, RateLimitError
+
+h_t = {"Content-Type": "application/json"}
 
 
 def request_sync(
     address,
     i=None,
     endpoint="test",
     jobj: dict = {"required": True},
-    header: dict = {"Content-Type": "application/json"},
-    ssl: bool=True
+    header: dict = h_t,
+    ssl: bool = True,
 ):
     """request_sync (internal function)
 
     Args:
         address (string): instance address
         i (string): user token
         endpoint (string): endpoint (example: notes/create)
-        jobj (dict): request params. Do not include the i.
+        jobj (dict): request params. Do not include the i. Defaults to {"Content-Type": "application/json"}.
         header (dict, optional): request header. Defaults to {"Content-Type": "application/json"}.
 
     Returns:
         dict: request result
     """
     url = address + "/api/" + endpoint
     if i is not None:
         jobj["i"] = i
-    res = requests.post(url, data=json.dumps(jobj, ensure_ascii=False), headers=header, verify=ssl)
+    res = requests.post(
+        url, data=json.dumps(jobj, ensure_ascii=False), headers=header, verify=ssl
+    )
     try:
         return res.json()
-    except:
+    except Exception as e:
         return True
 
 
 async def request(
     address,
     i=None,
-    endpoint="test",
-    jobj: dict = {"required": True},
+    endpoint="ping",
+    jobj: dict = {},
     files=None,
-    header=None,
+    header=h_t,
 ):
     """request (internal function)
 
     Args:
         address (string): instance address
         i (string): user token
         endpoint (string): endpoint (example: notes/create)
         jobj (dict): request params. Do not include the i.
 
     Returns:
         dict: request result
     """
-    async with httpx.AsyncClient() as client:
+    async with aiohttp.ClientSession() as client:
         url = address + "/api/" + endpoint
         if i is not None:
             jobj["i"] = i
         if files is not None:
-            if header is not None:
-                res = await client.post(
-                    url,
-                    data=jobj,
-                    files=files,
-                    headers=header,
-                )
-            else:
-                res = await client.post(url, files=files, data=jobj)
+            async with httpx.AsyncClient() as client:
+                if header is not None:
+                    res = await client.post(
+                        url,
+                        data=jobj,
+                        files=files,
+                        headers=header,
+                    )
+                else:
+                    res = await client.post(url, files=files, data=jobj)
             try:
-                try:
-                    if json.loads(res.text).get("error").get("kind") is not None:
-                        raise ClientException(
-                            res.json()["error"]["message"]
-                            + "\nid: "
-                            + res.json()["error"]["id"]
-                        )
-                    else:
-                        return res.json()
-                except AttributeError:
-                    return json.loads(res.text)
-            except json.decoder.JSONDecodeError:
-                raise HTTPException(res.status_code)
+                resp = res.json()
+            except json.JSONDecodeError:
+                resp = json.loads(res.text)
         else:
             if header is not None:
                 res = await client.post(
                     url, data=json.dumps(jobj, ensure_ascii=False), headers=header
                 )
                 try:
-                    return res.json()
+                    return await res.json()
                 except json.JSONDecodeError:
                     return True
             else:
                 res = await client.post(url, data=json.dumps(jobj, ensure_ascii=False))
-                try:
-                    return res.json()
-                except json.JSONDecodeError:
-                    return True
-
-
-async def request_guest(
-    address, endpoint, jobj: dict, header: dict = {"Content-Type": "application/json"}
-):
-    """request (internal function)
-
-    Args:
-        address (string): instance address
-        endpoint (string): endpoint (example: notes/create)
-        jobj (dict): request params. Do not include the i.
-        header (dict, optional): request header. Defaults to {"Content-Type": "application/json"}.
-
-    Returns:
-        dict: request result
-    """
-    async with aiohttp.ClientSession() as client:
-        res = await client.post(
-            address + "/api/" + endpoint,
-            data=json.dumps(jobj, ensure_ascii=False),
-        )
-        return res.json()
+            try:
+                resp = await res.json()
+            except json.JSONDecodeError:
+                resp = json.loads(await res.text)
+        if resp.get("error").get("kind") is not None:
+            if resp["error"]["code"] == "RATE_LIMIT_EXCEEDED":
+                raise RateLimitError(
+                    "We are being rate limited. Please try again in a few moments."
+                )
+            raise ClientException(
+                resp["error"]["message"] + "\nid: " + resp["error"]["id"]
+            )
+        else:
+            print(type(resp))
+            return resp
```

### Comparing `misspy-2023.9.17rc1/misspy/log.py` & `misspy-2024.4.0/misspy/log.py`

 * *Files identical despite different names*

### Comparing `misspy-2023.9.17rc1/misspy/reaction.py` & `misspy-2024.4.0/misspy/reaction.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,49 @@
-from .http import request
+from typing import Any
+from .core.http import request
 
 
-async def create(address, i, noteId, reaction):
-    """create reaction.
-
-    Args:
-        address (string): instance address
-        i (string): user token
-        noteId (string): noteId
-        reaction (string): Specify reaction. Reactions are Unicode emojis or custom emojis. For custom emoji, enclose the emoji name with a colon.
-
-    Returns:
-        dict: Misskey API response
-    """
-    return await request(
-        address, i, "notes/reactions/create", {"noteId": noteId, "reaction": reaction}
-    )
-
-
-async def delete(address, i, noteId):
-    """delete reaction.
-
-    Args:
-        address (string): instance address
-        i (string): user token
-        noteId (string): noteId
-
-    Returns:
-        dict: Misskey API response
-    """
-    return await request(address, i, "notes/reactions/delete", {"noteId": noteId})
+class reactions:
+    def __init__(self, address, i, ssl=True) -> None:
+        self.ssl = False
+        if ssl:
+            self.ssl = True
+
+        if not address.startswith("http://") and not address.startswith("https://"):
+            self.address = "http://" + address
+            if ssl:
+                self.address = "https://" + address
+            self.address_raw = address
+        else:
+            self.address = address
+            self.address_raw = address.replace("https://", "").replace("http://", "")
+        self.i = i
+
+    async def create(self, noteId, reaction):
+        """create reaction.
+
+        Args:
+            address (string): instance address
+            i (string): user token
+            noteId (string): noteId
+            reaction (string): Specify reaction. Reactions are Unicode emojis or custom emojis. For custom emoji, enclose the emoji name with a colon.
+
+        Returns:
+            dict: Misskey API response
+        """
+        return await request(
+            self.address, self.i, "notes/reactions/create", {"noteId": noteId, "reaction": reaction}
+        )
+
+
+    async def delete(self, noteId):
+        """delete reaction.
+
+        Args:
+            address (string): instance address
+            i (string): user token
+            noteId (string): noteId
+
+        Returns:
+            dict: Misskey API response
+        """
+        return await request(self.address, self.i, "notes/reactions/delete", {"noteId": noteId})
```

