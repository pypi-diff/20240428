# Comparing `tmp/fango-0.0.20.tar.gz` & `tmp/fango-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fango-0.0.20.tar", max compression
+gzip compressed data, was "fango-0.0.21.tar", max compression
```

## Comparing `fango-0.0.20.tar` & `fango-0.0.21.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      620 2024-02-24 18:07:20.033525 fango-0.0.20/README.md
--rw-r--r--   0        0        0     7456 2024-04-14 23:03:25.730166 fango-0.0.20/fango/adapters/pydantic.py
--rw-r--r--   0        0        0      848 2024-04-14 23:03:25.731065 fango-0.0.20/fango/adapters/types.py
--rw-r--r--   0        0        0     2681 2024-04-14 23:03:25.731578 fango-0.0.20/fango/auth.py
--rw-r--r--   0        0        0     4845 2024-04-14 23:03:25.731979 fango-0.0.20/fango/filters.py
--rw-r--r--   0        0        0      310 2024-04-14 23:03:25.732278 fango-0.0.20/fango/generics.py
--rw-r--r--   0        0        0     1907 2024-04-14 23:03:25.732567 fango-0.0.20/fango/log.py
--rw-r--r--   0        0        0        0 2024-04-14 23:03:25.733144 fango-0.0.20/fango/middleware/__init__.py
--rw-r--r--   0        0        0      997 2024-04-14 23:03:25.734606 fango-0.0.20/fango/middleware/common.py
--rw-r--r--   0        0        0     6639 2024-04-14 23:03:25.735056 fango-0.0.20/fango/pagination.py
--rw-r--r--   0        0        0     2447 2024-04-14 23:03:25.735385 fango-0.0.20/fango/permissions.py
--rw-r--r--   0        0        0      440 2024-04-14 23:03:25.735661 fango-0.0.20/fango/routing.py
--rw-r--r--   0        0        0     2341 2024-04-15 00:04:36.421870 fango-0.0.20/fango/schemas.py
--rw-r--r--   0        0        0      284 2024-04-14 23:03:25.741040 fango-0.0.20/fango/tests/client.py
--rw-r--r--   0        0        0      723 2024-04-14 23:03:25.741322 fango-0.0.20/fango/tests/fixtures.py
--rw-r--r--   0        0        0     3116 2024-04-14 23:03:25.741600 fango-0.0.20/fango/utils.py
--rw-r--r--   0        0        0     7253 2024-04-14 23:03:25.742114 fango-0.0.20/fango/viewsets.py
--rw-r--r--   0        0        0      536 2024-04-15 00:04:48.299023 fango-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 fango-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0      645 2024-04-28 12:17:49.759751 fango-0.0.21/README.md
+-rw-r--r--   0        0        0     7506 2024-04-28 12:17:53.363725 fango-0.0.21/fango/adapters/pydantic.py
+-rw-r--r--   0        0        0      848 2024-04-28 12:15:19.802157 fango-0.0.21/fango/adapters/types.py
+-rw-r--r--   0        0        0     2681 2024-04-28 12:15:19.802462 fango-0.0.21/fango/auth.py
+-rw-r--r--   0        0        0     4845 2024-04-28 12:15:19.802795 fango-0.0.21/fango/filters.py
+-rw-r--r--   0        0        0      310 2024-04-28 12:15:19.803100 fango-0.0.21/fango/generics.py
+-rw-r--r--   0        0        0     1907 2024-04-28 12:15:19.803391 fango-0.0.21/fango/log.py
+-rw-r--r--   0        0        0        0 2024-04-28 12:15:19.804239 fango-0.0.21/fango/middleware/__init__.py
+-rw-r--r--   0        0        0      586 2024-04-28 12:17:53.364000 fango-0.0.21/fango/middleware/common.py
+-rw-r--r--   0        0        0     6639 2024-04-28 12:15:19.806403 fango-0.0.21/fango/pagination.py
+-rw-r--r--   0        0        0     2403 2024-04-28 12:17:53.364249 fango-0.0.21/fango/permissions.py
+-rw-r--r--   0        0        0      440 2024-04-28 12:15:19.806985 fango-0.0.21/fango/routing.py
+-rw-r--r--   0        0        0     3495 2024-04-28 12:17:53.364495 fango-0.0.21/fango/schemas.py
+-rw-r--r--   0        0        0      284 2024-04-28 12:15:19.813139 fango-0.0.21/fango/tests/client.py
+-rw-r--r--   0        0        0      723 2024-04-28 12:15:19.813383 fango-0.0.21/fango/tests/fixtures.py
+-rw-r--r--   0        0        0     3064 2024-04-28 12:17:53.364884 fango-0.0.21/fango/utils.py
+-rw-r--r--   0        0        0     7259 2024-04-28 12:17:53.365313 fango-0.0.21/fango/viewsets.py
+-rw-r--r--   0        0        0      536 2024-04-28 12:17:53.365470 fango-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 fango-0.0.21/PKG-INFO
```

### Comparing `fango-0.0.20/README.md` & `fango-0.0.21/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 Some built in features of FANGO:
 
 1. Async cypher JWT auth
 2. DRF-like cursor paginaton
 3. DRF-lile GenericViewSet
 4. Adapter for save pydantic model data with ORM
 5. FastAPI TestClient for pytest-django tests
+6. Django-filter support
```

### Comparing `fango-0.0.20/fango/adapters/pydantic.py` & `fango-0.0.21/fango/adapters/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 __all__ = ["PydanticAdapter"]
 
 ForwardRel = ForeignKey | OneToOneField | OneToOneRel
 MultipleRel = ManyToOneRel | ManyToManyField
 
 
 class AdapterError(Exception):
-    ...
+    pass
 
 
 class PydanticAdapter(Model):
     """
     A base class for creating Django model instances from Pydantic schemas.
 
     """
@@ -223,14 +223,15 @@
 
     elif isinstance(value, PK) or key.endswith("_id"):
         return field.related_model.objects.get(pk=value)
 
     elif isinstance(value, Model):
         value.clean()
         value.save()
+        getattr(instance, field.name).add(value)
         return value
 
     else:
         raise AdapterError
 
 
 @log_params("PoetryAdapter")
```

### Comparing `fango-0.0.20/fango/adapters/types.py` & `fango-0.0.21/fango/adapters/types.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.20/fango/auth.py` & `fango-0.0.21/fango/auth.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.20/fango/filters.py` & `fango-0.0.21/fango/filters.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.20/fango/log.py` & `fango-0.0.21/fango/log.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.20/fango/pagination.py` & `fango-0.0.21/fango/pagination.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.20/fango/permissions.py` & `fango-0.0.21/fango/permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import inspect
 from types import MethodType
 from typing import get_args
 
 from django.contrib.auth.models import User
 from fastapi import Depends, HTTPException, Request
 
-from fango.utils import run_async, ttl_cache
+from fango.utils import ttl_cache
 
 __all__ = [
     "CHECK_MODEL_PERMISSIONS",
     "ALLOW_ANY",
 ]
 
 
 @ttl_cache(10)
-async def _get_user_permissions(user: "User") -> set[str]:
+def _get_user_permissions(user: "User") -> set[str]:
     """
     Function call user.get_all_permissions() in async context
     and caching to 10s.
 
     """
-    return await run_async(user.get_all_permissions)
+    return user.get_all_permissions()
 
 
 def _get_permissions_mapping(request: "Request"):
     """
     Function for checking stored permission_mapping, or return default.
 
     """
@@ -39,30 +39,30 @@
         "POST": ["%(app_label)s.add_%(model_name)s"],
         "PUT": ["%(app_label)s.change_%(model_name)s"],
         "PATCH": ["%(app_label)s.change_%(model_name)s"],
         "DELETE": ["%(app_label)s.delete_%(model_name)s"],
     }
 
 
-async def _check_model_permissions(request: "Request") -> None:
+def _check_model_permissions(request: "Request") -> None:
     """
     Model Permissions check implementation.
 
     """
 
     endpoint = request.scope["endpoint"]
 
     if isinstance(endpoint, MethodType):
         model = endpoint.__self__.queryset.model
     else:
         signature = inspect.signature(request.scope["route"].response_model)
         model = get_args(signature.parameters["results"].annotation)[0].model
 
     permissions_mapping = _get_permissions_mapping(request)
-    user_permissions = await _get_user_permissions(request.state.user)
+    user_permissions = _get_user_permissions(request.state.user)
 
     if request.method in permissions_mapping:
         permissions = permissions_mapping[request.method]
 
         if not permissions:
             return
```

### Comparing `fango-0.0.20/fango/tests/fixtures.py` & `fango-0.0.21/fango/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.20/fango/utils.py` & `fango-0.0.21/fango/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,19 @@
     """
     Decorator for TTL caching.
 
     """
 
     def decorator(func: Callable):
         @wraps(func)
-        async def wrapped(*args, **kwargs) -> Callable:
+        def wrapped(*args, **kwargs) -> Callable:
             key = "ttl_cache_key_{}_{}".format(func.__name__, hash(args) + hash(frozenset(kwargs.items())))
             result = cache.get(key)
             if result is not None:
                 return result
-            if iscoroutinefunction(func):
-                result = await func(*args, **kwargs)
             else:
                 result = func(*args, **kwargs)
             cache.set(key, result, timeout=ttl)
             return result
 
         return wrapped
 
@@ -116,8 +114,10 @@
 
 
 def get_choices_label(enum: type[Choices], value: int) -> str:
     """
     Function returns choices text.
 
     """
-    return enum.choices[value][1]
+
+    choices_dict = {k: v for k, v in enum.choices}
+    return choices_dict[value]
```

### Comparing `fango-0.0.20/fango/viewsets.py` & `fango-0.0.21/fango/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         route_name = request.scope["route"].name
 
         if model := self.pydantic_model_action_classes.get(route_name):
             return model
         else:
             return self.pydantic_model_action_classes["table"]
 
-    def get_queryset(self, request: Request) -> QuerySet:
+    async def get_queryset(self, request: Request) -> QuerySet:
         """
         Method for get queryset defined in ViewSet.
 
         """
         return self.queryset
```

### Comparing `fango-0.0.20/pyproject.toml` & `fango-0.0.21/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fango"
-version = "0.0.20"
+version = "0.0.21"
 description = "Metaframework for web with combined FastAPI and Django"
 repository = "https://github.com/egorgam/fango"
 keywords = ["fastapi", "django", "fango"]
 authors = ["Egor Gamazin <egorgamazin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fango-0.0.20/PKG-INFO` & `fango-0.0.21/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fango
-Version: 0.0.20
+Version: 0.0.21
 Summary: Metaframework for web with combined FastAPI and Django
 Home-page: https://github.com/egorgam/fango
 License: MIT
 Keywords: fastapi,django,fango
 Author: Egor Gamazin
 Author-email: egorgamazin@yandex.ru
 Requires-Python: >=3.10,<4.0
@@ -35,8 +35,9 @@
 Some built in features of FANGO:
 
 1. Async cypher JWT auth
 2. DRF-like cursor paginaton
 3. DRF-lile GenericViewSet
 4. Adapter for save pydantic model data with ORM
 5. FastAPI TestClient for pytest-django tests
+6. Django-filter support
```

