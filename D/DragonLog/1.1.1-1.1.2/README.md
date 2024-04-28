# Comparing `tmp/dragonlog-1.1.1.tar.gz` & `tmp/dragonlog-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonlog-1.1.1.tar", last modified: Sun Apr 21 07:46:14 2024, max compression
+gzip compressed data, was "dragonlog-1.1.2.tar", last modified: Sun Apr 28 08:33:03 2024, max compression
```

## Comparing `dragonlog-1.1.1.tar` & `dragonlog-1.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:46:14.344909 dragonlog-1.1.1/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:46:14.339420 dragonlog-1.1.1/DragonLog.egg-info/
--rw-rw-rw-   0        0        0     7401 2024-04-21 07:46:14.000000 dragonlog-1.1.1/DragonLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1603 2024-04-21 07:46:14.000000 dragonlog-1.1.1/DragonLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:46:14.000000 dragonlog-1.1.1/DragonLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-21 07:46:14.000000 dragonlog-1.1.1/DragonLog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-04-21 07:46:14.000000 dragonlog-1.1.1/DragonLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-21 07:46:14.000000 dragonlog-1.1.1/DragonLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.1.1/LICENCE.txt
--rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7401 2024-04-21 07:46:14.342414 dragonlog-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 07:46:14.205186 dragonlog-1.1.1/dragonlog/
--rw-rw-rw-   0        0        0    10562 2024-04-15 18:06:37.000000 dragonlog-1.1.1/dragonlog/CallBook.py
--rw-rw-rw-   0        0        0    63598 2024-04-21 07:43:44.000000 dragonlog-1.1.1/dragonlog/DragonLog.py
--rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.1.1/dragonlog/DragonLog_AppSelect.py
--rw-rw-rw-   0        0        0     3041 2024-04-21 07:45:09.000000 dragonlog-1.1.1/dragonlog/DragonLog_AppSelect_ui.py
--rw-rw-rw-   0        0        0    17410 2024-04-21 07:45:08.000000 dragonlog-1.1.1/dragonlog/DragonLog_MainWindow_ui.py
--rw-rw-rw-   0        0        0    47234 2024-04-19 18:34:33.000000 dragonlog-1.1.1/dragonlog/DragonLog_QSOForm.py
--rw-rw-rw-   0        0        0    38980 2024-04-21 07:45:09.000000 dragonlog-1.1.1/dragonlog/DragonLog_QSOForm_ui.py
--rw-rw-rw-   0        0        0    21133 2024-04-18 06:08:40.000000 dragonlog-1.1.1/dragonlog/DragonLog_Settings.py
--rw-rw-rw-   0        0        0    39219 2024-04-21 07:45:09.000000 dragonlog-1.1.1/dragonlog/DragonLog_Settings_ui.py
--rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.1.1/dragonlog/LoTW.py
--rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.1.1/dragonlog/Logger.py
--rw-rw-rw-   0        0        0     1134 2024-04-15 17:33:29.000000 dragonlog-1.1.1/dragonlog/RegEx.py
--rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.1.1/dragonlog/__init__.py
--rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.1.1/dragonlog/__main__.py
--rw-rw-rw-   0        0        0       65 2024-04-21 07:45:08.000000 dragonlog-1.1.1/dragonlog/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:46:14.219658 dragonlog-1.1.1/dragonlog/data/
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.1/dragonlog/data/README.md
--rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.1.1/dragonlog/data/bands.json
--rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.1.1/dragonlog/data/cb_channels.json
--rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.1.1/dragonlog/data/color_map.json
-drwxrwxrwx   0        0        0        0 2024-04-21 07:46:14.226644 dragonlog-1.1.1/dragonlog/data/i18n/
--rw-rw-rw-   0        0        0    24604 2024-04-21 07:45:12.000000 dragonlog-1.1.1/dragonlog/data/i18n/DragonLog_de.qm
--rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.1.1/dragonlog/data/i18n/ascii_replace_de.json
--rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.1.1/dragonlog/data/modes.json
--rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.1.1/dragonlog/eQSL.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:46:14.334430 dragonlog-1.1.1/dragonlog/icons/
--rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.1.1/dragonlog/icons/Screenshot.png
--rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.1.1/dragonlog/icons/db.png
--rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.1.1/dragonlog/icons/edit.png
--rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.1.1/dragonlog/icons/edit_add.png
--rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.1.1/dragonlog/icons/edit_addmulti.png
--rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.1.1/dragonlog/icons/edit_addmulti.xcf
--rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.1.1/dragonlog/icons/edit_remove.png
--rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.1.1/dragonlog/icons/exit.png
--rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.1.1/dragonlog/icons/file_doc.png
--rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.1.1/dragonlog/icons/fileexport.png
--rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.1.1/dragonlog/icons/fileimport.png
--rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.1.1/dragonlog/icons/gear.png
--rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.1.1/dragonlog/icons/help.png
--rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.1.1/dragonlog/icons/icons8-dragon-96.png
--rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.1.1/dragonlog/icons/icons8-dragon-96.xcf
--rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.1.1/dragonlog/icons/info.png
--rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.1.1/dragonlog/icons/logo.ico
--rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.1.1/dragonlog/icons/no.png
--rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.1.1/dragonlog/icons/ok.png
--rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.1.1/dragonlog/icons/player_play.png
--rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.1.1/dragonlog/icons/player_stop.png
--rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.1.1/dragonlog/icons/upload_lotw.png
--rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.1.1/dragonlog/icons/upload_lotw.xcf
--rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.1.1/dragonlog/icons/watch.png
--rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 07:46:14.345408 dragonlog-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.1.1/setup_msi.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.228769 dragonlog-1.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.218980 dragonlog-1.1.2/DragonLog.egg-info/
+-rw-rw-rw-   0        0        0     7401 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1603 2024-04-28 08:33:03.000000 dragonlog-1.1.2/DragonLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7401 2024-04-28 08:33:03.224316 dragonlog-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.105147 dragonlog-1.1.2/dragonlog/
+-rw-rw-rw-   0        0        0    10562 2024-04-15 18:06:37.000000 dragonlog-1.1.2/dragonlog/CallBook.py
+-rw-rw-rw-   0        0        0    63750 2024-04-21 09:50:28.000000 dragonlog-1.1.2/dragonlog/DragonLog.py
+-rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.1.2/dragonlog/DragonLog_AppSelect.py
+-rw-rw-rw-   0        0        0     3041 2024-04-28 08:31:54.000000 dragonlog-1.1.2/dragonlog/DragonLog_AppSelect_ui.py
+-rw-rw-rw-   0        0        0    17410 2024-04-28 08:31:53.000000 dragonlog-1.1.2/dragonlog/DragonLog_MainWindow_ui.py
+-rw-rw-rw-   0        0        0    47332 2024-04-28 08:25:13.000000 dragonlog-1.1.2/dragonlog/DragonLog_QSOForm.py
+-rw-rw-rw-   0        0        0    38980 2024-04-28 08:31:54.000000 dragonlog-1.1.2/dragonlog/DragonLog_QSOForm_ui.py
+-rw-rw-rw-   0        0        0    21133 2024-04-18 06:08:40.000000 dragonlog-1.1.2/dragonlog/DragonLog_Settings.py
+-rw-rw-rw-   0        0        0    39219 2024-04-28 08:31:54.000000 dragonlog-1.1.2/dragonlog/DragonLog_Settings_ui.py
+-rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.1.2/dragonlog/LoTW.py
+-rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.1.2/dragonlog/Logger.py
+-rw-rw-rw-   0        0        0     1134 2024-04-15 17:33:29.000000 dragonlog-1.1.2/dragonlog/RegEx.py
+-rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.1.2/dragonlog/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.1.2/dragonlog/__main__.py
+-rw-rw-rw-   0        0        0       65 2024-04-28 08:31:53.000000 dragonlog-1.1.2/dragonlog/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.117605 dragonlog-1.1.2/dragonlog/data/
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.2/dragonlog/data/README.md
+-rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.1.2/dragonlog/data/bands.json
+-rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.1.2/dragonlog/data/cb_channels.json
+-rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.1.2/dragonlog/data/color_map.json
+drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.125869 dragonlog-1.1.2/dragonlog/data/i18n/
+-rw-rw-rw-   0        0        0    24604 2024-04-28 08:31:57.000000 dragonlog-1.1.2/dragonlog/data/i18n/DragonLog_de.qm
+-rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.1.2/dragonlog/data/i18n/ascii_replace_de.json
+-rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.1.2/dragonlog/data/modes.json
+-rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.1.2/dragonlog/eQSL.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.211747 dragonlog-1.1.2/dragonlog/icons/
+-rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.1.2/dragonlog/icons/Screenshot.png
+-rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.1.2/dragonlog/icons/db.png
+-rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.1.2/dragonlog/icons/edit.png
+-rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.1.2/dragonlog/icons/edit_add.png
+-rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.1.2/dragonlog/icons/edit_addmulti.png
+-rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.1.2/dragonlog/icons/edit_addmulti.xcf
+-rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.1.2/dragonlog/icons/edit_remove.png
+-rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.1.2/dragonlog/icons/exit.png
+-rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.1.2/dragonlog/icons/file_doc.png
+-rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.1.2/dragonlog/icons/fileexport.png
+-rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.1.2/dragonlog/icons/fileimport.png
+-rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.1.2/dragonlog/icons/gear.png
+-rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.1.2/dragonlog/icons/help.png
+-rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.png
+-rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.xcf
+-rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.1.2/dragonlog/icons/info.png
+-rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.1.2/dragonlog/icons/logo.ico
+-rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.1.2/dragonlog/icons/no.png
+-rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.1.2/dragonlog/icons/ok.png
+-rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.1.2/dragonlog/icons/player_play.png
+-rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.1.2/dragonlog/icons/player_stop.png
+-rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.1.2/dragonlog/icons/upload_lotw.png
+-rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.1.2/dragonlog/icons/upload_lotw.xcf
+-rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.1.2/dragonlog/icons/watch.png
+-rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 08:33:03.229806 dragonlog-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.1.2/setup_msi.py
```

### Comparing `dragonlog-1.1.1/DragonLog.egg-info/PKG-INFO` & `dragonlog-1.1.2/DragonLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.1.1
+Version: 1.1.2
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonlog-1.1.1/DragonLog.egg-info/SOURCES.txt` & `dragonlog-1.1.2/DragonLog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/PKG-INFO` & `dragonlog-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.1.1
+Version: 1.1.2
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonlog-1.1.1/README.md` & `dragonlog-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/CallBook.py` & `dragonlog-1.1.2/dragonlog/CallBook.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog.py` & `dragonlog-1.1.2/dragonlog/DragonLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1399,14 +1399,21 @@
         e.accept()
 
 
 def main():
     app = QtWidgets.QApplication(sys.argv)
     app_path = os.path.dirname(__file__)
 
+    css = '''QToolBox::tab {
+        background: #b0c4de;
+        border-radius: 2px;
+        color: black;
+    }'''
+    app.setStyleSheet(css)
+
     translator = QtCore.QTranslator(app)
     translator.load(os.path.abspath(app_path + '/data/i18n/DragonLog_' + QtCore.QLocale.system().name()))
     app.installTranslator(translator)
 
     file = None
     args = app.arguments()
     if len(args) > 1:
```

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_AppSelect.py` & `dragonlog-1.1.2/dragonlog/DragonLog_AppSelect.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_AppSelect_ui.py` & `dragonlog-1.1.2/dragonlog/DragonLog_AppSelect_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_MainWindow_ui.py` & `dragonlog-1.1.2/dragonlog/DragonLog_MainWindow_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_QSOForm.py` & `dragonlog-1.1.2/dragonlog/DragonLog_QSOForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
                                               self.tr('Callsign not found') + f': {exc.args[0]}')
         except Exception as exc:
             self.log.exception(exc)
             QtWidgets.QMessageBox.warning(self, self.tr('Callbook search error'),
                                           self.tr('During callbook search an error occured') + f':\n{exc}')
 
     def saveLog(self):
-        if self.__old_values__['hamqth'] in ('Y', 'M'):
+        if self.__old_values__ and self.__old_values__['hamqth'] in ('Y', 'M'):
             self.hamQTHCheckBox.setChecked(True)
 
         if self.__change_mode__:
             self.dragonlog.updateQSO(self.qso_id)
         else:
             self.dragonlog.fetchQSO()
 
@@ -804,15 +804,17 @@
                 'PROGRAMID': self.dragonlog.programName,
                 'PROGRAMVERSION': self.dragonlog.programVersion,
                 'CREATED_TIMESTAMP': QtCore.QDateTime.currentDateTimeUtc().toString(
                     'yyyyMMdd HHmmss')
             },
             'RECORDS': [record]}
 
-        if self.hamQTHCheckBox.isChecked() and self.__old_values__['hamqth'] not in ('Y', 'M'):
+        upload_hamqth = self.__old_values__['hamqth'] not in ('Y', 'M') if self.__old_values__ else True
+
+        if self.hamQTHCheckBox.isChecked() and upload_hamqth:
             logbook = HamQTHCallBook(self.logger,
                                      f'{self.dragonlog.programName}-{self.dragonlog.programVersion}',
                                      )
             try:
                 logbook.upload_log(self.settings.value(f'callbook/HamQTH_user', ''),
                                    self.settings_form.callbookPassword(CallBookType.HamQTH),
                                    adif_doc)
```

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_QSOForm_ui.py` & `dragonlog-1.1.2/dragonlog/DragonLog_QSOForm_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_Settings.py` & `dragonlog-1.1.2/dragonlog/DragonLog_Settings.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/DragonLog_Settings_ui.py` & `dragonlog-1.1.2/dragonlog/DragonLog_Settings_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/LoTW.py` & `dragonlog-1.1.2/dragonlog/LoTW.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/Logger.py` & `dragonlog-1.1.2/dragonlog/Logger.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/RegEx.py` & `dragonlog-1.1.2/dragonlog/RegEx.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/data/README.md` & `dragonlog-1.1.2/dragonlog/data/README.md`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/data/bands.json` & `dragonlog-1.1.2/dragonlog/data/bands.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/data/cb_channels.json` & `dragonlog-1.1.2/dragonlog/data/cb_channels.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/data/color_map.json` & `dragonlog-1.1.2/dragonlog/data/color_map.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/data/i18n/DragonLog_de.qm` & `dragonlog-1.1.2/dragonlog/data/i18n/DragonLog_de.qm`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/data/modes.json` & `dragonlog-1.1.2/dragonlog/data/modes.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/eQSL.py` & `dragonlog-1.1.2/dragonlog/eQSL.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/Screenshot.png` & `dragonlog-1.1.2/dragonlog/icons/Screenshot.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/db.png` & `dragonlog-1.1.2/dragonlog/icons/db.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/edit.png` & `dragonlog-1.1.2/dragonlog/icons/edit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/edit_add.png` & `dragonlog-1.1.2/dragonlog/icons/edit_add.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/edit_addmulti.png` & `dragonlog-1.1.2/dragonlog/icons/edit_addmulti.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/edit_addmulti.xcf` & `dragonlog-1.1.2/dragonlog/icons/edit_addmulti.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/edit_remove.png` & `dragonlog-1.1.2/dragonlog/icons/edit_remove.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/exit.png` & `dragonlog-1.1.2/dragonlog/icons/exit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/file_doc.png` & `dragonlog-1.1.2/dragonlog/icons/file_doc.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/fileexport.png` & `dragonlog-1.1.2/dragonlog/icons/fileexport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/fileimport.png` & `dragonlog-1.1.2/dragonlog/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/gear.png` & `dragonlog-1.1.2/dragonlog/icons/gear.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/help.png` & `dragonlog-1.1.2/dragonlog/icons/help.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/icons8-dragon-96.png` & `dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/icons8-dragon-96.xcf` & `dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/info.png` & `dragonlog-1.1.2/dragonlog/icons/info.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/logo.ico` & `dragonlog-1.1.2/dragonlog/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/no.png` & `dragonlog-1.1.2/dragonlog/icons/no.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/ok.png` & `dragonlog-1.1.2/dragonlog/icons/ok.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/player_play.png` & `dragonlog-1.1.2/dragonlog/icons/player_play.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/player_stop.png` & `dragonlog-1.1.2/dragonlog/icons/player_stop.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/upload_lotw.png` & `dragonlog-1.1.2/dragonlog/icons/upload_lotw.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/upload_lotw.xcf` & `dragonlog-1.1.2/dragonlog/icons/upload_lotw.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/dragonlog/icons/watch.png` & `dragonlog-1.1.2/dragonlog/icons/watch.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/pyproject.toml` & `dragonlog-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.1/setup_msi.py` & `dragonlog-1.1.2/setup_msi.py`

 * *Files identical despite different names*

