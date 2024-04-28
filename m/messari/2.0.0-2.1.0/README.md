# Comparing `tmp/messari-2.0.0.tar.gz` & `tmp/messari-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messari-2.0.0.tar", last modified: Fri Apr 12 13:21:47 2024, max compression
+gzip compressed data, was "messari-2.1.0.tar", last modified: Sun Apr 28 12:58:01 2024, max compression
```

## Comparing `messari-2.0.0.tar` & `messari-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.437520 messari-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 13:21:38.000000 messari-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 13:21:47.437520 messari-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 13:21:38.000000 messari-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.433520 messari-2.0.0/messari/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 13:21:38.000000 messari-2.0.0/messari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 13:21:38.000000 messari-2.0.0/messari/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-12 13:21:38.000000 messari-2.0.0/messari/messari.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.437520 messari-2.0.0/messari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:21:47.437520 messari-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-12 13:21:38.000000 messari-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.437520 messari-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-12 13:21:38.000000 messari-2.0.0/tests/test_messari.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:58:01.035304 messari-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 12:57:52.000000 messari-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-28 12:58:01.035304 messari-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-28 12:57:52.000000 messari-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:58:01.031304 messari-2.1.0/messari/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-28 12:57:52.000000 messari-2.1.0/messari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-28 12:57:52.000000 messari-2.1.0/messari/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-28 12:57:52.000000 messari-2.1.0/messari/messari.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:58:01.035304 messari-2.1.0/messari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-28 12:58:00.000000 messari-2.1.0/messari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-28 12:58:01.000000 messari-2.1.0/messari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:58:00.000000 messari-2.1.0/messari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 12:58:00.000000 messari-2.1.0/messari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 12:58:00.000000 messari-2.1.0/messari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:58:01.035304 messari-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-28 12:57:52.000000 messari-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:58:01.035304 messari-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-28 12:57:52.000000 messari-2.1.0/tests/test_messari.py
```

### Comparing `messari-2.0.0/LICENSE` & `messari-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `messari-2.0.0/PKG-INFO` & `messari-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messari
-Version: 2.0.0
+Version: 2.1.0
 Summary: Unofficial Messari API client.
 Home-page: https://github.com/itzmestar/Messari
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -48,17 +48,34 @@
 ```
 from messari import Messari
 
 # initialize api client
 
 messari = Messari(key='xxxxxxxxxxxxxxx')
 
-# Get the paginated list of all assets and their metrics and profiles.
+# Get a list of all assets and their market caps, sorted by market cap descending.
 response = messari.get_all_assets()
 
+# Get the ID, name, symbol, slug, market cap, sector, category, and tags for a single asset.
+response = messari.get_asset_by_id(asset_id=asset_id)
+
+# Get market data for a specific asset.
+response = messari.get_market_data_by_asset(asset_id=asset_id)
+
+# Get a list ROI data for all assets.
+response = messari.get_roi()
+
+# Get a single assets ROI data.
+response = messari.get_roi_by_asset(asset_id=asset_id)
+
+# Get a list of market specific data for all markets.
+response = messari.get_markets()
+
+# Get a list of exchanges with market data.
+response = messari.get_exchanges()
 ```
 
 -------
 #### Donate & Help maintain the library
 
 [![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
```

### Comparing `messari-2.0.0/README.md` & `messari-2.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -30,17 +30,34 @@
 ```
 from messari import Messari
 
 # initialize api client
 
 messari = Messari(key='xxxxxxxxxxxxxxx')
 
-# Get the paginated list of all assets and their metrics and profiles.
+# Get a list of all assets and their market caps, sorted by market cap descending.
 response = messari.get_all_assets()
 
+# Get the ID, name, symbol, slug, market cap, sector, category, and tags for a single asset.
+response = messari.get_asset_by_id(asset_id=asset_id)
+
+# Get market data for a specific asset.
+response = messari.get_market_data_by_asset(asset_id=asset_id)
+
+# Get a list ROI data for all assets.
+response = messari.get_roi()
+
+# Get a single assets ROI data.
+response = messari.get_roi_by_asset(asset_id=asset_id)
+
+# Get a list of market specific data for all markets.
+response = messari.get_markets()
+
+# Get a list of exchanges with market data.
+response = messari.get_exchanges()
 ```
 
 -------
 #### Donate & Help maintain the library
 
 [![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
```

### Comparing `messari-2.0.0/messari/messari.py` & `messari-2.1.0/messari/messari.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         :param params: HTTP request parameters
         :return:
         """
         return self._send_message('GET', endpoint, params=params)
 
     def get_all_assets(self, **query_params):
         """
-        Get the paginated list of all assets and their metrics and profiles.
+        Returns a list of all assets and their market caps, sorted by market cap descending.
+        Each query parameter supports filtering on multiple, comma-separated values.
 
         :param query_params: dict of query parameters to filter the list
         :return: JSON response
         """
         path = '/asset/v1/assets'
 
         return self._get(path, params=query_params)
@@ -230,7 +231,32 @@
     def get_supported_assets(self, **kwargs):
         """
         Returns a list of all assets that Messari Intel actively covers.
         """
         path = f'/intel/v1/assets'
 
         return self._get(path, params=kwargs)
+
+    def get_news_feed(self, **kwargs):
+        """
+        Returns a list of all news articles, along with AI-generated summaries for each piece of content.
+        """
+        path = f'/news/v1/news/feed'
+
+        return self._get(path, params=kwargs)
+
+    def get_news_sources(self, **kwargs):
+        """
+        Returns a list of all news sources. Sources are the publications that Messari monitors.
+        """
+        path = f'/news/v1/news/sources'
+
+        return self._get(path, params=kwargs)
+
+    def get_news_assets(self, **kwargs):
+        """
+        Returns a list of all assets that have been tagged in news articles.
+        :return:
+        """
+        path = f'/news/v1/news/assets'
+
+        return self._get(path, params=kwargs)
```

### Comparing `messari-2.0.0/messari.egg-info/PKG-INFO` & `messari-2.1.0/messari.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messari
-Version: 2.0.0
+Version: 2.1.0
 Summary: Unofficial Messari API client.
 Home-page: https://github.com/itzmestar/Messari
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -48,17 +48,34 @@
 ```
 from messari import Messari
 
 # initialize api client
 
 messari = Messari(key='xxxxxxxxxxxxxxx')
 
-# Get the paginated list of all assets and their metrics and profiles.
+# Get a list of all assets and their market caps, sorted by market cap descending.
 response = messari.get_all_assets()
 
+# Get the ID, name, symbol, slug, market cap, sector, category, and tags for a single asset.
+response = messari.get_asset_by_id(asset_id=asset_id)
+
+# Get market data for a specific asset.
+response = messari.get_market_data_by_asset(asset_id=asset_id)
+
+# Get a list ROI data for all assets.
+response = messari.get_roi()
+
+# Get a single assets ROI data.
+response = messari.get_roi_by_asset(asset_id=asset_id)
+
+# Get a list of market specific data for all markets.
+response = messari.get_markets()
+
+# Get a list of exchanges with market data.
+response = messari.get_exchanges()
 ```
 
 -------
 #### Donate & Help maintain the library
 
 [![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
```

### Comparing `messari-2.0.0/setup.py` & `messari-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `messari-2.0.0/tests/test_messari.py` & `messari-2.1.0/tests/test_messari.py`

 * *Files identical despite different names*

