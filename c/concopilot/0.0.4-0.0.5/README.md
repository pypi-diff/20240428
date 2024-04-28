# Comparing `tmp/concopilot-0.0.4.tar.gz` & `tmp/concopilot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concopilot-0.0.4.tar", last modified: Mon Mar 18 04:18:08 2024, max compression
+gzip compressed data, was "concopilot-0.0.5.tar", last modified: Sun Apr 28 02:32:11 2024, max compression
```

## Comparing `concopilot-0.0.4.tar` & `concopilot-0.0.5.tar`

### file list

```diff
@@ -1,121 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.976883 concopilot-0.0.4/
--rw-rw-rw-   0        0        0    11558 2023-10-22 06:22:39.000000 concopilot-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     9844 2024-03-18 04:18:08.975885 concopilot-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     9063 2024-02-24 15:01:00.000000 concopilot-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.515116 concopilot-0.0.4/concopilot/
--rw-rw-rw-   0        0        0      165 2023-11-14 13:08:35.000000 concopilot-0.0.4/concopilot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.545036 concopilot-0.0.4/concopilot/basic/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.547086 concopilot-0.0.4/concopilot/basic/copilot/
--rw-rw-rw-   0        0        0      207 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/copilot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.548028 concopilot-0.0.4/concopilot/basic/interface/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.551021 concopilot-0.0.4/concopilot/basic/interface/cmd/
--rw-rw-rw-   0        0        0      205 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/interface/cmd/__init__.py
--rw-rw-rw-   0        0        0     2442 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/basic/interface/cmd/interface.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.566979 concopilot-0.0.4/concopilot/basic/message/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/message/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.568191 concopilot-0.0.4/concopilot/basic/message/manager/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/message/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.570967 concopilot-0.0.4/concopilot/basic/message/manager/jsonmanager/
--rw-rw-rw-   0        0        0      217 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/message/manager/jsonmanager/__init__.py
--rw-rw-rw-   0        0        0     7120 2024-03-16 07:50:10.000000 concopilot-0.0.4/concopilot/basic/message/manager/jsonmanager/manager.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.581938 concopilot-0.0.4/concopilot/basic/message/manager/strmanager/
--rw-rw-rw-   0        0        0      215 2023-11-14 13:08:35.000000 concopilot-0.0.4/concopilot/basic/message/manager/strmanager/__init__.py
--rw-rw-rw-   0        0        0     1504 2024-03-16 07:50:32.000000 concopilot-0.0.4/concopilot/basic/message/manager/strmanager/manager.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.593906 concopilot-0.0.4/concopilot/basic/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/plugin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.594902 concopilot-0.0.4/concopilot/basic/plugin/manager/
--rw-rw-rw-   0        0        0      234 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/plugin/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.596897 concopilot-0.0.4/concopilot/basic/resource/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.597895 concopilot-0.0.4/concopilot/basic/resource/category/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/resource/category/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.598892 concopilot-0.0.4/concopilot/basic/resource/category/disk/
--rw-rw-rw-   0        0        0      209 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/resource/category/disk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.599891 concopilot-0.0.4/concopilot/basic/resource/manager/
--rw-rw-rw-   0        0        0      232 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/resource/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.601884 concopilot-0.0.4/concopilot/basic/storage/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/storage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.606871 concopilot-0.0.4/concopilot/basic/storage/disk/
--rw-rw-rw-   0        0        0      193 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/basic/storage/disk/__init__.py
--rw-rw-rw-   0        0        0     5801 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/basic/storage/disk/storage.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.645050 concopilot-0.0.4/concopilot/framework/
--rw-rw-rw-   0        0        0      123 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.672695 concopilot-0.0.4/concopilot/framework/asset/
--rw-rw-rw-   0        0        0      109 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/framework/asset/__init__.py
--rw-rw-rw-   0        0        0    10223 2024-03-18 02:34:13.000000 concopilot-0.0.4/concopilot/framework/asset/asset.py
--rw-rw-rw-   0        0        0      338 2024-03-18 02:28:58.000000 concopilot-0.0.4/concopilot/framework/asset/asset_regex.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.675689 concopilot-0.0.4/concopilot/framework/cerebrum/
--rw-rw-rw-   0        0        0      222 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/cerebrum/__init__.py
--rw-rw-rw-   0        0        0     5108 2024-03-16 07:54:45.000000 concopilot-0.0.4/concopilot/framework/cerebrum/cerebrum.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.690647 concopilot-0.0.4/concopilot/framework/context/
--rw-rw-rw-   0        0        0       88 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/framework/context/__init__.py
--rw-rw-rw-   0        0        0      573 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/framework/context/context.py
--rw-rw-rw-   0        0        0     5886 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/framework/copilot.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.728547 concopilot-0.0.4/concopilot/framework/identity/
--rw-rw-rw-   0        0        0       91 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/identity/__init__.py
--rw-rw-rw-   0        0        0      506 2024-03-12 12:46:09.000000 concopilot-0.0.4/concopilot/framework/identity/identity.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.738564 concopilot-0.0.4/concopilot/framework/interactor/
--rw-rw-rw-   0        0        0      138 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/interactor/__init__.py
--rw-rw-rw-   0        0        0     2509 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/interactor/interactor.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.791379 concopilot-0.0.4/concopilot/framework/interface/
--rw-rw-rw-   0        0        0      102 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/interface/__init__.py
--rw-rw-rw-   0        0        0     2180 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/interface/interface.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.797442 concopilot-0.0.4/concopilot/framework/message/
--rw-rw-rw-   0        0        0       88 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/message/__init__.py
--rw-rw-rw-   0        0        0     1460 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/message/manager.py
--rw-rw-rw-   0        0        0     4175 2024-03-16 03:26:56.000000 concopilot-0.0.4/concopilot/framework/message/message.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.837256 concopilot-0.0.4/concopilot/framework/plugin/
--rw-rw-rw-   0        0        0      264 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/plugin/__init__.py
--rw-rw-rw-   0        0        0     7535 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/framework/plugin/manager.py
--rw-rw-rw-   0        0        0    16491 2024-03-16 06:06:03.000000 concopilot-0.0.4/concopilot/framework/plugin/plugin.py
--rw-rw-rw-   0        0        0     1196 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/plugin/promptgenerator.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.867176 concopilot-0.0.4/concopilot/framework/resource/
--rw-rw-rw-   0        0        0      245 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.879143 concopilot-0.0.4/concopilot/framework/resource/category/
--rw-rw-rw-   0        0        0      136 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/resource/category/__init__.py
--rw-rw-rw-   0        0        0     2092 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/resource/category/disk.py
--rw-rw-rw-   0        0        0     1685 2024-03-16 04:08:08.000000 concopilot-0.0.4/concopilot/framework/resource/category/model.py
--rw-rw-rw-   0        0        0     4379 2024-03-12 12:34:07.000000 concopilot-0.0.4/concopilot/framework/resource/manager.py
--rw-rw-rw-   0        0        0     1719 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/resource/resource.py
--rw-rw-rw-   0        0        0     2114 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/run.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.884131 concopilot-0.0.4/concopilot/framework/storage/
--rw-rw-rw-   0        0        0       88 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/framework/storage/__init__.py
--rw-rw-rw-   0        0        0     3219 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/framework/storage/storage.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.913054 concopilot-0.0.4/concopilot/package/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/package/__init__.py
--rw-rw-rw-   0        0        0     2082 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/package/captcha.py
--rw-rw-rw-   0        0        0     1172 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/package/check.py
--rw-rw-rw-   0        0        0     7065 2023-12-04 12:16:36.000000 concopilot-0.0.4/concopilot/package/config.py
--rw-rw-rw-   0        0        0    14362 2024-03-14 14:18:04.000000 concopilot-0.0.4/concopilot/package/conpack.py
--rw-rw-rw-   0        0        0      526 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/package/encrypt.py
--rw-rw-rw-   0        0        0      654 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/package/error.py
--rw-rw-rw-   0        0        0    11760 2024-03-05 06:46:04.000000 concopilot-0.0.4/concopilot/package/repo.py
--rw-rw-rw-   0        0        0     4355 2023-11-14 13:08:35.000000 concopilot-0.0.4/concopilot/package/request.py
--rw-rw-rw-   0        0        0     2149 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/package/transfer.py
--rw-rw-rw-   0        0        0     3089 2024-03-05 06:46:04.000000 concopilot-0.0.4/concopilot/package/validator.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.935006 concopilot-0.0.4/concopilot/util/
--rw-rw-rw-   0        0        0       93 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/util/__init__.py
--rw-rw-rw-   0        0        0     2698 2024-03-11 07:30:18.000000 concopilot-0.0.4/concopilot/util/class_dict.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.946963 concopilot-0.0.4/concopilot/util/config/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/util/config/__init__.py
--rw-rw-rw-   0        0        0      757 2023-12-04 12:16:36.000000 concopilot-0.0.4/concopilot/util/config/tool.py
--rw-rw-rw-   0        0        0      882 2023-11-09 05:34:47.000000 concopilot-0.0.4/concopilot/util/config/versions.py
--rw-rw-rw-   0        0        0     1227 2024-03-15 13:46:02.000000 concopilot-0.0.4/concopilot/util/dicts.py
--rw-rw-rw-   0        0        0      121 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/util/error.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.953945 concopilot-0.0.4/concopilot/util/initializer/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.4/concopilot/util/initializer/__init__.py
--rw-rw-rw-   0        0        0     3863 2023-11-14 13:08:35.000000 concopilot-0.0.4/concopilot/util/initializer/component.py
--rw-rw-rw-   0        0        0      486 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/util/jsons.py
--rw-rw-rw-   0        0        0      372 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/util/singleton.py
--rw-rw-rw-   0        0        0      241 2024-02-24 15:01:00.000000 concopilot-0.0.4/concopilot/util/yamls.py
-drwxrwxrwx   0        0        0        0 2024-03-18 04:18:08.973890 concopilot-0.0.4/concopilot.egg-info/
--rw-rw-rw-   0        0        0     9844 2024-03-18 04:18:08.000000 concopilot-0.0.4/concopilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3110 2024-03-18 04:18:08.000000 concopilot-0.0.4/concopilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 04:18:08.000000 concopilot-0.0.4/concopilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-03-18 04:18:08.000000 concopilot-0.0.4/concopilot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2024-03-18 04:18:08.000000 concopilot-0.0.4/concopilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-18 04:18:08.000000 concopilot-0.0.4/concopilot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      877 2024-03-10 11:20:08.000000 concopilot-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 04:18:08.977885 concopilot-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.292190 concopilot-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2023-10-22 06:22:39.000000 concopilot-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     9844 2024-04-28 02:32:11.290198 concopilot-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9063 2024-02-24 15:01:00.000000 concopilot-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.118657 concopilot-0.0.5/concopilot/
+-rw-rw-rw-   0        0        0      165 2023-11-14 13:08:35.000000 concopilot-0.0.5/concopilot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.146634 concopilot-0.0.5/concopilot/basic/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.147578 concopilot-0.0.5/concopilot/basic/copilot/
+-rw-rw-rw-   0        0        0      199 2024-04-05 08:46:31.000000 concopilot-0.0.5/concopilot/basic/copilot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.148575 concopilot-0.0.5/concopilot/basic/interface/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.152565 concopilot-0.0.5/concopilot/basic/interface/cmd/
+-rw-rw-rw-   0        0        0      205 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/interface/cmd/__init__.py
+-rw-rw-rw-   0        0        0     2604 2024-04-26 09:42:57.000000 concopilot-0.0.5/concopilot/basic/interface/cmd/interface.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.153562 concopilot-0.0.5/concopilot/basic/interface/duplex/
+-rw-rw-rw-   0        0        0      234 2024-04-05 08:46:31.000000 concopilot-0.0.5/concopilot/basic/interface/duplex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.155560 concopilot-0.0.5/concopilot/basic/message/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/message/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.156555 concopilot-0.0.5/concopilot/basic/message/manager/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/message/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.158549 concopilot-0.0.5/concopilot/basic/message/manager/jsonmanager/
+-rw-rw-rw-   0        0        0      217 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/message/manager/jsonmanager/__init__.py
+-rw-rw-rw-   0        0        0     7349 2024-04-10 01:24:07.000000 concopilot-0.0.5/concopilot/basic/message/manager/jsonmanager/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.163536 concopilot-0.0.5/concopilot/basic/message/manager/strmanager/
+-rw-rw-rw-   0        0        0      215 2023-11-14 13:08:35.000000 concopilot-0.0.5/concopilot/basic/message/manager/strmanager/__init__.py
+-rw-rw-rw-   0        0        0     1610 2024-04-10 01:24:07.000000 concopilot-0.0.5/concopilot/basic/message/manager/strmanager/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.164532 concopilot-0.0.5/concopilot/basic/plugin/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.165529 concopilot-0.0.5/concopilot/basic/plugin/manager/
+-rw-rw-rw-   0        0        0      227 2024-04-05 08:46:31.000000 concopilot-0.0.5/concopilot/basic/plugin/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.168522 concopilot-0.0.5/concopilot/basic/resource/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.169520 concopilot-0.0.5/concopilot/basic/resource/category/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/resource/category/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.170517 concopilot-0.0.5/concopilot/basic/resource/category/disk/
+-rw-rw-rw-   0        0        0      203 2024-04-05 08:46:31.000000 concopilot-0.0.5/concopilot/basic/resource/category/disk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.171514 concopilot-0.0.5/concopilot/basic/resource/manager/
+-rw-rw-rw-   0        0        0      225 2024-04-05 08:46:31.000000 concopilot-0.0.5/concopilot/basic/resource/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.172511 concopilot-0.0.5/concopilot/basic/storage/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/storage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.174506 concopilot-0.0.5/concopilot/basic/storage/disk/
+-rw-rw-rw-   0        0        0      193 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/basic/storage/disk/__init__.py
+-rw-rw-rw-   0        0        0     5801 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/basic/storage/disk/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.181488 concopilot-0.0.5/concopilot/framework/
+-rw-rw-rw-   0        0        0      175 2024-04-04 12:44:18.000000 concopilot-0.0.5/concopilot/framework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.185479 concopilot-0.0.5/concopilot/framework/asset/
+-rw-rw-rw-   0        0        0      109 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/asset/__init__.py
+-rw-rw-rw-   0        0        0    10223 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/asset/asset.py
+-rw-rw-rw-   0        0        0      338 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/asset/asset_regex.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.188481 concopilot-0.0.5/concopilot/framework/cerebrum/
+-rw-rw-rw-   0        0        0      222 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/cerebrum/__init__.py
+-rw-rw-rw-   0        0        0     5108 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/cerebrum/cerebrum.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.191460 concopilot-0.0.5/concopilot/framework/context/
+-rw-rw-rw-   0        0        0       88 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/context/__init__.py
+-rw-rw-rw-   0        0        0      573 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/context/context.py
+-rw-rw-rw-   0        0        0     7981 2024-04-28 02:02:12.000000 concopilot-0.0.5/concopilot/framework/copilot.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.196447 concopilot-0.0.5/concopilot/framework/identity/
+-rw-rw-rw-   0        0        0       91 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/identity/__init__.py
+-rw-rw-rw-   0        0        0      506 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/identity/identity.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.200436 concopilot-0.0.5/concopilot/framework/interactor/
+-rw-rw-rw-   0        0        0      138 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/interactor/__init__.py
+-rw-rw-rw-   0        0        0     3899 2024-04-26 06:00:32.000000 concopilot-0.0.5/concopilot/framework/interactor/interactor.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.205423 concopilot-0.0.5/concopilot/framework/interface/
+-rw-rw-rw-   0        0        0      346 2024-04-05 03:06:38.000000 concopilot-0.0.5/concopilot/framework/interface/__init__.py
+-rw-rw-rw-   0        0        0     3927 2024-04-26 09:42:57.000000 concopilot-0.0.5/concopilot/framework/interface/duplex.py
+-rw-rw-rw-   0        0        0     4304 2024-04-26 09:46:23.000000 concopilot-0.0.5/concopilot/framework/interface/interface.py
+-rw-rw-rw-   0        0        0     1905 2024-04-05 03:06:38.000000 concopilot-0.0.5/concopilot/framework/interface/simplex.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.212405 concopilot-0.0.5/concopilot/framework/message/
+-rw-rw-rw-   0        0        0       88 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/message/__init__.py
+-rw-rw-rw-   0        0        0     1606 2024-04-10 01:24:08.000000 concopilot-0.0.5/concopilot/framework/message/manager.py
+-rw-rw-rw-   0        0        0     4175 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/message/message.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.220383 concopilot-0.0.5/concopilot/framework/plugin/
+-rw-rw-rw-   0        0        0      264 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/plugin/__init__.py
+-rw-rw-rw-   0        0        0     7845 2024-04-04 12:44:18.000000 concopilot-0.0.5/concopilot/framework/plugin/manager.py
+-rw-rw-rw-   0        0        0    16929 2024-04-10 01:24:07.000000 concopilot-0.0.5/concopilot/framework/plugin/plugin.py
+-rw-rw-rw-   0        0        0     1196 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/framework/plugin/promptgenerator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.227365 concopilot-0.0.5/concopilot/framework/resource/
+-rw-rw-rw-   0        0        0      245 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.241327 concopilot-0.0.5/concopilot/framework/resource/category/
+-rw-rw-rw-   0        0        0      136 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/resource/category/__init__.py
+-rw-rw-rw-   0        0        0     2092 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/resource/category/disk.py
+-rw-rw-rw-   0        0        0     1685 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/resource/category/model.py
+-rw-rw-rw-   0        0        0     4379 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/framework/resource/manager.py
+-rw-rw-rw-   0        0        0     1719 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/framework/resource/resource.py
+-rw-rw-rw-   0        0        0     2114 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/framework/run.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.244321 concopilot-0.0.5/concopilot/framework/storage/
+-rw-rw-rw-   0        0        0       88 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/framework/storage/__init__.py
+-rw-rw-rw-   0        0        0     3219 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/framework/storage/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.264267 concopilot-0.0.5/concopilot/package/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/package/__init__.py
+-rw-rw-rw-   0        0        0     2082 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/package/captcha.py
+-rw-rw-rw-   0        0        0     1172 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/package/check.py
+-rw-rw-rw-   0        0        0     7065 2023-12-04 12:16:36.000000 concopilot-0.0.5/concopilot/package/config.py
+-rw-rw-rw-   0        0        0    14362 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/package/conpack.py
+-rw-rw-rw-   0        0        0      526 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/package/encrypt.py
+-rw-rw-rw-   0        0        0      654 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/package/error.py
+-rw-rw-rw-   0        0        0    11760 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/package/repo.py
+-rw-rw-rw-   0        0        0     4355 2023-11-14 13:08:35.000000 concopilot-0.0.5/concopilot/package/request.py
+-rw-rw-rw-   0        0        0     2149 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/package/transfer.py
+-rw-rw-rw-   0        0        0     3089 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/package/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.277231 concopilot-0.0.5/concopilot/util/
+-rw-rw-rw-   0        0        0       93 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/util/__init__.py
+-rw-rw-rw-   0        0        0     2698 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/util/class_dict.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.281221 concopilot-0.0.5/concopilot/util/config/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/util/config/__init__.py
+-rw-rw-rw-   0        0        0      757 2023-12-04 12:16:36.000000 concopilot-0.0.5/concopilot/util/config/tool.py
+-rw-rw-rw-   0        0        0      882 2023-11-09 05:34:47.000000 concopilot-0.0.5/concopilot/util/config/versions.py
+-rw-rw-rw-   0        0        0     1227 2024-03-18 12:46:15.000000 concopilot-0.0.5/concopilot/util/dicts.py
+-rw-rw-rw-   0        0        0      121 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/util/error.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.287204 concopilot-0.0.5/concopilot/util/initializer/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot-0.0.5/concopilot/util/initializer/__init__.py
+-rw-rw-rw-   0        0        0     3863 2024-04-08 10:42:49.000000 concopilot-0.0.5/concopilot/util/initializer/component.py
+-rw-rw-rw-   0        0        0     1966 2024-04-26 09:42:57.000000 concopilot-0.0.5/concopilot/util/interruptable_queue.py
+-rw-rw-rw-   0        0        0      486 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/util/jsons.py
+-rw-rw-rw-   0        0        0      372 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/util/singleton.py
+-rw-rw-rw-   0        0        0      241 2024-02-24 15:01:00.000000 concopilot-0.0.5/concopilot/util/yamls.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:32:11.289201 concopilot-0.0.5/concopilot.egg-info/
+-rw-rw-rw-   0        0        0     9844 2024-04-28 02:32:11.000000 concopilot-0.0.5/concopilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3278 2024-04-28 02:32:11.000000 concopilot-0.0.5/concopilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 02:32:11.000000 concopilot-0.0.5/concopilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-28 02:32:11.000000 concopilot-0.0.5/concopilot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2024-04-28 02:32:11.000000 concopilot-0.0.5/concopilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-28 02:32:11.000000 concopilot-0.0.5/concopilot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      877 2024-04-04 12:44:18.000000 concopilot-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 02:32:11.292190 concopilot-0.0.5/setup.cfg
```

### Comparing `concopilot-0.0.4/LICENSE` & `concopilot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/PKG-INFO` & `concopilot-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concopilot
-Version: 0.0.4
+Version: 0.0.5
 Summary: ConCopilot defines standards and common interfaces that would be helpful to make each part of a copilot reusable, replaceable, portable, and flexible.
 Author-email: ZHONG Weikun <zhong.weikun@live.com>
 Project-URL: Homepage, https://github.com/ConCopilot/concopilot
 Project-URL: Bug Tracker, https://github.com/ConCopilot/concopilot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `concopilot-0.0.4/README.md` & `concopilot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/basic/interface/cmd/interface.py` & `concopilot-0.0.5/concopilot/basic/interface/cmd/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # -*- coding: utf-8 -*-
 
 import json
 
 from typing import Dict, Optional
 
-from ....framework.interface import UserInterface
+from ....framework.interface import AgentDrivenSimplexUserInterface
 from ....framework.message import Message
 from ....package.config import Settings
 from ....util.jsons import JsonEncoder
 
 
 settings=Settings()
 
 
-class CmdUserInterface(UserInterface):
+class CmdUserInterface(AgentDrivenSimplexUserInterface):
     def __init__(self, config: Dict):
         super(CmdUserInterface, self).__init__(config)
         self.user_msg_prefix: str = self.config.config.user_msg_prefix if self.config.config.user_msg_prefix else ''
         self.user_msg_suffix: str = self.config.config.user_msg_suffix if self.config.config.user_msg_suffix else ''
         self.non_user_msg_prefix: str = self.config.config.non_user_msg_prefix if self.config.config.non_user_msg_prefix else ''
         self.non_user_msg_suffix: str = self.config.config.non_user_msg_suffix if self.config.config.non_user_msg_suffix else ''
         self.multiple_line_input: bool = self.config.config.multiple_line_input
 
         self.last_sender=None
         self.last_receiver=None
 
-    def send_msg_user(self, msg: Message):
+    def send_msg_to_user(self, msg: Message):
         print(self.non_user_msg_prefix)
         if msg.content:
             if isinstance(msg.content, str):
                 print(msg.content)
             else:
                 print(json.dumps(msg, cls=JsonEncoder, ensure_ascii=False, indent=4))
         else:
             print('')
         print(self.non_user_msg_suffix)
         self.last_sender=msg.sender
         self.last_receiver=msg.receiver
 
-    def on_msg_user(self, msg: Message) -> Optional[Message]:
-        self.send_msg_user(msg)
+    def on_msg_to_user(self, msg: Message) -> Optional[Message]:
+        self.send_msg_to_user(msg)
         return self.wait_user_msg()
 
     def has_user_msg(self) -> bool:
         return False
 
     def get_user_msg(self) -> Optional[Message]:
         return None
@@ -65,7 +65,14 @@
         while True:
             line=input()
             if line:
                 texts.append(line)
             if not self.multiple_line_input or not line:
                 break
         return '\n'.join(texts)
+
+    def interrupt(self):
+        pass
+
+    @property
+    def interrupted(self) -> bool:
+        return False
```

### Comparing `concopilot-0.0.4/concopilot/basic/message/manager/jsonmanager/manager.py` & `concopilot-0.0.5/concopilot/basic/message/manager/jsonmanager/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 # -*- coding: utf-8 -*-
 
 import json
 import re
 import regex
+import uuid
 import logging
 
-from typing import List, Dict, Tuple, Any, Optional
+from typing import List, Dict, Tuple, Any, Union, Optional
 
 from .....framework.message import Message
 from .....framework.message.manager import MessageManager
 from .....framework.cerebrum import InteractResponse
 from .....framework.identity import Identity
 from .....package.config import Settings
 
+
 settings=Settings()
 logger=logging.getLogger(__file__)
 
 
 class BasicJsonMessageManager(MessageManager):
     def __init__(self, config: Dict):
         super(BasicJsonMessageManager, self).__init__(config)
 
-    def parse(self, response: InteractResponse) -> List[Message]:
+    def parse(self, response: InteractResponse, thrd_id: Union[uuid.UUID, str, int] = None) -> List[Message]:
         msg_list=[]
         if response.content:
             try:
                 reply=fix_json_using_multiple_techniques(response.content)
                 if isinstance(reply, List):
                     for item in reply:
-                        msg_list.append(BasicJsonMessageManager.parse_as_msg(item))
+                        msg_list.append(BasicJsonMessageManager.parse_as_msg(item, thrd_id=thrd_id))
                 else:
-                    msg_list.append(BasicJsonMessageManager.parse_as_msg(reply))
+                    msg_list.append(BasicJsonMessageManager.parse_as_msg(reply, thrd_id=thrd_id))
             except Exception as e:
                 logger.warning('response.content parse failed!', exc_info=e)
-                msg_list.append(Message(content=response.content))
+                msg_list.append(Message(content=response.content, thrd_id=thrd_id))
         if response.plugin_calls:
             for plugin_call in response.plugin_calls:
                 content=Message.Command(**plugin_call)
                 msg_list.append(Message(
                     receiver=Identity(
                         role='plugin',
                         name=content.pop('plugin_name', None)
                     ),
                     content_type='command',
                     content=content,
-                    time=settings.current_time()
+                    time=settings.current_time(),
+                    thrd_id=thrd_id
                 ))
         return msg_list
 
     @staticmethod
-    def parse_as_msg(item: Any):
+    def parse_as_msg(item: Any, thrd_id: Union[uuid.UUID, str, int] = None):
         sender=None
         receiver=None
         content_type=None
         time=None
         if isinstance(item, Dict):
             sender=item.pop('sender', None)
             receiver=item.pop('receiver', None)
@@ -65,14 +68,15 @@
             item={}
         msg=Message(
             sender=sender,
             receiver=receiver,
             content_type=content_type,
             content=content,
             time=time if time else settings.current_time(),
+            thrd_id=thrd_id,
             **item
         )
         if msg.content_type is None and msg.content.command:
             msg.content_type='command'
         return msg
 
     def command(self, command_name: str, param: Any, **kwargs) -> Any:
```

### Comparing `concopilot-0.0.4/concopilot/basic/storage/disk/storage.py` & `concopilot-0.0.5/concopilot/basic/storage/disk/storage.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/asset/asset.py` & `concopilot-0.0.5/concopilot/framework/asset/asset.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/cerebrum/cerebrum.py` & `concopilot-0.0.5/concopilot/framework/cerebrum/cerebrum.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/context/context.py` & `concopilot-0.0.5/concopilot/framework/context/context.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/copilot.py` & `concopilot-0.0.5/concopilot/framework/copilot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 
 import abc
+import threading
 
-from typing import Dict, Any
+from typing import List, Dict, Any
 
 from .plugin import AbstractPlugin, PluginManager
 from .resource import ResourceManager
 from .cerebrum import Cerebrum
 from .storage import Storage
 from .interface import UserInterface
 from .message.manager import MessageManager
 from .interactor import Interactor
+from .resource import Resource
 from .context import Context
 from ..util.initializer import component
 from ..util import ClassDict
 
 
 class Copilot(AbstractPlugin):
     """
@@ -23,39 +25,52 @@
     All copilots implement the Plugin interface, so it is easy to use a copilot as a plugin in another copilot.
     """
 
     def __init__(self, config: Dict):
         """
         Configure the copilot without initialization.
 
-        Make sure the `type` in the config file is set to "copilot".
+        Make sure the `type` in the config file is set to "copilot" or "agent".
 
         :param config: configures read from its config file (default to "config.yaml")
         """
         super(Copilot, self).__init__(config)
-        assert self.type=='copilot'
+        assert self.type=='copilot' or self.type=='agent'
 
     @abc.abstractmethod
-    def initialize(self):
+    def config_copilot_resources(self):
+        pass
+
+    @abc.abstractmethod
+    def config_copilot_context(self):
+        pass
+
+    @property
+    @abc.abstractmethod
+    def copilot_context(self):
+        pass
+
+    @abc.abstractmethod
+    def initialize_copilot(self):
         """
         Initialize the framework and resources
         """
         pass
 
     @abc.abstractmethod
-    def finalize(self):
+    def finalize_copilot(self):
         """
-        Finalize the framework and resources
+        Finalize the framework and resources.
         """
         pass
 
     @abc.abstractmethod
     def run_interaction(self):
         """
-        Run the copilot interaction.
+        Run the copilot/agent interaction.
 
         This is the main logic of the copilot,
         so write your special task pipeline here.
         """
         pass
 
     @abc.abstractmethod
@@ -67,15 +82,15 @@
         """
         pass
 
     def command(self, command_name: str, param: Any, **kwargs) -> Any:
         """
         The Plugin command method.
 
-        Ignore this method if you are not expect your copilot acting as a plugin in other copilots,
+        Ignore this method if you are not expecting your copilot/agent acting as a plugin in other copilots/agents,
         or you have to override it as the same way of which in developing Plugins.
 
         :param command_name: command name
         :param param: command parameters
         :param kwargs: reserved, not recommend to use
         :return: the command result
         """
@@ -96,66 +111,109 @@
             self.config.config.interactor,
             self.resource_manager,
             self.cerebrum,
             self.plugin_manager,
             self.message_manager
         ) if self.config.config.interactor else None
 
+        self._outer_resources: List[Resource] = None
+        self._copilot_context: Context = None
+        self._running: threading.Event = threading.Event()
+        self._running_thrd: threading.Thread = None
+
     def config_resources(self, resource_manager: ResourceManager):
         super(BasicCopilot, self).config_resources(resource_manager)
+        if self.config.config.inherit_resources and resource_manager:
+            self._outer_resources=resource_manager.resources
+
+    def config_copilot_resources(self):
         if self.storage:
-            self.storage.config_resources(resource_manager)
+            self.storage.config_resources(self.resource_manager)
         if self.user_interface:
-            self.user_interface.config_resources(resource_manager)
+            self.user_interface.config_resources(self.resource_manager)
         if self.cerebrum:
-            self.cerebrum.config_resources(resource_manager)
+            self.cerebrum.config_resources(self.resource_manager)
         if self.plugin_manager:
-            self.plugin_manager.config_resources(resource_manager)
+            self.plugin_manager.config_resources(self.resource_manager)
         if self.message_manager:
-            self.message_manager.config_resources(resource_manager)
+            self.message_manager.config_resources(self.resource_manager)
         if self.interactor:
-            self.interactor.config_resources(resource_manager)
+            self.interactor.config_resources(self.resource_manager)
 
-    def config_context(self, context: Context):
-        super(BasicCopilot, self).config_context(context)
+    def config_copilot_context(self):
+        self._copilot_context=Context(
+            storage=self.storage,
+            assets=ClassDict(),
+            user_interface=self.user_interface
+        )
         if self.resource_manager:
-            self.resource_manager.config_context(context)
+            self.resource_manager.config_context(self._copilot_context)
         if self.storage:
-            self.storage.config_context(context)
+            self.storage.config_context(self._copilot_context)
         if self.user_interface:
-            self.user_interface.config_context(context)
+            self.user_interface.config_context(self._copilot_context)
         if self.cerebrum:
-            self.cerebrum.config_context(context)
+            self.cerebrum.config_context(self._copilot_context)
         if self.plugin_manager:
-            self.plugin_manager.config_context(context)
+            self.plugin_manager.config_context(self._copilot_context)
         if self.message_manager:
-            self.message_manager.config_context(context)
+            self.message_manager.config_context(self._copilot_context)
         if self.interactor:
-            self.interactor.config_context(context)
+            self.interactor.config_context(self._copilot_context)
 
-    def initialize(self):
+    @property
+    def copilot_context(self):
+        return self._copilot_context
+
+    def initialize_copilot(self):
         if self.resource_manager:
             self.resource_manager.initialize()
-            self.config_resources(self.resource_manager)
-        self.config_context(Context(
-            storage=self.storage,
-            assets=ClassDict(),
-            user_interface=self.user_interface
-        ))
+            if self.config.config.inherit_resources and self._outer_resources is not None:
+                for resource in self._outer_resources:
+                    self.resource_manager.add_resource(resource)
+            elif self.config.config.inherit_self_resources:
+                for resource in self.resources:
+                    self.resource_manager.add_resource(resource)
+            self.config_copilot_resources()
+        self.config_copilot_context()
+        if self.plugin_manager:
+            self.plugin_manager.initialize()
         if self.interactor:
             self.interactor.setup_prompts()
             self.interactor.setup_plugins()
 
-    def finalize(self):
+    def finalize_copilot(self):
+        if self.plugin_manager:
+            self.plugin_manager.finalize()
         if self.resource_manager:
             self.resource_manager.finalize()
 
     def run_interaction(self):
+        self._running.set()
         if self.interactor:
+            self.interactor.start()
             self.interactor.interact_loop()
         else:
             raise ValueError('No interactor configured!')
 
+    def initialize(self):
+        super(BasicCopilot, self).initialize()
+        self._running_thrd=threading.Thread(target=self.run)
+        self._running_thrd.start()
+        self._running.wait()
+
+    def finalize(self):
+        if self._running_thrd:
+            self._running.wait()
+            self.interactor.stop()
+            self.user_interface.interrupt()
+            self._running_thrd.join()
+        super(BasicCopilot, self).finalize()
+
     def run(self):
-        self.initialize()
+        self.initialize_copilot()
         self.run_interaction()
-        self.finalize()
+        self.finalize_copilot()
+
+
+Agent=Copilot
+BasicAgent=BasicCopilot
```

### Comparing `concopilot-0.0.4/concopilot/framework/interactor/interactor.py` & `concopilot-0.0.5/concopilot/framework/interactor/interactor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import abc
+import enum
 
 from typing import Dict, Any
 
 from ..plugin import AbstractPlugin, PluginManager
 from ..resource import ResourceManager
 from ..cerebrum import Cerebrum
 from ..message.manager import MessageManager
@@ -15,14 +16,21 @@
     An Interactor controls the information dispatching, task coordinating, and function calls in a copilot.
     It defines and controls the main working pipeline of specific copilots.
 
     During developing, generally,
     there's no need to implement `Copilot` interface for a new copilot, implement an `Interactor` interface instead.
     """
 
+    class Status(enum.IntEnum):
+        NOT_STARTED=0,
+        STARTING=1,
+        RUNNING=2,
+        STOPPING=3,
+        STOPPED=4
+
     def __init__(self, config: Dict):
         """
         Configure the Interactor without initialization.
 
         Make sure the `type` in the config file is set to "interactor".
 
         :param config: configures read from its config file (default to "config.yaml")
@@ -53,14 +61,50 @@
         """
         The main interaction loop.
 
         All main procedures of the interactor/copilot tasks should be defined here.
         """
         pass
 
+    @property
+    @abc.abstractmethod
+    def status(self) -> Status:
+        """
+        Return the status of the interactor.
+
+        Implementations should stop and exit the interaction loop when this method returns `STOPPING` or `STOPPED`.
+
+        :return: the status of the interactor
+        """
+        pass
+
+    @status.setter
+    @abc.abstractmethod
+    def status(self, value: Status):
+        """
+        The setter of the interactor status.
+
+        :param value: the value of the interactor status
+        """
+        pass
+
+    @abc.abstractmethod
+    def start(self):
+        """
+        Begin to start the interaction loop.
+        """
+        pass
+
+    @abc.abstractmethod
+    def stop(self):
+        """
+        Request to stop the interaction loop.
+        """
+        pass
+
     def command(self, command_name: str, param: Any, **kwargs) -> Any:
         return {}
 
 
 class BasicInteractor(Interactor, metaclass=abc.ABCMeta):
     def __init__(
         self,
@@ -72,12 +116,28 @@
     ):
         super(BasicInteractor, self).__init__(config)
         self.resource_manager: ResourceManager = resource_manager
         self.cerebrum: Cerebrum = cerebrum
         self.plugin_manager: PluginManager = plugin_manager
         self.message_manager: MessageManager = message_manager
 
+        self._status: Interactor.Status = Interactor.Status.NOT_STARTED
+
     def setup_prompts(self):
         self.plugin_manager.generate_prompt()
 
     def setup_plugins(self):
         self.cerebrum.setup_plugins(self.plugin_manager)
+
+    @property
+    def status(self) -> Interactor.Status:
+        return self._status
+
+    @status.setter
+    def status(self, value: Interactor.Status):
+        self._status=value
+
+    def start(self):
+        self.status=Interactor.Status.STARTING
+
+    def stop(self):
+        self.status=Interactor.Status.STOPPING
```

### Comparing `concopilot-0.0.4/concopilot/framework/interface/interface.py` & `concopilot-0.0.5/concopilot/framework/message/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,44 @@
 # -*- coding: utf-8 -*-
 
 import abc
+import uuid
 
-from typing import Dict, Optional, Any
+from typing import List, Dict, Union, Any
 
-from ..plugin import AbstractPlugin
 from ..message import Message
+from ..plugin import AbstractPlugin
+from ..cerebrum import InteractResponse
 
 
-class UserInterface(AbstractPlugin):
+class MessageManager(AbstractPlugin):
     """
-    The common interface to deal with interactions with user.
+    Translate the LLM natural language text from the Cerebrum response (`InteractResponse` type) into structured data (generally a `Dict`),
+    and encapsulate it with other information in the `InteractResponse` response into a Message for the main task pipeline.
+
+    The most popular form of this is to deserialize LLM json string into python `dict`.
     """
 
     def __init__(self, config: Dict):
         """
-        Configure the UserInterface without initialization.
+        Configure the MessageManager without initialization.
 
-        Make sure the `type` in the config file is set to "user_interface".
+        Make sure the `type` in the config file is set to "message_manager".
 
         :param config: configures read from its config file (default to "config.yaml")
         """
-        super(UserInterface, self).__init__(config)
-        assert self.type=='user_interface'
-
-    @abc.abstractmethod
-    def send_msg_user(self, msg: Message):
-        """
-        Send a message to the user.
-
-        :param msg: the message to be sent
-        """
-        pass
-
-    @abc.abstractmethod
-    def on_msg_user(self, msg: Message) -> Optional[Message]:
-        """
-        Send a message to the user and wait the user response.
-
-        This method must return the exact response to the input `msg`.
-        Implementations may need to take special mechanism to guarantee this.
-
-        :param msg: the message to be sent
-        :return: the message return by the user, None if the user want to stop the pipeline
-        """
-        pass
-
-    @abc.abstractmethod
-    def has_user_msg(self) -> bool:
-        """
-        Check if user has sent any message.
-
-        :return: True if there is any message from the user, otherwise False
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_user_msg(self) -> Optional[Message]:
-        """
-        Retrieve a new user message if any.
-
-        :return: the first message from the user, None if there is no user message currently
-        """
-        pass
+        super(MessageManager, self).__init__(config)
+        assert self.type=='message_manager'
 
     @abc.abstractmethod
-    def wait_user_msg(self) -> Optional[Message]:
+    def parse(self, response: InteractResponse, thrd_id: Union[uuid.UUID, str, int] = None) -> List[Message]:
         """
-        Wait for a new user message.
+        Parse the input `InteractResponse` object into a `Message` object.
 
-        :return: the first message from the user, None if the user want to stop the pipeline
+        :param response: the input InteractResponse generated by a Cerebrum
+        :param thrd_id: an optional thread id that the parsed messages belong to
+        :return: the passed information that encapsulated into a Message
         """
         pass
 
     def command(self, command_name: str, param: Any, **kwargs) -> Any:
         return {}
```

### Comparing `concopilot-0.0.4/concopilot/framework/message/message.py` & `concopilot-0.0.5/concopilot/framework/message/message.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/plugin/manager.py` & `concopilot-0.0.5/concopilot/framework/plugin/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,28 @@
 
     def config_context(self, context: Context):
         super(PluginManager, self).config_context(context)
         self.plugin_prompt_generator.config_context(context)
         for plugin in self.plugins:
             plugin.config_context(context)
 
+    def initialize(self):
+        """
+        Initialize all plugins.
+        """
+        for plugin in self.plugins:
+            plugin.initialize()
+
+    def finalize(self):
+        """
+        Finalize all plugins.
+        """
+        for plugin in self.plugins:
+            plugin.finalize()
+
     @abc.abstractmethod
     def generate_prompt(self):
         """
         Generate prompt for itself and managed plugins if necessary.
         """
         pass
```

### Comparing `concopilot-0.0.4/concopilot/framework/plugin/plugin.py` & `concopilot-0.0.5/concopilot/framework/plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,29 @@
         """
         Configure the context for this plugin, and for all components under this plugin if necessary.
 
         :param context: the input context.
         """
         pass
 
+    def initialize(self):
+        """
+        Initialize this plugin basing on its `config` property if necessary.
+
+        Developers should consider using `Resources` first,
+        because they can be shared across plugins.
+        """
+        pass
+
+    def finalize(self):
+        """
+        Finalize/Release this plugin if necessary.
+        """
+        pass
+
     @abc.abstractmethod
     def config_file_path(self, file_name: str = None) -> str:
         """
         Return the config file path with the given `file_name` of this plugin.
 
         The config file here is a general concept that indicates any file that is related to this plugin and has been pushed into the component repo.
 
@@ -170,15 +185,15 @@
     def resource_type_map(self) -> Dict[str, List['Resource']]:
         """
         :return: the plugin resource map arranged by the resource type
         """
         pass
 
     @abc.abstractmethod
-    def get_resource(self, *, resource_id: str = None, resource_name: str = None, resource_type: str = None) -> Optional['Resource']:
+    def get_resource(self, *, resource_id: Union[uuid.UUID, str, int] = None, resource_name: str = None, resource_type: str = None) -> Optional['Resource']:
         """
         Retrieve a resource with its resource id, resource name, and resource_type.
 
         if the `resource_id` is "default", it will be ignored.
 
         If the `resource_type` is provided alone, the first resource with the given resource type will be returned.
 
@@ -457,15 +472,16 @@
         content.pop('param', None)
         content.response=self.command(msg.content.command, msg.content.param)
         msg=Message(
             sender=Identity(role=msg.receiver.role, id=self.id, name=self.name),
             receiver=msg.sender,
             content_type='command',
             content=content,
-            time=settings.current_time()
+            time=settings.current_time(),
+            thrd_id=msg.thrd_id
         )
         return msg
 
     def has_msg(self) -> bool:
         return False
 
     def get_msg(self) -> Optional[Message]:
```

### Comparing `concopilot-0.0.4/concopilot/framework/plugin/promptgenerator.py` & `concopilot-0.0.5/concopilot/framework/plugin/promptgenerator.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/resource/category/disk.py` & `concopilot-0.0.5/concopilot/framework/resource/category/disk.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/resource/category/model.py` & `concopilot-0.0.5/concopilot/framework/resource/category/model.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/resource/manager.py` & `concopilot-0.0.5/concopilot/framework/resource/manager.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/resource/resource.py` & `concopilot-0.0.5/concopilot/framework/resource/resource.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/run.py` & `concopilot-0.0.5/concopilot/framework/run.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/framework/storage/storage.py` & `concopilot-0.0.5/concopilot/framework/storage/storage.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/captcha.py` & `concopilot-0.0.5/concopilot/package/captcha.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/check.py` & `concopilot-0.0.5/concopilot/package/check.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/config.py` & `concopilot-0.0.5/concopilot/package/config.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/conpack.py` & `concopilot-0.0.5/concopilot/package/conpack.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/encrypt.py` & `concopilot-0.0.5/concopilot/package/encrypt.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/error.py` & `concopilot-0.0.5/concopilot/package/error.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/repo.py` & `concopilot-0.0.5/concopilot/package/repo.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/request.py` & `concopilot-0.0.5/concopilot/package/request.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/transfer.py` & `concopilot-0.0.5/concopilot/package/transfer.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/package/validator.py` & `concopilot-0.0.5/concopilot/package/validator.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/util/class_dict.py` & `concopilot-0.0.5/concopilot/util/class_dict.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/util/config/tool.py` & `concopilot-0.0.5/concopilot/util/config/tool.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/util/config/versions.py` & `concopilot-0.0.5/concopilot/util/config/versions.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/util/dicts.py` & `concopilot-0.0.5/concopilot/util/dicts.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot/util/initializer/component.py` & `concopilot-0.0.5/concopilot/util/initializer/component.py`

 * *Files identical despite different names*

### Comparing `concopilot-0.0.4/concopilot.egg-info/PKG-INFO` & `concopilot-0.0.5/concopilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concopilot
-Version: 0.0.4
+Version: 0.0.5
 Summary: ConCopilot defines standards and common interfaces that would be helpful to make each part of a copilot reusable, replaceable, portable, and flexible.
 Author-email: ZHONG Weikun <zhong.weikun@live.com>
 Project-URL: Homepage, https://github.com/ConCopilot/concopilot
 Project-URL: Bug Tracker, https://github.com/ConCopilot/concopilot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `concopilot-0.0.4/concopilot.egg-info/SOURCES.txt` & `concopilot-0.0.5/concopilot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 concopilot.egg-info/requires.txt
 concopilot.egg-info/top_level.txt
 concopilot/basic/__init__.py
 concopilot/basic/copilot/__init__.py
 concopilot/basic/interface/__init__.py
 concopilot/basic/interface/cmd/__init__.py
 concopilot/basic/interface/cmd/interface.py
+concopilot/basic/interface/duplex/__init__.py
 concopilot/basic/message/__init__.py
 concopilot/basic/message/manager/__init__.py
 concopilot/basic/message/manager/jsonmanager/__init__.py
 concopilot/basic/message/manager/jsonmanager/manager.py
 concopilot/basic/message/manager/strmanager/__init__.py
 concopilot/basic/message/manager/strmanager/manager.py
 concopilot/basic/plugin/__init__.py
@@ -39,15 +40,17 @@
 concopilot/framework/context/__init__.py
 concopilot/framework/context/context.py
 concopilot/framework/identity/__init__.py
 concopilot/framework/identity/identity.py
 concopilot/framework/interactor/__init__.py
 concopilot/framework/interactor/interactor.py
 concopilot/framework/interface/__init__.py
+concopilot/framework/interface/duplex.py
 concopilot/framework/interface/interface.py
+concopilot/framework/interface/simplex.py
 concopilot/framework/message/__init__.py
 concopilot/framework/message/manager.py
 concopilot/framework/message/message.py
 concopilot/framework/plugin/__init__.py
 concopilot/framework/plugin/manager.py
 concopilot/framework/plugin/plugin.py
 concopilot/framework/plugin/promptgenerator.py
@@ -70,14 +73,15 @@
 concopilot/package/request.py
 concopilot/package/transfer.py
 concopilot/package/validator.py
 concopilot/util/__init__.py
 concopilot/util/class_dict.py
 concopilot/util/dicts.py
 concopilot/util/error.py
+concopilot/util/interruptable_queue.py
 concopilot/util/jsons.py
 concopilot/util/singleton.py
 concopilot/util/yamls.py
 concopilot/util/config/__init__.py
 concopilot/util/config/tool.py
 concopilot/util/config/versions.py
 concopilot/util/initializer/__init__.py
```

### Comparing `concopilot-0.0.4/pyproject.toml` & `concopilot-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="concopilot"
-version="0.0.4"
+version="0.0.5"
 authors=[
     {name="ZHONG Weikun", email="zhong.weikun@live.com"}
 ]
 description="ConCopilot defines standards and common interfaces that would be helpful to make each part of a copilot reusable, replaceable, portable, and flexible."
 readme="README.md"
 requires-python=">=3.8"
 classifiers = [
```

