# Comparing `tmp/pymstodo-0.1.7.tar.gz` & `tmp/pymstodo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymstodo-0.1.7.tar", last modified: Sat Aug 19 21:05:37 2023, max compression
+gzip compressed data, was "pymstodo-0.1.8.tar", last modified: Sun Apr 28 20:10:47 2024, max compression
```

## Comparing `pymstodo-0.1.7.tar` & `pymstodo-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 21:05:37.373835 pymstodo-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-19 21:05:26.000000 pymstodo-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-19 21:05:37.373835 pymstodo-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-19 21:05:26.000000 pymstodo-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 21:05:37.369835 pymstodo-0.1.7/pymstodo/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-19 21:05:26.000000 pymstodo-0.1.7/pymstodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-08-19 21:05:26.000000 pymstodo-0.1.7/pymstodo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-19 21:05:26.000000 pymstodo-0.1.7/pymstodo/windows_zones_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-08-19 21:05:26.000000 pymstodo-0.1.7/pymstodo/windows_zones_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 21:05:37.369835 pymstodo-0.1.7/pymstodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-19 21:05:37.000000 pymstodo-0.1.7/pymstodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-19 21:05:37.000000 pymstodo-0.1.7/pymstodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 21:05:37.000000 pymstodo-0.1.7/pymstodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-19 21:05:37.000000 pymstodo-0.1.7/pymstodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-19 21:05:37.000000 pymstodo-0.1.7/pymstodo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-19 21:05:37.373835 pymstodo-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-19 21:05:26.000000 pymstodo-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:10:47.767568 pymstodo-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 20:10:41.000000 pymstodo-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-28 20:10:47.767568 pymstodo-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-28 20:10:41.000000 pymstodo-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:10:47.767568 pymstodo-0.1.8/pymstodo/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/windows_zones_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/windows_zones_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:10:47.767568 pymstodo-0.1.8/pymstodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:10:47.767568 pymstodo-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-28 20:10:41.000000 pymstodo-0.1.8/setup.py
```

### Comparing `pymstodo-0.1.7/LICENSE` & `pymstodo-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.7/PKG-INFO` & `pymstodo-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.7
+Version: 0.1.8
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Serhiy Shliapuhin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests_oauthlib>=1.3.0
+Requires-Dist: defusedxml>=0.7.1
 
 # pymstodo ✔️
 [![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://github.com/inbalboa/pymstodo/actions/workflows/main.yml/badge.svg)](https://github.com/inbalboa/pymstodo/actions/workflows/main.yml) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 ### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
 
 ## Installation
@@ -37,15 +39,16 @@
 from pymstodo import ToDoConnection
 
 client_id = 'PLACE YOUR CLIENT ID'
 client_secret = 'PLACE YOUR CLIENT SECRET'
 
 auth_url = ToDoConnection.get_auth_url(client_id)
 redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
-token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
+token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)  # you have to save it somewhere
+print(token)
 todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
 
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
```

### Comparing `pymstodo-0.1.7/README.md` & `pymstodo-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from pymstodo import ToDoConnection
 
 client_id = 'PLACE YOUR CLIENT ID'
 client_secret = 'PLACE YOUR CLIENT SECRET'
 
 auth_url = ToDoConnection.get_auth_url(client_id)
 redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
-token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
+token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)  # you have to save it somewhere
+print(token)
 todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
 
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
```

### Comparing `pymstodo-0.1.7/pymstodo/client.py` & `pymstodo-0.1.8/pymstodo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
     Args:
         client_id: API client ID
         client_secret: API client secret
         token: Token obtained by method `get_token`
     '''
     _redirect: str = 'https://localhost/login/authorized'
-    _scope: str = 'openid Tasks.ReadWrite'
+    _scope: str = 'openid Tasks.ReadWrite offline_access'
     _authority: str = 'https://login.microsoftonline.com/common'
     _authorize_endpoint: str = '/oauth2/v2.0/authorize'
     _token_endpoint: str = '/oauth2/v2.0/token'
     _base_api_url: str = 'https://graph.microsoft.com/v1.0/me/todo/'
 
     def __init__(self, client_id: str, client_secret: str, token: Token) -> None:
         self.client_id: str = client_id
@@ -274,15 +274,14 @@
     @staticmethod
     def get_token(client_id: str, client_secret: str, redirect_resp: str) -> Any:
         '''Fetch the access token'''
         oa_sess = OAuth2Session(client_id, scope=ToDoConnection._scope, redirect_uri=ToDoConnection._redirect)
         token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
         return oa_sess.fetch_token(token_url, client_secret=client_secret, authorization_response=redirect_resp)
 
-
     def _refresh_token(self) -> None:
         now = time.time()
         expire_time = self.token['expires_at'] - 300
         if now >= expire_time:
             token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
             oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope,
                                     token=self.token, redirect_uri=ToDoConnection._redirect)
@@ -306,15 +305,14 @@
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists?$top={limit}')
         if not resp.ok:
             raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())['value']
         return [TaskList(**list_data) for list_data in contents]
 
-
     def create_list(self, name: str) -> TaskList:
         '''Create a new task list
 
         Args:
             name: Title of the new task list
 
         Returns:
@@ -432,15 +430,14 @@
             resp_content = json.loads(resp.content.decode())
             url = resp_content.get('@odata.nextLink')
             contents.extend(resp_content['value'])
         if limit:
             contents = contents[:limit]
         return [Task(**task_data) for task_data in contents]
 
-
     def create_task(self, title: str, list_id: str, due_date: datetime | None = None, body_text: str | None = None) -> Task:
         '''Create a new task in a specified task list
 
         Args:
             title: A brief description of the task
             list_id: Unique identifier for the task list
             due_date: The date and time that the task is to be finished
@@ -540,8 +537,7 @@
 
         Returns:
             A completed task
 
         Raises:
             PymstodoError: An error occurred accessing the API'''
         return self.update_task(task_id, list_id, status='completed')
-
```

### Comparing `pymstodo-0.1.7/pymstodo/windows_zones_data.py` & `pymstodo-0.1.8/pymstodo/windows_zones_data.py`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.7/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.1.8/pymstodo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.7
+Version: 0.1.8
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Serhiy Shliapuhin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests_oauthlib>=1.3.0
+Requires-Dist: defusedxml>=0.7.1
 
 # pymstodo ✔️
 [![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://github.com/inbalboa/pymstodo/actions/workflows/main.yml/badge.svg)](https://github.com/inbalboa/pymstodo/actions/workflows/main.yml) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 ### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
 
 ## Installation
@@ -37,15 +39,16 @@
 from pymstodo import ToDoConnection
 
 client_id = 'PLACE YOUR CLIENT ID'
 client_secret = 'PLACE YOUR CLIENT SECRET'
 
 auth_url = ToDoConnection.get_auth_url(client_id)
 redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
-token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
+token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)  # you have to save it somewhere
+print(token)
 todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
 
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
```

### Comparing `pymstodo-0.1.7/setup.py` & `pymstodo-0.1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import setuptools
 
 
 def long_description():
     with Path('README.md').open() as ld:
         return ld.read()
 
+
 def find_requires():
     with Path('requirements.txt').open() as reqs:
         return reqs.readlines()
 
+
 def find_version():
     with Path('VERSION').open() as ver:
         return ver.readline().strip()
 
 
 setuptools.setup(
     name='pymstodo',
```

