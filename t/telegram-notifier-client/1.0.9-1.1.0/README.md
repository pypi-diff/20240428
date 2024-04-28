# Comparing `tmp/telegram_notifier_client-1.0.9.tar.gz` & `tmp/telegram_notifier_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_notifier_client-1.0.9.tar", last modified: Sat Apr 20 11:46:10 2024, max compression
+gzip compressed data, was "telegram_notifier_client-1.1.0.tar", last modified: Sun Apr 28 14:57:21 2024, max compression
```

## Comparing `telegram_notifier_client-1.0.9.tar` & `telegram_notifier_client-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/PKG-INFO
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.0.9/README.md
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-04-20 11:43:55.000000 telegram_notifier_client-1.0.9/pyproject.toml
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/setup.cfg
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-04-20 11:43:55.000000 telegram_notifier_client-1.0.9/setup.py
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.147796 telegram_notifier_client-1.0.9/src/
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.147796 telegram_notifier_client-1.0.9/src/notifier_client/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.0.9/src/notifier_client/__init__.py
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    18780 2024-04-20 11:05:45.000000 telegram_notifier_client-1.0.9/src/notifier_client/web_app_notifier_client.py
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/PKG-INFO
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/requires.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/top_level.txt
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.1.0/README.md
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-04-28 14:56:42.000000 telegram_notifier_client-1.1.0/pyproject.toml
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/setup.cfg
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-04-28 14:56:42.000000 telegram_notifier_client-1.1.0/setup.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.471851 telegram_notifier_client-1.1.0/src/
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.471851 telegram_notifier_client-1.1.0/src/notifier_client/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.1.0/src/notifier_client/__init__.py
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    19776 2024-04-28 07:31:16.000000 telegram_notifier_client-1.1.0/src/notifier_client/web_app_notifier_client.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/requires.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/top_level.txt
```

### Comparing `telegram_notifier_client-1.0.9/PKG-INFO` & `telegram_notifier_client-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_notifier_client
-Version: 1.0.9
+Version: 1.1.0
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
 Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
 Keywords: telegram notifier client
```

### Comparing `telegram_notifier_client-1.0.9/pyproject.toml` & `telegram_notifier_client-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "telegram_notifier_client"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="rorschach", email="rorschach45001@gmail.com" },
 ]
 description = "telegram_notifier_client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `telegram_notifier_client-1.0.9/src/notifier_client/web_app_notifier_client.py` & `telegram_notifier_client-1.1.0/src/notifier_client/web_app_notifier_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,55 @@
+import json
 import logging
 from dataclasses import dataclass
 from logging import Logger
 from typing import Tuple, Optional, Union, List
 
 import requests
 
 logger = logging.getLogger('telegram')
 
 
+def prepare_for_html(message: str):
+    return message.replace("<", "&lt;").replace(">", "&gt;")
+
+
 @dataclass
 class Message:
     page: int
     content: str
     emergency: str = ''
     amend: dict = None
 
     def message(self) -> str:
         if self.emergency:
-            self.emergency = self.emergency.replace("<", "&lt;").replace(">", "&gt;")
-        self.content = self.content.replace("<", "&lt;").replace(">", "&gt;")
+            self.emergency = prepare_for_html(self.emergency)
+        self.content = prepare_for_html(self.content)
         emergency = f"<b>Emergency Message</b><blockquote>{self.emergency}</blockquote>\n" if self.emergency else ""
         return f"<blockquote>{self.content}</blockquote>\n{emergency}<b>Page: {self.page}</b>\n"
 
 
 @dataclass
-class ErrorMessage:
+class PrettifiedMessage:
     title: str
     apm_reference: str
+    body: str = None
     amend: dict = None
     mentions: str = None
 
     def message(self):
-        self.title = self.title.replace("<", "&lt;").replace(">", "&gt;")
+        self.title = prepare_for_html(self.title)
         developers = f'\n👨‍💻    {self.mentions}' if self.mentions else ''
-        return (f'<blockquote>🔵 Message:    <code class="language-python">{self.title}</code>\n'
-                f'📊 APM Reference:   <code>{self.apm_reference}</code>'
-                f'{developers}</blockquote>\n')
+        self.body = prepare_for_html(f"{self.body[:200]}...") if self.body and (len(self.body) > 200) else self.body
+        self.body = f'\n<b>Body</b>\n<pre><code class="language-python">{self.body}</code></pre>\n' if self.body else ''
+
+        return (f'<blockquote>🔵 <b>Title:</b>    <code class="language-python">{self.title}</code>\n'
+                f'📊 <b>APM Reference:</b>   <code>{self.apm_reference}</code>'
+                f'{developers}</blockquote>\n'
+                f'{self.body}')
 
 
 class WebAppNotifierClient:
     def __init__(self, receiver_id: int, server_url: str, auth_token: str, topic_id: int = None):
         """
         Initializes a new instance of the WebAppNotifierClient.
         Parameters:
@@ -61,15 +71,15 @@
             - amend (dict, optional): Additional data to amend the alert message.
         Returns:
             - int: The HTTP status code of the response (200 indicates that the message has been queued).
         """
         return requests.post(
             url=self.server_url + '/send_alert',
             headers={'AuthToken': self.auth_token},
-            json=dict(receiver_id=self.receiver_id, text=message, topic_id=self.topic_id, amend=amend),
+            data=self.__json_serialize(receiver_id=self.receiver_id, text=message, topic_id=self.topic_id, amend=amend),
             timeout=5
         ).status_code
 
     def send_message(self, message: str, amend: dict = None) -> int:
         """
         Sends a regular message to the configured receiver.
 
@@ -79,15 +89,15 @@
 
         Returns:
             - int: The HTTP status code of the response (200 indicates that the message has been queued).
         """
         return requests.post(
             url=self.server_url + '/send_message',
             headers={'AuthToken': self.auth_token},
-            json=dict(receiver_id=self.receiver_id, text=message, topic_id=self.topic_id, amend=amend),
+            data=self.__json_serialize(receiver_id=self.receiver_id, text=message, topic_id=self.topic_id, amend=amend),
             timeout=5
         ).status_code
 
     def send_message_by_threshold(self, message: str, amend: dict = None) -> Tuple[int, bool]:
         """
         Sends a message to the configured receiver with threshold checks.
 
@@ -98,15 +108,15 @@
         Returns:
             - Tuple[int, bool]: A tuple containing the HTTP status code and a boolean indicating whether
                                 the message has been added to the queue.
         """
         response = requests.post(
             url=self.server_url + '/send_message_threshold',
             headers={'AuthToken': self.auth_token},
-            json=dict(receiver_id=self.receiver_id, text=message, topic_id=self.topic_id, amend=amend),
+            data=self.__json_serialize(receiver_id=self.receiver_id, text=message, topic_id=self.topic_id, amend=amend),
             timeout=5
         )
         if response.status_code != 200:
             return response.status_code, False
         return response.status_code, response.json()['sending']
 
     def set_threshold_setting(self,
@@ -124,55 +134,64 @@
 
         Returns:
             - int: The HTTP status code of the response.
         """
         return requests.post(
             url=self.server_url + '/set_sending_threshold',
             headers={'AuthToken': self.auth_token},
-            json=dict(
+            data=self.__json_serialize(
                 message=message,
                 sending_threshold_number=sending_threshold_number,
                 sending_threshold_time=sending_threshold_time
             ),
             timeout=5
         ).status_code
 
     def send_message_once(self,
                           title: str,
                           apm_reference: str,
                           amend: dict = None,
                           mentions: str = None,
-                          expire: int = None
+                          expire: int = None,
+                          body: str = None
                           ):
         """
         The send_message_once function is used to notify the user of an error.
 
         :param title: str: Set the title of the notification
         :param apm_reference: str: Reference of the message in the ElasticAPM dashboard
         :param amend: dict: Add additional information to the message
         :param mentions: tuple: List of the developers that should be mentioned in the message
-        :param expire: int: Expire time of the message that prevents from sending repeated message in seconds.
-        Default is 2 day. If sets to `0` the message will be sent immediately.
+        :param expire: int: Expire time of the message that prevents from sending a repeated message in seconds.
+         Default is 2 days. If sets to `0` the message will be sent immediately.
+        :param body: str: the body of the message.
+        The maximum acceptable length is 200 characters.`Three dots` will replace the rest of the message.
+
         :return: A status code of the request
         """
 
         return requests.post(
             url=self.server_url + '/send_message_once',
             headers={'AuthToken': self.auth_token},
-            json=dict(
+            data=self.__json_serialize(
                 title=title,
                 apm_reference=apm_reference,
                 receiver_id=self.receiver_id,
                 topic_id=self.topic_id,
                 amend=amend,
                 mentions=mentions,
-                expire=expire),
+                expire=expire,
+                body=body),
             timeout=5
         ).status_code
 
+    @staticmethod
+    def __json_serialize(**data):
+        return json.dumps(data, default=str)
+
 
 class SendNotification:
     def __init__(
             self,
             receiver_id: int,
             server_url: str,
             auth_token: str,
@@ -289,47 +308,51 @@
         )
 
     def send_message_once(self,
                           title: str,
                           apm_reference: str,
                           amend: dict = None,
                           mentions: tuple = None,
-                          expire: int = None) -> Optional[int]:
+                          expire: int = None,
+                          body=None) -> Optional[int]:
 
         """
         The send_message_once function is used to send message the user only once in a time.
 
         :param title: str: Specify the title of the message
         :param apm_reference: str: Reference of the message in the ElasticAPM dashboard
         :param amend: dict: Add additional information to the message
         :param mentions: tuple: List of the developers that should be mentioned in the message
-        :param expire: int: Expire time of the message that prevents from sending repeated message in seconds.
-        Default is 2 day. If sets to `0` the message will be sent immediately.
+        :param expire: int: Expire time of the message that prevents from sending a repeated message in seconds.
+        Default is 2 days. If sets to `0` the message will be sent immediately.
+        :param body: str: the body of the message.
+        The maximum acceptable length is 200 characters.`Three dots` will replace the rest of the message.
+
         :return: The status code of the request
         """
 
         if self.test_env:
             self.test_env_logger.info(f"{title}: {apm_reference}")
             return
 
         res = 0
         if mentions:
             mentions = " ".join(mentions)
 
         try:
             for _ in range(self.retiring_number):
                 res = self.notifier_client.send_message_once(title=title, apm_reference=apm_reference, amend=amend,
-                                                             mentions=mentions, expire=expire)
+                                                             mentions=mentions, expire=expire, body=body)
                 if self.__check_status(res):
                     return res
 
         except Exception as e:
             logger.exception(f'exception:{e}')
 
-        message = ErrorMessage(title=title, apm_reference=apm_reference, amend=amend, mentions=mentions)
+        message = PrettifiedMessage(title=title, apm_reference=apm_reference, amend=amend, mentions=mentions, body=body)
         self.__send_emergency_message(message.message(), message.amend)
         return res
 
     def __split_msg(self, message: str, amend: dict = None, emergency_msg: str = '') -> List[Message]:
         """
         Splits a given message into multiple parts if it exceeds a predefined size.
         The method ensures that the split messages include the emergency message and amendments, if provided.
@@ -411,15 +434,15 @@
             - retrying (int): The number of times to retry sending the message.
         Returns:
             - None
         """
         for _ in range(retrying):
             logger.info(f'{message}, {self.receiver_id}')
             url = f'https://api.telegram.org/bot{self.telegram_bot_token}/sendMessage'
-            amend = str(amend).replace("<", "&lt;").replace(">", "&gt;")
+            amend = prepare_for_html(json.dumps(amend, default=str, indent=4))
             data = {
                 'chat_id': self.receiver_id,
                 'text': f'<b>Message </b>\n{message}\n'
                         f'<b>Amend</b>\n<pre><code class="language-python">{amend}</code></pre>\n\n'
                         f'<b>#emergency</b>',
                 'disable_web_page_preview': True,
                 "parse_mode": "HTML"
```

### Comparing `telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/PKG-INFO` & `telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-notifier-client
-Version: 1.0.9
+Version: 1.1.0
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
 Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
 Keywords: telegram notifier client
```

