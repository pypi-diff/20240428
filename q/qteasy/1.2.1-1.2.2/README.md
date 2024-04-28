# Comparing `tmp/qteasy-1.2.1.tar.gz` & `tmp/qteasy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-_y_lp3e3/qteasy-1.2.1.tar", last modified: Tue Apr 23 13:08:28 2024, max compression
+gzip compressed data, was "qteasy-1.2.2.tar", last modified: Sun Apr 28 16:37:03 2024, max compression
```

## Comparing `qteasy-1.2.1.tar` & `qteasy-1.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 13:08:28.000000 qteasy-1.2.1/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.1/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    28538 2024-04-23 13:08:28.000000 qteasy-1.2.1/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    25292 2024-04-23 12:59:07.000000 qteasy-1.2.1/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2236 2024-04-23 12:59:07.000000 qteasy-1.2.1/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8587 2024-04-23 12:59:07.000000 qteasy-1.2.1/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-04-23 09:42:51.000000 qteasy-1.2.1/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-21 23:36:55.000000 qteasy-1.2.1/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.1/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-04-23 05:23:43.000000 qteasy-1.2.1/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.2.1/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   111230 2024-04-23 12:18:08.000000 qteasy-1.2.1/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   390977 2024-04-23 10:14:34.000000 qteasy-1.2.1/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.1/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-21 23:36:55.000000 qteasy-1.2.1/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-05 14:28:39.000000 qteasy-1.2.1/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.1/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.2.1/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.2.1/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.1/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.2.1/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.2.1/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-04-23 10:20:55.000000 qteasy-1.2.1/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-04-23 09:39:03.000000 qteasy-1.2.1/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-04-23 10:08:45.000000 qteasy-1.2.1/qteasy/trader_cli.py
--rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-04-23 05:23:43.000000 qteasy-1.2.1/qteasy/trader_tui.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 14:28:39.000000 qteasy-1.2.1/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.1/qteasy/tsfuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)      840 2024-04-23 05:23:43.000000 qteasy-1.2.1/qteasy/tui_style.tcss
--rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-04-23 05:23:43.000000 qteasy-1.2.1/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.1/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    28538 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.1/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      155 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-23 13:08:28.000000 qteasy-1.2.1/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1580 2024-04-23 13:08:28.000000 qteasy-1.2.1/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.1/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 13:08:28.000000 qteasy-1.2.1/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.2.1/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.1/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.1/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.1/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.2.1/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-04-23 05:23:43.000000 qteasy-1.2.1/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.1/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.1/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.1/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.1/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.1/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.1/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-05 14:28:39.000000 qteasy-1.2.1/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-07 13:30:44.000000 qteasy-1.2.1/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.1/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.2.1/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-04-23 05:23:43.000000 qteasy-1.2.1/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-04-23 05:23:43.000000 qteasy-1.2.1/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.1/tests/test_trading.py
--rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-04-23 05:23:43.000000 qteasy-1.2.1/tests/test_tui.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.1/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.1/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.1/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.539524 qteasy-1.2.2/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.2/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    29111 2024-04-28 16:37:03.539268 qteasy-1.2.2/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    25387 2024-04-28 16:32:22.000000 qteasy-1.2.2/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-04-28 16:32:22.000000 qteasy-1.2.2/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.526354 qteasy-1.2.2/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-04-28 16:32:22.000000 qteasy-1.2.2/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-27 10:02:20.000000 qteasy-1.2.2/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.2/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-04-23 05:23:43.000000 qteasy-1.2.2/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142505 2024-04-28 16:28:11.000000 qteasy-1.2.2/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   111230 2024-04-27 14:57:02.000000 qteasy-1.2.2/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   390977 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.2/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-21 23:36:55.000000 qteasy-1.2.2/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-27 10:02:29.000000 qteasy-1.2.2/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.2/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.2.2/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.2.2/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.2/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-04-28 16:28:11.000000 qteasy-1.2.2/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   156061 2024-04-28 16:28:11.000000 qteasy-1.2.2/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/trader_cli.py
+-rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-04-23 05:23:43.000000 qteasy-1.2.2/qteasy/trader_tui.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 14:28:39.000000 qteasy-1.2.2/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.2/qteasy/tsfuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)      840 2024-04-23 05:23:43.000000 qteasy-1.2.2/qteasy/tui_style.tcss
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-04-27 14:12:34.000000 qteasy-1.2.2/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.2/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.538688 qteasy-1.2.2/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    29111 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.2/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      195 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-04-28 16:37:03.539881 qteasy-1.2.2/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.2/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.538414 qteasy-1.2.2/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-04-27 14:13:03.000000 qteasy-1.2.2/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.2/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.2/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.2/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.2/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.2/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.2/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-28 16:28:11.000000 qteasy-1.2.2/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-28 14:32:18.000000 qteasy-1.2.2/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.2/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    40797 2024-04-28 16:28:11.000000 qteasy-1.2.2/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.2/tests/test_trading.py
+-rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_tui.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.2/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.2/tests/test_visual.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qteasy-1.2.1/LICENSE` & `qteasy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/PKG-INFO` & `qteasy-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.1
+Version: 1.2.2
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -39,18 +39,32 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas>=1.1.0
+Requires-Dist: numpy>=1.18.1
+Requires-Dist: numba>=0.47.0
+Requires-Dist: tushare>=1.2.89
+Requires-Dist: mplfinance
+Requires-Dist: rich>=10.0.0
+Requires-Dist: textual
 Provides-Extra: talib
+Requires-Dist: ta-lib; extra == "talib"
 Provides-Extra: database
+Requires-Dist: pymysql>=1.0.0; extra == "database"
 Provides-Extra: feather
-License-File: LICENSE
+Requires-Dist: pyarrow>=3; extra == "feather"
+Provides-Extra: dev
+Requires-Dist: ta-lib; extra == "dev"
+Requires-Dist: pymysql>=1.0.0; extra == "dev"
+Requires-Dist: pyarrow>=3; extra == "dev"
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
@@ -92,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.1`
+- Latest Version: `1.2.2`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -568,14 +582,15 @@
         mode=0,  # 交易模式为实盘运行
         asset_type='E',  # 交易的标的类型为股票
         asset_pool=asset_pool,  # 交易股票池为所有银行股和家用电器股
         trade_batch_size=100,  # 交易批量为100股的整数倍
         sell_batch_size=1,  # 卖出数量为1股的整数倍
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
+        live_trade_ui_type='tui',  # 使用TUI界面监控实盘交易，默认使用CLI界面
 )
 
 qt.run(op)
 ```
 qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
 为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
```

### Comparing `qteasy-1.2.1/README.md` & `qteasy-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.1`
+- Latest Version: `1.2.2`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -518,14 +518,15 @@
         mode=0,  # 交易模式为实盘运行
         asset_type='E',  # 交易的标的类型为股票
         asset_pool=asset_pool,  # 交易股票池为所有银行股和家用电器股
         trade_batch_size=100,  # 交易批量为100股的整数倍
         sell_batch_size=1,  # 卖出数量为1股的整数倍
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
+        live_trade_ui_type='tui',  # 使用TUI界面监控实盘交易，默认使用CLI界面
 )
 
 qt.run(op)
 ```
 qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
 为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
```

### Comparing `qteasy-1.2.1/pyproject.toml` & `qteasy-1.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6, <3.13"
 keywords = ["quantitative investment", "quantitative trading", "stock", "finance", "investment"]
 dependencies = [
-    "pandas>=1.4.0",
+    "pandas>=1.1.0",
     "numpy>=1.18.1",
     "numba>=0.47.0",
     "tushare>=1.2.89",
     "mplfinance",
     "rich>=10.0.0",
     "textual",
 ]
@@ -66,10 +66,15 @@
 Documentation = "https://qteasy.readthedocs.io/zh/latest/"
 Issues = "https://github.com/shepherdpp/qteasy/issues"
 
 [project.optional-dependencies]
 talib = ["ta-lib"]
 database = ["pymysql >= 1.0.0"]
 feather = ["pyarrow >= 3"]
+dev = [
+    "ta-lib",
+    "pymysql >= 1.0.0",
+    "pyarrow >= 3",
+]
 
 [options.package_data]
 qteasy = "*.tcss"
```

### Comparing `qteasy-1.2.1/qteasy/__init__.py` & `qteasy-1.2.2/qteasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 
 
 # qteasy版本信息
 __version__ = '1.2.1'
 version_info = Namespace(
         major=1,
         minor=2,
-        patch=1,
+        patch=2,
         short=(1, 2),
-        full=(1, 2, 1),
-        string='1.2.1',
-        tuple=('1', '2', '1'),
+        full=(1, 2, 2),
+        string='1.2.2',
+        tuple=('1', '2', '2'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
 
@@ -183,14 +183,15 @@
 # if py_ver_major < 3 or (py_ver_major == 3 and py_ver_minor <= 6):
 #     warnings.warn(f'qteasy is not fully tested on Python version {py_ver_major}.{py_ver_minor}, '
 #                   f'it is highly recommended to use python 3.8 or later for qteasy!')
 # elif py_ver_major == 3 and py_ver_minor == 7:
 #     warnings.warn(f'A few features of qteasy are planned to be deprecated in Python 3.7, '
 #                   f'please updated to python 3.8 or later for qteasy!', DeprecationWarning)
 
+
 __all__ = [
     'run', 'set_config', 'get_configurations', 'get_config',
     'info', 'is_ready', 'configure', 'configuration', 'save_config', 'load_config', 'reset_config',
     'get_basic_info', 'get_stock_info', 'get_data_overview', 'refill_data_source',
     'get_history_data', 'filter_stock_codes', 'filter_stocks',
     'reconnect_ds', 'get_table_info', 'get_table_overview',
     'HistoryPanel', 'dataframe_to_hp', 'stack_dataframes',
```

### Comparing `qteasy-1.2.1/qteasy/_arg_validators.py` & `qteasy-1.2.2/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/backtest.py` & `qteasy-1.2.2/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/blender.py` & `qteasy-1.2.2/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/broker.py` & `qteasy-1.2.2/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/built_in.py` & `qteasy-1.2.2/qteasy/built_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Desc:
 #   Qteasy built-in Strategies.
 # ======================================
 
 import numpy as np
 from qteasy.strategy import RuleIterator, GeneralStg, FactorSorter
 # commonly used ta-lib funcs that have a None ta-lib version
-from .tafuncs import sma, ema, trix, bbands
+from .tafuncs import sma, ema, trix, bbands, sma_no_ta, ema_no_ta
 from .tafuncs import ht, kama, mama, t3, tema, trima, wma, sarext, adx
 from .tafuncs import aroon, aroonosc, cci, cmo, macdext, mfi, minus_di
 from .tafuncs import plus_di, minus_dm, plus_dm, mom, ppo, rsi, stoch, stochf
 from .tafuncs import stochrsi, ultosc, willr, ad, dema, apo, cdldoji, atr
 
 
 # Built-in Rolling timing strategies:
@@ -34,15 +34,15 @@
     None: 如果stg_id不为None，但该策略不存在，则返回None
 
     Examples
     --------
     >>> import qteasy as qt
     >>> qt.built_in_list()
     {
-     'crossline': qteasy.built_in.Crossline,
+     'crossline': qteasy.built_in.CROSSLINE,
      'macd': qteasy.built_in.MACD,
      'dma': qteasy.built_in.DMA,
      'trix': qteasy.built_in.TRIX,
      ...
       'ndaychg': qteasy.built_in.SelectingNDayChange,
      'ndayvol': qteasy.built_in.SelectingNDayVolatility
     }
@@ -155,15 +155,15 @@
         raise ValueError(f'stg_id ({stg_id}) is not valid, please check your input')
 
     return BUILT_IN_STRATEGIES[stg_id]()
 
 
 # All following strategies can be used to create strategies by referring to its strategy ID
 # Basic technical analysis based Timing strategies
-class Crossline(RuleIterator):
+class CROSSLINE(RuleIterator):
     """crossline择时策略类，利用长短均线的交叉确定多空状态
 
     策略参数：
         s: int, 短均线计算日期；
         l: int, 长均线计算日期；
         m: float, 均线边界宽度（百分比）；
     信号类型：
@@ -3668,81 +3668,81 @@
 
         # 计算ATR波动率, 因为输入数据包含多个股票的数据，因此需要分别计算每个股票的ATR，然后将结果合并，最后取最后一列（最后一天的ATR）
         factors = np.array(list(map(atr, high, low, close, [n]*len(high))))[:, -1]
 
         return factors
 
 
-BUILT_IN_STRATEGIES = {'crossline':     Crossline,  # TODO: TA-Lib free
-                       'macd':          MACD,  # TODO: TA-Lib free
-                       'dma':           DMA,  # TODO: TA-Lib free
-                       'trix':          TRIX,  # TODO: TA-Lib free
-                       'cdl':           CDL,
-                       'bband':         BBand,
-                       's-bband':       SoftBBand,
-                       'sarext':        SAREXT,
-                       'ssma':          SCRSSMA,
-                       'sdema':         SCRSDEMA,
-                       'sema':          SCRSEMA,
-                       'sht':           SCRSHT,
-                       'skama':         SCRSKAMA,
-                       'smama':         SCRSMAMA,
-                       'st3':           SCRST3,
-                       'stema':         SCRSTEMA,
-                       'strima':        SCRSTRIMA,
-                       'swma':          SCRSWMA,
-                       'dsma':          DCRSSMA,
-                       'ddema':         DCRSDEMA,
-                       'dema':          DCRSEMA,
-                       'dkama':         DCRSKAMA,
-                       'dmama':         DCRSMAMA,
-                       'dt3':           DCRST3,
-                       'dtema':         DCRSTEMA,
-                       'dtrima':        DCRSTRIMA,
-                       'dwma':          DCRSWMA,
-                       'slsma':         SLPSMA,
-                       'sldema':        SLPDEMA,
-                       'slema':         SLPEMA,
-                       'slht':          SLPHT,
-                       'slkama':        SLPKAMA,
-                       'slmama':        SLPMAMA,
-                       'slt3':          SLPT3,
-                       'sltema':        SLPTEMA,
-                       'sltrima':       SLPTRIMA,
-                       'slwma':         SLPWMA,
-                       'adx':           ADX,
-                       'apo':           APO,
-                       'aroon':         AROON,
-                       'aroonosc':      AROONOSC,
-                       'cci':           CCI,
-                       'cmo':           CMO,
-                       'macdext':       MACDEXT,
-                       'mfi':           MFI,
-                       'di':            DI,
-                       'dm':            DM,
-                       'mom':           MOM,
-                       'ppo':           PPO,
-                       'rsi':           RSI,
-                       'stoch':         STOCH,
-                       'stochf':        STOCHF,
-                       'stochrsi':      STOCHRSI,
-                       'ultosc':        ULTOSC,
-                       'willr':         WILLR,
-                       'signal_none':   SignalNone,
-                       'sellrate':      SellRate,
-                       'buyrate':       BuyRate,
-                       'long':          TimingLong,
-                       'short':         TimingShort,
-                       'zero':          TimingZero,
-                       'all':           SelectingAll,
-                       'select_none':   SelectingNone,
-                       'random':        SelectingRandom,
-                       'finance':       SelectingAvgIndicator,
-                       'ndaylast':      SelectingNDayLast,
-                       'ndayavg':       SelectingNDayAvg,
-                       'ndayrate':      SelectingNDayRateChange,
-                       'ndaychg':       SelectingNDayChange,
-                       'ndayvol':       SelectingNDayVolatility
+BUILT_IN_STRATEGIES = {'crossline':         CROSSLINE,
+                       'macd':              MACD,
+                       'dma':               DMA,
+                       'trix':              TRIX,
+                       'cdl':               CDL,
+                       'bband':             BBand,
+                       's-bband':           SoftBBand,
+                       'sarext':            SAREXT,
+                       'ssma':              SCRSSMA,
+                       'sdema':             SCRSDEMA,
+                       'sema':              SCRSEMA,
+                       'sht':               SCRSHT,
+                       'skama':             SCRSKAMA,
+                       'smama':             SCRSMAMA,
+                       'st3':               SCRST3,
+                       'stema':             SCRSTEMA,
+                       'strima':            SCRSTRIMA,
+                       'swma':              SCRSWMA,
+                       'dsma':              DCRSSMA,
+                       'ddema':             DCRSDEMA,
+                       'dema':              DCRSEMA,
+                       'dkama':             DCRSKAMA,
+                       'dmama':             DCRSMAMA,
+                       'dt3':               DCRST3,
+                       'dtema':             DCRSTEMA,
+                       'dtrima':            DCRSTRIMA,
+                       'dwma':              DCRSWMA,
+                       'slsma':             SLPSMA,
+                       'sldema':            SLPDEMA,
+                       'slema':             SLPEMA,
+                       'slht':              SLPHT,
+                       'slkama':            SLPKAMA,
+                       'slmama':            SLPMAMA,
+                       'slt3':              SLPT3,
+                       'sltema':            SLPTEMA,
+                       'sltrima':           SLPTRIMA,
+                       'slwma':             SLPWMA,
+                       'adx':               ADX,
+                       'apo':               APO,
+                       'aroon':             AROON,
+                       'aroonosc':          AROONOSC,
+                       'cci':               CCI,
+                       'cmo':               CMO,
+                       'macdext':           MACDEXT,
+                       'mfi':               MFI,
+                       'di':                DI,
+                       'dm':                DM,
+                       'mom':               MOM,
+                       'ppo':               PPO,
+                       'rsi':               RSI,
+                       'stoch':             STOCH,
+                       'stochf':            STOCHF,
+                       'stochrsi':          STOCHRSI,
+                       'ultosc':            ULTOSC,
+                       'willr':             WILLR,
+                       'signal_none':       SignalNone,
+                       'sellrate':          SellRate,
+                       'buyrate':           BuyRate,
+                       'long':              TimingLong,
+                       'short':             TimingShort,
+                       'zero':              TimingZero,
+                       'all':               SelectingAll,
+                       'select_none':       SelectingNone,
+                       'random':            SelectingRandom,
+                       'finance':           SelectingAvgIndicator,
+                       'ndaylast':          SelectingNDayLast,
+                       'ndayavg':           SelectingNDayAvg,
+                       'ndayrate':          SelectingNDayRateChange,
+                       'ndaychg':           SelectingNDayChange,
+                       'ndayvol':           SelectingNDayVolatility
                        }
 
 
 available_built_in_strategies = BUILT_IN_STRATEGIES.values()
```

### Comparing `qteasy-1.2.1/qteasy/core.py` & `qteasy-1.2.2/qteasy/core.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/database.py` & `qteasy-1.2.2/qteasy/database.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/emfuncs.py` & `qteasy-1.2.2/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/evaluate.py` & `qteasy-1.2.2/qteasy/evaluate.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/finance.py` & `qteasy-1.2.2/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/history.py` & `qteasy-1.2.2/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/optimization.py` & `qteasy-1.2.2/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/qt_operator.py` & `qteasy-1.2.2/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/space.py` & `qteasy-1.2.2/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/strategy.py` & `qteasy-1.2.2/qteasy/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1807,21 +1807,18 @@
         # 仅针对非nan值计算，忽略股票停牌时期
         hist_nonan = h_seg[~np.isnan(h_seg[:, 0])]
         if ref_seg is None:
             ref_nonan = None
         else:
             ref_nonan = ref_seg[~np.isnan(ref_seg[:, 0])]
 
-        try:
-            return self.realize(h=hist_nonan,
-                                r=ref_nonan,
-                                t=trade_data,
-                                pars=params)
-        except Exception:
-            return np.nan
+        return self.realize(h=hist_nonan,
+                            r=ref_nonan,
+                            t=trade_data,
+                            pars=params)
 
     @abstractmethod
     def realize(self,
                 h,
                 r=None,
                 t=None,
                 pars=None):
```

### Comparing `qteasy-1.2.1/qteasy/tafuncs.py` & `qteasy-1.2.2/qteasy/tafuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,46 @@
 # Author:   Jackie PENG
 # Contact:  jackie.pengzhao@gmail.com
 # Created:  2020-09-27
 # Desc:
 #   Interfaces to ta-lib functions.
 # ======================================
 
+
+# 尝试导入ta-lib，如果导入失败，打印warning信息，设置flag: TA_LIB_AVAILABLE = False
 import numpy as np
+import warnings
+
 try:
     # noinspection PyUnresolvedReferences
-    from talib import BBANDS, HT_TRENDLINE, KAMA, MA, MAMA, MAVP, MIDPOINT, MIDPRICE, SAR, SAREXT, \
-        T3, TEMA, TRIMA, WMA, ADX, ADXR, APO, BOP, CCI, CMO, DX, MACDEXT, AROON, AROONOSC, \
+    from talib import SMA, BBANDS, HT_TRENDLINE, KAMA, MA, MAMA, MAVP, MIDPOINT, MIDPRICE, SAR, SAREXT, \
+        T3, TEMA, TRIMA, WMA, ADX, ADXR, APO, BOP, CCI, CMO, DX, MACDEXT, AROON, AROONOSC, MACD, DEMA, \
         MFI, MINUS_DI, MINUS_DM, MOM, PLUS_DI, PLUS_DM, PPO, ROC, ROCP, ROCR, ROCR100, RSI, STOCH, \
         STOCHF, STOCHRSI, ULTOSC, WILLR, AD, ADOSC, OBV, ATR, NATR, TRANGE, AVGPRICE, MEDPRICE, TYPPRICE, \
         WCLPRICE, HT_DCPERIOD, HT_DCPHASE, HT_PHASOR, HT_SINE, HT_TRENDMODE, CDL2CROWS, CDL3BLACKCROWS, \
         CDL3INSIDE, CDL3LINESTRIKE, CDL3OUTSIDE, CDL3STARSINSOUTH, CDL3WHITESOLDIERS, CDLABANDONEDBABY, \
         CDLADVANCEBLOCK, CDLBELTHOLD, CDLBREAKAWAY, CDLCLOSINGMARUBOZU, CDLCONCEALBABYSWALL, CDLCOUNTERATTACK, \
         CDLDARKCLOUDCOVER, CDLDOJI, CDLDOJISTAR, CDLDRAGONFLYDOJI, CDLENGULFING, CDLEVENINGDOJISTAR, CDLEVENINGSTAR, \
         CDLGAPSIDESIDEWHITE, CDLGRAVESTONEDOJI, CDLHAMMER, CDLHANGINGMAN, CDLHARAMI, CDLHARAMICROSS, CDLHIGHWAVE, \
         CDLHIKKAKE, CDLHIKKAKEMOD, CDLHOMINGPIGEON, CDLIDENTICAL3CROWS, CDLINNECK, CDLINVERTEDHAMMER, CDLKICKING, \
         CDLKICKINGBYLENGTH, CDLLADDERBOTTOM, CDLLONGLEGGEDDOJI, CDLLONGLINE, CDLMARUBOZU, CDLMATCHINGLOW, CDLMATHOLD, \
         CDLMORNINGDOJISTAR, CDLMORNINGSTAR, CDLONNECK, CDLPIERCING, CDLRICKSHAWMAN, CDLRISEFALL3METHODS, \
         CDLSEPARATINGLINES, CDLSHOOTINGSTAR, CDLSHORTLINE, CDLSPINNINGTOP, CDLSTALLEDPATTERN, CDLSTICKSANDWICH, \
         CDLTAKURI, CDLTASUKIGAP, CDLTHRUSTING, CDLTRISTAR, CDLUNIQUE3RIVER, CDLUPSIDEGAP2CROWS, CDLXSIDEGAP3METHODS, \
         BETA, CORREL, LINEARREG, LINEARREG_ANGLE, LINEARREG_INTERCEPT, LINEARREG_SLOPE, STDDEV, TSF, VAR, ACOS, ASIN, \
-        ATAN, CEIL, COS, COSH, EXP, FLOOR, LN, LOG10, SIN, SINH, SQRT, TAN, TANH, ADD, DIV, MAX, MAXINDEX, MIN, MININDEX, \
-        MINMAX, MINMAXINDEX, MULT, SUB, SUM
+        ATAN, CEIL, COS, COSH, EXP, FLOOR, LN, LOG10, SIN, SINH, SQRT, TAN, TANH, ADD, DIV, MAX, MAXINDEX, MIN, \
+        MININDEX, \
+        MINMAX, MINMAXINDEX, MULT, SUB, SUM, EMA, TRIX, HT_TRENDLINE, KAMA, MA, MAMA, MAVP, MIDPOINT, MIDPRICE, SAR
+
+    TA_LIB_AVAILABLE = True
 except ImportError as e:
-    import warnings
     warnings.warn(f'TA-lib should be installed to use all TA functions, visit '
                   f'https://qteasy.readthedocs.io/zh/latest/faq.html to get more information',
                   ImportWarning)
+    TA_LIB_AVAILABLE = False
     pass
 
 
 # 以Technical Analysis talib为基础创建的一个金融函数库，包括talib库中已经实现的所有技术分析函数，如果TA-lib没有安装
 # 则提示用户安装
 
 # ========================
@@ -89,19 +96,40 @@
 
     close: float,收盘价
     period:
 
     Return
     ------
     """
-    try:
-        from talib import DEMA
+    if TA_LIB_AVAILABLE:
         return DEMA(close, period)
-    except ImportError:
-        return 2 * ema(close, period) - ema(ema(close, period), period)
+    else:
+        return dema_no_ta(close, period)
+
+
+def dema_no_ta(close, period: int = 30):
+    """Double Exponential Moving Average 双重指数平滑移动平均
+
+        The DEMA uses two exponential moving averages (EMAs) to eliminate lag,
+        as some traders view lag as a problem. The DEMA is used in a similar way
+        to traditional moving averages (MA). The average helps confirm up-trends
+        when the price is above the average, and helps confirm downtrends when
+        the price is below the average.
+
+        formula used for calculating DEMA is like following:
+
+        DEMA=2×EMA_N − EMA of EMA_N
+
+    close: float,收盘价
+    period:
+
+    Return
+    ------
+    """
+    return 2 * ema_no_ta(close, period) - ema_no_ta(ema_no_ta(close, period), period)
 
 
 def ema(close, span: int = 30):
     """Exponential Moving Average指数移动平均值
 
         The EMA is a type of weighted moving average (WMA) that gives
         more weighting or importance to recent price data. Like the
@@ -118,30 +146,55 @@
     close: float,收盘价 1-D ndarray, 输入数据，一维矩阵
     span: int, optional, 1 < span, 跨度
 
     Return
     ------
     1-D ndarray; 输入数据的指数平滑移动平均值
     """
-    try:
-        from talib import EMA
+    if TA_LIB_AVAILABLE:
         return EMA(close, span)
-    except ImportError:
-        alpha = 2 / (span + 1.0)
-        alpha_rev = 1 - alpha
-        n = close.shape[0]
-        pows = alpha_rev ** (np.arange(n + 1))
-        scale_arr = 1 / pows[:-1]
-        offset = close[0] * pows[1:]
-        pw0 = alpha * alpha_rev ** (n - 1)
-        mult = close * pw0 * scale_arr
-        cumsums = mult.cumsum()
-        out = offset + cumsums * scale_arr[::-1]
+    else:
+        return ema_no_ta(close, span)
+
+
+def ema_no_ta(close, span: int = 30):
+    """Exponential Moving Average指数移动平均值 不依赖ta-lib版本，计算结果与ta-lib版本接近但不完全一致
+
+        The EMA is a type of weighted moving average (WMA) that gives
+        more weighting or importance to recent price data. Like the
+        simple moving average, the exponential moving average is used
+        to see price trends over time, and watching several EMAs at
+        the same time is easy to do with moving average ribbons.
+
+        EMA is calculated with following formula:
 
-        return out
+        EMA=Price(t)×k+EMA(y)×(1−k)
+
+    Parameters
+    ----------
+    close: float,收盘价 1-D ndarray, 输入数据，一维矩阵
+    span: int, optional, 1 < span, 跨度
+
+    Return
+    ------
+    1-D ndarray; 输入数据的指数平滑移动平均值
+    """
+    alpha = 2 / (span + 1.0)
+    alpha_rev = 1 - alpha
+    n = close.shape[0]
+    pows = alpha_rev ** (np.arange(n + 1))
+    scale_arr = 1 / pows[:-1]
+    offset = close[0] * pows[1:]
+    pw0 = alpha * alpha_rev ** (n - 1)
+    mult = close * pw0 * scale_arr
+    cumsums = mult.cumsum()
+    out = offset + cumsums * scale_arr[::-1]
+    # out[:span - 1] = np.nan
+
+    return out
 
 
 def ht(close):
     """Hilbert Transform - Instantaneous Trendline 希尔伯特变换-瞬时趋势线
 
     In mathematics and in signal processing, the Hilbert transform is a
     specific linear operator that takes a function, u(t) of a real
@@ -354,24 +407,40 @@
 
     close: float,收盘价
     timeperiod:
 
     Return
     ------
     """
-    try:
-        from talib import SMA
+    if TA_LIB_AVAILABLE:
         return SMA(close, timeperiod)
-    except ImportError:
-        a = close.cumsum()
-        ar = np.roll(a, timeperiod)
-        ar[:timeperiod - 1] = np.nan
-        ar[timeperiod - 1] = 0
+    else:
+        return sma_no_ta(close, timeperiod)
+
+
+def sma_no_ta(close, timeperiod=30):
+    """Simple Moving Average 简单移动平均的不依赖ta-lib版本，计算结果与ta-lib版本一致
+
+    For a simple moving average, the formula is the sum of the data
+    points over a given period divided by the number of periods.
+
+    close: float,收盘价
+    timeperiod:
 
-        return (a - ar) / timeperiod
+    Return
+    ------
+    """
+    if len(close) < timeperiod:
+        return np.nan
+    a = close.cumsum()
+    ar = np.roll(a, timeperiod)
+    ar[:timeperiod - 1] = np.nan
+    ar[timeperiod - 1] = 0
+
+    return (a - ar) / timeperiod
 
 
 def t3(close, timeperiod=5, vfactor=0):
     """Triple Exponential Moving Average 三重指数移动平均线
 
     close: float,收盘价
     timeperiod:
@@ -822,22 +891,70 @@
 
     Return
     ------
         macd,
         macdsignal,
         macdhist
     """
-    try:
-        from talib import MACD
+    if TA_LIB_AVAILABLE:
         return MACD(close, fastperiod, slowperiod, signalperiod)
-    except ImportError:
-        macdhist = ema(close, fastperiod) - ema(close, slowperiod)
-        macdsignal = ema(macdhist, signalperiod)
-        macd = 2 * (macdhist - macdsignal)
-        return macd, macdsignal, macdhist
+    else:
+        return macd_no_ta(close, fastperiod, slowperiod, signalperiod)
+
+
+def macd_no_ta(close, fastperiod=12, slowperiod=26, signalperiod=9):
+    """Moving Average Convergence/Divergence:
+
+    The Moving Average Convergence/Divergence indicator is a momentum oscillator
+    primarily used to trade trends. Although it is an oscillator, it is not
+    typically used to identify over bought or oversold conditions. It appears on
+    the chart as two config_lines which oscillate without boundaries. The crossover of
+    the two config_lines give trading signals similar to a two moving average system.
+
+    - MACD crossing above zero is considered bullish, while crossing below zero
+    is bearish. Secondly, when MACD turns up from below zero it is considered
+    bullish. When it turns down from above zero it is considered bearish.
+
+    - When the MACD line crosses from below to above the signal line, the indicator
+    is considered bullish. The further below the zero line the stronger the signal.
+
+    - When the MACD line crosses from above to below the signal line, the indicator
+    is considered bearish. The further above the zero line the stronger the signal.
+
+    - During trading ranges the MACD will whipsaw, with the fast line crossing back
+    and forth across the signal line. Users of the MACD generally avoid trading in
+    this situation or close positions to reduce volatility within the portfolio.
+
+    - Divergence between the MACD and the price action is a stronger signal when it
+    confirms the crossover signals.
+
+    Calculation
+    An approximated MACD can be calculated by subtracting the value of a 26 period
+    Exponential Moving Average (EMA) from a 12 period EMA. The shorter EMA is
+    constantly converging toward, and diverging away from, the longer EMA. This
+    causes MACD to oscillate around the zero level. A signal line is created with
+    a 9 period EMA of the MACD line.
+
+    Parameters
+    ----------
+        close: float,收盘价
+        fastperiod:
+        slowperiod:
+        signalperiod:
+
+    Return
+    ------
+        macd,
+        macdsignal,
+        macdhist
+    """
+    macdhist = ema_no_ta(close, fastperiod) - ema_no_ta(close, slowperiod)
+    macdsignal = ema_no_ta(macdhist, signalperiod)
+    macd = 2 * (macdhist - macdsignal)
+    return macd, macdsignal, macdhist
 
 
 def macdext(close, fastperiod=12, fastmatype=0, slowperiod=26, slowmatype=0, signalperiod=9, signalmatype=0):
     """MACD with controllable MA type
 
     MACD extention: different ma types can be applied.
 
@@ -870,19 +987,15 @@
 
     Return
     ------
         macd,
         macdsignal,
         macdhist
     """
-    try:
-        from talib import MACDFIX
-        return MACDFIX(close, signalperiod)
-    except ImportError:
-        return macd(12, 26, signalperiod=signalperiod)
+    return macd(close, 12, 26, signalperiod=signalperiod)
 
 
 def mfi(high, low, close, volume, timeperiod=14):
     """Money Flow Index (货币流向指标):
 
     The Money Flow Index (MFI) is a momentum indicator that measures the
     flow of money into and out of a security over a specified period of time.
@@ -1409,21 +1522,35 @@
         收盘价
     timeperiod: int
         ema span
 
     Return
     ------
     """
-    try:
-        from talib import TRIX
+    if TA_LIB_AVAILABLE:
         return TRIX(close, timeperiod)
-    except ImportError:
-        tri_ema = ema(ema(ema(close, timeperiod), timeperiod), timeperiod)
-        res = tri_ema / np.roll(tri_ema, 1) - 1
-        return res
+    else:
+        return trix_no_ta(close, timeperiod)
+
+
+def trix_no_ta(close, timeperiod=30):
+    """1-day Rate-Of-Change (ROC) of a Triple Smooth EMA
+    TRIX 的不依赖ta-lib版本，计算结果与 ta-lib 版本近似但不完全一致
+
+    close: float, 1-d array of float
+        收盘价
+    timeperiod: int
+        ema span
+
+    Return
+    ------
+    """
+    tri_ema = ema_no_ta(ema_no_ta(ema_no_ta(close, timeperiod), timeperiod), timeperiod)
+    res = tri_ema / np.roll(tri_ema, 1) - 1
+    return res
 
 
 def ultosc(high, low, close, timeperiod1=7, timeperiod2=14, timeperiod3=28):
     """Ultimate Oscillator:
 
     The Ultimate Oscillator is a technical indicator that was developed by Larry Williams
     in 1976 to measure the price momentum of an asset across multiple timeframes. By using
@@ -1931,15 +2058,16 @@
         {Resolve the ArcTangent ambiguity}
         {Compute a differential phase, resolve phase wraparound, and limit delta phase errors}
         {Sum DeltaPhases to reach 360 degrees.  The sum is the instantaneous period.}
         {Resolve Instantaneous Period errors and smooth}
     Compute Dominant Cycle Phase
     Compute the Sine of the Dominant Cycle Phase
     Advance the Sine by 45 degrees to compute the HT Lead Sine
-    Return the Lead Sine of the Dominant Cycle Phase at the current bar of the Hilbert Transform Period measured at that bar
+    Return the Lead Sine of the Dominant Cycle Phase at the current bar of the Hilbert Transform Period measured at
+    that bar
 
     close: float,收盘价
 
     Return
     ------
     """
     return HT_DCPHASE(close)
@@ -2978,15 +3106,16 @@
     """
     return CDLHOMINGPIGEON(opn, high, low, close)
 
 
 def cdlidentical3crows(opn, high, low, close):
     """Identical Three Crows:
 
-    The Identical Three Crows is a three-line bearish reversal candlestick pattern. Every candle appears as a long line having a black body.
+    The Identical Three Crows is a three-line bearish reversal candlestick pattern. Every candle appears as a long
+    line having a black body.
 
     Forecast: bearish reversal
     Trend prior to the pattern: uptrend
     Opposite pattern: none
     See Also: Three Black Crows
 
     Construction:
@@ -3276,15 +3405,17 @@
     """
     return CDLMATHOLD(opn, high, low, close)
 
 
 def cdlmorningdojistar(opn, high, low, close):
     """Morning Doji Star:
 
-    The Morning Doji Star is a bullish reversal pattern, being very similar to the Morning Star. The only difference is that the Morning Doji Star needs to have a doji candle (except the Four-Price Doji) on the second line. The doji candle (second line) should not be preceded by or followed by a price gap.
+    The Morning Doji Star is a bullish reversal pattern, being very similar to the Morning Star. The only difference
+    is that the Morning Doji Star needs to have a doji candle (except the Four-Price Doji) on the second line. The
+    doji candle (second line) should not be preceded by or followed by a price gap.
 
     Forecast: bullish reversal
     Trend prior to the pattern: downtrend
     Opposite pattern: Evening Doji Star
 
     Construction:
```

### Comparing `qteasy-1.2.1/qteasy/trade_recording.py` & `qteasy-1.2.2/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/trader.py` & `qteasy-1.2.2/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/trader_cli.py` & `qteasy-1.2.2/qteasy/trader_cli.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/trader_tui.py` & `qteasy-1.2.2/qteasy/trader_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/trading_util.py` & `qteasy-1.2.2/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/tsfuncs.py` & `qteasy-1.2.2/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/tui_style.tcss` & `qteasy-1.2.2/qteasy/tui_style.tcss`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/utilfuncs.py` & `qteasy-1.2.2/qteasy/utilfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy/visual.py` & `qteasy-1.2.2/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/qteasy.egg-info/PKG-INFO` & `qteasy-1.2.2/qteasy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.1
+Version: 1.2.2
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -39,18 +39,32 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas>=1.1.0
+Requires-Dist: numpy>=1.18.1
+Requires-Dist: numba>=0.47.0
+Requires-Dist: tushare>=1.2.89
+Requires-Dist: mplfinance
+Requires-Dist: rich>=10.0.0
+Requires-Dist: textual
 Provides-Extra: talib
+Requires-Dist: ta-lib; extra == "talib"
 Provides-Extra: database
+Requires-Dist: pymysql>=1.0.0; extra == "database"
 Provides-Extra: feather
-License-File: LICENSE
+Requires-Dist: pyarrow>=3; extra == "feather"
+Provides-Extra: dev
+Requires-Dist: ta-lib; extra == "dev"
+Requires-Dist: pymysql>=1.0.0; extra == "dev"
+Requires-Dist: pyarrow>=3; extra == "dev"
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
@@ -92,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.1`
+- Latest Version: `1.2.2`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -568,14 +582,15 @@
         mode=0,  # 交易模式为实盘运行
         asset_type='E',  # 交易的标的类型为股票
         asset_pool=asset_pool,  # 交易股票池为所有银行股和家用电器股
         trade_batch_size=100,  # 交易批量为100股的整数倍
         sell_batch_size=1,  # 卖出数量为1股的整数倍
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
+        live_trade_ui_type='tui',  # 使用TUI界面监控实盘交易，默认使用CLI界面
 )
 
 qt.run(op)
 ```
 qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
 为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
```

### Comparing `qteasy-1.2.1/qteasy.egg-info/SOURCES.txt` & `qteasy-1.2.2/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/setup.cfg` & `qteasy-1.2.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.2.1
+version = 1.2.2
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
@@ -34,26 +34,30 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = qteasy
 python_requires = >=3.6
 install_requires = 
-	pandas>=1.4.0
+	pandas>=1.1.0
 	numpy>=1.18.1
 	numba>=0.47.0
 	tushare>=1.2.89
 	mplfinance
 	rich>=10.0.0
 	textual
 
 [options.extras_require]
 talib = ta-lib
 database = pymysql >= 1.0.0
 feather = pyarrow >= 3
+dev = 
+	ta-lib
+	pymysql >= 1.0.0
+	pyarrow >= 3
 
 [options.packages.find]
 where = qteasy
 
 [options.package_data]
 qteasy = *.tcss
```

### Comparing `qteasy-1.2.1/tests/test_broker.py` & `qteasy-1.2.2/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_cashplan.py` & `qteasy-1.2.2/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_config.py` & `qteasy-1.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_core_sub_funcs.py` & `qteasy-1.2.2/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_cost.py` & `qteasy-1.2.2/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_datasource.py` & `qteasy-1.2.2/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_eastmoney.py` & `qteasy-1.2.2/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_evaluations.py` & `qteasy-1.2.2/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_fast_experiments.py` & `qteasy-1.2.2/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_historypanel.py` & `qteasy-1.2.2/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_loop.py` & `qteasy-1.2.2/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_operator_and_strategy.py` & `qteasy-1.2.2/tests/test_operator_and_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -2279,24 +2279,24 @@
                            [1.049, 0.972, 0.741]])
 
         hit = np.allclose(res, target)
         self.assertTrue(hit)
 
         # test human_blender function:
         print('\ntest human_blender function')
-        strategy_ids = ['MACD', 'DMA', 'Crossline', 'TRIX', 'KDJ']
+        strategy_ids = ['MACD', 'DMA', 'CROSSLINE', 'TRIX', 'KDJ']
         blender_exp = 'avgpos_3_0.5(s0, s1, s2, s3, s4)'
         res = human_blender(blender_exp, strategy_ids)
         print(f'blended signals with blender "{blender_exp}" is \n{res}')
-        self.assertEqual(res, 'avgpos_3_0.5(MACD, DMA, Crossline, TRIX, KDJ)')
+        self.assertEqual(res, 'avgpos_3_0.5(MACD, DMA, CROSSLINE, TRIX, KDJ)')
 
         blender_exp = 'max(s0, s1, s2)+s3*s4'
         res = human_blender(blender_exp, strategy_ids)
         print(f'blended signals with blender "{blender_exp}" is \n{res}')
-        self.assertEqual(res, 'max(MACD, DMA, Crossline) + TRIX * KDJ')
+        self.assertEqual(res, 'max(MACD, DMA, CROSSLINE) + TRIX * KDJ')
 
         blender_exp = 'max(s0, s1/s0)+s1and0.5*s4'
         res = human_blender(blender_exp, strategy_ids)
         print(f'blended signals with blender "{blender_exp}" is \n{res}')
         self.assertEqual(res, 'max(MACD, DMA / MACD) + DMA and 0.5 * KDJ')
 
         blender_exp = 'max(s0, s1/s0)+s1^0.5*s6'
@@ -2357,15 +2357,15 @@
         self.assertEqual(op.strategies[1].pars, (0.5,))
         self.assertEqual(op.strategies[2].pars, (8, 26, 9))
 
         # Test Errors
         # op.set_opt_par主要在优化过程中自动生成，已经保证了参数的正确性，因此不再检查参数正确性
 
     def test_stg_attribute_get_and_set(self):
-        self.stg = qt.built_in.Crossline()
+        self.stg = qt.built_in.CROSSLINE()
         self.stg_type = 'RULE-ITER'
         self.stg_name = "CROSSLINE"
         self.stg_text = 'Moving average crossline strategy, determine long/short position according to the cross ' \
                         'point' \
                         ' of long and short term moving average prices '
         self.pars = (35, 120, 0.02)
         self.par_boes = [(10, 250), (10, 250), (0, 0.1)]
```

### Comparing `qteasy-1.2.1/tests/test_qt.py` & `qteasy-1.2.2/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_space.py` & `qteasy-1.2.2/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_ta_funcs.py` & `qteasy-1.2.2/tests/test_ta_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 # Desc:
 #   Unittest for all TA-Lib wrapper
 #   functions.
 # ======================================
 import unittest
 import numpy as np
 
-from qteasy.tafuncs import bbands, dema, ema, ht, kama, ma, mama, mavp, mid_point
-from qteasy.tafuncs import mid_price, sar, sarext, sma, t3, tema, trima, wma, adx, adxr
+from qteasy.tafuncs import bbands, dema, ema, ht, kama, ma, mama, mavp, mid_point, sma_no_ta, ema_no_ta
+from qteasy.tafuncs import mid_price, sar, sarext, sma, t3, tema, trima, wma, adx, adxr, trix_no_ta
 from qteasy.tafuncs import apo, bop, cci, cmo, dx, macd, macdext, aroon, aroonosc
 from qteasy.tafuncs import macdfix, mfi, minus_di, minus_dm, mom, plus_di, plus_dm
 from qteasy.tafuncs import ppo, roc, rocp, rocr, rocr100, rsi, stoch, stochf, stochrsi
 from qteasy.tafuncs import trix, ultosc, willr, ad, adosc, obv, atr, natr, trange
 from qteasy.tafuncs import avgprice, medprice, typprice, wclprice, ht_dcperiod
 from qteasy.tafuncs import ht_dcphase, ht_phasor, ht_sine, ht_trendmode, cdl2crows
 from qteasy.tafuncs import cdl3blackcrows, cdl3inside, cdl3linestrike, cdl3outside
@@ -89,14 +89,22 @@
 
     def test_ema(self):
         print(f'test TA function: ema\n'
               f'======================')
         res = ema(self.close, span=5)
         print(f'result is\n{res}')
 
+    def test_ema_and_ema_no_ta(self):
+        """ 测试ema和ema_no_ta的结果是否一致 """
+        res = ema(self.close, span=5)
+        res_no_ta = ema_no_ta(self.close, span=5)
+        print(f'result is\n{res}\n'
+              f'result_no_ta is\n{res_no_ta}')
+        self.assertTrue(np.allclose(res, res_no_ta, equal_nan=True, atol=0.02))
+
     def test_ht(self):
         print(f'test TA function: ht\n'
               f'======================')
         res = ht(self.close)
         print(f'result is\n{res}')
 
     def test_kama(self):
@@ -150,14 +158,22 @@
 
     def test_sma(self):
         print(f'test TA function: sma\n'
               f'======================')
         res = sma(self.close)
         print(f'result is \n{res}')
 
+    def test_sma_and_sma_no_ta(self):
+        """ 测试sma和sma_no_ta的结果是否一致 """
+        res = sma(self.close)
+        res_no_ta = sma_no_ta(self.close)
+        print(f'result is \n{res}'
+              f'result_no_ta is \n{res_no_ta}')
+        self.assertTrue(np.allclose(res, res_no_ta, equal_nan=True))
+
     def test_t3(self):
         print(f'test TA function: t3\n'
               f'=====================')
         res = t3(self.close)
         print(f'result is \n{res}')
 
     def test_tema(self):
@@ -342,14 +358,22 @@
 
     def test_trix(self):
         print(f'test TA function: trix\n'
               f'=======================')
         res = trix(self.close, timeperiod=5)
         print(f'result is \n{res}')
 
+    def test_trix_vs_trix_no_ta(self):
+        """ 测试trix和trix_no_ta的结果是否一致 """
+        res = trix(self.close, timeperiod=5)
+        res_no_ta = trix_no_ta(self.close, timeperiod=5)
+        print(f'result is \n{res}\n'
+              f'result_no_ta is \n{res_no_ta}')
+        self.assertTrue(np.allclose(res, res_no_ta, equal_nan=True, atol=0.02))
+
     def test_ultosc(self):
         print(f'test TA function: ultosc\n'
               f'=========================')
         res = ultosc(self.high, self.low, self.close)
         print(f'result is \n{res}')
 
     def test_willr(self):
```

### Comparing `qteasy-1.2.1/tests/test_trader.py` & `qteasy-1.2.2/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_trader_shell.py` & `qteasy-1.2.2/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_trading.py` & `qteasy-1.2.2/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_tui.py` & `qteasy-1.2.2/tests/test_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_tushare.py` & `qteasy-1.2.2/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_utilityfuncs.py` & `qteasy-1.2.2/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.1/tests/test_visual.py` & `qteasy-1.2.2/tests/test_visual.py`

 * *Files identical despite different names*

