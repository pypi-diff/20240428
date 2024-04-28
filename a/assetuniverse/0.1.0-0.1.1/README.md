# Comparing `tmp/assetuniverse-0.1.0.tar.gz` & `tmp/assetuniverse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assetuniverse-0.1.0.tar", last modified: Sun Apr 28 20:42:29 2024, max compression
+gzip compressed data, was "assetuniverse-0.1.1.tar", last modified: Sun Apr 28 21:40:59 2024, max compression
```

## Comparing `assetuniverse-0.1.0.tar` & `assetuniverse-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:42:29.253231 assetuniverse-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-28 20:42:29.249231 assetuniverse-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:42:29.249231 assetuniverse-0.1.0/assetuniverse/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/assetuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/assetuniverse/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:42:29.249231 assetuniverse-0.1.0/assetuniverse/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/assetuniverse/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/assetuniverse/utils/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/assetuniverse/utils/downloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:42:29.249231 assetuniverse-0.1.0/assetuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-28 20:42:29.000000 assetuniverse-0.1.0/assetuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-28 20:42:29.000000 assetuniverse-0.1.0/assetuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:42:29.000000 assetuniverse-0.1.0/assetuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:42:29.000000 assetuniverse-0.1.0/assetuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 20:42:29.000000 assetuniverse-0.1.0/assetuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-28 20:41:50.000000 assetuniverse-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:42:29.253231 assetuniverse-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:40:59.139130 assetuniverse-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-28 21:40:59.139130 assetuniverse-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:40:59.135131 assetuniverse-0.1.1/assetuniverse/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/assetuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/assetuniverse/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:40:59.139130 assetuniverse-0.1.1/assetuniverse/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/assetuniverse/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/assetuniverse/utils/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/assetuniverse/utils/downloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:40:59.139130 assetuniverse-0.1.1/assetuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-28 21:40:59.000000 assetuniverse-0.1.1/assetuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-28 21:40:59.000000 assetuniverse-0.1.1/assetuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:40:59.000000 assetuniverse-0.1.1/assetuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 21:40:59.000000 assetuniverse-0.1.1/assetuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 21:40:59.000000 assetuniverse-0.1.1/assetuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-28 21:40:22.000000 assetuniverse-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:40:59.139130 assetuniverse-0.1.1/setup.cfg
```

### Comparing `assetuniverse-0.1.0/LICENSE` & `assetuniverse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `assetuniverse-0.1.0/PKG-INFO` & `assetuniverse-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assetuniverse
-Version: 0.1.0
+Version: 0.1.1
 Summary: A downloader of historical daily returns for multiple investable assets with some analysis tools too.
 Author: Matthew Trotter
 License: GPL-3.0-or-later
 Keywords: historical returns,returns,daily returns,stocks,futures,commodities,interactive brokers,yahoo finance,fred
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,20 @@
 
 Download historical daily prices and returns of stocks, futures, cryptocurrencies, and fiat currencies. Plot historical returns and calculate correlation and covariance matrices. Asset Universe downloads historical data from the following sources:
 
 - [Interactive Brokers Trader Workstation](https://www.interactivebrokers.com/en/trading/tws.php)
 - [Yahoo Finance](https://finance.yahoo.com/)
 - [Federal Reserve Economic Database](https://fred.stlouisfed.org)
 
+## Installing
+Install the [package with pip](https://pypi.org/project/assetuniverse/0.1.0/#description):
+```bash
+pip install assetuniverse
+```
+
 ## Using
 ```python
 import datetime
 from assetuniverse import Asset, AssetUniverse
 
 # Set start date, end date, and assets to download
 days = 2*365    # 2 years
```

### Comparing `assetuniverse-0.1.0/README.md` & `assetuniverse-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 
 Download historical daily prices and returns of stocks, futures, cryptocurrencies, and fiat currencies. Plot historical returns and calculate correlation and covariance matrices. Asset Universe downloads historical data from the following sources:
 
 - [Interactive Brokers Trader Workstation](https://www.interactivebrokers.com/en/trading/tws.php)
 - [Yahoo Finance](https://finance.yahoo.com/)
 - [Federal Reserve Economic Database](https://fred.stlouisfed.org)
 
+## Installing
+Install the [package with pip](https://pypi.org/project/assetuniverse/0.1.0/#description):
+```bash
+pip install assetuniverse
+```
+
 ## Using
 ```python
 import datetime
 from assetuniverse import Asset, AssetUniverse
 
 # Set start date, end date, and assets to download
 days = 2*365    # 2 years
```

### Comparing `assetuniverse-0.1.0/assetuniverse/core.py` & `assetuniverse-0.1.1/assetuniverse/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
             fd.download(),
             od.download()
         ]
         ibd.shutdown()
 
         # Join all closes together on same date axis
         joined_prices = self._join_prices(prices_list)
-        self.last_dates_downloaded = pd.concat((ibd.last_dates_downloaded, yfd.last_dates_downloaded, fd.last_dates_downloaded, od.last_dates_downloaded))
+        d = [d for d in [ibd.last_dates_downloaded, yfd.last_dates_downloaded, fd.last_dates_downloaded, od.last_dates_downloaded] if d is not None and not d.empty]
+        self.last_dates_downloaded = pd.concat(d)
 
         # Rename cash and borrow rate
         cashname = 'Cash'
         borrowname = 'Borrow Rate'
         joined_prices = joined_prices.rename(columns={self.borrowrate.ticker: borrowname})
         self.borrowrate.ticker = borrowname
         if self.cashasset.ticker:
@@ -112,15 +113,15 @@
             if not joined_prices.empty:
                 # Join prices with previous prices
                 joined_prices = joined_prices.join(prices, how='inner')
         # closes = closes.join(annualBorrowRate, how='left')    # Do I need this for the borrow rate? Different than how='inner'
 
         # Forward fill all the NaNs and zeros
         joined_prices[joined_prices == 0] = np.nan
-        joined_prices.fillna(method="ffill", inplace=True)
+        joined_prices.ffill(inplace=True)
         joined_prices.dropna(axis=0, how="any", inplace=True)
 
         # # Forward-fill cash closes - Do I need this part?
         # idx = date_range(self.start, self.end)
         # closesCash = closesCash.reindex(idx, method='ffill')
 
         return joined_prices
```

### Comparing `assetuniverse-0.1.0/assetuniverse/utils/asset.py` & `assetuniverse-0.1.1/assetuniverse/utils/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         Parameters
         ----------
         prices : pd.Series
             Unnormalized daily closing prices.
         """
         self.prices = prices
-        self.prices_normalized = self.prices/self.prices[0] # Normalize price to start from $1
+        self.prices_normalized = self.prices/self.prices.iloc[0] # Normalize price to start from $1
         self.returns = self.prices.pct_change()
         self.returns = self.returns[1:]  # delete first row - pct_change() returns first row as NaN
 
     def __str__(self):
         result = f'{self.ticker}, '
         if len(self.alternate_tickers):
             alternate_names = ', '.join([t for t in self.alternate_tickers])
```

### Comparing `assetuniverse-0.1.0/assetuniverse/utils/downloaders.py` & `assetuniverse-0.1.1/assetuniverse/utils/downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 import ib_insync
 import yfinance as yf
 import pandas_datareader.data as web
 
 import datetime
 from pandas import DataFrame, date_range, Series
 import numpy as np
+from typing import Union
 
 class Downloader:
     def __init__(self, start, end, tickers) -> None:
         self.start = start
         self.end = end
         self.tickers = tickers
         self.last_dates_downloaded = None
 
-    def _calculate_last_date_downloaded(self, closes: DataFrame) -> None:
-        self.last_dates_downloaded = closes.apply(Series.last_valid_index)
+    def _calculate_last_date_downloaded(self, closes: DataFrame) -> Union[None, Series]:
+        self.last_dates_downloaded = closes.apply(Series.last_valid_index)  # type: Series
 
 class InteractiveBrokersDownloader(Downloader):
     def __init__(self, start, end, tickers, currencies, exchanges) -> None:
         super().__init__(start, end, tickers)
         self.currencies = currencies
         self.exchanges = exchanges
         self.ib = None
@@ -169,22 +170,22 @@
         closes = DataFrame()
         for ticker in self.tickers:
             closes = web.DataReader(
                 self.freddic.get(ticker, ticker), 
                 'fred', 
                 self.start, 
                 self.end+datetime.timedelta(1)
-                )
+                )   # type: DataFrame
             closes = closes.rename(columns={closes.columns[0]: ticker})
 
             # Reindex tickers that aren't updated often
             if ticker in ['Fed Funds Rate',]:
                 idx = date_range(start=self.start, end=self.end, freq='D')
                 closes = closes.reindex(idx)
-                closes.fillna(method="ffill", inplace=True)
+                closes.ffill(inplace=True)
         super()._calculate_last_date_downloaded(closes)
         return closes
 
 
 class OfflineDownloader(Downloader):
     """Generates random prices and returns for situations without internet access
     """
```

### Comparing `assetuniverse-0.1.0/assetuniverse.egg-info/PKG-INFO` & `assetuniverse-0.1.1/assetuniverse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assetuniverse
-Version: 0.1.0
+Version: 0.1.1
 Summary: A downloader of historical daily returns for multiple investable assets with some analysis tools too.
 Author: Matthew Trotter
 License: GPL-3.0-or-later
 Keywords: historical returns,returns,daily returns,stocks,futures,commodities,interactive brokers,yahoo finance,fred
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,20 @@
 
 Download historical daily prices and returns of stocks, futures, cryptocurrencies, and fiat currencies. Plot historical returns and calculate correlation and covariance matrices. Asset Universe downloads historical data from the following sources:
 
 - [Interactive Brokers Trader Workstation](https://www.interactivebrokers.com/en/trading/tws.php)
 - [Yahoo Finance](https://finance.yahoo.com/)
 - [Federal Reserve Economic Database](https://fred.stlouisfed.org)
 
+## Installing
+Install the [package with pip](https://pypi.org/project/assetuniverse/0.1.0/#description):
+```bash
+pip install assetuniverse
+```
+
 ## Using
 ```python
 import datetime
 from assetuniverse import Asset, AssetUniverse
 
 # Set start date, end date, and assets to download
 days = 2*365    # 2 years
```

### Comparing `assetuniverse-0.1.0/pyproject.toml` & `assetuniverse-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "assetuniverse"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Matthew Trotter"},
 ]
 description = "A downloader of historical daily returns for multiple investable assets with some analysis tools too."
 readme = "README.md"
 license = {text = "GPL-3.0-or-later"}
 requires-python = ">=3.7"
```

