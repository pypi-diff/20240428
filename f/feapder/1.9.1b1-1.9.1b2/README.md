# Comparing `tmp/feapder-1.9.1b1.tar.gz` & `tmp/feapder-1.9.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feapder-1.9.1b1.tar", last modified: Mon Apr  8 04:47:30 2024, max compression
+gzip compressed data, was "feapder-1.9.1b2.tar", last modified: Sun Apr 28 08:05:12 2024, max compression
```

## Comparing `feapder-1.9.1b1.tar` & `feapder-1.9.1b2.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.773420 feapder-1.9.1b1/
--rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.9.1b1/LICENSE
--rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.9.1b1/MANIFEST.in
--rw-r--r--   0 liubo      (501) staff       (20)     4828 2024-04-08 04:47:30.773050 feapder-1.9.1b1/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     4382 2023-09-15 11:36:15.000000 feapder-1.9.1b1/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.594898 feapder-1.9.1b1/feapder/
--rw-r--r--   0 liubo      (501) staff       (20)       11 2024-04-08 04:47:09.000000 feapder-1.9.1b1/feapder/VERSION
--rw-r--r--   0 liubo      (501) staff       (20)      815 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.604452 feapder-1.9.1b1/feapder/buffer/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/buffer/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)    14555 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/buffer/item_buffer.py
--rw-r--r--   0 liubo      (501) staff       (20)     5436 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/buffer/request_buffer.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.609740 feapder-1.9.1b1/feapder/commands/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/commands/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/commands/cmdline.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.618214 feapder-1.9.1b1/feapder/commands/create/
--rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.9.1b1/feapder/commands/create/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/commands/create/create_cookies.py
--rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.9.1b1/feapder/commands/create/create_init.py
--rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.9.1b1/feapder/commands/create/create_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/commands/create/create_json.py
--rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.9.1b1/feapder/commands/create/create_params.py
--rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/commands/create/create_project.py
--rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/commands/create/create_setting.py
--rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.9.1b1/feapder/commands/create/create_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-06-28 09:14:30.000000 feapder-1.9.1b1/feapder/commands/create/create_table.py
--rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.9.1b1/feapder/commands/create_builder.py
--rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/commands/retry.py
--rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.9.1b1/feapder/commands/shell.py
--rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/commands/zip.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.626825 feapder-1.9.1b1/feapder/core/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/core/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6501 2024-03-18 02:39:32.000000 feapder-1.9.1b1/feapder/core/base_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)     3256 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/core/collector.py
--rw-r--r--   0 liubo      (501) staff       (20)     2807 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/core/handle_failed_items.py
--rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/core/handle_failed_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)    32962 2024-03-19 11:52:17.000000 feapder-1.9.1b1/feapder/core/parser_control.py
--rw-r--r--   0 liubo      (501) staff       (20)    21531 2024-03-19 12:14:49.000000 feapder-1.9.1b1/feapder/core/scheduler.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.633720 feapder-1.9.1b1/feapder/core/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.9.1b1/feapder/core/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     4395 2024-03-19 12:15:05.000000 feapder-1.9.1b1/feapder/core/spiders/air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-09-05 03:48:50.000000 feapder-1.9.1b1/feapder/core/spiders/batch_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/core/spiders/spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/core/spiders/task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.638615 feapder-1.9.1b1/feapder/db/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.9.1b1/feapder/db/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-06-28 09:14:30.000000 feapder-1.9.1b1/feapder/db/memorydb.py
--rw-r--r--   0 liubo      (501) staff       (20)    15961 2024-03-18 02:57:07.000000 feapder-1.9.1b1/feapder/db/mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)    10959 2024-04-08 04:45:21.000000 feapder-1.9.1b1/feapder/db/mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)    30873 2024-03-18 02:56:54.000000 feapder-1.9.1b1/feapder/db/redisdb.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.644278 feapder-1.9.1b1/feapder/dedup/
--rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/dedup/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/dedup/basefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     4511 2023-12-11 13:13:43.000000 feapder-1.9.1b1/feapder/dedup/bitarray.py
--rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/dedup/bloomfilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/dedup/expirefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/dedup/litefilter.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.653090 feapder-1.9.1b1/feapder/network/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/network/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.660464 feapder-1.9.1b1/feapder/network/downloader/
--rw-r--r--   0 liubo      (501) staff       (20)      299 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/network/downloader/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/downloader/_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.9.1b1/feapder/network/downloader/_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/downloader/_selenium.py
--rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.9.1b1/feapder/network/downloader/base.py
--rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.662831 feapder-1.9.1b1/feapder/network/proxy_pool/
--rw-r--r--   0 liubo      (501) staff       (20)      200 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/proxy_pool/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      797 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/proxy_pool/base.py
--rw-r--r--   0 liubo      (501) staff       (20)     2033 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/proxy_pool/proxy_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-08-18 08:40:56.000000 feapder-1.9.1b1/feapder/network/proxy_pool_old.py
--rw-r--r--   0 liubo      (501) staff       (20)    18070 2024-03-18 03:14:24.000000 feapder-1.9.1b1/feapder/network/request.py
--rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/network/response.py
--rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/selector.py
--rw-r--r--   0 liubo      (501) staff       (20)   130399 2023-06-28 08:50:40.000000 feapder-1.9.1b1/feapder/network/user_agent.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.667036 feapder-1.9.1b1/feapder/network/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/network/user_pool/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/network/user_pool/base_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/network/user_pool/gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     5377 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/network/user_pool/guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/network/user_pool/normal_user_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.670041 feapder-1.9.1b1/feapder/pipelines/
--rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.9.1b1/feapder/pipelines/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.9.1b1/feapder/pipelines/console_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.9.1b1/feapder/pipelines/mongo_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.9.1b1/feapder/pipelines/mysql_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)      363 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)    11184 2024-03-18 02:46:57.000000 feapder-1.9.1b1/feapder/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.675492 feapder-1.9.1b1/feapder/templates/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b1/feapder/templates/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/templates/air_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.9.1b1/feapder/templates/batch_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.9.1b1/feapder/templates/item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.679257 feapder-1.9.1b1/feapder/templates/project_template/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b1/feapder/templates/project_template/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/templates/project_template/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.679977 feapder-1.9.1b1/feapder/templates/project_template/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/templates/project_template/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.9.1b1/feapder/templates/project_template/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     9191 2024-03-18 02:47:28.000000 feapder-1.9.1b1/feapder/templates/project_template/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.680330 feapder-1.9.1b1/feapder/templates/project_template/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/templates/project_template/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/templates/spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.1b1/feapder/templates/task_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.9.1b1/feapder/templates/update_item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.687044 feapder-1.9.1b1/feapder/utils/
--rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.9.1b1/feapder/utils/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.9.1b1/feapder/utils/custom_argparse.py
--rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/utils/email_sender.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.690464 feapder-1.9.1b1/feapder/utils/js/
--rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/utils/js/intercept.js
--rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.9.1b1/feapder/utils/js/stealth.min.js
--rw-r--r--   0 liubo      (501) staff       (20)     8468 2023-06-28 09:47:12.000000 feapder-1.9.1b1/feapder/utils/log.py
--rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-06-28 09:14:32.000000 feapder-1.9.1b1/feapder/utils/metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.9.1b1/feapder/utils/perfect_dict.py
--rw-r--r--   0 liubo      (501) staff       (20)     3714 2023-11-22 02:36:32.000000 feapder-1.9.1b1/feapder/utils/redis_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)      796 2024-03-19 12:13:54.000000 feapder-1.9.1b1/feapder/utils/tail_thread.py
--rw-r--r--   0 liubo      (501) staff       (20)    74948 2024-03-18 02:46:57.000000 feapder-1.9.1b1/feapder/utils/tools.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.697296 feapder-1.9.1b1/feapder/utils/webdriver/
--rw-r--r--   0 liubo      (501) staff       (20)      380 2023-06-28 09:14:30.000000 feapder-1.9.1b1/feapder/utils/webdriver/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     9344 2023-08-18 08:40:56.000000 feapder-1.9.1b1/feapder/utils/webdriver/playwright_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)    18034 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/utils/webdriver/selenium_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)     2579 2023-09-15 11:36:15.000000 feapder-1.9.1b1/feapder/utils/webdriver/webdirver.py
--rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-06-28 09:14:31.000000 feapder-1.9.1b1/feapder/utils/webdriver/webdriver_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.600585 feapder-1.9.1b1/feapder.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     4828 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     6162 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)       61 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/entry_points.txt
--rw-r--r--   0 liubo      (501) staff       (20)      435 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)        8 2024-04-08 04:47:30.000000 feapder-1.9.1b1/feapder.egg-info/top_level.txt
--rw-r--r--   0 liubo      (501) staff       (20)       38 2024-04-08 04:47:30.773511 feapder-1.9.1b1/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)     2103 2023-09-15 11:36:15.000000 feapder-1.9.1b1/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.720090 feapder-1.9.1b1/tests/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.723770 feapder-1.9.1b1/tests/air-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     1218 2024-03-18 03:14:21.000000 feapder-1.9.1b1/tests/air-spider/test_air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-06-28 09:14:30.000000 feapder-1.9.1b1/tests/air-spider/test_air_spider_filter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/air-spider/test_air_spider_item.py
--rw-r--r--   0 liubo      (501) staff       (20)      648 2023-09-15 11:36:15.000000 feapder-1.9.1b1/tests/air-spider/test_render_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.727772 feapder-1.9.1b1/tests/batch-spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.737319 feapder-1.9.1b1/tests/batch-spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.9.1b1/tests/batch-spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.9.1b1/tests/batch-spider/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     2020 2023-06-09 12:31:43.000000 feapder-1.9.1b1/tests/batch-spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/batch-spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.739157 feapder-1.9.1b1/tests/batch-spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.9.1b1/tests/batch-spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1575 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/batch-spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.9.1b1/tests/batch-spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.731798 feapder-1.9.1b1/tests/batch-spider-integration/
--rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/batch-spider-integration/batch_spider_integration_task.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.732840 feapder-1.9.1b1/tests/batch-spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/batch-spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.9.1b1/tests/batch-spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/batch-spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.735652 feapder-1.9.1b1/tests/batch-spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/batch-spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/batch-spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/batch-spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.740019 feapder-1.9.1b1/tests/db/
--rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.9.1b1/tests/db/test_redis.py
--rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/jd_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.9.1b1/tests/mongo_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.742300 feapder-1.9.1b1/tests/spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.748578 feapder-1.9.1b1/tests/spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.9.1b1/tests/spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.9.1b1/tests/spider/items/spider_data_item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.749588 feapder-1.9.1b1/tests/spider/log/
--rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.9.1b1/tests/spider/log/haha.log
--rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.9.1b1/tests/spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2676 2024-01-09 02:59:22.000000 feapder-1.9.1b1/tests/spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.752646 feapder-1.9.1b1/tests/spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.9.1b1/tests/spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      985 2024-03-18 03:04:19.000000 feapder-1.9.1b1/tests/spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.9.1b1/tests/spider/spiders/test_spider2.py
--rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.9.1b1/tests/spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.743641 feapder-1.9.1b1/tests/spider-integration/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.744313 feapder-1.9.1b1/tests/spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.9.1b1/tests/spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.746754 feapder-1.9.1b1/tests/spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.1b1/tests/spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.9.1b1/tests/spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.9.1b1/tests/spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.753615 feapder-1.9.1b1/tests/task-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     2133 2024-03-18 02:54:15.000000 feapder-1.9.1b1/tests/task-spider/test_task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.757910 feapder-1.9.1b1/tests/test-debugger/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b1/tests/test-debugger/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)       81 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.759039 feapder-1.9.1b1/tests/test-debugger/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      352 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     8791 2023-09-15 11:36:15.000000 feapder-1.9.1b1/tests/test-debugger/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.760925 feapder-1.9.1b1/tests/test-debugger/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       33 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      724 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test-debugger/spiders/test_debugger.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.765163 feapder-1.9.1b1/tests/test-pipeline/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.766820 feapder-1.9.1b1/tests/test-pipeline/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.9.1b1/tests/test-pipeline/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.9.1b1/tests/test-pipeline/pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.9.1b1/tests/test-pipeline/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.768618 feapder-1.9.1b1/tests/test-pipeline/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.9.1b1/tests/test-pipeline/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.9.1b1/tests/test-pipeline/table.sql
--rw-r--r--   0 liubo      (501) staff       (20)      796 2023-09-19 02:11:49.000000 feapder-1.9.1b1/tests/test.py
--rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test_dedup.py
--rw-r--r--   0 liubo      (501) staff       (20)      991 2023-09-21 06:41:27.000000 feapder-1.9.1b1/tests/test_download_midware.py
--rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.9.1b1/tests/test_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)      329 2023-06-28 09:47:12.000000 feapder-1.9.1b1/tests/test_log.py
--rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-06-28 09:14:32.000000 feapder-1.9.1b1/tests/test_metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.9.1b1/tests/test_mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.9.1b1/tests/test_mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-06-28 09:14:31.000000 feapder-1.9.1b1/tests/test_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-06-28 09:14:30.000000 feapder-1.9.1b1/tests/test_playwright2.py
--rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.9.1b1/tests/test_rander.py
--rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.9.1b1/tests/test_rander2.py
--rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.9.1b1/tests/test_rander3.py
--rw-r--r--   0 liubo      (501) staff       (20)     1990 2023-09-15 11:36:15.000000 feapder-1.9.1b1/tests/test_rander_xhr.py
--rw-r--r--   0 liubo      (501) staff       (20)      148 2023-11-22 02:35:16.000000 feapder-1.9.1b1/tests/test_redisdb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.9.1b1/tests/test_request.py
--rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.9.1b1/tests/test_spider_params.py
--rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.9.1b1/tests/test_task.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.769438 feapder-1.9.1b1/tests/test_template/
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.1b1/tests/test_template/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.9.1b1/tests/test_tools.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.9.1b1/tests/test_webdriver.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-08 04:47:30.772086 feapder-1.9.1b1/tests/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.9.1b1/tests/user_pool/test_gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.9.1b1/tests/user_pool/test_guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.9.1b1/tests/user_pool/test_normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.581410 feapder-1.9.1b2/
+-rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.9.1b2/LICENSE
+-rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.9.1b2/MANIFEST.in
+-rw-r--r--   0 liubo      (501) staff       (20)     4828 2024-04-28 08:05:12.581075 feapder-1.9.1b2/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     4382 2023-09-15 11:36:15.000000 feapder-1.9.1b2/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.403723 feapder-1.9.1b2/feapder/
+-rw-r--r--   0 liubo      (501) staff       (20)       11 2024-04-28 08:04:50.000000 feapder-1.9.1b2/feapder/VERSION
+-rw-r--r--   0 liubo      (501) staff       (20)      815 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.413876 feapder-1.9.1b2/feapder/buffer/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.1b2/feapder/buffer/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    14555 2024-03-19 11:52:17.000000 feapder-1.9.1b2/feapder/buffer/item_buffer.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5436 2024-03-19 11:52:17.000000 feapder-1.9.1b2/feapder/buffer/request_buffer.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.419309 feapder-1.9.1b2/feapder/commands/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b2/feapder/commands/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/commands/cmdline.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.428911 feapder-1.9.1b2/feapder/commands/create/
+-rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.9.1b2/feapder/commands/create/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/commands/create/create_cookies.py
+-rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.9.1b2/feapder/commands/create/create_init.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.9.1b2/feapder/commands/create/create_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/commands/create/create_json.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.9.1b2/feapder/commands/create/create_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/commands/create/create_project.py
+-rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.9.1b2/feapder/commands/create/create_setting.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.9.1b2/feapder/commands/create/create_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-06-28 09:14:30.000000 feapder-1.9.1b2/feapder/commands/create/create_table.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.9.1b2/feapder/commands/create_builder.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/commands/retry.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.9.1b2/feapder/commands/shell.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/commands/zip.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.438423 feapder-1.9.1b2/feapder/core/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.9.1b2/feapder/core/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6501 2024-03-18 02:39:32.000000 feapder-1.9.1b2/feapder/core/base_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3256 2024-03-19 11:52:17.000000 feapder-1.9.1b2/feapder/core/collector.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2807 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/core/handle_failed_items.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/core/handle_failed_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)    32962 2024-03-19 11:52:17.000000 feapder-1.9.1b2/feapder/core/parser_control.py
+-rw-r--r--   0 liubo      (501) staff       (20)    21531 2024-03-19 12:14:49.000000 feapder-1.9.1b2/feapder/core/scheduler.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.446784 feapder-1.9.1b2/feapder/core/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.9.1b2/feapder/core/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4395 2024-03-19 12:15:05.000000 feapder-1.9.1b2/feapder/core/spiders/air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-09-05 03:48:50.000000 feapder-1.9.1b2/feapder/core/spiders/batch_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/core/spiders/spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/core/spiders/task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.454175 feapder-1.9.1b2/feapder/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.9.1b2/feapder/db/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-06-28 09:14:30.000000 feapder-1.9.1b2/feapder/db/memorydb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    15978 2024-04-28 08:03:33.000000 feapder-1.9.1b2/feapder/db/mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10959 2024-04-08 04:45:21.000000 feapder-1.9.1b2/feapder/db/mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    30873 2024-03-18 02:56:54.000000 feapder-1.9.1b2/feapder/db/redisdb.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.462067 feapder-1.9.1b2/feapder/dedup/
+-rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.9.1b2/feapder/dedup/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.9.1b2/feapder/dedup/basefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4511 2023-12-11 13:13:43.000000 feapder-1.9.1b2/feapder/dedup/bitarray.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.9.1b2/feapder/dedup/bloomfilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/dedup/expirefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/dedup/litefilter.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.469819 feapder-1.9.1b2/feapder/network/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b2/feapder/network/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.475839 feapder-1.9.1b2/feapder/network/downloader/
+-rw-r--r--   0 liubo      (501) staff       (20)      299 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/network/downloader/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/network/downloader/_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.9.1b2/feapder/network/downloader/_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/network/downloader/_selenium.py
+-rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.9.1b2/feapder/network/downloader/base.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/network/item.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.478521 feapder-1.9.1b2/feapder/network/proxy_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)      200 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/network/proxy_pool/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      797 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/network/proxy_pool/base.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2033 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/network/proxy_pool/proxy_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-08-18 08:40:56.000000 feapder-1.9.1b2/feapder/network/proxy_pool_old.py
+-rw-r--r--   0 liubo      (501) staff       (20)    18070 2024-03-18 03:14:24.000000 feapder-1.9.1b2/feapder/network/request.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/network/response.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/network/selector.py
+-rw-r--r--   0 liubo      (501) staff       (20)   130399 2023-06-28 08:50:40.000000 feapder-1.9.1b2/feapder/network/user_agent.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.482353 feapder-1.9.1b2/feapder/network/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/network/user_pool/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/network/user_pool/base_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/network/user_pool/gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5377 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/network/user_pool/guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/network/user_pool/normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.486309 feapder-1.9.1b2/feapder/pipelines/
+-rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.9.1b2/feapder/pipelines/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.9.1b2/feapder/pipelines/console_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.9.1b2/feapder/pipelines/mongo_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.9.1b2/feapder/pipelines/mysql_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)      363 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)    11219 2024-04-28 08:02:43.000000 feapder-1.9.1b2/feapder/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.493848 feapder-1.9.1b2/feapder/templates/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b2/feapder/templates/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/templates/air_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.9.1b2/feapder/templates/batch_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.9.1b2/feapder/templates/item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.498247 feapder-1.9.1b2/feapder/templates/project_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b2/feapder/templates/project_template/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.9.1b2/feapder/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.9.1b2/feapder/templates/project_template/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.499139 feapder-1.9.1b2/feapder/templates/project_template/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b2/feapder/templates/project_template/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.9.1b2/feapder/templates/project_template/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     9207 2024-04-28 08:04:08.000000 feapder-1.9.1b2/feapder/templates/project_template/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.499619 feapder-1.9.1b2/feapder/templates/project_template/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.9.1b2/feapder/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/templates/spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.1b2/feapder/templates/task_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.9.1b2/feapder/templates/update_item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.506756 feapder-1.9.1b2/feapder/utils/
+-rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.9.1b2/feapder/utils/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.9.1b2/feapder/utils/custom_argparse.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/utils/email_sender.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.509613 feapder-1.9.1b2/feapder/utils/js/
+-rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/utils/js/intercept.js
+-rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.9.1b2/feapder/utils/js/stealth.min.js
+-rw-r--r--   0 liubo      (501) staff       (20)     8468 2023-06-28 09:47:12.000000 feapder-1.9.1b2/feapder/utils/log.py
+-rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-06-28 09:14:32.000000 feapder-1.9.1b2/feapder/utils/metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.9.1b2/feapder/utils/perfect_dict.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3714 2023-11-22 02:36:32.000000 feapder-1.9.1b2/feapder/utils/redis_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)      796 2024-03-19 12:13:54.000000 feapder-1.9.1b2/feapder/utils/tail_thread.py
+-rw-r--r--   0 liubo      (501) staff       (20)    74948 2024-03-18 02:46:57.000000 feapder-1.9.1b2/feapder/utils/tools.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.515754 feapder-1.9.1b2/feapder/utils/webdriver/
+-rw-r--r--   0 liubo      (501) staff       (20)      380 2023-06-28 09:14:30.000000 feapder-1.9.1b2/feapder/utils/webdriver/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     9344 2023-08-18 08:40:56.000000 feapder-1.9.1b2/feapder/utils/webdriver/playwright_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)    18034 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/utils/webdriver/selenium_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2579 2023-09-15 11:36:15.000000 feapder-1.9.1b2/feapder/utils/webdriver/webdirver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-06-28 09:14:31.000000 feapder-1.9.1b2/feapder/utils/webdriver/webdriver_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.409472 feapder-1.9.1b2/feapder.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     4828 2024-04-28 08:05:12.000000 feapder-1.9.1b2/feapder.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     6162 2024-04-28 08:05:12.000000 feapder-1.9.1b2/feapder.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-28 08:05:12.000000 feapder-1.9.1b2/feapder.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       61 2024-04-28 08:05:12.000000 feapder-1.9.1b2/feapder.egg-info/entry_points.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      435 2024-04-28 08:05:12.000000 feapder-1.9.1b2/feapder.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        8 2024-04-28 08:05:12.000000 feapder-1.9.1b2/feapder.egg-info/top_level.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       38 2024-04-28 08:05:12.581496 feapder-1.9.1b2/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)     2103 2023-09-15 11:36:15.000000 feapder-1.9.1b2/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.534770 feapder-1.9.1b2/tests/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.539668 feapder-1.9.1b2/tests/air-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     1218 2024-03-18 03:14:21.000000 feapder-1.9.1b2/tests/air-spider/test_air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-06-28 09:14:30.000000 feapder-1.9.1b2/tests/air-spider/test_air_spider_filter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/air-spider/test_air_spider_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)      648 2023-09-15 11:36:15.000000 feapder-1.9.1b2/tests/air-spider/test_render_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.542911 feapder-1.9.1b2/tests/batch-spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.550072 feapder-1.9.1b2/tests/batch-spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.9.1b2/tests/batch-spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.9.1b2/tests/batch-spider/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2020 2023-06-09 12:31:43.000000 feapder-1.9.1b2/tests/batch-spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.9.1b2/tests/batch-spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.551595 feapder-1.9.1b2/tests/batch-spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.9.1b2/tests/batch-spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1575 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/batch-spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.9.1b2/tests/batch-spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.545458 feapder-1.9.1b2/tests/batch-spider-integration/
+-rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.9.1b2/tests/batch-spider-integration/batch_spider_integration_task.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.546160 feapder-1.9.1b2/tests/batch-spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.1b2/tests/batch-spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.9.1b2/tests/batch-spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.1b2/tests/batch-spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.548568 feapder-1.9.1b2/tests/batch-spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.1b2/tests/batch-spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/batch-spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/batch-spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.552368 feapder-1.9.1b2/tests/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.9.1b2/tests/db/test_redis.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/jd_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.9.1b2/tests/mongo_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.554618 feapder-1.9.1b2/tests/spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.560428 feapder-1.9.1b2/tests/spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.9.1b2/tests/spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.9.1b2/tests/spider/items/spider_data_item.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.561217 feapder-1.9.1b2/tests/spider/log/
+-rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.9.1b2/tests/spider/log/haha.log
+-rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.9.1b2/tests/spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2676 2024-01-09 02:59:22.000000 feapder-1.9.1b2/tests/spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.563522 feapder-1.9.1b2/tests/spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.9.1b2/tests/spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      985 2024-03-18 03:04:19.000000 feapder-1.9.1b2/tests/spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.9.1b2/tests/spider/spiders/test_spider2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.9.1b2/tests/spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.556179 feapder-1.9.1b2/tests/spider-integration/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.556923 feapder-1.9.1b2/tests/spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.9.1b2/tests/spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.9.1b2/tests/spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.9.1b2/tests/spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.558830 feapder-1.9.1b2/tests/spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.9.1b2/tests/spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.9.1b2/tests/spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.9.1b2/tests/spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.564316 feapder-1.9.1b2/tests/task-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     2133 2024-03-18 02:54:15.000000 feapder-1.9.1b2/tests/task-spider/test_task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.567755 feapder-1.9.1b2/tests/test-debugger/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.9.1b2/tests/test-debugger/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test-debugger/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.568578 feapder-1.9.1b2/tests/test-debugger/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test-debugger/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      352 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test-debugger/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8791 2023-09-15 11:36:15.000000 feapder-1.9.1b2/tests/test-debugger/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.569785 feapder-1.9.1b2/tests/test-debugger/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       33 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test-debugger/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      724 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test-debugger/spiders/test_debugger.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.573130 feapder-1.9.1b2/tests/test-pipeline/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.574852 feapder-1.9.1b2/tests/test-pipeline/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/test-pipeline/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/test-pipeline/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.9.1b2/tests/test-pipeline/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.9.1b2/tests/test-pipeline/pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.9.1b2/tests/test-pipeline/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.576498 feapder-1.9.1b2/tests/test-pipeline/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.9.1b2/tests/test-pipeline/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/test-pipeline/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.9.1b2/tests/test-pipeline/table.sql
+-rw-r--r--   0 liubo      (501) staff       (20)      796 2023-09-19 02:11:49.000000 feapder-1.9.1b2/tests/test.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test_dedup.py
+-rw-r--r--   0 liubo      (501) staff       (20)      991 2023-09-21 06:41:27.000000 feapder-1.9.1b2/tests/test_download_midware.py
+-rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.9.1b2/tests/test_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2023-06-28 09:47:12.000000 feapder-1.9.1b2/tests/test_log.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-06-28 09:14:32.000000 feapder-1.9.1b2/tests/test_metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.9.1b2/tests/test_mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.9.1b2/tests/test_mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-06-28 09:14:31.000000 feapder-1.9.1b2/tests/test_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-06-28 09:14:30.000000 feapder-1.9.1b2/tests/test_playwright2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.9.1b2/tests/test_rander.py
+-rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.9.1b2/tests/test_rander2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.9.1b2/tests/test_rander3.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1990 2023-09-15 11:36:15.000000 feapder-1.9.1b2/tests/test_rander_xhr.py
+-rw-r--r--   0 liubo      (501) staff       (20)      148 2023-11-22 02:35:16.000000 feapder-1.9.1b2/tests/test_redisdb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.9.1b2/tests/test_request.py
+-rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.9.1b2/tests/test_spider_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.9.1b2/tests/test_task.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.577500 feapder-1.9.1b2/tests/test_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.9.1b2/tests/test_template/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.9.1b2/tests/test_tools.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.9.1b2/tests/test_webdriver.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-28 08:05:12.580253 feapder-1.9.1b2/tests/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.9.1b2/tests/user_pool/test_gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.9.1b2/tests/user_pool/test_guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.9.1b2/tests/user_pool/test_normal_user_pool.py
```

### Comparing `feapder-1.9.1b1/LICENSE` & `feapder-1.9.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/PKG-INFO` & `feapder-1.9.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.9.1b1
+Version: 1.9.1b2
 Summary: feapder是一款支持分布式、批次采集、数据防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.9.1b1/README.md` & `feapder-1.9.1b2/README.md`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/__init__.py` & `feapder-1.9.1b2/feapder/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/buffer/item_buffer.py` & `feapder-1.9.1b2/feapder/buffer/item_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/buffer/request_buffer.py` & `feapder-1.9.1b2/feapder/buffer/request_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/cmdline.py` & `feapder-1.9.1b2/feapder/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/__init__.py` & `feapder-1.9.1b2/feapder/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_cookies.py` & `feapder-1.9.1b2/feapder/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_init.py` & `feapder-1.9.1b2/feapder/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_item.py` & `feapder-1.9.1b2/feapder/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_json.py` & `feapder-1.9.1b2/feapder/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_params.py` & `feapder-1.9.1b2/feapder/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_project.py` & `feapder-1.9.1b2/feapder/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_setting.py` & `feapder-1.9.1b2/feapder/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_spider.py` & `feapder-1.9.1b2/feapder/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create/create_table.py` & `feapder-1.9.1b2/feapder/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/create_builder.py` & `feapder-1.9.1b2/feapder/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/retry.py` & `feapder-1.9.1b2/feapder/commands/retry.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/shell.py` & `feapder-1.9.1b2/feapder/commands/shell.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/commands/zip.py` & `feapder-1.9.1b2/feapder/commands/zip.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/base_parser.py` & `feapder-1.9.1b2/feapder/core/base_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/collector.py` & `feapder-1.9.1b2/feapder/core/collector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/handle_failed_items.py` & `feapder-1.9.1b2/feapder/core/handle_failed_items.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/handle_failed_requests.py` & `feapder-1.9.1b2/feapder/core/handle_failed_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/parser_control.py` & `feapder-1.9.1b2/feapder/core/parser_control.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/scheduler.py` & `feapder-1.9.1b2/feapder/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/spiders/air_spider.py` & `feapder-1.9.1b2/feapder/core/spiders/air_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/spiders/batch_spider.py` & `feapder-1.9.1b2/feapder/core/spiders/batch_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/spiders/spider.py` & `feapder-1.9.1b2/feapder/core/spiders/spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/core/spiders/task_spider.py` & `feapder-1.9.1b2/feapder/core/spiders/task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/db/memorydb.py` & `feapder-1.9.1b2/feapder/db/memorydb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/db/mongodb.py` & `feapder-1.9.1b2/feapder/db/mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,30 @@
         port=None,
         db=None,
         user_name=None,
         user_pass=None,
         url=None,
         **kwargs,
     ):
+        if not ip:
+            ip = setting.MONGO_IP
+        if not port:
+            port = setting.MONGO_PORT
+        if not db:
+            db = setting.MONGO_DB
+        if not user_name:
+            user_name = setting.MONGO_USER_NAME
+        if not user_pass:
+            user_pass = setting.MONGO_USER_PASS
+        if not url:
+            url = setting.MONGO_URL
+
         if url:
             self.client = MongoClient(url, **kwargs)
         else:
-            if not ip:
-                ip = setting.MONGO_IP
-            if not port:
-                port = setting.MONGO_PORT
-            if not db:
-                db = setting.MONGO_DB
-            if not user_name:
-                user_name = setting.MONGO_USER_NAME
-            if not user_pass:
-                user_pass = setting.MONGO_USER_PASS
             self.client = MongoClient(
                 host=ip, port=port, username=user_name, password=user_pass
             )
 
         self.db = self.get_database(db)
 
         # 缓存索引信息
```

### Comparing `feapder-1.9.1b1/feapder/db/mysqldb.py` & `feapder-1.9.1b2/feapder/db/mysqldb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/db/redisdb.py` & `feapder-1.9.1b2/feapder/db/redisdb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/dedup/__init__.py` & `feapder-1.9.1b2/feapder/dedup/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/dedup/basefilter.py` & `feapder-1.9.1b2/feapder/dedup/basefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/dedup/bitarray.py` & `feapder-1.9.1b2/feapder/dedup/bitarray.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/dedup/bloomfilter.py` & `feapder-1.9.1b2/feapder/dedup/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/dedup/expirefilter.py` & `feapder-1.9.1b2/feapder/dedup/expirefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/dedup/litefilter.py` & `feapder-1.9.1b2/feapder/dedup/litefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/downloader/_playwright.py` & `feapder-1.9.1b2/feapder/network/downloader/_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/downloader/_requests.py` & `feapder-1.9.1b2/feapder/network/downloader/_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/downloader/_selenium.py` & `feapder-1.9.1b2/feapder/network/downloader/_selenium.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/downloader/base.py` & `feapder-1.9.1b2/feapder/network/downloader/base.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/item.py` & `feapder-1.9.1b2/feapder/network/item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/proxy_pool/base.py` & `feapder-1.9.1b2/feapder/network/proxy_pool/base.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/proxy_pool/proxy_pool.py` & `feapder-1.9.1b2/feapder/network/proxy_pool/proxy_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/proxy_pool_old.py` & `feapder-1.9.1b2/feapder/network/proxy_pool_old.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/request.py` & `feapder-1.9.1b2/feapder/network/request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/response.py` & `feapder-1.9.1b2/feapder/network/response.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/selector.py` & `feapder-1.9.1b2/feapder/network/selector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/user_agent.py` & `feapder-1.9.1b2/feapder/network/user_agent.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/user_pool/base_user_pool.py` & `feapder-1.9.1b2/feapder/network/user_pool/base_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/user_pool/gold_user_pool.py` & `feapder-1.9.1b2/feapder/network/user_pool/gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/user_pool/guest_user_pool.py` & `feapder-1.9.1b2/feapder/network/user_pool/guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/network/user_pool/normal_user_pool.py` & `feapder-1.9.1b2/feapder/network/user_pool/normal_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/pipelines/__init__.py` & `feapder-1.9.1b2/feapder/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/pipelines/console_pipeline.py` & `feapder-1.9.1b2/feapder/pipelines/console_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/pipelines/mongo_pipeline.py` & `feapder-1.9.1b2/feapder/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/pipelines/mysql_pipeline.py` & `feapder-1.9.1b2/feapder/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/setting.py` & `feapder-1.9.1b2/feapder/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 # MONGODB
 MONGO_IP = os.getenv("MONGO_IP", "localhost")
 MONGO_PORT = int(os.getenv("MONGO_PORT", 27017))
 MONGO_DB = os.getenv("MONGO_DB")
 MONGO_USER_NAME = os.getenv("MONGO_USER_NAME")
 MONGO_USER_PASS = os.getenv("MONGO_USER_PASS")
+MONGO_URL = os.getenv("MONGO_URL")
 
 # REDIS
 # ip:port 多个可写为列表或者逗号隔开 如 ip1:port1,ip2:port2 或 ["ip1:port1", "ip2:port2"]
 REDISDB_IP_PORTS = os.getenv("REDISDB_IP_PORTS")
 REDISDB_USER_PASS = os.getenv("REDISDB_USER_PASS")
 REDISDB_DB = int(os.getenv("REDISDB_DB", 0))
 # 连接redis时携带的其他参数，如ssl=True
```

### Comparing `feapder-1.9.1b1/feapder/templates/.DS_Store` & `feapder-1.9.1b2/feapder/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/air_spider_template.tmpl` & `feapder-1.9.1b2/feapder/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/batch_spider_template.tmpl` & `feapder-1.9.1b2/feapder/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/project_template/.DS_Store` & `feapder-1.9.1b2/feapder/templates/project_template/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/project_template/CHECK_DATA.md` & `feapder-1.9.1b2/feapder/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/project_template/main.py` & `feapder-1.9.1b2/feapder/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/project_template/setting.py` & `feapder-1.9.1b2/feapder/templates/project_template/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 # # MONGODB
 # MONGO_IP = "localhost"
 # MONGO_PORT = 27017
 # MONGO_DB = ""
 # MONGO_USER_NAME = ""
 # MONGO_USER_PASS = ""
+# MONGO_URL = "
 #
 # # REDIS
 # # ip:port 多个可写为列表或者逗号隔开 如 ip1:port1,ip2:port2 或 ["ip1:port1", "ip2:port2"]
 # REDISDB_IP_PORTS = "localhost:6379"
 # REDISDB_USER_PASS = ""
 # REDISDB_DB = 0
 # # 连接redis时携带的其他参数，如ssl=True
```

### Comparing `feapder-1.9.1b1/feapder/templates/spider_template.tmpl` & `feapder-1.9.1b2/feapder/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/templates/task_spider_template.tmpl` & `feapder-1.9.1b2/feapder/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/custom_argparse.py` & `feapder-1.9.1b2/feapder/utils/custom_argparse.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/email_sender.py` & `feapder-1.9.1b2/feapder/utils/email_sender.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/js/intercept.js` & `feapder-1.9.1b2/feapder/utils/js/intercept.js`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/js/stealth.min.js` & `feapder-1.9.1b2/feapder/utils/js/stealth.min.js`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/log.py` & `feapder-1.9.1b2/feapder/utils/log.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/metrics.py` & `feapder-1.9.1b2/feapder/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/perfect_dict.py` & `feapder-1.9.1b2/feapder/utils/perfect_dict.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/redis_lock.py` & `feapder-1.9.1b2/feapder/utils/redis_lock.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/tail_thread.py` & `feapder-1.9.1b2/feapder/utils/tail_thread.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/tools.py` & `feapder-1.9.1b2/feapder/utils/tools.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/webdriver/playwright_driver.py` & `feapder-1.9.1b2/feapder/utils/webdriver/playwright_driver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/webdriver/selenium_driver.py` & `feapder-1.9.1b2/feapder/utils/webdriver/selenium_driver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/webdriver/webdirver.py` & `feapder-1.9.1b2/feapder/utils/webdriver/webdirver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder/utils/webdriver/webdriver_pool.py` & `feapder-1.9.1b2/feapder/utils/webdriver/webdriver_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/feapder.egg-info/PKG-INFO` & `feapder-1.9.1b2/feapder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.9.1b1
+Version: 1.9.1b2
 Summary: feapder是一款支持分布式、批次采集、数据防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.9.1b1/feapder.egg-info/SOURCES.txt` & `feapder-1.9.1b2/feapder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/setup.py` & `feapder-1.9.1b2/setup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/air-spider/test_air_spider.py` & `feapder-1.9.1b2/tests/air-spider/test_air_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/air-spider/test_air_spider_filter.py` & `feapder-1.9.1b2/tests/air-spider/test_air_spider_filter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/air-spider/test_air_spider_item.py` & `feapder-1.9.1b2/tests/air-spider/test_air_spider_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/air-spider/test_render_spider.py` & `feapder-1.9.1b2/tests/air-spider/test_render_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider/items/spider_data_item.py` & `feapder-1.9.1b2/tests/batch-spider/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider/main.py` & `feapder-1.9.1b2/tests/batch-spider/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider/setting.py` & `feapder-1.9.1b2/tests/batch-spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider/spiders/test_spider.py` & `feapder-1.9.1b2/tests/batch-spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider/table.sql` & `feapder-1.9.1b2/tests/batch-spider/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider-integration/batch_spider_integration_task.sql` & `feapder-1.9.1b2/tests/batch-spider-integration/batch_spider_integration_task.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider-integration/main.py` & `feapder-1.9.1b2/tests/batch-spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider-integration/setting.py` & `feapder-1.9.1b2/tests/batch-spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider-integration/spiders/sina_news_parser.py` & `feapder-1.9.1b2/tests/batch-spider-integration/spiders/sina_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/batch-spider-integration/spiders/tencent_news_parser.py` & `feapder-1.9.1b2/tests/batch-spider-integration/spiders/tencent_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/jd_spider.py` & `feapder-1.9.1b2/tests/jd_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/mongo_spider.py` & `feapder-1.9.1b2/tests/mongo_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/spider/log/haha.log` & `feapder-1.9.1b2/tests/spider/log/haha.log`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/spider/setting.py` & `feapder-1.9.1b2/tests/spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/spider/spiders/test_spider.py` & `feapder-1.9.1b2/tests/spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/spider/spiders/test_spider2.py` & `feapder-1.9.1b2/tests/spider/spiders/test_spider2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/spider-integration/main.py` & `feapder-1.9.1b2/tests/spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/spider-integration/setting.py` & `feapder-1.9.1b2/tests/spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/task-spider/test_task_spider.py` & `feapder-1.9.1b2/tests/task-spider/test_task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-debugger/.DS_Store` & `feapder-1.9.1b2/tests/test-debugger/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-debugger/setting.py` & `feapder-1.9.1b2/tests/test-debugger/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-debugger/spiders/test_debugger.py` & `feapder-1.9.1b2/tests/test-debugger/spiders/test_debugger.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-pipeline/items/spider_data_item.py` & `feapder-1.9.1b2/tests/test-pipeline/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-pipeline/main.py` & `feapder-1.9.1b2/tests/test-pipeline/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-pipeline/pipeline.py` & `feapder-1.9.1b2/tests/test-pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-pipeline/setting.py` & `feapder-1.9.1b2/tests/test-pipeline/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-pipeline/spiders/test_spider.py` & `feapder-1.9.1b2/tests/test-pipeline/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test-pipeline/table.sql` & `feapder-1.9.1b2/tests/test-pipeline/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test.py` & `feapder-1.9.1b2/tests/test.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_dedup.py` & `feapder-1.9.1b2/tests/test_dedup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_download_midware.py` & `feapder-1.9.1b2/tests/test_download_midware.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_metrics.py` & `feapder-1.9.1b2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_mongodb.py` & `feapder-1.9.1b2/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_playwright.py` & `feapder-1.9.1b2/tests/test_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_playwright2.py` & `feapder-1.9.1b2/tests/test_playwright2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_rander.py` & `feapder-1.9.1b2/tests/test_rander.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_rander2.py` & `feapder-1.9.1b2/tests/test_rander2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_rander3.py` & `feapder-1.9.1b2/tests/test_rander3.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_rander_xhr.py` & `feapder-1.9.1b2/tests/test_rander_xhr.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_request.py` & `feapder-1.9.1b2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_spider_params.py` & `feapder-1.9.1b2/tests/test_spider_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_task.py` & `feapder-1.9.1b2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_template/test_spider.py` & `feapder-1.9.1b2/tests/test_template/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/test_webdriver.py` & `feapder-1.9.1b2/tests/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/user_pool/test_gold_user_pool.py` & `feapder-1.9.1b2/tests/user_pool/test_gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/user_pool/test_guest_user_pool.py` & `feapder-1.9.1b2/tests/user_pool/test_guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.9.1b1/tests/user_pool/test_normal_user_pool.py` & `feapder-1.9.1b2/tests/user_pool/test_normal_user_pool.py`

 * *Files identical despite different names*

