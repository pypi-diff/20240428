# Comparing `tmp/melobot-2.6.2.tar.gz` & `tmp/melobot-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melobot-2.6.2.tar", last modified: Tue Apr 23 12:21:59 2024, max compression
+gzip compressed data, was "melobot-2.6.3.tar", last modified: Sun Apr 28 16:09:21 2024, max compression
```

## Comparing `melobot-2.6.2.tar` & `melobot-2.6.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1545 2024-04-17 07:58:06.600008 melobot-2.6.2/LICENSE-BSD
--rw-r--r--   0        0        0    20137 2024-04-17 10:10:23.406233 melobot-2.6.2/LICENSE-CC
--rw-r--r--   0        0        0     6410 2024-04-23 09:16:57.730052 melobot-2.6.2/README.md
--rw-r--r--   0        0        0     2651 2024-04-23 12:21:59.826860 melobot-2.6.2/pyproject.toml
--rw-r--r--   0        0        0      899 2024-04-23 10:40:08.419597 melobot-2.6.2/src/melobot/__init__.py
--rw-r--r--   0        0        0      413 2024-04-12 17:28:27.036962 melobot-2.6.2/src/melobot/base/__init__.py
--rw-r--r--   0        0        0    17110 2024-04-23 06:33:35.551425 melobot-2.6.2/src/melobot/base/abc.py
--rw-r--r--   0        0        0     1580 2024-04-22 08:16:24.050474 melobot-2.6.2/src/melobot/base/exceptions.py
--rw-r--r--   0        0        0    25436 2024-04-23 10:21:36.234391 melobot-2.6.2/src/melobot/base/tools.py
--rw-r--r--   0        0        0     3528 2024-04-20 15:16:09.229494 melobot-2.6.2/src/melobot/base/typing.py
--rw-r--r--   0        0        0      275 2024-04-20 16:29:46.707838 melobot-2.6.2/src/melobot/bot/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-13 14:31:36.963226 melobot-2.6.2/src/melobot/bot/hook.py
--rw-r--r--   0        0        0    17258 2024-04-21 16:44:04.275640 melobot-2.6.2/src/melobot/bot/init.py
--rw-r--r--   0        0        0     1295 2024-04-23 06:54:20.343255 melobot-2.6.2/src/melobot/context/__init__.py
--rw-r--r--   0        0        0    58081 2024-04-23 08:29:24.968118 melobot-2.6.2/src/melobot/context/action.py
--rw-r--r--   0        0        0    24809 2024-04-22 12:11:11.998149 melobot-2.6.2/src/melobot/context/session.py
--rw-r--r--   0        0        0        0 2024-04-12 17:28:27.040296 melobot-2.6.2/src/melobot/controller/__init__.py
--rw-r--r--   0        0        0     3843 2024-04-14 16:46:28.378025 melobot-2.6.2/src/melobot/controller/dispatcher.py
--rw-r--r--   0        0        0     2609 2024-04-22 12:52:49.846117 melobot-2.6.2/src/melobot/controller/responder.py
--rw-r--r--   0        0        0      168 2024-04-13 14:35:10.206863 melobot-2.6.2/src/melobot/io/__init__.py
--rw-r--r--   0        0        0    12244 2024-04-22 09:33:08.877780 melobot-2.6.2/src/melobot/io/duplex_http.py
--rw-r--r--   0        0        0     9874 2024-04-22 09:33:15.127783 melobot-2.6.2/src/melobot/io/forward_ws.py
--rw-r--r--   0        0        0     9674 2024-04-22 09:40:10.368679 melobot-2.6.2/src/melobot/io/reverse_ws.py
--rw-r--r--   0        0        0     3419 2024-04-23 12:20:27.062863 melobot-2.6.2/src/melobot/meta.py
--rw-r--r--   0        0        0      567 2024-04-21 07:13:00.995861 melobot-2.6.2/src/melobot/models/__init__.py
--rw-r--r--   0        0        0    25236 2024-04-23 11:41:39.490280 melobot-2.6.2/src/melobot/models/event.py
--rw-r--r--   0        0        0    15066 2024-04-20 17:04:39.132193 melobot-2.6.2/src/melobot/models/msg.py
--rw-r--r--   0        0        0       81 2024-04-12 17:28:27.040296 melobot-2.6.2/src/melobot/plugin/__init__.py
--rw-r--r--   0        0        0    11970 2024-04-20 16:56:47.014982 melobot-2.6.2/src/melobot/plugin/handler.py
--rw-r--r--   0        0        0    41423 2024-04-23 10:37:58.381931 melobot-2.6.2/src/melobot/plugin/init.py
--rw-r--r--   0        0        0     5929 2024-04-13 14:32:53.535365 melobot-2.6.2/src/melobot/plugin/ipc.py
--rw-r--r--   0        0        0      831 2024-04-23 10:35:17.904031 melobot-2.6.2/src/melobot/utils/__init__.py
--rw-r--r--   0        0        0    13171 2024-04-23 10:34:43.350432 melobot-2.6.2/src/melobot/utils/checker.py
--rw-r--r--   0        0        0     7445 2024-04-20 16:59:58.711851 melobot-2.6.2/src/melobot/utils/logger.py
--rw-r--r--   0        0        0     4171 2024-04-20 15:28:42.348446 melobot-2.6.2/src/melobot/utils/matcher.py
--rw-r--r--   0        0        0    14005 2024-04-23 10:24:16.008949 melobot-2.6.2/src/melobot/utils/parser.py
--rw-r--r--   0        0        0        0 2024-03-12 08:09:26.000000 melobot-2.6.2/tests/__init__.py
--rw-r--r--   0        0        0     7932 1970-01-01 00:00:00.000000 melobot-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1545 2024-04-17 07:58:06.600008 melobot-2.6.3/LICENSE-BSD
+-rw-r--r--   0        0        0    20137 2024-04-17 10:10:23.406233 melobot-2.6.3/LICENSE-CC
+-rw-r--r--   0        0        0     6410 2024-04-27 07:25:12.715861 melobot-2.6.3/README.md
+-rw-r--r--   0        0        0     2651 2024-04-28 16:09:21.212094 melobot-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0      899 2024-04-23 10:40:08.419597 melobot-2.6.3/src/melobot/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-25 06:54:57.347251 melobot-2.6.3/src/melobot/base/__init__.py
+-rw-r--r--   0        0        0    14200 2024-04-28 11:41:30.921982 melobot-2.6.3/src/melobot/base/abc.py
+-rw-r--r--   0        0        0     1905 2024-04-28 14:19:04.061972 melobot-2.6.3/src/melobot/base/exceptions.py
+-rw-r--r--   0        0        0     1695 2024-04-28 14:08:21.015679 melobot-2.6.3/src/melobot/base/ioc.py
+-rw-r--r--   0        0        0    19367 2024-04-28 12:16:36.012674 melobot-2.6.3/src/melobot/base/tools.py
+-rw-r--r--   0        0        0     4335 2024-04-28 09:08:39.804077 melobot-2.6.3/src/melobot/base/typing.py
+-rw-r--r--   0        0        0      275 2024-04-20 16:29:46.707838 melobot-2.6.3/src/melobot/bot/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-28 09:16:39.055982 melobot-2.6.3/src/melobot/bot/hook.py
+-rw-r--r--   0        0        0    16994 2024-04-28 14:32:27.974288 melobot-2.6.3/src/melobot/bot/init.py
+-rw-r--r--   0        0        0     1295 2024-04-26 09:48:10.186044 melobot-2.6.3/src/melobot/context/__init__.py
+-rw-r--r--   0        0        0    57163 2024-04-28 11:01:20.922336 melobot-2.6.3/src/melobot/context/action.py
+-rw-r--r--   0        0        0    24509 2024-04-28 12:11:14.151158 melobot-2.6.3/src/melobot/context/session.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:28:27.040296 melobot-2.6.3/src/melobot/controller/__init__.py
+-rw-r--r--   0        0        0     3825 2024-04-28 14:28:49.091222 melobot-2.6.3/src/melobot/controller/dispatcher.py
+-rw-r--r--   0        0        0     2593 2024-04-28 12:19:06.360136 melobot-2.6.3/src/melobot/controller/responder.py
+-rw-r--r--   0        0        0      168 2024-04-13 14:35:10.206863 melobot-2.6.3/src/melobot/io/__init__.py
+-rw-r--r--   0        0        0    11595 2024-04-28 14:12:18.210947 melobot-2.6.3/src/melobot/io/duplex_http.py
+-rw-r--r--   0        0        0     9981 2024-04-28 10:38:15.344402 melobot-2.6.3/src/melobot/io/forward_ws.py
+-rw-r--r--   0        0        0     9391 2024-04-28 10:37:59.760909 melobot-2.6.3/src/melobot/io/reverse_ws.py
+-rw-r--r--   0        0        0     3391 2024-04-28 12:15:54.262461 melobot-2.6.3/src/melobot/meta.py
+-rw-r--r--   0        0        0      567 2024-04-21 07:13:00.995861 melobot-2.6.3/src/melobot/models/__init__.py
+-rw-r--r--   0        0        0    24306 2024-04-28 11:01:58.152610 melobot-2.6.3/src/melobot/models/event.py
+-rw-r--r--   0        0        0    15488 2024-04-28 11:24:27.335986 melobot-2.6.3/src/melobot/models/msg.py
+-rw-r--r--   0        0        0       81 2024-04-12 17:28:27.040296 melobot-2.6.3/src/melobot/plugin/__init__.py
+-rw-r--r--   0        0        0    11808 2024-04-28 14:32:23.137546 melobot-2.6.3/src/melobot/plugin/handler.py
+-rw-r--r--   0        0        0    38803 2024-04-28 11:31:26.871233 melobot-2.6.3/src/melobot/plugin/init.py
+-rw-r--r--   0        0        0     5637 2024-04-28 11:44:35.493368 melobot-2.6.3/src/melobot/plugin/ipc.py
+-rw-r--r--   0        0        0      831 2024-04-23 10:35:17.904031 melobot-2.6.3/src/melobot/utils/__init__.py
+-rw-r--r--   0        0        0    12163 2024-04-28 11:48:44.035284 melobot-2.6.3/src/melobot/utils/checker.py
+-rw-r--r--   0        0        0    10622 2024-04-28 11:53:13.540736 melobot-2.6.3/src/melobot/utils/logger.py
+-rw-r--r--   0        0        0     4171 2024-04-20 15:28:42.348446 melobot-2.6.3/src/melobot/utils/matcher.py
+-rw-r--r--   0        0        0    12753 2024-04-28 14:16:06.137565 melobot-2.6.3/src/melobot/utils/parser.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:26:23.449222 melobot-2.6.3/tests/__init__.py
+-rw-r--r--   0        0        0     7932 1970-01-01 00:00:00.000000 melobot-2.6.3/PKG-INFO
```

### Comparing `melobot-2.6.2/LICENSE-BSD` & `melobot-2.6.3/LICENSE-BSD`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/LICENSE-CC` & `melobot-2.6.3/LICENSE-CC`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/README.md` & `melobot-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/pyproject.toml` & `melobot-2.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "2.6.2"
+version = "2.6.3"
 
 [project.license]
 text = "BSD"
 
 [project.urls]
 Homepage = "https://github.com/Meloland/melobot"
 Documentation = "https://docs.melobot.org"
@@ -63,19 +63,19 @@
 [tool.mypy]
 follow_imports = "skip"
 ignore_missing_imports = true
 show_column_numbers = true
 check_untyped_defs = true
 
 [tool.black]
-line-length = 88
+line-length = 90
 
 [tool.isort]
 profile = "black"
-line_length = 88
+line_length = 90
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.version]
 source = "file"
 path = "src/melobot/meta.py"
```

### Comparing `melobot-2.6.2/src/melobot/__init__.py` & `melobot-2.6.3/src/melobot/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/src/melobot/base/abc.py` & `melobot-2.6.3/src/melobot/base/abc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,50 @@
 import asyncio
 import json
 from abc import ABC, abstractmethod
 from copy import deepcopy
-from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING, Logger
+from dataclasses import dataclass
 
 from .exceptions import BotRuntimeError, BotUtilsError, BotValueError
-from .tools import is_retcoro
 from .typing import (
     TYPE_CHECKING,
     Any,
+    AsyncCallable,
     BotLife,
-    Callable,
-    Coroutine,
     Literal,
     LogicMode,
-    ModuleType,
     Optional,
     ParseArgs,
+    TracebackType,
     Type,
     Void,
 )
 
 if TYPE_CHECKING:
     from ..bot.hook import BotHookBus
     from ..controller.dispatcher import BotDispatcher
     from ..controller.responder import BotResponder
     from ..models.event import BotEventBuilder
     from ..plugin.handler import EventHandler
-
-
-class BaseLogger(Logger):
-    """日志器基类
-
-    .. admonition:: 提示
-       :class: tip
-
-       一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
-    """
-
-    LEVEL_MAP = {
-        "DEBUG": DEBUG,
-        "INFO": INFO,
-        "WARNING": WARNING,
-        "ERROR": ERROR,
-        "CRITICAL": CRITICAL,
-    }
-
-    LEVEL_FLAG_NAME = "__LOG_LEVEL_FLAG__"
-
-    def __init__(self, name: str, level: int) -> None:
-        super().__init__(name, level)
-        setattr(self, BaseLogger.LEVEL_FLAG_NAME, level)
-
-    def check_level_flag(
-        self, level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO"
-    ) -> bool:
-        """检查日志器是否可以输出指定日志等级的日志"""
-        return BaseLogger.LEVEL_MAP[level] >= getattr(self, BaseLogger.LEVEL_FLAG_NAME)
-
-    LEVEL_CHECK_METH_NAME = check_level_flag.__name__
+    from ..utils.logger import BotLogger
 
 
 class AbstractConnector(ABC):
     """抽象连接器类
 
     .. admonition:: 提示
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
     def __init__(self, cd_time: float) -> None:
         super().__init__()
         #: 连接器的日志器
-        self.logger: BaseLogger
+        self.logger: "BotLogger"
         #: 是否在 slack 状态
         self.slack: bool = False
         #: 连接器发送行为操作的冷却时间
         self.cd_time = cd_time
 
         self._used: bool = False
         self._ready_signal = asyncio.Event()
@@ -88,15 +55,15 @@
 
     @abstractmethod
     async def __aenter__(self):
         raise NotImplementedError
 
     @abstractmethod
     async def __aexit__(
-        self, exc_type: Type[Exception], exc_val: Exception, exc_tb: ModuleType
+        self, exc_type: Type[Exception], exc_val: Exception, exc_tb: TracebackType
     ) -> bool:
         if exc_type is None:
             return True
         elif exc_type == asyncio.CancelledError:
             return True
         else:
             return False
@@ -106,52 +73,49 @@
 
     def _bind(
         self,
         dispatcher: "BotDispatcher",
         responder: "BotResponder",
         event_builder: Type["BotEventBuilder"],
         bot_bus: "BotHookBus",
-        logger: BaseLogger,
+        logger: "BotLogger",
     ) -> None:
         self._event_builder = event_builder
         self._bot_bus = bot_bus
         self.logger = logger
         self._common_dispatcher = dispatcher
         self._resp_dispatcher = responder
 
     @abstractmethod
     async def _send(self, action: "BotAction") -> None:
         raise NotImplementedError
 
 
 class Flagable:
     def __init__(self) -> None:
-        self._flags_store: Optional[dict[str, dict[str, Any]]] = None
+        self._flags_store: dict[str, dict[str, Any]] = {}
 
     def mark(self, namespace: str, flag_name: str, val: Any = None) -> None:
         """为对象添加在指定命名空间下，名为 flag_name 的标记。 此后此对象会一直携带此标记，无法撤销。"""
-        if self._flags_store is None:
-            self._flags_store = {}
-        if self._flags_store.get(namespace) is None:
-            self._flags_store[namespace] = {}
-        if flag_name in self._flags_store[namespace].keys():
+        self._flags_store.setdefault(namespace, {})
+
+        if self._flags_store[namespace].get(flag_name) is not None:
             raise BotUtilsError(
-                f"对象不可被重复标记。在命名空间 {namespace} 中名为 {flag_name} 的标记已存在"
+                f"标记失败。对象的命名空间 {namespace} 中已存在名为 {flag_name} 的标记"
             )
+
         self._flags_store[namespace][flag_name] = val
 
     def flag_check(self, namespace: str, flag_name: str, val: Any = None) -> bool:
         """检查此对象是否携带有指定的标记"""
-        self._flags_store = self._flags_store
-        if self._flags_store is None:
-            return False
         if (flags := self._flags_store.get(namespace)) is None:
             return False
         if (flag := flags.get(flag_name, Void)) is Void:
             return False
+
         return flag is val if val is None else flag == val
 
 
 class Cloneable:
     def copy(self):
         """返回一个本对象的一个深拷贝对象"""
         return deepcopy(self)
@@ -164,15 +128,15 @@
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
     def __init__(self, rawEvent: dict) -> None:
         super().__init__()
-        #: 从 onebot 实现项目获得的未格式化的事件原始值
+        #: 从 onebot 实现获得的事件原始值
         self.raw: dict = rawEvent
 
     def __format__(self, format_spec: str) -> str:
         match format_spec:
             case "hexid":
                 return f"{id(self):#x}"
             case "raw":
@@ -206,16 +170,14 @@
 
     def is_meta_event(self) -> bool:
         """判断是否是元事件"""
         return self.type == "meta"
 
 
 class ActionArgs(ABC):
-    # 行为信息构造基类
-
     def __init__(self) -> None:
         super().__init__()
         self.type: str
         self.params: dict
 
 
 class BotAction(Flagable, Cloneable):
@@ -247,24 +209,26 @@
 
         self._ready = ready
 
     def __format__(self, format_spec: str) -> str:
         match format_spec:
             case "hexid":
                 return f"{id(self):#x}"
+
             case "raw":
                 trigger = (
                     f"{self.trigger.__class__.__name__}[{self.trigger:hexid}]"
                     if self.trigger is not None
                     else None
                 )
                 return (
                     f"BotAction(type={self.type}, trigger={trigger}, "
                     f"resp_id={self.resp_id}, params={self.params})"
                 )
+
             case _:
                 raise BotValueError(f"未知的 action 格式标识符：{format_spec}")
 
     def extract(self) -> dict:
         # 从对象提取标准 cq action dict
         obj = {
             "action": self.type,
@@ -285,15 +249,15 @@
             return
         raise BotRuntimeError("action 已记录触发它的 event，拒绝再次记录")
 
 
 class SessionRule(ABC):
     """会话规则基类
 
-    会话规则用于两事件是否在同一会话的判断。
+    会话规则用于判断两事件是否在同一会话中。
     """
 
     def __init__(self) -> None:
         super().__init__()
 
     @abstractmethod
     def compare(self, e1: BotEvent, e2: BotEvent) -> bool:
@@ -304,89 +268,56 @@
         :param e1: 判断时的事件1
         :param e2: 判断时的事件2
         :return: 判断结果
         """
         raise NotImplementedError
 
 
+@dataclass
 class EventHandlerArgs:
     """事件方法（事件执行器）构造参数"""
 
-    def __init__(
-        self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
-        type: Type["EventHandler"],
-        params: list[Any],
-    ) -> None:
-        self.executor = executor
-        if not is_retcoro(executor):
-            raise BotValueError(
-                f"事件处理函数 {executor.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        self.type = type
-        self.params = params
+    executor: AsyncCallable[..., None]
+    type: Type["EventHandler"]
+    params: list[Any]
 
 
+@dataclass
 class ShareObjArgs:
     """插件共享对象构造参数"""
 
-    def __init__(
-        self, namespace: str, id: str, reflector: Callable[[], Coroutine[Any, Any, Any]]
-    ) -> None:
-        if not is_retcoro(reflector):
-            raise BotValueError(
-                f"共享对象值获取函数 {reflector.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        self.reflector = reflector
-        self.namespace = namespace
-        self.id = id
+    reflector: AsyncCallable[..., Any]
+    namespace: str
+    id: str
 
 
+@dataclass
 class ShareObjCbArgs:
     """插件共享对象回调的构造参数"""
 
-    def __init__(
-        self, namespace: str, id: str, cb: Callable[..., Coroutine[Any, Any, Any]]
-    ) -> None:
-        if not is_retcoro(cb):
-            raise BotValueError(
-                f"共享对象的回调 {cb.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        self.namespace = namespace
-        self.id = id
-        self.cb = cb
+    namespace: str
+    id: str
+    cb: AsyncCallable[..., Any]
 
 
+@dataclass
 class PluginSignalHandlerArgs:
     """插件信号方法构造参数"""
 
-    def __init__(
-        self, func: Callable[..., Coroutine[Any, Any, Any]], namespace: str, signal: str
-    ) -> None:
-        if not is_retcoro(func):
-            raise BotValueError(
-                f"插件信号处理函数 {func.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        self.func = func
-        self.namespace = namespace
-        self.signal = signal
+    func: AsyncCallable[..., Any]
+    namespace: str
+    signal: str
 
 
+@dataclass
 class BotHookRunnerArgs:
     """钩子方法（生命周期回调）构造参数"""
 
-    def __init__(
-        self, func: Callable[..., Coroutine[Any, Any, None]], type: BotLife
-    ) -> None:
-        if not is_retcoro(func):
-            raise BotValueError(
-                f"bot 生命周期 hook {func.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        self.func = func
-        self.type = type
+    func: AsyncCallable[..., None]
+    type: BotLife
 
 
 class BotChecker(ABC, Cloneable):
     """检查器基类"""
 
     def __init__(self) -> None:
         """初始化一个检查器基类对象"""
```

### Comparing `melobot-2.6.2/src/melobot/base/exceptions.py` & `melobot-2.6.3/src/melobot/base/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+import logging
 import sys
 
 import better_exceptions
 
+better_exceptions.SUPPORTS_COLOR = True
+better_exceptions.color.SUPPORTS_COLOR = True
+better_exceptions.formatter.SUPPORTS_COLOR = True
 # 修复在 windows powershell 显示错误的 bug
 better_exceptions.encoding.ENCODING = sys.stdout.encoding
 better_exceptions.formatter.ENCODING = sys.stdout.encoding
-better_exceptions.hook()
+# 直接 hook，而不是让它使用环境变量触发
+sys.excepthook = better_exceptions.excepthook
+# 取消它的猴子补丁
+logging._loggerClass = logging.Logger  # type:ignore[attr-defined]
 
 
 class BotException(Exception):
     """Bot 异常基类
 
     在使用 melobot 编写代码时，若需要抛出异常，可以有意抛出该类。
     表明这是你设计的异常情况，而不是完全预期之外的异常。
@@ -19,14 +26,19 @@
         super().__init__(self, msg)
         self.err = msg
 
     def __str__(self):
         return self.err
 
 
+class BotValidateError(BotException):
+    def __init__(self, msg: str):
+        super().__init__(msg)
+
+
 class BotValueError(BotException):
     def __init__(self, msg: str):
         super().__init__(msg)
 
 
 class BotRuntimeError(BotException):
     def __init__(self, msg: str):
@@ -56,15 +68,10 @@
 class BotSessionTimeout(BotException):
     """会话暂停的超时异常"""
 
     def __init__(self, msg: str = ""):
         super().__init__(msg)
 
 
-class BotToolsError(BotException):
-    def __init__(self, msg: str):
-        super().__init__(msg)
-
-
 class FuncSafeExited(BotException):
     def __init__(self, msg: str = ""):
         super().__init__(msg)
```

### Comparing `melobot-2.6.2/src/melobot/base/tools.py` & `melobot-2.6.3/src/melobot/base/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import asyncio
 import inspect
 import os
 import pathlib
 import time
-from asyncio import iscoroutine
+import uuid
 from contextlib import asynccontextmanager
 from functools import wraps
 
-from .exceptions import BotRuntimeError, BotToolsError
-from .typing import T1, T2, T3, Any, Callable, Coroutine, Optional, P, T, cast
+from .exceptions import BotRuntimeError, BotValidateError
+from .typing import (
+    T1,
+    T2,
+    T3,
+    Any,
+    AsyncCallable,
+    Callable,
+    Coroutine,
+    Optional,
+    P,
+    T,
+    async_guard,
+    cast,
+)
 
 
 class Singleton:
     def __new__(cls, *args: Any, **kwargs: Any):
         if not hasattr(cls, "__instance__"):
             cls.__instance__ = super(Singleton, cls).__new__(cls)
         return cls.__instance__
@@ -71,117 +84,60 @@
 
     def __init__(self, read_limit: Optional[int] = None) -> None:
         """初始化一个异步读写控制器
 
         :param read_limit: 读取的数量限制，为空则不限制
         """
         write_semaphore = asyncio.Semaphore(1)
-        if read_limit:
-            read_semaphore = asyncio.Semaphore(read_limit)
-        else:
-            read_semaphore = None
+        read_semaphore = asyncio.Semaphore(read_limit) if read_limit else None
         read_num = 0
         read_num_lock = asyncio.Lock()
 
         @asynccontextmanager
         async def safe_read():
             nonlocal read_num, read_semaphore, write_semaphore, read_num_lock
+
             if read_semaphore:
                 await read_semaphore.acquire()
+
             async with read_num_lock:
                 if read_num == 0:
                     await write_semaphore.acquire()
                 read_num += 1
+
             try:
                 yield
             finally:
                 async with read_num_lock:
                     read_num -= 1
                     if read_num == 0:
                         write_semaphore.release()
                     if read_semaphore:
                         read_semaphore.release()
 
         @asynccontextmanager
         async def safe_write():
             nonlocal write_semaphore
+
             await write_semaphore.acquire()
             try:
                 yield
             finally:
                 write_semaphore.release()
 
         self.safe_read = safe_read
         self.safe_write = safe_write
 
 
-class IdWorker:
-    """雪花算法生成 ID"""
-
-    def __init__(self, datacenter_id, worker_id, sequence=0) -> None:
-        self.MAX_WORKER_ID = -1 ^ (-1 << 3)
-        self.MAX_DATACENTER_ID = -1 ^ (-1 << 5)
-        self.WOKER_ID_SHIFT = 12
-        self.DATACENTER_ID_SHIFT = 12 + 3
-        self.TIMESTAMP_LEFT_SHIFT = 12 + 3 + 5
-        self.SEQUENCE_MASK = -1 ^ (-1 << 12)
-        self.STARTEPOCH = 1064980800000
-        # sanity check
-        if worker_id > self.MAX_WORKER_ID or worker_id < 0:
-            raise ValueError("worker_id 值越界")
-        if datacenter_id > self.MAX_DATACENTER_ID or datacenter_id < 0:
-            raise ValueError("datacenter_id 值越界")
-        self.worker_id = worker_id
-        self.datacenter_id = datacenter_id
-        self.sequence = sequence
-        self.last_timestamp = -1
-
-    def __gen_timestamp(self) -> int:
-        """生成整数时间戳"""
-        return int(time.time_ns() / 1e6)
-
-    def get_id(self) -> int:
-        """获取新 ID"""
-        timestamp = self.__gen_timestamp()
-
-        # 时钟回拨
-        if timestamp < self.last_timestamp:
-            raise ValueError(f"时钟回拨，{self.last_timestamp} 前拒绝 id 生成请求")
-        if timestamp == self.last_timestamp:
-            self.sequence = (self.sequence + 1) & self.SEQUENCE_MASK
-            if self.sequence == 0:
-                timestamp = self.__til_next_millis(self.last_timestamp)
-        else:
-            self.sequence = 0
-        self.last_timestamp = timestamp
-        new_id = (
-            ((timestamp - self.STARTEPOCH) << self.TIMESTAMP_LEFT_SHIFT)
-            | (self.datacenter_id << self.DATACENTER_ID_SHIFT)
-            | (self.worker_id << self.WOKER_ID_SHIFT)
-            | self.sequence
-        )
-        return new_id
-
-    def __til_next_millis(self, last_timestamp) -> int:
-        """等到下一毫秒"""
-        timestamp = self.__gen_timestamp()
-        while timestamp <= last_timestamp:
-            timestamp = self.__gen_timestamp()
-        return timestamp
-
-
-_ID_WORKER = IdWorker(1, 1, 0)
-
-
 def get_id() -> str:
     """从 melobot 内部 id 获取器获得一个 id 值，不保证线程安全。
 
     :return: id 值
     """
-    return str(_ID_WORKER.get_id())
+    return uuid.uuid4().hex
 
 
 def this_dir(*relative_path: str) -> str:
     """包内 py 脚本通过该方法可获得所在目录的绝对路径。提供参数，还可拼接路径。
 
     使用方法：
 
@@ -229,25 +185,29 @@
     cur_idx: int
     caller_path: str | None = None
     stacks = inspect.stack()
 
     for idx, finfo in enumerate(stacks):
         if finfo.function == "this_dir" and os.path.samefile(finfo.filename, __file__):
             cur_finfo, cur_idx = finfo, idx
+
     if cur_finfo is None:
         raise BotRuntimeError("this_dir 定位失败，请检查本函数使用方式是否正确")
 
     for idx, finfo in enumerate(stacks[cur_idx + 1 :]):
+
         if finfo.function == "<module>":
             for val in finfo.frame.f_locals.values():
                 if val is __dir_inspector__:
                     caller_path = finfo.filename
                     break
+
             if caller_path is not None:
                 break
+
     if caller_path is None:
         raise BotRuntimeError("this_dir 定位失败，请检查本函数使用方式是否正确")
 
     return str(
         pathlib.Path(caller_path).parent.joinpath(*relative_path).resolve(strict=True)
     )
 
@@ -266,15 +226,15 @@
 
     async def wrapper():
         return func()
 
     if callable(func):
         return wrapper
     else:
-        raise BotToolsError("to_async 函数只支持同步函数作为参数")
+        raise BotValidateError("to_async 函数只支持同步函数作为参数")
 
 
 def to_coro(obj: Callable[[], T] | asyncio.Future[T]) -> Coroutine[Any, Any, T]:
     """协程包装函数
 
     将一个同步函数或 Future 对象包装为协程，保留返回值。如果需要传参使用 partial 包裹。
 
@@ -286,75 +246,49 @@
         return await obj
 
     if isinstance(obj, asyncio.Future):
         return as_coro(obj)
     elif callable(obj):
         return to_async(obj)()
     else:
-        raise BotToolsError("to_coro 函数只支持同步函数或 Future 对象作为参数")
-
-
-def to_task(obj: Coroutine[Any, Any, T] | asyncio.Future[T]) -> asyncio.Task[T]:
-    """任务包装器
-
-    将一个协程或 Future 对象包装为任务，保留返回值。
-
-    :param obj: 协程或 Future 对象
-    :return: 任务
-    """
-    if iscoroutine(obj):
-        return asyncio.create_task(obj)
-    elif isinstance(obj, asyncio.Future):
-        return asyncio.create_task(to_coro(obj))
-    else:
-        raise BotToolsError("to_task 函数只支持协程或 Future 对象作为参数")
+        raise BotValidateError("to_coro 函数只支持同步函数或 Future 对象作为参数")
 
 
-def lock(callback: Optional[Callable[[], Coroutine[Any, Any, T1]]] = None):
+def lock(callback: Optional[AsyncCallable[[], T1]] = None):
     """锁装饰器
 
     本方法作为异步函数的装饰器使用，可以为被装饰函数加锁。
 
     在获取锁冲突时，调用 `callback` 获得一个回调并执行。回调执行完毕后直接返回。
 
     `callback` 参数为空，只应用 :class:`asyncio.Lock` 的锁功能。
 
     被装饰函数的返回值：被装饰函数被执行 -> 被装饰函数返回值；执行任何回调 -> 那个回调的返回值
 
     :param callback: 获取锁冲突时的回调
     """
     alock = asyncio.Lock()
-    if callback is not None and not callable(callback):
-        raise BotToolsError(
-            f"lock 装饰器的 callback 参数不可调用，callback 值为：{callback}"
-        )
-
-    def deco_func(
-        func: Callable[P, Coroutine[Any, Any, T2]]
-    ) -> Callable[P, Coroutine[Any, Any, T1 | T2]]:
+
+    def deco_func(func: AsyncCallable[P, T2]) -> AsyncCallable[P, T1 | T2]:
+
         @wraps(func)
         async def wrapped_func(*args: Any, **kwargs: Any) -> T1 | T2:
             if callback is not None and alock.locked():
-                cb = callback()
-                if not iscoroutine(cb):
-                    raise BotToolsError(
-                        f"lock 装饰器的 callback 返回的不是协程，返回的回调为：{cb}"
-                    )
-                return await cb
+                return await async_guard(callback)
             async with alock:
-                return await func(*args, **kwargs)
+                return await async_guard(func, *args, **kwargs)
 
         return wrapped_func
 
     return deco_func
 
 
 def cooldown(
-    busy_callback: Optional[Callable[[], Coroutine[Any, Any, T1]]] = None,
-    cd_callback: Optional[Callable[[float], Coroutine[Any, Any, T2]]] = None,
+    busy_callback: Optional[AsyncCallable[[], T1]] = None,
+    cd_callback: Optional[AsyncCallable[[float], T2]] = None,
     interval: float = 5,
 ):
     """冷却装饰器
 
     本方法作为异步函数的装饰器使用，可以为被装饰函数添加 cd 时间。
 
     如果被装饰函数已有一个在运行，此时调用 `busy_callback` 生成回调并执行。回调执行完毕后直接返回。
@@ -370,150 +304,107 @@
 
     :param busy_callback: 已运行时的回调
     :param cd_callback: 冷却时间未结束的回调
     :param interval: 冷却时间
     """
     alock = asyncio.Lock()
     pre_finish_t = time.perf_counter() - interval - 1
-    if busy_callback is not None and not callable(busy_callback):
-        raise BotToolsError(
-            f"cooldown 装饰器的 busy_callback 参数不可调用，busy_callback 值为：{busy_callback}"
-        )
-    if cd_callback is not None and not callable(cd_callback):
-        raise BotToolsError(
-            f"cooldown 装饰器的 cd_callback 参数不可调用，cd_callback 值为：{cd_callback}"
-        )
-
-    def deco_func(
-        func: Callable[P, Coroutine[Any, Any, T3]]
-    ) -> Callable[P, Coroutine[Any, Any, T1 | T2 | T3]]:
+
+    def deco_func(func: AsyncCallable[P, T3]) -> AsyncCallable[P, T1 | T2 | T3]:
+
         @wraps(func)
         async def wrapped_func(*args: Any, **kwargs: Any) -> T1 | T2 | T3:
             nonlocal pre_finish_t
             if busy_callback is not None and alock.locked():
-                busy_cb = busy_callback()
-                if not iscoroutine(busy_cb):
-                    raise BotToolsError(
-                        f"cooldown 装饰器的 busy_callback 返回的不是协程，返回的回调为：{busy_cb}"
-                    )
-                return await busy_cb
+                return await async_guard(busy_callback)
 
             async with alock:
                 duration = time.perf_counter() - pre_finish_t
                 if duration > interval:
-                    ret = await func(*args, **kwargs)
+                    ret = await async_guard(func, *args, **kwargs)
                     pre_finish_t = time.perf_counter()
                     return ret
 
                 remain_t = interval - duration
                 if cd_callback is not None:
-                    cd_cb = cd_callback(remain_t)
-                    if not iscoroutine(cd_cb):
-                        raise BotToolsError(
-                            f"cooldown 装饰器的 cd_callback 返回的不是协程，返回的回调为：{cd_cb}"
-                        )
-                    return await cd_cb
+                    return await async_guard(cd_callback, remain_t)
                 else:
                     await asyncio.sleep(remain_t)
-                    ret = await func(*args, **kwargs)
+                    ret = await async_guard(func, *args, **kwargs)
                     pre_finish_t = time.perf_counter()
                     return ret
 
         return wrapped_func
 
     return deco_func
 
 
-def semaphore(
-    callback: Optional[Callable[[], Coroutine[Any, Any, T1]]] = None, value: int = -1
-):
+def semaphore(callback: Optional[AsyncCallable[[], T1]] = None, value: int = -1):
     """信号量装饰器
 
     本方法作为异步函数的装饰器使用，可以为被装饰函数添加信号量控制。
 
     在信号量无法立刻获取时，将调用 `callback` 获得回调并执行。回调执行完毕后直接返回。
 
     `callback` 参数为空，只应用 :class:`asyncio.Semaphore` 的信号量功能。
 
     被装饰函数的返回值：被装饰函数被执行 -> 被装饰函数返回值；执行任何回调 -> 那个回调的返回值
 
     :param callback: 信号量无法立即获取的回调
     :param value: 信号量阈值
     """
     a_semaphore = asyncio.Semaphore(value)
-    if callback is not None and not callable(callback):
-        raise BotToolsError(
-            f"semaphore 装饰器的 callback 参数不可调用，callback 值为：{callback}"
-        )
-
-    def deco_func(
-        func: Callable[P, Coroutine[Any, Any, T2]]
-    ) -> Callable[P, Coroutine[Any, Any, T1 | T2]]:
+
+    def deco_func(func: AsyncCallable[P, T2]) -> AsyncCallable[P, T1 | T2]:
+
         @wraps(func)
         async def wrapped_func(*args: Any, **kwargs: Any) -> T1 | T2:
             if callback is not None and a_semaphore.locked():
-                cb = callback()
-                if not iscoroutine(cb):
-                    raise BotToolsError(
-                        f"semaphore 装饰器的 callback 返回的不是协程，返回的回调为：{cb}"
-                    )
-                return await cb
+                return await async_guard(callback)
             async with a_semaphore:
-                return await func(*args, **kwargs)
+                return await async_guard(func, *args, **kwargs)
 
         return wrapped_func
 
     return deco_func
 
 
-def timelimit(
-    callback: Optional[Callable[[], Coroutine[Any, Any, T1]]] = None, timeout: float = 5
-):
+def timelimit(callback: Optional[AsyncCallable[[], T1]] = None, timeout: float = 5):
     """时间限制装饰器
 
     本方法作为异步函数的装饰器使用，可以为被装饰函数添加超时控制。
 
     超时之后，调用 `callback` 获得回调并执行，同时取消原任务。
 
     `callback` 参数为空，如果超时，则抛出 :class:`asyncio.TimeoutError` 异常。
 
     被装饰函数的返回值：被装饰函数被执行 -> 被装饰函数返回值；执行任何回调 -> 那个回调的返回值
 
     :param callback: 超时时的回调
     :param timeout: 超时时间
     """
-    if callback is not None and not callable(callback):
-        raise BotToolsError(
-            f"timelimit 装饰器的 callback 参数不可调用，callback 值为：{callback}"
-        )
-
-    def deco_func(
-        func: Callable[P, Coroutine[Any, Any, T2]]
-    ) -> Callable[P, Coroutine[Any, Any, T1 | T2]]:
+
+    def deco_func(func: AsyncCallable[P, T2]) -> AsyncCallable[P, T1 | T2]:
+
         @wraps(func)
         async def wrapped_func(*args: Any, **kwargs: Any) -> T1 | T2:
             try:
-                return await asyncio.wait_for(func(*args, **kwargs), timeout)
+                return await asyncio.wait_for(async_guard(func, *args, **kwargs), timeout)
             except asyncio.TimeoutError:
                 if callback is None:
-                    raise
-                cb = callback()
-                if not iscoroutine(cb):
-                    raise BotToolsError(
-                        f"timelimit 装饰器的 callback 返回的不是协程，返回的回调为：{cb}"
-                    )
-                return await cb
+                    raise TimeoutError("timelimit 所装饰的任务已超时")
+                return await async_guard(callback)
 
         return wrapped_func
 
     return deco_func
 
 
 def speedlimit(
-    callback: Optional[Callable[[], Coroutine[Any, Any, T1]]] = None,
+    callback: Optional[AsyncCallable[[], T1]] = None,
     limit: int = 60,
     duration: int = 60,
 ):
     """流量/速率限制装饰器
 
     本方法作为异步函数的装饰器使用，可以为被装饰函数添加流量控制：`duration` 秒内只允许 `limit` 次调用。
 
@@ -526,61 +417,59 @@
     :param callback: 超出速率限制时的回调
     :param limit: `duration` 秒内允许调用多少次
     :param duration: 时长区间
     """
     called_num = 0
     min_start = time.perf_counter()
     if limit <= 0:
-        raise BotToolsError("speedlimit 装饰器的 limit 参数必须 > 0")
+        raise BotValidateError("speedlimit 装饰器的 limit 参数必须 > 0")
     if duration <= 0:
-        raise BotToolsError("speedlimit 装饰器的 duration 参数必须 > 0")
-    if callback is not None and not callable(callback):
-        raise BotToolsError(
-            f"speedlimit 装饰器的 callback 参数不可调用，callback 值为：{callback}"
-        )
-
-    def deco_func(
-        func: Callable[P, Coroutine[Any, Any, T2]]
-    ) -> Callable[P, Coroutine[Any, Any, T1 | T2]]:
+        raise BotValidateError("speedlimit 装饰器的 duration 参数必须 > 0")
+
+    def deco_func(func: AsyncCallable[P, T2]) -> AsyncCallable[P, T1 | T2]:
+
         @wraps(func)
         async def wrapped_func(*args: Any, **kwargs: Any) -> T1 | T2:
             res_fut = _wrapped_func(func, *args, **kwargs)
             fut_ret = await res_fut
             if isinstance(fut_ret, Exception):
                 raise fut_ret
             return fut_ret
 
         return wrapped_func
 
     def _wrapped_func(
-        func: Callable[P, Coroutine[Any, Any, T2]], *args: Any, **kwargs: Any
+        func: AsyncCallable[P, T2], *args: Any, **kwargs: Any
     ) -> asyncio.Future[T1 | T2 | Exception]:
         # 分离出来定义，方便 result_set 调用形成递归。主要逻辑通过 Future 实现，有利于避免竞争问题。
         nonlocal called_num, min_start
         passed_time = time.perf_counter() - min_start
         res_fut: Any = asyncio.Future()
 
         if passed_time <= duration:
             if called_num < limit:
                 called_num += 1
                 asyncio.create_task(result_set(func, res_fut, -1, *args, **kwargs))
+
             elif callback is not None:
                 asyncio.create_task(result_set(callback, res_fut, -1))
+
             else:
                 asyncio.create_task(
                     result_set(func, res_fut, duration - passed_time, *args, **kwargs)
                 )
         else:
             called_num, min_start = 0, time.perf_counter()
             called_num += 1
             asyncio.create_task(result_set(func, res_fut, -1, *args, **kwargs))
+
         return res_fut
 
     async def result_set(
-        func: Callable[P, Coroutine[Any, Any, T]],
+        func: AsyncCallable[P, T],
         fut: asyncio.Future[T | Exception],
         delay: float,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         nonlocal called_num
         try:
@@ -590,16 +479,18 @@
             """
             if delay > 0:
                 await asyncio.sleep(delay)
                 res = await _wrapped_func(func, *args, **kwargs)
                 res = cast(T | Exception, res)
                 fut.set_result(res)
                 return
-            res = await func(*args, **kwargs)
+
+            res = await async_guard(func, *args, **kwargs)
             fut.set_result(res)
+
         except Exception as e:
             fut.set_result(e)
 
     return deco_func
 
 
 def call_later(callback: Callable[[], None], delay: float):
@@ -619,23 +510,22 @@
 
     在指定的时间戳调度一个 `callback` 执行。`callback` 应该是同步方法。`timestamp` <= 当前时刻回调立即执行
 
     :param callback: 同步函数
     :param timestamp: 在什么时刻调度
     :return: :class:`asyncio.TimerHandle` 对象
     """
+    loop = asyncio.get_running_loop()
     if timestamp <= time.time_ns() / 1e9:
-        return asyncio.get_running_loop().call_soon(callback)
+        return loop.call_soon(callback)
     else:
-        return asyncio.get_running_loop().call_later(
-            timestamp - time.time_ns() / 1e9, callback
-        )
+        return loop.call_later(timestamp - time.time_ns() / 1e9, callback)
 
 
-def async_later(callback: Coroutine[Any, Any, T], delay: float) -> asyncio.Future[T]:
+def async_later(callback: Coroutine[Any, Any, Any], delay: float) -> asyncio.Future[T]:
     """异步函数延迟调度（可自主选择是否等待）
 
     在指定的 `delay` 后调度一个 `callback` 执行。`callback` 是协程。
 
     返回一个 :class:`asyncio.Future` 对象，你可以选择等待或不等待。等待 :class:`asyncio.Future` 即是等待 `callback` 的返回值。
 
     注意：如果 `callback` 未完成就被取消，需要捕获 :class:`asyncio.CancelledError`。
@@ -654,15 +544,15 @@
             callback.close()
 
     fut: asyncio.Future[Any] = asyncio.Future()
     asyncio.create_task(async_cb(fut))
     return fut
 
 
-def async_at(callback: Coroutine[Any, Any, T], timestamp: float) -> asyncio.Future[T]:
+def async_at(callback: Coroutine[Any, Any, Any], timestamp: float) -> asyncio.Future[T]:
     """异步函数指定时间调度（可自主选择是否等待）
 
     在指定的时间戳调度一个 `callback` 执行。`callback` 是协程。
 
     返回一个 :class:`asyncio.Future` 对象，你可以选择等待或不等待。等待 :class:`asyncio.Future` 即是等待 `callback` 的返回值。
 
     注意：如果 `callback` 未完成就被取消，需要捕获 :class:`asyncio.CancelledError`。
@@ -698,41 +588,7 @@
                 await asyncio.sleep(interval)
                 await coro
         except asyncio.CancelledError:
             coro.close()
 
     t = asyncio.create_task(interval_cb())
     return t
-
-
-def is_retcoro(obj: Any, safe_mode: bool = False) -> bool:
-    """判断是否是可以返回协程的可调用对象
-
-    如果启用安全模式，传入的 `obj` 参数是 Future、Coroutine、Task，将会被自动取消。
-
-    :param obj: 对象
-    :param safe_mode: 是否启用安全模式。默认不启用。
-    :return: 判断结果
-    """
-    if safe_mode:
-        if inspect.iscoroutine(obj):
-            obj.close()
-            return False
-        elif isinstance(obj, asyncio.Task) or isinstance(obj, asyncio.Future):
-            obj.cancel()
-            return False
-
-    if not callable(obj):
-        return False
-    elif inspect.iscoroutinefunction(obj):
-        return True
-
-    try:
-        is_coro = False
-        res = obj()
-        is_coro = inspect.iscoroutine(res)
-    except Exception:
-        pass
-    finally:
-        if is_coro:
-            res.close()
-        return is_coro
```

### Comparing `melobot-2.6.2/src/melobot/base/typing.py` & `melobot-2.6.3/src/melobot/base/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+import inspect
 from enum import Enum
-from types import ModuleType
+from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
+    Awaitable,
     Callable,
     Coroutine,
+    Generic,
     Iterator,
     Literal,
     Optional,
     ParamSpec,
     Type,
     TypeAlias,
     TypedDict,
     TypeVar,
     Union,
     cast,
 )
 
 from typing_extensions import NotRequired
 
+from .exceptions import BotValidateError
+
 
 class MsgSegment(TypedDict):
     """onebot 标准的消息段对象"""
 
     type: str
     data: dict[str, float | int | str]
 
@@ -161,7 +166,26 @@
     """
 
     pass
 
 
 #: “无值”对象类型
 VoidType: TypeAlias = Type[Void]
+
+
+#: 参数为 P，返回 Awaitable[T] 的可调用对象
+AsyncCallable: TypeAlias = Callable[P, Awaitable[T]]
+
+
+async def async_guard(func: AsyncCallable[..., T], *args: Any, **kwargs: Any) -> T:
+    """在使用异步可调用对象时，提供用户友好的验证"""
+    if not callable(func):
+        raise BotValidateError(
+            f"{func} 不是异步可调用对象（返回 Awaitable 的可调用对象）"
+        )
+
+    await_obj = func(*args, **kwargs)
+    if inspect.isawaitable(await_obj):
+        return await await_obj
+    raise BotValidateError(
+        f"{func} 不是异步可调用对象（返回 Awaitable 的可调用对象），因为它的返回结果 {await_obj} 不可异步等待"
+    )
```

### Comparing `melobot-2.6.2/src/melobot/bot/hook.py` & `melobot-2.6.3/src/melobot/bot/hook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 import asyncio
 
-from ..base.abc import BaseLogger, BotLife
+from ..base.abc import BotLife
 from ..base.exceptions import BotValueError
-from ..base.typing import Any, Callable, Coroutine
-from ..utils.logger import log_exc
+from ..base.typing import TYPE_CHECKING, Any, AsyncCallable
+
+if TYPE_CHECKING:
+    from ..utils.logger import BotLogger
 
 
 class HookRunner:
     """bot hook 运行器"""
 
-    def __init__(
-        self, type: BotLife, func: Callable[..., Coroutine[Any, Any, None]]
-    ) -> None:
-        self.cb: Callable[..., Coroutine[Any, Any, None]] = func
+    def __init__(self, type: BotLife, func: AsyncCallable[..., None]) -> None:
+        self.cb: AsyncCallable[..., None] = func
         self.type: BotLife = type
 
 
 class BotHookBus:
     """bot hook 总线"""
 
     def __init__(self) -> None:
         self.store: dict[BotLife, list[HookRunner]] = {
-            v: [] for k, v in BotLife.__members__.items()
+            v: [] for v in BotLife.__members__.values()
         }
-        self.logger: BaseLogger
+        self.logger: "BotLogger"
 
-    def _bind(self, logger: BaseLogger) -> None:
+    def _bind(self, logger: "BotLogger") -> None:
         self.logger = logger
 
-    def register(
-        self, hook_type: BotLife, hook_func: Callable[..., Coroutine[Any, Any, None]]
-    ) -> None:
+    def register(self, hook_type: BotLife, hook_func: AsyncCallable[..., None]) -> None:
         if hook_type not in self.store.keys():
             raise BotValueError(
                 f"尝试添加一个 bot 生命周期 hook 方法，但是其指定的类型 {hook_type} 不存在"
             )
+
         runner = HookRunner(hook_type, hook_func)
         self.store[hook_type].append(runner)
 
     async def _run_on_ctx(self, runner: HookRunner, *args: Any, **kwargs: Any) -> None:
         try:
             await runner.cb(*args, **kwargs)
         except Exception as e:
             func_name = runner.cb.__qualname__
             self.logger.error(f"bot 生命周期 hook 方法 {func_name} 发生异常")
-            log_exc(self.logger, locals(), e)
+            self.logger.exc(locals=locals())
 
     async def emit(
         self, hook_type: BotLife, *args: Any, wait: bool = False, **kwargs: Any
     ) -> None:
-        if not wait:
-            for runner in self.store[hook_type]:
-                asyncio.create_task(self._run_on_ctx(runner, *args, **kwargs))
-        else:
-            tasks = []
-            for runner in self.store[hook_type]:
-                tasks.append(
-                    asyncio.create_task(self._run_on_ctx(runner, *args, **kwargs))
-                )
-            if len(tasks):
-                await asyncio.wait(tasks)
+        tasks = []
+        for runner in self.store[hook_type]:
+            task = asyncio.create_task(self._run_on_ctx(runner, *args, **kwargs))
+            tasks.append(task)
+
+        if wait and len(tasks):
+            await asyncio.wait(tasks)
```

### Comparing `melobot-2.6.2/src/melobot/bot/init.py` & `melobot-2.6.3/src/melobot/bot/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import asyncio
 import os
 from contextvars import ContextVar, Token
 
-from ..base.abc import AbstractConnector, BaseLogger
+from ..base.abc import AbstractConnector
 from ..base.exceptions import BotRuntimeError, BotValueError
 from ..base.typing import (
     TYPE_CHECKING,
     Any,
     BotLife,
     Coroutine,
     Literal,
     Optional,
     Void,
+    cast,
 )
 from ..context.session import SESSION_LOCAL, BotSessionManager
 from ..controller.dispatcher import BotDispatcher
 from ..controller.responder import BotResponder
 from ..meta import MetaInfo
 from ..models.event import BotEventBuilder
-from ..plugin.handler import EVENT_HANDLER_MAP
+from ..plugin.handler import EVENT_CHANNELS
 from ..plugin.init import BotPlugin, PluginLoader, PluginProxy
 from ..plugin.ipc import PluginBus, PluginStore
-from ..utils.logger import BotLogger, NullLogger, log_exc
+from ..utils.logger import BotLogger, NullLogger
 from .hook import BotHookBus
 
 if TYPE_CHECKING:
     from ..plugin.ipc import ShareObject
 
 if MetaInfo.OS_NAME != "nt":
     import uvloop
@@ -60,15 +61,15 @@
         MeloBot.BOTS[name] = self
 
         #: bot 的名字（唯一）
         self.name: str = name
         #: 元信息
         self.info: type[MetaInfo] = MetaInfo
         #: bot 的日志器
-        self.logger: BaseLogger
+        self.logger: BotLogger
         #: bot 的连接器
         self.connector: AbstractConnector
 
         self._plugins: dict[str, BotPlugin] = {}
         self._loader = PluginLoader
         self._ctx_manager = BotSessionManager
         self._event_builder = BotEventBuilder
@@ -87,15 +88,15 @@
         connector: AbstractConnector,
         enable_log: bool = True,
         logger_name: Optional[str] = None,
         log_level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO",
         log_to_console: bool = True,
         log_to_dir: Optional[str] = None,
         log_tag: bool = False,
-        custom_logger: Optional[BaseLogger] = None,
+        custom_logger: Optional[Any] = None,
     ) -> "MeloBot":
         """初始化 bot 实例
 
         :param connector: 使 bot 实例工作的连接器
         :param enable_log: 是否启用日志
         :param logger_name: 日志器名称, 为空则使用 bot 实例名字
         :param log_level: 日志器日志等级
@@ -108,68 +109,68 @@
         if connector._used:
             raise BotRuntimeError("bot 初始化时，不可使用已被其他 bot 实例使用的连接器")
         connector._used = True
         self.connector = connector
 
         if custom_logger is not None:
             self.logger = custom_logger
+
         elif not enable_log:
-            self.logger = NullLogger(f"__MELOBOT_NULL_{self.name}__")
+            self.logger = cast(BotLogger, NullLogger(f"__MELOBOT_NULL_{self.name}__"))
+
         else:
+            logger_name = self.name if logger_name is None else logger_name
             self.logger = BotLogger(
-                self.name if logger_name is None else logger_name,
-                log_level,
-                log_to_console,
-                log_to_dir,
-                not log_tag,
+                logger_name, log_level, log_to_console, log_to_dir, not log_tag
             )
         self.logger.debug(f"连接器已初始化，类型：{connector.__class__.__name__}")
 
         self._dispatcher._bind(
-            EVENT_HANDLER_MAP, self._bot_bus, self._ctx_manager, self.logger
+            EVENT_CHANNELS, self._bot_bus, self._ctx_manager, self.logger
         )
         self._plugin_bus._bind(self.logger)
         self._bot_bus._bind(self.logger)
         self._responder._bind(self.logger, self.connector)
         self.connector._bind(
             self._dispatcher,
             self._responder,
             self._event_builder,
             self._bot_bus,
             self.logger,
         )
+
         self.logger.debug("bot 初始化完成，各核心组件已初始化")
         self.__init_flag__ = True
         return self
 
-    def load_plugin(self, plugin_target: str | BotPlugin) -> "MeloBot":
+    def load_plugin(self, target: str | BotPlugin) -> "MeloBot":
         """为 bot 实例加载插件
 
-        :param plugin_target: 插件目标，可传入插件对象或插件包（一个插件即是一个 python package）的路径
+        :param target: 插件目标，可传入插件对象或插件包（一个插件即是一个 python package）的路径
         :return: bot 实例（因此支持链式调用）
         """
         if not self.__init_flag__:
             raise BotRuntimeError("bot 尚未初始化，不能加载插件")
 
-        plugin_dir = None if not isinstance(plugin_target, str) else plugin_target
-        if plugin_dir is None:
-            self.logger.debug(f"尝试加载插件 {plugin_target}")
+        dir = None if not isinstance(target, str) else target
+        if dir is None:
+            self.logger.debug(f"尝试加载插件 {target}")
         else:
-            self.logger.debug(f"尝试加载来自 {plugin_dir} 的插件")
-        plugin = self._loader.load(plugin_target)
+            self.logger.debug(f"尝试加载来自 {dir} 的插件")
+
+        plugin = self._loader.load(target)
         exist_plugin = self._plugins.get(plugin.ID)
         if exist_plugin is not None:
             self.logger.error(
                 f"加载插件出错：插件 id 重复, 重复的 id 为：{plugin.ID}，已取消该插件加载"
             )
             return self
+
         if not plugin.MULTI_USE and plugin._loaded_once:
-            raise BotRuntimeError(
-                f"插件 {plugin.ID} 不支持多 bot，但它已被其他 bot 加载"
-            )
+            raise BotRuntimeError(f"插件 {plugin.ID} 不支持多 bot，但它已被其他 bot 加载")
         plugin._loaded_once = True
 
         handlers = []
         for _ in plugin.__handler_args__:
             handler = _.type(_.executor, plugin, self.logger, *_.params)
             self._ctx_manager.register(handler)
             handlers.append(handler)
@@ -180,64 +181,72 @@
         for _ in plugin.__signal_args__:
             self._plugin_bus.register(_.namespace, _.signal, _.func)
         for _ in plugin.__hook_args__:
             self._bot_bus.register(_.type, _.func)
 
         self._plugins[plugin.ID] = plugin
         self._dispatcher.add_handlers(handlers)
+
         self.logger.info(f"成功加载插件：{plugin.ID}")
         return self
 
     def load_plugins(self, plugins_dir: str) -> "MeloBot":
         """为 bot 实例批量加载插件
 
         :param plugins_dir: 传入包含所有插件包（一个插件即是一个 python package）的目录
         :return: bot 实例（因此支持链式调用）
         """
         if not self.__init_flag__:
             raise BotRuntimeError("bot 尚未初始化，不能加载插件")
 
         self.logger.debug(f"尝试从目录 {plugins_dir} 批量加载插件")
         items = os.listdir(plugins_dir)
+
         for item in items:
             path = os.path.join(plugins_dir, item)
             if os.path.isdir(path) and os.path.basename(path) != "__pycache__":
                 self.load_plugin(path)
+
         return self
 
     async def _run(self) -> None:
         if not self.__init_flag__:
             raise BotRuntimeError("bot 尚未初始化，不能启动")
         if self.__run_flag__:
             raise BotRuntimeError("bot 已在运行，无需再次启动")
         if len(self._plugins) == 0:
             self.logger.warning("没有加载任何插件，bot 将不会有任何操作")
 
         self.logger.info(f"运行版本：{self.info.VER} | 平台：{self.info.PLATFORM}")
         bot_token = BOT_LOCAL._add_ctx(self)
         await self._bot_bus.emit(BotLife.LOADED)
         self.logger.debug("LOADED hook 已完成")
+
         try:
             async with self.connector:
                 self._dispatcher._set_ready()
                 self._responder._set_ready()
                 self.connector._set_ready()
+
                 self.__run_flag__ = True
                 self.logger.info("bot 开始正常运行")
-                self.logger.debug(
-                    f"使用的连接器类型：{self.connector.__class__.__name__}"
-                )
+                conn_name = self.connector.__class__.__name__
+                self.logger.debug(f"使用的连接器类型：{conn_name}")
+
                 await self._life_ended.wait()
+
         except Exception as e:
-            self.logger.error(f"bot 核心无法继续运行。异常：{e}")
-            log_exc(self.logger, locals(), e)
+            self.logger.error("bot 核心无法继续运行")
+            self.logger.exc(locals=locals())
+
         finally:
             await self._bot_bus.emit(BotLife.BEFORE_STOP, wait=True)
             self.logger.debug("BEFORE_STOP hook 已完成")
             self.logger.info("bot 已清理运行时资源")
+
             BOT_LOCAL._del_ctx(bot_token)
             self.__run_flag__ = False
 
     def run(self) -> None:
         """运行 bot 实例"""
         _safe_blocked_run(self._run())
 
@@ -311,33 +320,33 @@
         :param args: 传递给信号处理方法的 args
         :param kwargs: 传递给信号处理方法的 kwargs
         :return: 不等待信号处理方法处理，只返回 :obj:`None`；若等待则返回运行结果
         """
         if not self.__init_flag__:
             raise BotRuntimeError("bot 尚未初始化，不能执行此方法")
 
-        if self.logger.check_level_flag("DEBUG"):
+        if self.logger._check_level("DEBUG"):
             self.logger.debug(
                 f"bot 信号触发：{namespace}.{signal} | wait: {wait}"
-                f"（当前 session 上下文：{SESSION_LOCAL:hexid}），传递参数：args={args}, kwargs={kwargs}"
+                f"（当前会话上下文：{SESSION_LOCAL:hexid}），传递参数：args={args}, kwargs={kwargs}"
             )
         return self._plugin_bus.emit(namespace, signal, *args, wait=wait, **kwargs)
 
     def get_share(self, namespace: str, id: str) -> "ShareObject":
         """获得 bot 实例内的共享对象
 
         :param namespace: 共享对象的命名空间
         :param id: 共享对象的标识 id
         :return: 获得到的共享对象
         """
         if not self.__init_flag__:
             raise BotRuntimeError("bot 尚未初始化，不能执行此方法")
 
         self.logger.debug(
-            f"获取共享对象行为：{namespace}.{id}（当前 session 上下文：{SESSION_LOCAL:hexid}）"
+            f"获取共享对象行为：{namespace}.{id}（当前会话上下文：{SESSION_LOCAL:hexid}）"
         )
         return self._plugin_store.get(namespace, id)
 
     @classmethod
     def start(cls, *bots: "MeloBot") -> None:
         """同时运行多个 bot 实例
 
@@ -376,23 +385,25 @@
         """
         bot = cls.BOTS.get(target)
         if bot is None:
             raise BotValueError(f"单播指定的 bot 实例 {target} 不存在")
 
         b_token = BOT_LOCAL._add_ctx(bot)
         s_token = SESSION_LOCAL._add_ctx(Void)
+
         try:
             await bot.emit_signal(namespace, signal, *args, **kwargs, wait=wait)
+
         except AttributeError as e:
-            if "Void" in e.__str__():
-                raise BotRuntimeError(
-                    "多播或单播时，bot 和 session 的上下文传递将会被阻隔。如需使用，请将它们作为参数显式传递"
-                )
-            else:
+            if "Void" not in e.__str__():
                 raise e
+            raise BotRuntimeError(
+                "多播或单播时，bot 和会话的上下文传递将会被阻隔。如需使用，请将它们作为参数显式传递"
+            )
+
         finally:
             BOT_LOCAL._del_ctx(b_token)
             SESSION_LOCAL._del_ctx(s_token)
 
     @classmethod
     async def multicast(
         cls,
@@ -412,25 +423,24 @@
         :param self_exclude: 是否在多播时排除自己
         :param wait: 是否等待信号处理方法处理完毕
         :param args: 传递给信号处理方法的 args
         :param kwargs: 传递给信号处理方法的 kwargs
         """
         if isinstance(targets, list):
             _targets = targets
-        else:
-            _targets = list(cls.BOTS.keys())
-            if self_exclude:
-                _targets.remove(BOT_LOCAL.name)
+
+        _targets = list(cls.BOTS.keys())
+        if self_exclude:
+            _targets.remove(BOT_LOCAL.name)
+
         tasks = []
         for name in _targets:
-            tasks.append(
-                asyncio.create_task(
-                    cls.unicast(name, namespace, signal, *args, **kwargs, wait=wait)
-                )
-            )
+            task = cls.unicast(name, namespace, signal, *args, **kwargs, wait=wait)
+            tasks.append(asyncio.create_task(task))
+
         if len(tasks):
             await asyncio.wait(tasks)
 
     @classmethod
     def use_default_loop_policy(cls) -> None:
         """使用默认的事件循环策略
 
@@ -440,18 +450,16 @@
         """
         asyncio.set_event_loop_policy(None)
 
 
 class BotLocal:
     """bot 实例自动上下文"""
 
-    __slots__ = tuple(
-        list(filter(lambda x: not (len(x) >= 2 and x[:2] == "__"), dir(MeloBot)))
-        + ["__storage__"]
-    )
+    _ = lambda x: not x.startswith("__")
+    __slots__ = tuple(filter(_, dir(MeloBot))) + ("__storage__",)
 
     def __init__(self) -> None:
         object.__setattr__(self, "__storage__", ContextVar("melobot_ctx"))
         self.__storage__: ContextVar["MeloBot"]
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         setattr(self.__storage__.get(), __name, __value)
```

### Comparing `melobot-2.6.2/src/melobot/context/__init__.py` & `melobot-2.6.3/src/melobot/context/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/src/melobot/context/action.py` & `melobot-2.6.3/src/melobot/context/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..base.abc import ActionArgs, BotAction, BotEvent
 from ..base.exceptions import BotSessionError, BotValueError, FuncSafeExited
 from ..base.tools import get_id
-from ..base.typing import Any, Literal, MsgNode, MsgSegment, Optional, cast
-from ..models.msg import _to_cq_str_action, reply_msg, text_msg
+from ..base.typing import Literal, MsgNode, MsgSegment, Optional
+from ..models.msg import reply_msg, to_cq_str_action, to_msg_segment
 from .session import SESSION_LOCAL
 from .session import BotSessionManager as SessionManager
 
 __all__ = (
     "send_custom",
     "send",
     "send_custom_forward",
@@ -68,43 +68,14 @@
             self.params = {
                 "message_type": "group",
                 "group_id": groupId,
                 "message": msgs,
             }
 
 
-def _process_msg(content: str | MsgSegment | list[MsgSegment]) -> list[MsgSegment]:
-    """将多种可能的消息格式，统一转换为 cq 消息列表"""
-
-    def verify_segment(obj: Any) -> bool:
-        return (
-            isinstance(obj, dict)
-            and obj.get("type") is not None
-            and isinstance(obj.get("data"), dict)
-        )
-
-    if isinstance(content, str):
-        return [text_msg(content)]
-
-    elif verify_segment(content):
-        return [cast(MsgSegment, content)]
-
-    elif (
-        isinstance(content, list)
-        and len(content) > 0
-        and all(verify_segment(obj) for obj in content)
-    ):
-        return content
-
-    else:
-        raise BotValueError(
-            f"发送的消息内容有误，当前值是：{content}，但需要以下格式之一：字符串、消息段对象、消息段对象的列表（不可为空）"
-        )
-
-
 @SessionManager._handle
 def send_custom(
     content: str | MsgSegment | list[MsgSegment],
     isPrivate: bool,
     userId: Optional[int] = None,
     groupId: Optional[int] = None,
     cq_str: bool = False,
@@ -148,23 +119,26 @@
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param wait: 是否等待这个行为完成
     :param auto: 是否自动发送
     :return: :class:`.ActionHandle` 对象
     """
     if isPrivate and userId is None:
         raise BotValueError("为私聊时，构建发送消息 action 必须提供 userId 参数")
+
     if not isPrivate and groupId is None:
         raise BotValueError("为群聊时，构建发送消息 action 必须提供 groupId 参数")
+
     action = BotAction(
-        MsgActionArgs(_process_msg(content), isPrivate, userId, groupId),
+        MsgActionArgs(to_msg_segment(content), isPrivate, userId, groupId),
         resp_id=get_id() if wait else None,
         ready=auto,
     )
+
     if cq_str:
-        action = _to_cq_str_action(action)
+        action = to_cq_str_action(action)
     return action
 
 
 @SessionManager._handle
 def send(
     content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
@@ -205,27 +179,29 @@
     :param auto: 是否自动发送
     :return: :class:`.ActionHandle` 对象
     """
     try:
         session = SESSION_LOCAL
         action = BotAction(
             MsgActionArgs(
-                _process_msg(content),
+                to_msg_segment(content),
                 session.event.is_private(),
                 session.event.sender.id,
                 session.event.group_id,
             ),
             resp_id=get_id() if wait else None,
             ready=auto,
         )
+
         if cq_str:
-            action = _to_cq_str_action(action)
+            action = to_cq_str_action(action)
         return action
+
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
 
 
 class ForwardMsgActionArgs(ActionArgs):
     """转发消息 action 信息构造类"""
 
     def __init__(
         self,
@@ -298,15 +274,15 @@
     """
     action = BotAction(
         ForwardMsgActionArgs(msgNodes, isPrivate, userId, groupId),
         resp_id=get_id() if wait else None,
         ready=auto,
     )
     if cq_str:
-        action = _to_cq_str_action(action)
+        action = to_cq_str_action(action)
     return action
 
 
 @SessionManager._handle
 def send_forward(
     msgNodes: list[MsgNode],
     cq_str: bool = False,
@@ -361,19 +337,21 @@
                 session.event.is_private(),
                 session.event.sender.id,
                 session.event.group_id,
             ),
             resp_id=get_id() if wait else None,
             ready=auto,
         )
+
         if cq_str:
-            action = _to_cq_str_action(action)
+            action = to_cq_str_action(action)
         return action
+
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
 
 
 class MsgDelActionArgs(ActionArgs):
     """撤回消息 action 信息构造类"""
 
     def __init__(self, msgId: int) -> None:
         super().__init__()
@@ -1264,17 +1242,15 @@
         self.type = "get_group_honor_info"
         self.params = {"group_id": groupId, "type": type}
 
 
 @SessionManager._handle
 def get_group_honor(
     groupId: int,
-    type: Literal[
-        "talkative", "performer", "legend", "strong_newbie", "emotion", "all"
-    ],
+    type: Literal["talkative", "performer", "legend", "strong_newbie", "emotion", "all"],
     wait: bool = True,
     auto: bool = True,
 ) -> BotAction:
     """获取群荣誉信息
 
     详细说明参考：
     `获取群荣誉信息 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#get_group_honor_info-获取群荣誉信息>`_
@@ -1488,15 +1464,15 @@
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param overtime: 会话暂停的超时时间，超时将抛出 :class:`.BotSessionTimeout` 异常
     """
     await send(content, cq_str)
     try:
         await SessionManager._hup(SESSION_LOCAL._get_var(), overtime)
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
 
 
 async def send_reply(
     content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
     auto: bool = True,
 ) -> None:
@@ -1520,16 +1496,17 @@
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param auto: 是否自动发送
     """
     try:
         content_arr = [reply_msg(SESSION_LOCAL.event.id)]
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
-    content_arr.extend(_process_msg(content))
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
+
+    content_arr.extend(to_msg_segment(content))
     await send(content_arr, cq_str, wait=False, auto=auto)
 
 
 async def finish(
     content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
 ) -> None:
@@ -1555,15 +1532,16 @@
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     """
     await send(content, cq_str)
     try:
         SessionManager._expire(SESSION_LOCAL._get_var())
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
+
     raise FuncSafeExited("改函数或方法被安全地直接结束，请无视这个异常")
 
 
 async def reply_finish(
     content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
 ) -> None:
@@ -1588,16 +1566,18 @@
 
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     """
     try:
         content_arr = [reply_msg(SESSION_LOCAL.event.id)]
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
 
-    content_arr.extend(_process_msg(content))
+    content_arr.extend(to_msg_segment(content))
     await send(content_arr, cq_str)
+
     try:
         SessionManager._expire(SESSION_LOCAL._get_var())
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
+
     raise FuncSafeExited("改函数或方法被安全地直接结束，请无视这个异常")
```

### Comparing `melobot-2.6.2/src/melobot/context/session.py` & `melobot-2.6.3/src/melobot/context/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from ..base.abc import SessionRule
 from ..base.exceptions import (
     BotRuntimeError,
     BotSessionError,
     BotSessionTimeout,
     BotValueError,
 )
+from ..base.ioc import PendingDepend
 from ..base.tools import get_twin_event
 from ..base.typing import (
     TYPE_CHECKING,
     Any,
+    AsyncCallable,
     Callable,
-    Coroutine,
     Literal,
     Optional,
     P,
     Type,
     Union,
     Void,
     VoidType,
@@ -31,83 +32,79 @@
     from ..base.abc import BotAction, BotEvent, ParseArgs
     from ..bot.init import BotLocal, MeloBot
     from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
     from ..plugin.handler import EventHandler
 
 
 class BotSession:
-    """Bot Session 类。不需要直接实例化，必须通过 BotSessionBuilder 构造。"""
+    """Bot会话类。不需要直接实例化，必须通过 BotSessionBuilder 构造。"""
 
     def __init__(
         self,
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         manager: Type["BotSessionManager"],
         space_tag: Optional["EventHandler"] = None,
     ) -> None:
         super().__init__()
         self.store: dict[str, Any] = {}
-        # 永远指向当前上下文的 event
         self.event = event
         self.args: Union["ParseArgs", None] = None
 
         self._manager = manager
-        # session 是否空闲的标志，由 BotSessionManager 修改和管理
+        # 会话是否空闲的标志，由 BotSessionManager 修改和管理
         self._free_signal = asyncio.Event()
         self._free_signal.set()
-        # session 是否挂起的标志。二者互为孪生反状态。由 BotSessionManager 修改和管理
-        # 注意 session 挂起时一定是非空闲和非过期的
+        # 会话是否挂起的标志。二者互为孪生反状态。由 BotSessionManager 修改和管理
+        # 注意会话挂起时一定是非空闲和非过期的
         self._hup_signal, self._awake_signal = get_twin_event()
-        # session 是否过期的标志，由 BotSessionManager 修改和管理
+        # 会话是否过期的标志，由 BotSessionManager 修改和管理
         self._expired = False
-        # 用于标记该 session 属于哪个 session 空间，如果为 None 则表明是一次性 session
+        # 用于标记该会话属于哪个会话空间，如果为 None 则表明是一次性 会话
         self._space_tag: Optional["EventHandler"] = space_tag
 
     def __format__(self, format_spec: str) -> str:
         match format_spec:
             case "hexid":
                 return f"{id(self):#x}"
             case _:
-                raise BotSessionError(f"未知的 session 格式化标识符：{format_spec}")
+                raise BotSessionError(f"未知的会话格式化标识符：{format_spec}")
 
     def __lshift__(self, another: "BotSession") -> None:
-        """合并 session 的存储内容"""
+        """合并会话的存储内容"""
         self.store.update(another.store)
         self.args = another.args
 
 
 class SessionLocal:
-    """Session 自动上下文"""
+    """会话 自动上下文"""
 
-    __slots__ = tuple(
-        list(filter(lambda x: not (len(x) >= 2 and x[:2] == "__"), dir(BotSession)))
-        + ["__storage__"]
-    )
+    _ = lambda x: not x.startswith("__")
+    __slots__ = tuple(filter(_, dir(BotSession))) + ("__storage__",)
 
     def __init__(self) -> None:
         object.__setattr__(self, "__storage__", ContextVar("session_ctx"))
         self.__storage__: ContextVar[BotSession | VoidType]
 
     def __format__(self, format_spec: str) -> str:
         match format_spec:
             case "hexid":
                 try:
                     return f"{self._get_var():hexid}"
                 except LookupError:
                     return "None"
+
             case _:
-                raise BotSessionError(
-                    f"未知的 SessionLocal 格式化标识符：{format_spec}"
-                )
+                raise BotSessionError(f"未知的 SessionLocal 格式化标识符：{format_spec}")
 
     def _get_var(self) -> BotSession:
         var = self.__storage__.get()
         if var is Void:
             raise LookupError("上下文当前为 Void，识别为跨 bot 通信")
-        var = cast(BotSession, var)
-        return var
+
+        return cast(BotSession, var)
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         setattr(self._get_var(), __name, __value)
 
     def __getattr__(self, __name: str) -> Any:
         return getattr(self._get_var(), __name)
 
@@ -150,39 +147,39 @@
 
     def _get_val(self, e: "BotEvent", attrs: tuple[str, ...]) -> Any:
         val = e
         try:
             for attr in attrs:
                 val = getattr(val, attr)
         except AttributeError:
-            raise BotSessionError(f"session 规则指定的属性 {attr} 不存在")
+            raise BotSessionError(f"会话规则指定的属性 {attr} 不存在")
         return val
 
     def compare(self, e1: "BotEvent", e2: "BotEvent") -> bool:
         return self._get_val(e1, self.attrs) == self._get_val(e2, self.attrs)
 
 
 class BotSessionManager:
     STORAGE: dict["EventHandler", set[BotSession]] = {}
     HUP_STORAGE: dict["EventHandler", set[BotSession]] = {}
     # 各个 handler 对饮的操作锁
     WORK_LOCKS: dict["EventHandler", asyncio.Lock] = {}
-    # 用来标记 cls.get 等待一个挂起的 session 时的死锁
+    # 用来标记 cls.get 等待一个挂起的会话时的死锁
     DEADLOCK_FLAGS: dict["EventHandler", asyncio.Event] = {}
     # 对应每个 handler 的 try_attach 过程的操作锁
     ATTACH_LOCKS: dict["EventHandler", asyncio.Lock] = {}
     BOT_CTX: "MeloBot"
 
     @classmethod
     def _bind(cls, bot_local_var: "BotLocal") -> None:
         cls.BOT_CTX = bot_local_var  # type: ignore[assignment]
 
     @classmethod
     def register(cls, handler: "EventHandler") -> None:
-        """以 handler 为键，注册 handler 对应的 session 空间、操作锁和挂起 session 空间"""
+        """以 handler 为键，注册 handler 对应的会话空间、操作锁和挂起会话空间"""
         cls.STORAGE[handler] = set()
         cls.WORK_LOCKS[handler] = asyncio.Lock()
         cls.HUP_STORAGE[handler] = set()
         cls.DEADLOCK_FLAGS[handler] = asyncio.Event()
         cls.ATTACH_LOCKS[handler] = asyncio.Lock()
 
     @classmethod
@@ -191,248 +188,253 @@
 
     @classmethod
     def _attach(
         cls,
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         handler: "EventHandler",
     ) -> bool:
-        """Session 附着操作，临界区操作。只能在 cls.try_attach 中进行"""
+        """会话 附着操作，临界区操作。只能在 cls.try_attach 中进行"""
         session = None
+
         for s in cls.HUP_STORAGE[handler]:
-            # session 的挂起方法，保证 session 一定未过期，因此不进行过期检查
+            # 会话的挂起方法，保证会话一定未过期，因此不进行过期检查
             handler._rule = cast(AttrSessionRule, handler._rule)
             if handler._rule.compare(s.event, event):
                 session = s
                 break
-        # 如果获得一个挂起的 session，它一定是可附着的，附着后需要唤醒
+
+        # 如果获得一个挂起的 会话，它一定是可附着的，附着后需要唤醒
         if session:
             session.event = event
             cls._rouse(session)
             return True
         return False
 
     @classmethod
     async def try_attach(
         cls,
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         handler: "EventHandler",
     ) -> bool:
-        """检查是否有挂起的 session 可供 event 附着。 如果有则附着并唤醒，并返回 True。否则返回 False。"""
+        """检查是否有挂起的会话可供 event 附着。 如果有则附着并唤醒，并返回 True。否则返回 False。"""
         if handler._rule is None:
             return False
 
         async with cls.ATTACH_LOCKS[handler]:
             t1 = asyncio.create_task(cls.DEADLOCK_FLAGS[handler].wait(), name="flag")
             t2 = asyncio.create_task(cls.WORK_LOCKS[handler].acquire(), name="lock")
             done, _ = await asyncio.wait([t1, t2], return_when=asyncio.FIRST_COMPLETED)
+
             # 等待完成后，一定要记得取消另一个任务！否则可能异常加锁
             if done.pop().get_name() == "flag":
                 res = cls._attach(event, handler)
                 cls.DEADLOCK_FLAGS[handler].clear()
                 t2.cancel()
                 return res
+
             else:
                 res = cls._attach(event, handler)
                 cls.WORK_LOCKS[handler].release()
                 t1.cancel()
                 return res
 
     @classmethod
     async def _hup(cls, session: BotSession, overtime: Optional[float] = None) -> None:
-        """挂起 session"""
+        """挂起 会话"""
         if session._space_tag is None:
-            raise BotSessionError(
-                "当前 session 上下文因为缺乏 session_rule 作为唤醒标志，无法挂起"
-            )
+            raise BotSessionError("当前会话上下文因为缺乏会话规则作为唤醒标志，无法挂起")
         elif session._expired:
-            raise BotSessionError("过期的 session 不能被挂起")
+            raise BotSessionError("过期的会话不能被挂起")
+
         cls.fill_args(session, None)
         cls.STORAGE[session._space_tag].remove(session)
         cls.HUP_STORAGE[session._space_tag].add(session)
         session._awake_signal.clear()
 
         if overtime is None:
             await session._awake_signal.wait()
         elif overtime <= 0:
-            raise BotSessionError("session 挂起超时时间（秒数）必须 > 0")
+            raise BotSessionError("会话 挂起超时时间（秒数）必须 > 0")
+
         else:
-            await asyncio.wait(
-                [
-                    asyncio.create_task(session._awake_signal.wait()),
-                    asyncio.create_task(asyncio.sleep(overtime)),
-                ],
-                return_when=asyncio.FIRST_COMPLETED,
-            )
+            _awake = asyncio.create_task(session._awake_signal.wait())
+            _timeout = asyncio.create_task(asyncio.sleep(overtime))
+            await asyncio.wait([_awake, _timeout], return_when=asyncio.FIRST_COMPLETED)
+
             if not session._awake_signal.is_set():
                 cls._rouse(session)
-                raise BotSessionTimeout("session 挂起超时")
+                raise BotSessionTimeout("会话 挂起超时")
 
     @classmethod
     def _rouse(cls, session: BotSession) -> None:
-        """唤醒 session"""
+        """唤醒 会话"""
         if session._space_tag is None:
             raise BotSessionError(
-                "当前 session 上下文因为缺乏 session_rule 作为唤醒标志，无法唤醒"
+                "当前会话上下文因为缺乏 session_rule 作为唤醒标志，无法唤醒"
             )
+
         cls.HUP_STORAGE[session._space_tag].remove(session)
         cls.STORAGE[session._space_tag].add(session)
         session._awake_signal.set()
 
     @classmethod
     def _expire(cls, session: BotSession) -> None:
-        """标记该 session 为过期状态，并进行销毁操作（如果存在于某个 session_space，则从中移除）"""
+        """标记该会话为过期状态，并进行销毁操作（如果存在于某个 session_space，则从中移除）"""
         if session._expired:
             return
+
         session.store.clear()
         session._expired = True
         if session._space_tag:
             cls.STORAGE[session._space_tag].remove(session)
 
     @classmethod
     def recycle(cls, session: BotSession, alive: bool = False) -> None:
-        """Session 所在方法运行结束后，回收 session。 默认将 session 销毁。若 alive 为 True，则保留"""
+        """会话 所在方法运行结束后，回收 会话。 默认将会话销毁。若 alive 为 True，则保留"""
         session._free_signal.set()
         if not alive:
             cls._expire(session)
 
     @classmethod
     async def get(
         cls,
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         handler: "EventHandler",
     ) -> Optional[BotSession]:
-        """Handler 内获取 session 方法。自动根据 handler._rule 判断是否需要映射到 session_space 进行存储。
-        然后根据具体情况，获取已有 session 或新建 session。当尝试获取非空闲 session 时，如果 handler 指定不等待则返回
+        """Handler 内获取会话方法。自动根据 handler._rule 判断是否需要映射到 session_space 进行存储。
+        然后根据具体情况，获取已有会话或新建 会话。当尝试获取非空闲会话时，如果 handler 指定不等待则返回
         None."""
         if handler._rule:
             # session_space, session._free_signal 竞争，需要加锁
             async with cls.WORK_LOCKS[handler]:
                 session = await cls._get_on_rule(event, handler)
                 # 必须在锁的保护下修改 session._free_signal
                 if session:
                     session._free_signal.clear()
+
         else:
             session = cls._make(event, handler)
             session._free_signal.clear()
 
         return session
 
     @classmethod
     def _make(
         cls,
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         handler: Optional["EventHandler"] = None,
     ) -> BotSession:
-        """内部使用的创建 session 方法。如果 handler 为空，即缺乏 space_tag，则为一次性 session。 或 handler._rule
-        为空，则也为一次性 session."""
-        if handler:
-            if handler._rule:
-                session = BotSession(event, cls, handler)
-                cls.STORAGE[handler].add(session)
-                return session
+        """内部使用的创建会话方法。如果 handler 为空，即缺乏 space_tag，则为一次性 会话。 或 handler._rule
+        为空，则也为一次性 会话."""
+        if handler and handler._rule:
+            session = BotSession(event, cls, handler)
+            cls.STORAGE[handler].add(session)
+            return session
+
         session = BotSession(event, cls)
         return session
 
     @classmethod
     def make_temp(
         cls, event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"]
     ) -> BotSession:
-        """创建一次性 session。确定无需 session 管理机制时可以使用。 否则一定使用 cls.get 方法"""
+        """创建临时 会话。确定无需会话管理机制时可以使用。 否则一定使用 cls.get 方法"""
         return cls._make(event)
 
     @classmethod
     async def _get_on_rule(
         cls,
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         handler: "EventHandler",
     ) -> Optional[BotSession]:
-        """根据 handler 具体情况，从对应 session_space 中获取 session 或新建 session，或返回 None"""
+        """根据 handler 具体情况，从对应 session_space 中获取会话或新建 会话，或返回 None"""
         session = None
         check_rule, session_space, conflict_wait = (
             handler._rule,
             cls.STORAGE[handler],
             handler._wait_flag,
         )
 
         # for 循环都需要即时 break，保证遍历 session_space 时没有协程切换。因为切换后 session_space 可能发生变动
         for s in session_space:
             check_rule = cast(AttrSessionRule, check_rule)
             if check_rule.compare(s.event, event) and not s._expired:
                 session = s
                 break
-        # 如果会话不存在，生成一个新 session 变量
+
+        # 如果会话不存在，生成一个新会话变量
         if session is None:
             return cls._make(event, handler)
-        # 如果会话存在，且未过期，且空闲，则附着到这个 session 上
+
+        # 如果会话存在，且未过期，且空闲，则附着到这个会话上
         if session._free_signal.is_set():
             session.event = event
             return session
+
         # 如果会话存在，且未过期，但是不空闲，选择不等待
         if not conflict_wait:
             return None
+
         # 如果会话存在，且未过期，但是不空闲，选择等待，此时就不得不陷入等待（即将发生协程切换）
-        await asyncio.wait(
-            [
-                asyncio.create_task(session._free_signal.wait()),
-                asyncio.create_task(session._hup_signal.wait()),
-            ],
-            return_when=asyncio.FIRST_COMPLETED,
-        )
+        _free = asyncio.create_task(session._free_signal.wait())
+        _hup = asyncio.create_task(session._hup_signal.wait())
+        await asyncio.wait([_free, _hup], return_when=asyncio.FIRST_COMPLETED)
+
         if session._hup_signal.is_set():
             cls.DEADLOCK_FLAGS[handler].set()
             await session._free_signal.wait()
+
         """
-        重新切换回本协程后，session 有可能变为过期，但此时一定是空闲的。
+        重新切换回本协程后，会话 有可能变为过期，但此时一定是空闲的。
         同时一定是非挂起状态。因为上面解决了可能存在的挂起死锁问题。
-        即使该 session 因过期被所在的 session_space 清除也无妨，因为此处有引用，
-        该 session 并不会消失。且此处不操作 session_space，无需担心 session_space 变动
+        即使该会话因过期被所在的 session_space 清除也无妨，因为此处有引用，
+        该会话并不会消失。且此处不操作 session_space，无需担心 session_space 变动
         """
-        # 如果过期，生成一个新的 session 变量
+        # 如果过期，生成一个新的会话变量
         if session._expired:
             return cls._make(event, handler)
-        # 如果未过期，则附着到这个 session 上
+        # 如果未过期，则附着到这个会话上
         else:
             session.event = event
             return session
 
     @classmethod
     def _handle(
         cls, action_getter: Callable[P, "BotAction"]
     ) -> Callable[P, "ActionHandle"]:
 
         @wraps(action_getter)
         def wrapped_func(*args: Any, **kwargs: Any) -> ActionHandle:
             try:
                 if SESSION_LOCAL._expired:
                     raise BotSessionError(
-                        "当前  session 上下文已有过期标记，无法再执行 action 操作"
+                        "当前会话上下文已有过期标记，无法再执行 action 操作"
                     )
             except LookupError:
                 pass
 
             action: "BotAction" = action_getter(*args, **kwargs)
-            if cls.BOT_CTX.logger.check_level_flag("DEBUG"):
+
+            if cls.BOT_CTX.logger._check_level("DEBUG"):
                 cls.BOT_CTX.logger.debug(
-                    f"action {action:hexid} 构建完成（当前 session 上下文：{SESSION_LOCAL:hexid}）"
+                    f"action {action:hexid} 构建完成（当前会话上下文：{SESSION_LOCAL:hexid}）"
                 )
+
             try:
                 action._fill_trigger(SESSION_LOCAL.event)
             except LookupError:
                 pass
 
-            handle = ActionHandle(
-                action,
-                (
-                    cls.BOT_CTX._responder.take_action
-                    if action.resp_id is None
-                    else cls.BOT_CTX._responder.take_action_wait
-                ),
-                action.resp_id is not None,
-            )
+            exec_meth: AsyncCallable[["BotAction"], asyncio.Future[ActionResponse] | None]
+            if action.resp_id is None:
+                exec_meth = cls.BOT_CTX._responder.take_action
+            else:
+                exec_meth = cls.BOT_CTX._responder.take_action_wait
 
+            handle = ActionHandle(action, exec_meth, action.resp_id is not None)
             if not action._ready:
                 return handle
             else:
                 handle.execute()
                 return handle
 
         return wrapped_func
@@ -453,22 +455,17 @@
         #: 响应的状态码
         self.status: int
         #: 响应的数据
         self.data: dict[str, Any]
         #: 响应创建的时间
         self.time: int = int(time.time())
 
-        rawEvent = self.raw
-        self.status = rawEvent["retcode"]
-        if "echo" in rawEvent.keys():
-            self.id = rawEvent["echo"]
-        if "data" in rawEvent.keys():
-            self.data = rawEvent["data"]
-        else:
-            self.data = {}
+        self.status = self.raw["retcode"]
+        self.id = self.raw.get("echo")
+        self.data = self.raw.get("data", {})
 
     def __format__(self, format_spec: str) -> str:
         match format_spec:
             case "hexid":
                 return f"{id(self):#x}"
             case "raw":
                 return self.raw.__str__()
@@ -498,17 +495,15 @@
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
     def __init__(
         self,
         action: "BotAction",
-        exec_meth: Callable[
-            ["BotAction"], Coroutine[Any, Any, asyncio.Future[ActionResponse] | None]
-        ],
+        exec_meth: AsyncCallable[["BotAction"], asyncio.Future[ActionResponse] | None],
         wait: bool,
     ) -> None:
         #: 本操作包含的行为对象
         self.action: "BotAction" = action
         #: 本操作当前状态。分别对应：未执行、执行中、执行完成
         self.status: Literal["PENDING", "EXECUTING", "FINISHED"] = "PENDING"
 
@@ -518,14 +513,15 @@
         self._resp_done = asyncio.Event()
 
     @property
     async def resp(self) -> ActionResponse:
         """当前行为操作的响应数据，需要异步获取（行为操作函数 `wait` 参数为 :obj:`True` 时使用）"""
         if not self._wait:
             raise BotRuntimeError("行为操作未指定等待，无法获取响应")
+
         await self._resp_done.wait()
         return self._resp
 
     def __await__(self):
         yield
 
     async def wait(self) -> None:
@@ -533,39 +529,42 @@
         if not self._wait:
             raise BotRuntimeError("行为操作未指定等待，无法等待")
         await self._resp_done.wait()
 
     async def _execute(self) -> None:
         ret = await self._exec_meth(self.action)
         if self._wait:
-            self._resp = await cast(asyncio.Future[ActionResponse], ret)
+            ret = cast(asyncio.Future[ActionResponse], ret)
+            self._resp = await ret
             self._resp_done.set()
+
         self.status = "FINISHED"
 
     def execute(self) -> "ActionHandle":
         """手动触发行为操作的执行（行为操作函数 `auto` 参数为 :obj:`False` 时使用）
 
         :return: 本实例对象（因此支持链式调用）
         """
         if self.status != "PENDING":
             raise BotRuntimeError("行为操作正在执行或执行完毕，不应该再执行")
+
         self.status = "EXECUTING"
         asyncio.create_task(self._execute())
         return self
 
 
 def any_event() -> Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"]:
     """获取当前会话下的事件
 
     :return: 具体的事件
     """
     try:
         return SESSION_LOCAL.event
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        return PendingDepend(lambda: SESSION_LOCAL.event)  # type: ignore[return-value]
 
 
 def msg_event() -> "MessageEvent":
     """获取当前会话下的事件
 
     确定此事件是消息事件时使用，例如在消息事件的处理函数中，使用该方法即可获得精准的类型提示
 
@@ -608,44 +607,51 @@
     """获取当前会话下的，消息事件的纯文本内容的合并字符串。
     等价于手动读取消息事件的 :attr:`~.MessageEvent.text` 属性
 
     只能在确定当前会话下必为消息事件时使用
 
     :return: 纯文本内容的合并字符串
     """
-    return msg_event().text
+    try:
+        return SESSION_LOCAL.event.text
+    except LookupError:
+        return PendingDepend(lambda: SESSION_LOCAL.event.text)  # type: ignore[return-value]
 
 
 def msg_args() -> list[Any] | None:
     """获取当前会话下的消息事件的所有解析参数值。
 
     只能在确定当前会话下必为消息事件时使用
 
     :return: 解析参数值列表或 :obj:`None`
     """
-    try:
+
+    def _getter() -> list[Any] | None:
         if SESSION_LOCAL.args is not None:
             return SESSION_LOCAL.args.vals
         else:
             return None
+
+    try:
+        return _getter()
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        return PendingDepend(_getter)  # type: ignore[return-value]
 
 
 def session_store() -> dict:
     """返回当前会话的存储字典对象，可直接操作
 
     会话存储字典对象用于在会话层面保存和共享数据。
 
     :return: 会话的存储字典对象
     """
     try:
         return SESSION_LOCAL.store
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        return PendingDepend(lambda: SESSION_LOCAL.store)  # type: ignore[return-value]
 
 
 async def pause(overtime: Optional[float] = None) -> None:
     """会话暂停直到被同一会话的事件唤醒
 
     暂时停止本会话。当本会话的会话规则判断有属于本会话的另一事件发生，
     本会话将自动被唤醒。
@@ -655,15 +661,15 @@
     实现自定义的超时处理逻辑
 
     :param overtime: 超时时间
     """
     try:
         await BotSessionManager._hup(SESSION_LOCAL._get_var(), overtime)
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
 
 
 def dispose() -> None:
     """销毁当前会话
 
     将会清理会话的存储空间，并将会话标记为过期态。
     此时调用该方法的函数依然可以运行，但是此会话状态下无法再进行行为操作。
@@ -671,8 +677,8 @@
     一般来说，会话将会自动销毁。
     只有在绑定事件处理函数时使用 `session_hold=True`，才会需要使用此函数。
 
     """
     try:
         BotSessionManager._expire(SESSION_LOCAL._get_var())
     except LookupError:
-        raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
+        raise BotSessionError("当前会话上下文不存在，因此无法使用本方法")
```

### Comparing `melobot-2.6.2/src/melobot/controller/dispatcher.py` & `melobot-2.6.3/src/melobot/controller/dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import asyncio
 
 from ..base.typing import TYPE_CHECKING, BotLife, PriorLevel, Type, Union
-from ..utils.logger import log_exc
 
 if TYPE_CHECKING:
-    from ..base.abc import BaseLogger
     from ..bot.hook import BotHookBus
     from ..context.session import BotSessionManager
     from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
     from ..plugin.handler import EventHandler
+    from ..utils.logger import BotLogger
 
 
 class BotDispatcher:
     """Bot 分发模块。负责将传递的事件分发到各事件通道 （接收的事件类型：消息、请求、通知和元事件）"""
 
     def __init__(self) -> None:
         super().__init__()
         self.handlers: dict[Type["EventHandler"], list["EventHandler"]] = {}
         self._ready_signal = asyncio.Event()
 
     def _bind(
         self,
-        channel_map: dict[str, tuple[Type["EventHandler"], ...]],
+        channel_map: dict[type, tuple[Type["EventHandler"], ...]],
         bot_bus: "BotHookBus",
         ctx_manager: Type["BotSessionManager"],
-        logger: "BaseLogger",
+        logger: "BotLogger",
     ) -> None:
         self.logger = logger
         self._channel_map = channel_map
         self._bot_bus = bot_bus
-        self._ctx_managger = ctx_manager
+        self._ctx_manager = ctx_manager
 
         for tuple in self._channel_map.values():
             for channel in tuple:
                 if channel not in self.handlers.keys():
                     self.handlers[channel] = []
 
     def add_handlers(self, handlers: list["EventHandler"]) -> None:
         """绑定事件处理器列表"""
         for handler in handlers:
             self.handlers[handler.__class__].append(handler)
+
         for k in self.handlers.keys():
             self.handlers[k] = sorted(
                 self.handlers[k], key=lambda x: x.priority, reverse=True
             )
 
     def _set_ready(self) -> None:
         self._ready_signal.set()
@@ -53,38 +53,44 @@
         event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
         channel: Type["EventHandler"],
     ) -> None:
         """向指定的通道推送事件"""
         try:
             permit_priority = PriorLevel.MIN.value
             handlers = self.handlers[channel]
+
             for handler in handlers:
                 # 事件处理器优先级不够，则不分配给它处理
                 if handler.priority < permit_priority:
                     continue
+
                 if handler._direct_rouse and (
-                    await self._ctx_managger.try_attach(event, handler)
+                    await self._ctx_manager.try_attach(event, handler)
                 ):
                     if handler.set_block and handler.priority > permit_priority:
                         permit_priority = handler.priority
                     continue
+
                 # evoke 返回的值用于判断，事件处理器内部经过各种检查后，是否选择处理这个事件。
                 if not (await handler.evoke(event)):
                     # 如果决定不处理，则会跳过此次循环（也就是不进行“可能存在的优先级阻断操作”）
                     continue
+
                 if handler.set_block and handler.priority > permit_priority:
                     permit_priority = handler.priority
+
         except Exception as e:
             self.logger.error("bot dispatcher 抛出异常")
-            self.logger.error(f"异常点 event：{event:hexid}\n{event:raw}")
-            log_exc(self.logger, locals(), e)
+            self.logger.obj(event.raw, f"异常点 event {event:hexid}", level="ERROR")
+            self.logger.exc(locals=locals())
 
     async def dispatch(
         self, event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"]
     ) -> None:
         """把事件分发到对应的事件通道"""
         await self._ready_signal.wait()
         await self._bot_bus.emit(BotLife.EVENT_BUILT, event, wait=True)
         self.logger.debug(f"event {event:hexid} built hook 已完成")
-        for channel in self._channel_map[event.type]:
+
+        for channel in self._channel_map[type(event)]:
             self.logger.debug(f"向 {channel.__name__} 通道广播 event {event:hexid}")
             asyncio.create_task(self.broadcast(event, channel))
```

### Comparing `melobot-2.6.2/src/melobot/controller/responder.py` & `melobot-2.6.3/src/melobot/controller/responder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 import asyncio
 from asyncio import Future
 
 from ..base.typing import TYPE_CHECKING, cast
 from ..context.session import ActionResponse
-from ..utils.logger import log_exc, log_obj
 
 if TYPE_CHECKING:
-    from ..base.abc import AbstractConnector, BaseLogger, BotAction
+    from ..base.abc import AbstractConnector, BotAction
+    from ..utils.logger import BotLogger
 
 
 class BotResponder:
     """Bot 响应模块，是 action 发送方和 bot 连接模块的媒介。 提供 action 发送、响应回送功能"""
 
     def __init__(self) -> None:
         super().__init__()
         self._resp_table: dict[str, Future[ActionResponse]] = {}
-        self.logger: "BaseLogger"
+        self.logger: "BotLogger"
         self._action_sender: "AbstractConnector"
 
         self._ready_signal = asyncio.Event()
 
-    def _bind(self, logger: "BaseLogger", connector: "AbstractConnector") -> None:
+    def _bind(self, logger: "BotLogger", connector: "AbstractConnector") -> None:
         self.logger = logger
         self._action_sender = connector
 
     def _set_ready(self) -> None:
         self._ready_signal.set()
 
     async def respond(self, resp: ActionResponse) -> None:
         await self._ready_signal.wait()
 
         try:
-            if self.logger.check_level_flag("DEBUG"):
-                log_obj(self.logger.debug, resp.raw, f"收到 resp {resp:hexid}")
+            if self.logger._check_level("DEBUG"):
+                self.logger.obj(resp.raw, f"收到 resp {resp:hexid}")
+
             if resp.id is None:
                 return
+
             else:
                 resp_fut = self._resp_table.get(resp.id)
-                if resp_fut:
-                    resp_fut.set_result(resp)
-                    self._resp_table.pop(resp.id)
-                else:
-                    self.logger.error(f"收到了不匹配的携带 id 的响应：{resp.raw}")
+                if resp_fut is None:
+                    self.logger.obj(resp.raw, "收到了不匹配携带 id 的响应", level="ERROR")
+                    return
+
+                resp_fut.set_result(resp)
+                self._resp_table.pop(resp.id)
+
         except asyncio.InvalidStateError:
             self.logger.warning(
-                "等待响应的异步任务已被取消，这可能意味着连接器响应过慢，或任务设置的超时时间太短"
+                "响应的等待被取消，这可能意味着连接质量差，或等待超时时间太短"
             )
             self._resp_table.pop(cast(str, resp.id))
+
         except Exception as e:
             self.logger.error("bot responder.dispatch 抛出异常")
-            log_obj(self.logger.error, resp, "异常点 resp_event")
-            log_exc(self.logger, locals(), e)
+            self.logger.obj(resp, "异常点 resp_event", level="ERROR")
+            self.logger.exc(locals=locals())
 
     async def take_action(self, action: "BotAction") -> None:
         """响应器发送 action, 不等待完成"""
         await self._ready_signal.wait()
+
         await self._action_sender._send(action)
         return None
 
     async def take_action_wait(self, action: "BotAction") -> Future[ActionResponse]:
         """响应器发送 action，并返回一个 Future 用于等待完成"""
         await self._ready_signal.wait()
+
         fut: Future[ActionResponse] = Future()
-        self._resp_table[cast(str, action.resp_id)] = fut
+        fut_id = cast(str, action.resp_id)
+        self._resp_table[fut_id] = fut
+
         await self._action_sender._send(action)
         return fut
```

### Comparing `melobot-2.6.2/src/melobot/io/duplex_http.py` & `melobot-2.6.3/src/melobot/io/duplex_http.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 import aiohttp
 import aiohttp.log
 import aiohttp.web
 from aiohttp.client_exceptions import ClientConnectorError
 
 from ..base.abc import AbstractConnector, BotLife
-from ..base.typing import TYPE_CHECKING, ModuleType, Optional, Union, cast
+from ..base.typing import TYPE_CHECKING, Optional, TracebackType, Union, cast
 from ..context.session import ActionResponse
-from ..utils.logger import log_exc, log_obj
 
 if TYPE_CHECKING:
-    from ..base.abc import BotAction, BotEvent
+    from ..base.abc import BotAction
     from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
 
 
 class HttpConn(AbstractConnector):
     """HTTP 全双工连接器
 
     HTTP 全双工连接器将会同时开启 HTTP 服务端和客户端。
@@ -81,193 +80,197 @@
         self.secret = secret
         #: 操作鉴权的 access_token
         self.access_token = access_token
 
         self._send_queue: asyncio.Queue["BotAction"] = asyncio.Queue()
         self._pre_recv_time = time.time_ns()
         self._pre_send_time = time.time_ns()
+
         self._closed = asyncio.Event()
         self._close_lock = asyncio.Lock()
         self._onebot_onlined = asyncio.Event()
+
         self._allow_reconn = allow_reconnect
         self._connected_flag = False
 
     async def _start(self) -> None:
         """启动连接器"""
-        # 打开一个会话用于与 onebot 实现程序建立连接
         self.client_session = aiohttp.ClientSession()
-        # 开启 HTTP 服务端
         app = aiohttp.web.Application()
         app.add_routes([aiohttp.web.post("/", self._listen)])
         runner = aiohttp.web.AppRunner(app)
         await runner.setup()
         self.serve_site = aiohttp.web.TCPSite(runner, self.host, self.port)
         await self.serve_site.start()
 
-        self.logger.info(
-            "HTTP 通信就绪，等待 OneBot 实现程序上线中（即上报第一个事件）"
-        )
+        self.logger.info("HTTP 通信就绪，等待 OneBot 实现程序上线中（即上报第一个事件）")
         await self._onebot_onlined.wait()
         self.logger.info("HTTP 双向通信已建立")
         self._connected_flag = True
 
         if self.max_interval is not None and self.max_interval > 0:
-            asyncio.create_task(self._overtime_monitor(self.max_interval))
+            _monitor = self._overtime_monitor(self.max_interval)
+            asyncio.create_task(_monitor)
+
         await self._bot_bus.emit(BotLife.FIRST_CONNECTED)
         self.logger.debug("FIRST_CONNECTED hook 已完成")
 
     async def _close(self) -> None:
         """关闭连接器"""
         if self._closed.is_set():
             return
+
         async with self._close_lock:
             if self._closed.is_set():
                 return
-            # 关闭 HTTP 服务端
             await self.serve_site.stop()
-            # 关闭与 onebot 实现程序的连接会话
             await self.client_session.close()
             self._closed.set()
             self.logger.info("HTTP 双向通信已停止")
 
     async def _overtime_monitor(self, interval: float) -> None:
         """通过是否超时判断 OneBot 实现程序是否掉线"""
         try:
             while True:
                 if (abs(time.time_ns() - self._pre_recv_time)) / 1e9 > interval:
-                    self.logger.warning(
-                        "OneBot 实现程序已掉线，正在等待 OneBot 实现程序重新上线"
-                    )
+                    self.logger.warning("OneBot 实现程序已掉线，等待它重新上线中")
                     self._onebot_onlined.clear()
                     await self._onebot_onlined.wait()
+
                 await asyncio.sleep(interval)
+
         except asyncio.CancelledError:
             pass
 
     async def __aenter__(self) -> "HttpConn":
         asyncio.create_task(self._start())
         asyncio.create_task(self._watch_queue())
         return self
 
     async def __aexit__(
-        self, exc_type: type[Exception], exc_val: Exception, exc_tb: ModuleType
+        self, exc_type: type[Exception], exc_val: Exception, exc_tb: TracebackType
     ) -> bool:
         await self._close()
         if await super().__aexit__(exc_type, exc_val, exc_tb):
             return True
+
         self.logger.error("连接器出现预期外的异常")
-        log_exc(self.logger, locals(), exc_val)
+        self.logger.exc(e=exc_val, locals=locals())
         return False
 
     async def _listen(self, request: aiohttp.web.Request) -> aiohttp.web.Response:
         """从 OneBot 实现程序接收一个上报，并处理"""
         data = await request.content.read()
 
         if self.secret is not None:
             sign = hmac.new(self.secret.encode(), data, "sha1").hexdigest()
             recv_sign = request.headers["X-Signature"][len("sha1=") :]
+
             if sign != recv_sign:
                 self.logger.error("OneBot 实现程序鉴权不通过，本次上报数据将不会被处理")
-                log_obj(self.logger.error, data, "试图上报的数据：")
+                self.logger.obj(data, "试图上报的数据：", level="ERROR")
                 return
 
         self._pre_recv_time = time.time_ns()
-
         await self._ready_signal.wait()
+
         if not self._onebot_onlined.is_set():
             self._onebot_onlined.set()
-
             if self._connected_flag:
                 self.logger.info("OneBot 实现程序已经重新上线")
                 await self._bot_bus.emit(BotLife.RECONNECTED)
                 self.logger.debug("RECONNECTED hook 已完成")
 
         try:
             raw_event = json.loads(data.decode())
-            if self.logger.check_level_flag("DEBUG"):
-                self.logger.debug(f"收到上报，未格式化的字典：\n{raw_event}")
+            if self.logger._check_level("DEBUG"):
+                self.logger.obj(raw_event, "收到上报，未格式化的字典")
+
             event = self._event_builder.try_build(raw_event)
-            if self.logger.check_level_flag("DEBUG") and event is not None:
-                log_obj(self.logger.debug, event.raw, f"event {event:hexid} 构建完成")
+            if self.logger._check_level("DEBUG") and event is not None:
+                self.logger.obj(event.raw, f"event {event:hexid} 构建完成")
+
             event = cast(
                 Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
                 event,
             )
             asyncio.create_task(self._common_dispatcher.dispatch(event))
+
         except Exception as e:
             self.logger.error("bot 连接器监听任务抛出异常")
-            log_obj(self.logger.error, raw_event, "异常点的上报数据")
-            log_exc(self.logger, locals(), e)
+            self.logger.obj(raw_event, "异常点的上报数据", level="ERROR")
+            self.logger.exc(locals=locals())
+
         finally:
             return aiohttp.web.Response(status=204)
 
     async def _send(self, action: "BotAction") -> None:
         """发送一个 action 给连接器，实际上是先提交到 send_queue"""
         await self._ready_signal.wait()
-        await self._onebot_onlined.wait()
 
+        await self._onebot_onlined.wait()
         if self.slack:
             self.logger.debug(f"action {action:hexid} 因 slack 状态被丢弃")
             return
+
         await self._send_queue.put(action)
         self.logger.debug(f"action {action:hexid} 已成功加入发送队列")
 
-    async def _watch_queue(self) -> None:
-        """真正的发送方法。从 send_queue 提取 action 并按照一些处理步骤操作"""
+    async def _take_action(self, action: "BotAction") -> None:
+        try:
+            headers: dict | None = None
+            if self.access_token is not None:
+                headers = {"Authorization": f"Bearer {self.access_token}"}
+
+            http_resp = await self.client_session.post(
+                f"{self.onebot_url}/{action.type}",
+                json=action.params,
+                headers=headers,
+            )
+            if action.resp_id is None:
+                return
 
-        async def take_action(action: "BotAction") -> None:
-            try:
-                headers: dict | None = None
-                if self.access_token is not None:
-                    headers = {"Authorization": f"Bearer {self.access_token}"}
-
-                http_resp = await self.client_session.post(
-                    f"{self.onebot_url}/{action.type}",
-                    json=action.params,
-                    headers=headers,
-                )
-                if action.resp_id is None:
-                    return
-                resp_dict: dict = await http_resp.json()
-                resp = ActionResponse(resp_dict)
-                resp.id = action.resp_id
-                asyncio.create_task(self._resp_dispatcher.respond(resp))
-            except (RuntimeError, ClientConnectorError):
-                if not self._allow_reconn:
-                    self.logger.error("OneBot 实现程序已掉线，无法再执行行为操作")
-                    await self._close()
-                else:
-                    self.logger.warning(
-                        "OneBot 实现程序已掉线，正在等待 OneBot 实现程序重新上线"
-                    )
-                    self._onebot_onlined.clear()
-            except aiohttp.ContentTypeError:
-                self.logger.error(
-                    "bot 连接器无法解析上报数据。可能是 access_token 未配置或错误"
-                )
-            except Exception as e:
-                self.logger.error("bot 连接器发送任务抛出预期外的异常：")
-                log_exc(self.logger, locals(), e)
+            resp_dict: dict = await http_resp.json()
+            resp = ActionResponse(resp_dict)
+            resp.id = action.resp_id
+            asyncio.create_task(self._resp_dispatcher.respond(resp))
+
+        except (RuntimeError, ClientConnectorError):
+            if not self._allow_reconn:
+                self.logger.error("OneBot 实现程序已掉线，无法再执行行为操作")
+                await self._close()
+            else:
+                self.logger.warning("OneBot 实现程序已掉线，正在等待它重新上线")
+                self._onebot_onlined.clear()
+
+        except aiohttp.ContentTypeError:
+            self.logger.error("连接器无法解析上报数据。可能是 access_token 未配置或错误")
+
+        except Exception as e:
+            self.logger.error("bot 连接器发送任务抛出预期外的异常：")
+            self.logger.exc(locals=locals())
 
+    async def _watch_queue(self) -> None:
+        """真正的发送方法。从 send_queue 提取 action 并按照一些处理步骤操作"""
         await self._ready_signal.wait()
+
         try:
             while True:
                 action = await self._send_queue.get()
                 await self._onebot_onlined.wait()
-                if self.logger.check_level_flag("DEBUG"):
-                    log_obj(
-                        self.logger.debug,
-                        action.__dict__,
-                        f"action {action:hexid} 准备发送",
-                    )
+
+                if self.logger._check_level("DEBUG"):
+                    self.logger.obj(action.__dict__, f"action {action:hexid} 准备发送")
+
                 await self._bot_bus.emit(BotLife.ACTION_PRESEND, action, wait=True)
                 self.logger.debug(f"action {action:hexid} presend hook 已完成")
-                wait_time = self.cd_time - (
-                    (time.time_ns() - self._pre_send_time) / 1e9
-                )
+
+                wait_time = self.cd_time - ((time.time_ns() - self._pre_send_time) / 1e9)
                 self.logger.debug(f"action {action:hexid} 冷却等待：{wait_time}")
                 await asyncio.sleep(wait_time)
-                asyncio.create_task(take_action(action))
+
+                asyncio.create_task(self._take_action(action))
                 self.logger.debug(f"action {action:hexid} 已发送")
                 self._pre_send_time = time.time_ns()
+
         except asyncio.CancelledError:
             self.logger.debug("连接器发送队列监视任务已被结束")
```

### Comparing `melobot-2.6.2/src/melobot/io/forward_ws.py` & `melobot-2.6.3/src/melobot/io/forward_ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from itertools import count
 
 import websockets
 from websockets.exceptions import ConnectionClosed
 
 from ..base.abc import AbstractConnector, BotLife
 from ..base.exceptions import BotRuntimeError
-from ..base.typing import TYPE_CHECKING, Any, ModuleType, Optional, Type, Union, cast
+from ..base.typing import TYPE_CHECKING, Any, Optional, TracebackType, Type, Union, cast
 from ..context.session import ActionResponse
-from ..utils.logger import log_exc, log_obj
 
 if TYPE_CHECKING:
     import websockets.client
 
     from ..base.abc import BotAction
     from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
 
@@ -52,64 +51,68 @@
         super().__init__(cd_time)
         #: 连接失败最大重试次数
         self.max_retry: int = max_retry
         #: 连接失败重试间隔
         self.retry_delay: float = retry_delay if retry_delay > 0 else 0
         #: ws 连接的 url（形如：ws://xxx:xxx）
         self.url = f"ws://{connect_host}:{connect_port}"
-        #: 连接对象
-        self.conn: "websockets.client.WebSocketClientProtocol"
+        #: 连接对象（未建立连接时为空，连接建立后可认为一定不为空）
+        self.conn: Optional["websockets.client.WebSocketClientProtocol"] = None
         #: 连接器操作鉴权的 token
         self.access_token = access_token
 
         self._send_queue: asyncio.Queue["BotAction"] = asyncio.Queue()
         self._pre_send_time = time.time_ns()
+
         self._client_close: asyncio.Future[Any]
         self._conn_ready = asyncio.Event()
+
         self._allow_reconn = allow_reconnect
         self._reconn_flag = False
+
         self._run_lock = asyncio.Lock()
 
     async def _run(self) -> None:
         """运行客户端"""
         headers: dict | None = None
         if self.access_token is not None:
             headers = {"Authorization": f"Bearer {self.access_token}"}
 
         async with self._run_lock:
             self._client_close = asyncio.Future()
-            created_flag = False
+            ok_flag = False
             retry_iter = count(0) if self.max_retry < 0 else range(self.max_retry + 1)
 
             for _ in retry_iter:
                 try:
-                    self.conn = await websockets.connect(
-                        self.url, extra_headers=headers
-                    )
-                    created_flag = True
+                    self.conn = await websockets.connect(self.url, extra_headers=headers)
+                    ok_flag = True
                     break
+
                 except Exception as e:
                     self.logger.warning(
                         f"ws 连接建立失败，{self.retry_delay}s 后自动重试。错误：{e}"
                     )
                     if "403" in str(e):
                         self.logger.warning("403 错误可能是 access_token 未配置或无效")
                     await asyncio.sleep(self.retry_delay)
-            if not created_flag:
+
+            if not ok_flag:
                 raise BotRuntimeError("连接重试已达最大重试次数，已放弃建立连接")
 
             try:
                 self.logger.info("连接器与 OneBot 实现程序建立了 ws 连接")
                 self._conn_ready.set()
                 asyncio.create_task(self._listen())
                 await self._client_close
             finally:
-                await self.conn.close()
-                await self.conn.wait_closed()
-                self.logger.info("ws 客户端连接已关闭")
+                if self.conn is not None:
+                    await self.conn.close()
+                    await self.conn.wait_closed()
+                    self.logger.info("ws 客户端连接已关闭")
 
     def _close(self) -> None:
         """关闭连接"""
         if self._client_close.done():
             return
         else:
             self._allow_reconn = False
@@ -124,116 +127,125 @@
 
     async def __aenter__(self) -> "ForwardWsConn":
         asyncio.create_task(self._run())
         asyncio.create_task(self._watch_queue())
         return self
 
     async def __aexit__(
-        self, exc_type: Type[Exception], exc_val: Exception, exc_tb: ModuleType
+        self, exc_type: Type[Exception], exc_val: Exception, exc_tb: TracebackType
     ) -> bool:
         self._close()
         if await super().__aexit__(exc_type, exc_val, exc_tb):
             return True
+
         self.logger.error("连接器出现预期外的异常")
-        log_exc(self.logger, locals(), exc_val)
+        self.logger.exc(locals=locals())
         return False
 
     async def _send(self, action: "BotAction") -> None:
         """发送一个 action 给连接器。实际上是先提交到 send_queue"""
         await self._ready_signal.wait()
         await self._conn_ready.wait()
 
         if self.slack:
             self.logger.debug(f"action {action:hexid} 因 slack 状态被丢弃")
             return
+
         await self._send_queue.put(action)
         self.logger.debug(f"action {action:hexid} 已成功加入发送队列")
 
     async def _watch_queue(self) -> None:
         """真正的发送方法。从 send_queue 提取 action 并按照一些处理步骤操作"""
         await self._ready_signal.wait()
 
         try:
             while True:
                 action = await self._send_queue.get()
                 await self._conn_ready.wait()
-                if self.logger.check_level_flag("DEBUG"):
-                    log_obj(
-                        self.logger.debug,
-                        action.__dict__,
-                        f"action {action:hexid} 准备发送",
-                    )
+
+                if self.logger._check_level("DEBUG"):
+                    self.logger.obj(action.__dict__, f"action {action:hexid} 准备发送")
+
                 await self._bot_bus.emit(BotLife.ACTION_PRESEND, action, wait=True)
                 self.logger.debug(f"action {action:hexid} presend hook 已完成")
+
                 action_str = action.flatten()
-                wait_time = self.cd_time - (
-                    (time.time_ns() - self._pre_send_time) / 1e9
-                )
+                wait_time = self.cd_time - ((time.time_ns() - self._pre_send_time) / 1e9)
                 self.logger.debug(f"action {action:hexid} 冷却等待：{wait_time}")
                 await asyncio.sleep(wait_time)
+
+                self.conn = cast("websockets.client.WebSocketClientProtocol", self.conn)
                 await self.conn.send(action_str)
                 self.logger.debug(f"action {action:hexid} 已发送")
                 self._pre_send_time = time.time_ns()
+
         except asyncio.CancelledError:
             self.logger.debug("连接器发送队列监视任务已被结束")
         except ConnectionClosed:
-            self.logger.error(
-                "连接器与 OneBot 实现程序的通信已经停止，无法再执行行为操作"
-            )
+            self.logger.error("与 OneBot 实现程序的通信已经停止，无法再执行操作")
 
     async def _listen(self) -> None:
         """从 OneBot 实现程序接收一个事件，并处理"""
         await self._ready_signal.wait()
         await self._conn_ready.wait()
+
         if not self._reconn_flag:
             await self._bot_bus.emit(BotLife.FIRST_CONNECTED)
             self.logger.debug("FIRST_CONNECTED hook 已完成")
         else:
             await self._bot_bus.emit(BotLife.RECONNECTED)
             self.logger.debug("RECONNECTED hook 已完成")
 
         try:
             while True:
                 try:
+                    self.conn = cast(
+                        "websockets.client.WebSocketClientProtocol", self.conn
+                    )
                     raw = await self.conn.recv()
-                    self.logger.debug(f"收到上报，未格式化的字符串：\n{raw}")
+                    if self.logger._check_level("DEBUG"):
+                        self.logger.obj(raw, "收到上报，未格式化的字符串")
+
                     if raw == "":
                         continue
+
                     event = self._event_builder.try_build(raw)
-                    if self.logger.check_level_flag("DEBUG") and event is not None:
-                        log_obj(
-                            self.logger.debug,
-                            event.raw,
-                            f"event {event:hexid} 构建完成",
-                        )
+                    if self.logger._check_level("DEBUG") and event is not None:
+                        self.logger.obj(event.raw, f"event {event:hexid} 构建完成")
+
                     if event is None:
                         resp = ActionResponse(raw)
                         asyncio.create_task(self._resp_dispatcher.respond(resp))
                     else:
                         event = cast(
                             Union[
                                 "MessageEvent",
                                 "RequestEvent",
                                 "MetaEvent",
                                 "NoticeEvent",
                             ],
                             event,
                         )
                         asyncio.create_task(self._common_dispatcher.dispatch(event))
+
                 except ConnectionClosed:
                     raise
                 except Exception as e:
                     self.logger.error("bot 连接器监听任务抛出异常")
-                    log_obj(self.logger.error, raw, "异常点的上报数据")
-                    log_exc(self.logger, locals(), e)
+                    self.logger.obj(raw, "异常点的上报数据", level="ERROR")
+                    self.logger.exc(locals=locals())
+
         except asyncio.CancelledError:
             self.logger.debug("连接器监听任务已停止")
         except ConnectionClosed:
             self.logger.debug("连接器与 OneBot 实现程序的通信已经停止")
+
         finally:
+            self.conn = cast("websockets.client.WebSocketClientProtocol", self.conn)
             self.conn.close_timeout = 2
             if self._client_close.done():
                 return
+
             if not self._allow_reconn:
                 self._close()
-                return
-            await self._reconnect()
+            else:
+                await self._reconnect()
```

### Comparing `melobot-2.6.2/src/melobot/io/reverse_ws.py` & `melobot-2.6.3/src/melobot/io/reverse_ws.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 import websockets.server
 
 from ..base.abc import AbstractConnector, BotAction, BotLife
 from ..base.typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    ModuleType,
     Optional,
+    TracebackType,
     Union,
     cast,
 )
 from ..context.session import ActionResponse
-from ..utils.logger import log_exc, log_obj
 
 if TYPE_CHECKING:
     from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
 
 
 class ReverseWsConn(AbstractConnector):
     """反向 websocket 连接器
@@ -56,21 +55,24 @@
         #: 监听的 port
         self.port: int = listen_port
         #: 服务端对象
         self.server: "websockets.server.WebSocketServer"
         #: 连接器操作鉴权的 token
         self.access_token = access_token
 
+        self._conn: "websockets.server.WebSocketServerProtocol"
         self._send_queue: asyncio.Queue["BotAction"] = asyncio.Queue()
         self._pre_send_time = time.time_ns()
+
         self._server_close: asyncio.Future[Any]
-        self._conn: "websockets.server.WebSocketServerProtocol"
+
         self._conn_requested = False
         self._request_lock = asyncio.Lock()
         self._conn_ready = asyncio.Event()
+
         self._allow_reconn = allow_reconnect
         self._reconn_flag = False
 
     async def _req_check(
         self, path: str, headers: websockets.HeadersLike
     ) -> Optional[tuple[http.HTTPStatus, websockets.HeadersLike, bytes]]:
         """拦截握手请求，只允许一个客户端连接"""
@@ -84,15 +86,16 @@
 
         if self._conn_requested:
             return resp_403(reconn_refused)
 
         async with self._request_lock:
             if self._conn_requested:
                 return resp_403(reconn_refused)
-            elif (
+
+            if (
                 self.access_token is not None
                 and headers.get("Authorization") != f"Bearer {self.access_token}"
             ):
                 self.logger.warning("OneBot 实现程序的 access_token 不匹配，拒绝连接")
                 return resp_403(auth_failed)
 
             self._conn_requested = True
@@ -101,14 +104,15 @@
     async def _run(self) -> None:
         """运行服务"""
         self._server_close = asyncio.Future()
         self.server = await websockets.serve(
             self._listen, self.host, self.port, process_request=self._req_check
         )
         self.logger.info("连接器启动了 ws 服务，等待 ws 连接中")
+
         await self._server_close
         self.server.close()
         await self.server.wait_closed()
         self.logger.info("ws 服务已关闭")
 
     def _close(self) -> None:
         """关闭服务"""
@@ -127,118 +131,123 @@
 
     async def __aenter__(self) -> "ReverseWsConn":
         asyncio.create_task(self._run())
         asyncio.create_task(self._watch_queue())
         return self
 
     async def __aexit__(
-        self, exc_type: type[Exception], exc_val: Exception, exc_tb: ModuleType
+        self, exc_type: type[Exception], exc_val: Exception, exc_tb: TracebackType
     ) -> bool:
         self._close()
         if await super().__aexit__(exc_type, exc_val, exc_tb):
             return True
+
         self.logger.error("连接器出现预期外的异常")
-        log_exc(self.logger, locals(), exc_val)
+        self.logger.exc(locals=locals())
         return False
 
     async def _send(self, action: "BotAction") -> None:
         """发送一个 action 给连接器，实际上是先提交到 send_queue"""
         await self._ready_signal.wait()
         await self._conn_ready.wait()
 
         if self.slack:
             self.logger.debug(f"action {action:hexid} 因 slack 状态被丢弃")
             return
+
         await self._send_queue.put(action)
         self.logger.debug(f"action {action:hexid} 已成功加入发送队列")
 
     async def _watch_queue(self) -> None:
         """真正的发送方法。从 send_queue 提取 action 并按照一些处理步骤操作"""
         await self._ready_signal.wait()
 
         try:
             while True:
                 action = await self._send_queue.get()
                 await self._conn_ready.wait()
-                if self.logger.check_level_flag("DEBUG"):
-                    log_obj(
-                        self.logger.debug,
-                        action.__dict__,
-                        f"action {action:hexid} 准备发送",
-                    )
+
+                if self.logger._check_level("DEBUG"):
+                    self.logger.obj(action.__dict__, f"action {action:hexid} 准备发送")
+
                 await self._bot_bus.emit(BotLife.ACTION_PRESEND, action, wait=True)
                 self.logger.debug(f"action {action:hexid} presend hook 已完成")
+
                 action_str = action.flatten()
-                wait_time = self.cd_time - (
-                    (time.time_ns() - self._pre_send_time) / 1e9
-                )
+                wait_time = self.cd_time - ((time.time_ns() - self._pre_send_time) / 1e9)
                 self.logger.debug(f"action {action:hexid} 冷却等待：{wait_time}")
                 await asyncio.sleep(wait_time)
+
                 await self._conn.send(action_str)
                 self.logger.debug(f"action {action:hexid} 已发送")
                 self._pre_send_time = time.time_ns()
+
         except asyncio.CancelledError:
             self.logger.debug("连接器发送队列监视任务已被结束")
         except wse.ConnectionClosed:
-            self.logger.error(
-                "连接器与 OneBot 实现程序的通信已经停止，无法再执行行为操作"
-            )
+            self.logger.error("与 OneBot 实现程序的通信已经停止，无法再执行行为操作")
 
     async def _listen(self, ws: "websockets.server.WebSocketServerProtocol") -> None:
         """从 OneBot 实现程序接收一个事件，并处理"""
-        self._conn = ws
-        self.logger.info("连接器与 OneBot 实现程序建立了 ws 连接")
         await self._ready_signal.wait()
+        self._conn = ws
         self._conn_ready.set()
+        self.logger.info("连接器与 OneBot 实现程序建立了 ws 连接")
+
         if not self._reconn_flag:
             await self._bot_bus.emit(BotLife.FIRST_CONNECTED)
             self.logger.debug("FIRST_CONNECTED hook 已完成")
         else:
             await self._bot_bus.emit(BotLife.RECONNECTED)
             self.logger.debug("RECONNECTED hook 已完成")
 
         try:
             while True:
                 try:
                     raw = await self._conn.recv()
-                    self.logger.debug(f"收到上报，未格式化的字符串：\n{raw}")
+
+                    if self.logger._check_level("DEBUG"):
+                        self.logger.obj(raw, "收到上报，未格式化的字符串")
+
                     if raw == "":
                         continue
+
                     event = self._event_builder.try_build(raw)
-                    if self.logger.check_level_flag("DEBUG") and event is not None:
-                        log_obj(
-                            self.logger.debug,
-                            event.raw,
-                            f"event {event:hexid} 构建完成",
-                        )
+                    if self.logger._check_level("DEBUG") and event is not None:
+                        self.logger.obj(event.raw, f"event {event:hexid} 构建完成")
+
                     if event is None:
                         resp = ActionResponse(raw)
                         asyncio.create_task(self._resp_dispatcher.respond(resp))
                     else:
                         event = cast(
                             Union[
                                 "MessageEvent",
                                 "RequestEvent",
                                 "MetaEvent",
                                 "NoticeEvent",
                             ],
                             event,
                         )
                         asyncio.create_task(self._common_dispatcher.dispatch(event))
+
                 except wse.ConnectionClosed:
                     raise
                 except Exception as e:
                     self.logger.error("bot 连接器监听任务抛出异常")
-                    log_obj(self.logger.error, raw, "异常点的上报数据")
-                    log_exc(self.logger, locals(), e)
+                    self.logger.obj(raw, "异常点的上报数据", level="ERROR")
+                    self.logger.exc(locals=locals())
+
         except asyncio.CancelledError:
             self.logger.debug("连接器监听任务已停止")
         except wse.ConnectionClosed:
             self.logger.debug("连接器与 OneBot 实现程序的通信已经停止")
+
         finally:
             self._conn.close_timeout = 2
             if self._server_close.done():
                 return
+
             if not self._allow_reconn:
                 self._close()
-                return
-            self._restore_wait()
+            else:
+                self._restore_wait()
```

### Comparing `melobot-2.6.2/src/melobot/meta.py` & `melobot-2.6.3/src/melobot/meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import os
 import sys
 from typing import Any
 
 
 class ReadOnly(type):
-    def __new__(cls, name, bases, dic):
+    def __new__(cls, name: str, bases: tuple[type, ...], dic: dict[str, Any]):
         _class = super().__new__(cls, name, bases, dic)
         super().__setattr__(
             _class,
             "__cvars__",
             tuple(k for k in dic if not k.startswith("__")),
         )
         return _class
 
     def __setattr__(self, name: str, value: Any) -> None:
-        if name in self.__cvars__:  # type: ignore[attr-defined]
-            raise AttributeError(
-                f"{self.__name__} 类的类属性 {name} 是只读的，无法修改"
-            )
+        if name in getattr(self, "__cvars__"):
+            raise AttributeError(f"{self.__name__} 类的类属性 {name} 是只读的，无法修改")
         return super().__setattr__(name, value)
 
     def __instance_setattr(self, name: str, value: Any) -> None:
         if hasattr(self, name):
-            raise AttributeError(
-                f"{self.__class__.__name__} 类的实例属性 {name} 是只读的，无法修改"
-            )
+            _class = self.__class__.__name__
+            raise AttributeError(f"{_class} 类的实例属性 {name} 是只读的，无法修改")
         super(self.__class__, self).__setattr__(name, value)
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        self.__setattr__ = ReadOnly.__instance_setattr  # type: ignore[assignment]
+        setattr(self, "__setattr__", ReadOnly.__instance_setattr)
         return super().__call__(*args, **kwargs)
 
 
-__version__ = "2.6.2"
+__version__ = "2.6.3"
 
 
 class MetaInfo(metaclass=ReadOnly):
     """元信息类
 
     .. admonition:: 提示
        :class: tip
```

### Comparing `melobot-2.6.2/src/melobot/models/__init__.py` & `melobot-2.6.3/src/melobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/src/melobot/models/event.py` & `melobot-2.6.3/src/melobot/models/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import json
 import re
 
 from ..base.abc import BotEvent
 from ..base.typing import Any, Callable, Literal, MsgSegment, Optional, cast
-from .msg import _get_seg_datas, _get_segs, to_cq_str, to_segments
+from .msg import get_seg_datas, get_segs, to_cq_str, to_segments
 
 
 class BotEventBuilder:
     @staticmethod
     def try_build(rawEvent: dict | str) -> BotEvent | None:
         if isinstance(rawEvent, str):
             raw: dict[str, str | float | int] = json.loads(rawEvent)
         else:
             raw = rawEvent
 
-        etype = raw.get("post_type")
-        if etype in ("message_sent", "message"):
-            return MessageEvent(raw)
-        elif etype == "request":
-            return RequestEvent(raw)
-        elif etype == "notice":
-            return NoticeEvent(raw)
-        elif etype == "meta_event":
-            return MetaEvent(raw)
-        else:
-            return None
+        match raw.get("post_type"):
+            case "message_sent" | "message":
+                return MessageEvent(raw)
+            case "request":
+                return RequestEvent(raw)
+            case "notice":
+                return NoticeEvent(raw)
+            case "meta_event":
+                return MetaEvent(raw)
+            case _:
+                return None
 
 
 class MessageEvent(BotEvent):
     """消息事件类型
 
     .. admonition:: 提示
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
-    def __init__(self, rawEvent: dict) -> None:
-        super().__init__(rawEvent)
+    def __init__(self, raw: dict) -> None:
+        super().__init__(raw)
         #: 收到事件的机器人 qq 号
-        self.bot_id: int = cast(int, rawEvent.get("self_id"))
+        self.bot_id: int = cast(int, raw.get("self_id"))
         #: 消息事件的消息 id
         self.id: int
         #: 消息事件的发送者数据结构
         self.sender: MessageEvent.Sender
         #: 消息事件的来源群号，私聊时此属性也存在并为 :obj:`None`
         self.group_id: Optional[int]
         #: 使用 CQ 字符串表示的，本事件的所有消息内容
@@ -53,93 +53,98 @@
         #: 本事件的所有消息内容中，纯文本消息的合并字符串
         self.text: str
         #: 消息字体
         self.font: int
         #: 临时消息的来源标记，不是临时消息时为 :obj:`None`
         self.temp_src: Optional[str]
 
-        self._init()
+        self._cq_regex = re.compile(r"\[CQ:.*?\]")
+
+        self.id = raw["message_id"]
+        self.raw_content = self._format_to_str(raw["raw_message"])
+        self.content = self._format_to_array(raw["message"])
+        self.sender = MessageEvent.Sender(
+            raw=raw,
+            isGroup=self.is_group(),
+            isGroupAnonym=self.is_group_anonym(),
+        )
+        self.group_id = raw.get("group_id")
+
+        self.text = self._get_text(self.content)
+        self.font = raw["font"]
+
+        self.temp_src = None
+        if src := raw.get("temp_source"):
+            self.temp_src = MessageEvent._TEMP_SRC_MAP[src]
 
     @property
     def time(self) -> int:
         """事件发生时刻的时间戳"""
         return cast(int, self.raw.get("time"))
 
     @property
     def type(self) -> Literal["message"]:
         """事件的类型（返回指定字面量）"""
         return "message"
 
-    def _init(self) -> None:
-        rawEvent = self.raw
-
-        self._cq_regex = re.compile(r"\[CQ:.*?\]")
-        self.id = rawEvent["message_id"]
-        self.raw_content = self._format_to_str(rawEvent["raw_message"])
-        self.content = self._format_to_array(rawEvent["message"])
-        self.text = self._get_text(self.content)
-        self.font = rawEvent["font"]
-
-        self.temp_src = None
-        temp_src = rawEvent.get("temp_source")
-        if temp_src:
-            self.temp_src = MessageEvent._TEMP_SRC_MAP[temp_src]
-
-        self.sender = MessageEvent.Sender(
-            rawEvent=rawEvent,
-            isGroup=self.is_group(),
-            isGroupAnonym=self.is_group_anonym(),
-        )
-
-        self.group_id = None
-        if self.is_group():
-            self.group_id = rawEvent["group_id"]
+    _TEMP_SRC_MAP = {
+        0: "群聊",
+        1: "QQ咨询",
+        2: "查找",
+        3: "QQ电影",
+        4: "热聊",
+        6: "验证消息",
+        7: "多人聊天",
+        8: "约会",
+        9: "通讯录",
+    }
 
     def _format_to_str(self, content: list | str) -> str:
         """对外部零信任，强制转换为 cq 字符串格式"""
         if not isinstance(content, str):
             return to_cq_str(content)
         else:
             return content
 
     def _format_to_array(self, content: list | str) -> list[MsgSegment]:
         """对外部零信任，强制转换为消息段格式"""
-        if not isinstance(content, str):
-            for item in content:
-                if item["type"] == "text":
-                    continue
-                for k, v in item["data"].items():
-                    if not isinstance(v, str):
-                        continue
-                    if v.isdigit() or (len(v) >= 2 and v[0] == "-" and v[1:].isdigit()):
-                        item["data"][k] = int(v)
-                        continue
-                    try:
-                        item["data"][k] = float(v)
-                    except Exception:
-                        pass
-            return content
-        else:
+        if isinstance(content, str):
             return to_segments(content)
 
-    def _get_text(self, content: list[MsgSegment]) -> str:
-        """获取消息中所有文本消息，返回合并字符串"""
-        text_list: list[str] = []
         for item in content:
             if item["type"] == "text":
-                text_list.append(cast(str, item["data"]["text"]))
+                continue
+
+            for k, v in item["data"].items():
+                if not isinstance(v, str):
+                    continue
+                if v.isdigit() or (len(v) >= 2 and v[0] == "-" and v[1:].isdigit()):
+                    item["data"][k] = int(v)
+                    continue
+
+                try:
+                    item["data"][k] = float(v)
+                except Exception:
+                    pass
+        return content
+
+    def _get_text(self, content: list[MsgSegment]) -> str:
+        """获取消息中所有文本消息，返回合并字符串"""
+        text_list = [
+            cast(str, item["data"]["text"]) for item in content if item["type"] == "text"
+        ]
         return "".join(text_list)
 
     def get_segments(self, type: str) -> list[MsgSegment]:
         """提取指定类型的，消息段对象组成的消息段对象列表
 
         :param type: 消息段类型（对应 OneBot 标准中每种消息段对象的 type）
         :return: 消息段对象列表
         """
-        return _get_segs(self.content, type)
+        return get_segs(self.content, type)
 
     def get_datas(
         self, type: str, data: str, convert: Optional[Callable[[Any], Any]] = None
     ) -> list[Any]:
         """提取指定类型的消息段对象中的指定数据
 
         当没有任何对应类型的消息段时，为空列表。如果有对应类型的消息段，但是指定的数据键名不存在，
@@ -156,39 +161,35 @@
            # datas 将是此事件中，所有 at 消息段的 "qq" 数据值所组成的列表
 
         :param type: 消息段类型（对应 OneBot 标准中每种消息段对象的 type）
         :param data: 消息段对象 `data` 中的键名
         :param convert: 类型转换使用的函数
         :return: 值列表
         """
-        return _get_seg_datas(self.content, type, data, convert)
+        return get_seg_datas(self.content, type, data, convert)
 
     def is_private(self) -> bool:
         """是否为私聊消息（注意群临时会话属于该类别）"""
         return self.raw["message_type"] == "private"
 
     def is_friend(self) -> bool:
         """是否为好友消息"""
-        return (
-            self.raw["message_type"] == "private" and self.raw["sub_type"] == "friend"
-        )
+        return self.raw["message_type"] == "private" and self.raw["sub_type"] == "friend"
 
     def is_group(self) -> bool:
         """是否为群消息（正常群消息、群匿名消息、群自身消息、群系统消息属于该类型）"""
         return self.raw["message_type"] == "group"
 
     def is_group_normal(self) -> bool:
         """是否为正常群消息"""
         return self.raw["message_type"] == "group" and self.raw["sub_type"] == "normal"
 
     def is_group_anonym(self) -> bool:
         """是否为匿名群消息"""
-        return (
-            self.raw["message_type"] == "group" and self.raw["sub_type"] == "anonymous"
-        )
+        return self.raw["message_type"] == "group" and self.raw["sub_type"] == "anonymous"
 
     def is_group_self(self) -> bool:
         """是否为群自身消息（即 bot 自己群中发的消息）"""
         return (
             self.raw["message_type"] == "group" and self.raw["sub_type"] == "group_self"
         )
 
@@ -200,37 +201,25 @@
         """是否为临时会话（属于私聊的一种）"""
         return "temp_source" in self.raw.keys()
 
     def is_group_notice(self) -> bool:
         """是否为群中的\"系统消息\" """
         return self.raw["message_type"] == "group" and self.raw["sub_type"] == "notice"
 
-    _TEMP_SRC_MAP = {
-        0: "群聊",
-        1: "QQ咨询",
-        2: "查找",
-        3: "QQ电影",
-        4: "热聊",
-        6: "验证消息",
-        7: "多人聊天",
-        8: "约会",
-        9: "通讯录",
-    }
-
     class Sender:
         """消息事件发送者数据结构
 
         .. admonition:: 提示
            :class: tip
 
            一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
         """
 
-        def __init__(self, rawEvent: dict, isGroup: bool, isGroupAnonym: bool) -> None:
-            self._rawEvent = rawEvent
+        def __init__(self, raw: dict, isGroup: bool, isGroupAnonym: bool) -> None:
+            self._rawEvent = raw
             self._isGroup = isGroup
             self._isGroupAnonym = isGroupAnonym
 
             #: 发送者的 qq 号
             self.id: int
             #: 发送者昵称
             self.nickname: Optional[str]
@@ -252,47 +241,50 @@
             #: 匿名发送者的 id（此属性只在事件为群匿名消息事件时存在）
             self.anonym_id: Optional[int]
             #: 匿名发送者的名字（此属性只在事件为群匿名消息事件时存在）
             self.anonym_name: Optional[str]
             #: 匿名发送者的匿名 flag（此属性只在事件为群匿名消息事件时存在）
             self.anonym_flag: Optional[str]
 
-            self.id = rawEvent["user_id"]
-            self.nickname = rawEvent["sender"].get("nickname")
-            self.sex = rawEvent["sender"].get("sex")
-            self.age = rawEvent["sender"].get("age")
-
-            self.group_card = rawEvent["sender"].get("card")
-            self.group_role = rawEvent["sender"].get("role")
-            self.group_title = rawEvent["sender"].get("title")
-            self.group_area = rawEvent["sender"].get("area")
-            self.group_level = rawEvent["sender"].get("level")
+            self.id = raw["user_id"]
+            self.nickname = raw["sender"].get("nickname")
+            self.sex = raw["sender"].get("sex")
+            self.age = raw["sender"].get("age")
+
+            self.group_card = raw["sender"].get("card")
+            self.group_role = raw["sender"].get("role")
+            self.group_title = raw["sender"].get("title")
+            self.group_area = raw["sender"].get("area")
+            self.group_level = raw["sender"].get("level")
 
             if isGroup and isGroupAnonym:
-                self.anonym_id = rawEvent["anonymous"].get("id")
-                self.anonym_name = rawEvent["anonymous"].get("name")
-                self.anonym_flag = rawEvent["anonymous"].get("flag")
+                self.anonym_id = raw["anonymous"].get("id")
+                self.anonym_name = raw["anonymous"].get("name")
+                self.anonym_flag = raw["anonymous"].get("flag")
 
         def is_group_owner(self) -> bool:
             """判断是否为群主，若不是或不是群类型消息，返回 False"""
             if not self._isGroup:
                 return False
-            return self.group_role == "owner"
+            else:
+                return self.group_role == "owner"
 
         def is_group_admin(self) -> bool:
             """判断是否为群管理（包含群主），若不是或不是群类型消息，返回 False"""
             if not self._isGroup:
                 return False
-            return self.group_role == "admin" or self.group_role == "owner"
+            else:
+                return self.group_role == "admin" or self.group_role == "owner"
 
         def only_group_member(self) -> bool:
             """判断是否只是群员（注意只是群员，不包括群主、管理和匿名），若不是或不是群类型消息，返回 False"""
             if not self._isGroup:
                 return False
-            return self.group_role == "member"
+            else:
+                return self.group_role == "member"
 
         def is_bot(self) -> bool:
             """判断消息是否是bot自己发送的"""
             return self.id == self._rawEvent["self_id"]
 
 
 class RequestEvent(BotEvent):
@@ -300,58 +292,51 @@
 
     .. admonition:: 提示
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
-    def __init__(self, rawEvent: dict) -> None:
-        super().__init__(rawEvent)
+    def __init__(self, raw: dict) -> None:
+        super().__init__(raw)
 
         #: 收到事件的机器人 qq 号
-        self.bot_id: int = cast(int, rawEvent.get("self_id"))
+        self.bot_id: int = cast(int, raw.get("self_id"))
         #: 事件的来源 qq 号
         self.operator_id: int
         #: 事件的来源群号，请求来源于私聊时此属性为 :obj:`None`
         self.group_id: Optional[int]
         #: 加群或加好友的验证消息
         self.req_comment: str
         #: 加群或加好友请求的 flag，调用相关 API 时，需要使用
         self.req_flag: str
         #: 加群请求类型：直接加入和邀请，请求来源于私聊时此属性为 :obj:`None`
         self.group_req_type: Optional[Literal["add", "invite"]]
 
-        self._init()
+        if self.is_friend_req():
+            self.operator_id = raw["user_id"]
+            self.req_comment = raw["comment"]
+            self.req_flag = raw["flag"]
+        elif self.is_group_req():
+            self.group_req_type = raw.get("sub_type")
+            self.operator_id = raw["user_id"]
+            self.group_id = raw.get("group_id")
+            self.req_comment = raw["comment"]
+            self.req_flag = raw["flag"]
 
     @property
     def time(self) -> int:
         """事件发生时刻的时间戳"""
         return cast(int, self.raw.get("time"))
 
     @property
     def type(self) -> Literal["request"]:
         """事件的类型（返回指定字面量）"""
         return "request"
 
-    def _init(self) -> None:
-        rawEvent = self.raw
-        self.group_req_type = None
-        self.group_id = None
-
-        if self.is_friend_req():
-            self.operator_id = rawEvent["user_id"]
-            self.req_comment = rawEvent["comment"]
-            self.req_flag = rawEvent["flag"]
-        elif self.is_group_req():
-            self.group_req_type = rawEvent["sub_type"]
-            self.operator_id = rawEvent["user_id"]
-            self.group_id = rawEvent["group_id"]
-            self.req_comment = rawEvent["comment"]
-            self.req_flag = rawEvent["flag"]
-
     def is_friend_req(self) -> bool:
         """是否为加好友请求"""
         return self.raw["request_type"] == "friend"
 
     def is_group_req(self) -> bool:
         """是否为加群请求"""
         return self.raw["request_type"] == "group"
@@ -371,21 +356,18 @@
        受 onebot 协议实现项目的影响，及对通知事件本身复杂性的考虑，通知事件大多数实例属性，
        只会在特定类别的通知事件中存在。各个属性的含义与存在的时机，已在下方的注释说明。
 
        如果你仍不确定某个属性在何时出现，建议直接调试查看存在的属性。例如通过
        `print(event.__dict__)` 或调试器查看。
     """
 
-    def __init__(self, rawEvent: dict) -> None:
-        super().__init__(rawEvent)
+    def __init__(self, raw: dict) -> None:
+        super().__init__(raw)
         #: 收到事件的机器人 qq 号
-        self.bot_id: int = cast(int, rawEvent.get("self_id"))
-        # 修复某些 onebot 协议实现，user_id 缺失的问题
-        if "target_id" in rawEvent.keys() and "user_id" not in rawEvent:
-            rawEvent["user_id"] = rawEvent["target_id"]
+        self.bot_id: int = cast(int, raw.get("self_id"))
 
         #: 通知作用者或主体方的 id，如被禁言的一方
         self.user_id: int
         #: 通知若发生在群中的群 id
         self.group_id: int
         #: 通知发起者或操作方的 id，如禁言别人的管理员
         self.operator_id: int
@@ -429,72 +411,87 @@
     def _init(self) -> None:
         """外部确认为该类型事件时，调用此方法。"""
         rawEvent = self.raw
 
         if self.is_friend_recall():
             self.user_id = rawEvent["user_id"]
             self.msg_id = rawEvent["message_id"]
+
         elif self.is_group_recall():
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
             self.operator_id = rawEvent["operator_id"]
             self.msg_id = rawEvent["message_id"]
+
         elif self.is_group_increase():
             self.join_group_type = rawEvent["sub_type"]
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
             self.operator_id = rawEvent["operator_id"]
+
         elif self.is_group_decrease():
             self.leave_group_type = rawEvent["sub_type"]
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
             self.operator_id = rawEvent["operator_id"]
+
         elif self.is_group_admin():
             self.admin_change_type = rawEvent["sub_type"]
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
+
         elif self.is_group_upload():
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
-            self.file = NoticeEvent.File(rawEvent, isGroup=True)
+            self.file = NoticeEvent.File(rawEvent)
+
         elif self.is_group_ban():
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
             self.operator_id = rawEvent["operator_id"]
             self.group_ban_type = rawEvent["sub_type"]
             self.ban_time = rawEvent["duration"]
+
         elif self.is_friend_add():
             self.user_id = rawEvent["user_id"]
+
         elif self.is_poke():
             self.user_id = rawEvent["target_id"]
             self.operator_id = rawEvent["user_id"]
             if "group_id" in rawEvent.keys():
                 self.group_id = rawEvent["group_id"]
+
         elif self.is_lucky_king():
             self.user_id = rawEvent["target_id"]
             self.group_id = rawEvent["group_id"]
             self.operator_id = rawEvent["user_id"]
+
         elif self.is_honor():
             self.honor_change_type = rawEvent["honor_type"]
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
+
         elif self.is_title():
             self.new_title = rawEvent["title"]
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
+
         elif self.is_group_card():
             self.old_card = rawEvent["card_old"]
             self.new_card = rawEvent["card_new"]
             self.user_id = rawEvent["user_id"]
             self.group_id = rawEvent["group_id"]
+
         elif self.is_offline_file():
             self.user_id = rawEvent["user_id"]
-            self.file = NoticeEvent.File(rawEvent, isGroup=False)
+            self.file = NoticeEvent.File(rawEvent)
+
         elif self.is_client_status():
             self.client = NoticeEvent.Client(rawEvent)
+
         elif self.is_essence():
             self.essence_change_type = rawEvent["sub_type"]
             self.user_id = rawEvent["sender_id"]
             self.group_id = rawEvent["group_id"]
             self.operator_id = rawEvent["operator_id"]
             self.msg_id = rawEvent["message_id"]
 
@@ -577,67 +574,65 @@
 
         .. admonition:: 提示
            :class: tip
 
            一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
         """
 
-        def __init__(self, rawEvent: dict, isGroup: bool) -> None:
+        def __init__(self, raw: dict) -> None:
             #: 文件 id，私聊文件上传时为 :obj:`None`
             self.id: Optional[str] = None
             #: 文件名
             self.name: str
             #: 文件大小
             self.size: int
             #: 文件 busid，私聊文件上传时为 :obj:`None`
             self.busid: Optional[int] = None
             #: 文件 url 地址，群聊文件上传时为 :obj:`None`
             self.url: Optional[str] = None
 
-            self.name = rawEvent["file"]["name"]
-            self.size = rawEvent["file"]["size"]
-            if isGroup:
-                self.id = rawEvent["file"]["id"]
-                self.busid = rawEvent["file"]["busid"]
-            else:
-                self.url = rawEvent["file"]["url"]
+            self.name = raw["file"]["name"]
+            self.size = raw["file"]["size"]
+            self.id = raw["file"].get("id")
+            self.busid = raw["file"].get("busid")
+            self.url = raw["file"].get("url")
 
     class Client:
         """客户端在线状态变更通知的客户端信息数据结构
 
         .. admonition:: 提示
            :class: tip
 
            一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
         """
 
-        def __init__(self, rawEvent: dict) -> None:
+        def __init__(self, raw: dict) -> None:
             #: 当前客户端是否在线
-            self.online: bool = rawEvent["online"]
+            self.online: bool = raw["online"]
             #: 当前客户端 id
-            self.id: int = rawEvent["client"]["app_id"]
+            self.id: int = raw["client"]["app_id"]
             #: 客户端设备名称
-            self.name: str = rawEvent["client"]["device_name"]
+            self.name: str = raw["client"]["device_name"]
             #: 客户端设备类型
-            self.kind: str = rawEvent["client"]["device_kind"]
+            self.kind: str = raw["client"]["device_kind"]
 
 
 class MetaEvent(BotEvent):
     """元事件类型
 
     .. admonition:: 提示
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
-    def __init__(self, rawEvent: dict) -> None:
-        super().__init__(rawEvent)
+    def __init__(self, raw: dict) -> None:
+        super().__init__(raw)
         #: 收到事件的机器人 qq 号
-        self.bot_id: int = cast(int, rawEvent.get("self_id"))
+        self.bot_id: int = cast(int, raw.get("self_id"))
 
     @property
     def time(self) -> int:
         """事件发生时刻的时间戳"""
         return cast(int, self.raw.get("time"))
 
     @property
```

### Comparing `melobot-2.6.2/src/melobot/models/msg.py` & `melobot-2.6.3/src/melobot/models/msg.py`

 * *Files 7% similar despite different names*

```diff
@@ -328,28 +328,15 @@
     :param content: 消息结点内容
     :param sendName: 消息结点标记的发送人名字
     :param sendId: 消息结点标记的发送人 qq 号
     :param seq: 消息 seq 号（一般来说你不需要使用这个）
     :param useStd: 消息段对象构造时是否遵循 onebot 标准，默认为否（使用 go-cq 风格）
     :return: onebot 标准中的消息段对象
     """
-    if isinstance(content, str):
-        _ = text_msg(content)
-        if not isinstance(_, list):
-            msgs = [_]
-    elif isinstance(content, dict):
-        msgs = [content]
-    elif isinstance(content, list):
-        temp = []
-        for _ in content:
-            if isinstance(_, list):
-                temp.extend(_)
-            else:
-                temp.append(_)
-        msgs = temp
+    msgs = to_msg_segment(content)
     if not useStd:
         ret: MsgNode = {
             "type": "node",
             "data": {"name": sendName, "uin": str(sendId), "content": msgs},
         }
         if seq:
             ret["data"]["seq"] = seq  # type: ignore[typeddict-unknown-key]
@@ -430,105 +417,141 @@
 def to_segments(s: str) -> list[MsgSegment]:
     """将 cq 字符串转换为消息段对象列表
 
     :param s: cq 字符串
     :return: 消息段对象列表
     """
 
+    cq_texts: list[str] = []
+
     def replace_func(m) -> str:
         s, e = m.regs[0]
         cq_texts.append(m.string[s:e])
         return "\u0000"
 
     cq_regex = re.compile(r"\[CQ:.*?\]")
-    cq_texts: list[str] = []
+
     no_cq_str = cq_regex.sub(replace_func, s)
     pure_texts = map(
         lambda x: f"[CQ:text,text={x}]" if x != "" else x,
         no_cq_str.split("\u0000"),
     )
-    _: str = "".join(
+    cq_entity_str: str = "".join(
         chain.from_iterable(zip_longest(pure_texts, cq_texts, fillvalue=""))
     )
 
-    cq_entity: list[str] = _.split("]")[:-1]
+    cq_entity: list[str] = cq_entity_str.split("]")[:-1]
     content: list = []
+
     for e in cq_entity:
-        __ = e.split(",")
-        cq_type = __[0][4:]
+        cq_parts = e.split(",")
+        cq_type = cq_parts[0][4:]
         data: dict[str, float | int | str] = {}
-        for param_pair in __[1:]:
+
+        for param_pair in cq_parts[1:]:
             name, val = param_pair.split("=")
+
             if cq_type != "text":
                 val = cq_anti_escape(val)
-            if val.isdigit() or (len(val) >= 2 and val[0] == "-" and val[1:].isdigit()):
-                data[name] = int(val)
-                continue
+
             try:
                 data[name] = float(val)
+                tmp = int(val)
+                if tmp == data[name]:
+                    data[name] = tmp
             except Exception:
                 data[name] = val
+
         content.append({"type": cq_type, "data": data})
+
     return content
 
 
 def to_cq_str(content: list[MsgSegment]) -> str:
     """将消息段对象列表转换为 cq 字符串
 
     :param content: 消息段对象列表
     :return: cq 字符串
     """
     if isinstance(content, str):
         return content
+
     msgs: list[str] = []
     for item in content:
         if item["type"] == "text":
             msgs.append(cast(str, item["data"]["text"]))
             continue
-        s = f"[CQ:{item['type']}"
-        for k, v in item["data"].items():
-            s += f",{k}={cq_escape(str(v))}"
-        s += "]"
+
+        type = item["type"]
+        params = ",".join(f"{k}={cq_escape(str(v))}" for k, v in item["data"].items())
+        s = f"[CQ:{type},{params}]"
         msgs.append(s)
+
     return "".join(msgs)
 
 
-def _to_cq_str_action(action: "BotAction") -> "BotAction":
+def to_msg_segment(content: str | MsgSegment | list[MsgSegment]) -> list[MsgSegment]:
+    """将多种可能的消息格式，统一转换为 cq 消息列表"""
+
+    def verify_segment(obj: Any) -> bool:
+        return (
+            isinstance(obj, dict)
+            and obj.get("type") is not None
+            and isinstance(obj.get("data"), dict)
+        )
+
+    if isinstance(content, str):
+        return [text_msg(content)]
+
+    elif verify_segment(content):
+        return [cast(MsgSegment, content)]
+
+    elif (
+        isinstance(content, list)
+        and len(content) > 0
+        and all(verify_segment(obj) for obj in content)
+    ):
+        return content
+
+    else:
+        raise BotValueError(
+            f"发送的消息内容有误，当前值是：{content}，但需要以下格式之一：字符串、消息段对象、消息段对象的列表（不可为空）"
+        )
+
+
+def to_cq_str_action(action: "BotAction") -> "BotAction":
+
     def _format_msg_action(action: "BotAction") -> None:
         action.params["message"] = to_cq_str(action.params["message"])
 
     def _format_forward_action(action: "BotAction") -> None:
         for item in action.params["messages"]:
             if "id" in item["data"].keys():
                 continue
             item["data"]["content"] = to_cq_str(item["data"]["content"])
 
     _action = deepcopy(action)
+
     if _action.type == "send_msg":
         _format_msg_action(_action)
     elif _action.type in ("send_private_forward_msg", "send_group_forward_msg"):
         _format_forward_action(_action)
     else:
-        raise BotValueError(
-            "传入的 action 类型不是发送消息、发送转发消息，因此不可被 cq 序列化"
-        )
+        raise BotValueError("传入的 action 不可被 cq 序列化")
     return _action
 
 
-def _get_segs(content: list[MsgSegment], cq_type: str) -> list[MsgSegment]:
+def get_segs(content: list[MsgSegment], cq_type: str) -> list[MsgSegment]:
     return [item for item in content if item["type"] == cq_type]
 
 
-def _get_seg_datas(
+def get_seg_datas(
     content: list[MsgSegment],
     cq_type: str,
     param: str,
     type: Optional[Callable[[Any], Any]] = None,
 ) -> list[Any]:
-    res: list[Any] = []
-    for item in content:
-        if item["type"] == cq_type:
-            val = item["data"].get(param)
-            res.append(val)
+    res = (item["data"].get(param) for item in content if item["type"] == cq_type)
     if type is not None:
-        res = list(map(lambda x: type(x), res))
-    return res
+        return list(map(lambda x: type(x), res))
+    else:
+        return list(res)
```

### Comparing `melobot-2.6.2/src/melobot/plugin/handler.py` & `melobot-2.6.3/src/melobot/plugin/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 import asyncio
 
 from ..base.abc import BotParser
 from ..base.exceptions import BotValueError, FuncSafeExited
 from ..base.typing import (
     TYPE_CHECKING,
     Any,
-    Callable,
-    Coroutine,
+    AsyncCallable,
+    Awaitable,
     Optional,
+    P,
     PriorLevel,
     T,
     Type,
     Union,
-    Void,
     cast,
 )
 from ..context.session import SESSION_LOCAL, BotSessionManager, any_event
-from ..utils.logger import log_exc
+from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
 
 if TYPE_CHECKING:
     from ..base.abc import BotChecker, BotMatcher, SessionRule
     from ..context.session import BotSession
-    from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
     from ..utils.logger import BotLogger
     from .init import BotPlugin
 
 
 class EventHandler:
     def __init__(
         self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
+        executor: AsyncCallable[P, None],
         plugin: "BotPlugin",
         logger: "BotLogger",
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         set_block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         super().__init__()
         self.is_valid = True
-
         self.executor = executor
         self.logger = logger
         self.checker = checker
         self.priority = priority
         self.set_block = set_block
         self.temp = temp
 
+        self._plugin = plugin
         self._run_lock = asyncio.Lock()
+
         self._rule = session_rule
         self._hold = session_hold
-        self._plugin = plugin
         self._direct_rouse = direct_rouse
         self._conflict_cb = conflict_cb
         self._wait_flag = conflict_wait
 
         if conflict_wait and conflict_cb:
             raise BotValueError("参数 conflict_wait 为 True 时，冲突回调永远不会被调用")
 
@@ -74,89 +73,94 @@
         """验证事件是否有触发执行的资格（验权）"""
         if self.checker:
             return await self.checker.check(any_event())
         return True
 
     async def _run_on_ctx(
         self,
-        coro: Coroutine[Any, Any, T],
+        obj: Awaitable[T],
         session: "BotSession",
         timeout: Optional[float] = None,
     ) -> T:
-        """在指定 session 上下文中运行协程。异常将会抛出"""
+        """在指定会话上下文中运行协程。异常将会抛出"""
         try:
             s_token = SESSION_LOCAL._add_ctx(session)
-            return await asyncio.wait_for(asyncio.create_task(coro), timeout=timeout)
+            return await asyncio.wait_for(obj, timeout=timeout)
         finally:
             SESSION_LOCAL._del_ctx(s_token)
-            # 这里可能因 bot 停止运行，导致退出事件执行方法时 session 为挂起态。因此需要强制唤醒
+            # 这里可能因 bot 停止运行，导致退出事件执行方法时会话为挂起态。因此需要强制唤醒
             if session._hup_signal.is_set():
                 BotSessionManager._rouse(session)
 
     async def _run(
         self,
-        event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"],
+        event: Union[MessageEvent, RequestEvent, MetaEvent, NoticeEvent],
         pre_session: "BotSession",
     ) -> None:
-        """获取 session 然后准备运行 executor"""
+        """获取会话然后准备运行 executor"""
         try:
             session = None
+
             if not self._direct_rouse:
                 res = await BotSessionManager.try_attach(event, self)
                 if res:
                     return
+
             session = await BotSessionManager.get(event, self)
-            # 如果因为冲突没有获得 session，且指定了冲突回调
+
+            # 如果因为冲突没有获得 会话，且指定了冲突回调
             if session is None and self._conflict_cb:
                 await self._run_on_ctx(self._conflict_cb(), pre_session)
-            # 如果因为冲突没有获得 session，但没有冲突回调
+
+            # 如果因为冲突没有获得 会话，但没有冲突回调
             if session is None:
                 return
-            # 如果没有冲突，正常获得到了 session
+
+            # 如果没有冲突，正常获得到了 会话
             exec_coro = self.executor()
-            self.logger.debug(
-                f"event {event:hexid} 准备在 session {session:hexid} 中处理"
-            )
+            self.logger.debug(f"event {event:hexid} 准备在会话{session:hexid} 中处理")
             session << pre_session
             await self._run_on_ctx(exec_coro, session)
+
         except FuncSafeExited:
             pass
+
         except Exception as e:
-            executor_name = self.executor.__qualname__
-            self.logger.error(
-                f"插件 {self._plugin.ID} 事件处理方法 {executor_name} 发生异常"
-            )
-            self.logger.error(f"异常点 event：{event:hexid}\n{event:raw}")
-            log_exc(self.logger, locals(), e)
+            exec_name = self.executor.__qualname__
+            pid = self._plugin.ID
+            self.logger.error(f"插件 {pid} 事件处理方法 {exec_name} 发生异常")
+            self.logger.obj(event.raw, f"异常点 event {event:hexid}", level="ERROR")
+            self.logger.exc(locals=locals())
+
         finally:
             if session is None:
                 return
-            self.logger.debug(
-                f"event {event:hexid} 在 session {session:hexid} 中运行完毕"
-            )
+            self.logger.debug(f"event {event:hexid} 在会话{session:hexid} 中运行完毕")
             BotSessionManager.recycle(session, alive=self._hold)
 
     async def _pre_process(
-        self, event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"]
+        self, event: Union[MessageEvent, RequestEvent, MetaEvent, NoticeEvent]
     ) -> tuple[bool, "BotSession"]:
         session = BotSessionManager.make_temp(event)
         status = await self._run_on_ctx(self._verify(), session)
         return status, session
 
     async def evoke(
-        self, event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"]
+        self, event: Union[MessageEvent, RequestEvent, MetaEvent, NoticeEvent]
     ) -> bool:
         """接收总线分发的事件的方法。返回是否决定处理的判断。 便于 disptacher 进行优先级阻断。校验通过会自动处理事件。"""
         if not self.is_valid:
             return False
 
         status, tmp_session = await self._pre_process(event)
+
         if status:
             self.logger.debug(
-                f"event {event:hexid} 在 handler {self:hexid} pre_process 通过，处理方法为：{self.executor.__qualname__}"
+                f"event {event:hexid} 在 handler {self:hexid} 完成预处理，"
+                "即将运行处理函数：{self.executor.__qualname__}"
             )
         if not status:
             return False
 
         if not self.temp:
             asyncio.create_task(self._run(event, tmp_session))
             return True
@@ -169,26 +173,26 @@
             else:
                 return False
 
 
 class AllEventHandler(EventHandler):
     def __init__(
         self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
+        executor: AsyncCallable[P, None],
         plugin: Any,
         logger: "BotLogger",
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         set_block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         super().__init__(
             executor,
             plugin,
             logger,
             checker,
             priority,
@@ -201,28 +205,28 @@
             conflict_cb,
         )
 
 
 class MsgEventHandler(EventHandler):
     def __init__(
         self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
+        executor: AsyncCallable[P, None],
         plugin: Any,
         logger: "BotLogger",
         matcher: Optional["BotMatcher"] = None,
         parser: Optional["BotParser"] = None,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         set_block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         super().__init__(
             executor,
             plugin,
             logger,
             checker,
             priority,
@@ -238,49 +242,53 @@
         self.parser = parser
 
         # matcher 和 parser 不能同时存在
         if self.matcher and self.parser:
             raise BotValueError("参数 matcher 和 parser 不能同时存在")
 
     async def _pre_process(
-        self, event: Union["MessageEvent", "RequestEvent", "MetaEvent", "NoticeEvent"]
+        self, event: Union[MessageEvent, RequestEvent, MetaEvent, NoticeEvent]
     ) -> tuple[bool, "BotSession"]:
-        event = cast("MessageEvent", event)
+        event = cast(MessageEvent, event)
         session = BotSessionManager.make_temp(event)
+
         if self.matcher is not None:
-            return (
-                await self._run_on_ctx(self.matcher.match(event.text), session),
-                session,
-            )
+            _match = self.matcher.match(event.text)
+            status = await self._run_on_ctx(_match, session)
+            return status, session
 
         if self.parser is not None:
-            args = await self._run_on_ctx(self.parser.parse(event.text), session)
+            _parse = self.parser.parse(event.text)
+            args = await self._run_on_ctx(_parse, session)
             if args is None:
                 return False, session
             else:
                 BotSessionManager.fill_args(session, args)
 
-        return await self._run_on_ctx(self._verify(), session), session
+        if not await self._run_on_ctx(self._verify(), session):
+            return False, session
+
+        return True, session
 
 
 class ReqEventHandler(EventHandler):
     def __init__(
         self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
+        executor: AsyncCallable[P, None],
         plugin: Any,
         logger: "BotLogger",
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         set_block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         super().__init__(
             executor,
             plugin,
             logger,
             checker,
             priority,
@@ -293,26 +301,26 @@
             conflict_cb,
         )
 
 
 class NoticeEventHandler(EventHandler):
     def __init__(
         self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
+        executor: AsyncCallable[P, None],
         plugin: Any,
         logger: "BotLogger",
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         set_block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         super().__init__(
             executor,
             plugin,
             logger,
             checker,
             priority,
@@ -325,26 +333,26 @@
             conflict_cb,
         )
 
 
 class MetaEventHandler(EventHandler):
     def __init__(
         self,
-        executor: Callable[[], Coroutine[Any, Any, None]],
+        executor: AsyncCallable[P, None],
         plugin: Any,
         logger: "BotLogger",
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         set_block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         super().__init__(
             executor,
             plugin,
             logger,
             checker,
             priority,
@@ -354,13 +362,13 @@
             session_hold,
             direct_rouse,
             conflict_wait,
             conflict_cb,
         )
 
 
-EVENT_HANDLER_MAP: dict[str, tuple[Type[EventHandler], ...]] = {
-    "message": (MsgEventHandler, AllEventHandler),
-    "request": (ReqEventHandler, AllEventHandler),
-    "notice": (NoticeEventHandler, AllEventHandler),
-    "meta": (MetaEventHandler, AllEventHandler),
+EVENT_CHANNELS: dict[type, tuple[Type[EventHandler], ...]] = {
+    MessageEvent: (MsgEventHandler, AllEventHandler),
+    RequestEvent: (ReqEventHandler, AllEventHandler),
+    NoticeEvent: (NoticeEventHandler, AllEventHandler),
+    MetaEvent: (MetaEventHandler, AllEventHandler),
 }
```

### Comparing `melobot-2.6.2/src/melobot/plugin/init.py` & `melobot-2.6.3/src/melobot/plugin/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,46 +8,49 @@
     BotLife,
     EventHandlerArgs,
     PluginSignalHandlerArgs,
     ShareObjArgs,
     ShareObjCbArgs,
 )
 from ..base.exceptions import BotPluginError
+from ..base.ioc import DependManager
 from ..base.tools import to_async
 from ..base.typing import (
     TYPE_CHECKING,
     Any,
+    AsyncCallable,
     Callable,
-    Coroutine,
-    Literal,
     LogicMode,
     Optional,
     P,
     PriorLevel,
+    T,
     Union,
 )
 from ..meta import ReadOnly
-from ..utils.checker import AtMsgChecker, NoticeChecker, ReqChecker
+from ..utils.checker import AtMsgChecker
 from ..utils.matcher import (
     ContainMatcher,
     EndMatcher,
     FullMatcher,
     RegexMatcher,
     StartMatcher,
 )
+from ..utils.parser import CmdArgFormatter, CmdParser
 from .handler import (
     AllEventHandler,
+    EventHandler,
     MetaEventHandler,
     MsgEventHandler,
     NoticeEventHandler,
     ReqEventHandler,
 )
 
 if TYPE_CHECKING:
-    from ..base.abc import SessionRule, WrappedChecker
+    from ..base.abc import SessionRule
     from ..utils.checker import BotChecker
     from ..utils.matcher import BotMatcher
     from ..utils.parser import BotParser
 
 
 class PluginProxy(metaclass=ReadOnly):
     """Bot 插件代理类
@@ -101,40 +104,42 @@
     @staticmethod
     def load_from_dir(plugin_path: str) -> "BotPlugin":
         """从指定插件目录加载插件"""
         if not os.path.exists(os.path.join(plugin_path, "__init__.py")):
             raise BotPluginError(
                 f"{plugin_path} 缺乏入口主文件 __init__.py，插件无法加载"
             )
-        plugin_name = os.path.basename(plugin_path)
-        plugins_folder = str(pathlib.Path(plugin_path).parent.resolve(strict=True))
-        plugins_folder_name = os.path.basename(plugins_folder)
-
-        if plugins_folder not in sys.path:
-            importlib.import_module(plugins_folder_name)
-            sys.path.insert(0, plugins_folder)
-        module = importlib.import_module(
-            f"{plugins_folder_name}.{plugin_name}", f"{plugins_folder_name}"
-        )
+
+        p_name = os.path.basename(plugin_path)
+        p_folder = str(pathlib.Path(plugin_path).parent.resolve(strict=True))
+        p_folder_name = os.path.basename(p_folder)
+
+        if p_folder not in sys.path:
+            importlib.import_module(p_folder_name)
+            sys.path.insert(0, p_folder)
+
+        module = importlib.import_module(f"{p_folder_name}.{p_name}", f"{p_folder_name}")
 
         for obj in module.__dict__.values():
             if isinstance(obj, BotPlugin):
                 plugin = obj
                 break
         else:
             raise BotPluginError("指定的入口主文件中，未发现 Plugin 实例，无效导入")
+
         return plugin
 
     @staticmethod
     def load(target: Union[str, "BotPlugin"]) -> "BotPlugin":
         """加载插件"""
         if isinstance(target, str):
             plugin = PluginLoader.load_from_dir(target)
         else:
             plugin = target
+
         plugin._self_build()
         return plugin
 
 
 class BotPlugin:
     """插件类，使用该类实例化一个插件"""
 
@@ -190,84 +195,92 @@
             self.KEYWORDS,
             self.URL,
             self.MULTI_USE,
             [(args.namespace, args.id) for args in self.__share_args__],
             [(args.namespace, args.id) for args in self.__share_cb_args__],
             [(args.namespace, args.signal) for args in self.__signal_args__],
         )
+
         check_pass = all(
             False
             for pair in self.__proxy__.share_cbs
             if pair not in self.__proxy__.shares
         )
         if not check_pass:
             raise BotPluginError(f"插件 {self.ID} 不能为不属于自己的共享对象绑定回调")
 
+    def _on_event(
+        self, handler_type: type[EventHandler], params: list[Any]
+    ) -> Callable[[AsyncCallable[P, None]], AsyncCallable[P, None]]:
+
+        def save_args(executor: AsyncCallable[P, None]) -> AsyncCallable[P, None]:
+            self.__handler_args__.append(
+                EventHandlerArgs(
+                    executor=DependManager.inject(executor),
+                    type=handler_type,
+                    params=params,
+                )
+            )
+            return executor
+
+        return save_args
+
     def on_event(
         self,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个任意事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=AllEventHandler,
-                    params=[
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self._on_event(
+            AllEventHandler,
+            params=[
+                checker,
+                priority,
+                block,
+                temp,
+                session_rule,
+                session_hold,
+                direct_rouse,
+                conflict_wait,
+                conflict_cb,
+                conflict_cb,
+            ],
+        )
 
     def on_message(
         self,
         matcher: Optional["BotMatcher"] = None,
         parser: Optional["BotParser"] = None,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个消息事件处理方法
 
         :param matcher: 使用的匹配器（和解析器二选一）
         :param parser: 使用的解析器（和匹配器二选一）
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
@@ -275,55 +288,45 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        matcher,
-                        parser,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self._on_event(
+            MsgEventHandler,
+            params=[
+                matcher,
+                parser,
+                checker,
+                priority,
+                block,
+                temp,
+                session_rule,
+                session_hold,
+                direct_rouse,
+                conflict_wait,
+                conflict_cb,
+            ],
+        )
 
     def on_at_qq(
         self,
         qid: Optional[int] = None,
         matcher: Optional["BotMatcher"] = None,
         parser: Optional["BotParser"] = None,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个艾特消息事件处理方法
 
         消息必须是艾特消息，且匹配成功才能被进一步处理。
 
         :param qid: 被艾特的 qq 号。为空则接受所有艾特消息;不为空则只接受指定 qid 被艾特的艾特消息
         :param matcher: 使用的匹配器（和解析器二选一）
@@ -334,60 +337,93 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-        at_checker = AtMsgChecker(qid)
-        wrapped_checker: AtMsgChecker | "WrappedChecker"
-        if checker is not None:
-            wrapped_checker = at_checker & checker
-        else:
-            wrapped_checker = at_checker
+        return self.on_message(
+            matcher,
+            parser,
+            AtMsgChecker(qid) if checker is None else AtMsgChecker(qid) & checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        matcher,
-                        parser,
-                        wrapped_checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
+    def on_command(
+        self,
+        cmd_start: str | list[str],
+        cmd_sep: str | list[str],
+        targets: str | list[str],
+        formatters: Optional[list[CmdArgFormatter | None]] = None,
+        checker: Optional["BotChecker"] = None,
+        priority: PriorLevel = PriorLevel.MEAN,
+        block: bool = False,
+        temp: bool = False,
+        session_rule: Optional["SessionRule"] = None,
+        session_hold: bool = False,
+        direct_rouse: bool = True,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
+    ):
+        """绑定一个消息事件处理方法
 
-        return make_args
+        .. admonition:: 注意
+           :class: caution
+
+           - 命令起始符和命令间隔符不允许包含：引号，各种括号，反斜杠，数字，英文，控制字符及各类空白字符。
+           - 命令起始符不能是命令间隔符的子序列，反之亦然。
+
+        :param cmd_start: 命令起始符（可以是字符串或字符串列表）
+        :param cmd_sep: 命令间隔符（可以是字符串或字符串列表）
+        :param targets: 匹配的命令名
+        :param formatters: 格式化器列表（列表可以包含空值，即此位置的参数无格式化）
+        :param checker: 使用的检查器，为空则默认通过检查
+        :param priority: 优先级
+        :param block: 是否进行优先级阻断
+        :param temp: 是否是一次性的
+        :param session_rule: 会话规则，为空则不使用会话规则
+        :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
+        :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
+        :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
+        :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
+        """
+        return self.on_message(
+            None,
+            CmdParser(cmd_start, cmd_sep, targets, formatters),
+            checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
     def on_start_match(
         self,
         target: str | list[str],
         logic_mode: LogicMode = LogicMode.OR,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个字符串起始匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次起始匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行起始匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
@@ -401,55 +437,41 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-        start_matcher = StartMatcher(target, logic_mode)
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        start_matcher,
-                        None,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self.on_message(
+            StartMatcher(target, logic_mode),
+            None,
+            checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
     def on_contain_match(
         self,
         target: str | list[str],
         logic_mode: LogicMode = LogicMode.OR,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个字符串包含匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次包含匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行包含匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
@@ -463,55 +485,41 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-        contain_matcher = ContainMatcher(target, logic_mode)
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        contain_matcher,
-                        None,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self.on_message(
+            ContainMatcher(target, logic_mode),
+            None,
+            checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
     def on_full_match(
         self,
         target: str | list[str],
         logic_mode: LogicMode = LogicMode.OR,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个字符串全匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次全匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行全匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
@@ -525,55 +533,41 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-        full_matcher = FullMatcher(target, logic_mode)
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        full_matcher,
-                        None,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self.on_message(
+            FullMatcher(target, logic_mode),
+            None,
+            checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
     def on_end_match(
         self,
         target: str | list[str],
         logic_mode: LogicMode = LogicMode.OR,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个字符串结尾匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次结尾匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行结尾匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
@@ -587,54 +581,40 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-        end_matcher = EndMatcher(target, logic_mode)
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        end_matcher,
-                        None,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self.on_message(
+            EndMatcher(target, logic_mode),
+            None,
+            checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
     def on_regex_match(
         self,
         target: str,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个字符串正则匹配的消息事件处理方法
 
         消息必须匹配成功才能被进一步处理。
 
         :param target: 匹配目标的正则表达式，在匹配时，它应该可以使 :meth:`re.findall` 不返回空列表
         :param checker: 使用的检查器，为空则默认通过检查
@@ -643,189 +623,145 @@
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-        regex_matcher = RegexMatcher(target)
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        regex_matcher,
-                        None,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self.on_message(
+            RegexMatcher(target),
+            None,
+            checker,
+            priority,
+            block,
+            temp,
+            session_rule,
+            session_hold,
+            direct_rouse,
+            conflict_wait,
+            conflict_cb,
+        )
 
     def on_request(
         self,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个请求事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=ReqEventHandler,
-                    params=[
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self._on_event(
+            ReqEventHandler,
+            params=[
+                checker,
+                priority,
+                block,
+                temp,
+                session_rule,
+                session_hold,
+                direct_rouse,
+                conflict_wait,
+                conflict_cb,
+            ],
+        )
 
     def on_notice(
         self,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个通知事件处理方法
 
         :param type: 通知的类型，为 "ALL" 时接受所有通知
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=NoticeEventHandler,
-                    params=[
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self._on_event(
+            NoticeEventHandler,
+            params=[
+                checker,
+                priority,
+                block,
+                temp,
+                session_rule,
+                session_hold,
+                direct_rouse,
+                conflict_wait,
+                conflict_cb,
+            ],
+        )
 
     def on_meta_event(
         self,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = True,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine]] = None,
+        conflict_wait: bool = True,
+        conflict_cb: Optional[AsyncCallable[[], None]] = None,
     ):
         """绑定一个元事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
         :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
         :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
         :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
         """
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MetaEventHandler,
-                    params=[
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
+        return self._on_event(
+            MetaEventHandler,
+            params=[
+                checker,
+                priority,
+                block,
+                temp,
+                session_rule,
+                session_hold,
+                direct_rouse,
+                conflict_wait,
+                conflict_cb,
+            ],
+        )
 
     def on_signal(self, signal: str, namespace: Optional[str] = None):
         """绑定一个信号处理方法
 
         `namespace` 为空时，自动设置它为当前插件的 :attr:`~.BotPlugin.ID`
 
         本方法作为异步函数的装饰器使用，此时可绑定一个函数为信号处理方法。
@@ -846,31 +782,31 @@
 
            在一个 bot 实例的范围内，同命名空间同名称的信号，只能绑定一个处理方法。
 
         :param namespace: 信号的命名空间
         :param signal: 信号的名称
         """
 
-        def make_args(
-            func: Callable[P, Coroutine[Any, Any, Any]]
-        ) -> Callable[P, Coroutine[Any, Any, Any]]:
+        def make_args(func: AsyncCallable[P, T]) -> AsyncCallable[P, T]:
             self.__signal_args__.append(
                 PluginSignalHandlerArgs(
-                    func, namespace if namespace is not None else self.ID, signal
+                    DependManager.inject(func),
+                    namespace if namespace is not None else self.ID,
+                    signal,
                 )
             )
             return func
 
         return make_args
 
     def on_share(
         self,
         id: str,
         namespace: Optional[str] = None,
-        reflector: Optional[Callable[[], Any]] = None,
+        reflector: Optional[Callable[P, Any]] = None,
     ):
         """注册一个共享对象，同时绑定它的值获取方法
 
         `namespace` 为空时，自动设置它为当前插件的 :attr:`~.BotPlugin.ID`
 
         本方法可作为异步函数的装饰器使用，此时被装饰函数就是共享对象的值获取方法：
 
@@ -899,22 +835,22 @@
         :param namespace: 共享对象的命名空间
         :param id: 共享对象的 id 标识
         :param reflector: 本方法当作异步函数的装饰器使用时，本参数为空；直接使用本方法时，参数为共享对象值获取的同步函数
         """
         _namespace = namespace if namespace is not None else self.ID
         if reflector is not None:
             self.__share_args__.append(
-                ShareObjArgs(_namespace, id, to_async(reflector))
+                ShareObjArgs(DependManager.inject(to_async(reflector)), _namespace, id)
             )
             return
 
-        def make_args(
-            func: Callable[[], Coroutine[Any, Any, Any]]
-        ) -> Callable[[], Coroutine[Any, Any, Any]]:
-            self.__share_args__.append(ShareObjArgs(_namespace, id, func))
+        def make_args(func: AsyncCallable[P, T]) -> AsyncCallable[P, T]:
+            self.__share_args__.append(
+                ShareObjArgs(DependManager.inject(func), _namespace, id)
+            )
             return func
 
         return make_args
 
     def on_share_affected(self, id: str, namespace: Optional[str] = None):
         """为一个共享对象绑定回调方法
 
@@ -940,20 +876,20 @@
            在一个 bot 实例的范围内，同命名空间同名称的共享对象，只能绑定一个回调方法。
            而且这个共享对象必须在本插件通过 :meth:`on_share` 注册（共享对象注册、共享对象回调绑定先后顺序不重要）
 
         :param namespace: 共享对象的命名空间
         :param id: 共享对象的 id 标识
         """
 
-        def make_args(
-            func: Callable[P, Coroutine[Any, Any, Any]]
-        ) -> Callable[P, Coroutine[Any, Any, Any]]:
+        def make_args(func: AsyncCallable[P, T]) -> AsyncCallable[P, T]:
             self.__share_cb_args__.append(
                 ShareObjCbArgs(
-                    namespace if namespace is not None else self.ID, id, func
+                    namespace if namespace is not None else self.ID,
+                    id,
+                    DependManager.inject(func),
                 )
             )
             return func
 
         return make_args
 
     def on_bot_life(self, *types: BotLife):
@@ -970,19 +906,19 @@
                # melobot 对被装饰函数的要求：无参数，返回空值
                await send_custom("Hello~", isPrivate=True, userId=xxxxx)
            # 在这个示例中，bot 登录上号后，便会向 xxxxx 发送一条 Hello~ 消息
 
         :param types: bot 生命周期类型枚举值，可传入多个
         """
 
-        def make_args(
-            func: Callable[P, Coroutine[Any, Any, None]]
-        ) -> Callable[P, Coroutine[Any, Any, None]]:
+        def make_args(func: AsyncCallable[P, None]) -> AsyncCallable[P, None]:
             for type in types:
-                self.__hook_args__.append(BotHookRunnerArgs(func, type))
+                self.__hook_args__.append(
+                    BotHookRunnerArgs(DependManager.inject(func), type)
+                )
             return func
 
         return make_args
 
     @property
     def on_plugins_loaded(self):
         """绑定 bot 在 :attr:`.BotLife.LOADED` 生命周期的 hook 方法
```

### Comparing `melobot-2.6.2/src/melobot/plugin/ipc.py` & `melobot-2.6.3/src/melobot/plugin/ipc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,154 @@
 import asyncio
 
-from ..base.abc import BaseLogger
 from ..base.exceptions import BotIpcError
 from ..base.tools import RWController
-from ..base.typing import Any, Callable, Coroutine
-from ..utils.logger import log_exc
+from ..base.typing import TYPE_CHECKING, Any, AsyncCallable
+
+if TYPE_CHECKING:
+    from ..utils.logger import BotLogger
 
 
 class ShareObject:
     """共享对象"""
 
     def __init__(self, namespace: str, id: str) -> None:
         self.namespace = namespace
         self.id = id
         self.__rwc = RWController()
-        self.__reflect: Callable[[], Coroutine[Any, Any, Any]]
-        self.__callback: Callable[..., Coroutine[Any, Any, Any]]
+        self.__reflect: AsyncCallable[..., Any]
+        self.__callback: AsyncCallable[..., Any]
 
         self.__cb_set = asyncio.Event()
 
-    def _fill_ref(self, reflector: Callable[[], Coroutine[Any, Any, Any]]) -> None:
+    def _fill_ref(self, reflector: AsyncCallable[..., Any]) -> None:
         self.__reflect = reflector
 
-    def _fill_cb(self, callback: Callable[..., Coroutine[Any, Any, Any]]) -> None:
+    def _fill_cb(self, callback: AsyncCallable[..., Any]) -> None:
         self.__callback = callback
         self.__cb_set.set()
 
     @property
     async def val(self) -> Any:
         """共享对象引用的值"""
         async with self.__rwc.safe_read():
             return await self.__reflect()
 
     async def affect(self, *args: Any, **kwargs: Any) -> Any:
         """触发共享对象的回调，回调未设置时会等待。 如果本来就没有回调，则会陷入无休止等待"""
         await self.__cb_set.wait()
+
         async with self.__rwc.safe_write():
             return await self.__callback(*args, **kwargs)
 
 
 class PluginStore:
     """插件共享存储"""
 
     def __init__(self) -> None:
         self.store: dict[str, dict[str, ShareObject]] = {}
 
     def create_so(
-        self, reflector: Callable[[], Coroutine[Any, Any, Any]], namespace: str, id: str
+        self, reflector: AsyncCallable[..., Any], namespace: str, id: str
     ) -> None:
         """创建共享对象"""
-        if namespace not in self.store.keys():
-            self.store[namespace] = {}
+        self.store.setdefault(namespace, {})
         obj = self.store[namespace].get(id)
         if obj is not None:
             raise BotIpcError(
                 f"已在 {namespace} 命名空间中注册标记为 {id} 的共享对象，拒绝再次注册"
             )
+
         obj = ShareObject(namespace, id)
         self.store[namespace][id] = obj
         obj._fill_ref(reflector)
 
-    def bind_cb(
-        self, namespace: str, id: str, cb: Callable[..., Coroutine[Any, Any, Any]]
-    ) -> None:
+    def bind_cb(self, namespace: str, id: str, cb: AsyncCallable[..., Any]) -> None:
         """为共享对象绑定回调"""
         if namespace not in self.store.keys():
             raise BotIpcError(f"共享对象回调指定的命名空间 {namespace} 不存在")
+
         if id not in self.store[namespace].keys():
             raise BotIpcError(
                 f"共享对象回调指定的命名空间中，不存在标记为 {id} 的共享对象"
             )
+
         if self.store[namespace][id].__cb_set.is_set():
             raise BotIpcError(
                 f"{namespace} 中标记为 {id} 的共享对象已被绑定过回调，拒绝再次绑定"
             )
+
         self.store[namespace][id]._fill_cb(cb)
 
     def get(self, namespace: str, id: str) -> ShareObject:
         """获取共享对象"""
         if namespace not in self.store.keys():
             raise BotIpcError(f"无法获取不存在的共享对象：命名空间 {namespace} 不存在")
         if id not in self.store[namespace].keys():
             raise BotIpcError(f"无法获取不存在的共享对象：标识 {id} 不存在")
+
         return self.store[namespace][id]
 
 
 class PluginSignalHandler:
     """插件信号处理器"""
 
     def __init__(
-        self, namespace: str, signal: str, func: Callable[..., Coroutine[Any, Any, Any]]
+        self, namespace: str, signal: str, func: AsyncCallable[..., Any]
     ) -> None:
         self.cb = func
         self.namespace = namespace
         self.signal = signal
 
 
 class PluginBus:
     """插件信号总线"""
 
     def __init__(self) -> None:
         self.store: dict[str, dict[str, PluginSignalHandler]] = {}
-        self.logger: BaseLogger
+        self.logger: "BotLogger"
 
-    def _bind(self, logger: BaseLogger) -> None:
+    def _bind(self, logger: "BotLogger") -> None:
         self.logger = logger
 
     def register(
-        self, namespace: str, signal: str, func: Callable[..., Coroutine[Any, Any, Any]]
+        self, namespace: str, signal: str, func: AsyncCallable[..., Any]
     ) -> None:
         """绑定一个插件信号处理方法。由 plugin build 过程调用"""
-        if namespace not in self.store.keys():
-            self.store[namespace] = {}
+        self.store.setdefault(namespace, {})
         if signal in self.store[namespace].keys():
             raise BotIpcError("同一命名空间的同一信号只能绑定一个处理函数")
+
         self.store[namespace][signal] = PluginSignalHandler(namespace, signal, func)
 
     async def _run_on_ctx(
         self, handler: PluginSignalHandler, *args: Any, **kwargs: Any
     ) -> Any:
         """在指定的上下文下运行插件信号处理方法"""
         try:
             ret = await handler.cb(*args, **kwargs)
             return ret
         except Exception as e:
             func_name = handler.cb.__qualname__
             self.logger.error(f"插件信号处理方法 {func_name} 发生异常")
-            log_exc(self.logger, locals(), e)
+            self.logger.exc(locals=locals())
 
     async def emit(
         self, namespace: str, signal: str, *args: Any, wait: bool = False, **kwargs: Any
     ) -> Any:
-        """触发一个插件信号。如果指定 wait 为 True，则会等待所有插件信号处理方法完成。 若启用 forward，则会将 session
+        """触发一个插件信号。如果指定 wait 为 True，则会等待所有插件信号处理方法完成。 若启用 forward，则会将 会话
         从信号触发处转发到信号处理处。 但启用 forward，必须同时启用 wait。
 
         注意：如果你要等待返回结果，则需要指定 wait=True，否则不会等待且始终返回 None
         """
         if namespace not in self.store.keys():
             raise BotIpcError(f"插件信号命名空间 {namespace} 不存在，无法触发信号")
         if signal not in self.store[namespace].keys():
-            self.logger.warning(
-                f"命名空间 {namespace} 内，没有处理信号 {signal} 的处理函数"
-            )
-            return
+            raise BotIpcError(f"命名空间 {namespace} 内没有信号 {signal} 的处理函数")
 
         handler = self.store[namespace][signal]
+        task = self._run_on_ctx(handler, *args, **kwargs)
         if not wait:
-            asyncio.create_task(self._run_on_ctx(handler, *args, **kwargs))
+            asyncio.create_task(task)
             return None
         else:
-            return await self._run_on_ctx(handler, *args, **kwargs)
+            return await task
```

### Comparing `melobot-2.6.2/src/melobot/utils/__init__.py` & `melobot-2.6.3/src/melobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/src/melobot/utils/checker.py` & `melobot-2.6.3/src/melobot/utils/checker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,9 @@
 from ..base.abc import BotChecker, BotEvent
-from ..base.exceptions import BotValueError
-from ..base.tools import is_retcoro
-from ..base.typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Coroutine,
-    Literal,
-    Optional,
-    User,
-    cast,
-)
+from ..base.typing import TYPE_CHECKING, AsyncCallable, Callable, Optional, User, cast
 
 if TYPE_CHECKING:
     from ..models.event import MessageEvent, NoticeEvent, RequestEvent
 
 
 class MsgChecker(BotChecker):
     """初始化一个消息事件通用检查器"""
@@ -40,16 +29,16 @@
     def __init__(
         self,
         level: User,
         owner: Optional[int] = None,
         super_users: Optional[list[int]] = None,
         white_users: Optional[list[int]] = None,
         black_users: Optional[list[int]] = None,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         """初始化一个消息事件分级权限检查器
 
         :param level: 允许的等级（>= 此等级才能通过校验）
         :param owner: 主人的 qq 号
         :param super_users: 超级用户 qq 号列表
         :param white_users: 白名单用户 qq 号列表
@@ -58,23 +47,14 @@
         :param fail_cb: 检查不通过的回调
         """
         super().__init__()
         self.ok_cb = ok_cb
         self.fail_cb = fail_cb
         self.check_lvl = level
 
-        if ok_cb is not None and not is_retcoro(ok_cb):
-            raise BotValueError(
-                f"检查器成功回调 {ok_cb.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        if fail_cb is not None and not is_retcoro(fail_cb):
-            raise BotValueError(
-                f"检查器失败回调 {fail_cb.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-
         self.owner = owner
         self.su_list = super_users if super_users is not None else []
         self.white_list = white_users if white_users is not None else []
         self.black_list = black_users if black_users is not None else []
 
     def _get_level(self, event: "MessageEvent") -> User:
         """获得事件对应的登记"""
@@ -91,16 +71,18 @@
         else:
             return User.USER
 
     async def check(self, event: BotEvent) -> bool:
         event = cast("MessageEvent", event)
         if not event.is_msg_event():
             return False
+
         e_level = self._get_level(event)
         status = 0 < e_level.value and e_level.value >= self.check_lvl.value
+
         if status and self.ok_cb is not None:
             await self.ok_cb()
         if not status and self.fail_cb is not None:
             await self.fail_cb()
         return status
 
 
@@ -117,16 +99,16 @@
         self,
         level: User,
         owner: Optional[int] = None,
         super_users: Optional[list[int]] = None,
         white_users: Optional[list[int]] = None,
         black_users: Optional[list[int]] = None,
         white_groups: Optional[list[int]] = None,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         """初始化一个群聊消息事件分级权限检查器
 
         :param level: 允许的等级（>= 此等级才能通过校验）
         :param owner: 主人的 qq 号
         :param super_users: 超级用户 qq 号列表
         :param white_users: 白名单用户 qq 号列表
@@ -140,20 +122,22 @@
         )
         self.white_group_list = white_groups if white_groups is not None else []
 
     async def check(self, event: BotEvent) -> bool:
         event = cast("MessageEvent", event)
         if not event.is_msg_event():
             return False
+
         if (
             not event.is_group()
             or len(self.white_group_list) == 0
             or (event.group_id not in self.white_group_list)
         ):
             return False
+
         return await super().check(event)
 
 
 class PrivateMsgLvlChecker(MsgLvlChecker):
     """私聊消息事件分级权限检查器
 
     基本功能与 :class:`MsgLvlChecker` 一致。
@@ -164,16 +148,16 @@
     def __init__(
         self,
         level: User,
         owner: Optional[int] = None,
         super_users: Optional[list[int]] = None,
         white_users: Optional[list[int]] = None,
         black_users: Optional[list[int]] = None,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         """初始化一个私聊消息事件分级权限检查器
 
         :param level: 允许的等级（>= 此等级才能通过校验）
         :param owner: 主人的 qq 号
         :param super_users: 超级用户 qq 号列表
         :param white_users: 白名单用户 qq 号列表
@@ -187,14 +171,15 @@
 
     async def check(self, event: BotEvent) -> bool:
         event = cast("MessageEvent", event)
         if not event.is_msg_event():
             return False
         if not event.is_private():
             return False
+
         return await super().check(event)
 
 
 class MsgCheckerFactory:
     """消息事件分级权限检查器的工厂
 
     预先存储检查依据（各等级数据），指定检查等级后，可返回一个 :class:`MsgLvlChecker` 类的对象
@@ -203,16 +188,16 @@
     def __init__(
         self,
         owner: Optional[int] = None,
         super_users: Optional[list[int]] = None,
         white_users: Optional[list[int]] = None,
         black_users: Optional[list[int]] = None,
         white_groups: Optional[list[int]] = None,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> None:
         """初始化一个消息事件分级权限检查器的工厂
 
         :param owner: 主人的 qq 号
         :param super_users: 超级用户 qq 号列表
         :param white_users: 白名单用户 qq 号列表
         :param black_users: 黑名单用户 qq 号列表
@@ -222,45 +207,45 @@
         """
         self.owner = owner
         self.su_list = super_users if super_users is not None else []
         self.white_list = white_users if white_users is not None else []
         self.black_list = black_users if black_users is not None else []
         self.white_group_list = white_groups if white_groups is not None else []
 
-        self.united_ok_cb = ok_cb
-        self.united_fail_cb = fail_cb
+        self.ok_cb = ok_cb
+        self.fail_cb = fail_cb
 
     def get_base(
         self,
         level: User = User.USER,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> MsgLvlChecker:
         """根据内部依据和给定等级，生成一个 :class:`MsgLvlChecker` 对象
 
         :param level: 允许的等级（>= 此等级才能通过校验）
         :param ok_cb: 检查通过的回调（比实例化本类传入的参数优先级更高）
         :param fail_cb: 检查不通过的回调（比实例化本类传入的参数优先级更高）
         :return: 消息事件分级权限检查器
         """
         return MsgLvlChecker(
             level,
             self.owner,
             self.su_list,
             self.white_list,
             self.black_list,
-            self.united_ok_cb if ok_cb is None else ok_cb,
-            self.united_fail_cb if fail_cb is None else fail_cb,
+            self.ok_cb if ok_cb is None else ok_cb,
+            self.fail_cb if fail_cb is None else fail_cb,
         )
 
     def get_group(
         self,
         level: User = User.USER,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> GroupMsgLvlChecker:
         """根据内部依据和给定等级，生成一个 :class:`GroupMsgLvlChecker` 对象
 
         :param level: 允许的等级（>= 此等级才能通过校验）
         :param ok_cb: 检查通过的回调（比实例化本类传入的参数优先级更高）
         :param fail_cb: 检查不通过的回调（比实例化本类传入的参数优先级更高）
         :return: 群聊消息事件分级权限检查器
@@ -268,39 +253,39 @@
         return GroupMsgLvlChecker(
             level,
             self.owner,
             self.su_list,
             self.white_list,
             self.black_list,
             self.white_group_list,
-            self.united_ok_cb if ok_cb is None else ok_cb,
-            self.united_fail_cb if fail_cb is None else fail_cb,
+            self.ok_cb if ok_cb is None else ok_cb,
+            self.fail_cb if fail_cb is None else fail_cb,
         )
 
     def get_private(
         self,
         level: User = User.USER,
-        ok_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-        fail_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
+        ok_cb: Optional[AsyncCallable[[], None]] = None,
+        fail_cb: Optional[AsyncCallable[[], None]] = None,
     ) -> PrivateMsgLvlChecker:
         """根据内部依据和给定等级，生成一个 :class:`PrivateMsgLvlChecker` 对象
 
         :param level: 允许的等级（>= 此等级才能通过校验）
         :param ok_cb: 检查通过的回调（比实例化本类传入的参数优先级更高）
         :param fail_cb: 检查不通过的回调（比实例化本类传入的参数优先级更高）
         :return: 私聊消息事件分级权限检查器
         """
         return PrivateMsgLvlChecker(
             level,
             self.owner,
             self.su_list,
             self.white_list,
             self.black_list,
-            self.united_ok_cb if ok_cb is None else ok_cb,
-            self.united_fail_cb if fail_cb is None else fail_cb,
+            self.ok_cb if ok_cb is None else ok_cb,
+            self.fail_cb if fail_cb is None else fail_cb,
         )
 
 
 class AtMsgChecker(BotChecker):
     """艾特消息事件检查器"""
 
     def __init__(self, qid: Optional[int] = None) -> None:
@@ -311,25 +296,20 @@
         super().__init__()
         self.qid = qid
 
     async def check(self, event: BotEvent) -> bool:
         event = cast("MessageEvent", event)
         if not event.is_msg_event():
             return False
+
         qids = event.get_datas("at", "qq")
         if self.qid is None:
-            status = len(qids) > 0
+            return len(qids) > 0
         else:
-            for id in qids:
-                if id == self.qid:
-                    status = True
-                    break
-            else:
-                status = False
-        return status
+            return any(id == self.qid for id in qids)
 
 
 class ReqChecker(BotChecker):
     """请求事件通用检查器"""
 
     def __init__(self, check_func: Callable[["RequestEvent"], bool]) -> None:
         """初始化一个请求事件通用检查器
```

### Comparing `melobot-2.6.2/src/melobot/utils/matcher.py` & `melobot-2.6.3/src/melobot/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.2/src/melobot/utils/parser.py` & `melobot-2.6.3/src/melobot/utils/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import re
-import traceback
 from functools import lru_cache
 
 from ..base.abc import BotParser
 from ..base.exceptions import BotException, BotValueError
-from ..base.tools import is_retcoro
 from ..base.typing import (
     Any,
+    AsyncCallable,
     Callable,
-    Coroutine,
     Iterator,
-    ModuleType,
     Optional,
     ParseArgs,
+    TracebackType,
     Void,
     VoidType,
     cast,
 )
 from ..context.action import send
 
 
@@ -44,15 +42,15 @@
     def __init__(
         self,
         src: str | VoidType,
         src_desc: Optional[str],
         src_expect: Optional[str],
         idx: int,
         exc: Exception,
-        exc_tb: ModuleType,
+        exc_tb: Optional[TracebackType],
         group_id: str,
     ) -> None:
         #: 命令参数格式化前的原值
         self.src = src
         #: 命令参数值的功能描述
         self.src_desc = src_desc
         #: 命令参数值的值期待描述
@@ -77,19 +75,17 @@
         self,
         convert: Optional[Callable[[str], Any]] = None,
         verify: Optional[Callable[[Any], bool]] = None,
         src_desc: Optional[str] = None,
         src_expect: Optional[str] = None,
         default: Any = Void,
         default_replace_flag: Optional[str] = None,
-        convert_fail: Optional[
-            Callable[[FormatInfo], Coroutine[Any, Any, None]]
-        ] = None,
-        verify_fail: Optional[Callable[[FormatInfo], Coroutine[Any, Any, None]]] = None,
-        arg_lack: Optional[Callable[[FormatInfo], Coroutine[Any, Any, None]]] = None,
+        convert_fail: Optional[AsyncCallable[[FormatInfo], None]] = None,
+        verify_fail: Optional[AsyncCallable[[FormatInfo], None]] = None,
+        arg_lack: Optional[AsyncCallable[[FormatInfo], None]] = None,
     ) -> None:
         """初始化一个命令参数格式化器
 
         :param convert: 类型转换方法，为空则不进行类型转换
         :param verify: 值验证方法，为空则不对值进行验证
         :param src_desc: 命令参数值的功能描述
         :param src_expect: 命令参数值的值期待描述
@@ -99,163 +95,156 @@
         :param verify_fail: 值验证失败的回调，为空则使用默认回调
         :param arg_lack: 参数缺失的回调，为空则使用默认回调
         """
         self.convert = convert
         self.verify = verify
         self.src_desc = src_desc
         self.src_expect = src_expect
+
         self.default = default
         self.default_replace_flag = default_replace_flag
         if self.default is Void and self.default_replace_flag is not None:
             raise BotValueError(
                 "初始化参数格式化器时，使用“默认值替换标记”必须同时设置默认值"
             )
-        if convert_fail is not None and not is_retcoro(convert_fail):
-            raise BotValueError(
-                f"格式化器的类型转换失败回调 {convert_fail.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        if verify_fail is not None and not is_retcoro(verify_fail):
-            raise BotValueError(
-                f"格式化器的值验证失败回调 {verify_fail.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
-        if arg_lack is not None and not is_retcoro(arg_lack):
-            raise BotValueError(
-                f"格式化器的参数缺失回调 {arg_lack.__qualname__} 必须为异步函数，或其他返回协程的可调用对象"
-            )
 
         self.convert_fail = convert_fail
         self.verify_fail = verify_fail
         self.arg_lack = arg_lack
 
     def _get_val(self, args: ParseArgs, idx: int) -> Any:
         if self.default is Void:
             if len(args.vals) < idx + 1:
                 raise ArgLackError
             else:
                 return args.vals[idx]
+
         elif len(args.vals) < idx + 1:
             args.vals.append(self.default)
+
         return args.vals[idx]
 
     async def format(
         self,
         group_id: str,
         args: ParseArgs,
         idx: int,
     ) -> bool:
         # 格式化参数为对应类型的变量
         try:
             src = self._get_val(args, idx)
-            if (
-                self.default_replace_flag is not None
-                and src == self.default_replace_flag
-            ):
+            if self.default_replace_flag is not None and src == self.default_replace_flag:
                 src = self.default
             res = self.convert(src) if self.convert is not None else src
 
-            if self.verify is None:
-                pass
-            elif self.verify(res):
+            if self.verify is None or self.verify(res):
                 pass
             else:
                 raise ArgVerifyFailed
             args.vals[idx] = res
             return True
+
         except ArgVerifyFailed as e:
             info = FormatInfo(
-                src, self.src_desc, self.src_expect, idx, e, traceback, group_id
+                src, self.src_desc, self.src_expect, idx, e, e.__traceback__, group_id
             )
             if self.verify_fail:
                 await self.verify_fail(info)
             else:
                 await self._verify_fail_default(info)
             return False
+
         except ArgLackError as e:
             info = FormatInfo(
-                Void, self.src_desc, self.src_expect, idx, e, traceback, group_id
+                Void, self.src_desc, self.src_expect, idx, e, e.__traceback__, group_id
             )
             if self.arg_lack:
                 await self.arg_lack(info)
             else:
                 await self._arglack_default(info)
             return False
+
         except Exception as e:
             info = FormatInfo(
-                src, self.src_desc, self.src_expect, idx, e, traceback, group_id
+                src, self.src_desc, self.src_expect, idx, e, e.__traceback__, group_id
             )
             if self.convert_fail:
                 await self.convert_fail(info)
             else:
                 await self._convert_fail_default(info)
             return False
 
     async def _convert_fail_default(self, info: FormatInfo) -> None:
-        e_class = info.exc.__class__.__name__
+        e_class = info.exc.__class__.__qualname__
         src = info.src.__repr__() if isinstance(info.src, str) else info.src
-        tip = f"第 {info.idx+1} 个参数"
+
+        tip = f"第 {info.idx + 1} 个参数"
         tip += (
             f"（{info.src_desc}）无法处理，给定的值为：{src}。"
             if info.src_desc
             else f"给定的值 {src} 无法处理。"
         )
+
         tip += f"参数要求：{info.src_expect}。" if info.src_expect else ""
         tip += f"\n详细错误描述：[{e_class}] {info.exc}"
         tip = f"命令 {info.group_id} 参数格式化失败：\n{tip}"
+
         await send(tip)
 
     async def _verify_fail_default(self, info: FormatInfo) -> None:
         src = info.src.__repr__() if isinstance(info.src, str) else info.src
-        tip = f"第 {info.idx+1} 个参数"
+
+        tip = f"第 {info.idx + 1} 个参数"
         tip += (
             f"（{info.src_desc}）不符合要求，给定的值为：{src}。"
             if info.src_desc
             else f"给定的值 {src} 不符合要求。"
         )
+
         tip += f"参数要求：{info.src_expect}。" if info.src_expect else ""
         tip = f"命令 {info.group_id} 参数格式化失败：\n{tip}"
+
         await send(tip)
 
     async def _arglack_default(self, info: FormatInfo) -> None:
-        tip = f"第 {info.idx+1} 个参数"
+        tip = f"第 {info.idx + 1} 个参数"
         tip += f"（{info.src_desc}）缺失。" if info.src_desc else "缺失。"
         tip += f"参数要求：{info.src_expect}。" if info.src_expect else ""
         tip = f"命令 {info.group_id} 参数格式化失败：\n{tip}"
+
         await send(tip)
 
 
 @lru_cache(maxsize=128)
 def cmd_parse(
     text: str,
     start_regex: re.Pattern[str],
     sep_regex: re.Pattern[str],
     rm_empty: bool = True,
 ) -> dict[str, list[str]]:
 
-    def split_string(
-        string: str, regex: re.Pattern, popFirst: bool = True
-    ) -> Iterator[str]:
-        # 将复杂的各种分隔符替换为 特殊字符，方便分割
+    def _split(string: str, regex: re.Pattern, popFirst: bool = True) -> Iterator[str]:
         temp_string = regex.sub("\u0000", string)
         temp_list = re.split("\u0000", temp_string)
         if popFirst:
             temp_list.pop(0)
         return filter(lambda x: x != "", temp_list)
 
     pure_string = text.strip() if rm_empty else text
-    cmd_seqs = [
-        list(split_string(s, sep_regex, False))
-        for s in split_string(pure_string, start_regex)
-    ]
-    cmd_seqs_iter = filter(lambda x: len(x) > 0, cmd_seqs)
+    cmd_seqs = (
+        list(_split(s, sep_regex, False)) for s in _split(pure_string, start_regex)
+    )
+    seqs_filter = filter(lambda x: len(x) > 0, cmd_seqs)
 
     cmd_dict: dict[str, list[str]] = {}
-    for seq in cmd_seqs_iter:
+    for seq in seqs_filter:
         if len(seq) == 0:
             continue
         cmd_dict[seq[0]] = seq[1:]
+
     return cmd_dict
 
 
 class CmdParser(BotParser):
     """命令解析器
 
     通过解析命令名和命令参数的形式，解析字符串。
@@ -279,65 +268,64 @@
         :param cmd_start: 命令起始符（可以是字符串或字符串列表）
         :param cmd_sep: 命令间隔符（可以是字符串或字符串列表）
         :param targets: 匹配的命令名
         :param formatters: 格式化器列表（列表可以包含空值，即此位置的参数无格式化）
         """
         self.targets = targets if isinstance(targets, list) else [targets]
         self.formatters = formatters
-        self.need_format = True if self.formatters is not None else False
 
         self.start_tokens = cmd_start if isinstance(cmd_start, list) else [cmd_start]
         self.sep_tokens = cmd_sep if isinstance(cmd_sep, list) else [cmd_sep]
         self.ban_regex = re.compile(r"[\'\"\\\(\)\[\]\{\}\r\n\ta-zA-Z0-9]")
-        self._build_parse_regex()
+
+        self.cmd_start: list[str]
+        self.cmd_sep: list[str]
+        self.start_regex: re.Pattern[str]
+        self.sep_regex: re.Pattern[str]
 
         if self.ban_regex.findall(f"{''.join(cmd_start)}{''.join(cmd_sep)}"):
             raise BotValueError("存在命令解析器不支持的命令起始符，或命令间隔符")
 
+        self._build_parse_regex()
+
     def _build_parse_regex(self):
         """建立用于命令解析的正则 Pattern 对象，包含命令起始符正则 pattern 和 命令间隔符正则 pattern"""
-        temp_regex = re.compile(
+        _regex = re.compile(
             r"([\`\-\=\~\!\@\#\$\%\^\&\*\(\)\_\+\[\]\{\}\|\:\,\.\/\<\>\?])"
         )
+
         if not len(set(self.sep_tokens) & set(self.start_tokens)):
-            self.cmd_sep = [
-                temp_regex.sub(r"\\\1", sep_token) for sep_token in self.sep_tokens
-            ]
-            self.cmd_start = [
-                temp_regex.sub(r"\\\1", start_token)
-                for start_token in self.start_tokens
-            ]
-            self.sep_parse_regex = re.compile(rf"{'|'.join(self.cmd_sep)}")
-            self.start_parse_regex = re.compile(rf"{'|'.join(self.cmd_start)}")
+            self.cmd_sep = [_regex.sub(r"\\\1", token) for token in self.sep_tokens]
+            self.cmd_start = [_regex.sub(r"\\\1", token) for token in self.start_tokens]
+            self.sep_regex = re.compile(rf"{'|'.join(self.cmd_sep)}")
+            self.start_regex = re.compile(rf"{'|'.join(self.cmd_start)}")
         else:
             raise BotValueError("命令解析器起始符不能和间隔符重合")
 
     async def parse(self, text: str) -> Optional[ParseArgs]:
-        cmd_dict = cmd_parse(text, self.start_parse_regex, self.sep_parse_regex)
-        args_dict = {
-            cmd_name: ParseArgs(arg_vals) for cmd_name, arg_vals in cmd_dict.items()
-        }
+        cmd_dict = cmd_parse(text, self.start_regex, self.sep_regex)
+        args_dict = {cmd_name: ParseArgs(vals) for cmd_name, vals in cmd_dict.items()}
 
         for group_id in self.targets:
             args = args_dict.get(group_id)
             if args is not None:
                 break
         else:
             return None
 
-        if not self.need_format:
+        if self.formatters is None:
             return args
-        self.formatters = cast(list[Optional[CmdArgFormatter]], self.formatters)
+
         for idx, fmt in enumerate(self.formatters):
             if fmt is None:
                 continue
             status = await fmt.format(group_id, args, idx)
             if not status:
                 return None
-        args.vals = cast(list[Any], args.vals)
+
         args.vals = args.vals[: len(self.formatters)]
         return args
 
 
 class CmdParserFactory:
     """命令解析器的工厂
```

### Comparing `melobot-2.6.2/PKG-INFO` & `melobot-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melobot
-Version: 2.6.2
+Version: 2.6.3
 Summary: A bot framework with session control and plugin-supported.
 Keywords: qq,qq bot,onebot,bot framework,asyncio,coroutine,concurrency
 Author-Email: aicorein <melodyecho@glowmem.com>
 Maintainer-Email: aicorein <melodyecho@glowmem.com>
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: melobot Version: 2.6.2 Summary: A bot framework
+Metadata-Version: 2.1 Name: melobot Version: 2.6.3 Summary: A bot framework
 with session control and plugin-supported. Keywords: qq,qq bot,onebot,bot
 framework,asyncio,coroutine,concurrency Author-Email: aicorein
 glowmem.com> Maintainer-Email: aicorein
 glowmem.com> License: BSD Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

