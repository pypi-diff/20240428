# Comparing `tmp/that_depends-1.6.4.tar.gz` & `tmp/that_depends-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.6.4.tar", max compression
+gzip compressed data, was "that_depends-1.6.5.tar", max compression
```

## Comparing `that_depends-1.6.4.tar` & `that_depends-1.6.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.6.4/LICENSE
--rw-r--r--   0        0        0     7268 2024-04-21 16:47:48.481078 that_depends-1.6.4/README.md
--rw-r--r--   0        0        0     1482 2024-04-22 06:16:56.585595 that_depends-1.6.4/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.4/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.4/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.4/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-04-22 06:16:04.333831 that_depends-1.6.4/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.4/that_depends/providers/base.py
--rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.4/that_depends/providers/collections.py
--rw-r--r--   0        0        0     3525 2024-04-22 06:16:01.502161 that_depends-1.6.4/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.4/that_depends/providers/factories.py
--rw-r--r--   0        0        0     2948 2024-04-21 21:10:28.406639 that_depends-1.6.4/that_depends/providers/resources.py
--rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.4/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.4/that_depends/py.typed
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 that_depends-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.6.5/LICENSE
+-rw-r--r--   0        0        0     7277 2024-04-28 07:52:26.184942 that_depends-1.6.5/README.md
+-rw-r--r--   0        0        0     1482 2024-04-28 10:06:28.387006 that_depends-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.5/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.5/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.5/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-04-22 06:16:04.333831 that_depends-1.6.5/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.5/that_depends/providers/base.py
+-rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.5/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     3792 2024-04-28 07:52:26.186980 that_depends-1.6.5/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.5/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     2948 2024-04-21 21:10:28.406639 that_depends-1.6.5/that_depends/providers/resources.py
+-rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.5/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.5/that_depends/py.typed
+-rw-r--r--   0        0        0     7757 1970-01-01 00:00:00.000000 that_depends-1.6.5/PKG-INFO
```

### Comparing `that_depends-1.6.4/LICENSE` & `that_depends-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/README.md` & `that_depends-1.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 ```python
 import datetime
 
 from that_depends import BaseContainer, providers
 
 
 async def async_factory() -> datetime.datetime:
-    return datetime.datetime.now(tz=datetime.UTC)
+    return datetime.datetime.now(tz=datetime.timezone.utc)
 
 
 class DIContainer(BaseContainer):
     async_factory = providers.Factory(async_factory)
 ```
 ### List
 - List provider contains other providers.
```

### Comparing `that_depends-1.6.4/pyproject.toml` & `that_depends-1.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.6.4"
+version = "1.6.5"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
@@ -20,22 +20,22 @@
 pytest-asyncio = "*"
 pytest-cov = "*"
 ruff = "*"
 mypy = "*"
 typing-extensions = "*"
 
 [tool.mypy]
-python_version = "3.12"
+python_version = "3.10"
 strict = true
 
 [tool.ruff]
 fix = true
 unsafe-fixes = true
 line-length = 120
-target-version = "py312"
+target-version = "py310"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D1", # allow missing docstrings
     "S101", # allow asserts
     "TCH", # ignore flake8-type-checking
```

### Comparing `that_depends-1.6.4/that_depends/container.py` & `that_depends-1.6.5/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/that_depends/injection.py` & `that_depends-1.6.5/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/that_depends/providers/__init__.py` & `that_depends-1.6.5/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/that_depends/providers/base.py` & `that_depends-1.6.5/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/that_depends/providers/context_resources.py` & `that_depends-1.6.5/that_depends/providers/context_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
 import contextlib
 import inspect
+import logging
 import typing
 import uuid
 from contextvars import ContextVar
 
 from that_depends.providers.base import AbstractProvider, AbstractResource
 from that_depends.providers.resources import AsyncResource, Resource
 
 
 T = typing.TypeVar("T")
 P = typing.ParamSpec("P")
 context: ContextVar[dict[str, AbstractResource[typing.Any]]] = ContextVar("context")
+logger = logging.getLogger(__name__)
 
 AppType = typing.TypeVar("AppType")
 Scope = typing.MutableMapping[str, typing.Any]
 Message = typing.MutableMapping[str, typing.Any]
 Receive = typing.Callable[[], typing.Awaitable[Message]]
 Send = typing.Callable[[Message], typing.Awaitable[None]]
 ASGIApp = typing.Callable[[Scope, Receive, Send], typing.Awaitable[None]]
@@ -23,15 +25,20 @@
 
 @contextlib.asynccontextmanager
 async def container_context() -> typing.AsyncIterator[None]:
     token = context.set({})
     try:
         yield
     finally:
-        await asyncio.gather(*[provider.tear_down() for _, provider in context.get().items()], return_exceptions=True)
+        results = await asyncio.gather(
+            *[provider.tear_down() for _, provider in context.get().items()], return_exceptions=True
+        )
+        for exception in results:
+            if isinstance(exception, Exception):  # pragma: no cover
+                logger.error("Error in resource tear down", exc_info=exception)
         context.reset(token)
 
 
 class DIContextMiddleware:
     def __init__(self, app: ASGIApp) -> None:
         self.app = app
```

### Comparing `that_depends-1.6.4/that_depends/providers/factories.py` & `that_depends-1.6.5/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/that_depends/providers/resources.py` & `that_depends-1.6.5/that_depends/providers/resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/that_depends/providers/singleton.py` & `that_depends-1.6.5/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.4/PKG-INFO` & `that_depends-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.6.4
+Version: 1.6.5
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -274,15 +274,15 @@
 ```python
 import datetime
 
 from that_depends import BaseContainer, providers
 
 
 async def async_factory() -> datetime.datetime:
-    return datetime.datetime.now(tz=datetime.UTC)
+    return datetime.datetime.now(tz=datetime.timezone.utc)
 
 
 class DIContainer(BaseContainer):
     async_factory = providers.Factory(async_factory)
 ```
 ### List
 - List provider contains other providers.
```

