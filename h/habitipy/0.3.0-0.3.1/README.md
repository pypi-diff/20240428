# Comparing `tmp/habitipy-0.3.0.tar.gz` & `tmp/habitipy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/habitipy-0.3.0.tar", last modified: Sun Jan 13 23:27:51 2019, max compression
+gzip compressed data, was "habitipy-0.3.1.tar", last modified: Sun Apr 28 13:39:50 2024, max compression
```

## Comparing `habitipy-0.3.0.tar` & `habitipy-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 delphi    (1000) users      (100)        0 2019-01-13 23:27:51.000000 habitipy-0.3.0/
--rw-r--r--   0 delphi    (1000) users      (100)      922 2019-01-13 23:27:51.000000 habitipy-0.3.0/PKG-INFO
--rw-r--r--   0 delphi    (1000) users      (100)     7320 2019-01-13 23:27:43.000000 habitipy-0.3.0/README.md
-drwxr-xr-x   0 delphi    (1000) users      (100)        0 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy/
--rw-r--r--   0 delphi    (1000) users      (100)      210 2017-08-04 09:51:10.000000 habitipy-0.3.0/habitipy/__init__.py
--rw-r--r--   0 delphi    (1000) users      (100)     2299 2018-07-24 16:27:37.000000 habitipy-0.3.0/habitipy/aio.py
--rw-r--r--   0 delphi    (1000) users      (100)    17417 2019-01-13 21:50:57.000000 habitipy-0.3.0/habitipy/api.py
--rw-r--r--   0 delphi    (1000) users      (100)    89252 2018-03-13 20:18:46.000000 habitipy-0.3.0/habitipy/apidoc.txt
--rw-r--r--   0 delphi    (1000) users      (100)    28979 2019-01-13 23:23:03.000000 habitipy-0.3.0/habitipy/cli.py
-drwxr-xr-x   0 delphi    (1000) users      (100)        0 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy/i18n/
-drwxr-xr-x   0 delphi    (1000) users      (100)        0 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy/i18n/ru/
-drwxr-xr-x   0 delphi    (1000) users      (100)        0 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy/i18n/ru/LC_MESSAGES/
--rw-r--r--   0 delphi    (1000) users      (100)    13321 2019-01-13 23:15:39.000000 habitipy-0.3.0/habitipy/i18n/ru/LC_MESSAGES/habitipy.mo
--rw-r--r--   0 delphi    (1000) users      (100)     4621 2019-01-13 21:49:16.000000 habitipy-0.3.0/habitipy/util.py
-drwxr-xr-x   0 delphi    (1000) users      (100)        0 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/
--rw-r--r--   0 delphi    (1000) users      (100)      922 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/PKG-INFO
--rw-r--r--   0 delphi    (1000) users      (100)      359 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/SOURCES.txt
--rw-r--r--   0 delphi    (1000) users      (100)        1 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/dependency_links.txt
--rw-r--r--   0 delphi    (1000) users      (100)       55 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/entry_points.txt
--rw-r--r--   0 delphi    (1000) users      (100)       47 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/requires.txt
--rw-r--r--   0 delphi    (1000) users      (100)        9 2019-01-13 23:27:51.000000 habitipy-0.3.0/habitipy.egg-info/top_level.txt
--rw-r--r--   0 delphi    (1000) users      (100)       38 2019-01-13 23:27:51.000000 habitipy-0.3.0/setup.cfg
--rw-r--r--   0 delphi    (1000) users      (100)     1516 2019-01-13 23:27:43.000000 habitipy-0.3.0/setup.py
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.797000 habitipy-0.3.1/
+-rw-r--r--   0 delphi    (1000) users      (100)     1078 2017-07-19 12:42:01.000000 habitipy-0.3.1/LICENSE.txt
+-rw-r--r--   0 delphi    (1000) users      (100)      859 2024-04-28 13:39:50.793666 habitipy-0.3.1/PKG-INFO
+-rw-r--r--   0 delphi    (1000) users      (100)     6933 2024-04-28 12:20:31.000000 habitipy-0.3.1/README.md
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.787000 habitipy-0.3.1/habitipy/
+-rw-r--r--   0 delphi    (1000) users      (100)      210 2017-08-04 09:51:10.000000 habitipy-0.3.1/habitipy/__init__.py
+-rw-r--r--   0 delphi    (1000) users      (100)     2273 2019-08-18 20:28:08.000000 habitipy-0.3.1/habitipy/aio.py
+-rw-r--r--   0 delphi    (1000) users      (100)    17470 2024-04-28 08:23:08.000000 habitipy-0.3.1/habitipy/api.py
+-rw-r--r--   0 delphi    (1000) users      (100)    89254 2024-04-28 07:43:12.000000 habitipy-0.3.1/habitipy/apidoc.txt
+-rw-r--r--   0 delphi    (1000) users      (100)    30317 2019-08-18 20:28:08.000000 habitipy-0.3.1/habitipy/cli.py
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.777000 habitipy-0.3.1/habitipy/i18n/
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.777000 habitipy-0.3.1/habitipy/i18n/ru/
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.790333 habitipy-0.3.1/habitipy/i18n/ru/LC_MESSAGES/
+-rw-r--r--   0 delphi    (1000) users      (100)    13350 2019-08-18 20:28:08.000000 habitipy-0.3.1/habitipy/i18n/ru/LC_MESSAGES/habitipy.mo
+-rw-r--r--   0 delphi    (1000) users      (100)     5107 2024-04-28 10:23:41.000000 habitipy-0.3.1/habitipy/util.py
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.790333 habitipy-0.3.1/habitipy.egg-info/
+-rw-r--r--   0 delphi    (1000) users      (100)      859 2024-04-28 13:39:50.000000 habitipy-0.3.1/habitipy.egg-info/PKG-INFO
+-rw-r--r--   0 delphi    (1000) users      (100)      450 2024-04-28 13:39:50.000000 habitipy-0.3.1/habitipy.egg-info/SOURCES.txt
+-rw-r--r--   0 delphi    (1000) users      (100)        1 2024-04-28 13:39:50.000000 habitipy-0.3.1/habitipy.egg-info/dependency_links.txt
+-rw-r--r--   0 delphi    (1000) users      (100)       54 2024-04-28 13:39:50.000000 habitipy-0.3.1/habitipy.egg-info/entry_points.txt
+-rw-r--r--   0 delphi    (1000) users      (100)       58 2024-04-28 13:39:50.000000 habitipy-0.3.1/habitipy.egg-info/requires.txt
+-rw-r--r--   0 delphi    (1000) users      (100)        9 2024-04-28 13:39:50.000000 habitipy-0.3.1/habitipy.egg-info/top_level.txt
+-rw-r--r--   0 delphi    (1000) users      (100)       38 2024-04-28 13:39:50.797000 habitipy-0.3.1/setup.cfg
+-rw-r--r--   0 delphi    (1000) users      (100)     1485 2024-04-28 12:20:31.000000 habitipy-0.3.1/setup.py
+drwxr-xr-x   0 delphi    (1000) users      (100)        0 2024-04-28 13:39:50.793666 habitipy-0.3.1/tests/
+-rw-r--r--   0 delphi    (1000) users      (100)     4949 2018-11-12 20:40:42.000000 habitipy-0.3.1/tests/test_api.py
+-rw-r--r--   0 delphi    (1000) users      (100)     9509 2019-08-18 20:28:08.000000 habitipy-0.3.1/tests/test_cli.py
+-rw-r--r--   0 delphi    (1000) users      (100)     3431 2017-08-20 14:52:04.000000 habitipy-0.3.1/tests/test_habitipy.py
+-rw-r--r--   0 delphi    (1000) users      (100)     2121 2017-08-22 09:21:08.000000 habitipy-0.3.1/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `habitipy-0.3.0/PKG-INFO` & `habitipy-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: habitipy
-Version: 0.3.0
+Version: 0.3.1
 Summary: tools and library for Habitica restful API (http://habitica.com)
 Home-page: https://github.com/ASMfreaK/habitipy
 Author: Pavel Pletenev
 Author-email: cpp.create@gmail.com
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Internet
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
-Provides-Extra: aio
 Provides-Extra: emoji
+Provides-Extra: aio
+License-File: LICENSE.txt
```

### Comparing `habitipy-0.3.0/README.md` & `habitipy-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 1. Python wrapper for the RESTful Habitica API (`habitica.api.Habitipy` class)
 2. Command-line interface with subcommands (e.g. `> habitipy todos`)
 
 | Version | CI | Coverage |
 | ---- | ---- | ----- |
 | Master |  [![Build Status](https://api.travis-ci.org/ASMfreaK/habitipy.svg?branch=master)](https://travis-ci.org/ASMfreaK/habitipy) | [![Codecov](https://img.shields.io/codecov/c/github/ASMfreaK/habitipy.svg)](https://codecov.io/gh/ASMfreaK/habitipy)  |
-| Stable (v0.3.0) | [![Build Status](https://api.travis-ci.org/ASMfreaK/habitipy.svg?branch=v0.3.0)](https://travis-ci.org/ASMfreaK/habitipy)|  |
+| Stable (v0.3.1) | [![Build Status](https://api.travis-ci.org/ASMfreaK/habitipy.svg?branch=v0.3.1)](https://travis-ci.org/ASMfreaK/habitipy)|  |
 
 Features
 --------
 
 * Access to your Habitica account from command line
 * Colorful output
 * Easy and intuitive subcommands syntax
@@ -115,28 +115,16 @@
 The `super().main()` line is critical - all initialization takes place here.
 
 
 I18N
 ----
 `habitipy` command is meant to be internationalized. It is done using Python's standard library's `gettext` module. If you want `habitipy` to be translated to your language please read [contributing guidelines](./CONTRIBUTING.md).
 
-Shell completion
-----------------
-
-Thanks to [mohsend](https://github.com/mohsend), habitica now has shell completion! Basically, you'll want to add the following to your `~/.profile`:
-
-    if [ -f PATH_TO_SITE_PACKAGES/habitica/shell_completion.sh ]; then
-        . PATH_TO_SITE_PACKAGES/habitica/shell_completion.sh
-    fi
-
-You can find your site-packages path with `python -c 'import habitica; print
-habitica.__path__[0]'`.
-
 Thanks
 ------
 
 Many thanks to the following excellent projects:
 
-- [plumbum]()
+- [plumbum](https://plumbum.readthedocs.io/en/latest/)
 - [requests](https://github.com/kennethreitz/requests)
 
 And to the original author of [habitica]https://github.com/philadams/habitica).
```

### Comparing `habitipy-0.3.0/habitipy/aio.py` & `habitipy-0.3.1/habitipy/aio.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,10 +60,9 @@
                 Got return code {res.status}, but {node.retcode} was
                 expected for {node.uri}. It may be a typo in Habitica apiDoc.
                 Please file an issue to https://github.com/HabitRPG/habitica/issues""")
                 msg = textwrap.dedent(msg)
                 msg = msg.replace('\n', ' ').format(res=resp, node=self._node)
                 if self._strict:
                     raise WrongReturnCode(msg)
-                else:
-                    warnings.warn(msg)
+                warnings.warn(msg)
             return (await resp.json())['data']
```

### Comparing `habitipy-0.3.0/habitipy/api.py` & `habitipy-0.3.1/habitipy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,17 @@
             for part in api.parted_uri:
                 if cur_node.can_into(part):
                     _node = cur_node.into(part)
                 else:
                     try:
                         _node = cur_node.place(part, ApiNode())
                     except ParamAlreadyExist:
-                        warnings.warn('Ignoring conflicting param. Don\'t use {}'.format(api.uri))
+                        warnings.warn(
+                            'Ignoring conflicting param. Don\'t use {}'.format(  # noqa: Q00
+                                api.uri))
                         _node = cur_node.param
                 cur_node = _node  # type: ignore
                 prev_part += '/' + part
             cur_node.place(api.method, api)
         return node
 
     def _make_headers(self):
@@ -272,16 +274,15 @@
             Got return code {res.status_code}, but {node.retcode} was
             expected for {node.uri}. It may be a typo in Habitica apiDoc.
             Please file an issue to https://github.com/HabitRPG/habitica/issues""")
             msg = textwrap.dedent(msg)
             msg = msg.replace('\n', ' ').format(res=res, node=self._node)
             if self._strict:
                 raise WrongReturnCode(msg)
-            else:
-                warnings.warn(msg)
+            warnings.warn(msg)
         return res.json()['data']
 
     def __call__(self, **kwargs) -> Union[Dict, List]:
         return self._request(*self._prepare_request(**kwargs))
 
 
 def download_api(branch=None) -> str:
```

### Comparing `habitipy-0.3.0/habitipy/apidoc.txt` & `habitipy-0.3.1/habitipy/apidoc.txt`

 * *Files 0% similar despite different names*

```diff
@@ -942,15 +942,15 @@
 @apiError (400) {BadRequest} Text-ValidationFailed Path 'text' is required.
 @apiError (400) {BadRequest} Alias-ValidationFailed Task short names can only contain alphanumeric characters, underscores and dashes.
 @apiError (400) {BadRequest} Value-ValidationFailed `x` is not a valid enum value for path `(body param)`.
 @apiError (401) {NotAuthorized} There is no account that uses those credentials.
 @api {get} /api/v3/tasks/user Get a user's tasks
 @apiName GetUserTasks
 @apiGroup Task
-@apiParam (Query) {String="habits","dailys","todos","rewards","completedTodos"} type Optional query parameter to return just a type of tasks. By default all types will be returned except completed todos that must be requested separately. The "completedTodos" type returns only the 30 most recently completed.
+@apiParam (Query) {String="habits","dailys","todos","rewards","completedTodos"} [type] Optional query parameter to return just a type of tasks. By default all types will be returned except completed todos that must be requested separately. The "completedTodos" type returns only the 30 most recently completed.
 @apiSuccess {Array} data An array of tasks
 @apiSuccessExample
 @apiError (BadRequest) Invalid_request_parameters Error returned if the type URL param was not correct.
 @apiError (401) {NotAuthorized} There is no account that uses those credentials.
 @api {get} /api/v3/tasks/challenge/:challengeId Get a challenge's tasks
 @apiName GetChallengeTasks
 @apiGroup Task
```

### Comparing `habitipy-0.3.0/habitipy/cli.py` & `habitipy-0.3.1/habitipy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # pylint: disable=invalid-name, logging-format-interpolation,too-few-public-methods
 import warnings
 import logging
 import os
 import json
 import uuid
 from bisect import bisect
+from collections.abc import Mapping
+from itertools import chain
 from textwrap import dedent
 from typing import List, Union, Dict, Any  # pylint: disable=unused-import
 import pkg_resources
 from plumbum import local, cli, colors
 import requests
 from .api import Habitipy
 from .util import assert_secure_file, secure_filestore
@@ -119,53 +121,99 @@
         if self.verbose:
             self.log.setLevel(logging.DEBUG)
         else:
             base_level = logging.INFO
             self.log.setLevel(base_level + 10 * self.silence_level)
 
 
-def get_content(api, rebuild_cache=False):
-    """get content from server or cache"""
-    if hasattr(get_content, 'cache') and not rebuild_cache:
-        return get_content.cache
-    if not os.path.exists(CONTENT_JSON) or rebuild_cache:
-        import locale
-        content_endpoint = api.content.get
-        # pylint: disable=protected-access
-        try_langs = []
+class Content(Mapping):
+    """Caching class for Habitica content data"""
+    _cache = None
+
+    def __init__(self, api, rebuild_cache=False, path=None):
+        self._api = api
+        self._path = []
+        self._rebuild_cache = rebuild_cache
+        self._path = path
+        self._obj = None
+        self._resolve_path()
+
+    def __getitem__(self, i):
+        try:
+            ret = self._obj[i]
+            if isinstance(ret, (list, dict)):
+                return Content(self._api, self._rebuild_cache, [*self._path, i])
+            return ret
+        except (KeyError, IndexError):
+            if self._rebuild_cache:
+                raise
+            self._rebuild_cache = True
+            self._resolve_path()
+            return self.__getitem__(i)
+
+    def __iter__(self):
+        if self._obj:
+            yield from iter(self._obj)
+
+    def __len__(self):
+        if self._obj:
+            return len(self._obj)
+        return 0
+
+    def _resolve_path(self):
+        if self._path is None:
+            self._path = []
+        self._obj = self._get()
+        for e in self._path:
+            self._obj = self._obj[e]
+
+    def _get(self):
+        """get content from server or cache"""
+        if Content._cache and not self._rebuild_cache:
+            return Content._cache
+        if not os.path.exists(CONTENT_JSON) or self._rebuild_cache:
+            content_endpoint = self._api.content.get
+            # pylint: disable=protected-access
+            server_lang = content_endpoint._node.params['query']['language']
+            Content._cache = content_endpoint(**next((
+                {'language': lang}
+                for lang in chain(
+                    Content._lang_from_translation(),
+                    Content._lang_from_locale())
+                if lang in server_lang.possible_values
+            ), {}))  # default
+            with open(CONTENT_JSON, 'w') as f:
+                json.dump(Content._cache, f)
+            return Content._cache
         try:
-            lang = get_translation_for('habitipy').info()['language']
-            try_langs.append(lang)
+            with open(CONTENT_JSON) as f:
+                Content._cache = json.load(f)
+            return Content._cache
+        except JSONDecodeError:
+            self._rebuild_cache = True
+            return self._get()
+
+    @staticmethod
+    def _lang_from_translation():
+        try:
+            yield get_translation_for('habitipy').info()['language']
         except KeyError:
             pass
+
+    @staticmethod
+    def _lang_from_locale():
+        import locale
         try:
             loc = locale.getdefaultlocale()[0]
             if loc:
-                try_langs.append(loc)
-                try_langs.append(loc[:2])
+                # handle something like 'ru_RU' not available - only 'ru'
+                yield loc
+                yield loc[:2]
         except IndexError:
             pass
-        server_lang = content_endpoint._node.params['query']['language']
-        # handle something like 'ru_RU' not available - only 'ru'
-        for lang in try_langs:
-            if lang in server_lang.possible_values:
-                loc = {'language': lang}
-                break
-        else:
-            loc = {}
-        get_content.cache = content = content_endpoint(**loc)
-        with open(CONTENT_JSON, 'w') as f:
-            json.dump(content, f)
-        return content
-    try:
-        with open(CONTENT_JSON) as f:
-            get_content.cache = content = json.load(f)
-        return content
-    except JSONDecodeError:
-        return get_content(api, rebuild_cache=True)
 
 
 class ApplicationWithApi(ConfiguredApplication):
     """Application with configured Habitica API"""
     api = None  # type: Habitipy
 
     def main(self):
@@ -190,15 +238,15 @@
     def main(self):
         super().main()
         user = self.api.user.get()
         for key in ['hp', 'mp', 'exp']:
             user['stats'][key] = round(user['stats'][key])
         user['stats']['class'] = _(user['stats']['class']).capitalize()
         user['food'] = sum(user['items']['food'].values())
-        content = get_content(self.api)
+        content = Content(self.api)
         user['pet'] = user['items']['currentPet'] if 'currentPet' in user['items'] else None
         user['pet'] = content['petInfo'][user['pet']]['text'] if user['pet'] else ''
         user['pet'] = _("Pet: ") + user['pet'] if user['pet'] else _("No pet")  # noqa: Q000
         user['mount'] = user['items'].get('currentMount', None)
         user['mount'] = content['mountInfo'][user['mount']]['text'] if user['mount'] else ''
         if user['mount']:
             user['mount'] = _("Mount: ") + user['mount']  # noqa: Q000
@@ -225,15 +273,15 @@
 
     def quest_info(self, user):
         """Get current quest info or return None"""
         key = user['party']['quest'].get('key', None)
         if '_id' not in user['party'] or key is None:
             return None
         for refresh in False, True:
-            content = get_content(self.api, refresh)
+            content = Content(self.api, refresh)
             quest = content['quests'].get(key, None)
             if quest:
                 break
         else:
             self.log.warning(dedent(_(
                 """Quest {} not found in Habitica's content.
                 Please file an issue to https://github.com/ASMfreaK/habitipy/issues
@@ -360,15 +408,15 @@
             ) if todo['checklist'] else ''
         res = _("{1}{0}{text}{2}").format(check, score, checklist, **todo)  # noqa: Q000
         return res
 
 
 def get_additional_rewards(api):
     """returns list of non-user rewards (potion, armoire, gear)"""
-    c = get_content(api)
+    c = Content(api)
     tasks = [c[i] for i in ['potion', 'armoire']]
     tasks.extend(api.user.inventory.buy.get())
     for task in tasks:
         task['id'] = task['alias'] = task['key']
     return tasks
 
 
@@ -716,15 +764,15 @@
 class Spells(ApplicationWithApi):
     DESCRIPTION = _("Prints all available spells")  # noqa: Q000
     def main(self):
         if self.nested_command:
             return
         super().main()
         user = self.api.user.get()
-        content = get_content(self.api)
+        content = Content(self.api)
         user_level = user['stats']['lvl']
         if user_level < 10:
             print(_("Your level is too low. Come back on level 10 or higher"))  # noqa: Q000
         user_class = user['stats']['class']
         user_spells = [
             v for k, v in content['spells'][user_class].items()
             if user_level > v['lvl']
```

### Comparing `habitipy-0.3.0/habitipy/i18n/ru/LC_MESSAGES/habitipy.mo` & `habitipy-0.3.1/habitipy/i18n/ru/LC_MESSAGES/habitipy.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-01-14 00:57+0200\n"
+"POT-Creation-Date: 2019-08-18 21:57+0300\n"
 "PO-Revision-Date: 2018-03-13 22:41+0200\n"
 "Last-Translator: cpp.create@gmail.com\n"
 "Language-Team: Russian\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -108,14 +108,15 @@
 "Уровень {stats[lvl]} {stats[class]}\n"
 
 msgid "({food} food item)"
 msgid_plural "({food} food items)"
 msgstr[0] "({food} единица еды)"
 msgstr[1] "({food} единицы еды)"
 msgstr[2] "({food} единиц еды)"
+msgstr[3] "({food} единиц еды)"
 
 msgid "Add a habit <habit>"
 msgstr "Добавить привычку <habit>"
 
 msgid "Add a reward <reward>"
 msgstr "Добавить награду <reward>"
```

### Comparing `habitipy-0.3.0/habitipy/util.py` & `habitipy-0.3.1/habitipy/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,36 @@
 # pylint: disable=invalid-name,bad-whitespace
 import os
 import gettext
 from contextlib import contextmanager
 from functools import partial
 from textwrap import dedent
 import re
+from math import ceil
 from typing import Tuple
 # import logging
 import pkg_resources
 from plumbum import colors
 try:
     from emoji import emojize
 except ImportError:
     emojize = None  # type: ignore
 
 
-def progressed_bar(count, total=100, status=None, suffix=None, bar_len=10):
+def progressed_bar(
+        count,
+        total=100, status=None, suffix=None,
+        width=None, bar_len=10):
     """render a progressed.io like progress bar"""
     status = status or ''
     suffix = suffix or '%'
     assert isinstance(count, int)
+    max_width = 60 if status == '' else 90
+    width = max_width if width is None else width
+    bar_len = ceil(bar_len * width / max_width)
     count_normalized = count if count <= total else total
     filled_len = int(round(bar_len * count_normalized / float(total)))
     percents = 100.0 * count / float(total)
     color = '#5cb85c'
     if percents < 30.0:
         color = '#d9534f'
     if percents < 70.0:
@@ -41,35 +48,39 @@
     progressbar += (text_color | (str(count) + suffix))
     return progressbar
 
 
 _progressed_regex_str = r"""
 !
 \[[^]]*\]
-\(\s*http://progressed\.io/bar/(?P<progress>[0-9]{1,3})
+\(\s*(http://progressed\.io/bar|https://progress-bar.dev)/(?P<progress>[0-9]{1,3})/?
 (
 \?((
-(title=(?P<title>[^&) "]*))|
-(scale=(?P<scale>[^&) "]*))|
-(suffix=(?P<suffix>[^&) "]*))
+(title=(?P<title>[^&) "]*))
+|(scale=(?P<scale>[^&) "]*))
+|(suffix=(?P<suffix>[^&) "]*))
+|(width=(?P<width>[^&) "]*))
 )&*)*
 ){0,1}
 \s*("[^"]*")*\)
 """
 _progressed_regex = re.compile(_progressed_regex_str, re.VERBOSE)
 
 
 def _progressed_match(m, bar_len=10):
     progress = m['progress']
     scale = m['scale']
+    width = m['width']
     progress = int(progress) if progress is not None else 0
     scale = int(scale) if scale is not None else 100
+    width = int(width)  if width is not None else 100
     return progressed_bar(
         progress, total=scale,
         status=m['title'], suffix=m['suffix'],
+        width=width,
         bar_len=bar_len)
 
 
 def progressed(string):
     """
     helper function to replace all links to progressed.io with progress bars
 
@@ -95,16 +106,20 @@
     from habitipy.util import prettify
     print(prettify('Write thesis :book: ![progress](http://progressed.io/bar/0 "progress")'))
     ```
     ```
     Write thesis 📖 ██████████0%
     ```
     """
-    string = emojize(string, use_aliases=True) if emojize else string
-    string = progressed(string)
+    try:
+        string = emojize(string, language="alias") if emojize else string
+        string = progressed(string)
+    except Exception as error:
+        warnings.warn('Failed to prettify string: {}'.format(error))
+        pass
     return string
 
 
 @contextmanager
 def umask(mask):
     """
     temporarily change umask
```

### Comparing `habitipy-0.3.0/habitipy.egg-info/PKG-INFO` & `habitipy-0.3.1/habitipy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: habitipy
-Version: 0.3.0
+Version: 0.3.1
 Summary: tools and library for Habitica restful API (http://habitica.com)
 Home-page: https://github.com/ASMfreaK/habitipy
 Author: Pavel Pletenev
 Author-email: cpp.create@gmail.com
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Internet
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
-Provides-Extra: aio
 Provides-Extra: emoji
+Provides-Extra: aio
+License-File: LICENSE.txt
```

### Comparing `habitipy-0.3.0/setup.py` & `habitipy-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ habitipy - tools and library for Habitica restful API"""
 import sys
 from setuptools import setup
 
 INSTALL_REQUIRES = [
     'plumbum',
     'requests',
+    'setuptools',
 ]
 if sys.version_info < (3, 5):
     INSTALL_REQUIRES.append('typing')
 
 setup(
     name='habitipy',
-    version='0.3.0',
+    version='0.3.1',
     author='Pavel Pletenev',
     author_email='cpp.create@gmail.com',
     url='https://github.com/ASMfreaK/habitipy',
     license='MIT',
     description='tools and library for Habitica restful API (http://habitica.com)',
     packages=['habitipy'],
     install_requires=INSTALL_REQUIRES,
@@ -34,15 +35,14 @@
     extras_require={
         'emoji':  ['emoji'],
         'aio':  ['aiohttp']
     },
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Utilities',
         'Topic :: Games/Entertainment',
         'Topic :: Internet',
         'Environment :: Console',
```

