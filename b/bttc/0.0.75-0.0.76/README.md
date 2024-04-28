# Comparing `tmp/bttc-0.0.75.tar.gz` & `tmp/bttc-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.75.tar", last modified: Sun Apr 21 02:56:09 2024, max compression
+gzip compressed data, was "bttc-0.0.76.tar", last modified: Sun Apr 28 06:24:06 2024, max compression
```

## Comparing `bttc-0.0.75.tar` & `bttc-0.0.76.tar`

### file list

```diff
@@ -1,62 +1,74 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.053921 bttc-0.0.75/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.75/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2125 2024-04-21 02:56:09.053921 bttc-0.0.75/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1397 2024-04-21 02:55:47.000000 bttc-0.0.75/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.045921 bttc-0.0.75/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5313 2024-04-21 02:55:57.000000 bttc-0.0.75/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.75/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.75/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.75/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3850 2024-04-19 05:17:08.000000 bttc-0.0.75/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    31276 2024-04-19 06:08:37.000000 bttc-0.0.75/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.045921 bttc-0.0.75/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.053921 bttc-0.0.75/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.053921 bttc-0.0.75/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2125 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-21 02:56:09.000000 bttc-0.0.75/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-21 02:56:09.053921 bttc-0.0.75/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-15 13:48:29.000000 bttc-0.0.75/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.265039 bttc-0.0.76/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.76/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2134 2024-04-28 06:24:06.265039 bttc-0.0.76/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1406 2024-04-28 06:23:45.000000 bttc-0.0.76/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-04-28 06:22:52.000000 bttc-0.0.76/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.76/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.76/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.76/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.76/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1182 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    32048 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.257039 bttc-0.0.76/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.76/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5144 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4968 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.265039 bttc-0.0.76/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16204 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2134 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1587 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-28 06:24:06.265039 bttc-0.0.76/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.76/setup.py
```

### Comparing `bttc-0.0.75/LICENSE` & `bttc-0.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/PKG-INFO` & `bttc-0.0.76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.75
+Version: 0.0.76
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,17 +61,17 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
-* Release v0.0.66: #67, #84, #85
```

### Comparing `bttc-0.0.75/README.md` & `bttc-0.0.76/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
-* Release v0.0.66: #67, #84, #85
```

### Comparing `bttc-0.0.75/bttc/__init__.py` & `bttc-0.0.76/bttc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 
 BT testing common utilities.
 """
 import atexit
 
 import logging
 from mobly.controllers import android_device
+from mobly.controllers.android_device_lib import adb
 from bttc import core
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
-from typing import TypeAlias
+import shlex
+from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.75'
+__version__ = '0.0.76'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
 
 
@@ -151,7 +153,49 @@
   loaded_utils = []
   for field_name, field_obj in dut.__dict__.items():
     if isinstance(field_obj, core.UtilBase):
       print(f'Loaded "{field_name}": {field_obj.DESCRIPTION}')
       loaded_utils.append(field_obj)
 
   return loaded_utils
+
+
+def safe_adb_shell(
+    device: GeneralDevice,
+    use_shlex_split: bool = True,
+    timeout: float | None = None) -> Callable[[str], tuple[str, str, int]]:
+  """Gets safe adb shell executor.
+
+  Below is demo of this function:
+  ```python
+  >>> from bttc import bt_utils
+  >>> from mobly.controllers import android_device
+  >>> phone = android_device.create([{'serial': '07311JECB08252'}])[0]
+  >>> safe_adb = bt_utils.safe_adb_shell(phone)
+  >>> stdout, stderr, rt = safe_adb('getprop ro.build.version.sdk')
+  >>> stdout  # My phone is of SDK 30.
+  '30\n'
+  ```
+
+  Args:
+    device: Adb like device.
+    use_shlex_split: Leverage shlex.split iff True.
+    timeout: float, the number of seconds to wait before timing out. If not
+      specified, no timeout takes effect.
+
+  Returns:
+    Safe callable adb object.
+  """
+  def _adb_wrapper(command: str) -> tuple[str, str, int]:
+    try:
+      command = shlex.split(command) if use_shlex_split else command
+      command_output = device.adb.shell(command, timeout=timeout).decode()
+      return (command_output, '', 0)
+    except adb.AdbError as err:
+      return (err.stdout.decode(encoding='utf-8', errors='strict'),
+              err.stderr.decode(encoding='utf-8',
+                                errors='strict'), err.ret_code)
+    except adb.AdbTimeoutError as err:
+      device.log.warning('Timeout in executing command: %s', command)
+      return ('', str(err), -1)
+
+  return _adb_wrapper
```

### Comparing `bttc-0.0.75/bttc/apk_utils.py` & `bttc-0.0.76/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/ble_data.py` & `bttc-0.0.76/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/ble_utils.py` & `bttc-0.0.76/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/bt_data.py` & `bttc-0.0.76/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/bt_utils.py` & `bttc-0.0.76/bttc/bt_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility to support common BT operations/methods."""
 import datetime
+import deprecation
 from functools import partial
 import logging
 import time
 
 from mobly.controllers import android_device
 from mobly.controllers.android_device_lib import adb
 from bttc import bt_data
@@ -392,14 +393,20 @@
         map(lambda paired_info: paired_info['Name'], paired_devices))
 
   return [
       bt_data.PairedDeviceInfo.from_dict(pair_info_dict)
       for pair_info_dict in paired_devices]
 
 
+@deprecation.deprecated(
+    deprecated_in='0.0.75.x',
+    removed_in='0.0.77.x',
+    details=(
+        'This function is soon to be expired. '
+        'Please use `bttc.safe_adb_shell` instead'))
 def safe_adb_shell(
     device: android_device.AndroidDevice,
     use_shlex_split: bool = True,
     timeout: float | None = None) -> Callable[[str], tuple[str, str, int]]:
   """Gets safe adb shell executor.
 
   Below is demo of this function:
```

### Comparing `bttc-0.0.75/bttc/cli/__init__.py` & `bttc-0.0.76/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/cli/constants.py` & `bttc-0.0.76/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/cli/main.py` & `bttc-0.0.76/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/common_data.py` & `bttc-0.0.76/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/constants.py` & `bttc-0.0.76/bttc/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 # limitations under the License.
 
 """Module to hold constants used in BT operations."""
 import enum
 import re
 
 
+ACTIVITY_RECORD_COMPILED_PATTERN = re.compile(
+    r'ActivityRecord[{].* ([/.a-zA-Z0-9]+) [a-z0-9]+[}]')
+
 ADB_SHELL_CMD_OUTPUT_ENCODING = 'utf-8'
 ADB_SHELL_TIMEOUT_SEC: float = 60
 
 # Logcat message timestamp format
 LOGCAT_DATETIME_FMT = '%m-%d %H:%M:%S.%f'
 
 LOGTCAT_MSG_PATTERN = re.compile(
```

### Comparing `bttc-0.0.75/bttc/core.py` & `bttc-0.0.76/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/errors.py` & `bttc-0.0.76/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/general_utils.py` & `bttc-0.0.76/bttc/general_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from subprocess import Popen, PIPE
 import time
 
 from bttc import bt_utils
 from bttc import constants
 from bttc import core
 from bttc import errors
+from bttc import general_data
 from bttc.cli.constants import warning
 from bttc.utils import device_factory
 from bttc.utils import key_events_handler
 from bttc.utils import typing_utils
 from mobly import utils
 
 from mobly.controllers import android_device
@@ -45,14 +46,16 @@
 
 
 AUTO_LOAD = True
 ANDROID_DEVICE: TypeAlias = android_device.AndroidDevice
 BINDING_KEYWORD = "gm"
 
 
+_ActivityRecord = general_data.ActivityRecord
+
 # Default timeout for adb shell command.
 _ADB_SHELL_TIMEOUT_SEC = constants.ADB_SHELL_TIMEOUT_SEC
 
 # Logcat message timestamp format
 _DATETIME_FMT = constants.LOGCAT_DATETIME_FMT
 
 # Pattern to match message of logcat service.
@@ -346,14 +349,15 @@
     self.device_config = DeviceConfig(self._ad)
     self._bind(disable_airplane_mode)
     self._bind(dumpsys)
     self._bind(enable_airplane_mode)
     self._bind(follow_logcat)
     self._bind(follow_logcat_within)
     self._bind(get_call_state)
+    self._bind(get_current_activity)
     self._bind(get_device_time)
     self._bind(get_ui_xml)
     self._bind(is_apk_installed)
     self._bind(logcat_filter)
     self.props = Props(self._ad)
     self._bind(push_file)
     self.shell = bt_utils.safe_adb_shell(ad)
@@ -377,14 +381,18 @@
       self.disable_airplane_mode()
 
   @property
   def call_state(self) -> str:
     return self.get_call_state()
 
   @property
+  def current_activity(self) -> _ActivityRecord:
+    return self.get_current_activity()
+
+  @property
   def device_time(self) -> str:
     return self.get_device_time()
 
   @property
   def device_datetime(self) -> datetime.datetime:
     return self.get_device_time(to_datetime=True)
 
@@ -877,14 +885,33 @@
 
     return False
 
   return follow_logcat(
       ad, stop_callback, wait_time_sec, logcat_args=logcat_args)
 
 
+def get_current_activity(ad: typing_utils.AdbDevice) -> _ActivityRecord:
+  """Gets current activity that is currently opened to the user.
+
+  Args:
+    ad: Adb like object.
+
+  Returns:
+    The current activity information.
+  """
+  adb_output = (
+      ad.adb.shell(
+          'dumpsys activity activities | grep ResumedActivity').decode())
+  matcher = constants.ACTIVITY_RECORD_COMPILED_PATTERN.search(adb_output)
+  if not matcher:
+    raise ValueError(f'Unexpected adb output: {adb_output}')
+
+  return _ActivityRecord(full_activity_path=matcher.group(1))
+
+
 def get_ui_xml(ad: Any, xml_out_file_path: str) -> str:
   """Gets the XML object of current UI.
 
   Args:
     ad: Device to dump UI from.
     xml_out_file_path: The host file path to output current UI xml content.
```

### Comparing `bttc-0.0.75/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.76/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.76/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.76/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.76/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.76/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/avrcp/errors.py` & `bttc-0.0.76/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/__init__.py` & `bttc-0.0.76/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/constants.py` & `bttc-0.0.76/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/errors.py` & `bttc-0.0.76/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.76/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.76/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.76/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.76/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/strategy.py` & `bttc-0.0.76/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/ad_checker.py` & `bttc-0.0.76/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/device_factory.py` & `bttc-0.0.76/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/iperf/__init__.py` & `bttc-0.0.76/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/iperf/errors.py` & `bttc-0.0.76/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/key_events_handler.py` & `bttc-0.0.76/bttc/utils/key_events_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,23 @@
 from mobly.controllers.android_device_lib import adb
 
 from bttc.utils import retry
 from bttc.utils import typing_utils
 
 
 @enum.unique
+class MediaKeyCode(enum.Enum):
+  """Media key codes."""
+  NEXT = 87
+  PREVIOUS = 88
+  PLAY = 126
+  PAUSE = 127
+
+
+@enum.unique
 class KeycodeNumPad(enum.Enum):
   """Enum class for Numpad key event."""
 
   NUM_0 = '0'
   NUM_1 = '1'
   NUM_2 = '2'
   NUM_3 = '3'
@@ -77,35 +86,47 @@
 
   @retry.retry_on_exception(
       retry_value=adb.Error,
       retry_intervals=retry.FuzzedExponentialIntervals(
           initial_delay_sec=1,
           num_retries=5,
           factor=1.1))
-  def send_keycode(self, keycode: str):
+  def send_keycode(self, keycode: str | int):
     """Sends key event.
 
     Args:
       keycode: Key event code.
     """
-    self._device.adb.shell(shlex.split(
-        f'input keyevent KEYCODE_{keycode}'))
+    if isinstance(keycode, str):
+      self._device.adb.shell(shlex.split(
+          f'input keyevent KEYCODE_{keycode}'))
+    else:
+      self._device.adb.shell(shlex.split(
+          f'input keyevent {keycode}'))
+
+  def key_media_next(self):
+    """Sends key event MEDIA_NEXT."""
+    self.send_keycode(MediaKeyCode.NEXT.value)
 
   def key_media_play(self):
     """Sends key event MEDIA_PLAY."""
     self.send_keycode('MEDIA_PLAY')
 
   def key_media_pause(self):
     """Sends key event MEDIA_PAUSE."""
     self.send_keycode('MEDIA_PAUSE')
 
   def key_media_play_pause(self):
     """Sends key event MEDIA_PLAY_PAUSE."""
     self.send_keycode('MEDIA_PLAY_PAUSE')
 
+  def key_media_previous(self):
+    """Sends key event MEDIA_PREVIOUS."""
+    self.send_keycode(MediaKeyCode.PREVIOUS.value)
+
   def key_power(self):
     """Sends key event POWER.
 
     For details, please refer to go/android_keyevent_power
     """
     self.send_keycode('POWER')
```

### Comparing `bttc-0.0.75/bttc/utils/log_parser.py` & `bttc-0.0.76/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/logcat.py` & `bttc-0.0.76/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/retry.py` & `bttc-0.0.76/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils/typing_utils.py` & `bttc-0.0.76/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc/utils_loader.py` & `bttc-0.0.76/bttc/utils_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """Utility to load functional modules of device."""
 from bttc import core
 from bttc import apk_utils        # noqa: F401
 from bttc import ble_utils        # noqa: F401
 from bttc import general_utils    # noqa: F401
 from bttc import bt_utils         # noqa: F401
+from bttc import mc_utils       # noqa: F401
 from bttc import wifi_utils       # noqa: F401
 import dataclasses
 import deprecation
 import importlib
 import pkgutil
 from typing import Any
```

### Comparing `bttc-0.0.75/bttc/wifi_utils.py` & `bttc-0.0.76/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.75/bttc.egg-info/PKG-INFO` & `bttc-0.0.76/bttc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.75
+Version: 0.0.76
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,17 +61,17 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
-* Release v0.0.66: #67, #84, #85
```

### Comparing `bttc-0.0.75/bttc.egg-info/SOURCES.txt` & `bttc-0.0.76/bttc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 bttc/ble_utils.py
 bttc/bt_data.py
 bttc/bt_utils.py
 bttc/common_data.py
 bttc/constants.py
 bttc/core.py
 bttc/errors.py
+bttc/general_data.py
 bttc/general_utils.py
+bttc/mc_data.py
+bttc/mc_utils.py
 bttc/strategy.py
 bttc/utils_loader.py
 bttc/wifi_utils.py
 bttc.egg-info/PKG-INFO
 bttc.egg-info/SOURCES.txt
 bttc.egg-info/dependency_links.txt
 bttc.egg-info/requires.txt
@@ -42,8 +45,15 @@
 bttc/utils/device_factory.py
 bttc/utils/key_events_handler.py
 bttc/utils/log_parser.py
 bttc/utils/logcat.py
 bttc/utils/retry.py
 bttc/utils/typing_utils.py
 bttc/utils/iperf/__init__.py
-bttc/utils/iperf/errors.py
+bttc/utils/iperf/errors.py
+bttc/utils/media_player/media_player_agent_facade.py
+bttc/utils/media_player/yt_player_agent.py
+bttc/utils/ui_pages/__init__.py
+bttc/utils/ui_pages/errors.py
+bttc/utils/ui_pages/ui_core.py
+bttc/utils/ui_pages/ui_node.py
+bttc/utils/ui_pages/utils.py
```

### Comparing `bttc-0.0.75/setup.py` & `bttc-0.0.76/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     url='https://github.com/johnklee/bt_test_common',
     author='John Lee/Yuan Long Luo/Denny Chai',
     author_email='puremonkey2007@gmail.com',
     license='MIT License',
     packages=[
         'bttc', 'bttc.cli', 'bttc.utils', 'bttc.profiles.hfp', 'bttc.profiles.avrcp',
         'bttc.utils.iperf', 'bttc.mobly_android_device_lib',
+        'bttc.utils.ui_pages', 'bttc.utils.media_player',
         'bttc.mobly_android_device_lib.services'],
     install_requires=[
         'cmd2==2.4.3',
         'deprecation==2.1.0',
         'mobly>=1.12.2',
         'portpicker==1.6.0',
         'psutil==5.9.8',
```

