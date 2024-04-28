# Comparing `tmp/clovers_apscheduler-0.1.3.tar.gz` & `tmp/clovers_apscheduler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_apscheduler-0.1.3.tar", max compression
+gzip compressed data, was "clovers_apscheduler-0.1.4.tar", max compression
```

## Comparing `clovers_apscheduler-0.1.3.tar` & `clovers_apscheduler-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      686 2024-04-16 00:19:30.661186 clovers_apscheduler-0.1.3/clovers_apscheduler/__init__.py
--rw-r--r--   0        0        0      134 2024-04-16 00:11:50.723949 clovers_apscheduler-0.1.3/clovers_apscheduler/config.py
--rw-r--r--   0        0        0     1086 2024-04-15 06:57:05.229105 clovers_apscheduler-0.1.3/LICENSE
--rw-r--r--   0        0        0      353 2024-04-16 00:29:47.208872 clovers_apscheduler-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1203 2024-04-15 11:31:19.355372 clovers_apscheduler-0.1.3/README.md
--rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 clovers_apscheduler-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      666 2024-04-28 09:17:39.741706 clovers_apscheduler-0.1.4/clovers_apscheduler/__init__.py
+-rw-r--r--   0        0        0      134 2024-04-28 09:13:38.750565 clovers_apscheduler-0.1.4/clovers_apscheduler/config.py
+-rw-r--r--   0        0        0     1086 2024-04-28 09:13:38.749565 clovers_apscheduler-0.1.4/LICENSE
+-rw-r--r--   0        0        0      353 2024-04-28 09:16:31.589704 clovers_apscheduler-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1189 2024-04-28 09:19:52.455010 clovers_apscheduler-0.1.4/README.md
+-rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 clovers_apscheduler-0.1.4/PKG-INFO
```

### Comparing `clovers_apscheduler-0.1.3/clovers_apscheduler/__init__.py` & `clovers_apscheduler-0.1.4/clovers_apscheduler/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 plugin = Plugin()
 scheduler = AsyncIOScheduler()
 scheduler.configure(**config_data.scheduler_config)
 
 
 @plugin.startup
 async def _():
-    if scheduler.running:
-        return
-    scheduler.start()
+    if not scheduler.running:
+        scheduler.start()
 
 
 @plugin.shutdown
 async def _():
     if scheduler.running:
-        return
-    scheduler.shutdown()
+        scheduler.shutdown()
 
 
 __plugin__ = plugin
```

### Comparing `clovers_apscheduler-0.1.3/LICENSE` & `clovers_apscheduler-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_apscheduler-0.1.3/README.md` & `clovers_apscheduler-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-# clovers_apscheduler
+<div align="center">
+
+# clovers-apscheduler
 
 _✨ clovers APScheduler 定时任务插件 ✨_
 
-<div align="center">
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
-<a href="./LICENSE">
-  <img src="https://img.shields.io/github/license/KarisAya/clovers_apscheduler.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_apscheduler">
-  <img src="https://img.shields.io/pypi/v/clovers_apscheduler.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_apscheduler">
-  <img src="https://img.shields.io/pypi/dm/clovers_apscheduler" alt="pypi download">
-</a>
+<a href="./LICENSE"><img src="https://img.shields.io/github/license/KarisAya/clovers_apscheduler.svg" alt="license"></a>
+<a href="https://pypi.python.org/pypi/clovers_apscheduler"><img src="https://img.shields.io/pypi/v/clovers_apscheduler.svg" alt="pypi">
+</a><a href="https://pypi.python.org/pypi/clovers_apscheduler"><img src="https://img.shields.io/pypi/dm/clovers_apscheduler" alt="pypi download"></a>
+
 </div>
 
 ## 使用方式
 
 ```python
 from clovers_apscheduler import scheduler
 @scheduler.scheduled_job("cron", hour="*/4", misfire_grace_time=120)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-# clovers_apscheduler _â¨ clovers APScheduler å®æ¶ä»»å¡æä»¶ â¨_
-                    [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
+# clovers-apscheduler _â¨ clovers APScheduler å®æ¶ä»»å¡æä»¶ â¨_[python]
+                        _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ä½¿ç¨æ¹å¼ ```python from clovers_apscheduler import scheduler
 @scheduler.scheduled_job("cron", hour="*/4", misfire_grace_time=120) async def
 _(): pass ``` ## éç½®é¡¹ `apscheduler` çç¸å³éç½® åè [éç½®
 scheduler](https://apscheduler.readthedocs.io/en/latest/
 userguide.html#scheduler-config)ï¼[éç½®åæ°](https://
 apscheduler.readthedocs.io/en/latest/modules/schedulers/
 base.html#apscheduler.schedulers.base.BaseScheduler) éç½®éè¦åå«
```

### Comparing `clovers_apscheduler-0.1.3/PKG-INFO` & `clovers_apscheduler-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 Metadata-Version: 2.1
 Name: clovers-apscheduler
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
-Requires-Dist: clovers (>=0.1.2,<0.2.0)
+Requires-Dist: clovers (>=0.1.8,<0.2.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# clovers_apscheduler
+<div align="center">
+
+# clovers-apscheduler
 
 _✨ clovers APScheduler 定时任务插件 ✨_
 
-<div align="center">
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
-<a href="./LICENSE">
-  <img src="https://img.shields.io/github/license/KarisAya/clovers_apscheduler.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_apscheduler">
-  <img src="https://img.shields.io/pypi/v/clovers_apscheduler.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_apscheduler">
-  <img src="https://img.shields.io/pypi/dm/clovers_apscheduler" alt="pypi download">
-</a>
+<a href="./LICENSE"><img src="https://img.shields.io/github/license/KarisAya/clovers_apscheduler.svg" alt="license"></a>
+<a href="https://pypi.python.org/pypi/clovers_apscheduler"><img src="https://img.shields.io/pypi/v/clovers_apscheduler.svg" alt="pypi">
+</a><a href="https://pypi.python.org/pypi/clovers_apscheduler"><img src="https://img.shields.io/pypi/dm/clovers_apscheduler" alt="pypi download"></a>
+
 </div>
 
 ## 使用方式
 
 ```python
 from clovers_apscheduler import scheduler
 @scheduler.scheduled_job("cron", hour="*/4", misfire_grace_time=120)
```

#### html2text {}

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 2.1 Name: clovers-apscheduler Version: 0.1.3 Summary: Author:
-KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: apscheduler (>=3.10.4,<4.0.0) Requires-Dist: clovers
-(>=0.1.2,<0.2.0) Requires-Dist: pydantic (>=2.7.0,<3.0.0) Description-Content-
-Type: text/markdown # clovers_apscheduler _â¨ clovers APScheduler
-å®æ¶ä»»å¡æä»¶ â¨_
-                    [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
+Metadata-Version: 2.1 Name: clovers-apscheduler Version: 0.1.4 Summary: Author:
+KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
+Classifier: Programming Language :: Python :: 3 Requires-Dist: apscheduler
+(>=3.10.4,<4.0.0) Requires-Dist: clovers (>=0.1.8,<0.2.0) Requires-Dist:
+pydantic (>=2.7.0,<3.0.0) Description-Content-Type: text/markdown
+# clovers-apscheduler _â¨ clovers APScheduler å®æ¶ä»»å¡æä»¶ â¨_[python]
+                        _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ä½¿ç¨æ¹å¼ ```python from clovers_apscheduler import scheduler
 @scheduler.scheduled_job("cron", hour="*/4", misfire_grace_time=120) async def
 _(): pass ``` ## éç½®é¡¹ `apscheduler` çç¸å³éç½® åè [éç½®
 scheduler](https://apscheduler.readthedocs.io/en/latest/
 userguide.html#scheduler-config)ï¼[éç½®åæ°](https://
 apscheduler.readthedocs.io/en/latest/modules/schedulers/
 base.html#apscheduler.schedulers.base.BaseScheduler) éç½®éè¦åå«
```

