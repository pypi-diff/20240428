# Comparing `tmp/earnapi-1.0.5.tar.gz` & `tmp/earnapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earnapi-1.0.5.tar", last modified: Tue Jun  7 19:25:01 2022, max compression
+gzip compressed data, was "earnapi-1.1.0.tar", last modified: Sun Apr 28 18:01:33 2024, max compression
```

## Comparing `earnapi-1.0.5.tar` & `earnapi-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-06-07 19:25:01.280074 earnapi-1.0.5/
--rw-r--r--   0 pi        (1000) pi        (1000)    35149 2022-06-07 18:04:00.000000 earnapi-1.0.5/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     2986 2022-06-07 19:25:01.280074 earnapi-1.0.5/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2301 2022-06-07 18:33:32.000000 earnapi-1.0.5/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-06-07 19:25:01.276074 earnapi-1.0.5/earnapi/
--rw-r--r--   0 pi        (1000) pi        (1000)       70 2022-06-07 19:24:13.000000 earnapi-1.0.5/earnapi/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     8262 2022-06-07 18:33:37.000000 earnapi-1.0.5/earnapi/client.py
--rw-r--r--   0 pi        (1000) pi        (1000)      592 2022-06-07 18:33:35.000000 earnapi-1.0.5/earnapi/errors.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3003 2022-06-07 18:33:36.000000 earnapi-1.0.5/earnapi/models.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-06-07 19:25:01.276074 earnapi-1.0.5/earnapi.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2986 2022-06-07 19:24:59.000000 earnapi-1.0.5/earnapi.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2022-06-07 19:25:01.000000 earnapi-1.0.5/earnapi.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-06-07 19:24:59.000000 earnapi-1.0.5/earnapi.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2022-06-07 19:25:00.000000 earnapi-1.0.5/earnapi.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2022-06-07 19:25:00.000000 earnapi-1.0.5/earnapi.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      104 2022-06-07 19:23:27.000000 earnapi-1.0.5/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-06-07 19:25:01.280074 earnapi-1.0.5/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     1115 2022-06-07 19:24:10.000000 earnapi-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:01:33.157587 earnapi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 18:01:26.000000 earnapi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-28 18:01:33.157587 earnapi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-28 18:01:26.000000 earnapi-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:01:33.157587 earnapi-1.1.0/earnapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:01:33.157587 earnapi-1.1.0/earnapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-28 18:01:26.000000 earnapi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:01:33.157587 earnapi-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-28 18:01:26.000000 earnapi-1.1.0/setup.py
```

### Comparing `earnapi-1.0.5/LICENSE` & `earnapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earnapi-1.0.5/PKG-INFO` & `earnapi-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: earnapi
-Version: 1.0.5
-Summary: Asynchronous EarnApp API wrapper written in Python.
-Home-page: https://github.com/Vincydotzsh/earnapi
+Version: 1.1.0
+Summary: Asynchronous EarnApp API wrapper written in Python using asyncio.
+Home-page: https://github.com/Vinchethescript/earnapi
 Author: Vinche.zsh
-Author-email: vincysuper07@gmail.com
-Project-URL: Bug Tracker, https://github.com/Vincydotzsh/earnapi/issues
+Author-email: 
+License: GPL-3.0
 Keywords: python,earnapi,python earnapp api,python earnapp api wrapper,earnapp api wrapper,earnapp,passive income,earnapp api,earnapp dashboard,requests,python earnapp
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 
 # EarnAPI
 
-Asynchronous EarnApp API wrapper written in Python based on [pyEarnapp](https://github.com/fazalfarhan01/EarnApp-API.git) (synchronous).
+EarnApp API wrapper written in Python using asyncio, inspired
+from [pyEarnapp](https://github.com/fazalfarhan01/EarnApp-API.git) (which does not use asyncio).
+
+## Be careful how you use this library!
+This library is not officially supported by EarnApp. Use it at your own risk.
+I am not responsible for any damage caused by using this library.\
+Also, please do not spam the API with requests.
+It is not nice and can get you banned or rate limited, and EarnApp rate limits last a lot.
 
 ## Installation
 ```bash
 pip install earnapi
 ```
 ## Example usage
 ```python
@@ -58,21 +63,7 @@
     # Add a device (not tested)
     #await client.add_device("sdk-xxxxx-xxxxxxxxxxxx")
     # Delete a device (not tested)
     #await client.delete_device("sdk-xxxxx-xxxxxxxxxxxx")
 
 loop.run_until_complete(main())
 ```
-
-## Exceptions
-- The following exceptions are defined.
-    Exception | Reason
-    --- | ---
-    `EarnAppError`: The exception all exceptions are based on.
-    `AuthenticationError`: Raised on authentication failure.
-    `DeviceOperationError`: Raised when any operation with a device fails.
-    `DeviceNotFoundError`: Raised when a device to add wasn't found.
-    `DeviceAlreadyAddedError`: Raised when a device is already added.
-    `TooManyRequestsError`: Raised when you reach EarnApp's rate limit.
-    `IPCheckError`: Raised when there's an error checking for the IP.
-    `InvalidIPError`: Raised when the IP address isn't valid.
-    `RedeemError`: Raised when an error occurs trying to redeem.
```

### Comparing `earnapi-1.0.5/README.md` & `earnapi-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # EarnAPI
 
-Asynchronous EarnApp API wrapper written in Python based on [pyEarnapp](https://github.com/fazalfarhan01/EarnApp-API.git) (synchronous).
+EarnApp API wrapper written in Python using asyncio, inspired
+from [pyEarnapp](https://github.com/fazalfarhan01/EarnApp-API.git) (which does not use asyncio).
+
+## Be careful how you use this library!
+This library is not officially supported by EarnApp. Use it at your own risk.
+I am not responsible for any damage caused by using this library.\
+Also, please do not spam the API with requests.
+It is not nice and can get you banned or rate limited, and EarnApp rate limits last a lot.
 
 ## Installation
 ```bash
 pip install earnapi
 ```
 ## Example usage
 ```python
@@ -41,21 +48,7 @@
     # Add a device (not tested)
     #await client.add_device("sdk-xxxxx-xxxxxxxxxxxx")
     # Delete a device (not tested)
     #await client.delete_device("sdk-xxxxx-xxxxxxxxxxxx")
 
 loop.run_until_complete(main())
 ```
-
-## Exceptions
-- The following exceptions are defined.
-    Exception | Reason
-    --- | ---
-    `EarnAppError`: The exception all exceptions are based on.
-    `AuthenticationError`: Raised on authentication failure.
-    `DeviceOperationError`: Raised when any operation with a device fails.
-    `DeviceNotFoundError`: Raised when a device to add wasn't found.
-    `DeviceAlreadyAddedError`: Raised when a device is already added.
-    `TooManyRequestsError`: Raised when you reach EarnApp's rate limit.
-    `IPCheckError`: Raised when there's an error checking for the IP.
-    `InvalidIPError`: Raised when the IP address isn't valid.
-    `RedeemError`: Raised when an error occurs trying to redeem.
```

### Comparing `earnapi-1.0.5/earnapi/client.py` & `earnapi-1.1.0/earnapi/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,55 +3,57 @@
 import typing
 from .errors import *
 from .models import *
 from urllib.parse import urljoin
 from aiohttp import ClientResponseError, ClientSession
 
 ip_regex = re.compile(
-    "^((25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9]?[0-9])\.){3}(25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9]?[0-9])$"
+    r"^((25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9]?[0-9])\.){3}(25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9]?[0-9])$"
 )
 
 
-def is_a_valid_ip(ipaddress: str):
+def is_ip_valid(ipaddress: str):
     return bool(ip_regex.search(ipaddress))
 
 
 class Client:
     def __init__(self, auth_refresh_token) -> None:
-        self.params = {"appid": "earnapp_dashboard"}
+        self.params = {"appid": "earnapp"}
         self.headers = {}
         self.cookies = {
             "auth": "1",
             "auth-method": "google",
             "oauth-refresh-token": auth_refresh_token,
         }
 
     async def request(
         self,
         method: str,
         endpoint: str,
-        cls: Model = None,
+        cls: typing.Optional[Model] = None,
         listify=False,
         return_response=False,
         *args,
         **kwargs,
     ) -> typing.Any:
         ret = None
         if (
             self.cookies.get("xsrf-token") == None
             or self.headers.get("xsrf-token") == None
         ):
             self.cookies["xsrf-token"] = self.headers["xsrf-token"] = ""
             await self._rotate_xsrf()
 
+        headers = self.headers.copy()
+        headers["If-None-Match"] = 'W/"12a-zq7F7whpD0+Cs/eDHKaVIJj+87U"'
         async with ClientSession() as session:
             async with session.request(
                 method,
                 endpoint,
-                headers=self.headers,
+                headers=headers,
                 params=self.params,
                 cookies=self.cookies,
                 *args,
                 **kwargs,
             ) as response:
                 if return_response:
                     ret = response
@@ -68,25 +70,31 @@
                         e.content = response_content
 
                     if response.status == 403:
                         raise AuthenticationError from None
                     else:
                         raise e
 
-                if not return_response:
+                if cls and not return_response:
+                    clss = cls
                     cls = cls.create_list if listify else cls
                     try:
                         ret = json.loads(response_content)
                         if listify and "list" in ret and isinstance(ret["list"], list):
                             ret = ret["list"]
 
                     except json.JSONDecodeError:
                         ret = response_content
 
-                    ret = cls(ret)
+                    if issubclass(clss, Interactable):
+                        ret = cls(self, ret)
+                    else:
+                        ret = cls(ret)
+                elif not cls and not return_response:
+                    ret = response_content
 
         return ret
 
     async def _rotate_xsrf(self):
         resp = await self.request("GET", Endpoint.XSRF, str, False, True)
         token = resp.cookies["xsrf-token"].coded_value
         self.cookies["xsrf-token"] = token
@@ -94,34 +102,51 @@
         return token
 
     async def get_user_data(self, *args, **kwargs) -> User:
         return await self.request(
             "GET", Endpoint.USER_DATA, User, False, *args, **kwargs
         )
 
-    async def get_earnings(self, *args, **kwargs) -> Earning:
+    async def get_earnings(self, *args, **kwargs) -> EarningsData:
         return await self.request(
-            "GET", Endpoint.MONEY, Earning, False * args, **kwargs
+            "GET", Endpoint.MONEY, EarningsData, False * args, **kwargs
         )
 
     async def get_devices(self, *args, **kwargs) -> typing.List[Device]:
         return await self.request(
             "GET", Endpoint.DEVICES, Device, True, *args, **kwargs
         )
 
+    async def get_device(self, uuid: str) -> Device:
+        devs = await self.get_devices()
+        dev = list(filter(lambda x: x.uuid == uuid, devs))
+        if not dev:
+            return
+
+        return dev[0]
+
     async def get_transactions(self, *args, **kwargs) -> typing.List[Transaction]:
         return await self.request(
             "GET", Endpoint.TRANSACTIONS, Transaction, True, *args, **kwargs
         )
 
-    async def get_referrals(self, *args, **kwargs) -> typing.List[Referral]:
-        return await self.request(
-            "GET", Endpoint.REFEREES, Referral, True, *args, **kwargs
+    async def get_referrals(self) -> typing.List[Referral]:
+        first = json.loads(
+            await self.request("GET", Endpoint.REFEREES, json={"page": 0})
         )
 
+        ret = first["list"]
+
+        for i in range(1, first["pagination"]["max"] + 1):
+            ret += json.loads(
+                await self.request("GET", Endpoint.REFEREES, json={"page": i})
+            )["list"]
+
+        return Referral.create_list(ret)
+
     async def add_device(self, new_device_id, *args, **kwargs):
         data = {"uuid": new_device_id}
         try:
             content = await self.request(
                 "POST",
                 Endpoint.LINK_DEVICE,
                 dict,
@@ -165,17 +190,17 @@
         else:
             error_message = content.get("error", None)
             if error_message:
                 raise DeviceOperationError(error_message)
             else:
                 return True if content.get("status", None) == "ok" else False
 
-    async def is_ip_allowed(self, ip_address: str, *args, **kwargs) -> bool:
-        if not is_a_valid_ip(ip_address):
-            raise IPCheckError("The IP address is not valid.")
+    async def check_ip(self, ip_address: str, *args, **kwargs) -> bool:
+        if not is_ip_valid(ip_address):
+            raise IPCheckError("Invalid IP Address provided.")
         try:
             content = await self.request(
                 "GET",
                 urljoin(Endpoint.IP_CHECK, ip_address),
                 dict,
                 False,
                 *args,
@@ -209,33 +234,48 @@
             if "ok" in content:
                 return content.get("ok", False)
             if error_message:
                 raise RedeemError(error_message)
             else:
                 return content
 
-    async def get_device_statuses(self) -> dict:
-        devices = await self.get_devices()
+    async def get_online_devices(
+        self, *uuids: typing.Union[Device, str]
+    ) -> list[OnlineDeviceStatus]:
         devices_req = []
 
-        for device in devices:
-            devices_req.append({"uuid": device.uuid, "appid": "node_earnapp.com"})
+        for device in uuids:
+            devices_req.append({"uuid": getattr(device, "uuid", device)})
+
+        kwargs = {}
+        if devices_req:
+            kwargs["json"] = {"devices": devices_req}
 
         try:
             content = await self.request(
                 "POST",
                 Endpoint.DEVICE_STATUSES,
                 dict,
                 False,
-                json={"list": devices_req},
+                **kwargs,
             )
         except ClientResponseError as e:
             if e.status == 429:
                 raise TooManyRequestsError(e.content) from None
             else:
                 raise Exception(f"Failed to get device statuses: {e.content}") from None
         else:
             error_message = content.get("error", None)
             if error_message:
                 raise Exception(error_message)
             else:
-                return content["statuses"]
+                ret = []
+                for k, v in content.items():
+                    ret.append(
+                        OnlineDeviceStatus(
+                            uuid=k,
+                            since=datetime.fromtimestamp(v[0] / 1000),
+                            uptime_today=v[1] / 1000,
+                        )
+                    )
+
+                return ret
```

### Comparing `earnapi-1.0.5/earnapi/errors.py` & `earnapi-1.1.0/earnapi/errors.py`

 * *Files identical despite different names*

### Comparing `earnapi-1.0.5/earnapi.egg-info/PKG-INFO` & `earnapi-1.1.0/earnapi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: earnapi
-Version: 1.0.5
-Summary: Asynchronous EarnApp API wrapper written in Python.
-Home-page: https://github.com/Vincydotzsh/earnapi
+Version: 1.1.0
+Summary: Asynchronous EarnApp API wrapper written in Python using asyncio.
+Home-page: https://github.com/Vinchethescript/earnapi
 Author: Vinche.zsh
-Author-email: vincysuper07@gmail.com
-Project-URL: Bug Tracker, https://github.com/Vincydotzsh/earnapi/issues
+Author-email: 
+License: GPL-3.0
 Keywords: python,earnapi,python earnapp api,python earnapp api wrapper,earnapp api wrapper,earnapp,passive income,earnapp api,earnapp dashboard,requests,python earnapp
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 
 # EarnAPI
 
-Asynchronous EarnApp API wrapper written in Python based on [pyEarnapp](https://github.com/fazalfarhan01/EarnApp-API.git) (synchronous).
+EarnApp API wrapper written in Python using asyncio, inspired
+from [pyEarnapp](https://github.com/fazalfarhan01/EarnApp-API.git) (which does not use asyncio).
+
+## Be careful how you use this library!
+This library is not officially supported by EarnApp. Use it at your own risk.
+I am not responsible for any damage caused by using this library.\
+Also, please do not spam the API with requests.
+It is not nice and can get you banned or rate limited, and EarnApp rate limits last a lot.
 
 ## Installation
 ```bash
 pip install earnapi
 ```
 ## Example usage
 ```python
@@ -58,21 +63,7 @@
     # Add a device (not tested)
     #await client.add_device("sdk-xxxxx-xxxxxxxxxxxx")
     # Delete a device (not tested)
     #await client.delete_device("sdk-xxxxx-xxxxxxxxxxxx")
 
 loop.run_until_complete(main())
 ```
-
-## Exceptions
-- The following exceptions are defined.
-    Exception | Reason
-    --- | ---
-    `EarnAppError`: The exception all exceptions are based on.
-    `AuthenticationError`: Raised on authentication failure.
-    `DeviceOperationError`: Raised when any operation with a device fails.
-    `DeviceNotFoundError`: Raised when a device to add wasn't found.
-    `DeviceAlreadyAddedError`: Raised when a device is already added.
-    `TooManyRequestsError`: Raised when you reach EarnApp's rate limit.
-    `IPCheckError`: Raised when there's an error checking for the IP.
-    `InvalidIPError`: Raised when the IP address isn't valid.
-    `RedeemError`: Raised when an error occurs trying to redeem.
```

### Comparing `earnapi-1.0.5/setup.py` & `earnapi-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-import setuptools
+from setuptools import setup, find_packages
+import os
+import re
+
+packages = find_packages()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
+with open(
+    os.path.join(os.path.dirname(__file__), packages[0], "__init__.py"),
+    "r",
+    encoding="utf-8",
+) as f:
+    kwargs = {
+        var.strip("_"): val
+        for var, val in re.findall(
+            r'^(__\w+__)\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE
+        )
+    }
+    kwargs["author_email"] = kwargs.pop("email", "")
+
 # Setting up
-setuptools.setup(
+setup(
     name="earnapi",
-    version="1.0.5",
-    author="Vinche.zsh",
-    author_email="vincysuper07@gmail.com",
-    description="Asynchronous EarnApp API wrapper written in Python.",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=["earnapi"],
+    packages=packages,
     python_requires=">=3.7",
     install_requires=["aiohttp"],
-    url="https://github.com/Vincydotzsh/earnapi",
-    project_urls={
-        "Bug Tracker": "https://github.com/Vincydotzsh/earnapi/issues",
-    },
     keywords=[
         "python",
         "earnapi",
         "python earnapp api",
         "python earnapp api wrapper",
         "earnapp api wrapper",
         "earnapp",
         "passive income",
         "earnapp api",
         "earnapp dashboard",
         "requests",
         "python earnapp",
     ],
-    classifiers=[
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-    ],
+    **kwargs
 )
```

