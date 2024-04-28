# Comparing `tmp/amino.light.py-0.1.5.tar.gz` & `tmp/amino.light.py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.5.tar", last modified: Thu Apr 11 17:53:35 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.6.tar", last modified: Sun Apr 28 15:39:45 2024, max compression
```

## Comparing `amino.light.py-0.1.5.tar` & `amino.light.py-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 17:53:35.415404 amino.light.py-0.1.5/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:53:35.371405 amino.light.py-0.1.5/AminoLightPy/
--rw-rw-rw-   0        0        0      296 2024-04-10 21:46:16.000000 amino.light.py-0.1.5/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0    17388 2024-04-10 00:15:18.000000 amino.light.py-0.1.5/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    72472 2024-04-11 17:50:55.000000 amino.light.py-0.1.5/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2663 2024-04-11 17:52:38.000000 amino.light.py-0.1.5/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:53:35.373405 amino.light.py-0.1.5/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.5/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:53:35.378404 amino.light.py-0.1.5/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.5/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    32075 2024-04-09 21:58:19.000000 amino.light.py-0.1.5/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1354 2024-04-09 22:00:38.000000 amino.light.py-0.1.5/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    95642 2024-04-10 21:45:50.000000 amino.light.py-0.1.5/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    17113 2024-04-10 21:45:48.000000 amino.light.py-0.1.5/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    75181 2024-04-11 17:49:52.000000 amino.light.py-0.1.5/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3567 2024-04-11 17:53:35.415404 amino.light.py-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2771 2024-04-11 17:53:14.000000 amino.light.py-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 17:53:35.413408 amino.light.py-0.1.5/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     3567 2024-04-11 17:53:33.000000 amino.light.py-0.1.5/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-04-11 17:53:34.000000 amino.light.py-0.1.5/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 17:53:33.000000 amino.light.py-0.1.5/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-11 17:53:33.000000 amino.light.py-0.1.5/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 17:53:33.000000 amino.light.py-0.1.5/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 17:53:35.423406 amino.light.py-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-04-11 17:53:08.000000 amino.light.py-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.344263 amino.light.py-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.230541 amino.light.py-0.1.6/AminoLightPy/
+-rw-rw-rw-   0        0        0      297 2024-04-19 03:59:31.000000 amino.light.py-0.1.6/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    14819 2024-04-24 14:56:57.000000 amino.light.py-0.1.6/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    16533 2024-04-28 15:38:37.000000 amino.light.py-0.1.6/AminoLightPy/amino_socket.py
+-rw-rw-rw-   0        0        0    74156 2024-04-28 15:28:46.000000 amino.light.py-0.1.6/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2704 2024-04-24 14:56:35.000000 amino.light.py-0.1.6/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.233543 amino.light.py-0.1.6/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.1.6/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.258287 amino.light.py-0.1.6/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    82921 2024-04-23 09:48:31.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0      184 2024-04-24 15:17:48.000000 amino.light.py-0.1.6/AminoLightPy/managers.py
+-rw-rw-rw-   0        0        0    67523 2024-04-23 09:48:37.000000 amino.light.py-0.1.6/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3630 2024-04-28 15:39:45.343260 amino.light.py-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.334749 amino.light.py-0.1.6/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     3630 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-04-28 15:39:44.000000 amino.light.py-0.1.6/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 15:39:45.350260 amino.light.py-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-04-19 03:21:12.000000 amino.light.py-0.1.6/setup.py
```

### Comparing `amino.light.py-0.1.5/AminoLightPy/client.py` & `amino.light.py-0.1.6/AminoLightPy/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # pylint: disable=invalid-name
+# pylint: disable=too-many-lines
 
 from uuid import uuid4
 from typing import BinaryIO, Union
 
 from .constants import api, upload_media, AminoSession
-from .socket import Callbacks, SocketHandler, SocketRequests
+from .amino_socket import Callbacks, SocketHandler, SocketRequests
 from .lib.util import exceptions, objects, helpers, self_deviceId
 
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
 class Client(Callbacks, SocketHandler, SocketRequests):
+    "Module for work with global"
     def __init__(self, proxies: dict = None, socketDebugging = False, socket_enabled = True):
         self.api = api
         self.authenticated = False
         self.session = AminoSession()
         self.device_id = self.session.headers["NDCDEVICEID"]
 
         self.socket_enabled = socket_enabled
         if socket_enabled:
             SocketHandler.__init__(self, self, socketDebugging)
-            SocketRequests.__init__(self)
+            SocketRequests.__init__(self, self)
             Callbacks.__init__(self)
 
         self.session.proxies = proxies
 
         self.sid = None
         self.profile = objects.UserProfile(None).UserProfile
         self.profile.session = self.session
@@ -82,15 +84,15 @@
             self.session.headers["NDCDEVICEID"] = self_deviceId(email)
 
         data = {
             "email": email,
             "secret": f"0 {password}",
             "clientType": 100,
             "deviceID": self.session.headers["NDCDEVICEID"],
-            "v": 2
+            "v": 2,
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
         self.sid = json["sid"]
         self.profile = objects.UserProfile(json["userProfile"]).UserProfile
@@ -271,25 +273,22 @@
             "deviceID": self.device_id,
             "clientType": 100
         }
 
         response = self.session.post(f"{api}/g/s/auth/logout", json=data)
         self.authenticated = False
         self.sid = None
-        self.profile: None
+        self.profile = None
         self.session.headers.update({
             "NDCAUTH": None,
             "AUID": None
         })
 
         self.profile.session = None
 
-        if self.socket_enabled:
-            self.close()
-
         return response.status_code
 
     def configure(self, age: int, gender: str):
         """
         Configure the settings of an account.
 
         **Parameters**
@@ -908,15 +907,15 @@
             - **Success** : :meth:`List of User IDs <None>`
 
             - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/block/full-list?start={start}&size={size}")
         return response.json()["blockerUidList"]
 
-    def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
+    def get_wall_comments(self, userId: str, sorting: str = "newest", start: int = 0, size: int = 25):
         """
         List of Wall Comments of an User.
 
         **Parameters**
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
@@ -990,15 +989,19 @@
         response = self.session.post(f"{api}/g/s/{flg}", json=data)
         return response.status_code
 
     def check_values(self, *args):
         "Check params in send_message metod."
         return any(arg is None for arg in args)
 
-    def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
+    def send_message(self, chatId: str, message: str = None, messageType: int = 0,
+                        file: BinaryIO = None, fileType: str = None, replyTo: str = None,
+                        mentionUserIds: list = None, stickerId: str = None, embedId: str = None,
+                        embedType: int = None, embedLink: str = None, embedTitle: str = None,
+                        embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
             - **chatId** : ID of the Chat.
             - **file** : File to be sent.
@@ -1108,15 +1111,20 @@
         """
         data = {
             "messageId": messageId,
         }
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/mark-as-read", json=data)
         return response.status_code
 
-    def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
+    def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None,
+            title: str = None, icon: str = None, backgroundImage: str = None,
+            content: str = None, announcement: str = None, coHosts: list = None,
+            keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None,
+            canTip: bool = None, viewOnly: bool = None, canInvite: bool = None,
+            fansOnly: bool = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **title** : Title of the Chat.
             - **content** : Content of the Chat.
@@ -1161,58 +1169,96 @@
             data["publishToGlobal"] = 1
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
                 data = {"alertOption": 2}
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/alert",
+                    json=data
+                )
                 res.append(response.status_code)
             if not doNotDisturb:
                 data = {"alertOption": 1}
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/alert",
+                    json=data
+                )
                 res.append(response.status_code)
         if pinChat is not None:
             if pinChat:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/pin", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/pin",
+                    json=data
+                )
                 res.append(response.status_code)
             if not pinChat:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/unpin", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/unpin",
+                    json=data
+                )
                 res.append(response.status_code)
         if backgroundImage is not None:
             data = {"media": [100, backgroundImage, None]}
-            response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/background", json=data)
+            response = self.session.post(
+                url=f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/background",
+                json=data
+            )
             res.append(response.status_code)
         if coHosts is not None:
             data = {"uidList": coHosts}
-            response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/co-host", json=data)
+            response = self.session.post(
+                url=f"{api}/g/s/chat/thread/{chatId}/co-host",
+                son=data
+            )
             res.append(response.status_code)
         if viewOnly is not None:
             if viewOnly:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/view-only/enable", json={})
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/view-only/enable"
+                )
                 res.append(response.status_code)
 
             if not viewOnly:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/view-only/disable", json={})
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/view-only/disable"
+                )
                 res.append(response.status_code)
         if canInvite is not None:
             if canInvite:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/members-can-invite/enable", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/members-can-invite/enable",
+                    json=data
+                )
                 res.append(response.status_code)
             if not canInvite:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/members-can-invite/disable", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/members-can-invite/disable",
+                    json=data
+                )
                 res.append(response.status_code)
         if canTip is not None:
             if canTip:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable",
+                    json=data
+                )
                 res.append(response.status_code)
             if not canTip:
-                response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable", json=data)
+                response = self.session.post(
+                    url=f"{api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable",
+                    json=data
+                )
                 res.append(response.status_code)
-        response = self.session.post(f"{api}/g/s/chat/thread/{chatId}", json=data)
+
+        response = self.session.post(
+            url=f"{api}/g/s/chat/thread/{chatId}",
+            json=data
+        )
         res.append(response.status_code)
 
         return res
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
         """
         Sends coins to a specified blog, chat, or object in the community.
@@ -1504,45 +1550,52 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {"ndcIds": comIds}
-        response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/reorder", json=data)
+        response = self.session.post(
+            url=f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/reorder",
+            json=data
+        )
         return response.status_code
 
     def add_linked_community(self, comId: int):
         """
         Add a Linked Community on your profile.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/{comId}")
+        response = self.session.post(
+            url=f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/{comId}"
+        )
         return response.status_code
 
     def remove_linked_community(self, comId: int):
         """
         Remove a Linked Community on your profile.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/{comId}")
+        response = self.session.delete(
+            url=f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/{comId}"
+        )
         return response.status_code
 
     def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None):
         """
         Comment on a User's Wall, Blog or Wiki.
 
         **Parameters**
@@ -2057,19 +2110,38 @@
             "size": size,
             "pagingType": "t"
         }
 
         response = self.session.get(f"{api}/g/s/topic/0/feed/community", params=params)
         return objects.CommunityList(response.json()["communityList"]).CommunityList
 
-
     def get_blockers(self) -> list[str]:
         """
         Get ids of user ho block you.
 
         **Returns**
             - **Success** : :meth:`List <str>`
 
             - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/block/full-list")
         return response.json()["blockerUidList"]
+
+    def set_privacy_status(self, isAnonymous: bool = False, getNotifications: bool = False):
+        """
+        Allow or disable global notification.
+
+        **Returns**
+            - **Success** : :meth:`List <str>`
+
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        data = {
+            "privacyMode": 2 if isAnonymous else 1
+        }
+        if not getNotifications:
+            data["notificationStatus"] = 2
+        else:
+            data["privacyMode"] = 1
+
+        response = self.session.post(f"{api}/g/s/account/visit-settings", json=data)
+        return response.json()
```

### Comparing `amino.light.py-0.1.5/AminoLightPy/constants.py` & `amino.light.py-0.1.6/AminoLightPy/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from time import time
 from json import dumps
 from hashlib import sha1
 from typing import BinaryIO
-from requests import Session
 from collections import OrderedDict
+from requests import Session
 
 from .lib.util.exceptions import SpecifyType
 from .lib.util import signature, gen_deviceId
 from .lib.util.exceptions import CheckException
 
 # add by August Light
 
@@ -16,28 +16,30 @@
 cache = OrderedDict()
 
 class AminoSession(Session):
     def __init__(self) -> None:
         super().__init__()
         self.headers.update({
             "NDCDEVICEID": device_id,
+            "Accept-Encoding": "gzip, deflate",
             "User-Agent": "Apple iPhone13,1 iOS v16.5 Main/3.19.0"
         })
 
     def request(self, method, url, *args, **kwargs):
 
         headers = kwargs.get("headers", {})
         data = kwargs.get("data", None)
 
         if method.lower() == "post":
             if "json" in kwargs and data is None:
-                data = kwargs.get("json")
-                
+                data = kwargs.get("json") or {}
                 data["timestamp"] = int(time() * 1000)
+
                 data = dumps(data)
+
                 headers["Content-Type"] = "application/json"
                 headers["NDC-MSG-SIG"] = signature(data)
 
             elif data is None:
                 headers["Content-Type"] = "application/x-www-form-urlencoded"
 
         kwargs["headers"] = headers
@@ -74,23 +76,23 @@
         t = "audio/aac"
     elif fileType == "image":
         t = "image/jpg"
     elif fileType == "gif":
         t = "image/gif"
     else: raise SpecifyType(fileType)
 
-    
     custom_headers = self.session.headers
     custom_headers["Content-Type"] = t
 
     response = self.session.post(
         url=f"{api}/g/s/media/upload",
         data=data,
         headers=custom_headers,
         stream=True
     )
 
     cache[file_hash] = response.json()["mediaValue"]
     if len(cache) >= 32:
         cache.popitem(last=False)
 
-    return cache[file_hash]
+    return cache[file_hash]
+
```

### Comparing `amino.light.py-0.1.5/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.6/AminoLightPy/lib/util/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=too-many-lines
 from json import loads, JSONDecodeError
 
 class UnsupportedService(Exception):
     """
     - **API Code** : 100
     - **API Message** : Unsupported service. Your client may be out of date. Please update it to the latest version.
     - **API String** : ``Unknown String``
@@ -359,15 +360,15 @@
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 class InsufficientLevel(Exception):
     """
     - **API Code** : 551
-    - **API Message** : This post type is restricted to members with a level ``X`` ranking and above.
+    - **API Message** : This post type is restricted to members with a level ``X`` ranking.
     - **API String** : ``Unknown String``
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 class WallCommentingDisabled(Exception):
     """
@@ -870,87 +871,168 @@
         try:
             api_code = data["api:statuscode"]
         except KeyError as e:
             raise UnknownError(data) from e
     except JSONDecodeError:
         api_code = 403
 
-    if api_code == 100: raise UnsupportedService(data)
-    elif api_code == 102: raise FileTooLarge(data)
-    elif api_code == 103 or api_code == 104: raise InvalidRequest(data)
-    elif api_code == 105: raise InvalidSession(data)
-    elif api_code == 106: raise AccessDenied(data)
-    elif api_code == 107: raise UnexistentData(data)
-    elif api_code == 110: raise ActionNotAllowed(data)
-    elif api_code == 111: raise ServiceUnderMaintenance(data)
-    elif api_code == 113: raise MessageNeeded(data)
-    elif api_code == 200: raise InvalidAccountOrPassword(data)
-    elif api_code == 201: raise AccountDisabled(data)
-    elif api_code == 213: raise InvalidEmail(data)
-    elif api_code == 214: raise InvalidPassword(data)
-    elif api_code == 215: raise EmailAlreadyTaken(data) and UnsupportedEmail(data)
-    elif api_code == 216: raise AccountDoesntExist(data)
-    elif api_code == 218: raise InvalidDevice(data)
-    elif api_code == 219: raise AccountLimitReached(data) or TooManyRequests(data)
-    elif api_code == 221: raise CantFollowYourself(data)
-    elif api_code == 225: raise UserUnavailable(data)
-    elif api_code == 229: raise YouAreBanned(data)
-    elif api_code == 230: raise UserNotMemberOfCommunity(data)
-    elif api_code == 235: raise RequestRejected(data)
-    elif api_code == 238: raise ActivateAccount(data)
-    elif api_code == 239: raise CantLeaveCommunity(data)
-    elif api_code == 240: raise ReachedTitleLength(data)
-    elif api_code == 245: raise UserHasBeenDeleted(data)
-    elif api_code == 246: raise AccountDeleted(data)
-    elif api_code == 251: raise API_ERR_EMAIL_NO_PASSWORD(data)
-    elif api_code == 257: raise API_ERR_COMMUNITY_USER_CREATED_COMMUNITIES_VERIFY(data)
-    elif api_code == 262: raise ReachedMaxTitles(data)
-    elif api_code == 270: raise VerificationRequired(data)
-    elif api_code == 271: raise API_ERR_INVALID_AUTH_NEW_DEVICE_LINK(data)
-    elif api_code == 291: raise CommandCooldown(data)
-    elif api_code == 293: raise UserBannedByTeamAmino(data)
-    elif api_code == 300: raise BadImage(data)
-    elif api_code == 313: raise InvalidThemepack(data)
-    elif api_code == 314: raise InvalidVoiceNote(data)
-    elif api_code == 403: raise IpTemporaryBan(data)
-    elif api_code == 500 or api_code == 700 or api_code == 1600: raise RequestedNoLongerExists(data)
-    elif api_code == 503: raise PageRepostedTooRecently(data)
-    elif api_code == 551: raise InsufficientLevel(data)
-    elif api_code == 702: raise WallCommentingDisabled(data)
-    elif api_code == 801: raise CommunityNoLongerExists(data)
-    elif api_code == 802: raise InvalidCodeOrLink(data)
-    elif api_code == 805: raise CommunityNameAlreadyTaken(data)
-    elif api_code == 806: raise CommunityCreateLimitReached(data)
-    elif api_code == 814: raise CommunityDisabled(data)
-    elif api_code == 833: raise CommunityDeleted(data)
-    elif api_code == 1501: raise DuplicatePollOption(data)
-    elif api_code == 1507: raise ReachedMaxPollOptions(data)
-    elif api_code == 1602: raise TooManyChats(data)
-    elif api_code == 1605: raise ChatFull(data)
-    elif api_code == 1606: raise TooManyInviteUsers(data)
-    elif api_code == 1611: raise ChatInvitesDisabled(data)
-    elif api_code == 1612: raise RemovedFromChat(data)
-    elif api_code == 1613: raise UserNotJoined(data)
-    elif api_code == 1627: raise API_ERR_CHAT_VVCHAT_NO_MORE_REPUTATIONS(data)
-    elif api_code == 1637: raise MemberKickedByOrganizer(data)
-    elif api_code == 1661: raise LevelFiveRequiredToEnableProps(data)
-    elif api_code == 1663: raise ChatViewOnly(data)
-    elif api_code == 1664: raise ChatMessageTooBig(data)
-    elif api_code == 1900: raise InviteCodeNotFound(data)
-    elif api_code == 2001: raise AlreadyRequestedJoinCommunity(data)
-    elif api_code == 2501: raise API_ERR_PUSH_SERVER_LIMITATION_APART(data)
-    elif api_code == 2502: raise API_ERR_PUSH_SERVER_LIMITATION_COUNT(data)
-    elif api_code == 2503: raise API_ERR_PUSH_SERVER_LINK_NOT_IN_COMMUNITY(data)
-    elif api_code == 2504: raise API_ERR_PUSH_SERVER_LIMITATION_TIME(data)
-    elif api_code == 2601: raise AlreadyCheckedIn(data)
-    elif api_code == 2611: raise AlreadyUsedMonthlyRepair(data)
-    elif api_code == 2800: raise AccountAlreadyRestored(data)
-    elif api_code == 3102: raise IncorrectVerificationCode(data)
-    elif api_code == 3905: raise NotOwnerOfChatBubble(data)
-    elif api_code == 4300: raise NotEnoughCoins(data)
-    elif api_code == 4400: raise AlreadyPlayedLottery(data)
-    elif api_code == 4500 or api_code == 4501: raise CannotSendCoins(data)
-    elif api_code == 4805: raise FailedSubscribeFanClub(data)
-    elif api_code == 6001: raise AminoIDAlreadyChanged(data)
-    elif api_code == 6002: raise InvalidAminoID(data)
-    elif api_code == 9901: raise InvalidName(data)
-    else: raise Exception(data)
+    if api_code == 100:
+        raise UnsupportedService(data)
+    elif api_code == 102:
+        raise FileTooLarge(data)
+    elif api_code == 103 or api_code == 104:
+        raise InvalidRequest(data)
+    elif api_code == 105:
+        raise InvalidSession(data)
+    elif api_code == 106:
+        raise AccessDenied(data)
+    elif api_code == 107:
+        raise UnexistentData(data)
+    elif api_code == 110:
+        raise ActionNotAllowed(data)
+    elif api_code == 111:
+        raise ServiceUnderMaintenance(data)
+    elif api_code == 113:
+        raise MessageNeeded(data)
+    elif api_code == 200:
+        raise InvalidAccountOrPassword(data)
+    elif api_code == 201:
+        raise AccountDisabled(data)
+    elif api_code == 213:
+        raise InvalidEmail(data)
+    elif api_code == 214:
+        raise InvalidPassword(data)
+    elif api_code == 215:
+        raise EmailAlreadyTaken(data) and UnsupportedEmail(data)
+    elif api_code == 216:
+        raise AccountDoesntExist(data)
+    elif api_code == 218:
+        raise InvalidDevice(data)
+    elif api_code == 219:
+        raise AccountLimitReached(data) or TooManyRequests(data)
+    elif api_code == 221:
+        raise CantFollowYourself(data)
+    elif api_code == 225:
+        raise UserUnavailable(data)
+    elif api_code == 229:
+        raise YouAreBanned(data)
+    elif api_code == 230:
+        raise UserNotMemberOfCommunity(data)
+    elif api_code == 235:
+        raise RequestRejected(data)
+    elif api_code == 238:
+        raise ActivateAccount(data)
+    elif api_code == 239:
+        raise CantLeaveCommunity(data)
+    elif api_code == 240:
+        raise ReachedTitleLength(data)
+    elif api_code == 245:
+        raise UserHasBeenDeleted(data)
+    elif api_code == 246:
+        raise AccountDeleted(data)
+    elif api_code == 251:
+        raise API_ERR_EMAIL_NO_PASSWORD(data)
+    elif api_code == 257:
+        raise API_ERR_COMMUNITY_USER_CREATED_COMMUNITIES_VERIFY(data)
+    elif api_code == 262:
+        raise ReachedMaxTitles(data)
+    elif api_code == 270:
+        raise VerificationRequired(data)
+    elif api_code == 271:
+        raise API_ERR_INVALID_AUTH_NEW_DEVICE_LINK(data)
+    elif api_code == 291:
+        raise CommandCooldown(data)
+    elif api_code == 293:
+        raise UserBannedByTeamAmino(data)
+    elif api_code == 300:
+        raise BadImage(data)
+    elif api_code == 313:
+        raise InvalidThemepack(data)
+    elif api_code == 314:
+        raise InvalidVoiceNote(data)
+    elif api_code == 403:
+        raise IpTemporaryBan(data)
+    elif api_code == 500 or api_code == 700 or api_code == 1600:
+        raise RequestedNoLongerExists(data)
+    elif api_code == 503:
+        raise PageRepostedTooRecently(data)
+    elif api_code == 551:
+        raise InsufficientLevel(data)
+    elif api_code == 702:
+        raise WallCommentingDisabled(data)
+    elif api_code == 801:
+        raise CommunityNoLongerExists(data)
+    elif api_code == 802:
+        raise InvalidCodeOrLink(data)
+    elif api_code == 805:
+        raise CommunityNameAlreadyTaken(data)
+    elif api_code == 806:
+        raise CommunityCreateLimitReached(data)
+    elif api_code == 814:
+        raise CommunityDisabled(data)
+    elif api_code == 833:
+        raise CommunityDeleted(data)
+    elif api_code == 1501:
+        raise DuplicatePollOption(data)
+    elif api_code == 1507:
+        raise ReachedMaxPollOptions(data)
+    elif api_code == 1602:
+        raise TooManyChats(data)
+    elif api_code == 1605:
+        raise ChatFull(data)
+    elif api_code == 1606:
+        raise TooManyInviteUsers(data)
+    elif api_code == 1611:
+        raise ChatInvitesDisabled(data)
+    elif api_code == 1612:
+        raise RemovedFromChat(data)
+    elif api_code == 1613:
+        raise UserNotJoined(data)
+    elif api_code == 1627:
+        raise API_ERR_CHAT_VVCHAT_NO_MORE_REPUTATIONS(data)
+    elif api_code == 1637:
+        raise MemberKickedByOrganizer(data)
+    elif api_code == 1661:
+        raise LevelFiveRequiredToEnableProps(data)
+    elif api_code == 1663:
+        raise ChatViewOnly(data)
+    elif api_code == 1664:
+        raise ChatMessageTooBig(data)
+    elif api_code == 1900:
+        raise InviteCodeNotFound(data)
+    elif api_code == 2001:
+        raise AlreadyRequestedJoinCommunity(data)
+    elif api_code == 2501:
+        raise API_ERR_PUSH_SERVER_LIMITATION_APART(data)
+    elif api_code == 2502:
+        raise API_ERR_PUSH_SERVER_LIMITATION_COUNT(data)
+    elif api_code == 2503:
+        raise API_ERR_PUSH_SERVER_LINK_NOT_IN_COMMUNITY(data)
+    elif api_code == 2504:
+        raise API_ERR_PUSH_SERVER_LIMITATION_TIME(data)
+    elif api_code == 2601:
+        raise AlreadyCheckedIn(data)
+    elif api_code == 2611:
+        raise AlreadyUsedMonthlyRepair(data)
+    elif api_code == 2800:
+        raise AccountAlreadyRestored(data)
+    elif api_code == 3102:
+        raise IncorrectVerificationCode(data)
+    elif api_code == 3905:
+        raise NotOwnerOfChatBubble(data)
+    elif api_code == 4300:
+        raise NotEnoughCoins(data)
+    elif api_code == 4400:
+        raise AlreadyPlayedLottery(data)
+    elif api_code == 4500 or api_code == 4501:
+        raise CannotSendCoins(data)
+    elif api_code == 4805:
+        raise FailedSubscribeFanClub(data)
+    elif api_code == 6001:
+        raise AminoIDAlreadyChanged(data)
+    elif api_code == 6002:
+        raise InvalidAminoID(data)
+    elif api_code == 9901:
+        raise InvalidName(data)
+    else:
+        raise UnknownError(data)
+
```

### Comparing `amino.light.py-0.1.5/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.6/AminoLightPy/lib/util/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,55 @@
 from base64 import b64decode, b64encode
 
 PREFIX = b'\x19'
 SIG_KEY = b'\xdf\xa5\xed\x19-\xdan\x88\xa1/\xe1!0\xdcb\x06\xb1%\x1eD'
 DEVICE_KEY = b"\xe70\x9e\xcc\tS\xc6\xfa`\x00['e\xf9\x9d\xbb\xc9e\xc8\xe9"
 
 def gen_deviceId(data: bytes = None) -> str:
+    """
+    Generate a device ID using the provided data or random bytes.
+    """
     if isinstance(data, str):
         data = bytes(data, 'utf-8')
     identifier = PREFIX + (data or urandom(20))
     mac = new(DEVICE_KEY, identifier, sha1)
     return f"{identifier.hex()}{mac.hexdigest()}".upper()
 
 def signature(data: Union[str, bytes]) -> str:
+    """
+    Generate a signature for the given data.
+    """
     data = data if isinstance(data, bytes) else data.encode("utf-8")
     return b64encode(PREFIX + new(SIG_KEY, data, sha1).digest()).decode("utf-8")
 
 def update_deviceId(device: str) -> str:
+    """
+    Update a device ID using its hexadecimal representation.
+    """
     return gen_deviceId(bytes.fromhex(device[2:42]))
 
-def self_deviceId(email: str) -> str:
-    return gen_deviceId(sha1(email.encode()).digest())
+def self_deviceId(login: str) -> str:
+    """
+    Generate a device ID using the SHA1 hash of an login.
+    """
+    return gen_deviceId(sha1(login.encode()).digest())
 
 def decode_sid(sid: str) -> dict:
+    """
+    Decode a SID into a dictionary.
+    """
     sid = sid.replace("-", "+").replace("_", "/")
     sid += "=" * (-len(sid) % 4)
     decoded_bytes = b64decode(sid.encode())
     return loads(decoded_bytes[1:-20].decode())
 
 def sid_to_uid(SID: str) -> str:
+    """
+    Extract the user ID from a decoded SID.
+    """
     return decode_sid(SID)["2"]
 
 def sid_to_ip_address(SID: str) -> str:
-    return decode_sid(SID)["4"]
+    """
+    Extract the IP address from a decoded SID.
+    """
+    return decode_sid(SID)["4"]
```

### Comparing `amino.light.py-0.1.5/AminoLightPy/socket.py` & `amino.light.py-0.1.6/AminoLightPy/amino_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,96 @@
 # pylint: disable=invalid-name
+# pylint: disable=no-member
+
+import traceback
+import threading
 
 from json import loads, dumps
 from time import time, sleep
-from threading import Thread
 from websocket import WebSocketApp
 
-from .lib.util.objects import Event
+from .lib.util import objects
 from .lib.util.helpers import gen_deviceId, signature
 
 
 class SocketHandler:
     def __init__(self, client, debug=False):
-        self.socket_url = "wss://ws1.aminoapps.com"
+        self.socket_url = "ws://ws1.aminoapps.com"
         self.client = client
         self.debug = debug
-        self.active = False
-        self.headers = None
         self.socket = None
-        self.reconnectTime = 180
-
-        if self.socket_enabled:
-            self.reconnect_thread = Thread(target=self.reconnect_handler)
-            self.reconnect_thread.start()
-
-    def reconnect_handler(self):
-        while True:
-            sleep(self.reconnectTime)
-
-            if self.active:
-                self.debug_print("[socket][reconnect_handler] Reconnecting Socket")
-                self.close()
-                self.run_amino_socket()
+        self.thread_event = threading.Event()
 
-    def handle_message(self, ws, data):
+    def on_message(self, ws, data):
         self.client.handle_socket_message(data)
 
+    def is_connected(self):
+        return self.socket.sock and self.socket.sock.connected
+
     def send(self, data):
         self.debug_print(f"[socket][send] Sending Data : {data}")
 
-        if not self.socket_thread:
+        if not self.is_connected():
             self.run_amino_socket()
             sleep(5)
 
         self.socket.send(data)
 
+    def on_close(self, ws, data, status):
+        self.debug_print("[socket][reconnect_handler] Reconnecting Socket")
+        self.starting_process()
+
+    def on_error(self, ws, error):
+        traceback.print_exc()
+        print("On error: ", error)
+
+    def on_open(self, ws):
+        self.debug_print("[socket][start] Socket Started")
+        self.thread_event.set()
+
+    def starting_process(self):
+        deviceId = gen_deviceId()
+
+        final = f"{deviceId}|{int(time() * 1000)}"
+
+        headers = {
+            "NDCDEVICEID": deviceId,
+            "NDCAUTH": f"sid={self.client.sid}",
+            "NDC-MSG-SIG": signature(final)
+        }
+
+        self.socket = WebSocketApp(
+            f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
+            on_open=self.on_open,
+            on_error=self.on_error,
+            on_message=self.on_message,
+            on_close=self.on_close,
+            header=headers,
+        )
+
+        threading.Thread(target=self.socket.run_forever, kwargs={
+            "ping_interval": 10,
+            "ping_payload": '{"t": 116, "o": {"threadChannelUserInfoList": []}}'
+        }).start()
+
     def run_amino_socket(self):
-        try:
-            self.debug_print("[socket][start] Starting Socket")
+        if self.client.sid is None:
+            return
 
-            if self.client.sid is None:
-                return
-            
-            deviceId = gen_deviceId()
-
-            final = f"{deviceId}|{int(time() * 1000)}"
-
-            self.headers = {
-                "NDCDEVICEID": deviceId,
-                "NDCAUTH": f"sid={self.client.sid}",
-                "NDC-MSG-SIG": signature(final)
-            }
-
-            self.socket = WebSocketApp(
-                f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
-                on_message=self.handle_message,
-                header=self.headers
-            )
-
-            self.active = True
-            self.socket_thread = Thread(target=self.socket.run_forever)
-            self.socket_thread.start()
-
-            if self.reconnect_thread is None:
-                self.reconnect_thread = Thread(target=self.reconnect_handler)
-                self.reconnect_thread.start()
-
-            self.debug_print("[socket][start] Socket Started")
-        except Exception as e:
-            print(e)
-
-    def close(self):
-        self.debug_print("[socket][close] Closing Socket")
-
-        self.active = False
-        try:
-            self.socket.close()
-        except Exception as closeError:
-            self.debug_print(f"[socket][close] Error while closing Socket : {closeError}")
+        threading.Thread(target=self.starting_process).start()
+        self.thread_event.wait()
 
     def debug_print(self, message):
         if self.debug:
             print(message)
 
 
 class SocketRequests:
-    def __init__(self) -> None:
+    def __init__(self, client) -> None:
+        self.client = client
         self.active_live_chats = set()
 
     def join_voice_chat(self, comId: int, chatId: str, joinType: int = 1):
         """
         Joins a Voice Chat
         **Parameters**
             - **comId** : ID of the Community
@@ -112,15 +104,15 @@
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
             },
             "t": 112
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
     def join_video_chat(self, comId: int, chatId: str, joinType: int = 1):
         """
         Joins a Video Chat
         **Parameters**
             - **comId** : ID of the Community
             - **chatId** : ID of the Chat
@@ -134,102 +126,73 @@
                 "threadId": chatId,
                 "joinRole": joinType,
                 "channelType": 5,
             },
             "t": 108
         }
         data = dumps(data)
-        self.send(data)
-
-    def join_video_chat_as_viewer(self, comId: int, chatId: str):
-        data = {
-            "o":
-                {
-                    "ndcId": int(comId),
-                    "threadId": chatId,
-                    "joinRole": 2,
-                },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
 
     # Fixed by vedansh#4039
     def leave_from_live_chat(self, chatId: str):
         if chatId in self.active_live_chats:
             self.active_live_chats.remove(chatId)
 
  
     def run_vc(self, comId: int, chatId: str, joinType: str):
         while chatId in self.active_live_chats:
             try:
-                data = {
-                    "o": {
-                        "ndcId": int(comId),
-                        "threadId": chatId,
-                        "joinRole": joinType,
-                    },
-                    "t": 112
-                }
-                data = dumps(data)
-                self.send(data)
+                self.join_video_chat(
+                    comId=comId,
+                    chatId=chatId,
+                    joinType=joinType
+                )
                 sleep(60)
 
             except Exception as e:
                 print(e)
 
     def start_vc(self, comId: int, chatId: str, joinType: int = 1):
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-            },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
+        self.join_video_chat(
+            comId=comId,
+            chatId=chatId,
+            joinType=joinType
+        )
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "channelType": 1,
             },
             "t": 108
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
         self.active_live_chats.add(chatId)
-        Thread(target=self.run_vc, args=(comId, chatId, joinType)).start()
+        threading.Thread(target=self.run_vc, args=(comId, chatId, joinType)).start()
 
     def end_vc(self, comId: int, chatId: str, joinType: int = 2):
         self.leave_from_live_chat(chatId)
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-            },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
-        self.active_live_chats.remove(chatId)
+        self.join_video_chat(
+            comId=comId,
+            chatId=chatId,
+            joinType=joinType
+        )
 
     def Browsing(self, comId: int, blogId: str = None, blogType: int = 0):
         """
         Send Browsing Action
 
         **Paramaters**
             - **blogId**: 2 For Public 1 & 0 For Private (str)
             - **blogType**: Type Of the Blog *poll & blog & wiki* (int)
 
         **Return**
-            - **SetAction**:  (Class)
+            - None
         """
         if blogId and blogType:
             target = f"ndc://x{comId}/blog/"
         else:
             target = f"ndc://x{comId}/featured"
 
         data = {
@@ -238,25 +201,25 @@
                 "target": target,
                 "ndcId": int(comId),
                 "params": {"blogType": blogType},
             },
             "t": 306
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
     def Chatting(self, comId: int, chatId: str, threadType: int = 2):
         """
         Send Chatting Action
 
         **Paramaters**
             - **threadType**: 2 For Public 1 & 0 For Private (int)
 
         **Return**
-            - **SetAction**:  (Class)
+            - None
         """
         data = {
             "o": {
                 "actions": ["Chatting"],
                 "target": f"ndc://x{comId}/chat-thread/{chatId}",
                 "ndcId": int(comId),
                 "params": {
@@ -264,78 +227,96 @@
                     "membershipStatus": 1,
                     "threadType": threadType
                 },
             },
             "t": 306
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
     def PublicChats(self, comId: int,):
         """
         Send PublicChats Action
 
         **Return**
-            - **SetAction**:  (Class)
+            - None
         """
         data = {
             "o": {
                 "actions": ["Browsing"],
                 "target": f"ndc://x{comId}/public-chats",
                 "ndcId": int(comId),
                 "params": {"duration": 859},
             },
             "t": 306
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
     def LeaderBoards(self, comId: int,):
         """
         Send LeaderBoard Action
 
         **Return**
-            - **SetAction**:  (Class)
+            - None
         """
         data = {
             "o": {
                 "actions": ["Browsing"],
                 "target": f"ndc://x{comId}/leaderboards",
                 "ndcId": int(comId),
                 "params": {"duration": 859},
             },
             "t": 306
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
     def start_video_chat(self, comId: str, chatId: str, joinType: int = 1):
+        self.join_video_chat(
+            comId=comId,
+            chatId=chatId,
+            joinType=joinType
+        )
+
         data = {
             "o": {
-                "ndcId": comId,
+                "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
+                "channelType": 4,
             },
-            "t": 112
+            "t": 108
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
+    def typing_request(self, comId: int, chatId: str, stop: bool):
         data = {
             "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-                "channelType": 4,
+                "actions": ["Typing"],
+                "target": f"ndc://x{comId}/chat-thread/{chatId}",
+                "ndcId": comId,
             },
-            "t": 108
+            "t": 306 if stop else 304
         }
         data = dumps(data)
-        self.send(data)
+        self.client.send(data)
 
+    def recording_reqest(self, comId: int, chatId: str, stop: bool):
+        data = {
+            "o": {
+                "actions": ["Recording"],
+                "target": f"ndc://x{comId}/chat-thread/{chatId}",
+                "ndcId": comId,
+            },
+            "t": 306 if stop else 304
+        }
+        data = dumps(data)
+        self.client.send(data)
 
 class Callbacks:
     def __init__(self):
         self.handlers = {}
 
         self.methods = {
             304: self._resolve_chat_action_start,
@@ -426,15 +407,15 @@
                 self.handlers[type] = [handler]
             return handler
 
         return registerHandler
 
     def event_handler_decorator(func):
         def wrapper(self, data):
-            event = Event(data["o"]).Event
+            event = objects.Event(data["o"]).Event
             self.call(func.__name__, event)
         return wrapper
 
     @event_handler_decorator
     def on_text_message(self, data): pass
     @event_handler_decorator
     def on_image_message(self, data): pass
```

### Comparing `amino.light.py-0.1.5/LICENSE` & `amino.light.py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.5/PKG-INFO` & `amino.light.py-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -39,17 +39,18 @@
   <a href="#notes">Notes</a>
   <br>
   <a href="https://aminopy.readthedocs.io/en/latest/index.html" target="_blank">Documentation</a>
 </p>
 
 <h2 align="center">Features</h2>
 
-*  ⚡ **Optimization** : Most of the code has been rewritten.
+* ⚡ **Optimization** : Most of the code has been rewritten.
 * ⚙ **Backward compatibility** : Write code with correct syntax.
 * 🎮 **Commands support** : Go even further with new requests.
+* 🍎 **Supported on iPhones** : free, and without jailbreak.
 
 <h2 align="center">Usage</h2>
 
 Install the package :
 
 `pip install amino.light.py`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.5 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.6 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -15,15 +15,16 @@
          AminoApps python framework to create bots and scripts easily.
                         _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_D_o_c_s_]_[_l_i_c_e_n_c_e_]
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
-Go even further with new requests.
+Go even further with new requests. * ð **Supported on iPhones** : free, and
+without jailbreak.
                                ********** UUssaaggee **********
 Install the package : `pip install amino.light.py` --- Import the `Client` and
 `SubClient` objects into your bot's code, and create your own help manual :
 ```py from AminoLightPy import Client, SubClient # Your help message
 help_message = """ Welcome! This is help page. """ # Create Client object
 client = Client() # Login into account client.login("example_mail@gmail.com",
 "example_password") # And display the help ! @client.event("on_text_message")
```

### Comparing `amino.light.py-0.1.5/README.md` & `amino.light.py-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,18 @@
   <a href="#notes">Notes</a>
   <br>
   <a href="https://aminopy.readthedocs.io/en/latest/index.html" target="_blank">Documentation</a>
 </p>
 
 <h2 align="center">Features</h2>
 
-*  ⚡ **Optimization** : Most of the code has been rewritten.
+* ⚡ **Optimization** : Most of the code has been rewritten.
 * ⚙ **Backward compatibility** : Write code with correct syntax.
 * 🎮 **Commands support** : Go even further with new requests.
+* 🍎 **Supported on iPhones** : free, and without jailbreak.
 
 <h2 align="center">Usage</h2>
 
 Install the package :
 
 `pip install amino.light.py`
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
          AminoApps python framework to create bots and scripts easily.
                         _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_D_o_c_s_]_[_l_i_c_e_n_c_e_]
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
-Go even further with new requests.
+Go even further with new requests. * ð **Supported on iPhones** : free, and
+without jailbreak.
                                ********** UUssaaggee **********
 Install the package : `pip install amino.light.py` --- Import the `Client` and
 `SubClient` objects into your bot's code, and create your own help manual :
 ```py from AminoLightPy import Client, SubClient # Your help message
 help_message = """ Welcome! This is help page. """ # Create Client object
 client = Client() # Login into account client.login("example_mail@gmail.com",
 "example_password") # And display the help ! @client.event("on_text_message")
```

### Comparing `amino.light.py-0.1.5/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.1.6/amino.light.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -39,17 +39,18 @@
   <a href="#notes">Notes</a>
   <br>
   <a href="https://aminopy.readthedocs.io/en/latest/index.html" target="_blank">Documentation</a>
 </p>
 
 <h2 align="center">Features</h2>
 
-*  ⚡ **Optimization** : Most of the code has been rewritten.
+* ⚡ **Optimization** : Most of the code has been rewritten.
 * ⚙ **Backward compatibility** : Write code with correct syntax.
 * 🎮 **Commands support** : Go even further with new requests.
+* 🍎 **Supported on iPhones** : free, and without jailbreak.
 
 <h2 align="center">Usage</h2>
 
 Install the package :
 
 `pip install amino.light.py`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.5 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.6 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -15,15 +15,16 @@
          AminoApps python framework to create bots and scripts easily.
                         _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_D_o_c_s_]_[_l_i_c_e_n_c_e_]
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
-Go even further with new requests.
+Go even further with new requests. * ð **Supported on iPhones** : free, and
+without jailbreak.
                                ********** UUssaaggee **********
 Install the package : `pip install amino.light.py` --- Import the `Client` and
 `SubClient` objects into your bot's code, and create your own help manual :
 ```py from AminoLightPy import Client, SubClient # Your help message
 help_message = """ Welcome! This is help page. """ # Create Client object
 client = Client() # Login into account client.login("example_mail@gmail.com",
 "example_password") # And display the help ! @client.event("on_text_message")
```

### Comparing `amino.light.py-0.1.5/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.6/amino.light.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 AminoLightPy/__init__.py
 AminoLightPy/acm.py
+AminoLightPy/amino_socket.py
 AminoLightPy/client.py
 AminoLightPy/constants.py
-AminoLightPy/socket.py
+AminoLightPy/managers.py
 AminoLightPy/sub_client.py
 AminoLightPy/lib/__init__.py
 AminoLightPy/lib/util/__init__.py
 AminoLightPy/lib/util/exceptions.py
 AminoLightPy/lib/util/helpers.py
 AminoLightPy/lib/util/objects.py
 amino.light.py.egg-info/PKG-INFO
```

### Comparing `amino.light.py-0.1.5/setup.py` & `amino.light.py-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "augustlight",
     "aminolightpy",
     "amino.py"
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.5",
+    version="0.1.6",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

