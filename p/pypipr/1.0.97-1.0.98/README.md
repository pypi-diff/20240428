# Comparing `tmp/pypipr-1.0.97.tar.gz` & `tmp/pypipr-1.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.97.tar", max compression
+gzip compressed data, was "pypipr-1.0.98.tar", max compression
```

## Comparing `pypipr-1.0.97.tar` & `pypipr-1.0.98.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     3487 2024-04-28 13:09:18.716396 pypipr-1.0.97/pypipr/__init__.py
--rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/ComparePerformance.py
--rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/LINUX.py
--rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.97/pypipr/ibuiltins/RunParallel.py
--rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/WINDOWS.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/__init__.py
--rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/avg.py
--rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/basename.py
--rw-r--r--   0        0        0      623 2024-04-28 13:05:27.756396 pypipr-1.0.97/pypipr/ibuiltins/chr_to_int.py
--rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.97/pypipr/ibuiltins/chunk_array.py
--rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/create_folder.py
--rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/datetime_from_string.py
--rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/datetime_now.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/dict_first.py
--rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/dirname.py
--rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.97/pypipr/ibuiltins/exit_if_empty.py
--rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/filter_empty.py
--rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.97/pypipr/ibuiltins/get_by_index.py
--rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.97/pypipr/ibuiltins/get_class_method.py
--rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/get_filemtime.py
--rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/get_filesize.py
--rw-r--r--   0        0        0      610 2024-04-28 13:08:11.692396 pypipr-1.0.97/pypipr/ibuiltins/int_to_chr.py
--rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.97/pypipr/ibuiltins/is_empty.py
--rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/is_iterable.py
--rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/is_valid_url.py
--rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.97/pypipr/ibuiltins/ivars.py
--rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/password_generator.py
--rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.97/pypipr/ibuiltins/random_bool.py
--rw-r--r--   0        0        0      114 2024-04-25 14:37:53.772148 pypipr-1.0.97/pypipr/ibuiltins/restart.py
--rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/ibuiltins/set_timeout.py
--rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/ibuiltins/sets_ordered.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/ibuiltins/str_cmp.py
--rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/ibuiltins/to_str.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iconsole/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iconsole/choices.py
--rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iconsole/console_run.py
--rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.97/pypipr/iconsole/input_char.py
--rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iconsole/log.py
--rw-r--r--   0        0        0      541 2024-04-27 07:44:48.048476 pypipr-1.0.97/pypipr/iconsole/print_colorize.py
--rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.97/pypipr/iconsole/print_dir.py
--rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.97/pypipr/iconsole/print_log.py
--rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.97/pypipr/iconsole/print_to_last_line.py
--rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iconsole/text_colorize.py
--rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/idjango/APIMixinView.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/idjango/__init__.py
--rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iengineering/PintUreg.py
--rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iengineering/PintUregQuantity.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iengineering/__init__.py
--rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.97/pypipr/iengineering/batch_calculate.py
--rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iengineering/batchmaker.py
--rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.97/pypipr/iengineering/calculate.py
--rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.97/pypipr/iflow/auto_reload.py
--rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/iflow/github_pull.py
--rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/iflow/github_push.py
--rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/iflow/github_user.py
--rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.97/pypipr/iflow/pip_freeze_without_version.py
--rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/iflow/poetry_publish.py
--rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/iflow/poetry_update_version.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/__init__.py
--rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.97/pypipr/ifunctions/iargv.py
--rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/idumps.py
--rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/idumps_html.py
--rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.97/pypipr/ifunctions/ienv.py
--rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/iexec.py
--rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/ijoin.py
--rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.97/pypipr/ifunctions/iloads.py
--rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.97/pypipr/ifunctions/iloads_html.py
--rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/iopen.py
--rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.97/pypipr/ifunctions/iprint.py
--rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/irange.py
--rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.97/pypipr/ifunctions/ireplace.py
--rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.97/pypipr/ifunctions/iscandir.py
--rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.97/pypipr/ifunctions/isplit.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.97/pypipr/pypipr.py.bak
--rw-r--r--   0        0        0     1800 2024-04-24 08:29:46.253049 pypipr-1.0.97/pypipr/terminal.py
--rw-r--r--   0        0        0      544 2024-04-28 13:09:31.144396 pypipr-1.0.97/pyproject.toml
--rw-r--r--   0        0        0    50406 2024-04-28 13:09:23.300396 pypipr-1.0.97/readme.md
--rw-r--r--   0        0        0    51092 1970-01-01 00:00:00.000000 pypipr-1.0.97/PKG-INFO
+-rw-r--r--   0        0        0     3487 2024-04-28 13:23:42.904396 pypipr-1.0.98/pypipr/__init__.py
+-rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/ComparePerformance.py
+-rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/LINUX.py
+-rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.98/pypipr/ibuiltins/RunParallel.py
+-rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/WINDOWS.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/avg.py
+-rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/basename.py
+-rw-r--r--   0        0        0      714 2024-04-28 13:23:17.812396 pypipr-1.0.98/pypipr/ibuiltins/chr_to_int.py
+-rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.98/pypipr/ibuiltins/chunk_array.py
+-rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/create_folder.py
+-rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/datetime_from_string.py
+-rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/datetime_now.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/dict_first.py
+-rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/dirname.py
+-rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.98/pypipr/ibuiltins/exit_if_empty.py
+-rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/filter_empty.py
+-rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.98/pypipr/ibuiltins/get_by_index.py
+-rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.98/pypipr/ibuiltins/get_class_method.py
+-rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/get_filemtime.py
+-rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/get_filesize.py
+-rw-r--r--   0        0        0      610 2024-04-28 13:08:11.692396 pypipr-1.0.98/pypipr/ibuiltins/int_to_chr.py
+-rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.98/pypipr/ibuiltins/is_empty.py
+-rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/is_iterable.py
+-rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/is_valid_url.py
+-rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.98/pypipr/ibuiltins/ivars.py
+-rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/password_generator.py
+-rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/random_bool.py
+-rw-r--r--   0        0        0      114 2024-04-25 14:37:53.772148 pypipr-1.0.98/pypipr/ibuiltins/restart.py
+-rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/set_timeout.py
+-rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/sets_ordered.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/str_cmp.py
+-rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/to_str.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/__init__.py
+-rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/choices.py
+-rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/console_run.py
+-rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.98/pypipr/iconsole/input_char.py
+-rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/log.py
+-rw-r--r--   0        0        0      541 2024-04-27 07:44:48.048476 pypipr-1.0.98/pypipr/iconsole/print_colorize.py
+-rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.98/pypipr/iconsole/print_dir.py
+-rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.98/pypipr/iconsole/print_log.py
+-rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.98/pypipr/iconsole/print_to_last_line.py
+-rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/text_colorize.py
+-rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/idjango/APIMixinView.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/idjango/__init__.py
+-rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/PintUreg.py
+-rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/PintUregQuantity.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.98/pypipr/iengineering/batch_calculate.py
+-rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/batchmaker.py
+-rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/calculate.py
+-rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.98/pypipr/iflow/auto_reload.py
+-rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/github_pull.py
+-rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/github_push.py
+-rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/github_user.py
+-rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.98/pypipr/iflow/pip_freeze_without_version.py
+-rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/poetry_publish.py
+-rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/poetry_update_version.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.98/pypipr/ifunctions/iargv.py
+-rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/idumps.py
+-rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/idumps_html.py
+-rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.98/pypipr/ifunctions/ienv.py
+-rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/iexec.py
+-rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/ijoin.py
+-rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.98/pypipr/ifunctions/iloads.py
+-rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.98/pypipr/ifunctions/iloads_html.py
+-rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/iopen.py
+-rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.98/pypipr/ifunctions/iprint.py
+-rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/irange.py
+-rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/ireplace.py
+-rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.98/pypipr/ifunctions/iscandir.py
+-rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.98/pypipr/ifunctions/isplit.py
+-rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.98/pypipr/pypipr.py.bak
+-rw-r--r--   0        0        0     1800 2024-04-24 08:29:46.253049 pypipr-1.0.98/pypipr/terminal.py
+-rw-r--r--   0        0        0      544 2024-04-28 13:23:53.456396 pypipr-1.0.98/pyproject.toml
+-rw-r--r--   0        0        0    50405 2024-04-28 13:23:47.860396 pypipr-1.0.98/readme.md
+-rw-r--r--   0        0        0    51091 1970-01-01 00:00:00.000000 pypipr-1.0.98/PKG-INFO
```

### Comparing `pypipr-1.0.97/pypipr/__init__.py` & `pypipr-1.0.98/pypipr/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/ComparePerformance.py` & `pypipr-1.0.98/pypipr/ibuiltins/ComparePerformance.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/RunParallel.py` & `pypipr-1.0.98/pypipr/ibuiltins/RunParallel.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/chr_to_int.py` & `pypipr-1.0.98/pypipr/ibuiltins/chr_to_int.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,21 @@
     print(chr_to_int('abc', numbers="abc"))  # Output: 10
     ```
     """
     result = 0
     digit = len(numbers)
     for char in s:
         result = result * digit + numbers.index(char) + 1
-    return result - start
+    return result + start - 1
+
 
 if __name__ == "__main__":
-    print(chr_to_int('z'))  # Output: 25
-    print(chr_to_int('aa'))  # Output: 26
-    print(chr_to_int('abc', numbers="abc"))  # Output: 5
+    print(chr_to_int("z"))  # Output: 25
+    print(chr_to_int("aa"))  # Output: 26
+    print(chr_to_int("abc", numbers="abc"))  # Output: 5
+    for i in "abcdefghijklmnopqrstuvwxyz":
+        print(chr_to_int(i, start=9))
+
+
+
+
+
```

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/filter_empty.py` & `pypipr-1.0.98/pypipr/ibuiltins/filter_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/get_class_method.py` & `pypipr-1.0.98/pypipr/ibuiltins/get_class_method.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/int_to_chr.py` & `pypipr-1.0.98/pypipr/ibuiltins/int_to_chr.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/is_empty.py` & `pypipr-1.0.98/pypipr/ibuiltins/is_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/is_iterable.py` & `pypipr-1.0.98/pypipr/ibuiltins/is_iterable.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/is_valid_url.py` & `pypipr-1.0.98/pypipr/ibuiltins/is_valid_url.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/ivars.py` & `pypipr-1.0.98/pypipr/ibuiltins/ivars.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/set_timeout.py` & `pypipr-1.0.98/pypipr/ibuiltins/set_timeout.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ibuiltins/to_str.py` & `pypipr-1.0.98/pypipr/ibuiltins/to_str.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/choices.py` & `pypipr-1.0.98/pypipr/iconsole/choices.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/console_run.py` & `pypipr-1.0.98/pypipr/iconsole/console_run.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/input_char.py` & `pypipr-1.0.98/pypipr/iconsole/input_char.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/log.py` & `pypipr-1.0.98/pypipr/iconsole/log.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/print_colorize.py` & `pypipr-1.0.98/pypipr/iconsole/print_colorize.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/print_dir.py` & `pypipr-1.0.98/pypipr/iconsole/print_dir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iconsole/print_to_last_line.py` & `pypipr-1.0.98/pypipr/iconsole/print_to_last_line.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/idjango/APIMixinView.py` & `pypipr-1.0.98/pypipr/idjango/APIMixinView.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iengineering/batch_calculate.py` & `pypipr-1.0.98/pypipr/iengineering/batch_calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iengineering/batchmaker.py` & `pypipr-1.0.98/pypipr/iengineering/batchmaker.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iengineering/calculate.py` & `pypipr-1.0.98/pypipr/iengineering/calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iflow/auto_reload.py` & `pypipr-1.0.98/pypipr/iflow/auto_reload.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iflow/github_push.py` & `pypipr-1.0.98/pypipr/iflow/github_push.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iflow/github_user.py` & `pypipr-1.0.98/pypipr/iflow/github_user.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iflow/pip_freeze_without_version.py` & `pypipr-1.0.98/pypipr/iflow/pip_freeze_without_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/iflow/poetry_update_version.py` & `pypipr-1.0.98/pypipr/iflow/poetry_update_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/iargv.py` & `pypipr-1.0.98/pypipr/ifunctions/iargv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/idumps.py` & `pypipr-1.0.98/pypipr/ifunctions/idumps.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/idumps_html.py` & `pypipr-1.0.98/pypipr/ifunctions/idumps_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/ienv.py` & `pypipr-1.0.98/pypipr/ifunctions/ienv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/ijoin.py` & `pypipr-1.0.98/pypipr/ifunctions/ijoin.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/iloads.py` & `pypipr-1.0.98/pypipr/ifunctions/iloads.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/iloads_html.py` & `pypipr-1.0.98/pypipr/ifunctions/iloads_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/iopen.py` & `pypipr-1.0.98/pypipr/ifunctions/iopen.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/iprint.py` & `pypipr-1.0.98/pypipr/ifunctions/iprint.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/irange.py` & `pypipr-1.0.98/pypipr/ifunctions/irange.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/ireplace.py` & `pypipr-1.0.98/pypipr/ifunctions/ireplace.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/ifunctions/iscandir.py` & `pypipr-1.0.98/pypipr/ifunctions/iscandir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/pypipr.py.bak` & `pypipr-1.0.98/pypipr/pypipr.py.bak`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pypipr/terminal.py` & `pypipr-1.0.98/pypipr/terminal.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.97/pyproject.toml` & `pypipr-1.0.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypipr"
-version = "1.0.97"
+version = "1.0.98"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
```

### Comparing `pypipr-1.0.97/readme.md` & `pypipr-1.0.98/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 print(chr_to_int('z'))  # Output: 26  
 print(chr_to_int('aa'))  # Output: 27  
 print(chr_to_int('abc', numbers="abc"))  # Output: 10  
 ```
 
 Output:
 ```py
-25
 26
-17
+27
+18
 ```
 
 ## chunk_array
 
 `chunk_array(array, size, start=0)`
 
 Membagi array menjadi potongan-potongan dengan besaran yg diinginkan  
@@ -93,15 +93,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x7693218140>
+<generator object chunk_array at 0x776a6b4140>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -144,17 +144,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-28 20:09:20.747067+07:00
-2024-04-28 13:09:20.748416+00:00
-2024-04-28 06:09:20.751713-07:00
+2024-04-28 20:23:44.929045+07:00
+2024-04-28 13:23:44.930043+00:00
+2024-04-28 06:23:44.931315-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -213,15 +213,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x76931aed40>
+<generator object filter_empty at 0x776a646d40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -259,16 +259,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x76931af010>
-[<function ExampleGetClassMethod.a at 0x7693221800>, <function ExampleGetClassMethod.b at 0x76932216c0>, <function ExampleGetClassMethod.c at 0x76932218a0>, <function ExampleGetClassMethod.d at 0x7693221940>]
+<generator object get_class_method at 0x776a647010>
+[<function ExampleGetClassMethod.a at 0x776a6b9760>, <function ExampleGetClassMethod.b at 0x776a6b9620>, <function ExampleGetClassMethod.c at 0x776a6b9800>, <function ExampleGetClassMethod.d at 0x776a6b98a0>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -434,15 +434,15 @@
 Output:
 ```py
 {'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
             'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
             'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
             'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
             'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x769a347750>)>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x7770ee6f90>)>,
             'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
             'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
             'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
             'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
             'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
             'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
             'io': <module 'io' (frozen)>,
@@ -472,90 +472,90 @@
             'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
  'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
            'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
            'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
            'PintUregQuantity': <class 'pint.Quantity'>},
  'variable': {'LINUX': True,
               'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x76a14a7d50>},
- 'function': {'avg': <function avg at 0x76a41aed40>,
-              'basename': <function basename at 0x76a417e8e0>,
-              'chr_to_int': <function chr_to_int at 0x76a13e5080>,
-              'chunk_array': <function chunk_array at 0x76a13e5260>,
-              'create_folder': <function create_folder at 0x76a13e5440>,
-              'datetime_from_string': <function datetime_from_string at 0x76a13e5620>,
-              'datetime_now': <function datetime_now at 0x76a148d620>,
-              'dict_first': <function dict_first at 0x76a148d580>,
-              'dirname': <function dirname at 0x76a148d4e0>,
-              'exit_if_empty': <function exit_if_empty at 0x76a148d3a0>,
-              'filter_empty': <function filter_empty at 0x76a148d1c0>,
-              'get_by_index': <function get_by_index at 0x76a148ce00>,
-              'get_class_method': <function get_class_method at 0x76a148ccc0>,
-              'get_filemtime': <function get_filemtime at 0x76a148cb80>,
-              'get_filesize': <function get_filesize at 0x76a148c9a0>,
-              'int_to_chr': <function int_to_chr at 0x76a148c900>,
-              'is_empty': <function is_empty at 0x76a148d260>,
-              'is_iterable': <function is_iterable at 0x76a148cfe0>,
-              'is_valid_url': <function is_valid_url at 0x76a148c7c0>,
-              'ivars': <function ivars at 0x76a148c720>,
-              'password_generator': <function password_generator at 0x76a148c180>,
-              'random_bool': <function random_bool at 0x76a148c4a0>,
-              'restart': <function restart at 0x76a148f920>,
-              'set_timeout': <function set_timeout at 0x76a148fa60>,
-              'sets_ordered': <function sets_ordered at 0x76a148fba0>,
-              'str_cmp': <function str_cmp at 0x76a148fc40>,
-              'to_str': <function to_str at 0x76a148cea0>,
-              'choices': <function choices at 0x76a148fce0>,
-              'console_run': <function console_run at 0x76a148ff60>,
-              'input_char': <function input_char at 0x76a14b00e0>,
-              'log': <function log at 0x76a14b02c0>,
-              'print_colorize': <function print_colorize at 0x76a14b0360>,
-              'print_dir': <function print_dir at 0x76a14b04a0>,
-              'print_log': <function print_log at 0x76a14b0180>,
-              'print_to_last_line': <function print_to_last_line at 0x76a148fec0>,
-              'text_colorize': <function text_colorize at 0x76a14b0040>,
-              'batch_calculate': <function batch_calculate at 0x769a33d800>,
-              'batchmaker': <function batchmaker at 0x76a14b05e0>,
-              'calculate': <function calculate at 0x769a33e520>,
-              'auto_reload': <function auto_reload at 0x769a33e7a0>,
-              'github_pull': <function github_pull at 0x769a33e2a0>,
-              'github_push': <function github_push at 0x769a33e980>,
-              'github_user': <function github_user at 0x769a33eca0>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x769a076200>,
-              'poetry_publish': <function poetry_publish at 0x769a0763e0>,
-              'poetry_update_version': <function poetry_update_version at 0x769a09ac00>,
-              'iargv': <function iargv at 0x76933e8360>,
-              'idumps': <function idumps at 0x76933e84a0>,
-              'idumps_html': <function idumps_html at 0x7693450ea0>,
-              'ienv': <function ienv at 0x76933e85e0>,
-              'iexec': <function iexec at 0x7693451120>,
-              'ijoin': <function ijoin at 0x769a076160>,
-              'iloads': <function iloads at 0x76934511c0>,
-              'iloads_html': <function iloads_html at 0x7693451440>,
-              'iopen': <function iopen at 0x769a076480>,
-              'iprint': <function iprint at 0x7693451300>,
-              'irange': <function irange at 0x769a33e660>,
-              'ireplace': <function ireplace at 0x76934514e0>,
-              'iscandir': <function iscandir at 0x7693453100>,
-              'isplit': <function isplit at 0x76934531a0>}}
+              'PintUreg': <pint.registry.UnitRegistry object at 0x7776e3fd50>},
+ 'function': {'avg': <function avg at 0x777bfb6d40>,
+              'basename': <function basename at 0x777bf868e0>,
+              'chr_to_int': <function chr_to_int at 0x7776d79080>,
+              'chunk_array': <function chunk_array at 0x7776d791c0>,
+              'create_folder': <function create_folder at 0x7776d793a0>,
+              'datetime_from_string': <function datetime_from_string at 0x7776d79580>,
+              'datetime_now': <function datetime_now at 0x7776e21620>,
+              'dict_first': <function dict_first at 0x7776e21580>,
+              'dirname': <function dirname at 0x7776e214e0>,
+              'exit_if_empty': <function exit_if_empty at 0x7776e213a0>,
+              'filter_empty': <function filter_empty at 0x7776e211c0>,
+              'get_by_index': <function get_by_index at 0x7776e20e00>,
+              'get_class_method': <function get_class_method at 0x7776e20cc0>,
+              'get_filemtime': <function get_filemtime at 0x7776e20b80>,
+              'get_filesize': <function get_filesize at 0x7776e209a0>,
+              'int_to_chr': <function int_to_chr at 0x7776e20900>,
+              'is_empty': <function is_empty at 0x7776e21260>,
+              'is_iterable': <function is_iterable at 0x7776e20fe0>,
+              'is_valid_url': <function is_valid_url at 0x7776e207c0>,
+              'ivars': <function ivars at 0x7776e20720>,
+              'password_generator': <function password_generator at 0x7776e205e0>,
+              'random_bool': <function random_bool at 0x7776e20400>,
+              'restart': <function restart at 0x7776e23880>,
+              'set_timeout': <function set_timeout at 0x7776e239c0>,
+              'sets_ordered': <function sets_ordered at 0x7776e23b00>,
+              'str_cmp': <function str_cmp at 0x7776e23ba0>,
+              'to_str': <function to_str at 0x7776e20f40>,
+              'choices': <function choices at 0x7776e23c40>,
+              'console_run': <function console_run at 0x7776e23ec0>,
+              'input_char': <function input_char at 0x7776e44040>,
+              'log': <function log at 0x7776e44220>,
+              'print_colorize': <function print_colorize at 0x7776e442c0>,
+              'print_dir': <function print_dir at 0x7776e44400>,
+              'print_log': <function print_log at 0x7776e440e0>,
+              'print_to_last_line': <function print_to_last_line at 0x7776e23e20>,
+              'text_colorize': <function text_colorize at 0x7776e23f60>,
+              'batch_calculate': <function batch_calculate at 0x7770ef1760>,
+              'batchmaker': <function batchmaker at 0x7776e44540>,
+              'calculate': <function calculate at 0x7770ef2480>,
+              'auto_reload': <function auto_reload at 0x7770ef2700>,
+              'github_pull': <function github_pull at 0x7770ef2200>,
+              'github_push': <function github_push at 0x7770ef28e0>,
+              'github_user': <function github_user at 0x7770ef2c00>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x7770c22160>,
+              'poetry_publish': <function poetry_publish at 0x7770c22340>,
+              'poetry_update_version': <function poetry_update_version at 0x7770c46b60>,
+              'iargv': <function iargv at 0x776d2702c0>,
+              'idumps': <function idumps at 0x776d270400>,
+              'idumps_html': <function idumps_html at 0x776d2d4e00>,
+              'ienv': <function ienv at 0x776d270540>,
+              'iexec': <function iexec at 0x776d2d5080>,
+              'ijoin': <function ijoin at 0x7770c220c0>,
+              'iloads': <function iloads at 0x776d2d5120>,
+              'iloads_html': <function iloads_html at 0x776d2d53a0>,
+              'iopen': <function iopen at 0x7770c223e0>,
+              'iprint': <function iprint at 0x776d2d5260>,
+              'irange': <function irange at 0x7770ef25c0>,
+              'ireplace': <function ireplace at 0x776d2d5440>,
+              'iscandir': <function iscandir at 0x776d2d7060>,
+              'isplit': <function isplit at 0x776d2d7100>}}
 ```
 
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-(\Rowj%0
+5M|h(ik`
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -565,15 +565,15 @@
   
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-False
+True
 ```
 
 ## restart
 
 `restart(*argv)`
 
 ## set_timeout
@@ -591,15 +591,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 509250788592)>
+<Timer(Thread-2, started 512858504432)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -609,15 +609,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x76932282b0>
+<generator object sets_ordered at 0x776a6c42b0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -763,29 +763,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : -3350061026485791588
+            __hash__ : -1747193618484435558
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x76a145cc50>
-               _hash : -3350061026485791588
+            _flavour : <pathlib._PosixFlavour object at 0x7776df0bd0>
+               _hash : -1747193618484435558
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -799,15 +799,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x7693204740>
+             iterdir : <generator object Path.iterdir at 0x776a69c740>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -866,15 +866,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x76931afb50>
+<generator object batch_calculate at 0x776a647b50>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -891,15 +891,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x76932143a0>
+<generator object batchmaker at 0x776a6b03a0>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1255,15 +1255,15 @@
     recursive_flat=True))  
 print(ijoin(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(ijoin(10, ' '))  
 ```
 
 Output:
 ```py
-weq, asd, qweqw, dfs
+qweqw, dfs, weq, asd
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -1364,15 +1364,15 @@
    ':Rp. 1.222.000/gram',
    'Update harga LM Pegadaian :31 Agustus 2023']],
  [['Spot Harga Emas Hari Ini (Market Close)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
   ['Ounce\xa0(oz)', '2.337,94 (+3,37)', '16.208,00', '37.893.332'],
   ['Gram\xa0(gr)', '75,17', '16.208,00', '1.218.299 (+1.756)'],
   ['Kilogram\xa0(kg)', '75.166,52', '16.208,00', '1.218.298.900'],
-  ['Update harga emas :28 April 2024, pukul 20:09Update kurs :28 April 2024, '
+  ['Update harga emas :28 April 2024, pukul 20:23Update kurs :28 April 2024, '
    'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100', '126.812.000', '1.268.120', '124.985.000', '1.249.850'],
   ['50', '63.445.000', '1.268.900', '62.545.000', '1.250.900'],
   ['25', '31.762.000', '1.270.480', '31.375.000', '1.255.000'],
@@ -1415,15 +1415,15 @@
   ['gr', '41,27', '+33,90+82,13%', '586.653', '+631.646+107,67%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
   ['USD', '75,17↓', '%'],
   ['KURS', '16.241,30↓', '%'],
   ['IDR', '1.220.801,94↓', '%'],
-  ['Minggu, 28 April 2024 20:09']],
+  ['Minggu, 28 April 2024 20:23']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
@@ -1480,15 +1480,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x76a41be3a0>, <Element a at 0x7693256a80>, <Element a at 0x7693256b20>, <Element a at 0x7693256b70>, <Element a at 0x7693256bc0>, <Element a at 0x7693256c10>, <Element a at 0x7693256c60>, <Element a at 0x7693256cb0>, <Element a at 0x7693256d00>, <Element a at 0x7693256d50>, <Element a at 0x7693256da0>, <Element a at 0x7693256df0>, <Element a at 0x7693256e40>, <Element a at 0x7693256e90>, <Element a at 0x7693256ee0>, <Element a at 0x7693256f30>, <Element a at 0x7693256f80>, <Element a at 0x7693256fd0>]
+[<Element a at 0x776a6a7d90>, <Element a at 0x776a6f2990>, <Element a at 0x776a6f2a30>, <Element a at 0x776a6f2a80>, <Element a at 0x776a6f2ad0>, <Element a at 0x776a6f2b20>, <Element a at 0x776a6f2b70>, <Element a at 0x776a6f2bc0>, <Element a at 0x776a6f2c10>, <Element a at 0x776a6f2c60>, <Element a at 0x776a6f2cb0>, <Element a at 0x776a6f2d00>, <Element a at 0x776a6f2d50>, <Element a at 0x776a6f2da0>, <Element a at 0x776a6f2df0>, <Element a at 0x776a6f2e40>, <Element a at 0x776a6f2e90>, <Element a at 0x776a6f2ee0>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1521,16 +1521,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x76931e2bd0>
-<generator object irange at 0x76931e2bd0>
+<generator object irange at 0x776a67abd0>
+<generator object irange at 0x776a67abd0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1565,15 +1565,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x7693218740>
+<generator object iscandir at 0x776a6b4740>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1622,15 +1622,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x76932285f0>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x776a6c45f0>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
```

### Comparing `pypipr-1.0.97/PKG-INFO` & `pypipr-1.0.98/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 1.0.97
+Version: 1.0.98
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -97,17 +97,17 @@
 print(chr_to_int('z'))  # Output: 26  
 print(chr_to_int('aa'))  # Output: 27  
 print(chr_to_int('abc', numbers="abc"))  # Output: 10  
 ```
 
 Output:
 ```py
-25
 26
-17
+27
+18
 ```
 
 ## chunk_array
 
 `chunk_array(array, size, start=0)`
 
 Membagi array menjadi potongan-potongan dengan besaran yg diinginkan  
@@ -116,15 +116,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x7693218140>
+<generator object chunk_array at 0x776a6b4140>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -167,17 +167,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-28 20:09:20.747067+07:00
-2024-04-28 13:09:20.748416+00:00
-2024-04-28 06:09:20.751713-07:00
+2024-04-28 20:23:44.929045+07:00
+2024-04-28 13:23:44.930043+00:00
+2024-04-28 06:23:44.931315-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -236,15 +236,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x76931aed40>
+<generator object filter_empty at 0x776a646d40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -282,16 +282,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x76931af010>
-[<function ExampleGetClassMethod.a at 0x7693221800>, <function ExampleGetClassMethod.b at 0x76932216c0>, <function ExampleGetClassMethod.c at 0x76932218a0>, <function ExampleGetClassMethod.d at 0x7693221940>]
+<generator object get_class_method at 0x776a647010>
+[<function ExampleGetClassMethod.a at 0x776a6b9760>, <function ExampleGetClassMethod.b at 0x776a6b9620>, <function ExampleGetClassMethod.c at 0x776a6b9800>, <function ExampleGetClassMethod.d at 0x776a6b98a0>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -457,15 +457,15 @@
 Output:
 ```py
 {'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
             'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
             'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
             'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
             'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x769a347750>)>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x7770ee6f90>)>,
             'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
             'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
             'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
             'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
             'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
             'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
             'io': <module 'io' (frozen)>,
@@ -495,90 +495,90 @@
             'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
  'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
            'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
            'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
            'PintUregQuantity': <class 'pint.Quantity'>},
  'variable': {'LINUX': True,
               'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x76a14a7d50>},
- 'function': {'avg': <function avg at 0x76a41aed40>,
-              'basename': <function basename at 0x76a417e8e0>,
-              'chr_to_int': <function chr_to_int at 0x76a13e5080>,
-              'chunk_array': <function chunk_array at 0x76a13e5260>,
-              'create_folder': <function create_folder at 0x76a13e5440>,
-              'datetime_from_string': <function datetime_from_string at 0x76a13e5620>,
-              'datetime_now': <function datetime_now at 0x76a148d620>,
-              'dict_first': <function dict_first at 0x76a148d580>,
-              'dirname': <function dirname at 0x76a148d4e0>,
-              'exit_if_empty': <function exit_if_empty at 0x76a148d3a0>,
-              'filter_empty': <function filter_empty at 0x76a148d1c0>,
-              'get_by_index': <function get_by_index at 0x76a148ce00>,
-              'get_class_method': <function get_class_method at 0x76a148ccc0>,
-              'get_filemtime': <function get_filemtime at 0x76a148cb80>,
-              'get_filesize': <function get_filesize at 0x76a148c9a0>,
-              'int_to_chr': <function int_to_chr at 0x76a148c900>,
-              'is_empty': <function is_empty at 0x76a148d260>,
-              'is_iterable': <function is_iterable at 0x76a148cfe0>,
-              'is_valid_url': <function is_valid_url at 0x76a148c7c0>,
-              'ivars': <function ivars at 0x76a148c720>,
-              'password_generator': <function password_generator at 0x76a148c180>,
-              'random_bool': <function random_bool at 0x76a148c4a0>,
-              'restart': <function restart at 0x76a148f920>,
-              'set_timeout': <function set_timeout at 0x76a148fa60>,
-              'sets_ordered': <function sets_ordered at 0x76a148fba0>,
-              'str_cmp': <function str_cmp at 0x76a148fc40>,
-              'to_str': <function to_str at 0x76a148cea0>,
-              'choices': <function choices at 0x76a148fce0>,
-              'console_run': <function console_run at 0x76a148ff60>,
-              'input_char': <function input_char at 0x76a14b00e0>,
-              'log': <function log at 0x76a14b02c0>,
-              'print_colorize': <function print_colorize at 0x76a14b0360>,
-              'print_dir': <function print_dir at 0x76a14b04a0>,
-              'print_log': <function print_log at 0x76a14b0180>,
-              'print_to_last_line': <function print_to_last_line at 0x76a148fec0>,
-              'text_colorize': <function text_colorize at 0x76a14b0040>,
-              'batch_calculate': <function batch_calculate at 0x769a33d800>,
-              'batchmaker': <function batchmaker at 0x76a14b05e0>,
-              'calculate': <function calculate at 0x769a33e520>,
-              'auto_reload': <function auto_reload at 0x769a33e7a0>,
-              'github_pull': <function github_pull at 0x769a33e2a0>,
-              'github_push': <function github_push at 0x769a33e980>,
-              'github_user': <function github_user at 0x769a33eca0>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x769a076200>,
-              'poetry_publish': <function poetry_publish at 0x769a0763e0>,
-              'poetry_update_version': <function poetry_update_version at 0x769a09ac00>,
-              'iargv': <function iargv at 0x76933e8360>,
-              'idumps': <function idumps at 0x76933e84a0>,
-              'idumps_html': <function idumps_html at 0x7693450ea0>,
-              'ienv': <function ienv at 0x76933e85e0>,
-              'iexec': <function iexec at 0x7693451120>,
-              'ijoin': <function ijoin at 0x769a076160>,
-              'iloads': <function iloads at 0x76934511c0>,
-              'iloads_html': <function iloads_html at 0x7693451440>,
-              'iopen': <function iopen at 0x769a076480>,
-              'iprint': <function iprint at 0x7693451300>,
-              'irange': <function irange at 0x769a33e660>,
-              'ireplace': <function ireplace at 0x76934514e0>,
-              'iscandir': <function iscandir at 0x7693453100>,
-              'isplit': <function isplit at 0x76934531a0>}}
+              'PintUreg': <pint.registry.UnitRegistry object at 0x7776e3fd50>},
+ 'function': {'avg': <function avg at 0x777bfb6d40>,
+              'basename': <function basename at 0x777bf868e0>,
+              'chr_to_int': <function chr_to_int at 0x7776d79080>,
+              'chunk_array': <function chunk_array at 0x7776d791c0>,
+              'create_folder': <function create_folder at 0x7776d793a0>,
+              'datetime_from_string': <function datetime_from_string at 0x7776d79580>,
+              'datetime_now': <function datetime_now at 0x7776e21620>,
+              'dict_first': <function dict_first at 0x7776e21580>,
+              'dirname': <function dirname at 0x7776e214e0>,
+              'exit_if_empty': <function exit_if_empty at 0x7776e213a0>,
+              'filter_empty': <function filter_empty at 0x7776e211c0>,
+              'get_by_index': <function get_by_index at 0x7776e20e00>,
+              'get_class_method': <function get_class_method at 0x7776e20cc0>,
+              'get_filemtime': <function get_filemtime at 0x7776e20b80>,
+              'get_filesize': <function get_filesize at 0x7776e209a0>,
+              'int_to_chr': <function int_to_chr at 0x7776e20900>,
+              'is_empty': <function is_empty at 0x7776e21260>,
+              'is_iterable': <function is_iterable at 0x7776e20fe0>,
+              'is_valid_url': <function is_valid_url at 0x7776e207c0>,
+              'ivars': <function ivars at 0x7776e20720>,
+              'password_generator': <function password_generator at 0x7776e205e0>,
+              'random_bool': <function random_bool at 0x7776e20400>,
+              'restart': <function restart at 0x7776e23880>,
+              'set_timeout': <function set_timeout at 0x7776e239c0>,
+              'sets_ordered': <function sets_ordered at 0x7776e23b00>,
+              'str_cmp': <function str_cmp at 0x7776e23ba0>,
+              'to_str': <function to_str at 0x7776e20f40>,
+              'choices': <function choices at 0x7776e23c40>,
+              'console_run': <function console_run at 0x7776e23ec0>,
+              'input_char': <function input_char at 0x7776e44040>,
+              'log': <function log at 0x7776e44220>,
+              'print_colorize': <function print_colorize at 0x7776e442c0>,
+              'print_dir': <function print_dir at 0x7776e44400>,
+              'print_log': <function print_log at 0x7776e440e0>,
+              'print_to_last_line': <function print_to_last_line at 0x7776e23e20>,
+              'text_colorize': <function text_colorize at 0x7776e23f60>,
+              'batch_calculate': <function batch_calculate at 0x7770ef1760>,
+              'batchmaker': <function batchmaker at 0x7776e44540>,
+              'calculate': <function calculate at 0x7770ef2480>,
+              'auto_reload': <function auto_reload at 0x7770ef2700>,
+              'github_pull': <function github_pull at 0x7770ef2200>,
+              'github_push': <function github_push at 0x7770ef28e0>,
+              'github_user': <function github_user at 0x7770ef2c00>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x7770c22160>,
+              'poetry_publish': <function poetry_publish at 0x7770c22340>,
+              'poetry_update_version': <function poetry_update_version at 0x7770c46b60>,
+              'iargv': <function iargv at 0x776d2702c0>,
+              'idumps': <function idumps at 0x776d270400>,
+              'idumps_html': <function idumps_html at 0x776d2d4e00>,
+              'ienv': <function ienv at 0x776d270540>,
+              'iexec': <function iexec at 0x776d2d5080>,
+              'ijoin': <function ijoin at 0x7770c220c0>,
+              'iloads': <function iloads at 0x776d2d5120>,
+              'iloads_html': <function iloads_html at 0x776d2d53a0>,
+              'iopen': <function iopen at 0x7770c223e0>,
+              'iprint': <function iprint at 0x776d2d5260>,
+              'irange': <function irange at 0x7770ef25c0>,
+              'ireplace': <function ireplace at 0x776d2d5440>,
+              'iscandir': <function iscandir at 0x776d2d7060>,
+              'isplit': <function isplit at 0x776d2d7100>}}
 ```
 
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-(\Rowj%0
+5M|h(ik`
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -588,15 +588,15 @@
   
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-False
+True
 ```
 
 ## restart
 
 `restart(*argv)`
 
 ## set_timeout
@@ -614,15 +614,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 509250788592)>
+<Timer(Thread-2, started 512858504432)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -632,15 +632,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x76932282b0>
+<generator object sets_ordered at 0x776a6c42b0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -786,29 +786,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : -3350061026485791588
+            __hash__ : -1747193618484435558
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x76a145cc50>
-               _hash : -3350061026485791588
+            _flavour : <pathlib._PosixFlavour object at 0x7776df0bd0>
+               _hash : -1747193618484435558
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -822,15 +822,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x7693204740>
+             iterdir : <generator object Path.iterdir at 0x776a69c740>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -889,15 +889,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x76931afb50>
+<generator object batch_calculate at 0x776a647b50>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -914,15 +914,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x76932143a0>
+<generator object batchmaker at 0x776a6b03a0>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1278,15 +1278,15 @@
     recursive_flat=True))  
 print(ijoin(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(ijoin(10, ' '))  
 ```
 
 Output:
 ```py
-weq, asd, qweqw, dfs
+qweqw, dfs, weq, asd
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -1387,15 +1387,15 @@
    ':Rp. 1.222.000/gram',
    'Update harga LM Pegadaian :31 Agustus 2023']],
  [['Spot Harga Emas Hari Ini (Market Close)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
   ['Ounce\xa0(oz)', '2.337,94 (+3,37)', '16.208,00', '37.893.332'],
   ['Gram\xa0(gr)', '75,17', '16.208,00', '1.218.299 (+1.756)'],
   ['Kilogram\xa0(kg)', '75.166,52', '16.208,00', '1.218.298.900'],
-  ['Update harga emas :28 April 2024, pukul 20:09Update kurs :28 April 2024, '
+  ['Update harga emas :28 April 2024, pukul 20:23Update kurs :28 April 2024, '
    'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100', '126.812.000', '1.268.120', '124.985.000', '1.249.850'],
   ['50', '63.445.000', '1.268.900', '62.545.000', '1.250.900'],
   ['25', '31.762.000', '1.270.480', '31.375.000', '1.255.000'],
@@ -1438,15 +1438,15 @@
   ['gr', '41,27', '+33,90+82,13%', '586.653', '+631.646+107,67%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
   ['USD', '75,17↓', '%'],
   ['KURS', '16.241,30↓', '%'],
   ['IDR', '1.220.801,94↓', '%'],
-  ['Minggu, 28 April 2024 20:09']],
+  ['Minggu, 28 April 2024 20:23']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
@@ -1503,15 +1503,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x76a41be3a0>, <Element a at 0x7693256a80>, <Element a at 0x7693256b20>, <Element a at 0x7693256b70>, <Element a at 0x7693256bc0>, <Element a at 0x7693256c10>, <Element a at 0x7693256c60>, <Element a at 0x7693256cb0>, <Element a at 0x7693256d00>, <Element a at 0x7693256d50>, <Element a at 0x7693256da0>, <Element a at 0x7693256df0>, <Element a at 0x7693256e40>, <Element a at 0x7693256e90>, <Element a at 0x7693256ee0>, <Element a at 0x7693256f30>, <Element a at 0x7693256f80>, <Element a at 0x7693256fd0>]
+[<Element a at 0x776a6a7d90>, <Element a at 0x776a6f2990>, <Element a at 0x776a6f2a30>, <Element a at 0x776a6f2a80>, <Element a at 0x776a6f2ad0>, <Element a at 0x776a6f2b20>, <Element a at 0x776a6f2b70>, <Element a at 0x776a6f2bc0>, <Element a at 0x776a6f2c10>, <Element a at 0x776a6f2c60>, <Element a at 0x776a6f2cb0>, <Element a at 0x776a6f2d00>, <Element a at 0x776a6f2d50>, <Element a at 0x776a6f2da0>, <Element a at 0x776a6f2df0>, <Element a at 0x776a6f2e40>, <Element a at 0x776a6f2e90>, <Element a at 0x776a6f2ee0>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1544,16 +1544,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x76931e2bd0>
-<generator object irange at 0x76931e2bd0>
+<generator object irange at 0x776a67abd0>
+<generator object irange at 0x776a67abd0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1588,15 +1588,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x7693218740>
+<generator object iscandir at 0x776a6b4740>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1645,15 +1645,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x76932285f0>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x776a6c45f0>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
```

