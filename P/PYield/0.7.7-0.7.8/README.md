# Comparing `tmp/pyield-0.7.7.tar.gz` & `tmp/pyield-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.7.tar", last modified: Thu Apr 25 00:26:44 2024, max compression
+gzip compressed data, was "pyield-0.7.8.tar", last modified: Sat Apr 27 14:04:14 2024, max compression
```

## Comparing `pyield-0.7.7.tar` & `pyield-0.7.8.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.7/LICENSE
--rw-r--r--   0        0        0     6467 2024-04-21 17:20:40.545037 pyield-0.7.7/README.md
--rw-r--r--   0        0        0       22 2024-04-25 00:10:29.617147 pyield-0.7.7/pyield/__about__.py
--rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.7/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.7/pyield/bday.py
--rw-r--r--   0        0        0     6091 2024-04-25 00:25:19.404158 pyield-0.7.7/pyield/data_access.py
--rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.7/pyield/data_analysis.py
--rw-r--r--   0        0        0      333 2024-04-21 13:45:50.722682 pyield-0.7.7/pyield/futures/__init__.py
--rw-r--r--   0        0        0    10269 2024-04-25 00:06:20.078463 pyield-0.7.7/pyield/futures/common.py
--rw-r--r--   0        0        0     3433 2024-04-24 23:25:56.361359 pyield-0.7.7/pyield/futures/ddi.py
--rw-r--r--   0        0        0     5369 2024-04-24 23:27:06.122355 pyield-0.7.7/pyield/futures/di.py
--rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.7/pyield/futures/di_xml.py
--rw-r--r--   0        0        0     2185 2024-04-24 23:24:39.630264 pyield-0.7.7/pyield/futures/frc.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.7/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.7/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.7/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.7/pyield/holidays/core.py
--rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.7/pyield/indicators.py
--rw-r--r--   0        0        0     3500 2024-04-25 00:22:37.836841 pyield-0.7.7/pyield/projections.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.7/pyield/py.typed
--rw-r--r--   0        0        0     6617 2024-04-21 13:41:53.731824 pyield-0.7.7/pyield/treasuries.py
--rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.7/pyield/utils.py
--rw-r--r--   0        0        0     1195 2024-04-25 00:26:44.621381 pyield-0.7.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.7/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.7/tests/test_bday.py
--rw-r--r--   0        0        0     2585 2024-04-22 23:45:59.541771 pyield-0.7.7/tests/test_futures.py
--rw-r--r--   0        0        0     8522 1970-01-01 00:00:00.000000 pyield-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.8/LICENSE
+-rw-r--r--   0        0        0     6508 2024-04-26 00:32:17.834190 pyield-0.7.8/README.md
+-rw-r--r--   0        0        0       22 2024-04-27 11:56:16.299935 pyield-0.7.8/pyield/__about__.py
+-rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.8/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.8/pyield/bday.py
+-rw-r--r--   0        0        0     6268 2024-04-27 13:08:29.971193 pyield-0.7.8/pyield/data_access.py
+-rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.8/pyield/data_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 23:39:41.039220 pyield-0.7.8/pyield/futures/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-27 12:39:19.772667 pyield-0.7.8/pyield/futures/historical/__init__.py
+-rw-r--r--   0        0        0     9277 2024-04-27 12:35:06.344046 pyield-0.7.8/pyield/futures/historical/common.py
+-rw-r--r--   0        0        0     2121 2024-04-27 12:38:36.571050 pyield-0.7.8/pyield/futures/historical/dap.py
+-rw-r--r--   0        0        0     2717 2024-04-26 08:19:58.862579 pyield-0.7.8/pyield/futures/historical/ddi.py
+-rw-r--r--   0        0        0     3095 2024-04-27 13:03:13.689638 pyield-0.7.8/pyield/futures/historical/di.py
+-rw-r--r--   0        0        0    11501 2024-04-27 13:47:29.988597 pyield-0.7.8/pyield/futures/historical/di_xml.py
+-rw-r--r--   0        0        0     2175 2024-04-26 08:20:47.784608 pyield-0.7.8/pyield/futures/historical/frc.py
+-rw-r--r--   0        0        0       71 2024-04-26 17:05:33.986164 pyield-0.7.8/pyield/futures/intraday/__init__.py
+-rw-r--r--   0        0        0     3595 2024-04-26 09:06:08.639852 pyield-0.7.8/pyield/futures/intraday/trading_data.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.8/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.8/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.8/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.8/pyield/holidays/core.py
+-rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.8/pyield/indicators.py
+-rw-r--r--   0        0        0     3500 2024-04-25 00:22:37.836841 pyield-0.7.8/pyield/projections.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.8/pyield/py.typed
+-rw-r--r--   0        0        0     6622 2024-04-27 13:46:18.187573 pyield-0.7.8/pyield/treasuries.py
+-rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.8/pyield/utils.py
+-rw-r--r--   0        0        0     1203 2024-04-27 14:04:14.278968 pyield-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.8/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.8/tests/test_bday.py
+-rw-r--r--   0        0        0     1225 2024-04-27 13:28:21.555207 pyield-0.7.8/tests/test_futures.py
+-rw-r--r--   0        0        0     8571 1970-01-01 00:00:00.000000 pyield-0.7.8/PKG-INFO
```

### Comparing `pyield-0.7.7/LICENSE` & `pyield-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/README.md` & `pyield-0.7.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 dtype: datetime64[ns]
 ```
 
 ### Futures Data
 ```python
 # Fetch current DI Futures data from B3 (15 minutes delay)
 >>> yd.fetch_asset(asset_code="DI1")
-TradeTimestamp      TickerSymbol ExpirationDate BDaysToExp ... MaxRate LastAskRate LastBidRate LastRate
+TradeTimestamp      TickerSymbol ExpirationDate BDaysToExp ... MaxRate LastAskRate LastBidRate CurrentRate
 2024-04-21 13:37:39       DI1K24     2024-05-02          7 ... 0.10660     0.10652     0.10660  0.10660
 2024-04-21 13:37:39       DI1M24     2024-06-03         28 ... 0.10518     0.10510     0.10516  0.10518
 2024-04-21 13:37:39       DI1N24     2024-07-01         48 ... 0.10480     0.10456     0.10462  0.10460
                 ...          ...            ...        ... ...     ...         ...         ...      ...
 2024-04-21 13:37:39       DI1F37     2037-01-02       3183 ...    <NA>        <NA>     0.11600     <NA>
 2024-04-21 13:37:39       DI1F38     2038-01-04       3432 ...    <NA>        <NA>     0.11600     <NA>
 2024-04-21 13:37:39       DI1F39     2039-01-03       3683 ...    <NA>        <NA>        <NA>     <NA>
@@ -111,19 +111,19 @@
    NTN-F    2024-04-11   2035-01-01     -1.27
 ```
 
 ### Indicators Data
 ```python
 # Fetch the SELIC target rate from the Central Bank of Brazil
 >>> yd.fetch_indicator(indicator_code="SELIC", reference_date='2024-04-12')
-10.75
+0.1075  # 10.75%
 
 # Fetch the IPCA monthly inflation rate from IBGE
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-03-18')
-0.16
+0.16  # 0.16%
 
 # If no data is yet available for the indicator, the function returns None
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-04-10')
 None
 ```
 
 ### Projections Data
@@ -131,13 +131,13 @@
 # Fetch current month projection for IPCA from IBGE API
 >>> ipca = yd.fetch_projection(projection_code="IPCA_CM")
 >>> print(ipca)
 IndicatorProjection(
     last_updated=Timestamp('2024-04-19 18:55:00'),
     reference_month_ts=Timestamp('2024-04-01 00:00:00'),
     reference_month_br='ABR/2024',
-    projected_value=0.0035
+    projected_value=0.0035  # 0.35%
 )
 >>> ipca.projected_value
-0.0035
+0.0035  # 0.35%
 ```
```

### Comparing `pyield-0.7.7/pyield/bday.py` & `pyield-0.7.8/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/data_access.py` & `pyield-0.7.8/pyield/data_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 
-from . import futures as ft
 from . import indicators as it
 from . import projections as pr
 from . import treasuries as tr
+from .futures import historical as fh
+from .futures import intraday as fi
 from .utils import _normalize_date
 
 
 def fetch_asset(
     asset_code: str,
     reference_date: str | pd.Timestamp | None = None,
     **kwargs,
@@ -20,14 +21,15 @@
         Supported options:
             - "TRB": Treasury bonds (indicative rates from ANBIMA).
             - "LTN", "LFT", "NTN-F", "NTN-B": Specific types of Brazilian treasury bonds
                   (indicative rates from ANBIMA).
             - "DI1": One-day Interbank Deposit Futures (Futuro de DI) from B3.
             - "DDI": DI x U.S. Dollar Spread Futures (Futuro de Cupom Cambial) from B3.
             - "FRC": Forward Rate Agreement (FRA) from B3.
+            - "DAP": DI x IPCA Spread Futures
         reference_date (str | pd.Timestamp | None): The reference date for which data is
             fetched. Defaults to the last business day if None.
         **kwargs: Additional keyword arguments, specifically:
             - return_raw (bool): Whether to return raw data without processing. Defaults
               to False.
 
     Returns:
@@ -39,32 +41,38 @@
     Examples:
         >>> fetch_asset('TRB', '2023-04-01')
         >>> fetch_asset('DI1', '2023-04-01', return_raw=True)
     """
     return_raw = kwargs.get("return_raw", False)
     normalized_date = _normalize_date(reference_date)
 
+    today = pd.Timestamp.today().normalize()
+    if normalized_date == today:
+        return fi.fetch_intraday(future_code=asset_code.upper())
+
     if asset_code.lower() == "trb":
         return tr.fetch_bonds(reference_date=normalized_date, return_raw=return_raw)
-    elif asset_code.lower() in ["ltn", "lft", "ntn-f", "ntn-b"]:
+
+    if asset_code.lower() in ["ltn", "lft", "ntn-f", "ntn-b"]:
         df = tr.fetch_bonds(reference_date=normalized_date)
         return df.query(f"BondType == '{asset_code.upper()}'")
 
-    elif asset_code.lower() == "di1":
-        today = pd.Timestamp.today().normalize()
-        if normalized_date == today:
-            return ft.fetch_last_di()
-        else:
-            return ft.fetch_past_di(trade_date=normalized_date, return_raw=return_raw)
-    elif asset_code.lower() == "ddi":
-        return ft.fetch_past_ddi(trade_date=normalized_date, return_raw=return_raw)
-    elif asset_code.lower() == "frc":
-        return ft.fetch_past_frc(trade_date=normalized_date, return_raw=return_raw)
-    else:
-        raise ValueError("Asset type not supported.")
+    if asset_code.lower() == "di1":
+        return fh.fetch_di(trade_date=normalized_date, return_raw=return_raw)
+
+    if asset_code.lower() == "ddi":
+        return fh.fetch_ddi(trade_date=normalized_date, return_raw=return_raw)
+
+    if asset_code.lower() == "frc":
+        return fh.fetch_frc(trade_date=normalized_date, return_raw=return_raw)
+
+    if asset_code.lower() == "dap":
+        return fh.fetch_dap(trade_date=normalized_date, return_raw=return_raw)
+
+    raise ValueError("Asset type not supported.")
 
 
 def fetch_indicator(
     indicator_code: str,
     reference_date: str | pd.Timestamp | None = None,
 ) -> float | None:
     """
```

### Comparing `pyield-0.7.7/pyield/data_analysis.py` & `pyield-0.7.8/pyield/data_analysis.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/futures/common.py` & `pyield-0.7.8/pyield/futures/historical/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,13 @@
 import io
 
 import pandas as pd
 import requests
 
-from .. import bday
-
-COLUMNS_MAPPING = {
-    "VENCTO": "ExpirationCode",
-    "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
-    "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
-    "NÚM. NEGOC.": "TradeCount",
-    "CONTR. NEGOC.": "TradeVolume",
-    "VOL.": "FinancialVolume",
-    "AJUSTE": "SettlementPrice",
-    "AJUSTE ANTER. (3)": "PrevSettlementRate",
-    "AJUSTE CORRIG. (4)": "AdjSettlementRate",
-    "AJUSTE  DE REF.": "SettlementRate",  # FRC
-    "PREÇO MÍN.": "MinRate",
-    "PREÇO MÉD.": "AvgRate",
-    "PREÇO MÁX.": "MaxRate",
-    "PREÇO ABERTU.": "FirstRate",
-    "ÚLT. PREÇO": "CloseRate",
-    "VAR. PTOS.": "PointsVariation",
-    # Attention: bid/ask rates are inverted
-    "ÚLT.OF. COMPRA": "CloseAskRate",
-    "ÚLT.OF. VENDA": "CloseBidRate",
-}
+from ... import bday
 
 
 def get_expiration_date(expiration_code: str) -> pd.Timestamp:
     """
     Converts an expiration code into its corresponding expiration date.
 
     This function translates an expiration code into a specific expiration date based on
@@ -149,15 +127,36 @@
         # Must use old holiday list, since this contract code was used until 2006.
         return bday.offset_bdays(expiration_date, offset=0, holiday_list="old")
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
-def fetch_past_raw_df(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
+def convert_prices_to_rates(
+    prices: pd.Series, days_to_expiration: pd.Series, count_convention: int
+) -> pd.Series:
+    """
+    Internal function to convert DI futures prices to rates.
+
+    Args:
+        prices (pd.Series): The futures prices to be converted.
+        days_to_expiration (pd.Series): The number of days to expiration for each price.
+        count_convention (int): The count convention for the DI futures contract.
+            Normally, it is 252 business days or 360 calendar days.
+
+    Returns:
+        pd.Series: A pd.Series containing the futures rates.
+    """
+    rates = (100_000 / prices) ** (count_convention / days_to_expiration) - 1
+
+    # Round to 5 (3 in %) dec. places (contract's current max. precision)
+    return rates.round(5)
+
+
+def fetch_raw_df(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Fetch the historical futures data from B3 for a specific trade date. If the data is
     not available, an empty DataFrame is returned.
 
     Args:
         trade_date (pd.Timestamp): The trade date for which the data should be fetched.
 
@@ -195,68 +194,15 @@
     # Force "AJUSTE CORRIG. (4)" to be float, since it can be also read as int
     if "AJUSTE CORRIG. (4)" in df.columns:
         df["AJUSTE CORRIG. (4)"] = df["AJUSTE CORRIG. (4)"].astype(pd.Float64Dtype())
 
     return df
 
 
-def fetch_last_raw_df(future_code: str) -> pd.DataFrame:
-    """
-    Fetch the latest data for a given future code from B3 derivatives quotation API.
-
-    Args:
-    future_code (str): The future code to fetch data for.
-
-    Returns:
-    pd.DataFrame: A DataFrame containing the normalized and cleaned data from the API.
-
-    Raises:
-    Exception: An exception is raised if the data fetch operation fails.
-    """
-
-    url = f"https://cotacao.b3.com.br/mds/api/v1/DerivativeQuotation/{future_code}"
-
-    try:
-        r = requests.get(url)
-        r.raise_for_status()  # Check for HTTP request errors
-    except requests.exceptions.RequestException:
-        raise Exception(f"Failed to fetch data for {future_code}.") from None
-
-    r.encoding = "utf-8"  # Explicitly set response encoding to utf-8 for consistency
-
-    # Normalize JSON response into a flat table
-    df = pd.json_normalize(r.json()["Scty"])
-
-    # Clean and reformat the DataFrame columns
-    df.columns = (df.columns
-        .str.replace("SctyQtn.", "")
-        .str.replace("asset.AsstSummry.", "")
-    )  # fmt: skip
-    df.drop(columns=["desc", "asset.code", "mkt.cd"], inplace=True)
-
-    # Convert maturity codes to datetime and drop rows with missing values
-    df["mtrtyCode"] = pd.to_datetime(df["mtrtyCode"], errors="coerce")
-    df.dropna(subset=["mtrtyCode"], inplace=True)
-
-    # Sort the DataFrame by maturity code and reset the index
-    df.sort_values("mtrtyCode", inplace=True, ignore_index=True)
-
-    # Get current date and time
-    now = pd.Timestamp.now().round("s")
-    # Subtract 15 minutes from the current time to account for API delay
-    trade_ts = now - pd.Timedelta(minutes=15)
-    df["TradeTimestamp"] = trade_ts
-
-    # Convert DataFrame to use nullable data types for better type consistency
-    df = df.convert_dtypes(dtype_backend="numpy_nullable")
-
-    return df
-
-
-def rename_columns(df: pd.DataFrame):
+def rename_columns(df: pd.DataFrame) -> pd.DataFrame:
     all_columns = {
         "VENCTO": "ExpirationCode",
         "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
         "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
         "NÚM. NEGOC.": "TradeCount",
         "CONTR. NEGOC.": "TradeVolume",
         "VOL.": "FinancialVolume",
@@ -270,21 +216,47 @@
         "PREÇO ABERTU.": "FirstRate",
         "ÚLT. PREÇO": "CloseRate",
         "VAR. PTOS.": "PointsVariation",
         # Attention: bid/ask rates are inverted
         "ÚLT.OF. COMPRA": "CloseAskRate",
         "ÚLT.OF. VENDA": "CloseBidRate",
     }
-    rename_dict = {}
-    for col in all_columns:
-        if col in df.columns:
-            rename_dict[col] = all_columns[col]
+    rename_dict = {c: all_columns[c] for c in all_columns if c in df.columns}
     return df.rename(columns=rename_dict)
 
 
+def process_raw_df(
+    df: pd.DataFrame, trade_date: pd.Timestamp, asset_code: str
+) -> pd.DataFrame:
+    df = rename_columns(df)
+
+    df["TradeDate"] = trade_date
+    # Convert to datetime64[ns] since it is pandas default type for timestamps
+    df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
+
+    df["TickerSymbol"] = asset_code + df["ExpirationCode"]
+
+    # Contract code format was changed in 22/05/2006
+    if trade_date < pd.Timestamp("2006-05-22"):
+        df["ExpirationDate"] = df["ExpirationCode"].apply(
+            get_old_expiration_date, args=(trade_date,)
+        )
+    else:
+        df["ExpirationDate"] = df["ExpirationCode"].apply(get_expiration_date)
+
+    # Columns where 0 means NaN
+    cols_with_nan = [col for col in df.columns if "Rate" in col]
+    if "SettlementPrice" in df.columns:
+        cols_with_nan.append("SettlementPrice")
+    # Replace 0 with NaN in these columns
+    df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
+
+    return df
+
+
 def reorder_columns(df: pd.DataFrame):
     all_columns = [
         "TradeDate",
         "TickerSymbol",
         # "ExpirationCode",
         "ExpirationDate",
         "BDaysToExp",
@@ -301,12 +273,9 @@
         "MinRate",
         "AvgRate",
         "MaxRate",
         "CloseAskRate",
         "CloseBidRate",
         "CloseRate",
     ]
-    reordered_columns = []
-    for col in all_columns:
-        if col in df.columns:
-            reordered_columns.append(col)
+    reordered_columns = [col for col in all_columns if col in df.columns]
     return df[reordered_columns]
```

### Comparing `pyield-0.7.7/pyield/futures/ddi.py` & `pyield-0.7.8/pyield/futures/historical/di.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,91 @@
 import pandas as pd
 
+from ... import bday as bd
 from . import common as cm
 
 
-def _convert_prices_to_rates(prices: pd.Series, n_days: pd.Series) -> pd.Series:
+def _convert_prices_to_rates(prices: pd.Series, bd: pd.Series) -> pd.Series:
     """
-    Internal function to convert DDI futures prices to rates.
+    Internal function to convert DI futures prices to rates.
 
     Args:
-        prices (pd.Series): A pd.Series containing DDI futures prices.
-        bd (pd.Series): A serie containing the number of days to expiration.
+        prices (pd.Series): A pd.Series containing DI futures prices.
+        bd (pd.Series): A serie containing the number of business days to expiration.
 
     Returns:
-        pd.Series: A pd.Series containing DDI futures rates.
+        pd.Series: A pd.Series containing DI futures rates.
     """
-    rates = (100_000 / prices - 1) * (360 / n_days)
+    rates = (100_000 / prices) ** (252 / bd) - 1
+
     # Round to 5 (3 in %) dec. places (contract's current max. precision)
     return rates.round(5)
 
 
-def _process_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _adjust_older_contracts_rates(df: pd.DataFrame, rate_cols: list) -> pd.DataFrame:
+    for col in rate_cols:
+        df[col] = _convert_prices_to_rates(df[col], df["BDaysToExp"])
+
+    # Invert low and high prices
+    df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
+
+    return df
+
+
+def _process_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
         pd.DataFrame: Processed and transformed data as a Pandas pd.DataFrame.
     """
-    df = cm.rename_columns(df)
-
-    df["TradeDate"] = trade_date
-    # Convert to datetime64[ns] since it is pandas default type for timestamps
-    df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
-
-    # Contract code format was changed in 22/05/2006
-    if trade_date < pd.Timestamp("2006-05-22"):
-        df["ExpirationDate"] = df["ExpirationCode"].apply(
-            cm.get_old_expiration_date, args=(trade_date,)
-        )
-    else:
-        df["ExpirationDate"] = df["ExpirationCode"].apply(cm.get_expiration_date)
-
-    df["DaysToExp"] = (df["ExpirationDate"] - trade_date).dt.days
-    # Convert to nullable integer, since other columns use this data type
-    df["DaysToExp"] = df["DaysToExp"].astype(pd.Int64Dtype())
+    df["BDaysToExp"] = bd.count_bdays(trade_date, df["ExpirationDate"])
 
     # Remove expired contracts
-    df.query("DaysToExp > 0", inplace=True)
+    df.query("BDaysToExp > 0", inplace=True)
 
-    # Columns where 0 means NaN
     rate_cols = [col for col in df.columns if "Rate" in col]
-    cols_with_nan = rate_cols + ["SettlementPrice"]
-    # Replace 0 with NaN in these columns
-    df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
-
-    df[rate_cols] = df[rate_cols].div(100).round(5)
+    # Prior to 17/01/2002 (inclusive), prices were not converted to rates
+    if trade_date > pd.Timestamp("2002-01-17"):
+        # Remove % and round to 5 (3 in %) dec. places in rate columns
+        df[rate_cols] = df[rate_cols].div(100).round(5)
+    else:
+        df = _adjust_older_contracts_rates(df, rate_cols)
 
     # Calculate SettlementRate
     df["SettlementRate"] = _convert_prices_to_rates(
-        df["SettlementPrice"], df["DaysToExp"]
+        df["SettlementPrice"], df["BDaysToExp"]
     )
 
-    df["TickerSymbol"] = "DI1" + df["ExpirationCode"]
-
-    # Filter and order columns
-    df = cm.reorder_columns(df)
-
     return df
 
 
-def fetch_past_ddi(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def fetch_di(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
     """
-    Fetchs the DDI futures data for a given date from B3.
+    Fetchs the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
-    trade date. It's the primary external interface for accessing DI data.
+    trade date. It's the primary external interface for accessing DI data. If the data
+    is not available, an empty DataFrame is returned.
 
     Args:
         trade_date (pd.Timestamp): The trade date to fetch the DI futures data.
-        raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
+        return_raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
             Defaults to False.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
 
-    Examples:
-        >>> from pyield.futures import di
-        >>> di.fetch_ddi(pd.Timestamp("2021-01-04"))
-
     Notes:
-        - DaysToExp: number of business days to ExpirationDate.
+        - BDaysToExp: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = cm.fetch_past_raw_df(asset_code="DDI", trade_date=trade_date)
+    df_raw = cm.fetch_raw_df(asset_code="DI1", trade_date=trade_date)
     if return_raw or df_raw.empty:
         return df_raw
-    return _process_raw_df(df_raw, trade_date)
+    df = cm.process_raw_df(df_raw, trade_date, asset_code="DI1")
+    df = _process_df(df, trade_date)
+    return cm.reorder_columns(df)
```

### Comparing `pyield-0.7.7/pyield/futures/di_xml.py` & `pyield-0.7.8/pyield/futures/historical/di_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import pandas as pd
 import requests
 from lxml import etree
 from pandas import DataFrame, Timestamp
 
-from .. import bday
+from ... import bday
 from . import common as cm
 
 
 def _get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
     """
     Types of XML files available:
     Full Price Report (all assets)
@@ -202,15 +202,15 @@
         # Must invert bid/ask for rates
         "BestAskPric": "BestBidRate",
         "BestBidPric": "BestAskRate",
         "MinPric": "MinRate",
         "TradAvrgPric": "AvgRate",
         "MaxPric": "MaxRate",
         "FrstPric": "FirstRate",
-        "LastPric": "LastRate",
+        "LastPric": "CloseRate",
         "AdjstdQtTax": "SettlementRate",
         # "RglrTxsQty"
         # "RglrTraddCtrcts"
         # "NtlRglrVol"
         # "IntlRglrVol",
         # "AdjstdQtStin",
         # "PrvsAdjstdQt",
```

### Comparing `pyield-0.7.7/pyield/futures/frc.py` & `pyield-0.7.8/pyield/futures/historical/frc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 
 from . import common as cm
 
 
-def _process_past_data(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _process_frc_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
@@ -29,33 +29,32 @@
         df["ExpirationDate"] = df["ExpirationCode"].apply(cm.get_expiration_date)
 
     # Replace 0 values in rate columns with pd.NA and remove percentage
     rate_cols = [col for col in df.columns if "Rate" in col]
     # Round to 5 decimal places (3 in %) since it is the contract's precision
     df[rate_cols] = df[rate_cols].replace(0, pd.NA).div(100).round(5)
 
-    df["TickerSymbol"] = "FRC" + df["ExpirationCode"]
-
-    # Filter and order columns
-    df = cm.reorder_columns(df)
     return df
 
 
-def fetch_past_frc(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def fetch_frc(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
     """
     Fetchs the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
     trade date. It's the primary external interface for accessing DI data.
 
     Args:
         trade_date (pd.Timestamp): The trade date to fetch the DI futures data.
         raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
             Defaults to False.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
     """
-    df_raw = cm.fetch_past_raw_df(asset_code="FRC", trade_date=trade_date)
+    df_raw = cm.fetch_raw_df(asset_code="FRC", trade_date=trade_date)
     if return_raw or df_raw.empty:
         return df_raw
-    return _process_past_data(df_raw, trade_date)
+    # Filter and order columns
+    df = cm.process_raw_df(df_raw, trade_date, asset_code="FRC")
+    df = _process_frc_df(df, trade_date)
+    return cm.reorder_columns(df)
```

### Comparing `pyield-0.7.7/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.8/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.8/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/holidays/core.py` & `pyield-0.7.8/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/indicators.py` & `pyield-0.7.8/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/projections.py` & `pyield-0.7.8/pyield/projections.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyield/treasuries.py` & `pyield-0.7.8/pyield/treasuries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import pandas as pd
 import requests
 
-from . import futures as ft
+from .futures import historical as fh
 
 # URL Constants
 ANBIMA_NON_MEMBER_URL = "https://www.anbima.com.br/informacoes/merc-sec/arqs/"
 ANBIMA_MEMBER_URL = "http://www.anbima.associados.rtm/merc_sec/arqs/"
 
 # Constant for conversion to basis points
 BPS_CONVERSION_FACTOR = 10_000
@@ -146,15 +146,15 @@
 
     Returns:
         pd.DataFrame: A DataFrame containing the bond type, reference date, maturity
             date, and the calculated DI spread in basis points. The data is sorted by
             bond type and maturity date.
     """
     # Fetch DI rates and adjust the maturity date format for compatibility
-    df_di = ft.fetch_past_di(reference_date)[["ExpirationDate", "SettlementRate"]]
+    df_di = fh.fetch_di(reference_date)[["ExpirationDate", "SettlementRate"]]
 
     # Renaming the columns to match the ANBIMA structure
     df_di.rename(columns={"ExpirationDate": "MaturityDate"}, inplace=True)
 
     # Adjusting maturity date to match bond data format
     df_di["MaturityDate"] = df_di["MaturityDate"].dt.to_period("M").dt.to_timestamp()
```

### Comparing `pyield-0.7.7/pyield/utils.py` & `pyield-0.7.8/pyield/utils.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/pyproject.toml` & `pyield-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Financial and Insurance Industry",
     "Topic :: Office/Business :: Financial :: Investment",
 ]
 dependencies = [
-    "requests",
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
     "python-calamine>=0.2.0",
+    "requests>=2.31.0",
 ]
 dynamic = []
-version = "0.7.7"
+version = "0.7.8"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.7/tests/test_bday.py` & `pyield-0.7.8/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.7/PKG-INFO` & `pyield-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
         
@@ -28,21 +28,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Project-URL: Source, https://github.com/crdcj/PYield
 Requires-Python: >=3.11
-Requires-Dist: requests
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: numpy
 Requires-Dist: beautifulsoup4
 Requires-Dist: html5lib
 Requires-Dist: lxml
 Requires-Dist: python-calamine>=0.2.0
+Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/pyield.svg)](https://pypi.python.org/pypi/pyield)
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
 # PYield: Brazilian Fixed Income Toolkit
@@ -97,15 +97,15 @@
 dtype: datetime64[ns]
 ```
 
 ### Futures Data
 ```python
 # Fetch current DI Futures data from B3 (15 minutes delay)
 >>> yd.fetch_asset(asset_code="DI1")
-TradeTimestamp      TickerSymbol ExpirationDate BDaysToExp ... MaxRate LastAskRate LastBidRate LastRate
+TradeTimestamp      TickerSymbol ExpirationDate BDaysToExp ... MaxRate LastAskRate LastBidRate CurrentRate
 2024-04-21 13:37:39       DI1K24     2024-05-02          7 ... 0.10660     0.10652     0.10660  0.10660
 2024-04-21 13:37:39       DI1M24     2024-06-03         28 ... 0.10518     0.10510     0.10516  0.10518
 2024-04-21 13:37:39       DI1N24     2024-07-01         48 ... 0.10480     0.10456     0.10462  0.10460
                 ...          ...            ...        ... ...     ...         ...         ...      ...
 2024-04-21 13:37:39       DI1F37     2037-01-02       3183 ...    <NA>        <NA>     0.11600     <NA>
 2024-04-21 13:37:39       DI1F38     2038-01-04       3432 ...    <NA>        <NA>     0.11600     <NA>
 2024-04-21 13:37:39       DI1F39     2039-01-03       3683 ...    <NA>        <NA>        <NA>     <NA>
@@ -154,19 +154,19 @@
    NTN-F    2024-04-11   2035-01-01     -1.27
 ```
 
 ### Indicators Data
 ```python
 # Fetch the SELIC target rate from the Central Bank of Brazil
 >>> yd.fetch_indicator(indicator_code="SELIC", reference_date='2024-04-12')
-10.75
+0.1075  # 10.75%
 
 # Fetch the IPCA monthly inflation rate from IBGE
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-03-18')
-0.16
+0.16  # 0.16%
 
 # If no data is yet available for the indicator, the function returns None
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-04-10')
 None
 ```
 
 ### Projections Data
@@ -174,13 +174,13 @@
 # Fetch current month projection for IPCA from IBGE API
 >>> ipca = yd.fetch_projection(projection_code="IPCA_CM")
 >>> print(ipca)
 IndicatorProjection(
     last_updated=Timestamp('2024-04-19 18:55:00'),
     reference_month_ts=Timestamp('2024-04-01 00:00:00'),
     reference_month_br='ABR/2024',
-    projected_value=0.0035
+    projected_value=0.0035  # 0.35%
 )
 >>> ipca.projected_value
-0.0035
+0.0035  # 0.35%
 ```
```

