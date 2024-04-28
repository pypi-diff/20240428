# Comparing `tmp/greyhorse-0.4.2.tar.gz` & `tmp/greyhorse-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse-0.4.2.tar", max compression
+gzip compressed data, was "greyhorse-0.4.3.tar", max compression
```

## Comparing `greyhorse-0.4.2.tar` & `greyhorse-0.4.3.tar`

### file list

```diff
@@ -1,60 +1,58 @@
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/builders/__init__.py
--rw-r--r--   0        0        0    13843 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/builders/module.py
--rw-r--r--   0        0        0     2858 2024-04-09 22:29:40.601420 greyhorse-0.4.2/greyhorse/app/builders/resource.py
--rw-r--r--   0        0        0    10686 2024-04-20 11:56:32.782673 greyhorse-0.4.2/greyhorse/app/context.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/entities/__init__.py
--rw-r--r--   0        0        0     8340 2024-04-10 16:01:20.918796 greyhorse-0.4.2/greyhorse/app/entities/application.py
--rw-r--r--   0        0        0     4812 2024-04-14 12:30:24.508646 greyhorse-0.4.2/greyhorse/app/entities/controller.py
--rw-r--r--   0        0        0      910 2024-04-14 12:24:31.419245 greyhorse-0.4.2/greyhorse/app/entities/deps.py
--rw-r--r--   0        0        0    19413 2024-04-17 16:38:43.638882 greyhorse-0.4.2/greyhorse/app/entities/module.py
--rw-r--r--   0        0        0      253 2024-04-18 23:28:44.736666 greyhorse-0.4.2/greyhorse/app/entities/operator.py
--rw-r--r--   0        0        0     2903 2024-04-20 10:49:17.227923 greyhorse-0.4.2/greyhorse/app/entities/providers.py
--rw-r--r--   0        0        0     1577 2024-04-09 22:29:40.601420 greyhorse-0.4.2/greyhorse/app/entities/resource.py
--rw-r--r--   0        0        0     6110 2024-04-09 22:29:35.965597 greyhorse-0.4.2/greyhorse/app/entities/service.py
--rw-r--r--   0        0        0     1528 2024-04-10 15:13:55.985794 greyhorse-0.4.2/greyhorse/app/errors.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.965597 greyhorse-0.4.2/greyhorse/app/schemas/__init__.py
--rw-r--r--   0        0        0      883 2024-04-20 11:54:14.943578 greyhorse-0.4.2/greyhorse/app/schemas/components.py
--rw-r--r--   0        0        0      587 2024-04-20 11:54:14.975577 greyhorse-0.4.2/greyhorse/app/schemas/controller.py
--rw-r--r--   0        0        0     1762 2024-04-20 11:54:14.955577 greyhorse-0.4.2/greyhorse/app/schemas/module.py
--rw-r--r--   0        0        0      590 2024-04-20 11:54:14.963577 greyhorse-0.4.2/greyhorse/app/schemas/service.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/app/tasks/__init__.py
--rw-r--r--   0        0        0     1308 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/app/tasks/app.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/app/utils/__init__.py
--rw-r--r--   0        0        0     6880 2024-04-17 14:33:40.645939 greyhorse-0.4.2/greyhorse/app/utils/registry.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/cache/__init__.py
--rw-r--r--   0        0        0     1909 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/cache/base.py
--rw-r--r--   0        0        0     2438 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/cache/method.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/models/__init__.py
--rw-r--r--   0        0        0     1868 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/models/base.py
--rw-r--r--   0        0        0     3575 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/fields.py
--rw-r--r--   0        0        0     2088 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/filterable.py
--rw-r--r--   0        0        0     4491 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/model.py
--rw-r--r--   0        0        0     1615 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/serializable.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/repositories/__init__.py
--rw-r--r--   0        0        0     2752 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/repositories/base.py
--rw-r--r--   0        0        0     2387 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/repositories/filterable.py
--rw-r--r--   0        0        0      117 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/serializers/__init__.py
--rw-r--r--   0        0        0      564 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/serializers/base.py
--rw-r--r--   0        0        0      513 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/serializers/pickle.py
--rw-r--r--   0        0        0     1902 2024-04-20 11:58:08.771261 greyhorse-0.4.2/greyhorse/data/storage.py
--rw-r--r--   0        0        0      131 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/i18n/__init__.py
--rw-r--r--   0        0        0     2663 2024-04-18 23:30:16.265809 greyhorse-0.4.2/greyhorse/i18n/translator.py
--rw-r--r--   0        0        0     1584 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/logging.py
--rw-r--r--   0        0        0     2575 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/messagebus.py
--rw-r--r--   0        0        0     4130 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/result.py
--rw-r--r--   0        0        0     3761 2024-04-10 15:15:08.074854 greyhorse-0.4.2/greyhorse/translations.toml
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/confs.py
--rw-r--r--   0        0        0     2169 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/dicts.py
--rw-r--r--   0        0        0      568 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/hashes.py
--rw-r--r--   0        0        0      922 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/imports.py
--rw-r--r--   0        0        0     1157 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/injectors.py
--rw-r--r--   0        0        0     1573 2024-04-20 10:13:14.653404 greyhorse-0.4.2/greyhorse/utils/invoke.py
--rw-r--r--   0        0        0      452 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/json.py
--rw-r--r--   0        0        0      823 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/strings.py
--rw-r--r--   0        0        0     1095 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/time.py
--rw-r--r--   0        0        0     1040 2024-04-20 11:58:08.375275 greyhorse-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 greyhorse-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/app/builders/__init__.py
+-rw-r--r--   0        0        0    12549 2024-04-28 16:06:53.142337 greyhorse-0.4.3/greyhorse/app/builders/module.py
+-rw-r--r--   0        0        0    12327 2024-04-21 00:04:20.478630 greyhorse-0.4.3/greyhorse/app/context.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/app/entities/__init__.py
+-rw-r--r--   0        0        0     8384 2024-04-28 15:34:05.766225 greyhorse-0.4.3/greyhorse/app/entities/application.py
+-rw-r--r--   0        0        0     4812 2024-04-14 12:30:24.508646 greyhorse-0.4.3/greyhorse/app/entities/controller.py
+-rw-r--r--   0        0        0      910 2024-04-14 12:24:31.419245 greyhorse-0.4.3/greyhorse/app/entities/deps.py
+-rw-r--r--   0        0        0    19413 2024-04-17 16:38:43.638882 greyhorse-0.4.3/greyhorse/app/entities/module.py
+-rw-r--r--   0        0        0      253 2024-04-18 23:28:44.736666 greyhorse-0.4.3/greyhorse/app/entities/operator.py
+-rw-r--r--   0        0        0     2903 2024-04-20 10:49:17.227923 greyhorse-0.4.3/greyhorse/app/entities/providers.py
+-rw-r--r--   0        0        0     7355 2024-04-28 16:15:29.403350 greyhorse-0.4.3/greyhorse/app/entities/service.py
+-rw-r--r--   0        0        0     1528 2024-04-10 15:13:55.985794 greyhorse-0.4.3/greyhorse/app/errors.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.965597 greyhorse-0.4.3/greyhorse/app/schemas/__init__.py
+-rw-r--r--   0        0        0      883 2024-04-20 11:54:14.943578 greyhorse-0.4.3/greyhorse/app/schemas/components.py
+-rw-r--r--   0        0        0      587 2024-04-20 11:54:14.975577 greyhorse-0.4.3/greyhorse/app/schemas/controller.py
+-rw-r--r--   0        0        0     1762 2024-04-20 11:54:14.955577 greyhorse-0.4.3/greyhorse/app/schemas/module.py
+-rw-r--r--   0        0        0      590 2024-04-20 11:54:14.963577 greyhorse-0.4.3/greyhorse/app/schemas/service.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/app/tasks/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/app/tasks/app.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/app/utils/__init__.py
+-rw-r--r--   0        0        0     6880 2024-04-17 14:33:40.645939 greyhorse-0.4.3/greyhorse/app/utils/registry.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/cache/__init__.py
+-rw-r--r--   0        0        0     1909 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/cache/base.py
+-rw-r--r--   0        0        0     2438 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/cache/method.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/models/__init__.py
+-rw-r--r--   0        0        0     1868 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/models/base.py
+-rw-r--r--   0        0        0     3575 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/fields.py
+-rw-r--r--   0        0        0     2088 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/filterable.py
+-rw-r--r--   0        0        0     4491 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/model.py
+-rw-r--r--   0        0        0     1615 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/serializable.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/repositories/__init__.py
+-rw-r--r--   0        0        0     2752 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/repositories/base.py
+-rw-r--r--   0        0        0     2387 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/repositories/filterable.py
+-rw-r--r--   0        0        0      117 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/serializers/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/serializers/base.py
+-rw-r--r--   0        0        0      513 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/serializers/pickle.py
+-rw-r--r--   0        0        0     1902 2024-04-20 11:58:08.771261 greyhorse-0.4.3/greyhorse/data/storage.py
+-rw-r--r--   0        0        0      131 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/i18n/__init__.py
+-rw-r--r--   0        0        0     2663 2024-04-18 23:30:16.265809 greyhorse-0.4.3/greyhorse/i18n/translator.py
+-rw-r--r--   0        0        0     1584 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/logging.py
+-rw-r--r--   0        0        0     2575 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/messagebus.py
+-rw-r--r--   0        0        0     4130 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/result.py
+-rw-r--r--   0        0        0     3761 2024-04-10 15:15:08.074854 greyhorse-0.4.3/greyhorse/translations.toml
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/confs.py
+-rw-r--r--   0        0        0     2169 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/dicts.py
+-rw-r--r--   0        0        0      568 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/hashes.py
+-rw-r--r--   0        0        0      959 2024-04-27 19:03:47.313480 greyhorse-0.4.3/greyhorse/utils/imports.py
+-rw-r--r--   0        0        0     1157 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/injectors.py
+-rw-r--r--   0        0        0     1573 2024-04-20 10:13:14.653404 greyhorse-0.4.3/greyhorse/utils/invoke.py
+-rw-r--r--   0        0        0      452 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/json.py
+-rw-r--r--   0        0        0      823 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/strings.py
+-rw-r--r--   0        0        0     1095 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/time.py
+-rw-r--r--   0        0        0     1040 2024-04-28 14:53:41.171207 greyhorse-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 greyhorse-0.4.3/PKG-INFO
```

### Comparing `greyhorse-0.4.2/greyhorse/app/builders/module.py` & `greyhorse-0.4.3/greyhorse/app/builders/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,58 @@
 import sys
 from itertools import chain
 
 import pydantic
 
 from greyhorse.result import Result
+from greyhorse.utils.imports import import_path
 from greyhorse.utils.injectors import ParamsInjector
 from greyhorse.utils.invoke import invoke_sync
-from greyhorse.utils.imports import import_path
-
 from ..entities.application import Application
 from ..entities.controller import Controller, ControllerFactoryFn
 from ..entities.module import Module, ModuleErrorsItem
 from ..entities.service import Service, ServiceFactoryFn
 from ..errors import ControllerCreationError, CtrlFactoryNotFoundError, InvalidModuleConfError, ModuleCreationError, \
     ModuleLoadError, ModuleUnloadError, ModuleValidationError, ServiceCreationError, ServiceFactoryNotFoundError
 from ..schemas.controller import ControllerConf
 from ..schemas.module import ModuleConf, ModuleDesc
 from ..schemas.service import ServiceConf
 from ...i18n import tr
 from ...logging import logger
-import sys
-from itertools import chain
 
-import pydantic
 
-from greyhorse.result import Result
-from greyhorse.utils.imports import import_path
-from greyhorse.utils.injectors import ParamsInjector
-from greyhorse.utils.invoke import invoke_sync
-from ..entities.application import Application
-from ..entities.controller import Controller, ControllerFactoryFn
-from ..entities.module import Module, ModuleErrorsItem
-from ..entities.service import Service, ServiceFactoryFn
-from ..errors import ControllerCreationError, CtrlFactoryNotFoundError, InvalidModuleConfError, ModuleCreationError, \
-    ModuleLoadError, ModuleUnloadError, ModuleValidationError, ServiceCreationError, ServiceFactoryNotFoundError
-from ..schemas.controller import ControllerConf
-from ..schemas.module import ModuleConf, ModuleDesc
-from ..schemas.service import ServiceConf
-from ...i18n import tr
-from ...logging import logger
+def _get_module_package(desc: ModuleDesc) -> str:
+    if not desc.path.startswith('.'):
+        return desc.path
+
+    path = desc.path
+    dots_count = 0
+
+    for c in path[1:]:
+        if '.' == c:
+            dots_count += 1
+        else:
+            path = path[dots_count + 1:]
+            break
+
+    initpath = desc._initpath
+    dots_count = min(dots_count, len(initpath))
+    initpath = initpath[0:len(initpath) - dots_count]
+    return '.'.join(initpath + [path])
 
 
 class ModuleBuilder:
     def __init__(
         self, app: Application, root_desc: ModuleDesc,
     ):
         self._app = app
         self._injector = ParamsInjector()
         self._key_stack: list[str] = []
         self._root_desc = root_desc
 
-    def get_module_init_path(self, desc: ModuleDesc) -> str:
-        initpath = desc._initpath
-        path = desc.path
-
-        if desc.path.startswith('.'):
-            dots_count = 0
-
-            for c in path[1:]:
-                if '.' == c:
-                    dots_count += 1
-                else:
-                    path = path[dots_count + 1:]
-                    break
-
-            dots_count = min(dots_count, len(initpath))
-            initpath = initpath[0:len(initpath) - dots_count]
-
-        return '.'.join(initpath + [path]) if desc is not self._root_desc else desc.path
-
     def load_pass(self, desc: ModuleDesc | None = None) -> Result[ModuleConf | None]:
         desc = desc or self._root_desc
 
         if not desc.enabled:
             return Result.from_ok()
 
         res = self._load_module(desc)
@@ -149,20 +129,19 @@
         logger.info(tr('app.builder.create-success').format(path=desc.path))
         return Result.from_ok(instance)
 
     def _load_module(self, desc: ModuleDesc) -> Result:
         if desc._conf is not None:
             return Result.from_ok()
 
-        module_init_path = self.get_module_init_path(desc)
-        func_name = module_init_path + ':__init__'
-        logger.info(tr('app.builder.try-load').format(module_init_path=module_init_path))
+        module_path = _get_module_package(desc)
+        logger.info(tr('app.builder.try-load').format(module_init_path=module_path))
 
         try:
-            func = import_path(func_name)
+            func = import_path(f'{module_path}:__init__')
 
         except (ImportError, AttributeError) as e:
             error = ModuleLoadError(exc=e)
             logger.error(error.message)
             return Result.from_error(error)
 
         injected_args = self._injector(func, values=desc.args)
@@ -176,19 +155,19 @@
             return Result.from_error(error)
         except Exception as e:
             error = ModuleLoadError(exc=e)
             logger.error(error.message)
             return Result.from_error(error)
 
         if not isinstance(res, ModuleConf):
-            error = InvalidModuleConfError(module_init_path=module_init_path)
+            error = InvalidModuleConfError(module_init_path=module_path)
             logger.error(error.message)
             return Result.from_error(error)
 
-        logger.info(tr('app.builder.load-success').format(module_init_path=module_init_path))
+        logger.info(tr('app.builder.load-success').format(module_init_path=module_path))
         desc._conf = res
         return Result.from_ok()
 
     def _create_controller(
         self, module: Module, conf: ControllerConf, factory: ControllerFactoryFn,
     ) -> Result[Controller]:
         logger.info(tr('app.builder.try-ctrl').format(name=conf.name))
@@ -308,17 +287,14 @@
         self, app: Application, root_desc: ModuleDesc,
     ):
         self._app = app
         self._injector = ParamsInjector()
         self._key_stack: list[str] = []
         self._root_desc = root_desc
 
-    def get_module_init_path(self, desc: ModuleDesc) -> str:
-        return '.'.join(desc._initpath + [desc.path]) if desc is not self._root_desc else desc.path
-
     def unload_pass(self, desc: ModuleDesc | None = None) -> Result:
         desc = desc or self._root_desc
 
         if not desc.enabled or not desc._conf:
             return Result.from_ok()
 
         conf = desc._conf
@@ -365,31 +341,30 @@
         logger.info(tr('app.builder.destroy-success').format(path=desc.path))
         return Result.from_ok()
 
     def _unload_module(self, desc: ModuleDesc) -> Result:
         if desc._conf is None:
             return Result.from_ok()
 
-        module_init_path = self.get_module_init_path(desc)
-        func_name = module_init_path + ':__fini__'
-        logger.info(tr('app.builder.try-unload').format(module_init_path=module_init_path))
+        module_path = _get_module_package(desc)
+        logger.info(tr('app.builder.try-unload').format(module_init_path=module_path))
 
         try:
-            func = import_path(func_name)
+            func = import_path(f'{module_path}:__fini__')
 
         except (ImportError, AttributeError):
             pass
         else:
             injected_args = self._injector(func, types={ModuleConf: desc._conf})
 
             try:
                 invoke_sync(func, *injected_args.args, **injected_args.kwargs)
 
             except Exception as e:
                 error = ModuleUnloadError(exc=e)
                 logger.error(error.message)
                 return Result.from_error(error)
 
-        logger.info(tr('app.builder.unload-success').format(module_init_path=module_init_path))
+        logger.info(tr('app.builder.unload-success').format(module_init_path=module_path))
         desc._conf = None
-        del sys.modules[module_init_path]
+        del sys.modules[module_path]
         return Result.from_ok()
```

### Comparing `greyhorse-0.4.2/greyhorse/app/context.py` & `greyhorse-0.4.3/greyhorse/app/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import asyncio
+import inspect
 import threading
+from collections import defaultdict
 from contextlib import AbstractAsyncContextManager, AbstractContextManager, AsyncExitStack, ExitStack
 from contextvars import ContextVar
 from typing import Any, AsyncContextManager, Awaitable, Callable, ContextManager, Mapping, override
 from uuid import uuid4
 
 from greyhorse.utils.invoke import get_asyncio_loop, invoke_async, invoke_sync
 
 type FieldFactory[T] = (
     T | Callable[[], Awaitable[T] | T] |
-    AbstractContextManager[T] | AbstractAsyncContextManager[T]
+    Callable[[], AbstractContextManager[T]] | Callable[[], AbstractAsyncContextManager[T]]
 )
 
 
 class Context(object):
     __slots__ = (
         '_factory', '_field_factories', '_finalizers',
-        '_params', '_object', '_ident', '_parent',
+        '_params', '_object', '_ident', '_parent', '_prev',
     )
 
     def __init__(
         self, factory: Callable[[...], Any] | None = None,
         fields: Mapping[str, FieldFactory[Any]] | None = None,
         finalizers: list[Callable[[], Awaitable[None] | None]] | None = None,
     ):
         self._factory = factory
         self._field_factories = fields or {}
         self._finalizers = finalizers or []
         self._params: dict[str, Any] = {}
         self._object = None
         self._ident = str(uuid4())
         self._parent: Context | None = None
+        self._prev: Context | None = None
 
     @property
     def ident(self) -> str:
         return self._ident
 
     def __enter__(self) -> Any:
         raise NotImplementedError
@@ -45,57 +48,84 @@
     async def __aenter__(self) -> Any:
         raise NotImplementedError
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         raise NotImplementedError
 
 
-_ctx: ContextVar[Context] = ContextVar('_ctx')
+class _ContextStorage(threading.local):
+    __slots__ = ('_storage',)
 
+    def __init__(self):
+        self._storage: dict[type, list[Context]] = defaultdict(list)
 
-def get_context() -> Context | None:
-    return _ctx.get(None)
+    def add(self, kind: type, instance: Context):
+        self._storage[kind].append(instance)
 
+    def remove(self, kind: type, instance: Context):
+        self._storage[kind].remove(instance)
 
-def current_scope_id() -> str:
-    if ctx := _ctx.get(None):
-        return ctx.ident
-    elif loop := get_asyncio_loop():
-        return str(id(asyncio.current_task(loop)))
+    def get_last(self, kind: type) -> Context | None:
+        if objects := self._storage.get(kind, []):
+            return objects[0]
+        return None
+
+
+_current_context: ContextVar[Context] = ContextVar('_ctx')
+_context_storage = _ContextStorage()
+
+
+def current_context(kind: type | None = None) -> Context | None:
+    if kind is None:
+        return _current_context.get(None)
     else:
-        return str(threading.current_thread().ident)
+        return _context_storage.get_last(kind)
+
+
+def current_scope_id(kind: type | None = None) -> str:
+    if kind is None:
+        if ctx := _current_context.get(None):
+            return ctx.ident
+    else:
+        if ctx := _context_storage.get_last(kind):
+            return ctx.ident
+
+    if loop := get_asyncio_loop():
+        return f'asyncio:{id(asyncio.current_task(loop))}'
+    else:
+        return f'thread:{threading.current_thread().ident}'
 
 
 class SyncContext[T](Context, ContextManager):
     __slots__ = (
         '_sync_stack', '_sub_contexts', '_counter', '_lock',
     )
 
     def __init__(
         self, factory: Callable[[...], T] | None = None,
         fields: Mapping[str, FieldFactory[T]] | None = None,
         finalizers: list[Callable[[], Awaitable[None] | None]] | None = None,
-        contexts: list[AbstractContextManager[T]] | None = None,
+        contexts: list[Callable[[], AbstractContextManager[T]]] | None = None,
     ):
         super().__init__(factory, fields, finalizers)
         self._sync_stack = ExitStack()
-        self._sub_contexts: list[tuple[AbstractContextManager[T], str | None]] = []
+        self._sub_contexts: list[tuple[Callable[[], AbstractContextManager[T]], str | None]] = []
         self._counter = 0
         self._lock = threading.Lock()
 
         if contexts:
             self._sub_contexts = [(ctx, None) for ctx in contexts]
 
         names_to_remove = []
 
         for name, factory in self._field_factories.items():
-            if isinstance(factory, AbstractContextManager):
+            if inspect.isgeneratorfunction(inspect.unwrap(factory)):
                 self._sub_contexts.append((factory, name))
                 names_to_remove.append(name)
-            elif isinstance(factory, AbstractAsyncContextManager):
+            elif inspect.isasyncgenfunction(inspect.unwrap(factory)):
                 names_to_remove.append(name)
 
         for name in names_to_remove:
             self._field_factories.pop(name)
 
     def _create(self):
         if self._factory is not None:
@@ -118,36 +148,41 @@
             if 1 != self._counter:
                 self._nested_enter()
                 return self._object
 
         self._sync_stack.__enter__()
 
         for ctx, field in self._sub_contexts:
-            if value := self._sync_stack.enter_context(ctx):
+            if value := self._sync_stack.enter_context(ctx()):
                 if field is not None:
                     self._params[field] = value
 
         for name, value in self._field_factories.items():
             if callable(value):
                 value = invoke_sync(value)
             self._params[name] = value
 
         self._create()
-        self._parent = _ctx.get(None)
-        _ctx.set(self)
+
+        self._prev = _current_context.get(None)
+        _current_context.set(self)
+        self._parent = _context_storage.get_last(type(self._object))
+        _context_storage.add(type(self._object), self)
         return self._object
 
     @override
     def __exit__(self, exc_type, exc_value, traceback):
         with self._lock:
             self._counter = max(self._counter - 1, 0)
             if 0 != self._counter:
                 self._nested_exit()
                 return
 
+        _context_storage.remove(type(self._object), self)
+
         try:
             self._destroy()
         except Exception:
             pass
 
         for name, value in self._field_factories.items():
             self._params.pop(name, None)
@@ -163,51 +198,52 @@
 
         for finalizer in self._finalizers:
             try:
                 invoke_sync(finalizer)
             except Exception:
                 pass
 
-        _ctx.set(self._parent)
+        _current_context.set(self._prev)
+        self._prev = self._parent = None
 
 
 class AsyncContext[T](Context, AsyncContextManager):
     __slots__ = (
         '_sync_stack', '_async_stack', '_sync_sub_contexts',
         '_async_sub_contexts', '_counter', '_lock',
     )
 
     def __init__(
         self, factory: Callable[[...], T] | None = None,
         fields: Mapping[str, FieldFactory[T]] | None = None,
         finalizers: list[Callable[[], Awaitable[None] | None]] | None = None,
-        contexts: list[AbstractContextManager[T] | AbstractAsyncContextManager[T]] | None = None,
+        contexts: list[Callable[[], AbstractContextManager[T] | AbstractAsyncContextManager[T]]] | None = None,
     ):
         super().__init__(factory, fields, finalizers)
         self._sync_stack = ExitStack()
         self._async_stack = AsyncExitStack()
-        self._sync_sub_contexts: list[tuple[AbstractContextManager[T], str | None]] = []
-        self._async_sub_contexts: list[tuple[AbstractAsyncContextManager[T], str | None]] = []
+        self._sync_sub_contexts: list[tuple[Callable[[], AbstractContextManager[T]], str | None]] = []
+        self._async_sub_contexts: list[tuple[Callable[[], AbstractAsyncContextManager[T]], str | None]] = []
         self._counter = 0
         self._lock = asyncio.Lock()
 
         if contexts:
             for ctx in contexts:
-                if isinstance(ctx, AbstractAsyncContextManager):
+                if inspect.isasyncgenfunction(inspect.unwrap(ctx)):
                     self._async_sub_contexts.append((ctx, None))
-                elif isinstance(ctx, AbstractContextManager):
+                elif inspect.isgeneratorfunction(inspect.unwrap(ctx)):
                     self._sync_sub_contexts.append((ctx, None))
 
         names_to_remove = []
 
         for name, factory in self._field_factories.items():
-            if isinstance(factory, AbstractAsyncContextManager):
+            if inspect.isasyncgenfunction(inspect.unwrap(factory)):
                 self._async_sub_contexts.append((factory, name))
                 names_to_remove.append(name)
-            elif isinstance(factory, AbstractContextManager):
+            elif inspect.isgeneratorfunction(inspect.unwrap(factory)):
                 self._sync_sub_contexts.append((factory, name))
                 names_to_remove.append(name)
 
         for name in names_to_remove:
             self._field_factories.pop(name)
 
     async def _create(self):
@@ -232,41 +268,46 @@
                 await self._nested_enter()
                 return self._object
 
         self._sync_stack.__enter__()
         await self._async_stack.__aenter__()
 
         for ctx, field in self._sync_sub_contexts:
-            if value := self._sync_stack.enter_context(ctx):
+            if value := self._sync_stack.enter_context(ctx()):
                 if field is not None:
                     self._params[field] = value
 
         for ctx, field in self._async_sub_contexts:
-            if value := await self._async_stack.enter_async_context(ctx):
+            if value := await self._async_stack.enter_async_context(ctx()):
                 if field is not None:
                     self._params[field] = value
 
         for name, value in self._field_factories.items():
             if callable(value):
                 value = await invoke_async(value)
             self._params[name] = value
 
         await self._create()
-        self._parent = _ctx.get(None)
-        _ctx.set(self)
+
+        self._prev = _current_context.get(None)
+        _current_context.set(self)
+        self._parent = _context_storage.get_last(type(self._object))
+        _context_storage.add(type(self._object), self)
         return self._object
 
     @override
     async def __aexit__(self, exc_type, exc_value, traceback):
         async with self._lock:
             self._counter = max(self._counter - 1, 0)
             if 0 != self._counter:
                 await self._nested_exit()
                 return
 
+        _context_storage.remove(type(self._object), self)
+
         try:
             await self._destroy()
         except Exception:
             pass
 
         for name, value in self._field_factories.items():
             self._params.pop(name, None)
@@ -291,28 +332,29 @@
 
         for finalizer in self._finalizers:
             try:
                 await invoke_async(finalizer)
             except Exception:
                 pass
 
-        _ctx.set(self._parent)
+        _current_context.set(self._prev)
+        self._prev = self._parent = None
 
 
 class SyncContextBuilder[T]:
     def __init__(self, factory: Callable[[...], T]):
         self._factory = factory
         self._fields = {}
         self._finalizers = []
         self._contexts = []
 
     def add_param(self, name: str, value: FieldFactory[T]):
         self._fields[name] = value
 
-    def add_context(self, context: AbstractContextManager[T]):
+    def add_context(self, context: Callable[[], AbstractContextManager[T]]):
         self._contexts.append(context)
 
     def add_finalizer(self, finalizer: Callable[[], Awaitable[None] | None]):
         self._finalizers.append(finalizer)
 
     def build(self) -> SyncContext[T]:
         return SyncContext[T](
@@ -327,15 +369,15 @@
         self._fields = {}
         self._finalizers = []
         self._contexts = []
 
     def add_param(self, name: str, value: FieldFactory[T]):
         self._fields[name] = value
 
-    def add_context(self, context: AbstractContextManager[T] | AbstractAsyncContextManager[T]):
+    def add_context(self, context: Callable[[], AbstractContextManager[T] | AbstractAsyncContextManager[T]]):
         self._contexts.append(context)
 
     def add_finalizer(self, finalizer: Callable[[], Awaitable[None] | None]):
         self._finalizers.append(finalizer)
 
     def build(self) -> AsyncContext[T]:
         return AsyncContext[T](
```

### Comparing `greyhorse-0.4.2/greyhorse/app/entities/application.py` & `greyhorse-0.4.3/greyhorse/app/entities/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from greyhorse.result import Result
 from .controller import Controller, ControllerKey
 from .module import Module, ModuleErrorsItem, ModuleProviderItem
 from .service import Service, ServiceKey
 from ..errors import AppNotLoadedError
 from ...i18n import tr
 from ...logging import logger
-from ...utils.invoke import get_asyncio_loop
+from ...utils.invoke import get_asyncio_loop, caller_path
 
 if TYPE_CHECKING:
     from ..schemas.module import ModuleDesc
 
 
 class Application:
     def __init__(
@@ -114,15 +114,16 @@
 
     def load(self, module_path: str, args: dict[str, Any] | None = None) -> Result:
         from ..builders.module import ModuleBuilder
         from ..schemas.module import ModuleDesc
 
         logger.info(tr('app.application.try-load').format(module_path=module_path))
 
-        root_desc = ModuleDesc(path=module_path, args=args or {}, _initpath='')
+        root_desc = ModuleDesc(path=module_path, args=args or {})
+        root_desc._initpath = caller_path(2)
         builder = ModuleBuilder(self, root_desc)
 
         res = builder.load_pass()
         if not res.success:
             return res
 
         self._root_desc = root_desc
```

### Comparing `greyhorse-0.4.2/greyhorse/app/entities/controller.py` & `greyhorse-0.4.3/greyhorse/app/entities/controller.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/entities/deps.py` & `greyhorse-0.4.3/greyhorse/app/entities/deps.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/entities/module.py` & `greyhorse-0.4.3/greyhorse/app/entities/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/entities/providers.py` & `greyhorse-0.4.3/greyhorse/app/entities/providers.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/entities/service.py` & `greyhorse-0.4.3/greyhorse/app/entities/service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import threading
 from abc import ABC, abstractmethod
-from typing import Awaitable, Callable, Mapping, TYPE_CHECKING, cast
+from typing import Awaitable, Callable, Mapping, TYPE_CHECKING, cast, override
 
 from greyhorse.result import Result
 from .deps import DepsProvider
 from .operator import OperatorFactoryFn, OperatorFactoryRegistry, OperatorKey
 from .providers import ProviderFactoryFn, ProviderFactoryRegistry, ProviderKey
 from ..errors import NoOpFoundForPattern, NoProvFoundForPattern, OpPolicyViolation, ProvPolicyViolation
 from ..utils.registry import DictRegistry, KeyMapping
@@ -165,7 +165,67 @@
 
         for p in policies_dict.values():
             logger.warn(tr('app.entities.provider-unused-policy').format(
                 type='service', name=self.name, key=str(p.key.__name__), pattern=p.name_pattern or '-',
             ))
 
         return Result.from_ok(key_mapping)
+
+
+class SyncService(Service, ABC):
+    def __init__(self, name: str):
+        super().__init__(name)
+        self._event = threading.Event()
+
+    @property
+    def active(self) -> bool:
+        return not self._event.is_set()
+
+    @override
+    def create(self) -> Result:
+        return Result.from_ok()
+
+    @override
+    def destroy(self) -> Result:
+        return Result.from_ok()
+
+    @override
+    def start(self) -> None:
+        self._event.clear()
+
+    @override
+    def stop(self) -> None:
+        self._event.set()
+
+    @override
+    def wait(self) -> threading.Event:
+        return self._event
+
+
+class AsyncService(Service, ABC):
+    def __init__(self, name: str):
+        super().__init__(name)
+        self._event = asyncio.Event()
+
+    @property
+    def active(self) -> bool:
+        return not self._event.is_set()
+
+    @override
+    async def create(self) -> Result:
+        return Result.from_ok()
+
+    @override
+    async def destroy(self) -> Result:
+        return Result.from_ok()
+
+    @override
+    async def start(self) -> None:
+        self._event.clear()
+
+    @override
+    async def stop(self) -> None:
+        self._event.set()
+
+    @override
+    def wait(self) -> asyncio.Event:
+        return self._event
```

### Comparing `greyhorse-0.4.2/greyhorse/app/errors.py` & `greyhorse-0.4.3/greyhorse/app/errors.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/schemas/components.py` & `greyhorse-0.4.3/greyhorse/app/schemas/components.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/schemas/controller.py` & `greyhorse-0.4.3/greyhorse/app/schemas/controller.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/schemas/module.py` & `greyhorse-0.4.3/greyhorse/app/schemas/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/schemas/service.py` & `greyhorse-0.4.3/greyhorse/app/schemas/service.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/tasks/app.py` & `greyhorse-0.4.3/greyhorse/app/tasks/app.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/app/utils/registry.py` & `greyhorse-0.4.3/greyhorse/app/utils/registry.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/cache/base.py` & `greyhorse-0.4.3/greyhorse/data/cache/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/cache/method.py` & `greyhorse-0.4.3/greyhorse/data/cache/method.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/models/base.py` & `greyhorse-0.4.3/greyhorse/data/models/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/models/fields.py` & `greyhorse-0.4.3/greyhorse/data/models/fields.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/models/filterable.py` & `greyhorse-0.4.3/greyhorse/data/models/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/models/model.py` & `greyhorse-0.4.3/greyhorse/data/models/model.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/models/serializable.py` & `greyhorse-0.4.3/greyhorse/data/models/serializable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/repositories/base.py` & `greyhorse-0.4.3/greyhorse/data/repositories/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/repositories/filterable.py` & `greyhorse-0.4.3/greyhorse/data/repositories/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/serializers/base.py` & `greyhorse-0.4.3/greyhorse/data/serializers/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/serializers/pickle.py` & `greyhorse-0.4.3/greyhorse/data/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/data/storage.py` & `greyhorse-0.4.3/greyhorse/data/storage.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/i18n/translator.py` & `greyhorse-0.4.3/greyhorse/i18n/translator.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/logging.py` & `greyhorse-0.4.3/greyhorse/logging.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/messagebus.py` & `greyhorse-0.4.3/greyhorse/messagebus.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/result.py` & `greyhorse-0.4.3/greyhorse/result.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/translations.toml` & `greyhorse-0.4.3/greyhorse/translations.toml`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/utils/dicts.py` & `greyhorse-0.4.3/greyhorse/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/utils/hashes.py` & `greyhorse-0.4.3/greyhorse/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/utils/injectors.py` & `greyhorse-0.4.3/greyhorse/utils/injectors.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/utils/invoke.py` & `greyhorse-0.4.3/greyhorse/utils/invoke.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/utils/strings.py` & `greyhorse-0.4.3/greyhorse/utils/strings.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/greyhorse/utils/time.py` & `greyhorse-0.4.3/greyhorse/utils/time.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.2/pyproject.toml` & `greyhorse-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse"
-version = "0.4.2"
+version = "0.4.3"
 description = "Greyhorse library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `greyhorse-0.4.2/PKG-INFO` & `greyhorse-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greyhorse
-Version: 0.4.2
+Version: 0.4.3
 Summary: Greyhorse library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
```

