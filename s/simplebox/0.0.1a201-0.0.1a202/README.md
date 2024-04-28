# Comparing `tmp/simplebox-0.0.1a201-py3-none-any.whl.zip` & `tmp/simplebox-0.0.1a202-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 459117 bytes, number of entries: 157
--rw-rw-rw-  2.0 fat     5191 b- defN 24-Apr-27 07:48 simplebox/__init__.py
+Zip file size: 460219 bytes, number of entries: 158
+-rw-rw-rw-  2.0 fat     5191 b- defN 24-Apr-28 17:17 simplebox/__init__.py
 -rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-07 16:46 simplebox/backend.py
 -rw-rw-rw-  2.0 fat    17626 b- defN 24-Apr-07 16:46 simplebox/character.py
 -rw-rw-rw-  2.0 fat     4829 b- defN 24-Apr-14 15:04 simplebox/classes.py
 -rw-rw-rw-  2.0 fat    16962 b- defN 24-Apr-20 14:21 simplebox/cmd.py
 -rw-rw-rw-  2.0 fat     5481 b- defN 23-Nov-14 15:01 simplebox/converter.py
 -rw-rw-rw-  2.0 fat     1638 b- defN 24-Apr-07 15:02 simplebox/enums.py
 -rw-rw-rw-  2.0 fat      306 b- defN 23-May-31 16:53 simplebox/generic.py
@@ -143,17 +143,18 @@
 -rw-rw-rw-  2.0 fat       47 b- defN 23-Mar-20 13:52 simplebox/scheduler/_cron/__init__.py
 -rw-rw-rw-  2.0 fat      226 b- defN 23-Mar-20 13:52 simplebox/scheduler/_cron/_expressions.py
 -rw-rw-rw-  2.0 fat      783 b- defN 23-Mar-25 15:32 simplebox/scheduler/_cron/_fields.py
 -rw-rw-rw-  2.0 fat       47 b- defN 23-May-03 14:12 simplebox/utils/__init__.py
 -rw-rw-rw-  2.0 fat    16556 b- defN 24-Apr-18 15:30 simplebox/utils/computer.py
 -rw-rw-rw-  2.0 fat     2173 b- defN 24-Apr-07 15:48 simplebox/utils/enums.py
 -rw-rw-rw-  2.0 fat     2735 b- defN 24-Apr-27 14:18 simplebox/utils/locks.py
--rw-rw-rw-  2.0 fat    13702 b- defN 24-Apr-27 07:11 simplebox/utils/objects.py
+-rw-rw-rw-  2.0 fat    14864 b- defN 24-Apr-28 15:25 simplebox/utils/objects.py
 -rw-rw-rw-  2.0 fat     3258 b- defN 24-Apr-14 14:42 simplebox/utils/optionals.py
+-rw-rw-rw-  2.0 fat     3230 b- defN 24-Apr-28 17:10 simplebox/utils/reflect.py
 -rw-rw-rw-  2.0 fat    19546 b- defN 24-Apr-07 15:48 simplebox/utils/strings.py
 -rw-rw-rw-  2.0 fat      247 b- defN 23-Feb-28 15:31 simplebox/valid/__init__.py
 -rw-rw-rw-  2.0 fat    16632 b- defN 24-Apr-15 17:12 simplebox/valid/_validator.py
--rw-rw-rw-  2.0 fat     1358 b- defN 24-Apr-27 14:29 simplebox-0.0.1a201.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 14:29 simplebox-0.0.1a201.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-27 14:29 simplebox-0.0.1a201.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    13672 b- defN 24-Apr-27 14:29 simplebox-0.0.1a201.dist-info/RECORD
-157 files, 1442231 bytes uncompressed, 437549 bytes compressed:  69.7%
+-rw-rw-rw-  2.0 fat     1279 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    13755 b- defN 24-Apr-28 17:17 simplebox-0.0.1a202.dist-info/RECORD
+158 files, 1446627 bytes uncompressed, 438523 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -444,29 +444,32 @@
 
 Filename: simplebox/utils/objects.py
 Comment: 
 
 Filename: simplebox/utils/optionals.py
 Comment: 
 
+Filename: simplebox/utils/reflect.py
+Comment: 
+
 Filename: simplebox/utils/strings.py
 Comment: 
 
 Filename: simplebox/valid/__init__.py
 Comment: 
 
 Filename: simplebox/valid/_validator.py
 Comment: 
 
-Filename: simplebox-0.0.1a201.dist-info/METADATA
+Filename: simplebox-0.0.1a202.dist-info/METADATA
 Comment: 
 
-Filename: simplebox-0.0.1a201.dist-info/WHEEL
+Filename: simplebox-0.0.1a202.dist-info/WHEEL
 Comment: 
 
-Filename: simplebox-0.0.1a201.dist-info/top_level.txt
+Filename: simplebox-0.0.1a202.dist-info/top_level.txt
 Comment: 
 
-Filename: simplebox-0.0.1a201.dist-info/RECORD
+Filename: simplebox-0.0.1a202.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplebox/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
-__version__ = "0.0.1.alpha201"
+__version__ = "0.0.1.alpha202"
 
 banner = f"""
  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------. 
 | .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. |
 | |    _______   | || |     _____    | || | ____    ____ | || |   ______     | || |   _____      | || |  _________   | || |   ______     | || |     ____     | || |  ____  ____  | |
 | |   /  ___  |  | || |    |_   _|   | || ||_   \  /   _|| || |  |_   __ \   | || |  |_   _|     | || | |_   ___  |  | || |  |_   _ \    | || |   .'    `.   | || | |_  _||_  _| | |
 | |  |  (__ \_|  | || |      | |     | || |  |   \/   |  | || |    | |__) |  | || |    | |       | || |   | |_  \_|  | || |    | |_) |   | || |  /  .--.  \  | || |   \ \  / /   | |
```

## simplebox/utils/objects.py

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 from inspect import stack, getframeinfo, currentframe
 from random import sample
 from collections.abc import Iterable
+from typing import Any
 
 import regex as re
 from regex import findall
 
+from .._handler._str_handler import _strings
 from ..classes import StaticClass
 from ..exceptions import raise_exception, NonePointerException
 from ..generic import V, T
 
 _base_str = 'ABCDEFGHIGKLMNOPQRSTUVWXYZabcdefghigklmnopqrstuvwxyz0123456789'
 loc = locals()
 
@@ -238,58 +240,46 @@
         :param default: Default value
         """
         if src:
             return src
         return default
 
     @staticmethod
-    def generate_random_str(length: int = 16, base_str: str = None, prefix: str = '', suffix: str = '') -> str:
+    def generate_random_str(length: int = 16, base_str: str = _base_str, prefix: str = '', suffix: str = '') -> str:
         """
         Generates a random string of a specified length
         :params length:  of generated string
         """
         ObjectsUtils.check_type(length, int)
         ObjectsUtils.check_type(base_str, str)
         ObjectsUtils.check_type(prefix, str)
         ObjectsUtils.check_type(suffix, str)
-        if len(base_str) == 0 or length == 0:
+        if _strings.is_black(base_str) or length == 0:
             return ""
         base_str_len = len(base_str)
         if length <= base_str_len:
             content = "".join(sample(base_str, length))
         else:
             strings = []
             step = length // base_str_len
             remainder = length % base_str_len
             for _ in range(step):
                 strings.extend(sample(base_str, base_str_len))
             strings.extend(sample(base_str, remainder))
             content = "".join(strings)
-        return f'{suffix}{content}{prefix}'
+        return f'{prefix}{content}{suffix}'
 
     @staticmethod
     def get_current_function_name() -> str:
         """
         Gets the name of the current function inside the function
         """
         return stack()[1][3]
 
     @staticmethod
-    def get_private_attribute(obj, name: str):
-        """
-        Gets the private property value of the object, and if it is a private method, returns the function object.
-        """
-        obj_name = obj.__class__.__name__
-        for attribute in obj.__dir__():
-            attr_name = f"_{obj_name}{name}"
-            if obj_name in attribute and attr_name == attribute:
-                return getattr(obj, attr_name)
-        return None
-
-    @staticmethod
     def call_limit(func_file=None, func_names=None):
         """
         Limit the call of functions
         example:
             a.py
                 def inner_f1():
                     # expect to only be called in the a.py
@@ -311,40 +301,82 @@
                     raise RuntimeError(f"'{name}' is restricted from being called.")
                 else:
                     raise RuntimeError(f"limit calls.")
             else:
                 raise RuntimeError(f"'{called.function}' is restricted from being called.")
 
     @staticmethod
-    def check_type(src_type, except_type: type or tuple[type]):
+    def check_type(obj, *except_types: type):
         """
         check that src_type is a subclass of except_type.
         """
-        if isinstance(except_type, tuple):
-            for t in except_type:
-                if not isinstance(t, type):
-                    raise TypeError(f'excepted type is \'type\', got a \'{type(t).__name__}\'')
-        else:
-            if not isinstance(except_type, type):
-                raise TypeError(f'excepted type is \'type\', got a \'{type(except_type).__name__}\'')
+        for t in except_types:
+            if not issubclass(t_ := type(t), type):
+                raise TypeError(f'excepted type is \'type\', got a \'{t_.__name__}\'')
+
+        if not issubclass(t_ := type(obj), except_types):
+            raise TypeError(f'"{obj}": excepted type in \'{[t.__name__ for t in except_types]}\', '
+                            f'got a \'{t_.__name__}\'')
 
-        if not issubclass(t_ := type(src_type), except_type):
-            raise TypeError(f'excepted type is \'{except_type.__name__}\', got a \'{t_.__name__}\'')
+    @staticmethod
+    def check_iter_type(objs: iter, except_type: type):
+        """
+        check if an element in objs is a subclass of the except_type
+        usage:
+            check_iter_type('a', 'b', 'c', str) => ok
+
+            check_iter_type('a', 1, 'b', str) => raise exception
+        """
+        if not objs:
+            return
+        if not isinstance(t_ := type(except_type), type):
+            raise TypeError(f'excepted type is \'type\', got a \'{t_.__name__}\'')
+        for obj in objs:
+            if not issubclass(t_ := type(obj), except_type):
+                raise TypeError(f'"{obj}": excepted type is \'{except_type.__name__}\', got a \'{t_.__name__}\'')
 
     @staticmethod
-    def check_instance(instance, except_type: type or tuple[type]):
+    def check_types(*metas: tuple[Any, tuple[type]]):
+        """
+        ObjectsUtils.check_type's wrapper function.
+        usage:
+            check_types((obj, (str, int)), (obj, (list, dict)))
+        """
+        for obj, except_types in metas:
+            ObjectsUtils.check_type(obj, *except_types)
+
+    @staticmethod
+    def check_instance(instance, *except_types: type):
         """
         check that instance is an instance of except_type.
+        """
+        for t in except_types:
+            if not issubclass(t_ := type(t), type):
+                raise TypeError(f'except_type excepted type is \'type\', got a \'{t_.__name__}\'')
 
+        if not isinstance(instance, except_types):
+            raise TypeError(f'"{instance}": excepted type is \'{[t.__name__ for t in except_types]}\', '
+                            f'got a \'{type(instance).__name__}\'')
+
+    @staticmethod
+    def check_iter_instance(instances, except_type: type):
+        """
+        Check if an element in instances is an instance of except_type.
+        """
+        if not issubclass(t := type(except_type), type):
+            raise TypeError(f'except_type excepted type is \'type\', got a \'{t.__name__}\'')
+
+        for instance in instances:
+            if not isinstance(instance, except_type):
+                raise TypeError(f'"{instance}": excepted type is \'{except_type.__name__}\', '
+                                f'got a \'{type(instance).__name__}\'')
+
+    @staticmethod
+    def check_instances(*metas: tuple[Any, tuple[type]]):
+        """
+        ObjectsUtils.check_instance's wrapper function.
         """
-        if isinstance(except_type, tuple):
-            for t in except_type:
-                if not isinstance(t, type):
-                    raise TypeError(f'except_type excepted type is \'type\', got a \'{type(t).__name__}\'')
-        else:
-            if not isinstance(except_type, type):
-                raise TypeError(f'excepted type is \'type\', got a \'{type(except_type).__name__}\'')
-        if not isinstance(instance, except_type):
-            raise TypeError(f'excepted type is \'{except_type.__name__}\', got a \'{type(instance).__name__}\'')
+        for instance, except_types in metas:
+            ObjectsUtils.check_instance(instance, *except_types)
 
 
 __all__ = [ObjectsUtils]
```

## Comparing `simplebox-0.0.1a201.dist-info/METADATA` & `simplebox-0.0.1a202.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplebox
-Version: 0.0.1a201
+Version: 0.0.1a202
 Summary: 简易工具箱。
 Author: fuck
 License: MIT Licence
 Keywords: pip,simplebox,backend,fast,fasttools,box,simple
 Platform: any
 Requires-Python: >=3.9
 Requires-Dist: psutil (==5.9.2)
@@ -16,16 +16,14 @@
 Requires-Dist: flameprof (==0.4)
 Requires-Dist: jsonpath (==0.82)
 Requires-Dist: ujson (==5.7.0)
 Requires-Dist: rfc3986 (<2.0,>=1.1.0)
 Requires-Dist: brotlipy (<1.0,>=0.7.0)
 Requires-Dist: service-identity (==24.1.0)
 Requires-Dist: pyOpenSSL (==24.1.0)
-Requires-Dist: urllib3 (==1.26.18)
-Requires-Dist: charset-normalizer (==2.1.1)
 Requires-Dist: DBUtils (==3.1.0)
 Requires-Dist: pymysql (==1.1.0)
 Requires-Dist: sqlalchemy (==2.0.29)
 Requires-Dist: cx-Oracle (==8.3.0)
 
 
     工具箱主要提供以下功能：
```

## Comparing `simplebox-0.0.1a201.dist-info/RECORD` & `simplebox-0.0.1a202.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-simplebox/__init__.py,sha256=hvpTpjw8H-8gnPMDLqSoVAFf9DlRNXWzqnwuDfCH8xs,5191
+simplebox/__init__.py,sha256=qUTuapyqk8pfIuui1WMsjR8M6kcRmq2uFIuNs75GAbQ,5191
 simplebox/backend.py,sha256=yR3gveO0iKcTKWKW5K57513u-s7O3oGes84Kp8HUZho,2090
 simplebox/character.py,sha256=NEbQqFmD3rpkl_E3MeES7rRfAmtc_DJHoKcF8GNK92g,17626
 simplebox/classes.py,sha256=vGD0PVglh-Nlz8I3PTqDmDquQf_Z2BNoXIvp9aRS140,4829
 simplebox/cmd.py,sha256=5SK-ne4vAyjNdEztS0TyMWUuQC6bBc4RCtnbdQBvVF4,16962
 simplebox/converter.py,sha256=DZ_sb-ZBIorTZAlpuNyGjxnlPAjtSp7yKMIDSiwws0g,5481
 simplebox/enums.py,sha256=KzziG7TboPMIENPrc4HrsUagSEMd4JfLFG6Bn2T0HAs,1638
 simplebox/generic.py,sha256=tBDzlqFHQ7I6bb8_iC9PEqyMaD0sxJee9a7zR3YwxRw,306
@@ -142,16 +142,17 @@
 simplebox/scheduler/_cron/__init__.py,sha256=CtZuEO8oVkrRxwm4_fsQYg0wdQ6o3znWt5v6hZ1BBgc,47
 simplebox/scheduler/_cron/_expressions.py,sha256=fBtOoIHV3wjv9PlKgnALqtccU0U39M3jxE0sbh_gf14,226
 simplebox/scheduler/_cron/_fields.py,sha256=iYBrX15zyYSSwmwDc1fSl0tAux_0OXPBGbzF0Io1eGQ,783
 simplebox/utils/__init__.py,sha256=CtZuEO8oVkrRxwm4_fsQYg0wdQ6o3znWt5v6hZ1BBgc,47
 simplebox/utils/computer.py,sha256=WYBYAbZ2ViWUMjNW8LtutFpKHfgpr-wg4kcim3DKWk4,16556
 simplebox/utils/enums.py,sha256=rwMAmDqUFy2iJey9v0aThBCAFcR-tKqVI9LELw4BKcw,2173
 simplebox/utils/locks.py,sha256=KP_utNUBYeWjJhsWzu1-rn5sG6jzi2cDrFXtSmgJCHE,2735
-simplebox/utils/objects.py,sha256=jMVj-Iz1htBCeLjaSEzp072GrzZqAN9OFV3MjP1dEHI,13702
+simplebox/utils/objects.py,sha256=jaTS8DaHdrdspANFzol2ad6UKRQnFCPCvHHnSu5R2d4,14864
 simplebox/utils/optionals.py,sha256=XDlteLGkfbWHOgJPdGykE-a79Ae-P7Fbfsabmiwdjuw,3258
+simplebox/utils/reflect.py,sha256=My7m5kCd08gjFfg31Pg0l-l0XjNmt971lneX6Wg6J5U,3230
 simplebox/utils/strings.py,sha256=yvdvMVI-ULs-DIWElpmjdYHp9CPLbETc5M-16L9gflk,19546
 simplebox/valid/__init__.py,sha256=7deSv2vW7Wj-83Db3JbO0SZK9Pf-G9pDqbCAgkxr8PI,247
 simplebox/valid/_validator.py,sha256=xj3ju6Lpx73bF3NZR9eGHJl_pTk6kPMsFL4hrhbM2cw,16632
-simplebox-0.0.1a201.dist-info/METADATA,sha256=EI7vEwGfKi2jDSXGiWsFJaRTK88Wgy8Lx3e-GpKKtIA,1358
-simplebox-0.0.1a201.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simplebox-0.0.1a201.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
-simplebox-0.0.1a201.dist-info/RECORD,,
+simplebox-0.0.1a202.dist-info/METADATA,sha256=il34JgelsjZRQi5RbUGRBciRxGooavaC-pRPM6vXUdM,1279
+simplebox-0.0.1a202.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simplebox-0.0.1a202.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
+simplebox-0.0.1a202.dist-info/RECORD,,
```

