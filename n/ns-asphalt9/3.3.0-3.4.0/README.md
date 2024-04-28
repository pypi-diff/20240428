# Comparing `tmp/ns_asphalt9-3.3.0.tar.gz` & `tmp/ns_asphalt9-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-3.3.0.tar", last modified: Sat Apr 13 06:58:54 2024, max compression
+gzip compressed data, was "ns_asphalt9-3.4.0.tar", last modified: Sun Apr 28 17:02:37 2024, max compression
```

## Comparing `ns_asphalt9-3.3.0.tar` & `ns_asphalt9-3.4.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.346037 ns_asphalt9-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-13 06:58:54.346037 ns_asphalt9-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.330037 ns_asphalt9-3.3.0/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.334037 ns_asphalt9-3.3.0/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.338037 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/autocode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.338037 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44295 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.342037 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/console.png
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/record.png
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward.png
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward3.png
--rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/screen.png
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20338 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/reset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.346037 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/error_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/online_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/page_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/thread_lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data_win.py
--rw-r--r--   0 runner    (1001) docker     (127)    15272 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.346037 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 06:58:54.000000 ns_asphalt9-3.3.0/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-13 06:58:54.346037 ns_asphalt9-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 06:58:54.346037 ns_asphalt9-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-13 06:58:48.000000 ns_asphalt9-3.3.0/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.814328 ns_asphalt9-3.4.0/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.818328 ns_asphalt9-3.4.0/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.822328 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/autocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.822328 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45507 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.822328 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/record.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/screen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20338 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/reset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/error_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/online_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/page_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/process_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/thread_lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_win.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-28 17:02:37.830328 ns_asphalt9-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/tests/test_pages.py
```

### Comparing `ns_asphalt9-3.3.0/LICENSE` & `ns_asphalt9-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/PKG-INFO` & `ns_asphalt9-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.3.0
+Version: 3.4.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.3.0/README.md` & `ns_asphalt9-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/actions/__init__.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/actions/autocode.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/autocode.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/process_race.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import json
 
 from .. import consts, globals, ocr
 from ..controller import Buttons, pro
 from ..utils.log import logger
 from ..utils.count import count
 from ..utils.track_navi_data import get_navi_data
-from ..utils.track_navi_data_v2 import track_navi_data as navi_data_v2
 from .common import get_race_mode
 
 
 def generate_random_filename():
     random_name = str(uuid.uuid4().hex)[:8]
     return random_name
 
@@ -29,38 +28,36 @@
 
 
 def race_worker(
     progress_manager, navi_data, pro, race_navi_event, race_worker_quit, track_name
 ):
     count = 0
     processed_progress = []
-    if track_name in navi_data_v2:
-        action_data = navi_data_v2[track_name]["data"]
-        version = 2
-    else:
-        action_data = navi_data
+    if isinstance(navi_data, list):
         version = 1
+    else:
+        version = 2
     while race_navi_event.is_set():
         if version == 2:
             progress = progress_manager.get_progress()
             progress = str(round(progress))
-            if progress in action_data and progress not in processed_progress:
-                buttons = action_data[progress]
+            if progress in navi_data and progress not in processed_progress:
+                buttons = navi_data[progress]
                 for button in buttons:
-                    if button["key"] in ["DPAD_LEFT", "DPAD_RIGHT", "Y"]:
+                    if button["key"] in ["DPAD_LEFT", "DPAD_RIGHT", "Y", "X"]:
                         pro.press_buttons(button["key"])
                     else:
                         pro.press_buttons(
                             button["key"], down=button["down"] / 1000, up=0.05
                         )
                 processed_progress.append(progress)
 
         else:
             progress = progress_manager.get_progress()
-            action, duration = get_action(progress, action_data)
+            action, duration = get_action(progress, navi_data)
             if action:
                 if action == "L":
                     pro.press_buttons(Buttons.DPAD_LEFT)
                 elif action == "R":
                     pro.press_buttons(Buttons.DPAD_RIGHT)
                 elif action == "LL":
                     pro.press_buttons([Buttons.DPAD_LEFT, Buttons.DPAD_LEFT])
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/cache.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/capture.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/capture.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/consts.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/event.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/event.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/globals.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from . import consts
 from .utils.thread_lifo_queue import LIFOQueue
 
 packet_queue = queue.Queue()
 
 input_packet = {}
 
+progress_data = []
+
 input_queue = queue.Queue()
 output_queue = queue.Queue()
 notify_queue = queue.Queue()
 
 frame_queue = LIFOQueue()
 
 task_queue = queue.Queue()
@@ -19,14 +21,16 @@
 
 CONFIG = None
 
 # 回放停止事件
 G_REPLAY_RUN = threading.Event()
 G_REPLAY_STOP = threading.Event()
 
+G_OCR_PROGRESS = threading.Event()
+
 # 程序运行
 G_RUN = threading.Event()
 
 #
 G_OUT_WORKER = threading.Event()
 
 # 退出循环事件
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 import os
 import tkinter
+import time
+
 import cv2
 from collections import OrderedDict
 
 import customtkinter
 from PIL import Image, ImageTk
 
 
@@ -452,24 +454,36 @@
         def on_key_press(event):
             self.show(f"On key press, key = {event.char}, {event.keysym}")
             key = keysym_mapping.get(event.keysym, event.keysym)
             if key in key_pro_mapping:
                 button: Button = pro_buttons.get(key_pro_mapping[key], None)
                 if button:
                     button._on_enter()
-                    self.queue.put({"action": "press", "key": key})
+                    self.queue.put(
+                        {
+                            "action": "press",
+                            "key": key,
+                            "timestamp": time.time_ns() // 10**6,
+                        }
+                    )
 
         def on_key_release(event):
             self.show(f"On key release, key = {event.char} {event.keysym}")
             key = keysym_mapping.get(event.keysym, event.keysym)
             if key in key_pro_mapping:
                 button: Button = pro_buttons.get(key_pro_mapping[key], None)
                 if button:
                     button._on_leave()
-                    self.queue.put({"action": "release", "key": key})
+                    self.queue.put(
+                        {
+                            "action": "release",
+                            "key": key,
+                            "timestamp": time.time_ns() // 10**6,
+                        }
+                    )
                     # self.queue.put(key)
 
         self.key_label.bind("<KeyRelease>", on_key_release)
         self.key_label.bind("<KeyPress>", on_key_press)
 
     def _build_record(self):
         self.record_frame = customtkinter.CTkFrame(
@@ -490,31 +504,56 @@
             )
 
         record_group_frame = customtkinter.CTkFrame(self.record_frame, width=450)
         record_group_frame.grid(
             row=0, column=1, padx=(20, 20), pady=(20, 20), sticky="nsew"
         )
 
+        label = customtkinter.CTkLabel(master=record_group_frame, text="选择模式:")
+        label.grid(
+            row=0,
+            column=1,
+            columnspan=1,
+            padx=20,
+            pady=20,
+            sticky="",
+        )
+
+        self.record_mode_option = customtkinter.CTkOptionMenu(
+            record_group_frame,
+            dynamic_resizing=False,
+            values=["普通", "导航"],
+            width=120,
+            height=28,
+            button_color="black",
+            fg_color="black",
+            text_color="white",
+            button_hover_color=("gray70", "gray30"),
+            command=self.save_settings,
+        )
+        self.record_mode_option.grid(row=0, column=2, padx=(20, 20), pady=(20, 20))
+
         def start_record(**kwargs):
-            self.queue.put("start_record")
+            mode = self.record_mode_option.get()
+            self.queue.put(f"start_record {mode}")
 
         self.record_start_button = Button(
             record_group_frame,
             text="开始录制",
             fg_color="black",
             text_color="white",
             hover_color=("gray70", "gray30"),
             corner_radius=40,
             height=20,
             width=20,
             state="normal",
             command=start_record,
         )
         self.record_start_button.grid(
-            row=0, column=1, padx=(20, 20), pady=(20, 20), sticky="ew"
+            row=1, column=1, padx=(20, 20), pady=(20, 20), sticky="ew"
         )
 
         def stop_record(**kwargs):
             self.queue.put("stop_record")
             self.replay_file_option.destroy()
             self.replay_file_option = customtkinter.CTkOptionMenu(
                 replay_group_frame,
@@ -539,15 +578,15 @@
             corner_radius=40,
             height=20,
             width=20,
             state="normal",
             command=stop_record,
         )
         self.record_stop_button.grid(
-            row=0, column=2, padx=(20, 20), pady=(20, 20), sticky="ew"
+            row=1, column=2, padx=(20, 20), pady=(20, 20), sticky="ew"
         )
 
         replay_group_frame = customtkinter.CTkFrame(self.record_frame, width=450)
         replay_group_frame.grid(
             row=1, column=1, padx=(20, 20), pady=(20, 20), sticky="ew"
         )
 
@@ -580,15 +619,14 @@
             fg_color="black",
             text_color="white",
             button_hover_color=("gray70", "gray30"),
             command=self.save_settings,
         )
         self.replay_file_option.grid(row=1, column=2, padx=(20, 20), pady=(20, 20))
 
-
         label = customtkinter.CTkLabel(master=replay_group_frame, text="执行次数:")
         label.grid(
             row=2,
             column=1,
             columnspan=1,
             padx=20,
             pady=20,
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/console.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/console.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/record.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/record.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward1.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward1.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward2.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward2.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward3.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward3.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/screen.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/screen.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/ocr.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/pages.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/reset_data.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/reset_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/tasks.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/test.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/test.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/count.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/count.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/credits.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/credits.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/error_process.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/error_process.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/lifo_queue.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/notify.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/notify.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/online_tracker.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/online_tracker.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/page_stack.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/page_stack.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/thread_lifo_queue.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/thread_lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import json
 
 from .track_navi_data_update import data as updated_navi_data
 from .track_navi_data_win import track_navi_data
+from .track_navi_data_v2 import track_navi_data as track_navi_data_v2
 
 
 def get_navi_data(name):
     navi_data = []
     data = None
 
     try:
         with open("navi_data.json", "r") as file:
             custom_navi_data = json.load(file)
     except Exception as e:
         custom_navi_data = {}
 
+    # win端转换数据
     if name in track_navi_data:
         data = track_navi_data[name]
+    # 根据ns端更新数据
     if name in updated_navi_data:
         data = updated_navi_data[name]
+    # 第二版本数据
+    if name in track_navi_data_v2:
+        data = track_navi_data_v2[name]
+    # 自定义数据
     if name in custom_navi_data:
         data = custom_navi_data[name]
     if data:
+        if "L" not in data:
+            return data
         for k in data["L"]:
             navi_data.append((k, "L", 0))
         for k in data["R"]:
             navi_data.append((k, "R", 0))
 
         for extra in ["LL", "RR", "B", "BB", "YY-1", "YY-2", "YY-3"]:
             if extra in data:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data_update.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_update.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data_v2.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,90 +1,85 @@
 track_navi_data = {
     "GOLD RUSH": {
         "trackcn": "淘金狂飙",
-        "data": {
-            "2": [{"key": "Y", "down": 63}, {"key": "Y", "down": 124}],
-            "14": [{"key": "DPAD_LEFT", "down": 85}],
-            "15": [{"key": "DPAD_LEFT", "down": 85}],
-            "17": [{"key": "Y", "down": 113}, {"key": "Y", "down": 84}],
-            "28": [{"key": "B", "down": 8582}],
-            "42": [{"key": "Y", "down": 133}, {"key": "Y", "down": 106}],
-            "44": [{"key": "B", "down": 1453}],
-            "47": [{"key": "DPAD_LEFT", "down": 130}],
-            "48": [{"key": "DPAD_LEFT", "down": 130}],
-            "50": [{"key": "Y", "down": 128}, {"key": "Y", "down": 84}],
-            "65": [{"key": "DPAD_RIGHT", "down": 103}],
-            "66": [{"key": "DPAD_RIGHT", "down": 103}],
-            "69": [{"key": "Y", "down": 132}, {"key": "Y", "down": 87}],
-            "76": [{"key": "DPAD_LEFT", "down": 75}],
-            "77": [{"key": "DPAD_LEFT", "down": 75}],
-            "88": [{"key": "B", "down": 2933}],
-            "93": [{"key": "Y", "down": 123}, {"key": "Y", "down": 101}],
-        },
+        "2": [{"key": "Y", "down": 63}, {"key": "Y", "down": 124}],
+        "14": [{"key": "DPAD_LEFT", "down": 85}],
+        "15": [{"key": "DPAD_LEFT", "down": 85}],
+        "17": [{"key": "Y", "down": 113}, {"key": "Y", "down": 84}],
+        "28": [{"key": "B", "down": 8582}],
+        "42": [{"key": "Y", "down": 133}, {"key": "Y", "down": 106}],
+        "44": [{"key": "B", "down": 1453}],
+        "47": [{"key": "DPAD_LEFT", "down": 130}],
+        "48": [{"key": "DPAD_LEFT", "down": 130}],
+        "50": [{"key": "Y", "down": 128}, {"key": "Y", "down": 84}],
+        "65": [{"key": "DPAD_RIGHT", "down": 103}],
+        "66": [{"key": "DPAD_RIGHT", "down": 103}],
+        "69": [{"key": "Y", "down": 132}, {"key": "Y", "down": 87}],
+        "76": [{"key": "DPAD_LEFT", "down": 75}],
+        "77": [{"key": "DPAD_LEFT", "down": 75}],
+        "88": [{"key": "B", "down": 2933}],
+        "93": [{"key": "Y", "down": 123}, {"key": "Y", "down": 101}],
     },
     "ANCIENT RUINS": {
         "trackcn": "古代遗迹",
-        "data": {
-            "1": [{"key": "DPAD_RIGHT", "down": 109}],
-            "2": [{"key": "DPAD_RIGHT", "down": 109}],
-            "4": [{"key": "DPAD_RIGHT", "down": 107}],
-            "5": [{"key": "DPAD_RIGHT", "down": 107}],
-            "8": [{"key": "Y", "down": 47}, {"key": "Y", "down": 116}],
-            "15": [{"key": "DPAD_RIGHT", "down": 100}],
-            "16": [{"key": "DPAD_RIGHT", "down": 100}],
-            "27": [{"key": "Y", "down": 78}, {"key": "Y", "down": 104}],
-            "29": [
-                {"key": "DPAD_RIGHT", "down": 204},
-                {"key": "Y", "down": 78},
-                {"key": "Y", "down": 104},
-            ],
-            "30": [{"key": "DPAD_RIGHT", "down": 204}],
-            "33": [{"key": "DPAD_LEFT", "down": 178}],
-            "34": [{"key": "DPAD_LEFT", "down": 178}],
-            "38": [{"key": "DPAD_LEFT", "down": 94}],
-            "39": [{"key": "DPAD_LEFT", "down": 94}],
-            "41": [{"key": "Y", "down": 118}, {"key": "Y", "down": 102}],
-            "51": [{"key": "B", "down": 10093}],
-            "65": [{"key": "Y", "down": 150}, {"key": "Y", "down": 126}],
-            "67": [{"key": "DPAD_LEFT", "down": 196}],
-            "68": [{"key": "DPAD_LEFT", "down": 196}],
-            "69": [{"key": "B", "down": 2116}],
-            "74": [{"key": "Y", "down": 133}, {"key": "Y", "down": 108}],
-            "77": [{"key": "B", "down": 1545}],
-            "80": [{"key": "Y", "down": 137}, {"key": "Y", "down": 111}],
-            "83": [{"key": "B", "down": 1814}],
-            "87": [{"key": "Y", "down": 151}, {"key": "Y", "down": 96}],
-            "89": [{"key": "DPAD_LEFT", "down": 150}],
-            "90": [{"key": "DPAD_LEFT", "down": 150}],
-            "92": [{"key": "B", "down": 2148}],
-            "96": [{"key": "Y", "down": 129}, {"key": "Y", "down": 109}],
-        },
+        "1": [{"key": "DPAD_RIGHT", "down": 109}],
+        "2": [{"key": "DPAD_RIGHT", "down": 109}],
+        "4": [{"key": "DPAD_RIGHT", "down": 107}],
+        "5": [{"key": "DPAD_RIGHT", "down": 107}],
+        "8": [{"key": "Y", "down": 47}, {"key": "Y", "down": 116}],
+        "15": [{"key": "DPAD_RIGHT", "down": 100}],
+        "16": [{"key": "DPAD_RIGHT", "down": 100}],
+        "27": [{"key": "Y", "down": 78}, {"key": "Y", "down": 104}],
+        "29": [
+            {"key": "DPAD_RIGHT", "down": 204},
+            {"key": "Y", "down": 78},
+            {"key": "Y", "down": 104},
+        ],
+        "30": [{"key": "DPAD_RIGHT", "down": 204}],
+        "33": [{"key": "DPAD_LEFT", "down": 178}],
+        "34": [{"key": "DPAD_LEFT", "down": 178}],
+        "38": [{"key": "DPAD_LEFT", "down": 94}],
+        "39": [{"key": "DPAD_LEFT", "down": 94}],
+        "41": [{"key": "Y", "down": 118}, {"key": "Y", "down": 102}],
+        "51": [{"key": "B", "down": 10093}],
+        "65": [{"key": "Y", "down": 150}, {"key": "Y", "down": 126}],
+        "67": [{"key": "DPAD_LEFT", "down": 196}],
+        "68": [{"key": "DPAD_LEFT", "down": 196}],
+        "69": [{"key": "B", "down": 2116}],
+        "74": [{"key": "Y", "down": 133}, {"key": "Y", "down": 108}],
+        "77": [{"key": "B", "down": 1545}],
+        "80": [{"key": "Y", "down": 137}, {"key": "Y", "down": 111}],
+        "83": [{"key": "B", "down": 1814}],
+        "87": [{"key": "Y", "down": 151}, {"key": "Y", "down": 96}],
+        "89": [{"key": "DPAD_LEFT", "down": 150}],
+        "90": [{"key": "DPAD_LEFT", "down": 150}],
+        "92": [{"key": "B", "down": 2148}],
+        "96": [{"key": "Y", "down": 129}, {"key": "Y", "down": 109}],
+
     },
     "NANJING STROLL": {
         "trackcn": "漫步南京路",
-        "data": {
-            "0": [{"key": "DPAD_RIGHT", "down": 76}, {"key": "DPAD_RIGHT", "down": 76}],
-            "1": [{"key": "Y", "down": 112}, {"key": "Y", "down": 75}],
-            "22": [{"key": "Y", "down": 80}, {"key": "Y", "down": 75}],
-            "29": [{"key": "B", "down": 1831}],
-            "34": [{"key": "Y", "down": 138}, {"key": "Y", "down": 100}],
-            "37": [{"key": "B", "down": 11499}],
-            "54": [{"key": "Y", "down": 118}, {"key": "Y", "down": 86}],
-            "56": [{"key": "B", "down": 3389}],
-            "60": [{"key": "Y", "down": 108}, {"key": "Y", "down": 90}],
-            "66": [{"key": "B", "down": 2522}],
-            "70": [
-                {"key": "DPAD_LEFT", "down": 185},
-                {"key": "DPAD_LEFT", "down": 185},
-            ],
-            "72": [{"key": "Y", "down": 102}, {"key": "Y", "down": 82}],
-            "74": [{"key": "B", "down": 2690}],
-            "78": [{"key": "Y", "down": 114}, {"key": "Y", "down": 88}],
-            "82": [{"key": "B", "down": 3026}],
-            "87": [{"key": "Y", "down": 134}, {"key": "Y", "down": 87}],
-            "89": [{"key": "B", "down": 1406}],
-            "91": [{"key": "Y", "down": 138}, {"key": "Y", "down": 98}],
-            "93": [{"key": "B", "down": 1364}],
-            "96": [{"key": "Y", "down": 102}, {"key": "Y", "down": 87}],
-        },
+        "0": [{"key": "DPAD_RIGHT", "down": 76}, {"key": "DPAD_RIGHT", "down": 76}],
+        "1": [{"key": "Y", "down": 112}, {"key": "Y", "down": 75}],
+        "22": [{"key": "Y", "down": 80}, {"key": "Y", "down": 75}],
+        "29": [{"key": "B", "down": 1831}],
+        "34": [{"key": "Y", "down": 138}, {"key": "Y", "down": 100}],
+        "37": [{"key": "B", "down": 11499}],
+        "54": [{"key": "Y", "down": 118}, {"key": "Y", "down": 86}],
+        "56": [{"key": "B", "down": 3389}],
+        "60": [{"key": "Y", "down": 108}, {"key": "Y", "down": 90}],
+        "66": [{"key": "B", "down": 2522}],
+        "70": [
+            {"key": "DPAD_LEFT", "down": 185},
+            {"key": "DPAD_LEFT", "down": 185},
+        ],
+        "72": [{"key": "Y", "down": 102}, {"key": "Y", "down": 82}],
+        "74": [{"key": "B", "down": 2690}],
+        "78": [{"key": "Y", "down": 114}, {"key": "Y", "down": 88}],
+        "82": [{"key": "B", "down": 3026}],
+        "87": [{"key": "Y", "down": 134}, {"key": "Y", "down": 87}],
+        "89": [{"key": "B", "down": 1406}],
+        "91": [{"key": "Y", "down": 138}, {"key": "Y", "down": 98}],
+        "93": [{"key": "B", "down": 1364}],
+        "96": [{"key": "Y", "down": 102}, {"key": "Y", "down": 87}], 
     },
 }
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/core/utils/track_navi_data_win.py` & `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_win.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9/main.py` & `ns_asphalt9-3.4.0/ns_asphalt9/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,35 +6,43 @@
 import threading
 import time
 import traceback
 import types
 import inspect
 import cv2
 import re
-
-from PIL import Image
+import json
 
 from .core import consts, errors
 from .core import globals as G
+from .core.actions import *  # noqa
 from .core.controller import pro
 from .core.gui.app import App
 from .core.ocr import OCR
 from .core.pages import Page
 from .core.tasks import TaskManager
 from .core.utils.log import logger
 from .core.utils.online_tracker import online_tracker
 from .core.utils.notify import Notify
-from .core.actions import *  # noqa
 from .core.utils.page_stack import page_stack
+from .core.utils.process_record_data import (
+    filter_navi_data,
+    to_navi_data,
+    to_record_data,
+)
 from .core.event import Event
-from .core.reset_data import reset_data
 
 
 G.input_packet["packet"] = pro.nx.create_input_packet()
 
+
+def timestamp():
+    return time.time_ns() // 10**6
+
+
 def process_screen(page: Page):
     """根据显示内容执行动作"""
 
     page_stack.add_item(page.name)
     if page.name != consts.empty and page.action:
         page.call_action()
 
@@ -77,16 +85,16 @@
 
     TaskManager.destroy()
     G.G_RACE_QUIT_EVENT.set()
 
 
 def command_input(queue):
     record = False
+    record_mode = None
     record_data = []
-    last_button_time = 0
 
     while G.G_RUN.is_set():
         command = queue.get()
         logger.info(f"Get command from queue: {command}")
         if isinstance(command, str):
             if command == "stop":
                 # 停止挂机
@@ -116,47 +124,131 @@
                 logger.info(f"G_RUN status = {G.G_RUN.is_set()}")
                 for timer in TaskManager.timers:
                     timer.cancel()
 
             elif command == "ocr":
                 OCR.get_page()
 
-            elif command == "start_record":
+            elif "start_record" in command:
+                _, record_mode = command.split(" ")
+                if record_mode == "导航":
+                    G.G_OCR_PROGRESS.set()
+                    start_ocr_progress_worker()
                 record = True
                 record_data = []
 
             elif command == "stop_record":
+                if record_mode == "导航":
+                    G.G_OCR_PROGRESS.clear()
                 record = False
                 if record_data:
                     if not os.path.exists("./record"):
                         os.makedirs("record")
-                    filename = f"record_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.py"
-                    with open(os.path.join("./record", filename), "w") as file:
-                        file.writelines(record_data)
+                    merge_data = filter_navi_data(record_data)
+                    if record_mode == "导航":
+                        record_data = to_navi_data(merge_data)
+                        filename = f"record_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.json"
+                        with open(os.path.join("./record", filename), "w") as file:
+                            file.write(json.dumps(record_data, indent=2))
+                    else:
+                        record_data = to_record_data(merge_data)
+                        filename = f"record_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.py"
+                        with open(os.path.join("./record", filename), "w") as file:
+                            file.writelines(record_data)
                     record_data = []
+
             elif "start_replay" in command:
                 _, filename, replay_times = command.split(" ")
                 logger.info(f"开始回放 {filename} 回放次数 {replay_times}")
-                with open(os.path.join("./record", filename)) as file:
-                    replay_text = file.read()
 
-                def replay_worker(replay_text, replay_times):
-                    try:
-                        for index in range(int(replay_times)):
-                            logger.info(f"回放次数: {index + 1}")
-                            exec(replay_text)
-                    except errors.ReplayStopException:
-                        logger.info("回放停止")
-                    logger.info("回放结束")
+                if filename.endswith(".py"):
+                    with open(os.path.join("./record", filename)) as file:
+                        replay_text = file.read()
+
+                    def replay_worker(replay_text, replay_times):
+                        try:
+                            for index in range(int(replay_times)):
+                                if not G.G_REPLAY_RUN.is_set():
+                                    break
+                                logger.info(f"回放次数: {index + 1}")
+                                exec(replay_text)
+                        except errors.ReplayStopException:
+                            logger.info("回放停止")
+                        logger.info("回放结束")
+
+                    G.G_REPLAY_RUN.set()
+                    t = threading.Thread(
+                        target=replay_worker,
+                        args=(replay_text, replay_times),
+                        daemon=True,
+                    )
+                    t.start()
 
-                t = threading.Thread(target=replay_worker, args=(replay_text, replay_times), daemon=True)
-                t.start()
+                else:
+                    with open(os.path.join("./record", filename)) as file:
+                        navi_data = json.load(file)
+                    logger.info(f"Load navi data {navi_data}")
+
+                    def replay_navi_worker(navi_data):
+                        processed_data = []
+                        showed_progress = [-1]
+                        last_button = None
+
+                        while True:
+                            if not G.G_REPLAY_RUN.is_set():
+                                break
+
+                            progress = G.progress_data[-1]["progress"]
+
+                            if progress not in showed_progress:
+                                logger.info(f"Get progress from screen_data {progress}")
+                                if (
+                                    progress - showed_progress[-1] >= 5
+                                    and last_button != "B"
+                                ):
+                                    continue
+                                showed_progress.append(progress)
+                            if (
+                                str(progress) in navi_data
+                                and progress not in processed_data
+                            ):
+                                buttons = navi_data[str(progress)]
+                                for button in buttons:
+                                    logger.debug(f"Press button {button}")
+                                    if button["key"] in [
+                                        "DPAD_LEFT",
+                                        "DPAD_RIGHT",
+                                        "Y",
+                                        "X",
+                                    ]:
+                                        pro.press_buttons(button["key"])
+                                    else:
+                                        pro.press_buttons(
+                                            button["key"],
+                                            down=button["down"] / 1000,
+                                            up=0.05,
+                                        )
+
+                                    last_button = button["key"]
+                                processed_data.append(progress)
+                            if progress >= 98:
+                                break
+
+                    G.G_REPLAY_RUN.set()
+                    G.G_OCR_PROGRESS.set()
+                    start_ocr_progress_worker()
+                    t = threading.Thread(
+                        target=replay_navi_worker, args=(navi_data,), daemon=True
+                    )
+                    t.start()
 
             elif "stop_replay" == command:
-                G.G_REPLAY_STOP.set()
+                # G.G_REPLAY_STOP.set()
+                G.G_REPLAY_RUN.clear()
+                G.G_OCR_PROGRESS.clear()
 
             elif "code" in command:
                 from .core.actions.autocode import enter_code, batch_enter_code
 
                 if command == "batch_code":
                     batch_enter_code()
                 else:
@@ -205,23 +297,16 @@
                     and not inspect.isclass(obj)
                 }
                 for name, doc in non_builtin_functions.items():
                     lines.append(f"{name}: {doc}")
                 logger.info("\n".join(lines))
 
             elif command in consts.KEY_MAPPING:
-                # 手柄操作
+                # 鼠标操作手柄
                 control_data = consts.KEY_MAPPING.get(command)
-                if record:
-                    if last_button_time:
-                        current_button_time = time.time()
-                        duration = round(current_button_time - last_button_time, 2)
-                        record_data.append(f"time.sleep({duration})\n")
-                    last_button_time = time.time()
-                    record_data.append(f"pro.press_button('{control_data}', 0)\n")
                 if isinstance(control_data, str):
                     pro.press_button(control_data, 0)
 
                 if isinstance(control_data, types.FunctionType):
                     control_data()
             else:
                 global_vars = globals()
@@ -235,38 +320,43 @@
                         logger.info(f"{command} process err = {err}")
                 else:
                     logger.info(f"{command} command not support!")
 
         elif isinstance(command, dict):
             try:
                 if "action" in command:
+                    # 按键操作手柄
                     control_data = consts.KEY_MAPPING.get(command["key"])
                     packet = G.input_packet["packet"]
                     if command["action"] == "press":
                         packet[control_data] = True
                     else:
                         packet[control_data] = False
 
-                        if record:
-                            if last_button_time:
-                                current_button_time = time.time()
-                                duration = round(current_button_time - last_button_time, 2)
-                                record_data.append(f"time.sleep({duration})\n")
-                            last_button_time = time.time()
-                            record_data.append(f"pro.press_button('{control_data}', 0)\n")
-                            
+                    if record:
+                        if record_mode == "导航":
+                            progress = G.progress_data[-1]["progress"]
+                        else:
+                            progress = -1
+                        record_data.append(
+                            {
+                                "progress": progress,
+                                "timestamp": command["timestamp"],
+                                "event_type": command["action"],
+                                "control_data": control_data,
+                            }
+                        )
                     G.input_packet["packet"] = packet
                 else:
                     logger.info("Received config update message.")
                     G.CONFIG = command
             except Exception as err:
                 logger.info(
                     f"{command} process err = {err} traceback = {traceback.format_exc()}"
                 )
-
         else:
             logger.info(f"{command} command not support!")
 
 
 def start_command_input(queue):
     t = threading.Thread(target=command_input, args=(queue,), daemon=True)
     t.start()
@@ -283,14 +373,35 @@
         if G.G_RACE_RUN_EVENT.is_set():
             event_loop()
         else:
             time.sleep(1)
     logger.info("Woker quit.")
 
 
+def ocr_progress_worker(progress_data):
+    debug = os.environ.get("A9_DEBUG", 0)
+    start = timestamp()
+    while G.G_OCR_PROGRESS.is_set():
+        if debug:
+            progress = int((timestamp() - start) / 1000)
+        else:
+            progress = OCR.get_progress()
+        current_data = {"progress": progress}
+        if progress_data and current_data == progress_data[-1]:
+            continue
+        progress_data.append(current_data)
+
+
+def start_ocr_progress_worker():
+    p = threading.Thread(
+        target=ocr_progress_worker, args=(G.progress_data,), daemon=True
+    )
+    p.start()
+
+
 def start_worker():
     p = threading.Thread(
         target=worker, args=(G.input_queue, G.output_queue), daemon=True
     )
     p.start()
 
 
@@ -354,15 +465,15 @@
     args = parser.parse_args()
     return args.config
 
 
 def console_version():
     try:
         output = subprocess.check_output(
-            f"pip show ns-asphalt9 | grep Version", shell=True, universal_newlines=True
+            "pip show ns-asphalt9 | grep Version", shell=True, universal_newlines=True
         )
         output = output.strip()
     except subprocess.CalledProcessError:
         output = "Package not found."
 
     logger.info(output)
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-3.4.0/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.3.0
+Version: 3.4.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.3.0/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-3.4.0/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 ns_asphalt9/core/utils/decorator.py
 ns_asphalt9/core/utils/error_process.py
 ns_asphalt9/core/utils/lifo_queue.py
 ns_asphalt9/core/utils/log.py
 ns_asphalt9/core/utils/notify.py
 ns_asphalt9/core/utils/online_tracker.py
 ns_asphalt9/core/utils/page_stack.py
+ns_asphalt9/core/utils/process_record_data.py
 ns_asphalt9/core/utils/thread_lifo_queue.py
 ns_asphalt9/core/utils/timer.py
 ns_asphalt9/core/utils/track_data.py
 ns_asphalt9/core/utils/track_navi_data.py
 ns_asphalt9/core/utils/track_navi_data_update.py
 ns_asphalt9/core/utils/track_navi_data_v2.py
 ns_asphalt9/core/utils/track_navi_data_win.py
```

### Comparing `ns_asphalt9-3.3.0/setup.cfg` & `ns_asphalt9-3.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 3.3.0
+version = 3.4.0
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-3.3.0/tests/test_pages.py` & `ns_asphalt9-3.4.0/tests/test_pages.py`

 * *Files identical despite different names*

