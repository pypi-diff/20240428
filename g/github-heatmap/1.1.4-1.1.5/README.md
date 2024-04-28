# Comparing `tmp/github_heatmap-1.1.4.tar.gz` & `tmp/github_heatmap-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_heatmap-1.1.4.tar", last modified: Tue Mar 26 01:55:18 2024, max compression
+gzip compressed data, was "github_heatmap-1.1.5.tar", last modified: Sun Apr 28 01:43:49 2024, max compression
```

## Comparing `github_heatmap-1.1.4.tar` & `github_heatmap-1.1.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.899261 github_heatmap-1.1.4/
--rw-r--r--   0 shareit    (501) staff       (20)     1063 2023-12-21 11:20:04.000000 github_heatmap-1.1.4/LICENSE
--rw-r--r--   0 shareit    (501) staff       (20)     1056 2024-03-26 01:55:18.898949 github_heatmap-1.1.4/PKG-INFO
--rw-r--r--   0 shareit    (501) staff       (20)    24306 2024-03-21 08:27:09.000000 github_heatmap-1.1.4/README.md
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.887239 github_heatmap-1.1.4/github_heatmap/
--rw-r--r--   0 shareit    (501) staff       (20)        0 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)       75 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/__main__.py
--rw-r--r--   0 shareit    (501) staff       (20)     6365 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/circluar_drawer.py
--rw-r--r--   0 shareit    (501) staff       (20)     6628 2024-02-06 08:01:02.000000 github_heatmap-1.1.4/github_heatmap/cli.py
--rw-r--r--   0 shareit    (501) staff       (20)     1130 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/config.py
--rw-r--r--   0 shareit    (501) staff       (20)     9803 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/drawer.py
--rw-r--r--   0 shareit    (501) staff       (20)      261 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/err.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.889371 github_heatmap-1.1.4/github_heatmap/html_parser/
--rw-r--r--   0 shareit    (501) staff       (20)      206 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/html_parser/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)     1586 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/html_parser/github_parser.py
--rw-r--r--   0 shareit    (501) staff       (20)      256 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/html_parser/gitlab_parser.py
--rw-r--r--   0 shareit    (501) staff       (20)     2007 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/html_parser/jike_parse.py
--rw-r--r--   0 shareit    (501) staff       (20)      257 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/html_parser/kindle_parser.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.897153 github_heatmap-1.1.4/github_heatmap/loader/
--rw-r--r--   0 shareit    (501) staff       (20)     3503 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)     5188 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/apple_health_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     7507 2024-02-06 07:59:58.000000 github_heatmap-1.1.4/github_heatmap/loader/base_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     4150 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/bbdc_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3298 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/bilibili_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2197 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/chatgpt_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3289 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/cichang_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     6415 2024-02-12 04:57:49.000000 github_heatmap-1.1.4/github_heatmap/loader/config.py
--rw-r--r--   0 shareit    (501) staff       (20)     1962 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/covid_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     1561 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/dota2_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2596 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/duolingo_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2496 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/forest_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2829 2023-12-22 03:49:45.000000 github_heatmap-1.1.4/github_heatmap/loader/from_github_issue_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2798 2023-12-22 03:49:45.000000 github_heatmap-1.1.4/github_heatmap/loader/garmin_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     1771 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/github_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3414 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/gitlab_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3170 2023-12-22 03:49:45.000000 github_heatmap-1.1.4/github_heatmap/loader/gpx_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     7136 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/jike_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     1096 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/json_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     1681 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/kindle_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2597 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/leetcode_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     1393 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/multiple_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2715 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/neodb_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3928 2024-03-19 07:00:12.000000 github_heatmap-1.1.4/github_heatmap/loader/notion_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3765 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/nrc_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3323 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/ns_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3439 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/openlanguage_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2365 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/shanbay_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3144 2023-12-22 03:49:45.000000 github_heatmap-1.1.4/github_heatmap/loader/strava_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)      966 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/summary_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     5288 2023-12-22 03:49:45.000000 github_heatmap-1.1.4/github_heatmap/loader/todoist_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     2973 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/wakatime_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3177 2024-03-26 01:52:57.000000 github_heatmap-1.1.4/github_heatmap/loader/weread_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     1641 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/loader/youtube_loader.py
--rw-r--r--   0 shareit    (501) staff       (20)     3849 2024-01-13 06:01:05.000000 github_heatmap-1.1.4/github_heatmap/poster.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.897690 github_heatmap-1.1.4/github_heatmap/skyline/
--rw-r--r--   0 shareit    (501) staff       (20)       75 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/skyline/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)      185 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/skyline/config.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.897836 github_heatmap-1.1.4/github_heatmap/skyline/font/
--rw-r--r--   0 shareit    (501) staff       (20)        0 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/skyline/font/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)     4015 2023-12-22 03:44:18.000000 github_heatmap-1.1.4/github_heatmap/skyline/skyline.py
--rw-r--r--   0 shareit    (501) staff       (20)     1674 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/structures.py
--rw-r--r--   0 shareit    (501) staff       (20)     2211 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/github_heatmap/utils.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.888022 github_heatmap-1.1.4/github_heatmap.egg-info/
--rw-r--r--   0 shareit    (501) staff       (20)     1056 2024-03-26 01:55:18.000000 github_heatmap-1.1.4/github_heatmap.egg-info/PKG-INFO
--rw-r--r--   0 shareit    (501) staff       (20)     2262 2024-03-26 01:55:18.000000 github_heatmap-1.1.4/github_heatmap.egg-info/SOURCES.txt
--rw-r--r--   0 shareit    (501) staff       (20)        1 2024-03-26 01:55:18.000000 github_heatmap-1.1.4/github_heatmap.egg-info/dependency_links.txt
--rw-r--r--   0 shareit    (501) staff       (20)       59 2024-03-26 01:55:18.000000 github_heatmap-1.1.4/github_heatmap.egg-info/entry_points.txt
--rw-r--r--   0 shareit    (501) staff       (20)      228 2024-03-26 01:55:18.000000 github_heatmap-1.1.4/github_heatmap.egg-info/requires.txt
--rw-r--r--   0 shareit    (501) staff       (20)       21 2024-03-26 01:55:18.000000 github_heatmap-1.1.4/github_heatmap.egg-info/top_level.txt
--rw-r--r--   0 shareit    (501) staff       (20)       31 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/pyproject.toml
--rw-r--r--   0 shareit    (501) staff       (20)       38 2024-03-26 01:55:18.899305 github_heatmap-1.1.4/setup.cfg
--rw-r--r--   0 shareit    (501) staff       (20)     1001 2024-03-26 01:54:37.000000 github_heatmap-1.1.4/setup.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-03-26 01:55:18.898030 github_heatmap-1.1.4/tests/
--rw-r--r--   0 shareit    (501) staff       (20)        0 2023-12-21 11:20:05.000000 github_heatmap-1.1.4/tests/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)      733 2023-12-22 03:44:17.000000 github_heatmap-1.1.4/tests/test_poster_utils.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.663352 github_heatmap-1.1.5/
+-rw-r--r--   0 shareit    (501) staff       (20)     1063 2023-12-21 11:20:04.000000 github_heatmap-1.1.5/LICENSE
+-rw-r--r--   0 shareit    (501) staff       (20)     1056 2024-04-28 01:43:49.663130 github_heatmap-1.1.5/PKG-INFO
+-rw-r--r--   0 shareit    (501) staff       (20)    24733 2024-04-26 04:29:22.000000 github_heatmap-1.1.5/README.md
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.651457 github_heatmap-1.1.5/github_heatmap/
+-rw-r--r--   0 shareit    (501) staff       (20)        0 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)       75 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/__main__.py
+-rw-r--r--   0 shareit    (501) staff       (20)     6365 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/circluar_drawer.py
+-rw-r--r--   0 shareit    (501) staff       (20)     7094 2024-04-26 11:42:36.000000 github_heatmap-1.1.5/github_heatmap/cli.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1273 2024-04-26 11:50:48.000000 github_heatmap-1.1.5/github_heatmap/config.py
+-rw-r--r--   0 shareit    (501) staff       (20)    10426 2024-04-28 01:32:23.000000 github_heatmap-1.1.5/github_heatmap/drawer.py
+-rw-r--r--   0 shareit    (501) staff       (20)      261 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/err.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.653507 github_heatmap-1.1.5/github_heatmap/html_parser/
+-rw-r--r--   0 shareit    (501) staff       (20)      206 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/html_parser/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1586 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/html_parser/github_parser.py
+-rw-r--r--   0 shareit    (501) staff       (20)      256 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/html_parser/gitlab_parser.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2007 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/html_parser/jike_parse.py
+-rw-r--r--   0 shareit    (501) staff       (20)      257 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/html_parser/kindle_parser.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.661351 github_heatmap-1.1.5/github_heatmap/loader/
+-rw-r--r--   0 shareit    (501) staff       (20)     3503 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)     5188 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/apple_health_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     7507 2024-02-06 07:59:58.000000 github_heatmap-1.1.5/github_heatmap/loader/base_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     4150 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/bbdc_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3298 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/bilibili_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2197 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/chatgpt_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3289 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/cichang_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     6415 2024-02-12 04:57:49.000000 github_heatmap-1.1.5/github_heatmap/loader/config.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1962 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/covid_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1561 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/dota2_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2596 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/duolingo_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2496 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/forest_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2829 2023-12-22 03:49:45.000000 github_heatmap-1.1.5/github_heatmap/loader/from_github_issue_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2798 2023-12-22 03:49:45.000000 github_heatmap-1.1.5/github_heatmap/loader/garmin_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1771 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/github_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3414 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/gitlab_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3170 2023-12-22 03:49:45.000000 github_heatmap-1.1.5/github_heatmap/loader/gpx_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     7136 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/jike_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1096 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/json_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1681 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/kindle_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2597 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/leetcode_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1393 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/multiple_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2715 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/neodb_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3864 2024-04-24 02:15:19.000000 github_heatmap-1.1.5/github_heatmap/loader/notion_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3765 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/nrc_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3323 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/ns_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3439 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/openlanguage_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2365 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/shanbay_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3144 2023-12-22 03:49:45.000000 github_heatmap-1.1.5/github_heatmap/loader/strava_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)      966 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/summary_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     5288 2023-12-22 03:49:45.000000 github_heatmap-1.1.5/github_heatmap/loader/todoist_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2973 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/wakatime_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     3203 2024-04-26 10:59:41.000000 github_heatmap-1.1.5/github_heatmap/loader/weread_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1641 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/loader/youtube_loader.py
+-rw-r--r--   0 shareit    (501) staff       (20)     4073 2024-04-26 06:44:09.000000 github_heatmap-1.1.5/github_heatmap/poster.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.661960 github_heatmap-1.1.5/github_heatmap/skyline/
+-rw-r--r--   0 shareit    (501) staff       (20)       75 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/skyline/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)      185 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/skyline/config.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.662100 github_heatmap-1.1.5/github_heatmap/skyline/font/
+-rw-r--r--   0 shareit    (501) staff       (20)        0 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/skyline/font/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)     4015 2023-12-22 03:44:18.000000 github_heatmap-1.1.5/github_heatmap/skyline/skyline.py
+-rw-r--r--   0 shareit    (501) staff       (20)     1674 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/structures.py
+-rw-r--r--   0 shareit    (501) staff       (20)     2211 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/github_heatmap/utils.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.652494 github_heatmap-1.1.5/github_heatmap.egg-info/
+-rw-r--r--   0 shareit    (501) staff       (20)     1056 2024-04-28 01:43:49.000000 github_heatmap-1.1.5/github_heatmap.egg-info/PKG-INFO
+-rw-r--r--   0 shareit    (501) staff       (20)     2262 2024-04-28 01:43:49.000000 github_heatmap-1.1.5/github_heatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 shareit    (501) staff       (20)        1 2024-04-28 01:43:49.000000 github_heatmap-1.1.5/github_heatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 shareit    (501) staff       (20)       59 2024-04-28 01:43:49.000000 github_heatmap-1.1.5/github_heatmap.egg-info/entry_points.txt
+-rw-r--r--   0 shareit    (501) staff       (20)      228 2024-04-28 01:43:49.000000 github_heatmap-1.1.5/github_heatmap.egg-info/requires.txt
+-rw-r--r--   0 shareit    (501) staff       (20)       21 2024-04-28 01:43:49.000000 github_heatmap-1.1.5/github_heatmap.egg-info/top_level.txt
+-rw-r--r--   0 shareit    (501) staff       (20)       31 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/pyproject.toml
+-rw-r--r--   0 shareit    (501) staff       (20)       38 2024-04-28 01:43:49.663397 github_heatmap-1.1.5/setup.cfg
+-rw-r--r--   0 shareit    (501) staff       (20)     1001 2024-04-28 01:43:36.000000 github_heatmap-1.1.5/setup.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2024-04-28 01:43:49.662274 github_heatmap-1.1.5/tests/
+-rw-r--r--   0 shareit    (501) staff       (20)        0 2023-12-21 11:20:05.000000 github_heatmap-1.1.5/tests/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)      733 2023-12-22 03:44:17.000000 github_heatmap-1.1.5/tests/test_poster_utils.py
```

### Comparing `github_heatmap-1.1.4/LICENSE` & `github_heatmap-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/PKG-INFO` & `github_heatmap-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github_heatmap
-Version: 1.1.4
+Version: 1.1.5
 Summary: Make everything a GitHub svg poster and Skyline!
 Home-page: https://github.com/malinkang/GitHubPoster
 Author: malinkang
 Author-email: linkang.ma@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `github_heatmap-1.1.4/README.md` & `github_heatmap-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -734,8 +734,10 @@
 - @[guaguaguaxia](https://github.com/guaguaguaxia) OpenLanguage loader
 - @[rip-tyang](https://github.com/rip-tyang) AppleHealth loader
 
 # 赞赏
 
 谢谢就够了
 
-Just enjoy it
+Just enjoy it
+
+python3 -m github_heatmap notion  --notion_token "secret_xvMkQzLkCRtZL478L8MhvLdIDOxicjjSUm9U9voAwbb" --database_id "cf6359306f94456da01908af73191a61" --date_prop_name "时间" --value_prop_name "金币" --unit "金币" --year 2024 --me "哈哈哈" --without-type-name --with-animation --background-color=#FFFFFF --track-color=#f44336 --special-color1=#ffd966 --special-color2=#549F57 --dom-color=#EBEDF0 --text-color=#000000
```

### Comparing `github_heatmap-1.1.4/github_heatmap/circluar_drawer.py` & `github_heatmap-1.1.5/github_heatmap/circluar_drawer.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/cli.py` & `github_heatmap-1.1.5/github_heatmap/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 from github_heatmap.circluar_drawer import CircularDrawer
 from github_heatmap.config import TYPE_INFO_DICT
 from github_heatmap.drawer import Drawer
 from github_heatmap.err import DepNotInstalledError
 from github_heatmap.loader import LOADER_DICT
 from github_heatmap.poster import Poster
 from github_heatmap.utils import parse_years, reduce_year_list
+from github_heatmap.config import (
+    HEAD_FONT_SIZE,
+    YEAR_FONT_SIZE,
+    MONTH_FONT_SIZE,
+    DOM_BOX_PADING,
+    DOM_BOX_TUPLE,
+    MARGIN_TOP,
+    MARGIN_LEFT
+)
 
 OUT_FOLDER = os.path.join(os.getcwd(), "OUT_FOLDER")
 
 
 def run():
     """Handle command line arguments and call other modules as needed."""
     p = Poster()
@@ -122,15 +131,23 @@
     }
     if args.special_number1:
         p.special_number["special_number1"] = args.special_number1
     if args.special_number2:
         p.special_number["special_number2"] = args.special_number2
     # the length of this poster
     poster_length = len(p.years) if args.type != "summary" else len(loader.loader_list)
-    p.height = 10 + poster_length * 38
+    p.width = MARGIN_LEFT * 2 + (DOM_BOX_PADING + DOM_BOX_TUPLE[0]) * 53
+    p.height = (
+        MARGIN_TOP
+        + HEAD_FONT_SIZE
+        + poster_length
+        * (YEAR_FONT_SIZE + MONTH_FONT_SIZE+DOM_BOX_PADING*3 + (DOM_BOX_PADING + DOM_BOX_TUPLE[0]) * 7)
+    )
+    print(f"高度 = {p.height}")
+    print(f"宽度 = {p.width}")
     if not os.path.exists(OUT_FOLDER):
         os.mkdir(OUT_FOLDER)
     # support different issues, maybe better way
     file_name = str(args.type)
 
     # make different drawer
     is_circular = args.is_circular
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `github_heatmap-1.1.4/github_heatmap/drawer.py` & `github_heatmap-1.1.5/github_heatmap/drawer.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 
 from github_heatmap.config import (
     COLOR_TUPLE,
     DEFAULT_DOM_COLOR,
     DOM_BOX_DICT,
     DOM_BOX_TUPLE,
     MONTH_NAMES,
+    YEAR_FONT_SIZE,
+    MONTH_FONT_SIZE,
+    DOM_BOX_PADING,
+    DOM_BOX_RADIUS,
 )
 from github_heatmap.err import BaseDrawError
 from github_heatmap.utils import interpolate_color, make_key_times
 
 
 class Drawer:
     name = "github"
 
     def __init__(self, p):
         self.poster = p
-        self.year_size = 80 * 3.0 / 80.0
-        self.year_style = f"font-size:{self.year_size}px; font-family:Arial;"
-        self.year_length_style = f"font-size:{80 * 3.0 / 80.0}px; font-family:Arial;"
-        self.month_names_style = "font-size:2.5px; font-family:Arial"
+        self.year_style = f"font-size:{YEAR_FONT_SIZE}px; font-family:Arial;"
+        self.month_names_style = f"font-size:{MONTH_FONT_SIZE}px; font-family:Arial"
 
     @property
     def type_color_dict(self):
         """
         for multiple types
         """
         return dict(
@@ -85,15 +87,21 @@
         if day_tracks:
             color = self.make_color(self.poster.length_range_by_date, day_tracks)
             if day_tracks >= self.poster.special_number["special_number1"]:
                 color = self.poster.colors.get("special2") or self.poster.colors.get(
                     "special"
                 )
             date_title = f"{date_title} {day_tracks} {self.poster.units}"
-        rect = dr.rect((rect_x, rect_y), DOM_BOX_TUPLE, fill=color,rx=0.4, ry=0.4)
+        rect = dr.rect(
+            (rect_x, rect_y),
+            DOM_BOX_TUPLE,
+            fill=color,
+            rx=DOM_BOX_RADIUS,
+            ry=DOM_BOX_RADIUS,
+        )
         if with_animation:
             rect = self.__add_animation(rect, key_times, animate_index)
         rect.set_desc(title=date_title)
         yield rect
 
     def _gen_day_boxes(
         self,
@@ -121,15 +129,21 @@
             for _type in self.poster.type_list:
                 num = day_tracks.get(_type, 0)
                 length_range = self.poster.length_range_by_date_dict.get(_type, 1)
                 if not num:
                     continue
                 dom = dom_tuple[index]
                 color = self.make_color(length_range, num)
-                rect = dr.rect((rect_x, rect_y), dom, fill=color,rx=0.4, ry=0.4)
+                rect = dr.rect(
+                    (rect_x, rect_y),
+                    dom,
+                    fill=color,
+                    rx=DOM_BOX_RADIUS,
+                    ry=DOM_BOX_RADIUS,
+                )
                 date_title = f"{date_title} {num} for {_type}"
                 if with_animation:
                     rect = self.__add_animation(rect, key_times, animate_index)
                 rect.set_desc(title=date_title)
                 yield rect
                 rect_y += dom_tuple[index][1]
                 index += 1
@@ -137,14 +151,15 @@
             rect = dr.rect((rect_x, rect_y), DOM_BOX_TUPLE, fill=DEFAULT_DOM_COLOR)
             if with_animation:
                 rect = self.__add_animation(rect, key_times, animate_index)
             yield rect
 
     # noinspection PyArgumentList
     def _draw_one_calendar(self, dr, year, offset, _type=None):
+        print(year)
         start_date_weekday, _ = calendar.monthrange(year, 1)
         github_rect_first_day = datetime.date(year, 1, 1)
         # GitHub profile the first day start from the last Monday of the last year
         # or the first Monday of this year.
         # It depends on if the first day of this year is Monday or not.
         github_rect_day = github_rect_first_day + datetime.timedelta(
             -start_date_weekday
@@ -152,66 +167,77 @@
         year_length = self.poster.total_sum_year_dict.get(year, 0)
         year_units = self.poster.units
         if self.poster.units == "mins":
             year_length = int(year_length / 60)
             # change to hours from mins
             year_units = "hours"
         year_length = str(int(year_length)) + f" {year_units}"
+        # 绘制经验
+        offset.y += DOM_BOX_PADING
+        offset.y += YEAR_FONT_SIZE
         dr.add(
             dr.text(
                 f"{year}: {year_length}" if _type is None else f"{_type}",
                 insert=offset.tuple(),
                 fill=self.poster.colors["text"],
-                dominant_baseline="hanging",
                 style=self.year_style,
             )
         )
+        offset.y += DOM_BOX_PADING
+        offset.y += MONTH_FONT_SIZE
+        size = DOM_BOX_PADING + DOM_BOX_TUPLE[1]
+        # 绘制月份
+        # for num, name in enumerate(MONTH_NAMES):
 
-        # if not self.poster.is_multiple_type:
-        #     dr.add(
-        #         dr.text(
-        #             f"{year_length}",
-        #             insert=(offset.tuple()[0] + 165, offset.tuple()[1] + 5),
-        #             fill=self.poster.colors["text"],
-        #             dominant_baseline="hanging",
-        #             style=self.year_length_style,
-        #         )
-        #     )
-        # add month name up to the poster one by one
-        # because of svg text auto trim the spaces.
-        for num, name in enumerate(MONTH_NAMES):
-            dr.add(
-                dr.text(
-                    f"{name}",
-                    insert=(offset.tuple()[0] + 15.5 * num, offset.tuple()[1] + self.year_size +4),
-                    fill=self.poster.colors["text"],
-                    style=self.month_names_style,
-                )
-            )
-
-        rect_x = 10.0
+        rect_x = offset.x
         animate_index = 1
         year_count, key_times = 0, ""
         if self.poster.with_animation:
             # set default count 10
             year_count = self.poster.year_tracks_date_count_dict.get(str(year), 10)
             key_times = make_key_times(year_count)
 
         # add every day of this year for 53 weeks and per week has 7 days
-        for _ in range(54):
-            rect_y = offset.y + self.year_size + 2
-            for _ in range(7):
+        month = MONTH_NAMES[0]
+        for index in range(54):
+            if index == 0:
+                dr.add(
+                    dr.text(
+                        f"{month}",
+                        insert=(
+                            rect_x,
+                            offset.y,
+                        ),
+                        fill=self.poster.colors["text"],
+                        style=self.month_names_style,
+                    )
+                )
+            if index > 0 and index < 53 and month!=MONTH_NAMES[github_rect_day.month - 1]:
+                month = MONTH_NAMES[github_rect_day.month - 1]
+                dr.add(
+                    dr.text(
+                        f"{month}",
+                        insert=(
+                            rect_x,
+                            offset.y,
+                        ),
+                        fill=self.poster.colors["text"],
+                        style=self.month_names_style,
+                    )
+                )
+            # 一个box的大小+间距
+            for week in range(7):
+                """绘制列"""
                 if int(github_rect_day.year) > year:
                     break
-                rect_y += 3.5
+                rect_y = offset.y + size * week + DOM_BOX_PADING
                 date_title = str(github_rect_day)
                 day_tracks = None
                 if date_title in self.poster.tracks:
                     day_tracks = self.poster.tracks[date_title]
-
                     # tricky for may cause animate error
                     if animate_index < len(key_times) - 1:
                         animate_index += 1
                 gen_box_func = (
                     self._gen_day_box
                     if len(self.poster.type_list) == 1
                     else self._gen_day_boxes
@@ -224,16 +250,17 @@
                     day_tracks,
                     self.poster.with_animation,
                     key_times,
                     animate_index,
                 ):
                     dr.add(rect)
                 github_rect_day += datetime.timedelta(1)
-            rect_x += 3.5
-        offset.y += 3.5 * 9 + self.year_size + 1.0
+            rect_x += size
+        # 绘制一年的
+        offset.y += size * 7
 
     def draw(self, dr, offset, is_summary=False):
         if self.poster.tracks is None:
             raise BaseDrawError("No tracks to draw")
 
         if is_summary:
             for loader in self.poster.loader_list:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `github_heatmap-1.1.4/github_heatmap/html_parser/github_parser.py` & `github_heatmap-1.1.5/github_heatmap/html_parser/github_parser.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/html_parser/jike_parse.py` & `github_heatmap-1.1.5/github_heatmap/html_parser/jike_parse.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/__init__.py` & `github_heatmap-1.1.5/github_heatmap/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/apple_health_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/apple_health_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/base_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/bbdc_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/bbdc_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/bilibili_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/bilibili_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/chatgpt_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/chatgpt_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/cichang_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/cichang_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/config.py` & `github_heatmap-1.1.5/github_heatmap/loader/config.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/covid_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/covid_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/dota2_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/dota2_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/duolingo_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/duolingo_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/forest_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/forest_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/from_github_issue_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/from_github_issue_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/garmin_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/garmin_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/github_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/github_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/gitlab_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/gitlab_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/gpx_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/gpx_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/jike_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/jike_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/json_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/json_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/kindle_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/kindle_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/leetcode_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/leetcode_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/multiple_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/multiple_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/neodb_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/neodb_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/notion_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/notion_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,14 @@
             if date and value:
                 dt = date.get("start")
                 type = value.get("type")
                 if(type == "formula" and value.get(type).get("type") == "number"):
                     value = int(value.get(type).get("number"))
                 
                 date_str = pendulum.parse(dt).to_date_string()
-                print(f"date_str = {date_str} value = {value}")
                 self.number_by_date_dict[date_str] = self.number_by_date_dict.get(date_str,0) + value
         for _, v in self.number_by_date_dict.items():
             self.number_list.append(v)
 
     def get_all_track_data(self):
         self.make_track_dict()
         self.make_special_number()
```

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/nrc_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/nrc_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/ns_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/ns_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/openlanguage_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/openlanguage_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/shanbay_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/shanbay_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/strava_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/strava_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/summary_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/summary_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/todoist_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/todoist_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/wakatime_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/wakatime_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/weread_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/weread_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
                 result = cookie_str
         return result
     
     def get_api_data(self):
         self.session.get(WEREAD_BASE_URL)
         r = self.session.get(WEREAD_HISTORY_URL)
         if not r.ok:
+            print(r.text)
             # need to refresh cookie
             if r.json()["errcode"] == -2012:
                 raise Exception("Cookie过期了请重新设置cookie")
             else:
                 raise Exception("Can not get weread history data")
         return r.json()
```

### Comparing `github_heatmap-1.1.4/github_heatmap/loader/youtube_loader.py` & `github_heatmap-1.1.5/github_heatmap/loader/youtube_loader.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/poster.py` & `github_heatmap-1.1.5/github_heatmap/poster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Create a poster from track data."""
 from collections import defaultdict
 
 import svgwrite
 
 from github_heatmap.structures import XY, ValueRange
-
+from github_heatmap.config import (
+    HEAD_FONT_SIZE,
+    MARGIN_LEFT,
+    MARGIN_TOP
+)
 
 class Poster:
     def __init__(self):
         self.title = None
         self.tracks = {}
         self.type_list = []
         self.loader_list = []
@@ -17,17 +21,18 @@
         self.units = "metric"
         self.colors = {
             "background": "#222222",
             "text": "#FFFFFF",
             "special": "#FFFF00",
             "track": "#4DD2FF",
         }
-        self.width = 200
+        self.width = 400
         self.height = 300
         self.years = None
+        self.offset = XY(MARGIN_LEFT,MARGIN_TOP)
         # maybe support more type
         self.tracks_drawer = None
         self.trans = None
         self.with_animation = False
         self.animation_time = 10
         self.year_tracks_date_count_dict = defaultdict(int)
         self.year_tracks_type_dict = defaultdict(dict)
@@ -80,27 +85,30 @@
         height = self.height
         width = self.width
         self.tracks_drawer = drawer
         d = svgwrite.Drawing(output, (f"{width}mm", f"{height}mm"))
         d.viewbox(0, 0, self.width, height)
         d.add(d.rect((0, 0), (width, height), fill=self.colors["background"]))
         self.__draw_header(d)
-        self.__draw_tracks(d, XY(10, 14))
+        self.__draw_tracks(d, self.offset)
         # for multiple types show
         if self.is_multiple_type:
             self.__draw_footer(d)
         d.save()
 
     def __draw_tracks(self, d, offset):
         self.tracks_drawer.draw(d, offset, self.is_summary)
 
     def __draw_header(self, d):
+        self.offset.y += HEAD_FONT_SIZE
         text_color = self.colors["text"]
-        title_style = "font-size:6px; font-family:Arial; font-weight:bold;"
-        d.add(d.text(self.title, insert=(10, 10), fill=text_color, style=title_style))
+        title_style = f"font-size:{HEAD_FONT_SIZE}px; font-family:Arial; font-weight:bold;"
+        d.add(d.text(self.title, insert=(self.offset.x, self.offset.y), fill=text_color, style=title_style))
+     
+
 
     def __draw_footer(self, d):
         self.tracks_drawer.draw_footer(d)
 
     def compute_track_statistics(self, t):
         total_sum_year_dict = defaultdict(int)
         for date, num in self.tracks.items():
```

### Comparing `github_heatmap-1.1.4/github_heatmap/skyline/skyline.py` & `github_heatmap-1.1.5/github_heatmap/skyline/skyline.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/structures.py` & `github_heatmap-1.1.5/github_heatmap/structures.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap/utils.py` & `github_heatmap-1.1.5/github_heatmap/utils.py`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/github_heatmap.egg-info/PKG-INFO` & `github_heatmap-1.1.5/github_heatmap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-heatmap
-Version: 1.1.4
+Version: 1.1.5
 Summary: Make everything a GitHub svg poster and Skyline!
 Home-page: https://github.com/malinkang/GitHubPoster
 Author: malinkang
 Author-email: linkang.ma@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `github_heatmap-1.1.4/github_heatmap.egg-info/SOURCES.txt` & `github_heatmap-1.1.5/github_heatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `github_heatmap-1.1.4/setup.py` & `github_heatmap-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name="github_heatmap",
     author="malinkang",
     author_email="linkang.ma@gmail.com",
     url="https://github.com/malinkang/GitHubPoster",
     license="MIT",
-    version="1.1.4",
+    version="1.1.5",
     description="Make everything a GitHub svg poster and Skyline!",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "requests",
         "svgwrite",
         "pendulum==3.0.0",
```

### Comparing `github_heatmap-1.1.4/tests/test_poster_utils.py` & `github_heatmap-1.1.5/tests/test_poster_utils.py`

 * *Files identical despite different names*

