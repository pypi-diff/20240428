# Comparing `tmp/buildz-0.5.2.tar.gz` & `tmp/buildz-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.2.tar", last modified: Thu Apr 25 17:53:28 2024, max compression
+gzip compressed data, was "buildz-0.5.3.tar", last modified: Sun Apr 28 15:57:38 2024, max compression
```

## Comparing `buildz-0.5.2.tar` & `buildz-0.5.3.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.043943 buildz-0.5.2/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.2/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2705 2024-04-25 17:53:28.043943 buildz-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.968517 buildz-0.5.2/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.2/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.2/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.5.2/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.971522 buildz-0.5.2/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.972522 buildz-0.5.2/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.2/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.2/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.973522 buildz-0.5.2/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.5.2/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.2/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.974522 buildz-0.5.2/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.976521 buildz-0.5.2/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.2/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.2/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.2/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.2/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.2/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.979522 buildz-0.5.2/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.2/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.2/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.2/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.2/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.2/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.2/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.980522 buildz-0.5.2/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.2/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.2/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.2/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.981521 buildz-0.5.2/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.2/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.2/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.984522 buildz-0.5.2/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.2/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.2/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.5.2/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.2/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.986538 buildz-0.5.2/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.2/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.2/buildz/ioc/base.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.2/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.988521 buildz-0.5.2/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.2/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.2/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.2/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.998942 buildz-0.5.2/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.2/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.010942 buildz-0.5.2/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.2/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      828 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      932 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1021 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6134 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1087 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.2/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1082 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.2/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.011942 buildz-0.5.2/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.2/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.2/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.017943 buildz-0.5.2/buildz/xf/
--rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.2/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.2/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0      960 2024-04-25 14:34:17.000000 buildz-0.5.2/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.020942 buildz-0.5.2/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.2/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.2/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.026943 buildz-0.5.2/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.2/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.2/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.2/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.2/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.2/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.2/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.2/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.2/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.2/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.2/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.2/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.2/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.2/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.2/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.030942 buildz-0.5.2/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-16 13:01:38.000000 buildz-0.5.2/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.2/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.035943 buildz-0.5.2/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      533 2024-04-16 10:23:04.000000 buildz-0.5.2/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     1787 2024-04-16 12:27:38.000000 buildz-0.5.2/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.2/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0      699 2024-04-16 10:17:43.000000 buildz-0.5.2/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      452 2024-04-16 12:57:03.000000 buildz-0.5.2/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      691 2024-04-16 13:02:05.000000 buildz-0.5.2/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.2/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.2/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.2/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.5.2/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.2/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.2/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     3032 2024-04-25 17:50:27.000000 buildz-0.5.2/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.2/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1751 2024-04-25 17:51:42.000000 buildz-0.5.2/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0     2009 2024-04-23 09:07:57.000000 buildz-0.5.2/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.2/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2746 2024-04-25 17:36:02.000000 buildz-0.5.2/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.2/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1477 2024-04-25 14:36:40.000000 buildz-0.5.2/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.039943 buildz-0.5.2/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.2/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.2/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.042942 buildz-0.5.2/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.2/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.2/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.2/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.2/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.2/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.2/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.2/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.2/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.970522 buildz-0.5.2/buildz.egg-info/
--rw-rw-rw-   0        0        0     2705 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3724 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 17:53:28.043943 buildz-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-25 17:52:05.000000 buildz-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2705 2024-04-28 15:57:38.417507 buildz-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.323733 buildz-0.5.3/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.3/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.3/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.5.3/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.3/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.3/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.5.3/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.3/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.3/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.3/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.3/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.3/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.3/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.3/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.3/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.3/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.3/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.3/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.3/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.3/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.3/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.3/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.3/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.3/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.3/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.3/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.5.3/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.3/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.3/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.3/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.3/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.3/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.3/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.3/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.370605 buildz-0.5.3/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.3/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.386231 buildz-0.5.3/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.3/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      828 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      932 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1021 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6134 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1087 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.3/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1082 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.3/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.386231 buildz-0.5.3/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.3/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.3/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.386231 buildz-0.5.3/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.3/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.3/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0      960 2024-04-25 14:34:17.000000 buildz-0.5.3/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.401853 buildz-0.5.3/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.3/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.3/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.401853 buildz-0.5.3/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.3/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.3/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.3/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.3/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.3/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.3/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.3/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.3/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.3/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.3/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.3/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.3/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.3/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.3/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.401853 buildz-0.5.3/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.3/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.3/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.3/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     2055 2024-04-26 07:39:31.000000 buildz-0.5.3/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.3/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.3/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.3/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.3/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.3/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.3/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.3/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.5.3/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.3/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.3/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3515 2024-04-26 08:09:20.000000 buildz-0.5.3/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.3/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.3/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.3/buildz/xf/loaderz/test1.py
+-rw-rw-rw-   0        0        0     2009 2024-04-23 09:07:57.000000 buildz-0.5.3/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.3/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2746 2024-04-25 17:36:02.000000 buildz-0.5.3/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.3/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-04-25 14:36:40.000000 buildz-0.5.3/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.3/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.3/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.3/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.3/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.3/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.3/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.3/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.3/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.3/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.3/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2705 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3751 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 15:57:38.417507 buildz-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-28 15:56:06.000000 buildz-0.5.3/setup.py
```

### Comparing `buildz-0.5.2/LICENSE` & `buildz-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/PKG-INFO` & `buildz-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.2
+Version: 0.5.3
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.2/README.md` & `buildz-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/argx.py` & `buildz-0.5.3/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/ioc/deal.py` & `buildz-0.5.3/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/ioc/help.py` & `buildz-0.5.3/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/myers/deal.py` & `buildz-0.5.3/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/res/conf/main.js` & `buildz-0.5.3/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/res/help/ioc.js` & `buildz-0.5.3/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/res/help/myers.js` & `buildz-0.5.3/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/res/help/search.js` & `buildz-0.5.3/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/res/help/xf.js` & `buildz-0.5.3/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/res/test.js` & `buildz-0.5.3/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/search/deal.py` & `buildz-0.5.3/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/demo/test.py` & `buildz-0.5.3/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/fz/dirz.py` & `buildz-0.5.3/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/fz/fio.py` & `buildz-0.5.3/buildz/fz/fio.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/fz/lsf.py` & `buildz-0.5.3/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc/base.py` & `buildz-0.5.3/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc/conf.py` & `buildz-0.5.3/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc/confs.py` & `buildz-0.5.3/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.3/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/ioc/ioc_deal/xfile.py` & `buildz-0.5.3/buildz/ioc/ioc_deal/xfile.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/pyz.py` & `buildz-0.5.3/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/tz/myers_diff.py` & `buildz-0.5.3/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/file.py` & `buildz-0.5.3/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/base.py` & `buildz-0.5.3/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/buffer.py` & `buildz-0.5.3/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/listz.py` & `buildz-0.5.3/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/lr.py` & `buildz-0.5.3/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.3/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.3/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.3/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/reval.py` & `buildz-0.5.3/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/setz.py` & `buildz-0.5.3/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/spt.py` & `buildz-0.5.3/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/deal/strz.py` & `buildz-0.5.3/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/item.py` & `buildz-0.5.3/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/mg.py` & `buildz-0.5.3/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loader/pos.py` & `buildz-0.5.3/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/base.py` & `buildz-0.5.3/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/buffer.py` & `buildz-0.5.3/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.3/buildz/xf/loaderz/deal/lrval.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,40 @@
 from .. import base
 from .. import item
 from .. import exp
 from . import lr
-class ListDeal(lr.LRDeal):
+from . import reval
+class Fcs:
+    def __init__(self):
+        self.maps = {}
+    def set(self, _type, fc):
+        self.maps[_type] = fc
+    def __call__(self, val, _type):
+        if _type not in self.maps:
+            raise Exception("unreginize type:"+_type)
+        return self.maps[_type](val)
+
+pass
+
+
+class LRValDeal(lr.LRDeal):
     """
-        分隔符，有分隔符后将缓存的数据当作字符串
     """
-    def init(self, left, right):
-        super().init(left, right, 'list')
+    def init(self, left, right, fc):
+        super().init(left, right, 'lrval')
+        self.fc = fc
     def build(self, arr):
         rst = []
+        if len(arr)!=2:
+            raise Exception("error in lrval:"+arr)
         for _item in arr:
             if not _item.is_val:
                 raise Exception("error in list:"+_item)
             rst.append(_item.val)
-        return item.Item(rst, type='list', is_val = 1)
+        try:
+            val = self.fc(rst[0], rst[1])
+        except Exception as exp1:
+            print("exp:", exp1)
+            raise Exception(f"error in lrval fc: {self.fc}({rst}): {exp1} ")
+        return item.Item(val, type='val', is_val = 1)
 
-pass
+pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `buildz-0.5.2/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.3/buildz/xf/loaderz/deal/lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,25 +22,34 @@
                 buffer.clean2read(self.lr)
                 break
             if not mg.deal(buffer, _arr):
                 raise Exception("Error lr")
         buffer.clean()
         if len(rm)>0:
             _arr.append(item.Item(rm ,type = '', is_val=False))
+        # dts = []
+        # for k in _arr:
+        #     _k = mg.build(k)
+        #     if item.is_null(_k):
+        #         continue
+        #     dts.append(_k)
+        #dts = [mg.build(k) for k in _arr]
+        dts = mg.build_arr(_arr)
+        obj = self.build_arr(dts)
+        rst.append(obj)
+        return True
+    def to_vals(self, _arr, mg):
         dts = []
         for k in _arr:
             _k = mg.build(k)
             if item.is_null(_k):
                 continue
             dts.append(_k)
-        #dts = [mg.build(k) for k in _arr]
-        obj = self.build(dts)
-        rst.append(obj)
-        return True
-    def build(self, obj):
+        return dts
+    def build_arr(self, obj):
         return item.Item(obj, type = self.type, is_val=True)
     """
         分隔符，有分隔符后将缓存的数据当作字符串
     """
     def prepare(self, mg):
         self.left = mg.like(self.left)
         self.right = mg.like(self.right)
```

### Comparing `buildz-0.5.2/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.3/buildz/xf/loaderz/deal/reval.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .. import item
 from .. import exp
 from . import lr
 import re
 class ValDeal(base.BaseDeal):
     def prepare(self,mg):
         self.pt = mg.like(self.pt)
+        self.type = mg.type
     def types(self):
         return [""]
     """
         正则表达式匹配
     """
     def init(self, pt, fc):
         st = "^"
@@ -18,13 +19,15 @@
             pt = st+pt
         if pt[-1]!=ed:
             pt = pt+ed
         self.pt = pt
         self.fc = fc
     def build(self, obj):
         val = obj.val
+        if type(val) != self.type:
+            return None
         if re.match(self.pt, val) is None:
             return None
         val = self.fc(val)
         return item.Item(val, type = "val", is_val = 1)
 
 pass
```

### Comparing `buildz-0.5.2/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.3/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.3/buildz/xf/loaderz/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/item.py` & `buildz-0.5.3/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/mg.py` & `buildz-0.5.3/buildz/xf/loaderz/mg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,220 @@
 00000000: 0d0a 6672 6f6d 202e 2069 6d70 6f72 7420  ..from . import 
 00000010: 6275 6666 6572 0d0a 6672 6f6d 202e 2069  buffer..from . i
 00000020: 6d70 6f72 7420 6261 7365 0d0a 6672 6f6d  mport base..from
 00000030: 202e 2069 6d70 6f72 7420 706f 730d 0a66   . import pos..f
 00000040: 726f 6d20 2e20 696d 706f 7274 2065 7870  rom . import exp
-00000050: 0d0a 6672 6f6d 202e 2e73 7461 636b 2069  ..from ..stack i
-00000060: 6d70 6f72 7420 5374 6163 6b0d 0a63 6c61  mport Stack..cla
-00000070: 7373 204d 616e 6167 6572 3a0d 0a20 2020  ss Manager:..   
-00000080: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000090: 6c66 2c20 6173 5f62 7974 6573 203d 2046  lf, as_bytes = F
-000000a0: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
-000000b0: 7365 6c66 2e69 6e64 6578 203d 2030 0d0a  self.index = 0..
-000000c0: 2020 2020 2020 2020 7365 6c66 2e61 735f          self.as_
-000000d0: 6279 7465 7320 3d20 6173 5f62 7974 6573  bytes = as_bytes
-000000e0: 0d0a 2020 2020 2020 2020 6966 2061 735f  ..        if as_
-000000f0: 6279 7465 733a 0d0a 2020 2020 2020 2020  bytes:..        
-00000100: 2020 2020 7365 6c66 2e74 7970 6520 3d20      self.type = 
-00000110: 6279 7465 730d 0a20 2020 2020 2020 2065  bytes..        e
-00000120: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000130: 2020 7365 6c66 2e74 7970 6520 3d20 7374    self.type = st
-00000140: 720d 0a20 2020 2020 2020 2073 656c 662e  r..        self.
-00000150: 6465 616c 7320 3d20 7b7d 0d0a 2020 2020  deals = {}..    
-00000160: 2020 2020 7365 6c66 2e62 7569 6c64 7320      self.builds 
-00000170: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00000180: 6c66 2e64 6566 6175 6c74 5f64 6561 6c20  lf.default_deal 
-00000190: 3d20 7365 6c66 2e6c 696b 6528 2222 290d  = self.like("").
-000001a0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
-000001b0: 5f64 6561 6c73 2873 656c 6629 3a0d 0a20  _deals(self):.. 
-000001c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000001d0: 6c66 2e64 6561 6c73 5b73 656c 662e 6465  lf.deals[self.de
-000001e0: 6661 756c 745f 6465 616c 5d0d 0a20 2020  fault_deal]..   
-000001f0: 2064 6566 2067 6574 5f64 6561 6c73 2873   def get_deals(s
-00000200: 656c 662c 2063 293a 0d0a 2020 2020 2020  elf, c):..      
-00000210: 2020 6966 2063 2069 6e20 7365 6c66 2e64    if c in self.d
-00000220: 6561 6c73 3a0d 0a20 2020 2020 2020 2020  eals:..         
-00000230: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
-00000240: 6561 6c73 5b63 5d0d 0a20 2020 2020 2020  eals[c]..       
-00000250: 2072 6574 7572 6e20 5b5d 0d0a 2020 2020   return []..    
-00000260: 6465 6620 6c69 6b65 2873 656c 662c 2073  def like(self, s
-00000270: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-00000280: 656c 662e 7479 7065 203d 3d74 7970 6528  elf.type ==type(
-00000290: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-000002a0: 2072 6574 7572 6e20 730d 0a20 2020 2020   return s..     
-000002b0: 2020 2069 6620 7479 7065 2873 293d 3d73     if type(s)==s
-000002c0: 7472 3a0d 0a20 2020 2020 2020 2020 2020  tr:..           
-000002d0: 2072 6574 7572 6e20 732e 656e 636f 6465   return s.encode
-000002e0: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
-000002f0: 726e 2073 2e64 6563 6f64 6528 290d 0a20  rn s.decode().. 
-00000300: 2020 2064 6566 2061 6464 2873 656c 662c     def add(self,
-00000310: 6f62 6a29 3a0d 0a20 2020 2020 2020 206f  obj):..        o
-00000320: 626a 2e72 6567 6973 7428 7365 6c66 290d  bj.regist(self).
-00000330: 0a20 2020 2020 2020 206c 6273 203d 206f  .        lbs = o
-00000340: 626a 2e6c 6162 656c 7328 290d 0a20 2020  bj.labels()..   
-00000350: 2020 2020 206c 6273 203d 205b 7365 6c66       lbs = [self
-00000360: 2e6c 696b 6528 6b5b 3a31 5d29 2066 6f72  .like(k[:1]) for
-00000370: 206b 2069 6e20 6c62 735d 0d0a 2020 2020   k in lbs]..    
-00000380: 2020 2020 666f 7220 6c62 2069 6e20 6c62      for lb in lb
-00000390: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000003a0: 6966 206c 6220 6e6f 7420 696e 2073 656c  if lb not in sel
-000003b0: 662e 6465 616c 733a 0d0a 2020 2020 2020  f.deals:..      
-000003c0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000003d0: 6561 6c73 5b6c 625d 203d 205b 5d0d 0a20  eals[lb] = [].. 
-000003e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000003f0: 6465 616c 735b 6c62 5d2e 6170 7065 6e64  deals[lb].append
-00000400: 286f 626a 290d 0a20 2020 2020 2020 2074  (obj)..        t
-00000410: 7970 6573 203d 206f 626a 2e74 7970 6573  ypes = obj.types
-00000420: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
-00000430: 5f74 7970 6520 696e 2074 7970 6573 3a0d  _type in types:.
-00000440: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000450: 5f74 7970 6520 6e6f 7420 696e 2073 656c  _type not in sel
-00000460: 662e 6275 696c 6473 3a0d 0a20 2020 2020  f.builds:..     
-00000470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000480: 6275 696c 6473 5b5f 7479 7065 5d20 3d20  builds[_type] = 
-00000490: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000004a0: 7365 6c66 2e62 7569 6c64 735b 5f74 7970  self.builds[_typ
-000004b0: 655d 2e61 7070 656e 6428 6f62 6a29 0d0a  e].append(obj)..
-000004c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000004d0: 656c 660d 0a20 2020 2064 6566 2064 6f28  elf..    def do(
-000004e0: 7365 6c66 2c20 6663 732c 202a 6172 6776  self, fcs, *argv
-000004f0: 2c20 2a2a 6d61 7073 293a 0d0a 2020 2020  , **maps):..    
-00000500: 2020 2020 666f 7220 6663 2069 6e20 6663      for fc in fc
-00000510: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000520: 6966 2066 6328 2a61 7267 762c 202a 2a6d  if fc(*argv, **m
-00000530: 6170 7329 3a0d 0a20 2020 2020 2020 2020  aps):..         
-00000540: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00000550: 7565 0d0a 2020 2020 2020 2020 7265 7475  ue..        retu
-00000560: 726e 2046 616c 7365 0d0a 2020 2020 6465  rn False..    de
-00000570: 6620 7265 6769 7374 2873 656c 6629 3a0d  f regist(self):.
-00000580: 0a20 2020 2020 2020 2069 6420 3d20 7365  .        id = se
-00000590: 6c66 2e69 6e64 6578 0d0a 2020 2020 2020  lf.index..      
-000005a0: 2020 7365 6c66 2e69 6e64 6578 2b3d 310d    self.index+=1.
-000005b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000005c0: 2269 645f 222b 7374 7228 6964 290d 0a20  "id_"+str(id).. 
-000005d0: 2020 2064 6566 2062 7569 6c64 2873 656c     def build(sel
-000005e0: 662c 206f 626a 293a 0d0a 2020 2020 2020  f, obj):..      
-000005f0: 2020 2370 7269 6e74 2866 225b 5445 5354    #print(f"[TEST
-00000600: 5a5d 206f 626a 3a20 7b6f 626a 7d22 290d  Z] obj: {obj}").
-00000610: 0a20 2020 2020 2020 205f 7479 7065 203d  .        _type =
-00000620: 206f 626a 2e74 7970 650d 0a20 2020 2020   obj.type..     
-00000630: 2020 2069 6620 5f74 7970 6520 6e6f 7420     if _type not 
-00000640: 696e 2073 656c 662e 6275 696c 6473 3a0d  in self.builds:.
-00000650: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000660: 6f62 6a2e 6973 5f76 616c 3a0d 0a20 2020  obj.is_val:..   
-00000670: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00000680: 7572 6e20 6f62 6a0d 0a20 2020 2020 2020  urn obj..       
-00000690: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-000006a0: 7469 6f6e 2822 756e 7370 7420 7479 7065  tion("unspt type
-000006b0: 3a22 2b5f 7479 7065 290d 0a20 2020 2020  :"+_type)..     
-000006c0: 2020 2062 7569 6c64 7320 3d20 7365 6c66     builds = self
-000006d0: 2e62 7569 6c64 735b 5f74 7970 655d 0d0a  .builds[_type]..
-000006e0: 2020 2020 2020 2020 666f 7220 6465 616c          for deal
-000006f0: 2069 6e20 6275 696c 6473 3a0d 0a20 2020   in builds:..   
-00000700: 2020 2020 2020 2020 2072 7374 203d 2064           rst = d
-00000710: 6561 6c2e 6275 696c 6428 6f62 6a29 0d0a  eal.build(obj)..
-00000720: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00000730: 7374 2069 7320 6e6f 7420 4e6f 6e65 3a0d  st is not None:.
-00000740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000750: 2072 6574 7572 6e20 7273 740d 0a20 2020   return rst..   
-00000760: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00000770: 7469 6f6e 2822 756e 7370 7420 6465 616c  tion("unspt deal
-00000780: 2074 7970 653a 222b 5f74 7970 6529 0d0a   type:"+_type)..
-00000790: 2020 2020 6465 6620 6465 616c 2873 656c      def deal(sel
-000007a0: 662c 2062 7566 6665 722c 2061 7272 293a  f, buffer, arr):
-000007b0: 0d0a 2020 2020 2020 2020 6320 3d20 6275  ..        c = bu
-000007c0: 6666 6572 2e72 6561 6428 290d 0a20 2020  ffer.read()..   
-000007d0: 2020 2020 2069 6620 6c65 6e28 6329 3d3d       if len(c)==
-000007e0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000007f0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00000800: 2020 2020 2020 6465 616c 7320 3d20 7365        deals = se
-00000810: 6c66 2e67 6574 5f64 6561 6c73 2863 290d  lf.get_deals(c).
-00000820: 0a20 2020 2020 2020 2066 696e 6420 3d20  .        find = 
-00000830: 4661 6c73 650d 0a20 2020 2020 2020 2066  False..        f
-00000840: 6f72 2064 6561 6c20 696e 2064 6561 6c73  or deal in deals
-00000850: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000860: 6620 6465 616c 2e64 6561 6c28 6275 6666  f deal.deal(buff
-00000870: 6572 2c20 6172 722c 2073 656c 6629 3a0d  er, arr, self):.
-00000880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000890: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
-000008a0: 2020 2020 2020 6465 616c 7320 3d20 7365        deals = se
-000008b0: 6c66 2e64 6566 6175 6c74 5f64 6561 6c73  lf.default_deals
-000008c0: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
-000008d0: 6465 616c 2069 6e20 6465 616c 733a 0d0a  deal in deals:..
-000008e0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-000008f0: 6561 6c2e 6465 616c 2862 7566 6665 722c  eal.deal(buffer,
-00000900: 2061 7272 2c20 7365 6c66 293a 0d0a 2020   arr, self):..  
-00000910: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000920: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00000930: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00000940: 0a20 2020 2064 6566 206c 6f61 6428 7365  .    def load(se
-00000950: 6c66 2c20 6275 6666 6572 293a 0d0a 2020  lf, buffer):..  
-00000960: 2020 2020 2020 6172 7220 3d20 5b5d 0d0a        arr = []..
-00000970: 2020 2020 2020 2020 7768 696c 6520 7365          while se
-00000980: 6c66 2e64 6561 6c28 6275 6666 6572 2c20  lf.deal(buffer, 
-00000990: 6172 7229 3a0d 0a20 2020 2020 2020 2020  arr):..         
-000009a0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-000009b0: 2061 7272 203d 205b 6b2e 7661 6c20 666f   arr = [k.val fo
-000009c0: 7220 6b20 696e 2061 7272 5d0d 0a20 2020  r k in arr]..   
-000009d0: 2020 2020 2072 7374 203d 205b 5d0d 0a20       rst = [].. 
-000009e0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-000009f0: 6172 723a 0d0a 2020 2020 2020 2020 2020  arr:..          
-00000a00: 2020 6966 2074 7970 6528 6b29 203d 3d20    if type(k) == 
-00000a10: 7365 6c66 2e74 7970 653a 0d0a 2020 2020  self.type:..    
-00000a20: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00000a30: 656e 286b 2e73 7472 6970 2829 293d 3d30  en(k.strip())==0
-00000a40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000a50: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00000a60: 0a20 2020 2020 2020 2020 2020 2072 7374  .            rst
-00000a70: 2e61 7070 656e 6428 6b29 0d0a 2020 2020  .append(k)..    
-00000a80: 2020 2020 6172 7220 3d20 7273 740d 0a20      arr = rst.. 
-00000a90: 2020 2020 2020 2069 6620 6c65 6e28 6172         if len(ar
-00000aa0: 7229 3d3d 313a 0d0a 2020 2020 2020 2020  r)==1:..        
-00000ab0: 2020 2020 6172 7220 3d20 6172 725b 305d      arr = arr[0]
-00000ac0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000ad0: 2061 7272 0d0a 2020 2020 6465 6620 6c6f   arr..    def lo
-00000ae0: 6164 7328 7365 6c66 2c20 7265 6164 6572  ads(self, reader
-00000af0: 293a 0d0a 2020 2020 2020 2020 6966 2074  ):..        if t
-00000b00: 7970 6528 7265 6164 6572 2920 3d3d 2073  ype(reader) == s
-00000b10: 656c 662e 7479 7065 3a0d 0a20 2020 2020  elf.type:..     
-00000b20: 2020 2020 2020 2023 7072 696e 7428 6622         #print(f"
-00000b30: 7472 7920 7374 722c 207b 6c65 6e28 7265  try str, {len(re
-00000b40: 6164 6572 297d 2229 0d0a 2020 2020 2020  ader)}")..      
-00000b50: 2020 2020 2020 6275 6666 203d 2062 7566        buff = buf
-00000b60: 6665 722e 5374 7242 7566 6665 7228 7265  fer.StrBuffer(re
-00000b70: 6164 6572 290d 0a20 2020 2020 2020 2065  ader)..        e
-00000b80: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000b90: 2020 6275 6666 203d 2062 7566 6665 722e    buff = buffer.
-00000ba0: 4275 6666 6572 2872 6561 6465 7229 0d0a  Buffer(reader)..
-00000bb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000bc0: 656c 662e 6c6f 6164 2862 7566 6629 0d0a  elf.load(buff)..
-00000bd0: 0d0a 7061 7373 0d0a                      ..pass..
+00000050: 0d0a 6672 6f6d 202e 2069 6d70 6f72 7420  ..from . import 
+00000060: 6974 656d 0d0a 6672 6f6d 202e 2e73 7461  item..from ..sta
+00000070: 636b 2069 6d70 6f72 7420 5374 6163 6b0d  ck import Stack.
+00000080: 0a63 6c61 7373 204d 616e 6167 6572 3a0d  .class Manager:.
+00000090: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000000a0: 5f28 7365 6c66 2c20 6173 5f62 7974 6573  _(self, as_bytes
+000000b0: 203d 2046 616c 7365 293a 0d0a 2020 2020   = False):..    
+000000c0: 2020 2020 7365 6c66 2e69 6e64 6578 203d      self.index =
+000000d0: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
+000000e0: 2e61 735f 6279 7465 7320 3d20 6173 5f62  .as_bytes = as_b
+000000f0: 7974 6573 0d0a 2020 2020 2020 2020 6966  ytes..        if
+00000100: 2061 735f 6279 7465 733a 0d0a 2020 2020   as_bytes:..    
+00000110: 2020 2020 2020 2020 7365 6c66 2e74 7970          self.typ
+00000120: 6520 3d20 6279 7465 730d 0a20 2020 2020  e = bytes..     
+00000130: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000140: 2020 2020 2020 7365 6c66 2e74 7970 6520        self.type 
+00000150: 3d20 7374 720d 0a20 2020 2020 2020 2073  = str..        s
+00000160: 656c 662e 6465 616c 7320 3d20 7b7d 0d0a  elf.deals = {}..
+00000170: 2020 2020 2020 2020 7365 6c66 2e62 7569          self.bui
+00000180: 6c64 7320 3d20 7b7d 0d0a 2020 2020 2020  lds = {}..      
+00000190: 2020 7365 6c66 2e64 6566 6175 6c74 5f64    self.default_d
+000001a0: 6561 6c20 3d20 7365 6c66 2e6c 696b 6528  eal = self.like(
+000001b0: 2222 290d 0a20 2020 2064 6566 2064 6566  "")..    def def
+000001c0: 6175 6c74 5f64 6561 6c73 2873 656c 6629  ault_deals(self)
+000001d0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000001e0: 6e20 7365 6c66 2e64 6561 6c73 5b73 656c  n self.deals[sel
+000001f0: 662e 6465 6661 756c 745f 6465 616c 5d0d  f.default_deal].
+00000200: 0a20 2020 2064 6566 2067 6574 5f64 6561  .    def get_dea
+00000210: 6c73 2873 656c 662c 2063 293a 0d0a 2020  ls(self, c):..  
+00000220: 2020 2020 2020 6966 2063 2069 6e20 7365        if c in se
+00000230: 6c66 2e64 6561 6c73 3a0d 0a20 2020 2020  lf.deals:..     
+00000240: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000250: 6c66 2e64 6561 6c73 5b63 5d0d 0a20 2020  lf.deals[c]..   
+00000260: 2020 2020 2072 6574 7572 6e20 5b5d 0d0a       return []..
+00000270: 2020 2020 6465 6620 6c69 6b65 2873 656c      def like(sel
+00000280: 662c 2073 293a 0d0a 2020 2020 2020 2020  f, s):..        
+00000290: 6966 2073 656c 662e 7479 7065 203d 3d74  if self.type ==t
+000002a0: 7970 6528 7329 3a0d 0a20 2020 2020 2020  ype(s):..       
+000002b0: 2020 2020 2072 6574 7572 6e20 730d 0a20       return s.. 
+000002c0: 2020 2020 2020 2069 6620 7479 7065 2873         if type(s
+000002d0: 293d 3d73 7472 3a0d 0a20 2020 2020 2020  )==str:..       
+000002e0: 2020 2020 2072 6574 7572 6e20 732e 656e       return s.en
+000002f0: 636f 6465 2829 0d0a 2020 2020 2020 2020  code()..        
+00000300: 7265 7475 726e 2073 2e64 6563 6f64 6528  return s.decode(
+00000310: 290d 0a20 2020 2064 6566 2061 6464 2873  )..    def add(s
+00000320: 656c 662c 6f62 6a29 3a0d 0a20 2020 2020  elf,obj):..     
+00000330: 2020 206f 626a 2e72 6567 6973 7428 7365     obj.regist(se
+00000340: 6c66 290d 0a20 2020 2020 2020 206c 6273  lf)..        lbs
+00000350: 203d 206f 626a 2e6c 6162 656c 7328 290d   = obj.labels().
+00000360: 0a20 2020 2020 2020 206c 6273 203d 205b  .        lbs = [
+00000370: 7365 6c66 2e6c 696b 6528 6b5b 3a31 5d29  self.like(k[:1])
+00000380: 2066 6f72 206b 2069 6e20 6c62 735d 0d0a   for k in lbs]..
+00000390: 2020 2020 2020 2020 666f 7220 6c62 2069          for lb i
+000003a0: 6e20 6c62 733a 0d0a 2020 2020 2020 2020  n lbs:..        
+000003b0: 2020 2020 6966 206c 6220 6e6f 7420 696e      if lb not in
+000003c0: 2073 656c 662e 6465 616c 733a 0d0a 2020   self.deals:..  
+000003d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000003e0: 6c66 2e64 6561 6c73 5b6c 625d 203d 205b  lf.deals[lb] = [
+000003f0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+00000400: 656c 662e 6465 616c 735b 6c62 5d2e 6170  elf.deals[lb].ap
+00000410: 7065 6e64 286f 626a 290d 0a20 2020 2020  pend(obj)..     
+00000420: 2020 2074 7970 6573 203d 206f 626a 2e74     types = obj.t
+00000430: 7970 6573 2829 0d0a 2020 2020 2020 2020  ypes()..        
+00000440: 666f 7220 5f74 7970 6520 696e 2074 7970  for _type in typ
+00000450: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00000460: 2069 6620 5f74 7970 6520 6e6f 7420 696e   if _type not in
+00000470: 2073 656c 662e 6275 696c 6473 3a0d 0a20   self.builds:.. 
+00000480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000490: 656c 662e 6275 696c 6473 5b5f 7479 7065  elf.builds[_type
+000004a0: 5d20 3d20 5b5d 0d0a 2020 2020 2020 2020  ] = []..        
+000004b0: 2020 2020 7365 6c66 2e62 7569 6c64 735b      self.builds[
+000004c0: 5f74 7970 655d 2e61 7070 656e 6428 6f62  _type].append(ob
+000004d0: 6a29 0d0a 2020 2020 2020 2020 7265 7475  j)..        retu
+000004e0: 726e 2073 656c 660d 0a20 2020 2064 6566  rn self..    def
+000004f0: 2064 6f28 7365 6c66 2c20 6663 732c 202a   do(self, fcs, *
+00000500: 6172 6776 2c20 2a2a 6d61 7073 293a 0d0a  argv, **maps):..
+00000510: 2020 2020 2020 2020 666f 7220 6663 2069          for fc i
+00000520: 6e20 6663 733a 0d0a 2020 2020 2020 2020  n fcs:..        
+00000530: 2020 2020 6966 2066 6328 2a61 7267 762c      if fc(*argv,
+00000540: 202a 2a6d 6170 7329 3a0d 0a20 2020 2020   **maps):..     
+00000550: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000560: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
+00000570: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+00000580: 2020 6465 6620 7265 6769 7374 2873 656c    def regist(sel
+00000590: 6629 3a0d 0a20 2020 2020 2020 2069 6420  f):..        id 
+000005a0: 3d20 7365 6c66 2e69 6e64 6578 0d0a 2020  = self.index..  
+000005b0: 2020 2020 2020 7365 6c66 2e69 6e64 6578        self.index
+000005c0: 2b3d 310d 0a20 2020 2020 2020 2072 6574  +=1..        ret
+000005d0: 7572 6e20 2269 645f 222b 7374 7228 6964  urn "id_"+str(id
+000005e0: 290d 0a20 2020 2064 6566 2062 7569 6c64  )..    def build
+000005f0: 2873 656c 662c 206f 626a 293a 0d0a 2020  (self, obj):..  
+00000600: 2020 2020 2020 2370 7269 6e74 2866 225b        #print(f"[
+00000610: 5445 5354 5a5d 206f 626a 3a20 7b6f 626a  TESTZ] obj: {obj
+00000620: 7d22 290d 0a20 2020 2020 2020 205f 7479  }")..        _ty
+00000630: 7065 203d 206f 626a 2e74 7970 650d 0a20  pe = obj.type.. 
+00000640: 2020 2020 2020 2069 6620 5f74 7970 6520         if _type 
+00000650: 6e6f 7420 696e 2073 656c 662e 6275 696c  not in self.buil
+00000660: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00000670: 2069 6620 6f62 6a2e 6973 5f76 616c 3a0d   if obj.is_val:.
+00000680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000690: 2072 6574 7572 6e20 6f62 6a0d 0a20 2020   return obj..   
+000006a0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000006b0: 7863 6570 7469 6f6e 2822 756e 7370 7420  xception("unspt 
+000006c0: 7479 7065 3a22 2b5f 7479 7065 290d 0a20  type:"+_type).. 
+000006d0: 2020 2020 2020 2062 7569 6c64 7320 3d20         builds = 
+000006e0: 7365 6c66 2e62 7569 6c64 735b 5f74 7970  self.builds[_typ
+000006f0: 655d 0d0a 2020 2020 2020 2020 666f 7220  e]..        for 
+00000700: 6465 616c 2069 6e20 6275 696c 6473 3a0d  deal in builds:.
+00000710: 0a20 2020 2020 2020 2020 2020 2072 7374  .            rst
+00000720: 203d 2064 6561 6c2e 6275 696c 6428 6f62   = deal.build(ob
+00000730: 6a29 0d0a 2020 2020 2020 2020 2020 2020  j)..            
+00000740: 6966 2072 7374 2069 7320 6e6f 7420 4e6f  if rst is not No
+00000750: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00000760: 2020 2020 2072 6574 7572 6e20 7273 740d       return rst.
+00000770: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
+00000780: 7863 6570 7469 6f6e 2822 756e 7370 7420  xception("unspt 
+00000790: 6465 616c 2074 7970 653a 222b 5f74 7970  deal type:"+_typ
+000007a0: 6529 0d0a 2020 2020 6465 6620 6465 616c  e)..    def deal
+000007b0: 2873 656c 662c 2062 7566 6665 722c 2061  (self, buffer, a
+000007c0: 7272 293a 0d0a 2020 2020 2020 2020 6320  rr):..        c 
+000007d0: 3d20 6275 6666 6572 2e72 6561 6428 290d  = buffer.read().
+000007e0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000007f0: 6329 3d3d 3020 616e 6420 6275 6666 6572  c)==0 and buffer
+00000800: 2e73 697a 6528 293d 3d30 3a0d 0a20 2020  .size()==0:..   
+00000810: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000820: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+00000830: 6561 6c73 203d 2073 656c 662e 6765 745f  eals = self.get_
+00000840: 6465 616c 7328 6329 0d0a 2020 2020 2020  deals(c)..      
+00000850: 2020 6669 6e64 203d 2046 616c 7365 0d0a    find = False..
+00000860: 2020 2020 2020 2020 666f 7220 6465 616c          for deal
+00000870: 2069 6e20 6465 616c 733a 0d0a 2020 2020   in deals:..    
+00000880: 2020 2020 2020 2020 6966 2064 6561 6c2e          if deal.
+00000890: 6465 616c 2862 7566 6665 722c 2061 7272  deal(buffer, arr
+000008a0: 2c20 7365 6c66 293a 0d0a 2020 2020 2020  , self):..      
+000008b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000008c0: 2054 7275 650d 0a20 2020 2020 2020 2064   True..        d
+000008d0: 6561 6c73 203d 2073 656c 662e 6465 6661  eals = self.defa
+000008e0: 756c 745f 6465 616c 7328 290d 0a20 2020  ult_deals()..   
+000008f0: 2020 2020 2066 6f72 2064 6561 6c20 696e       for deal in
+00000900: 2064 6561 6c73 3a0d 0a20 2020 2020 2020   deals:..       
+00000910: 2020 2020 2069 6620 6465 616c 2e64 6561       if deal.dea
+00000920: 6c28 6275 6666 6572 2c20 6172 722c 2073  l(buffer, arr, s
+00000930: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+00000940: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00000950: 7565 0d0a 2020 2020 2020 2020 7265 7475  ue..        retu
+00000960: 726e 2046 616c 7365 0d0a 2020 2020 6465  rn False..    de
+00000970: 6620 6275 696c 645f 6172 7228 7365 6c66  f build_arr(self
+00000980: 2c20 5f61 7272 293a 0d0a 2020 2020 2020  , _arr):..      
+00000990: 2020 6474 7320 3d20 5b5d 0d0a 2020 2020    dts = []..    
+000009a0: 2020 2020 666f 7220 6b20 696e 205f 6172      for k in _ar
+000009b0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+000009c0: 5f6b 203d 2073 656c 662e 6275 696c 6428  _k = self.build(
+000009d0: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
+000009e0: 6966 2069 7465 6d2e 6973 5f6e 756c 6c28  if item.is_null(
+000009f0: 5f6b 293a 0d0a 2020 2020 2020 2020 2020  _k):..          
+00000a00: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00000a10: 2020 2020 2020 2020 2020 2020 6474 732e              dts.
+00000a20: 6170 7065 6e64 285f 6b29 0d0a 2020 2020  append(_k)..    
+00000a30: 2020 2020 7265 7475 726e 2064 7473 0d0a      return dts..
+00000a40: 2020 2020 6465 6620 6c6f 6164 2873 656c      def load(sel
+00000a50: 662c 2062 7566 6665 7229 3a0d 0a20 2020  f, buffer):..   
+00000a60: 2020 2020 2061 7272 203d 205b 5d0d 0a20       arr = [].. 
+00000a70: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
+00000a80: 662e 6465 616c 2862 7566 6665 722c 2061  f.deal(buffer, a
+00000a90: 7272 293a 0d0a 2020 2020 2020 2020 2020  rr):..          
+00000aa0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+00000ab0: 2361 7272 203d 205b 6b2e 7661 6c20 666f  #arr = [k.val fo
+00000ac0: 7220 6b20 696e 2061 7272 5d0d 0a20 2020  r k in arr]..   
+00000ad0: 2020 2020 2023 7273 7420 3d20 5b5d 0d0a       #rst = []..
+00000ae0: 2020 2020 2020 2020 2320 666f 7220 6b20          # for k 
+00000af0: 696e 2061 7272 3a0d 0a20 2020 2020 2020  in arr:..       
+00000b00: 2023 2020 2020 2069 6620 7479 7065 286b   #     if type(k
+00000b10: 2920 3d3d 2073 656c 662e 7479 7065 3a0d  ) == self.type:.
+00000b20: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00000b30: 2020 2069 6620 6c65 6e28 6b2e 7374 7269     if len(k.stri
+00000b40: 7028 2929 3d3d 303a 0d0a 2020 2020 2020  p())==0:..      
+00000b50: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00000b60: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00000b70: 2020 2320 2020 2020 7273 742e 6170 7065    #     rst.appe
+00000b80: 6e64 286b 290d 0a20 2020 2020 2020 2061  nd(k)..        a
+00000b90: 7272 203d 2073 656c 662e 6275 696c 645f  rr = self.build_
+00000ba0: 6172 7228 6172 7229 0d0a 2020 2020 2020  arr(arr)..      
+00000bb0: 2020 6f62 6a20 3d20 6974 656d 2e49 7465    obj = item.Ite
+00000bc0: 6d28 6172 722c 2074 7970 6520 3d20 2222  m(arr, type = ""
+00000bd0: 2c20 6973 5f76 616c 203d 2030 290d 0a20  , is_val = 0).. 
+00000be0: 2020 2020 2020 206f 626a 203d 2073 656c         obj = sel
+00000bf0: 662e 6275 696c 6428 6f62 6a29 0d0a 2020  f.build(obj)..  
+00000c00: 2020 2020 2020 2361 7272 203d 2072 7374        #arr = rst
+00000c10: 0d0a 2020 2020 2020 2020 2369 6620 6c65  ..        #if le
+00000c20: 6e28 6172 7229 3d3d 313a 0d0a 2020 2020  n(arr)==1:..    
+00000c30: 2020 2020 2320 2020 2061 7272 203d 2061      #    arr = a
+00000c40: 7272 5b30 5d0d 0a20 2020 2020 2020 2076  rr[0]..        v
+00000c50: 616c 203d 206f 626a 2e76 616c 0d0a 2020  al = obj.val..  
+00000c60: 2020 2020 2020 6966 2074 7970 6528 7661        if type(va
+00000c70: 6c29 3d3d 6c69 7374 2061 6e64 206c 656e  l)==list and len
+00000c80: 2876 616c 293d 3d31 3a0d 0a20 2020 2020  (val)==1:..     
+00000c90: 2020 2020 2020 2076 616c 203d 2076 616c         val = val
+00000ca0: 5b30 5d0d 0a20 2020 2020 2020 2072 6574  [0]..        ret
+00000cb0: 7572 6e20 7661 6c0d 0a20 2020 2064 6566  urn val..    def
+00000cc0: 206c 6f61 6473 2873 656c 662c 2072 6561   loads(self, rea
+00000cd0: 6465 7229 3a0d 0a20 2020 2020 2020 2069  der):..        i
+00000ce0: 6620 7479 7065 2872 6561 6465 7229 203d  f type(reader) =
+00000cf0: 3d20 7365 6c66 2e74 7970 653a 0d0a 2020  = self.type:..  
+00000d00: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
+00000d10: 2866 2274 7279 2073 7472 2c20 7b6c 656e  (f"try str, {len
+00000d20: 2872 6561 6465 7229 7d22 290d 0a20 2020  (reader)}")..   
+00000d30: 2020 2020 2020 2020 2062 7566 6620 3d20           buff = 
+00000d40: 6275 6666 6572 2e53 7472 4275 6666 6572  buffer.StrBuffer
+00000d50: 2872 6561 6465 7229 0d0a 2020 2020 2020  (reader)..      
+00000d60: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000d70: 2020 2020 2062 7566 6620 3d20 6275 6666       buff = buff
+00000d80: 6572 2e42 7566 6665 7228 7265 6164 6572  er.Buffer(reader
+00000d90: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00000da0: 6e20 7365 6c66 2e6c 6f61 6428 6275 6666  n self.load(buff
+00000db0: 290d 0a0d 0a70 6173 730d 0a              )....pass..
```

### Comparing `buildz-0.5.2/buildz/xf/loaderz/pos.py` & `buildz-0.5.3/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/loaderz/test.py` & `buildz-0.5.3/buildz/xf/loaderz/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,26 +51,26 @@
 pass
 print("test D")
 json.dumps(_arr)
 print("test E")
 json.dumps(_map)
 print("test F")
 js = json.dumps(rst)
-js = "\n\n"+js+"\n"
+#js = "\n\n"+js+"\n"
 #js = xf.dumps(rst, json_format=1)
 # js = r"""
 # [
 #     1,2,3,{"4":5,"6":7,"8":9,"10":11,"4":6}
 # ]
 # """
 print("start")
 jv = cost("json.loads", json.loads,js)
 xv = cost("rz.loads",rz.loads,js)
 print(f"judge: {jv==xv}")
-_xv = cost("rd.loads",rd.loads, js)
+#_xv = cost("rd.loads",rd.loads, js)
 #with open("test.json", 'w') as f:
 #    f.write(js)
 if n>3 or m>3 or l > 3:
     exit()
 print(json.dumps(jv))
 print(json.dumps(xv))
```

### Comparing `buildz-0.5.2/buildz/xf/mapz.py` & `buildz-0.5.3/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/read.py` & `buildz-0.5.3/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/readz.py` & `buildz-0.5.3/buildz/xf/readz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/stack.py` & `buildz-0.5.3/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/write.py` & `buildz-0.5.3/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/base.py` & `buildz-0.5.3/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/conf.py` & `buildz-0.5.3/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/deal/listz.py` & `buildz-0.5.3/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.3/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/deal/strz.py` & `buildz-0.5.3/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/itemz.py` & `buildz-0.5.3/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/writer/mg.py` & `buildz-0.5.3/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz/xf/xargs.py` & `buildz-0.5.3/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.2/buildz.egg-info/PKG-INFO` & `buildz-0.5.3/buildz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.2
+Version: 0.5.3
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.2/buildz.egg-info/SOURCES.txt` & `buildz-0.5.3/buildz.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 buildz/xf/loaderz/base.py
 buildz/xf/loaderz/buffer.py
 buildz/xf/loaderz/exp.py
 buildz/xf/loaderz/item.py
 buildz/xf/loaderz/mg.py
 buildz/xf/loaderz/pos.py
 buildz/xf/loaderz/test.py
+buildz/xf/loaderz/test1.py
 buildz/xf/loaderz/deal/listz.py
 buildz/xf/loaderz/deal/lr.py
 buildz/xf/loaderz/deal/lrval.py
 buildz/xf/loaderz/deal/mapz.py
 buildz/xf/loaderz/deal/nextz.py
 buildz/xf/loaderz/deal/reval.py
 buildz/xf/loaderz/deal/setz.py
```

### Comparing `buildz-0.5.2/setup.py` & `buildz-0.5.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.2',
+    version = '0.5.3',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

