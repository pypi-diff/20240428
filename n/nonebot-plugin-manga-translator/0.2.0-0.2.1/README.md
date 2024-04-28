# Comparing `tmp/nonebot_plugin_manga_translator-0.2.0.tar.gz` & `tmp/nonebot_plugin_manga_translator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_manga_translator-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_manga_translator-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_manga_translator-0.2.0.tar` & `nonebot_plugin_manga_translator-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/LICENSE
--rw-r--r--   0        0        0     9353 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/README.md
--rw-r--r--   0        0        0     6922 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/__init__.py
--rw-r--r--   0        0        0      334 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/config.py
--rw-r--r--   0        0        0    10693 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/utils.py
--rw-r--r--   0        0        0      524 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10157 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-28 11:34:18.648225 nonebot_plugin_manga_translator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9353 2024-04-28 11:34:18.648225 nonebot_plugin_manga_translator-0.2.1/README.md
+-rw-r--r--   0        0        0     6922 2024-04-28 11:34:18.648225 nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-28 11:34:18.652225 nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/config.py
+-rw-r--r--   0        0        0    10693 2024-04-28 11:34:18.652225 nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/utils.py
+-rw-r--r--   0        0        0      524 2024-04-28 11:34:18.652225 nonebot_plugin_manga_translator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10157 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_manga_translator-0.2.0/LICENSE` & `nonebot_plugin_manga_translator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.2.0/README.md` & `nonebot_plugin_manga_translator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/__init__.py` & `nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/utils.py` & `nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.2.0/pyproject.toml` & `nonebot_plugin_manga_translator-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-manga-translator"
-version = "0.2.0"
+version = "0.2.1"
 description = "基于nonebot2的适配多种api的图片/漫画翻译插件"
 authors = ["xenophon <674550338@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_manga_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_manga_translator-0.2.0/PKG-INFO` & `nonebot_plugin_manga_translator-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-manga-translator
-Version: 0.2.0
+Version: 0.2.1
 Summary: 基于nonebot2的适配多种api的图片/漫画翻译插件
 License: MIT
 Author: xenophon
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.2.0
+Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.2.1
 Summary: åºäºnonebot2çééå¤ç§apiçå¾ç/æ¼«ç»ç¿»è¯æä»¶ License:
 MIT Author: xenophon Author-email: 674550338@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: Pillow
```

