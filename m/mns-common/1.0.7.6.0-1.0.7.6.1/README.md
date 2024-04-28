# Comparing `tmp/mns_common-1.0.7.6.0.tar.gz` & `tmp/mns_common-1.0.7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.7.6.0.tar", last modified: Sun Apr 28 03:07:57 2024, max compression
+gzip compressed data, was "mns_common-1.0.7.6.1.tar", last modified: Sun Apr 28 04:36:50 2024, max compression
```

## Comparing `mns_common-1.0.7.6.0.tar` & `mns_common-1.0.7.6.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.990888 mns_common-1.0.7.6.0/
--rw-rw-rw-   0        0        0       61 2024-04-28 03:07:57.989891 mns_common-1.0.7.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.948004 mns_common-1.0.7.6.0/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.6.0/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.949998 mns_common-1.0.7.6.0/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.6.0/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.954985 mns_common-1.0.7.6.0/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.956980 mns_common-1.0.7.6.0/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.6.0/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-12-18 12:33:18.000000 mns_common-1.0.7.6.0/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0    12619 2023-12-18 12:33:18.000000 mns_common-1.0.7.6.0/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.957977 mns_common-1.0.7.6.0/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.958974 mns_common-1.0.7.6.0/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.959972 mns_common-1.0.7.6.0/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.960969 mns_common-1.0.7.6.0/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.961966 mns_common-1.0.7.6.0/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.962964 mns_common-1.0.7.6.0/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.964958 mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.965956 mns_common-1.0.7.6.0/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.6.0/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.968948 mns_common-1.0.7.6.0/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.6.0/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.0/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.7.6.0/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.6.0/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.969944 mns_common-1.0.7.6.0/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.6.0/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.970942 mns_common-1.0.7.6.0/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.6.0/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.6.0/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.6.0/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.6.0/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.971940 mns_common-1.0.7.6.0/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.6.0/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.972937 mns_common-1.0.7.6.0/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     2626 2024-04-23 08:59:18.000000 mns_common-1.0.7.6.0/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9578 2024-04-24 06:12:21.000000 mns_common-1.0.7.6.0/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.973935 mns_common-1.0.7.6.0/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2023-12-17 11:33:58.000000 mns_common-1.0.7.6.0/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.6.0/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.974931 mns_common-1.0.7.6.0/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.6.0/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.6.0/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.975929 mns_common-1.0.7.6.0/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.976926 mns_common-1.0.7.6.0/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.977924 mns_common-1.0.7.6.0/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.979918 mns_common-1.0.7.6.0/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.6.0/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.980915 mns_common-1.0.7.6.0/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/real_time/real_time_common_service_api.py
--rw-rw-rw-   0        0        0     1034 2024-01-05 08:29:27.000000 mns_common-1.0.7.6.0/mns_common/component/real_time/real_time_symbol_bid_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.981913 mns_common-1.0.7.6.0/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.7.6.0/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     1436 2024-04-28 03:04:11.000000 mns_common-1.0.7.6.0/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.982910 mns_common-1.0.7.6.0/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.6.0/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.983908 mns_common-1.0.7.6.0/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.0/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.6.0/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.985902 mns_common-1.0.7.6.0/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.6.0/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-04-21 02:57:24.000000 mns_common-1.0.7.6.0/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.6.0/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.6.0/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.986899 mns_common-1.0.7.6.0/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.7.6.0/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.6.0/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.988894 mns_common-1.0.7.6.0/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.6.0/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.6.0/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.6.0/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.6.0/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.6.0/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:07:57.989891 mns_common-1.0.7.6.0/mns_common.egg-info/
--rw-rw-rw-   0        0        0       61 2024-04-28 03:07:57.000000 mns_common-1.0.7.6.0/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3603 2024-04-28 03:07:57.000000 mns_common-1.0.7.6.0/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 03:07:57.000000 mns_common-1.0.7.6.0/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-28 03:07:57.000000 mns_common-1.0.7.6.0/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 03:07:57.990888 mns_common-1.0.7.6.0/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-04-28 03:07:56.000000 mns_common-1.0.7.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.846086 mns_common-1.0.7.6.1/
+-rw-rw-rw-   0        0        0       61 2024-04-28 04:36:50.846086 mns_common-1.0.7.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.799985 mns_common-1.0.7.6.1/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.6.1/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.802978 mns_common-1.0.7.6.1/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.6.1/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.805970 mns_common-1.0.7.6.1/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.808962 mns_common-1.0.7.6.1/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.6.1/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-12-18 12:33:18.000000 mns_common-1.0.7.6.1/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0    12619 2023-12-18 12:33:18.000000 mns_common-1.0.7.6.1/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.809959 mns_common-1.0.7.6.1/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.810956 mns_common-1.0.7.6.1/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.812197 mns_common-1.0.7.6.1/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.813175 mns_common-1.0.7.6.1/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.814172 mns_common-1.0.7.6.1/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.815170 mns_common-1.0.7.6.1/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.817164 mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.818160 mns_common-1.0.7.6.1/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.6.1/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.821153 mns_common-1.0.7.6.1/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.6.1/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.6.1/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.7.6.1/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.6.1/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.822149 mns_common-1.0.7.6.1/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.6.1/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.823148 mns_common-1.0.7.6.1/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.6.1/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.6.1/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.6.1/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.6.1/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.825142 mns_common-1.0.7.6.1/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.6.1/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.826139 mns_common-1.0.7.6.1/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     2626 2024-04-23 08:59:18.000000 mns_common-1.0.7.6.1/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9578 2024-04-24 06:12:21.000000 mns_common-1.0.7.6.1/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.828134 mns_common-1.0.7.6.1/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2023-12-17 11:33:58.000000 mns_common-1.0.7.6.1/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.6.1/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.829131 mns_common-1.0.7.6.1/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.6.1/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.6.1/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.829131 mns_common-1.0.7.6.1/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.831125 mns_common-1.0.7.6.1/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.832123 mns_common-1.0.7.6.1/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.834118 mns_common-1.0.7.6.1/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.6.1/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.836112 mns_common-1.0.7.6.1/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/real_time/real_time_common_service_api.py
+-rw-rw-rw-   0        0        0     1034 2024-01-05 08:29:27.000000 mns_common-1.0.7.6.1/mns_common/component/real_time/real_time_symbol_bid_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.837111 mns_common-1.0.7.6.1/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.7.6.1/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     1599 2024-04-28 03:51:48.000000 mns_common-1.0.7.6.1/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.838108 mns_common-1.0.7.6.1/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.6.1/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.839104 mns_common-1.0.7.6.1/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.6.1/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.6.1/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.841098 mns_common-1.0.7.6.1/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.6.1/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1393 2024-04-28 04:36:28.000000 mns_common-1.0.7.6.1/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.6.1/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.6.1/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.842096 mns_common-1.0.7.6.1/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.7.6.1/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.6.1/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.845088 mns_common-1.0.7.6.1/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.6.1/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.6.1/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.6.1/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.6.1/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.6.1/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:36:50.845088 mns_common-1.0.7.6.1/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       61 2024-04-28 04:36:50.000000 mns_common-1.0.7.6.1/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3603 2024-04-28 04:36:50.000000 mns_common-1.0.7.6.1/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 04:36:50.000000 mns_common-1.0.7.6.1/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-28 04:36:50.000000 mns_common-1.0.7.6.1/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 04:36:50.846086 mns_common-1.0.7.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-04-28 04:36:28.000000 mns_common-1.0.7.6.1/setup.py
```

### Comparing `mns_common-1.0.7.6.0/README.md` & `mns_common-1.0.7.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.7.6.1/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.7.6.1/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.7.6.1/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.7.6.1/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.7.6.1/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.7.6.1/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.7.6.1/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.7.6.1/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.7.6.1/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.7.6.1/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.7.6.1/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.7.6.1/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.7.6.1/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.7.6.1/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.7.6.1/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.7.6.1/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.7.6.1/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.7.6.1/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/data/data_init_api.py` & `mns_common-1.0.7.6.1/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.7.6.1/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.7.6.1/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/real_time/real_time_symbol_bid_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/real_time/real_time_symbol_bid_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/trade/trade_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/trade/trade_service_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 14
 project_path = file_path[0:end]
 sys.path.append(project_path)
 from loguru import logger
 import easytrader
+from easytrader import grid_strategies
 
 user = easytrader.use('ths')
 user.connect(r'D:\Program Files\ths\xiadan.exe')
+user.grid_strategy = grid_strategies.Xls
+user.grid_strategy_instance.tmp_folder = 'C:\\custom_folder'
 
 
 # 下单
 def order_buy(symbol, buy_price, buy_volume):
     logger.warning("买入代码:{},买入价格:{},买入数量:{}", symbol, buy_price, buy_volume)
     user.enable_type_keys_for_editor()
     buy_result = user.buy(symbol, buy_price, buy_volume)
@@ -42,14 +45,15 @@
 def order_cancel(entrust_no):
     user.enable_type_keys_for_editor()
     cancel_result = user.cancel_entrust(entrust_no)
     return cancel_result
 
 
 if __name__ == '__main__':
+    # while True:
     position_df = get_position()
     print(position_df)
     # buy_result_df = order_buy('300085', '10.28', 1000)
     # print(buy_result_df)
     # auto_ipo_buy()
     # cancel_result_df = order_cancel('0111735004')
     # print(cancel_result_df)
```

### Comparing `mns_common-1.0.7.6.0/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.7.6.1/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/constant/db_name_constant.py` & `mns_common-1.0.7.6.1/mns_common/constant/db_name_constant.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,7 +39,10 @@
 TODAY_NEW_CONCEPT_LIST = 'today_new_concept_list'
 
 # 开票啦历史数据
 KPL_BEST_CHOOSE_HIS = 'kpl_best_choose_his'
 
 # 开票啦每日数据
 KPL_BEST_CHOOSE_DAILY = 'kpl_best_choose_daily'
+
+# 当前持仓股票
+POSITION_STOCK = 'position_stock'
```

### Comparing `mns_common-1.0.7.6.0/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.7.6.1/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.7.6.1/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/db/MongodbUtil.py` & `mns_common-1.0.7.6.1/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/utils/data_frame_util.py` & `mns_common-1.0.7.6.1/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common/utils/date_handle_util.py` & `mns_common-1.0.7.6.1/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.6.0/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.7.6.1/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

