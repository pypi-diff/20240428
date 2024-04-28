# Comparing `tmp/permission_manager-0.2.0.tar.gz` & `tmp/permission_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permission_manager-0.2.0.tar", max compression
+gzip compressed data, was "permission_manager-0.3.0.tar", max compression
```

## Comparing `permission_manager-0.2.0.tar` & `permission_manager-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2024-02-12 01:31:52.754593 permission_manager-0.2.0/LICENSE
--rw-r--r--   0        0        0     2505 2024-02-12 01:31:52.754593 permission_manager-0.2.0/README.md
--rw-r--r--   0        0        0      160 2024-02-12 01:31:52.754593 permission_manager-0.2.0/permission_manager/__init__.py
--rw-r--r--   0        0        0      959 2024-02-12 01:31:52.754593 permission_manager-0.2.0/permission_manager/decorators.py
--rw-r--r--   0        0        0      190 2024-02-12 01:31:52.754593 permission_manager-0.2.0/permission_manager/exceptions.py
--rw-r--r--   0        0        0     4628 2024-02-12 01:31:52.754593 permission_manager-0.2.0/permission_manager/manager.py
--rw-r--r--   0        0        0      560 2024-02-12 01:31:52.754593 permission_manager-0.2.0/permission_manager/result.py
--rw-r--r--   0        0        0     2094 2024-02-12 01:31:52.754593 permission_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 permission_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-28 01:55:53.317114 permission_manager-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2508 2024-04-28 01:55:53.317114 permission_manager-0.3.0/README.md
+-rw-r--r--   0        0        0      160 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/__init__.py
+-rw-r--r--   0        0        0     1201 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/decorators.py
+-rw-r--r--   0        0        0      198 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/exceptions.py
+-rw-r--r--   0        0        0     4848 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/manager.py
+-rw-r--r--   0        0        0     1495 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/result.py
+-rw-r--r--   0        0        0     2241 2024-04-28 01:55:53.317114 permission_manager-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 permission_manager-0.3.0/PKG-INFO
```

### Comparing `permission_manager-0.2.0/LICENSE` & `permission_manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `permission_manager-0.2.0/README.md` & `permission_manager-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 # > False
 manager.has_permission('access')
 # > PermissionResult(value=False, message=['Due status'])
 
 manager.resolve()
 # > {'access': False, 'create': True, 'delete': False}
 manager.resolve(with_messages=True)
-# > {'access': {'allow': False, 'message': ['Due status']},
-#    'create': {'allow': True, 'message': None},
-#    'delete': {'allow': False, 'message': None}}
+# > {'access': {'allow': False, 'messages': ['Due status']},
+#    'create': {'allow': True, 'messages': None},
+#    'delete': {'allow': False, 'messages': None}}
 ```
 
 Also, it's include `PermissionManager`, which add additional functionality to check parent permissions
 
 ```python
 import dataclasses
 from permission_manager import PermissionManager
```

### Comparing `permission_manager-0.2.0/permission_manager/manager.py` & `permission_manager-0.3.0/permission_manager/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,162 +1,169 @@
 import re
+from collections.abc import Iterable
 from contextlib import suppress
 from functools import cached_property
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import Any
 
-from .result import PermissionResult
 from .decorators import cache_permission, catch_denied_exception
-from .exceptions import PermissionManagerException
+from .exceptions import PermissionManagerError
+from .result import PermissionResult
 
 
 permission_re = re.compile(r'^has_(\w+)_permission$')
 
 
 class BasePermissionMeta(type):
-    """Metaclass for bind permission actions"""
+    """Metaclass for bind permission actions."""
 
     def __new__(cls, *args, **kwargs) -> type:
         new_cls = super().__new__(cls, *args, **kwargs)
         new_cls._actions = {}
         new_cls._aliases = {}
         new_cls.bind_actions()
         return new_cls
 
     def bind_actions(cls) -> None:
-        """Collect all actions, add decorators"""
+        """Collect all actions, add decorators."""
         for attr_name in dir(cls):
             if action_name := permission_re.match(attr_name):
                 permission_fn = cache_permission(
                     catch_denied_exception(getattr(cls, attr_name))
                 )
                 setattr(cls, attr_name, permission_fn)
                 cls._actions[action_name.group(1)] = permission_fn
 
                 if alias := getattr(
-                    permission_fn, '_permission_manager_alias', None
+                    permission_fn, 'permission_manager_alias', None
                 ):
                     cls._aliases[alias] = permission_fn
 
 
 class BasePermissionManager(metaclass=BasePermissionMeta):
-    """Base permission manager class"""
+    """Base permission manager class."""
 
     def __init__(
         self,
-        user: Optional[Any] = None,
-        instance: Optional[Any] = None,
+        *,
+        user: Any | None = None,
+        instance: Any | None = None,
         cache: bool = False,
         **context,
     ) -> None:
         self.user = user
         self.instance = instance
         self.context = context
         self.cache = cache
         self._cache = {}
 
     @classmethod
-    def create(cls, name: str, **type_dict) -> type:
-        """Create new manager dynamically"""
-
+    def create(
+        cls: type['BasePermissionManager'],
+        name: str,
+        **type_dict,
+    ) -> type:
+        """Create new manager dynamically."""
         return type(name, (cls,), type_dict)
 
     def has_permission(self, action: str) -> bool:
-        """Check permission"""
-
+        """Check permission."""
         with suppress(KeyError):
             return self._actions[action](self)
 
         try:
             return self._aliases[action](self)
         except KeyError as exc:
             raise ValueError(
                 f'"{self.__class__.__name__}" doesn\'t have "{action}" action.'
             ) from exc
 
     def get_result_value(
         self,
-        value: Union[bool, dict, PermissionResult],
+        *,
+        value: bool | dict | PermissionResult,
         with_messages: bool = False,
-    ) -> Union[bool, dict]:
-        """Serialize result value"""
-
+    ) -> bool | dict:
+        """Serialize result value."""
         if isinstance(value, dict):
             return {
                 k: self.get_result_value(
                     value=v,
                     with_messages=with_messages,
                 )
                 for k, v in value.items()
             }
 
         result = bool(value)
 
         if with_messages:
             result = {
                 'allow': result,
-                'message': getattr(value, 'message', None),
+                'messages': getattr(value, 'returned_message', None),
             }
         return result
 
     def resolve(
         self,
-        actions: Optional[Iterable] = None,
+        *,
+        actions: Iterable | None = None,
         with_messages: bool = False,
-    ) -> Dict:
-        """Resolve list of actions"""
-
+    ) -> dict:
+        """Resolve list of actions."""
         if actions is None:
             actions = self._actions.keys()
 
         return {
             action: self.get_result_value(
                 value=self.has_permission(action),
                 with_messages=with_messages,
             )
             for action in actions
         }
 
 
 class PermissionManager(BasePermissionManager):
-    """Permission manager class with additional functionality to check parent permissions"""
+    """Permission manager class.
+
+    Permission manager class with additional functionality
+    to check parent permissions.
+    """
 
-    parent_attr: Optional[str] = None
+    parent_attr: str | None = None
 
     @cached_property
     def parent(self) -> Any:
-        """Get parent object"""
-
+        """Get parent object."""
         if parent := self.context.get('parent'):
             return parent
         return self.get_parent_from_instance()
 
     def get_parent_from_instance(self) -> Any:
-        """Get parent object from instance"""
-
+        """Get parent object from instance."""
         if not self.instance:
-            raise PermissionManagerException('Instance is missing.')
+            raise PermissionManagerError('Instance is missing.')
 
         if not self.parent_attr:
-            raise PermissionManagerException(
+            raise PermissionManagerError(
                 'Attribute `parent_attr` is not defined.'
             )
 
         return getattr(self.instance, self.parent_attr)
 
     @property
     def has_parent(self) -> bool:
-        """Check if object has parent"""
-
+        """Check if object has parent."""
         try:
             return bool(self.parent)
-        except PermissionManagerException:
+        except PermissionManagerError:
             return False
 
     @cached_property
     def parent_permission_manager(self) -> 'PermissionManager':
-        """Get parent permission manager"""
+        """Get parent permission manager."""
+        if from_context := self.context.get('parent_permission_manager'):
+            return from_context
 
         return self.parent.permission_manager(
             user=self.user,
             instance=self.parent,
             context=self.context,
         )
```

### Comparing `permission_manager-0.2.0/PKG-INFO` & `permission_manager-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permission-manager
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple way to manage object permissions.
 Home-page: https://github.com/kindlycat/permission-manager
 License: MIT
 Keywords: permissions
 Author: Grigory Mishchenko
 Author-email: grishkokot@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -81,17 +81,17 @@
 # > False
 manager.has_permission('access')
 # > PermissionResult(value=False, message=['Due status'])
 
 manager.resolve()
 # > {'access': False, 'create': True, 'delete': False}
 manager.resolve(with_messages=True)
-# > {'access': {'allow': False, 'message': ['Due status']},
-#    'create': {'allow': True, 'message': None},
-#    'delete': {'allow': False, 'message': None}}
+# > {'access': {'allow': False, 'messages': ['Due status']},
+#    'create': {'allow': True, 'messages': None},
+#    'delete': {'allow': False, 'messages': None}}
 ```
 
 Also, it's include `PermissionManager`, which add additional functionality to check parent permissions
 
 ```python
 import dataclasses
 from permission_manager import PermissionManager
```

