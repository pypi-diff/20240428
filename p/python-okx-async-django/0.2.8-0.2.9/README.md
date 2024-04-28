# Comparing `tmp/python-okx-async-django-0.2.8.tar.gz` & `tmp/python-okx-async-django-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-okx-async-django-0.2.8.tar", last modified: Thu Apr 25 13:44:57 2024, max compression
+gzip compressed data, was "python-okx-async-django-0.2.9.tar", last modified: Sat Apr 27 10:04:55 2024, max compression
```

## Comparing `python-okx-async-django-0.2.8.tar` & `python-okx-async-django-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-25 13:44:57.151762 python-okx-async-django-0.2.8/
--rw-r--r--   0 chiang     (501) staff       (20)     3031 2024-04-25 13:44:57.151260 python-okx-async-django-0.2.8/PKG-INFO
--rw-r--r--   0 chiang     (501) staff       (20)     2618 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/README.md
-drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-25 13:44:57.127359 python-okx-async-django-0.2.8/okx/
--rw-r--r--   0 chiang     (501) staff       (20)    11585 2024-04-25 09:08:44.000000 python-okx-async-django-0.2.8/okx/Account.py
--rw-r--r--   0 chiang     (501) staff       (20)     5217 2024-04-25 09:08:47.000000 python-okx-async-django-0.2.8/okx/BlockTrading.py
--rw-r--r--   0 chiang     (501) staff       (20)     1635 2024-04-25 09:06:39.000000 python-okx-async-django-0.2.8/okx/Convert.py
--rw-r--r--   0 chiang     (501) staff       (20)     2945 2024-04-25 09:07:17.000000 python-okx-async-django-0.2.8/okx/CopyTrading.py
--rw-r--r--   0 chiang     (501) staff       (20)     3873 2024-04-25 09:08:34.000000 python-okx-async-django-0.2.8/okx/Earning.py
--rw-r--r--   0 chiang     (501) staff       (20)      998 2024-04-25 09:09:34.000000 python-okx-async-django-0.2.8/okx/FDBroker.py
--rw-r--r--   0 chiang     (501) staff       (20)     6366 2024-04-25 01:53:19.000000 python-okx-async-django-0.2.8/okx/Funding.py
--rw-r--r--   0 chiang     (501) staff       (20)     6919 2024-04-25 01:52:06.000000 python-okx-async-django-0.2.8/okx/Grid.py
--rw-r--r--   0 chiang     (501) staff       (20)     5649 2024-04-25 01:50:34.000000 python-okx-async-django-0.2.8/okx/MarketData.py
--rw-r--r--   0 chiang     (501) staff       (20)     5302 2024-04-25 01:49:39.000000 python-okx-async-django-0.2.8/okx/NDBroker.py
--rw-r--r--   0 chiang     (501) staff       (20)     5879 2024-04-25 01:51:51.000000 python-okx-async-django-0.2.8/okx/PublicData.py
--rw-r--r--   0 chiang     (501) staff       (20)     4138 2024-04-25 01:43:27.000000 python-okx-async-django-0.2.8/okx/SpreadTrading.py
--rw-r--r--   0 chiang     (501) staff       (20)      702 2024-04-25 01:44:10.000000 python-okx-async-django-0.2.8/okx/Status.py
--rw-r--r--   0 chiang     (501) staff       (20)     4121 2024-04-25 01:45:22.000000 python-okx-async-django-0.2.8/okx/SubAccount.py
--rw-r--r--   0 chiang     (501) staff       (20)    13353 2024-04-25 01:47:03.000000 python-okx-async-django-0.2.8/okx/Trade.py
--rw-r--r--   0 chiang     (501) staff       (20)     2709 2024-04-25 01:48:08.000000 python-okx-async-django-0.2.8/okx/TradingData.py
--rw-r--r--   0 chiang     (501) staff       (20)       58 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/okx/__init__.py
--rw-r--r--   0 chiang     (501) staff       (20)    14331 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/okx/consts.py
--rw-r--r--   0 chiang     (501) staff       (20)     1212 2024-04-25 09:08:39.000000 python-okx-async-django-0.2.8/okx/exceptions.py
--rw-r--r--   0 chiang     (501) staff       (20)     2360 2024-04-24 15:18:15.000000 python-okx-async-django-0.2.8/okx/okxclient.py
--rw-r--r--   0 chiang     (501) staff       (20)     1826 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/okx/utils.py
-drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-25 13:44:57.130530 python-okx-async-django-0.2.8/okx/websocket/
--rw-r--r--   0 chiang     (501) staff       (20)      850 2024-04-25 11:04:09.000000 python-okx-async-django-0.2.8/okx/websocket/WebSocketFactory.py
--rw-r--r--   0 chiang     (501) staff       (20)     2154 2024-04-25 11:10:17.000000 python-okx-async-django-0.2.8/okx/websocket/WsPrivateAsync.py
--rw-r--r--   0 chiang     (501) staff       (20)     1439 2024-04-25 11:09:42.000000 python-okx-async-django-0.2.8/okx/websocket/WsPublicAsync.py
--rw-r--r--   0 chiang     (501) staff       (20)     2377 2024-04-25 10:52:16.000000 python-okx-async-django-0.2.8/okx/websocket/WsUtils.py
--rw-r--r--   0 chiang     (501) staff       (20)        0 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/okx/websocket/__init__.py
-drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-25 13:44:57.134958 python-okx-async-django-0.2.8/python_okx_async_django.egg-info/
--rw-r--r--   0 chiang     (501) staff       (20)     3031 2024-04-25 13:44:57.000000 python-okx-async-django-0.2.8/python_okx_async_django.egg-info/PKG-INFO
--rw-r--r--   0 chiang     (501) staff       (20)     1124 2024-04-25 13:44:57.000000 python-okx-async-django-0.2.8/python_okx_async_django.egg-info/SOURCES.txt
--rw-r--r--   0 chiang     (501) staff       (20)        1 2024-04-25 13:44:57.000000 python-okx-async-django-0.2.8/python_okx_async_django.egg-info/dependency_links.txt
--rw-r--r--   0 chiang     (501) staff       (20)       91 2024-04-25 13:44:57.000000 python-okx-async-django-0.2.8/python_okx_async_django.egg-info/requires.txt
--rw-r--r--   0 chiang     (501) staff       (20)        9 2024-04-25 13:44:57.000000 python-okx-async-django-0.2.8/python_okx_async_django.egg-info/top_level.txt
--rw-r--r--   0 chiang     (501) staff       (20)       38 2024-04-25 13:44:57.152454 python-okx-async-django-0.2.8/setup.cfg
--rw-r--r--   0 chiang     (501) staff       (20)      854 2024-04-25 13:44:44.000000 python-okx-async-django-0.2.8/setup.py
-drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-25 13:44:57.148531 python-okx-async-django-0.2.8/test/
--rw-r--r--   0 chiang     (501) staff       (20)     5577 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/AccountTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     2886 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/BlockTradingTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     2862 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/BrokerTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     1171 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/ConvertTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     1608 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/CopyTradingTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     1624 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/EarningTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     3571 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/FundingTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     3772 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/GridTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     2732 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/MarketTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     3517 2024-04-24 15:29:09.000000 python-okx-async-django-0.2.8/test/PublicDataTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     1815 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/SpreadTest.py
--rw-r--r--   0 chiang     (501) staff       (20)      988 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/StackingTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     2461 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/SubAccountTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     9864 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/TradeTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     1589 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/TradingDataTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     1203 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.8/test/WsPrivateAsyncTest.py
--rw-r--r--   0 chiang     (501) staff       (20)     2360 2024-04-25 11:10:27.000000 python-okx-async-django-0.2.8/test/WsPublicAsyncTest.py
--rw-r--r--   0 chiang     (501) staff       (20)        0 2024-04-24 15:06:17.000000 python-okx-async-django-0.2.8/test/__init__.py
+drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-27 10:04:55.253869 python-okx-async-django-0.2.9/
+-rw-r--r--   0 chiang     (501) staff       (20)     3031 2024-04-27 10:04:55.253241 python-okx-async-django-0.2.9/PKG-INFO
+-rw-r--r--   0 chiang     (501) staff       (20)     2618 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/README.md
+drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-27 10:04:55.226073 python-okx-async-django-0.2.9/okx/
+-rw-r--r--   0 chiang     (501) staff       (20)    11585 2024-04-25 09:08:44.000000 python-okx-async-django-0.2.9/okx/Account.py
+-rw-r--r--   0 chiang     (501) staff       (20)     5217 2024-04-25 09:08:47.000000 python-okx-async-django-0.2.9/okx/BlockTrading.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1635 2024-04-25 09:06:39.000000 python-okx-async-django-0.2.9/okx/Convert.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2945 2024-04-25 09:07:17.000000 python-okx-async-django-0.2.9/okx/CopyTrading.py
+-rw-r--r--   0 chiang     (501) staff       (20)     3873 2024-04-25 09:08:34.000000 python-okx-async-django-0.2.9/okx/Earning.py
+-rw-r--r--   0 chiang     (501) staff       (20)      998 2024-04-25 09:09:34.000000 python-okx-async-django-0.2.9/okx/FDBroker.py
+-rw-r--r--   0 chiang     (501) staff       (20)     6366 2024-04-25 01:53:19.000000 python-okx-async-django-0.2.9/okx/Funding.py
+-rw-r--r--   0 chiang     (501) staff       (20)     6919 2024-04-25 01:52:06.000000 python-okx-async-django-0.2.9/okx/Grid.py
+-rw-r--r--   0 chiang     (501) staff       (20)     5649 2024-04-25 01:50:34.000000 python-okx-async-django-0.2.9/okx/MarketData.py
+-rw-r--r--   0 chiang     (501) staff       (20)     5302 2024-04-25 01:49:39.000000 python-okx-async-django-0.2.9/okx/NDBroker.py
+-rw-r--r--   0 chiang     (501) staff       (20)     5879 2024-04-25 01:51:51.000000 python-okx-async-django-0.2.9/okx/PublicData.py
+-rw-r--r--   0 chiang     (501) staff       (20)     4138 2024-04-25 01:43:27.000000 python-okx-async-django-0.2.9/okx/SpreadTrading.py
+-rw-r--r--   0 chiang     (501) staff       (20)      702 2024-04-25 01:44:10.000000 python-okx-async-django-0.2.9/okx/Status.py
+-rw-r--r--   0 chiang     (501) staff       (20)     4121 2024-04-25 01:45:22.000000 python-okx-async-django-0.2.9/okx/SubAccount.py
+-rw-r--r--   0 chiang     (501) staff       (20)    13353 2024-04-25 01:47:03.000000 python-okx-async-django-0.2.9/okx/Trade.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2709 2024-04-25 01:48:08.000000 python-okx-async-django-0.2.9/okx/TradingData.py
+-rw-r--r--   0 chiang     (501) staff       (20)       58 2024-04-27 10:03:49.000000 python-okx-async-django-0.2.9/okx/__init__.py
+-rw-r--r--   0 chiang     (501) staff       (20)    14331 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/okx/consts.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1212 2024-04-25 09:08:39.000000 python-okx-async-django-0.2.9/okx/exceptions.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2360 2024-04-24 15:18:15.000000 python-okx-async-django-0.2.9/okx/okxclient.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2014 2024-04-27 09:14:22.000000 python-okx-async-django-0.2.9/okx/utils.py
+drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-27 10:04:55.229968 python-okx-async-django-0.2.9/okx/websocket/
+-rw-r--r--   0 chiang     (501) staff       (20)      850 2024-04-25 11:04:09.000000 python-okx-async-django-0.2.9/okx/websocket/WebSocketFactory.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2048 2024-04-27 09:28:10.000000 python-okx-async-django-0.2.9/okx/websocket/WsPrivateAsync.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1446 2024-04-27 09:28:34.000000 python-okx-async-django-0.2.9/okx/websocket/WsPublicAsync.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2377 2024-04-25 10:52:16.000000 python-okx-async-django-0.2.9/okx/websocket/WsUtils.py
+-rw-r--r--   0 chiang     (501) staff       (20)        0 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/okx/websocket/__init__.py
+drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-27 10:04:55.233962 python-okx-async-django-0.2.9/python_okx_async_django.egg-info/
+-rw-r--r--   0 chiang     (501) staff       (20)     3031 2024-04-27 10:04:55.000000 python-okx-async-django-0.2.9/python_okx_async_django.egg-info/PKG-INFO
+-rw-r--r--   0 chiang     (501) staff       (20)     1124 2024-04-27 10:04:55.000000 python-okx-async-django-0.2.9/python_okx_async_django.egg-info/SOURCES.txt
+-rw-r--r--   0 chiang     (501) staff       (20)        1 2024-04-27 10:04:55.000000 python-okx-async-django-0.2.9/python_okx_async_django.egg-info/dependency_links.txt
+-rw-r--r--   0 chiang     (501) staff       (20)       91 2024-04-27 10:04:55.000000 python-okx-async-django-0.2.9/python_okx_async_django.egg-info/requires.txt
+-rw-r--r--   0 chiang     (501) staff       (20)        9 2024-04-27 10:04:55.000000 python-okx-async-django-0.2.9/python_okx_async_django.egg-info/top_level.txt
+-rw-r--r--   0 chiang     (501) staff       (20)       38 2024-04-27 10:04:55.254039 python-okx-async-django-0.2.9/setup.cfg
+-rw-r--r--   0 chiang     (501) staff       (20)      854 2024-04-27 10:03:52.000000 python-okx-async-django-0.2.9/setup.py
+drwxr-xr-x   0 chiang     (501) staff       (20)        0 2024-04-27 10:04:55.252354 python-okx-async-django-0.2.9/test/
+-rw-r--r--   0 chiang     (501) staff       (20)     5577 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/AccountTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2886 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/BlockTradingTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2862 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/BrokerTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1171 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/ConvertTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1608 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/CopyTradingTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1624 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/EarningTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     3571 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/FundingTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     3772 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/GridTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2732 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/MarketTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     3517 2024-04-24 15:29:09.000000 python-okx-async-django-0.2.9/test/PublicDataTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1815 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/SpreadTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)      988 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/StackingTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2461 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/SubAccountTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     9864 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/TradeTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1589 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/TradingDataTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     1203 2024-04-24 14:17:12.000000 python-okx-async-django-0.2.9/test/WsPrivateAsyncTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)     2360 2024-04-25 11:10:27.000000 python-okx-async-django-0.2.9/test/WsPublicAsyncTest.py
+-rw-r--r--   0 chiang     (501) staff       (20)        0 2024-04-24 15:06:17.000000 python-okx-async-django-0.2.9/test/__init__.py
```

### Comparing `python-okx-async-django-0.2.8/PKG-INFO` & `python-okx-async-django-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx-async-django
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python SDK for OKX async
 Home-page: https://okx.com/docs-v5/
 Author: djangocc
 Author-email: djangonomo@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-okx-async-django-0.2.8/README.md` & `python-okx-async-django-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Account.py` & `python-okx-async-django-0.2.9/okx/Account.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/BlockTrading.py` & `python-okx-async-django-0.2.9/okx/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Convert.py` & `python-okx-async-django-0.2.9/okx/Convert.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/CopyTrading.py` & `python-okx-async-django-0.2.9/okx/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Earning.py` & `python-okx-async-django-0.2.9/okx/Earning.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/FDBroker.py` & `python-okx-async-django-0.2.9/okx/FDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Funding.py` & `python-okx-async-django-0.2.9/okx/Funding.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Grid.py` & `python-okx-async-django-0.2.9/okx/Grid.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/MarketData.py` & `python-okx-async-django-0.2.9/okx/MarketData.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/NDBroker.py` & `python-okx-async-django-0.2.9/okx/NDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/PublicData.py` & `python-okx-async-django-0.2.9/okx/PublicData.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/SpreadTrading.py` & `python-okx-async-django-0.2.9/okx/SpreadTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Status.py` & `python-okx-async-django-0.2.9/okx/Status.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/SubAccount.py` & `python-okx-async-django-0.2.9/okx/SubAccount.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/Trade.py` & `python-okx-async-django-0.2.9/okx/Trade.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/TradingData.py` & `python-okx-async-django-0.2.9/okx/TradingData.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/consts.py` & `python-okx-async-django-0.2.9/okx/consts.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/exceptions.py` & `python-okx-async-django-0.2.9/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/okxclient.py` & `python-okx-async-django-0.2.9/okx/okxclient.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/utils.py` & `python-okx-async-django-0.2.9/okx/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import hmac
 import base64
 import datetime
 from . import consts as c
 
 
 def sign(message, secretKey):
@@ -57,7 +58,14 @@
         body = ''
     message = str(timestamp) + str.upper(method) + request_path + str(body)
 
     mac = hmac.new(bytes(secret_key, encoding='utf8'), bytes(message, encoding='utf-8'), digestmod='sha256')
     d = mac.digest()
 
     return base64.b64encode(d)
+
+background_tasks = set()
+
+def run_async_task(coro):
+    task = asyncio.create_task(coro)
+    background_tasks.add(task)
+    task.add_done_callback(background_tasks.discard)
```

### Comparing `python-okx-async-django-0.2.8/okx/websocket/WebSocketFactory.py` & `python-okx-async-django-0.2.9/okx/websocket/WebSocketFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/okx/websocket/WsPrivateAsync.py` & `python-okx-async-django-0.2.9/okx/websocket/WsPrivateAsync.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 import logging
 
+from okx.utils import run_async_task
 from okx.websocket import WsUtils
 from okx.websocket.WebSocketFactory import WebSocketFactory
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("WsPrivate")
 
 
@@ -21,15 +22,14 @@
         self.useServerTime = useServerTime
 
     async def connect(self):
         self.websocket = await self.factory.connect()
 
     async def consume(self):
         async for message in self.websocket:
-            logger.info("Received message: {%s}", message)
             if self.callback:
                 self.callback(message)
 
     async def subscribe(self, params: list, callback):
         self.callback = callback
 
         logRes = await self.login()
@@ -50,20 +50,18 @@
         return True
 
     async def unsubscribe(self, params: list, callback):
         self.callback = callback
         payload = json.dumps({"op": "unsubscribe", "args": params})
         logger.info(f"unsubscribe: {payload}")
         await self.websocket.send(payload)
-        # for param in params:
-        #     self.subscriptions.discard(param)
 
     async def stop(self):
         await self.factory.close()
 
     async def start(self):
         logger.info("Connecting to WebSocket...")
         await self.connect()
-        asyncio.create_task(self.consume())
+        run_async_task(self.consume())
 
     def stop_sync(self):
         asyncio.get_running_loop().run_until_complete(self.stop())
```

### Comparing `python-okx-async-django-0.2.8/okx/websocket/WsPublicAsync.py` & `python-okx-async-django-0.2.9/okx/websocket/WsPublicAsync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 import logging
 
+from okx.utils import run_async_task
 from okx.websocket.WebSocketFactory import WebSocketFactory
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("WsPublic")
 
 
 class WsPublicAsync:
@@ -16,34 +17,36 @@
         self.factory = WebSocketFactory(url)
 
     async def connect(self):
         self.websocket = await self.factory.connect()
 
     async def consume(self):
         async for message in self.websocket:
-            logger.info("Received message: {%s}", message)
             if self.callback:
                 self.callback(message)
 
     async def subscribe(self, params: list, callback):
         self.callback = callback
         payload = json.dumps({"op": "subscribe", "args": params})
         await self.websocket.send(payload)
         # await self.consume()
 
     async def unsubscribe(self, params: list, callback):
         self.callback = callback
-        payload = json.dumps({"op": "unsubscribe", "args": params})
+        payload = json.dumps({
+            "op": "unsubscribe",
+            "args": params
+        })
         logger.info(f"unsubscribe: {payload}")
         await self.websocket.send(payload)
 
     async def stop(self):
         await self.factory.close()
 
     async def start(self):
         logger.info("Connecting to WebSocket...")
         await self.connect()
-        asyncio.create_task(self.consume())
+        run_async_task(self.consume())
 
     def stop_sync(self):
         asyncio.get_running_loop().run_until_complete(self.stop())
```

### Comparing `python-okx-async-django-0.2.8/okx/websocket/WsUtils.py` & `python-okx-async-django-0.2.9/okx/websocket/WsUtils.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/python_okx_async_django.egg-info/PKG-INFO` & `python-okx-async-django-0.2.9/python_okx_async_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx-async-django
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python SDK for OKX async
 Home-page: https://okx.com/docs-v5/
 Author: djangocc
 Author-email: djangonomo@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-okx-async-django-0.2.8/python_okx_async_django.egg-info/SOURCES.txt` & `python-okx-async-django-0.2.9/python_okx_async_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/setup.py` & `python-okx-async-django-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/AccountTest.py` & `python-okx-async-django-0.2.9/test/AccountTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/BlockTradingTest.py` & `python-okx-async-django-0.2.9/test/BlockTradingTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/BrokerTest.py` & `python-okx-async-django-0.2.9/test/BrokerTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/ConvertTest.py` & `python-okx-async-django-0.2.9/test/ConvertTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/CopyTradingTest.py` & `python-okx-async-django-0.2.9/test/CopyTradingTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/EarningTest.py` & `python-okx-async-django-0.2.9/test/EarningTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/FundingTest.py` & `python-okx-async-django-0.2.9/test/FundingTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/GridTest.py` & `python-okx-async-django-0.2.9/test/GridTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/MarketTest.py` & `python-okx-async-django-0.2.9/test/MarketTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/PublicDataTest.py` & `python-okx-async-django-0.2.9/test/PublicDataTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/SpreadTest.py` & `python-okx-async-django-0.2.9/test/SpreadTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/StackingTest.py` & `python-okx-async-django-0.2.9/test/StackingTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/SubAccountTest.py` & `python-okx-async-django-0.2.9/test/SubAccountTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/TradeTest.py` & `python-okx-async-django-0.2.9/test/TradeTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/TradingDataTest.py` & `python-okx-async-django-0.2.9/test/TradingDataTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/WsPrivateAsyncTest.py` & `python-okx-async-django-0.2.9/test/WsPrivateAsyncTest.py`

 * *Files identical despite different names*

### Comparing `python-okx-async-django-0.2.8/test/WsPublicAsyncTest.py` & `python-okx-async-django-0.2.9/test/WsPublicAsyncTest.py`

 * *Files identical despite different names*

