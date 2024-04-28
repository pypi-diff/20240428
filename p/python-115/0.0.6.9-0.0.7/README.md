# Comparing `tmp/python_115-0.0.6.9.tar.gz` & `tmp/python_115-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.9.tar", max compression
+gzip compressed data, was "python_115-0.0.7.tar", max compression
```

## Comparing `python_115-0.0.6.9.tar` & `python_115-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.9/LICENSE
--rwxr-xr-x   0        0        0   278288 2024-04-27 06:52:19.943731 python_115-0.0.6.9/p115/__init__.py
--rwxr-xr-x   0        0        0      115 2024-04-26 14:30:33.715269 python_115-0.0.6.9/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.9/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.9/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.9/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.9/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.9/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.9/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.9/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.9/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.9/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.9/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.9/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.9/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.9/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.9/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.9/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.9/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.9/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.9/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.9/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.9/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.9/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.9/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.9/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-27 07:46:40.661926 python_115-0.0.6.9/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.9/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7/LICENSE
+-rwxr-xr-x   0        0        0   287484 2024-04-28 15:43:44.390863 python_115-0.0.7/p115/__init__.py
+-rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6857 2024-04-28 15:44:22.845020 python_115-0.0.7/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7/p115/py.typed
+-rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7/p115/tool/__init__.py
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1270 2024-04-28 14:00:49.525373 python_115-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7/readme.md
+-rw-r--r--   0        0        0    35894 1970-01-01 00:00:00.000000 python_115-0.0.7/PKG-INFO
```

### Comparing `python_115-0.0.6.9/LICENSE` & `python_115-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/__init__.py` & `python_115-0.0.7/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 from __future__ import annotations
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 6)
+__version__ = (0, 0, 7)
 __all__ = [
     "P115Client", "P115Path", "P115FileSystem", "P115SharePath", "P115ShareFileSystem", 
     "P115ZipPath", "P115ZipFileSystem", "P115Offline", "P115Recyclebin", "P115Sharing", 
+    "LabelList", 
 ]
 
 import errno
 
 from abc import ABC, abstractmethod
 from asyncio import get_running_loop, run_coroutine_threadsafe, run, to_thread
 from binascii import b2a_hex
@@ -187,27 +188,32 @@
                 info2[k2] = datetime.fromtimestamp(t)
                 if k3:
                     info2[k3] = t
             except ValueError:
                 pass
     if "pc" in info:
         info2["pickcode"] = info["pc"]
-    if "m" in info:
-        info2["star"] = bool(info["m"])
     if "fl" in info:
         info2["labels"] = info["fl"]
-    if "fdes" in info:
-        info2["comment"] = info["fdes"]
     if "score" in info:
-        info2["score"] = info["score"]
+        info2["score"] = int(info["score"])
+    if "m" in info:
+        info2["star"] = bool(info["m"])
+    if "issct" in info:
+        info2["shortcut"] = bool(info["issct"])
+    if "hdf":
+        info2["hidden"] = bool(info["hdf"])
+    if "fdes" in info:
+        info2["described"] = bool(info["fdes"])
+    if "c" in info:
+        info2["violated"] = bool(info["c"])
     if "u" in info:
         info2["thumb"] = info["u"]
     if "play_long" in info:
         info2["play_long"] = info["play_long"]
-    info2["is_violation"] = bool(info.get("c", False))
     if keep_raw:
         info2["raw"] = info
     if extra_data:
         info2.update(extra_data)
     return info2
 
 
@@ -232,44 +238,40 @@
         return f"{type(self).__qualname__}({str(self)!r}, {self.__dict__})"
 
     def geturl(self) -> str:
         return str(self)
 
 
 class P115Client:
-    cookie: str
     session: Session
     user_id: int
     user_key: str
 
     def __init__(self, /, cookie=None, login_app: str = "web"):
         ns = self.__dict__
         session = ns["session"] = Session()
         session.headers["User-Agent"] = f"Mozilla/5.0 115disk/{APP_VERSION}"
         if not cookie:
             resp = self.login_with_qrcode(login_app)
             cookie = resp["data"]["cookie"]
-        self.set_cookie(cookie)
+        self.cookie = cookie
         resp = self.upload_info
         if resp["errno"]:
             raise AuthenticationError(resp)
         ns.update(user_id=resp["user_id"], user_key=resp["userkey"])
 
     def __del__(self, /) -> None:
         self.close()
 
     def __eq__(self, other, /) -> bool:
         return type(self) is type(other) and self.user_id == other.user_id
 
     def __hash__(self, /) -> int:
         return hash((self.user_id, self.cookie))
 
-    def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attributes")
-
     @cached_property
     def async_session(self, /) -> ClientSession:
         session = ClientSession(raise_for_status=True)
         session.headers.update(self.session.headers) # type: ignore
         cookiejar = session.cookie_jar
         cookiejar.clear()
         cookiejar.update_cookies(self.session.cookies, URL("http://.115.com"))
@@ -286,15 +288,20 @@
             try:
                 loop = get_running_loop()
             except RuntimeError:
                 run(ns["async_session"].close())
             else:
                 run_coroutine_threadsafe(ns["async_session"].close(), loop)
 
-    def set_cookie(self, cookie, /):
+    @property
+    def cookie(self, /) -> str:
+        return self.__dict__["cookie"]
+
+    @cookie.setter
+    def cookie(self, cookie, /):
         if isinstance(cookie, str):
             cookie = cookies_str_to_dict(cookie)
         cookiejar = self.session.cookies
         cookiejar.clear()
         if isinstance(cookie, Mapping):
             for key in ("UID", "CID", "SEID"):
                 cookiejar.set_cookie(
@@ -382,15 +389,15 @@
         self, 
         /, 
         app: str = "web", 
         **request_kwargs, 
     ):
         if not self.is_login(**request_kwargs):
             cookie = self.login_with_qrcode(app, **request_kwargs)["data"]["cookie"]
-            self.set_cookie(cookie)
+            self.cookie = cookie
 
     def _request(
         self, 
         /, 
         url: str, 
         method: str = "GET", 
         parse: None | bool | Callable = False, 
@@ -917,15 +924,15 @@
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
             - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
             - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
             - source: str = <default>
-            - star: 0 | 1 = <default>
+            - star: 0 | 1 = <default> # 是否星标文件
             - suffix: str = <default>
             - type: int | str = <default>
                 # 文件类型：
                 # - 所有: 0
                 # - 文档: 1
                 # - 图片: 2
                 # - 音频: 3
@@ -971,15 +978,15 @@
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
             - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
             - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
             - source: str = <default>
-            - star: 0 | 1 = <default>
+            - star: 0 | 1 = <default> # 是否星标文件
             - suffix: str = <default>
             - type: int | str = <default>
                 # 文件类型：
                 # - 所有: 0
                 # - 文档: 1
                 # - 图片: 2
                 # - 音频: 3
@@ -1064,40 +1071,45 @@
         payload:
             - fid[0]: int | str
             - fid[1]: int | str
             - ...
             - hidden: 0 | 1 = 1
         """
         api = "https://webapi.115.com/files/hiddenfiles"
-        if isinstance(payload, (int | str)):
+        if isinstance(payload, (int, str)):
             payload = {"hidden": 1, "fid[0]": payload}
         elif isinstance(payload, dict):
             payload = {"hidden": 1, **payload}
         else:
             payload = {f"f[{i}]": f for i, f in enumerate(payload)}
             if not payload:
                 return {"state": False, "message": "no op"}
             payload["hidden"] = 1
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_hidden_switch(
         self, 
-        payload: dict, 
+        payload: str | dict = "", 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """切换隐藏模式
         POST https://115.com/?ct=hiddenfiles&ac=switching
         payload:
-            show: 0 | 1 = 1
-            safe_pwd: int | str = <default> # 密码，如果需要进入隐藏模式，请传递此参数
+            safe_pwd: str = "" # 密码，如果需要进入隐藏模式，请传递此参数
+            show: 0 | 1 = <default>
             valid_type: int = 1
         """
         api = "https://115.com/?ct=hiddenfiles&ac=switching"
+        if isinstance(payload, str):
+            if payload:
+                payload = {"valid_type": 1, "show": 1, "safe_pwd": payload}
+            else:
+                payload = {"valid_type": 1, "show": 0}
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_statistic(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
@@ -1251,87 +1263,14 @@
         api = "https://webapi.115.com/files/search"
         if isinstance(payload, str):
             payload = {"aid": 1, "cid": 0, "format": "json", "limit": 32, "offset": 0, "show_dir": 1, "search_value": payload}
         else:
             payload = {"aid": 1, "cid": 0, "format": "json", "limit": 32, "offset": 0, "show_dir": 1, **payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
-    def comment_get(
-        self, 
-        payload: int | str | dict, 
-        /, 
-        async_: bool = False, 
-        **request_kwargs, 
-    ) -> dict:
-        """获取文件或文件夹的备注
-        GET https://webapi.115.com/files/desc
-        payload:
-            - file_id: int | str
-            - format: str = "json"
-            - compat: 0 | 1 = 1
-            - new_html: 0 | 1 = 1
-        """
-        api = "https://webapi.115.com/files/desc"
-        if isinstance(payload, (int, str)):
-            payload = {"format": "json", "compat": 1, "new_html": 1, "file_id": payload}
-        else:
-            payload = {"format": "json", "compat": 1, "new_html": 1, **payload}
-        return self.request(api, params=payload, async_=async_, **request_kwargs)
-
-    def comment_set(
-        self, 
-        fids: int | str | Iterable[int | str], 
-        /, 
-        file_desc: str = "", 
-        async_: bool = False, 
-        **request_kwargs, 
-    ) -> dict:
-        """为文件或文件夹设置备注，此接口是对 `fs_files_edit` 的封装
-
-        :param fids: 单个或多个文件或文件夹 id
-        :param file_desc: 备注信息，可以用 html
-        """
-        if isinstance(fids, (int, str)):
-            payload = [("fid", fids)]
-        else:
-            payload = [("fid[]", fid) for fid in fids]
-            if not payload:
-                return {"state": False, "message": "no op"}
-        payload.append(("file_desc", file_desc))
-        return self.fs_files_edit(payload, async_=async_, **request_kwargs)
-
-    def label_add(
-        self, 
-        /, 
-        *lables: str, 
-        async_: bool = False, 
-        **request_kwargs, 
-    ) -> dict:
-        """添加标签（可以接受多个）
-        POST https://webapi.115.com/label/add_multi
-
-        可传入多个 label 描述，每个 label 的格式都是 "{label_name}\x07{color}"，例如 "tag\x07#FF0000"
-        """
-        api = "https://webapi.115.com/label/add_multi"
-        payload = [("name[]", label) for label in lables if label]
-        if not payload:
-            return {"state": False, "message": "no op"}
-        if (headers := request_kwargs.get("headers")):
-            headers = request_kwargs["headers"] = dict(headers)
-        else:
-            headers = request_kwargs["headers"] = {}
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-        return self.request(
-            api, 
-            "POST", 
-            data=urlencode(payload), 
-            async_=async_, 
-            **request_kwargs, 
-        )
-
     def fs_export_dir(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
@@ -1376,15 +1315,28 @@
             file_ids: int | str   # 有多个时，用逗号 "," 隔开
             target: str = "U_1_0" # 导出目录树到这个目录
             layer_limit: int = <default> # 层级深度，自然数
         """
         resp = check_response(self.fs_export_dir(payload, async_=async_, **request_kwargs))
         return ExportDirStatus(self, resp["data"]["export_id"])
 
-    def fs_shortcut(
+    def fs_shortcut_get(
+        self, 
+        payload: int | str | dict, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """罗列所有的快捷入口
+        GET https://webapi.115.com/category/shortcut
+        """
+        api = "https://webapi.115.com/category/shortcut"
+        return self.request(api, async_=async_, **request_kwargs)
+
+    def fs_shortcut_set(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """把一个目录设置或取消为快捷入口
@@ -1394,89 +1346,82 @@
             op: "add" | "delete" = "add"
         """
         api = "https://webapi.115.com/category/shortcut"
         if isinstance(payload, (int, str)):
             payload = {"file_id": payload}
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
-    def fs_shortcut_list(
+    def fs_cover(
         self, 
-        payload: int | str | dict, 
+        fids: int | str | Iterable[int | str], 
         /, 
+        fid_cover: int | str = 0, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        """罗列所有的快捷入口
-        GET https://webapi.115.com/category/shortcut
-        """
-        api = "https://webapi.115.com/category/shortcut"
-        return self.request(api, async_=async_, **request_kwargs)
+        """设置目录的封面，此接口是对 `fs_files_edit` 的封装
 
-    # TODO: 还需要接口，获取单个标签 id 对应的信息，也就是通过 id 来获取
+        :param fids: 单个或多个文件或文件夹 id
+        :param file_label: 图片的 id，如果为 0 则是删除封面
+        """
+        api = "https://webapi.115.com/label/delete"
+        if isinstance(fids, (int, str)):
+            payload = [("fid", fids)]
+        else:
+            payload = [("fid[]", fid) for fid in fids]
+            if not payload:
+                return {"state": False, "message": "no op"}
+        payload.append(("fid_cover", fid_cover))
+        return self.fs_files_edit(payload, async_=async_, **request_kwargs)
 
-    def label_del(
+    def fs_desc_get(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        """删除标签
-        POST https://webapi.115.com/label/delete
+        """获取文件或文件夹的备注
+        GET https://webapi.115.com/files/desc
         payload:
-            - id: int | str # 标签 id
+            - file_id: int | str
+            - format: str = "json"
+            - compat: 0 | 1 = 1
+            - new_html: 0 | 1 = 1
         """
-        api = "https://webapi.115.com/label/delete"
+        api = "https://webapi.115.com/files/desc"
         if isinstance(payload, (int, str)):
-            payload = {"id": payload}
-        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+            payload = {"format": "json", "compat": 1, "new_html": 1, "file_id": payload}
+        else:
+            payload = {"format": "json", "compat": 1, "new_html": 1, **payload}
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
 
-    def label_edit(
+    def fs_desc(
         self, 
-        payload: dict, 
+        fids: int | str | Iterable[int | str], 
         /, 
+        file_desc: str = "", 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        """编辑标签
-        POST https://webapi.115.com/label/edit
-        payload:
-            - id: int | str # 标签 id
-            - name: str = <default>  # 标签名
-            - color: str = <default> # 标签颜色，支持 css 颜色语法
-        """
-        api = "https://webapi.115.com/label/edit"
-        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+        """为文件或文件夹设置备注，最多允许 65535 个字节 (64 KB 以内)，此接口是对 `fs_files_edit` 的封装
 
-    def label_list(
-        self, 
-        payload: dict = {}, 
-        /, 
-        async_: bool = False, 
-        **request_kwargs, 
-    ) -> dict:
-        """罗列标签列表（如果要获取做了标签的文件列表，用 `fs_search` 接口）
-        GET https://webapi.115.com/label/list
-        payload:
-            - offset: int = 0 # 索引偏移，从 0 开始
-            - limit: int = 11500 # 一页大小
-            - keyword: str = <default> # 搜索关键词
-            - sort: "name" | "update_time" | "create_time" = <default>
-                # 排序字段：
-                # - 名称: "name"
-                # - 创建时间: "create_time"
-                # - 更新时间: "update_time"
-            - order: "asc" | "desc" = <default> # 排序顺序："asc"(升序), "desc"(降序)
-            - user_id: int | str = <default>
+        :param fids: 单个或多个文件或文件夹 id
+        :param file_desc: 备注信息，可以用 html
         """
-        api = "https://webapi.115.com/label/list"
-        payload = {"offset": 0, "limit": 11500, **payload}
-        return self.request(api, params=payload, async_=async_, **request_kwargs)
+        if isinstance(fids, (int, str)):
+            payload = [("fid", fids)]
+        else:
+            payload = [("fid[]", fid) for fid in fids]
+            if not payload:
+                return {"state": False, "message": "no op"}
+        payload.append(("file_desc", file_desc))
+        return self.fs_files_edit(payload, async_=async_, **request_kwargs)
 
-    def label_set(
+    def fs_label(
         self, 
         fids: int | str | Iterable[int | str], 
         /, 
         file_label: int | str = "", 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
@@ -1490,15 +1435,15 @@
         else:
             payload = [("fid[]", fid) for fid in fids]
             if not payload:
                 return {"state": False, "message": "no op"}
         payload.append(("file_label", file_label))
         return self.fs_files_edit(payload, async_=async_, **request_kwargs)
 
-    def label_batch(
+    def fs_label_batch(
         self, 
         payload: dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """批量设置标签
@@ -1513,34 +1458,140 @@
             - file_ids: int | str # 文件或文件夹 id，如果有多个，用逗号 "," 隔开
             - file_label: int | str = <default> # 标签 id，如果有多个，用逗号 "," 隔开
             - file_label[{file_label}]: int | str = <default> # action 为 replace 时使用此参数，file_label[{原标签id}]: {目标标签id}，例如 file_label[123]: 456，就是把 id 是 123 的标签替换为 id 是 456 的标签
         """
         api = "https://webapi.115.com/files/batch_label"
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
-    def star_set(
+    def fs_score(
         self, 
-        payload: int | str | dict, 
+        file_id: int | str, 
         /, 
+        score: int = 0, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """给文件或文件夹评分
+        POST https://webapi.115.com/files/score
+        payload:
+            - file_id: int | str # 文件或文件夹 id，如果有多个，用逗号 "," 隔开
+            - score: int = 0     # 0 为删除评分
+        """
+        api = "https://webapi.115.com/files/score"
+        payload = {"file_id": file_id, "score": score}
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    def fs_star(
+        self, 
+        file_id: int | str, 
+        /, 
+        star: bool = True, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """为文件或文件夹设置或取消星标
         POST https://webapi.115.com/files/star
         payload:
             - file_id: int | str # 文件或文件夹 id，如果有多个，用逗号 "," 隔开
             - star: 0 | 1 = 1
         """
         api = "https://webapi.115.com/files/star"
-        if isinstance(payload, (int, str)):
-            payload = {"star": 1, "file_id": payload}
+        payload = {"file_id": file_id, "star": int(star)}
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    # TODO: 还需要接口，获取单个标签 id 对应的信息，也就是通过 id 来获取
+
+    def label_add(
+        self, 
+        /, 
+        *lables: str, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """添加标签（可以接受多个）
+        POST https://webapi.115.com/label/add_multi
+
+        可传入多个 label 描述，每个 label 的格式都是 "{label_name}\x07{color}"，例如 "tag\x07#FF0000"
+        """
+        api = "https://webapi.115.com/label/add_multi"
+        payload = [("name[]", label) for label in lables if label]
+        if not payload:
+            return {"state": False, "message": "no op"}
+        if (headers := request_kwargs.get("headers")):
+            headers = request_kwargs["headers"] = dict(headers)
         else:
-            payload = {"star": 1, **payload}
+            headers = request_kwargs["headers"] = {}
+        headers["Content-Type"] = "application/x-www-form-urlencoded"
+        return self.request(
+            api, 
+            "POST", 
+            data=urlencode(payload), 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def label_del(
+        self, 
+        payload: int | str | dict, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """删除标签
+        POST https://webapi.115.com/label/delete
+        payload:
+            - id: int | str # 标签 id，如果有多个，用逗号 "," 隔开
+        """
+        api = "https://webapi.115.com/label/delete"
+        if isinstance(payload, (int, str)):
+            payload = {"id": payload}
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    def label_edit(
+        self, 
+        payload: dict, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """编辑标签
+        POST https://webapi.115.com/label/edit
+        payload:
+            - id: int | str # 标签 id
+            - name: str = <default>  # 标签名
+            - color: str = <default> # 标签颜色，支持 css 颜色语法
+            - sort: int = <default> # 序号
+        """
+        api = "https://webapi.115.com/label/edit"
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
+    def label_list(
+        self, 
+        payload: dict = {}, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """罗列标签列表（如果要获取做了标签的文件列表，用 `fs_search` 接口）
+        GET https://webapi.115.com/label/list
+        payload:
+            - offset: int = 0 # 索引偏移，从 0 开始
+            - limit: int = 11500 # 一页大小
+            - keyword: str = <default> # 搜索关键词
+            - sort: "name" | "update_time" | "create_time" = <default>
+                # 排序字段:
+                # - 名称: "name"
+                # - 创建时间: "create_time"
+                # - 更新时间: "update_time"
+            - order: "asc" | "desc" = <default> # 排序顺序："asc"(升序), "desc"(降序)
+        """
+        api = "https://webapi.115.com/label/list"
+        payload = {"offset": 0, "limit": 11500, **payload}
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
     def life_list(
         self, 
         payload: dict = {}, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
@@ -4001,34 +4052,48 @@
 
     def get_zip_fs(self, id_or_pickcode: int | str, /, *args, **kwargs) -> P115ZipFileSystem:
         """
         """
         return P115ZipFileSystem(self, id_or_pickcode, *args, **kwargs)
 
     @cached_property
+    def label(self, /) -> LabelList:
+        """
+        """
+        return LabelList(self)
+
+    @cached_property
     def offline(self, /) -> P115Offline:
         """
         """
         return P115Offline(self)
 
     def get_offline(self, /, *args, **kwargs) -> P115Offline:
         return P115Offline(self, *args, **kwargs)
 
     @cached_property
     def recyclebin(self, /) -> P115Recyclebin:
+        """
+        """
         return P115Recyclebin(self)
 
     def get_recyclebin(self, /, *args, **kwargs) -> P115Recyclebin:
+        """
+        """
         return P115Recyclebin(self, *args, **kwargs)
 
     @cached_property
     def sharing(self, /) -> P115Sharing:
+        """
+        """
         return P115Sharing(self)
 
     def get_sharing(self, /, *args, **kwargs) -> P115Sharing:
+        """
+        """
         return P115Sharing(self, *args, **kwargs)
 
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
         headers: Optional[Mapping] = None, 
@@ -5604,14 +5669,22 @@
             overwrite_or_ignore=overwrite_or_ignore, 
             recursive=True, 
         )
         if attr is None:
             return None
         return type(self)(attr)
 
+    @property
+    def description(self, /):
+        return self.fs.desc(self)
+
+    @description.setter
+    def description(self, /, desc: str = ""):
+        return self.fs.desc(self, desc=desc)
+
     def mkdir(self, /, exist_ok: bool = True) -> Self:
         self.__dict__.update(self.fs.makedirs(self, exist_ok=exist_ok))
         return self
 
     def move(
         self, 
         /, 
@@ -5700,42 +5773,41 @@
     get_version: Optional[Callable]
     path_class = P115Path
 
     def __init__(
         self, 
         /, 
         client: P115Client, 
+        password: str = "", 
         attr_cache: Optional[MutableMapping[int, dict]] = None, 
         path_to_id: Optional[MutableMapping[str, int]] = None, 
         get_version: Optional[Callable] = lambda attr: attr.get("mtime", 0), 
     ):
         if attr_cache is not None:
             attr_cache = {}
         if type(path_to_id) is dict:
             path_to_id["/"] = 0
         elif path_to_id is not None:
             path_to_id = ChainMap(path_to_id, {"/": 0})
         self.__dict__.update(
             client = client, 
             cid = 0, 
             path = "/", 
+            password = password, 
             path_to_id = path_to_id, 
             attr_cache = attr_cache, 
             get_version = get_version, 
         )
 
     def __delitem__(self, id_or_path: IDOrPathType, /):
         self.rmtree(id_or_path)
 
     def __len__(self, /) -> int:
         return self.get_directory_capacity(self.cid)
 
-    def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attributes")
-
     def __setitem__(
         self, 
         id_or_path: IDOrPathType, 
         file: None | str | bytes | bytearray | memoryview | PathLike = None, 
         /, 
     ):
         if file is None:
@@ -5757,14 +5829,22 @@
         cookie = None, 
         app: str = "web", 
         **kwargs, 
     ) -> Self:
         kwargs["client"] = P115Client(cookie, login_app=app)
         return cls(**kwargs)
 
+    @property
+    def password(self, /) -> str:
+        return self.__dict__["password"]
+
+    @password.setter
+    def password(self, /, password: str = ""):
+        self.__dict__["password"] = password
+
     @check_response
     def fs_mkdir(self, name: str, /, pid: int = 0) -> dict:
         return self.client.fs_mkdir({"cname": name, "pid": pid})
 
     @check_response
     def fs_copy(self, id: int, /, pid: int = 0) -> dict:
         return self.client.fs_copy(id, pid)
@@ -6392,14 +6472,29 @@
         if id:
             ls.extend(
                 {"name": p["name"], "id": int(p["cid"]), "parent_id": int(p["pid"]), "is_directory": True} 
                 for p in self.fs_files(id, limit=1)["path"][1:]
             )
         return ls
 
+    def desc(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        desc: None | str = None, 
+    ) -> str:
+        fid = self.get_id(id_or_path, pid)
+        if fid == 0:
+            return ""
+        if desc is None:
+            return check_response(self.client.fs_desc_get(fid))["desc"]
+        else:
+            return check_response(self.client.fs_desc(fid, desc))["file_description"]
+
     def get_ancestors(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> list[dict]:
         attr = self.attr(id_or_path, pid)
@@ -6440,15 +6535,15 @@
         detail: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         return self.client.download_url(
             attr["pickcode"], 
-            use_web_api=attr["is_violation"] and attr["size"] < 1024 * 1024 * 115, 
+            use_web_api=attr.get("violated", False) and attr["size"] < 1024 * 1024 * 115, 
             detail=detail, 
             headers=headers, 
         )
 
     def get_url_from_pickcode(
         self, 
         /, 
@@ -6458,14 +6553,38 @@
     ) -> str:
         return self.client.download_url(
             pickcode, 
             detail=detail, 
             headers=headers, 
         )
 
+    def hide(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        show: None | bool = None, 
+    ) -> bool:
+        if show is None:
+            return self.attr(id_or_path, pid)["hidden"]
+        else:
+            fid = self.get_id(id_or_path, pid)
+            if fid == 0:
+                return False
+            hidden = not show
+            check_response(self.client.fs_files_hidden({"hidden": int(hidden), "fid[0]": fid}))
+            return hidden
+
+    def hidden_switch(
+        self, 
+        show: bool = True, 
+        password: str = "", 
+    ):
+        check_response(self.client.fs_hidden_switch({"show": int(show), "safe_pwd": password or self.password}))
+
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
         attr: dict | P115Path
@@ -6476,14 +6595,22 @@
                 attr = self.attr(id_or_path, pid)
             except FileNotFoundError:
                 return True
         if attr["is_directory"]:
             return self.get_directory_capacity(attr["id"]) > 0
         return attr["size"] == 0
 
+    def labels(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+    ) -> list[dict]:
+        return self.attr(id_or_path, pid)["labels"]
+
     def makedirs(
         self, 
         path: str | PathLike[str] | Sequence[str] | AttrDict, 
         /, 
         pid: Optional[int] = None, 
         exist_ok: bool = False, 
     ) -> dict:
@@ -6776,14 +6903,30 @@
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
     ) -> dict:
         return self.remove(id_or_path, pid, recursive=True)
 
+    def score(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        score: None | int = None, 
+    ) -> int:
+        if score is None:
+            return self.attr(id_or_path, pid).get("score", 0)
+        else:
+            fid = self.get_id(id_or_path, pid)
+            if fid == 0:
+                return 0
+            self.client.fs_score(fid, score)
+            return score
+
     def search(
         self, 
         search_value: str, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         page_size: int = 1_000, 
@@ -6813,14 +6956,30 @@
             for attr in resp["data"]:
                 attr = normalize_info(attr, fs=self, last_update=last_update)
                 yield P115Path(attr)
             offset = payload["offset"] = offset + resp["page_size"]
             if offset >= resp["count"]:
                 break
 
+    def star(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        star: None | bool = None, 
+    ) -> int:
+        if star is None:
+            return self.attr(id_or_path, pid).get("star", False)
+        else:
+            fid = self.get_id(id_or_path, pid)
+            if fid == 0:
+                return False
+            check_response(self.client.fs_star(fid, star))
+            return star
+
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> stat_result:
         attr = self.attr(id_or_path, pid)
@@ -8062,14 +8221,161 @@
         })
 
     @check_response
     def update(self, /, share_code: str, **payload) -> dict:
         return self.client.share_update({"share_code": share_code, **payload})
 
 
+class LabelList:
+    __slots__ = "client",
+
+    def __init__(self, client: P115Client, /):
+        self.client = client
+
+    def __contains__(self, id_or_name: int | str, /) -> bool:
+        if isinstance(id_or_name, int):
+            return self.client.label_edit({"id": id_or_name})["code"] != 21005
+        else:
+            name = id_or_name
+            return any(item["name"] == name for item in self.iter(keyword=name))
+
+    def __delitem__(self, id_or_name: int | str, /):
+        if isinstance(id_or_name, int):
+            id = id_or_name
+        else:
+            try:
+                item = self[id_or_name]
+            except LookupError:
+                return
+            id = item["id"]
+        self.client.label_del(id)
+
+    def __getitem__(self, id_or_name: int | str, /) -> dict:
+        if isinstance(id_or_name, int):
+            id = str(id_or_name)
+            for item in self.iter():
+                if item["id"] == id:
+                    return item
+        else:
+            name = id_or_name
+            for item in self.iter(keyword=name):
+                if item["name"] == name:
+                    return item
+        raise LookupError(f"no such id: {id!r}")
+
+    def __setitem__(self, id_or_name: int | str, value: str | dict, /):
+        if isinstance(id_or_name, int):
+            id = id_or_name
+        else:
+            item = self[id_or_name]
+            id = item["id"]
+        if isinstance(value, str):
+            payload = {"id": id, "name": value}
+        else:
+            payload = {**value, "id": id}
+        self.client.label_edit(payload)
+
+    def __iter__(self, /) -> Iterator[dict]:
+        return self.iter()
+
+    def __len__(self, /) -> int:
+        return check_response(self.client.label_list({"limit": 1}))["data"]["total"]
+
+    def __repr__(self, /) -> str:
+        cls = type(self)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module != "__main__":
+            name = module + "." + name
+        return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
+
+    def add(
+        self, 
+        /, 
+        *labels: str, 
+    ) -> list[dict]:
+        return check_response(self.client.label_add(*labels))["data"]
+
+    def clear(self, /):
+        self.client.label_del(",".join(item["id"] for item in self.iter()))
+
+    def get(self, id_or_name: int | str, /, default=None):
+        try:
+            return self[id_or_name]
+        except LookupError:
+            return default
+
+    def iter(
+        self, 
+        /, 
+        offset: int = 0, 
+        page_size: int = 11500, 
+        keyword: str = "", 
+        sort: Literal["", "name", "create_time", "update_time"] = "", 
+        order: Literal["", "asc", "desc"] = "", 
+    ) -> Iterator[dict]:
+        if offset < 0:
+            offset = 0
+        if page_size <= 0:
+            page_size = 11500
+        payload = {
+            "offset": offset, 
+            "limit": page_size, 
+            "keyword": keyword, 
+            "sort": sort, 
+            "order": order, 
+        }
+        count = 0
+        while True:
+            resp = check_response(self.client.label_list(payload))
+            total = resp["data"]["total"]
+            if count == 0:
+                count = total
+            elif count != total:
+                raise RuntimeError("detected count changes during iteration")
+            ls = resp["data"]["list"]
+            yield from ls
+            if len(ls) < page_size:
+                break
+            payload["offset"] += page_size # type: ignore
+
+    def iter_files(
+        self, 
+        id_or_name: int | str, 
+        /, 
+    ) -> Iterator[P115Path]:
+        if isinstance(id_or_name, int):
+            id = id_or_name
+        else:
+            id = self[id_or_name]["id"]
+        return self.client.fs.search("", 0, file_label=id)
+
+    def list(
+        self, 
+        /, 
+        offset: int = 0, 
+        limit: int = 0, 
+        keyword: str = "", 
+        sort: Literal["", "name", "create_time", "update_time"] = "", 
+        order: Literal["", "asc", "desc"] = "", 
+    ) -> list[dict]:
+        if limit <= 0:
+            return list(self.iter(offset, keyword=keyword, sort=sort, order=order))
+        return check_response(self.client.label_list({
+            "offset": offset, 
+            "limit": limit, 
+            "keyword": keyword, 
+            "sort": sort, 
+            "order": order, 
+        }))["data"]["list"]
+
+    edit = __setitem__
+    remove = __delitem__
+
+
 # TODO upload_tree 多线程和进度条，并且为每一个上传返回一个 task，可重试
 # TODO 能及时处理文件已不存在
 # TODO 为各个fs接口添加额外的请求参数
 # TODO 115中多个文件可以在同一目录下同名，如何处理
 # TODO 提供一个新的上传函数，上传如果失败，因为名字问题，则尝试用uuid名字，上传成功后，再进行改名，如果成功，删除原来的文件，不成功，则删掉上传的文件（如果上传成功了的话）
 # TODO 如果压缩包尚未解压，则使用 zipfile 之类的模块，去模拟文件系统
```

### Comparing `python_115-0.0.6.9/p115/cmd/iterdir.py` & `python_115-0.0.7/p115/cmd/iterdir.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__: list[str] = []
 __doc__ = "115 文件夹信息遍历导出"
 
 KEYS = (
     "id", "parent_id", "name", "path", "sha1", "pickcode", "is_directory", 
-    "size", "ctime", "mtime", "atime", "thumb", "star", 
+    "size", "ctime", "mtime", "atime", "hidden", "violated", "play_long", 
+    "thumb", "star", "score", "labels", "description", 
 )
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
 
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
@@ -114,15 +115,15 @@
             speed = total / (cur_t - start_t)
             write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
         file = open(output_file, "w")
         path_it = iter(progress(path_it))
     else:
         file = stdout # type: ignore
 
-    records = ({k: p.get(k) for k in keys} for p in path_it)
+    records = ({k: p.get(k) if k != "description" else p.description for k in keys} for p in path_it)
 
     dumps: Callable[..., bytes]
     if output_type in ("log", "json"):
         try:
             from orjson import dumps
         except ImportError:
             odumps: Callable[..., str]
```

### Comparing `python_115-0.0.6.9/p115/cmd/qrcode.py` & `python_115-0.0.7/p115/cmd/qrcode.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,22 +28,31 @@
     outfile = args.output_file
     file: TextIO
     if outfile:
         file = open(outfile, "w")
     else:
         from sys import stdout as file
 
-    client = P115Client(login_app=args.app)
+    cookie: str
+    if args.cookie:
+        from p115.tool import login_scan_cookie
+
+        client = P115Client(args.cookie)
+        cookie = login_scan_cookie(client, app=args.app)
+    else:
+        client = P115Client(login_app=args.app)
+        cookie = client.cookie
     print()
-    print(client.cookie, file=file)
+    print(cookie, file=file)
 
 
 parser.add_argument("app", nargs="?", choices=("web", "android", "ios", "linux", "mac", "windows", "tv", "alipaymini", "wechatmini", "qandroid"), default="web", 
                     help="选择一个 app 进行登录，注意：这会把已经登录的相同 app 踢下线")
 parser.add_argument("-o", "--output-file", help="保存到文件，未指定时输出到 stdout")
+parser.add_argument("-c", "--cookie", help="115 登录 cookie，如果提供了，就可以用这个 cookie 进行自动扫码，否则需要你用手机来手动扫码")
 parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
 parser.set_defaults(func=main)
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     main(args)
```

### Comparing `python_115-0.0.6.9/p115/util/_init_mimetypes.py` & `python_115-0.0.7/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/cipher.py` & `python_115-0.0.7/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/concurrent.py` & `python_115-0.0.7/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/download.py` & `python_115-0.0.7/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/file.py` & `python_115-0.0.7/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/hash.py` & `python_115-0.0.7/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/ignore.py` & `python_115-0.0.7/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/iter.py` & `python_115-0.0.7/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/path.py` & `python_115-0.0.7/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/property.py` & `python_115-0.0.7/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/response.py` & `python_115-0.0.7/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/retry.py` & `python_115-0.0.7/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/text.py` & `python_115-0.0.7/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/p115/util/urlopen.py` & `python_115-0.0.7/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/pyproject.toml` & `python_115-0.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.9"
+version = "0.0.7"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.9/readme.md` & `python_115-0.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.9/PKG-INFO` & `python_115-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.9
+Version: 0.0.7
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

