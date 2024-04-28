# Comparing `tmp/croning-0.0.1.tar.gz` & `tmp/croning-0.1.0.tar.gz`

## Comparing `croning-0.0.1.tar` & `croning-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 croning-0.0.1/requirements.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 croning-0.0.1/src/croning/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 croning-0.0.1/src/croning/exceptions.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 croning-0.0.1/src/croning/schedule.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 croning-0.0.1/src/croning/scheduler.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 croning-0.0.1/src/croning/singleton.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 croning-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 croning-0.0.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 croning-0.0.1/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 croning-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 croning-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 croning-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 croning-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 croning-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 croning-0.1.0/src/croning/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 croning-0.1.0/src/croning/exceptions.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 croning-0.1.0/src/croning/schedule.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 croning-0.1.0/src/croning/scheduler.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 croning-0.1.0/src/croning/singleton.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 croning-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 croning-0.1.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 croning-0.1.0/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 croning-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 croning-0.1.0/PKG-INFO
```

### Comparing `croning-0.0.1/src/croning/schedule.py` & `croning-0.1.0/src/croning/schedule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Callable, Any
 from .scheduler import Scheduler
 
 
-def schedule_function(cron_format: str, identificator: str | None = None):
+def schedule_function(
+    cron_format: str | Callable[[], str], identificator: str | None = None
+):
 
     def register(function: Callable[[], Any]):
 
         function_identificator: str = (
             function.__name__ if identificator is None else identificator
         )
         Scheduler().register_function(
```

### Comparing `croning-0.0.1/src/croning/scheduler.py` & `croning-0.1.0/src/croning/scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,40 +6,46 @@
 from datetime import datetime
 
 
 class Scheduler(metaclass=Singleton):
 
     def __init__(self) -> None:
         self.__function_callback: dict[str, Callable] = {}
-        self.__cron_formats: dict[str, str] = {}
+        self.__cron_formats: dict[str, str | Callable[[], str]] = {}
         self.__current_zone_info: ZoneInfo | None = None
         self.__last_execution: dict[str, datetime] = {}
 
     @property
     def zone_info(self) -> ZoneInfo | None:
         return self.__current_zone_info
 
     @property
     def now(self) -> datetime:
         return datetime.now(tz=self.zone_info)
 
     def register_function(
-        self, function: Callable[[], Any], cron_format: str, identificator: str
+        self,
+        function: Callable[[], Any],
+        cron_format: str | Callable[[], str],
+        identificator: str,
     ):
         if identificator in self.__function_callback.keys():
             raise FunctionAlreadyRegistered(function_identificator=identificator)
 
         self.__function_callback[identificator] = function
         self.__cron_formats[identificator] = cron_format
         self.__last_execution[identificator] = self.now
 
     def get_cron(self, identificator: str) -> croniter:
 
+        cron_format = self.__cron_formats[identificator]
+        cron_format_parsed = cron_format() if callable(cron_format) else cron_format
+
         return croniter(
-            self.__cron_formats[identificator],
+            cron_format_parsed,
             ret_type=datetime,
             start_time=self.__last_execution[identificator],
         )
 
     def next_execution(self, identificator: str) -> datetime:
 
         return self.get_cron(identificator=identificator).next()
```

### Comparing `croning-0.0.1/.gitignore` & `croning-0.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+no_load*
```

### Comparing `croning-0.0.1/LICENSE` & `croning-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `croning-0.0.1/pyproject.toml` & `croning-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "croning"
-version = "0.0.1"
+version = "0.1.0"
 dependencies = ["croniter==2.0.5"]
 requires-python = ">=3.8"
 authors = [{ name = "Pedro García", email = "pedroluisgarciamontil@gmail.com" }]
 maintainers = [
     { name = "Pedro García", email = "pedroluisgarciamontil@gmail.com" },
 ]
 description = "Cron-style scheduling library."
```

### Comparing `croning-0.0.1/PKG-INFO` & `croning-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: croning
-Version: 0.0.1
+Version: 0.1.0
 Summary: Cron-style scheduling library.
 Project-URL: Repository, https://github.com/me/spam.git
 Author-email: Pedro García <pedroluisgarciamontil@gmail.com>
 Maintainer-email: Pedro García <pedroluisgarciamontil@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Pedro García
```

