# Comparing `tmp/cxalio_studio_tools-0.1.7.tar.gz` & `tmp/cxalio_studio_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.1.7.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.1.8.tar", max compression
```

## Comparing `cxalio_studio_tools-0.1.7.tar` & `cxalio_studio_tools-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.1.7/LICENSE
--rw-r--r--   0        0        0      939 2024-04-26 02:04:09.273368 cxalio_studio_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      878 2024-04-26 02:20:05.540612 cxalio_studio_tools-0.1.7/README.md
--rw-r--r--   0        0        0      160 2024-04-26 02:03:52.295482 cxalio_studio_tools-0.1.7/src/cx_core/__init__.py
--rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/abstract_app.py
--rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/app_logger.py
--rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/datapackage.py
--rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/ffmpeg_progress_parser.py
--rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/folder_expander.py
--rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/timecode.py
--rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/timepoint.py
--rw-r--r--   0        0        0      466 2024-04-16 07:18:34.907476 cxalio_studio_tools-0.1.7/src/cx_core/tui_elements.py
--rw-r--r--   0        0        0      956 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_core/utils.py
--rw-r--r--   0        0        0       83 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     4579 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      482 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     3271 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-16 07:18:34.907476 cxalio_studio_tools-0.1.7/src/media_killer/env.py
--rw-r--r--   0        0        0     1840 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/media_killer/example_project.toml
--rw-r--r--   0        0        0     4004 2024-04-26 02:12:28.498590 cxalio_studio_tools-0.1.7/src/media_killer/help.md
--rw-r--r--   0        0        0     7178 2024-04-16 07:18:34.907476 cxalio_studio_tools-0.1.7/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     3719 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/media_killer/planner.py
--rw-r--r--   0        0        0     5006 2024-04-26 02:18:01.906577 cxalio_studio_tools-0.1.7/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     2382 2024-04-24 01:33:16.029996 cxalio_studio_tools-0.1.7/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     2791 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     3773 2024-04-24 01:33:16.029996 cxalio_studio_tools-0.1.7/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/sub_conv/__init__.py
--rw-r--r--   0        0        0      278 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/sub_conv/env.py
--rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     2937 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/sub_conv/help.md
--rw-r--r--   0        0        0     7432 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.7/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.1.8/LICENSE
+-rw-r--r--   0        0        0      995 2024-04-28 05:16:06.031109 cxalio_studio_tools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      927 2024-04-28 05:16:06.031109 cxalio_studio_tools-0.1.8/README.md
+-rw-r--r--   0        0        0      186 2024-04-28 05:16:06.031109 cxalio_studio_tools-0.1.8/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/abstract_app.py
+-rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/app_logger.py
+-rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/datapackage.py
+-rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/ffmpeg_progress_parser.py
+-rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/folder_expander.py
+-rw-r--r--   0        0        0      465 2024-04-28 05:16:06.031109 cxalio_studio_tools-0.1.8/src/cx_core/osinfo.py
+-rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/timecode.py
+-rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/timepoint.py
+-rw-r--r--   0        0        0      466 2024-04-16 07:18:34.907476 cxalio_studio_tools-0.1.8/src/cx_core/tui_elements.py
+-rw-r--r--   0        0        0      956 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_core/utils.py
+-rw-r--r--   0        0        0       83 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     4579 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      482 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     3271 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-16 07:18:34.907476 cxalio_studio_tools-0.1.8/src/media_killer/env.py
+-rw-r--r--   0        0        0     1840 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0     4004 2024-04-28 01:50:00.027410 cxalio_studio_tools-0.1.8/src/media_killer/help.md
+-rw-r--r--   0        0        0     7178 2024-04-28 05:16:06.031109 cxalio_studio_tools-0.1.8/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     3719 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/media_killer/planner.py
+-rw-r--r--   0        0        0     5006 2024-04-28 01:50:00.027410 cxalio_studio_tools-0.1.8/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     2382 2024-04-24 01:33:16.029996 cxalio_studio_tools-0.1.8/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     2791 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     3773 2024-04-24 01:33:16.029996 cxalio_studio_tools-0.1.8/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/sub_conv/env.py
+-rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     2937 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/sub_conv/help.md
+-rw-r--r--   0        0        0     7432 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.1.8/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.1.8/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.1.7/LICENSE` & `cxalio_studio_tools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/pyproject.toml` & `cxalio_studio_tools-0.1.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.1.7"
+version = "0.1.8"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
@@ -24,11 +24,12 @@
 python-ffmpeg = "^2.0.10"
 python-docx = "^1.1.0"
 openpyxl = "^3.1.2"
 
 [tool.poetry.scripts]
 mediakiller = 'media_killer:run'
 subconv = 'sub_conv:run'
+update_githubhosts = 'systools.update_githubhosts:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cxalio_studio_tools-0.1.7/README.md` & `cxalio_studio_tools-0.1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -30,10 +30,14 @@
 
 #### To-do
 
 - media-inspector 解析媒体信息
 
 #### Change-log
 
+- 0.1.8
+
+  增加 update-githubhosts 工具
+
 - 0.1.7
   
   media-killer 对map的设置进行了特殊处理，解决了无法重映射媒体流的bug
```

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/abstract_env.py` & `cxalio_studio_tools-0.1.8/src/cx_core/abstract_env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/app_logger.py` & `cxalio_studio_tools-0.1.8/src/cx_core/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/datapackage.py` & `cxalio_studio_tools-0.1.8/src/cx_core/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/ffmpeg_progress_parser.py` & `cxalio_studio_tools-0.1.8/src/cx_core/ffmpeg_progress_parser.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/folder_expander.py` & `cxalio_studio_tools-0.1.8/src/cx_core/folder_expander.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/timecode.py` & `cxalio_studio_tools-0.1.8/src/cx_core/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/timepoint.py` & `cxalio_studio_tools-0.1.8/src/cx_core/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_core/utils.py` & `cxalio_studio_tools-0.1.8/src/cx_core/utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.1.8/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.1.8/src/cx_subtitle/saver.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.1.8/src/cx_subtitle/subtitle_formatter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/env.py` & `cxalio_studio_tools-0.1.8/src/media_killer/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.1.8/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/help.md` & `cxalio_studio_tools-0.1.8/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.1.8/src/media_killer/media_killer_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class MediaKillerApp(AbstractApp):
     def __init__(self):
         super(MediaKillerApp,self).__init__()
         self.global_task = None
         self.app_name = 'media-killer'
-        self.app_version = '0.1.2'
+        self.app_version = '0.1.8'
         parser = ArgumentParser(prog=self.app_name, formatter_class=RichHelpFormatter,
                                 description='简单批量转码工具', epilog='Designed by xiii_1991')
         parser.add_argument('profile', help='指定配置文件路径', default=None, nargs='?')
         parser.add_argument('-g', '--generate-example-profile',
                             action="store_true", dest='generate_example',
                             help='生成范例文件')
         parser.add_argument('-a', '--add-source',
```

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/planner.py` & `cxalio_studio_tools-0.1.8/src/media_killer/planner.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.1.8/src/media_killer/profile_loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.1.8/src/media_killer/script_writer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.1.8/src/media_killer/source_adapter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.1.8/src/media_killer/transcoder.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/sub_conv/help.md` & `cxalio_studio_tools-0.1.8/src/sub_conv/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/src/sub_conv/subconv_app.py` & `cxalio_studio_tools-0.1.8/src/sub_conv/subconv_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.7/PKG-INFO` & `cxalio_studio_tools-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
@@ -53,11 +53,15 @@
 
 #### To-do
 
 - media-inspector 解析媒体信息
 
 #### Change-log
 
+- 0.1.8
+
+  增加 update-githubhosts 工具
+
 - 0.1.7
   
   media-killer 对map的设置进行了特殊处理，解决了无法重映射媒体流的bug
```

