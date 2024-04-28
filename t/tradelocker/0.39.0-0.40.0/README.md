# Comparing `tmp/tradelocker-0.39.0.tar.gz` & `tmp/tradelocker-0.40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradelocker-0.39.0.tar", max compression
+gzip compressed data, was "tradelocker-0.40.0.tar", max compression
```

## Comparing `tradelocker-0.39.0.tar` & `tradelocker-0.40.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-01-29 04:25:19.335223 tradelocker-0.39.0/LICENSE.txt
--rw-r--r--   0        0        0     2829 2024-01-29 10:24:46.154995 tradelocker-0.39.0/README.md
--rw-r--r--   0        0        0     1311 2024-01-29 10:57:38.076394 tradelocker-0.39.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-11-12 17:41:23.849110 tradelocker-0.39.0/src/tradelocker/__about__.py
--rw-r--r--   0        0        0       85 2024-01-12 15:21:56.408569 tradelocker-0.39.0/src/tradelocker/__init__.py
--rw-r--r--   0        0        0        0 2023-11-12 17:41:23.849205 tradelocker-0.39.0/src/tradelocker/py.typed
--rw-r--r--   0        0        0    48890 2024-01-29 09:52:28.461285 tradelocker-0.39.0/src/tradelocker/tradelocker_api.py
--rw-r--r--   0        0        0     5025 2024-01-11 23:43:20.999591 tradelocker-0.39.0/src/tradelocker/types.py
--rw-r--r--   0        0        0     9118 2024-01-29 09:52:28.462879 tradelocker-0.39.0/src/tradelocker/utils.py
--rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 tradelocker-0.39.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-28 19:44:48.930398 tradelocker-0.40.0/LICENSE.txt
+-rw-r--r--   0        0        0     2829 2024-04-28 19:44:48.931056 tradelocker-0.40.0/README.md
+-rw-r--r--   0        0        0     1476 2024-04-28 19:50:08.283720 tradelocker-0.40.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-28 19:44:48.950787 tradelocker-0.40.0/src/tradelocker/__about__.py
+-rw-r--r--   0        0        0       85 2024-04-28 19:44:48.941751 tradelocker-0.40.0/src/tradelocker/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:44:48.950881 tradelocker-0.40.0/src/tradelocker/py.typed
+-rw-r--r--   0        0        0    52279 2024-04-28 19:50:08.275201 tradelocker-0.40.0/src/tradelocker/tradelocker_api.py
+-rw-r--r--   0        0        0     5342 2024-04-28 19:50:08.275982 tradelocker-0.40.0/src/tradelocker/types.py
+-rw-r--r--   0        0        0     9168 2024-04-28 19:50:08.276686 tradelocker-0.40.0/src/tradelocker/utils.py
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 tradelocker-0.40.0/PKG-INFO
```

### Comparing `tradelocker-0.39.0/LICENSE.txt` & `tradelocker-0.40.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tradelocker-0.39.0/README.md` & `tradelocker-0.40.0/README.md`

 * *Files identical despite different names*

### Comparing `tradelocker-0.39.0/pyproject.toml` & `tradelocker-0.40.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tradelocker"
-version = "0.39.0"
+version = "0.40.0"
 description = "TradeLocker Trading API support for Python"
 authors = ["TradeLocker <admin@tradelocker.com>"]
 license = "MIT"
 readme = "README.md"
 keywords=["tradelocker","api", "rest", "trading", "exchange", "algotrading", "algo", "bots", "strategies"]
 urls.Source = "https://github.com/tradelocker/tradelocker-python/"
 urls.Issues = "https://github.com/tradelocker/tradelocker-python/issues"
@@ -16,15 +16,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 
 pandas = "2.1.1"
 PyJWT = "2.8.0"
 Requests = "2.31.0"
-typeguard = "4.1.5"
+# typeguard is removed as being a dependency that is installed by since it causes problems with pyinstaller and nuitka -- add it manually if you prefer to use it.
+# typeguard = "4.1.5"
 colorlog = "6.6.0"
 python-dotenv = "1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.4.2"
 pytest-cov = "4.1.0"
 mypy = "1.5.1"
```

### Comparing `tradelocker-0.39.0/src/tradelocker/tradelocker_api.py` & `tradelocker-0.40.0/src/tradelocker/tradelocker_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from math import floor
 from functools import lru_cache
 from typing import cast, Literal, Optional, Tuple
 
 import requests
 import pandas as pd
 
+import logging
+
 from tradelocker.utils import (
-    ColorLogger,
+    color_logger,
     log_func,
     get_nested_key,
     resolve_lookback_and_timestamps,
     retry,
     tl_typechecked,
     tl_check_type,
     estimate_history_size,
@@ -23,14 +25,15 @@
 from .types import (
     DailyBarType,
     ColumnConfigKeysType,
     ColumnConfigValuesType,
     ConfigColumnType,
     ConfigType,
     InstrumentDetailsType,
+    LimitsType,
     LocaleType,
     LogLevelType,
     MarketDepthlistType,
     ModificationParamsType,
     OrderTypeType,
     RequestsMappingType,
     ResolutionType,
@@ -56,42 +59,68 @@
 
 from time import sleep
 
 # More information about the API: https://tradelocker.com/api
 
 # Constants
 _TIMEOUT: Tuple[int, int] = (10, 30)  # (connection_timeout, read_timeout
-_MAX_HISTORY_ROWS: int = 40000
 _EPS: float = 0.00001
 _MIN_LOT_SIZE: float = (
     0.01  ## TODO: this should probably be fetched per-instrument from BE
 )
 
 
 class TLAPI:
     """TradeLocker API Client
 
     Implements a REST connection to the TradeLocker REST API.
 
     See https://tradelocker.com/api/ for more information.
     """
 
+    _instances = {}
+
+    # This is here to ensure that users don't accidentally create multiple instances
+    # of the same TLAPI object, which would lead to multiple connections to the API for no reason.
+    # However, different instances can be created with different parameters,
+    # or a new instance will be created in case the access token has expired.
+    def __new__(cls, *args, **kwargs):
+        multiton_key = (cls, args, frozenset(kwargs.items()))
+        # Generate a new instance only if the key is not in the instances dict or the access token has expired
+
+        if (
+            multiton_key in cls._instances
+            and hasattr(cls._instances[multiton_key], "_access_token")
+            and time_to_token_expiry(cls._instances[multiton_key]._access_token) > 0
+        ):
+            # Just warn the user, and reuse the existing instance
+            logging.warning(f"Reusing existing TLAPI instance for {cls.__name__}")
+        else:
+            # Create a new instance
+            cls._instances[multiton_key] = super(TLAPI, cls).__new__(cls)
+        return cls._instances[multiton_key]
+
     @tl_typechecked
     def __init__(
         self,
         environment: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         server: Optional[str] = None,
         access_token: Optional[str] = None,
         refresh_token: Optional[str] = None,
         account_id: int = 0,
         acc_num: int = 0,
         log_level: LogLevelType = "debug",
     ) -> None:
+        # Those object with _initialized tag have already been initialized,
+        # so there is no need to re-initialize anything.
+        if hasattr(self, "_initialized") and self._initialized:
+            return
+
         """Initializes the TradeLocker API client."""
         self._base_url: str = f"{environment}/backend-api"
         self._credentials: Optional[CredentialsType] = None
 
         self._access_token: str = ""
         self._refresh_token: str = ""
         self.acc_num: int = 0
@@ -101,15 +130,15 @@
         if username and password and server:
             self._credentials = {
                 "username": username,
                 "password": password,
                 "server": server,
             }
 
-        self.log = ColorLogger(__name__, log_level=log_level).get_logger()
+        self.log = color_logger
 
         if self._credentials:
             self._auth_with_password(
                 username=self._credentials["username"],
                 password=self._credentials["password"],
                 server=self._credentials["server"],
             )
@@ -117,14 +146,16 @@
         elif access_token and refresh_token:
             self._auth_with_tokens(access_token, refresh_token)
             self._set_account_id_and_acc_num(account_id, acc_num)
         else:
             error_msg = f"Either username/pass/server, or access_token/refresh_token must be provided!"
             raise Exception(error_msg)
 
+        self._initialized = True
+
     def get_base_url(self) -> str:
         """Returns the base URL of the API."""
         return self._base_url
 
     ############################## AUTH ROUTES ##########################
 
     def get_access_token(self) -> str:
@@ -234,15 +265,15 @@
 
     @lru_cache
     @tl_typechecked
     def _get_column_names(self, object_name: ColumnConfigKeysType) -> list[str]:
         """Returns the column names of values in orders/positions, etc. from the /config endpoint
 
         Args:
-            object_name (_ColumnConfigKeysType): The name of the object to get the column names for
+            object_name (ColumnConfigKeysType): The name of the object to get the column names for
         Returns:
             list[str]: The column names
         """
         config_dict: ConfigType = self.get_config()
 
         # Using cast because /config is really ugly and irregular, so mypy needs help.
         config_for_object: ColumnConfigValuesType = cast(
@@ -264,14 +295,25 @@
         return self._get_route_id(instrument_id, "TRADE")
 
     @lru_cache
     def _get_info_route_id(self, instrument_id: int) -> str:
         """Returns the "INFO" route_id for the specified instrument_id"""
         return self._get_route_id(instrument_id, "INFO")
 
+    @lru_cache
+    def _get_max_history_rows(self) -> int:
+        config_dict: ConfigType = self.get_config()
+        limits: list[LimitsType] = get_nested_key(
+            config_dict, ["limits"], list[LimitsType]
+        )
+        for limit in limits:
+            if limit["limitType"] == "QUOTES_HISTORY_BARS":
+                return limit["limit"]
+        raise Exception("Failed to fetch max history rows")
+
     @tl_typechecked
     def _get_route_id(self, instrument_id: int, route_type: RouteTypeType) -> str:
         """Returns the route_id for the specified instrument_id and route_type (TRADE/INFO)"""
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments: pd.DataFrame = all_instruments[
             all_instruments["tradableInstrumentId"] == instrument_id
         ]
@@ -412,32 +454,63 @@
                 except Exception as err:
                     self.log.warning(
                         f"Failed to apply type {column_types[column]} to column {column}: {err}"
                     )
 
     ############################## PUBLIC UTILS #######################
 
-    @log_func
     @tl_typechecked
+    @lru_cache
+    @log_func
     def get_instrument_id_from_symbol_name(self, symbol_name: str) -> int:
-        """Returns the instrument Id from the given symol.
+        """Returns the instrument Id from the given symol's name.
 
         Args:
             symbol_name (str): Name of the symbol, for example `BTCUSD`
 
         Raises:
             ValueError: Will be raised if instrument was with given symbol name was not found
 
         Returns:
             int: On success the instrument Id will be returned
         """
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments = all_instruments[all_instruments["name"] == symbol_name]
         if len(matching_instruments) == 0:
-            raise ValueError(f"No instrument found with symbol = {symbol_name}")
+            raise ValueError(f"No instrument found with {symbol_name=}")
+        if len(matching_instruments) > 1:
+            self.log.warning(
+                f"Multiple instruments found with {symbol_name=}. Using the first one."
+            )
+
+        return int(matching_instruments["tradableInstrumentId"].iloc[0])
+
+    @log_func
+    @tl_typechecked
+    def get_instrument_id_from_symbol_id(self, symbol_id: int) -> int:
+        """Returns the instrument Id from the given symbol's id.
+
+        Args:
+            symbol_id (int): Id the symbol
+
+        Raises:
+            ValueError: Will be raised if instrument was with given symbol id was not found
+
+        Returns:
+            int: On success the instrument Id will be returned
+        """
+        all_instruments: pd.DataFrame = self.get_all_instruments()
+        matching_instruments = all_instruments[all_instruments["id"] == symbol_id]
+        if len(matching_instruments) == 0:
+            raise ValueError(f"No instrument found with {symbol_id=}")
+        if len(matching_instruments) > 1:
+            self.log.warning(
+                f"Multiple instruments found with {symbol_id=}. Using the first one."
+            )
+
         return int(matching_instruments["tradableInstrumentId"].iloc[0])
 
     @log_func
     @tl_typechecked
     def get_symbol_name_from_instrument_id(self, instrument_id: int) -> str:
         """Returns the symbol name from the given instrument Id.
 
@@ -450,24 +523,29 @@
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments = all_instruments[
             all_instruments["tradableInstrumentId"] == instrument_id
         ]
         if len(matching_instruments) == 0:
             raise ValueError(f"No instrument found with id = {instrument_id}")
 
-        print(f"(get_symbol_name_from_instrument_id) instrument_id: {instrument_id}")
-        print(f"matching_instruments:\n{matching_instruments}")
+        self.log.debug(
+            f"(get_symbol_name_from_instrument_id) instrument_id: {instrument_id}"
+        )
+        self.log.debug(f"matching_instruments:\n{matching_instruments}")
         return matching_instruments["name"].iloc[0]
 
     @log_func
     @tl_typechecked
     def close_all_positions(self, instrument_id_filter: int = 0) -> bool:
-        """Closes all open positions.
+        """Places an order to close all open positions.
 
-        If instrument_id is provied, only positions in this instrument will be closed
+        If instrument_id is provied, only positions in this instrument will be closed.
+
+        IMPORTANT: Isn't guaranteed to close all positions, or close them immediately.
+        Will attempt to place an IOC, then GTC closing order, so the execution might be delayed.
 
         Args:
             instrument_id_filter (int, optional): _description_. Defaults to 0.
 
         Returns:
             bool: True if executed successfully False otherwise
         """
@@ -567,19 +645,22 @@
         return response_status == "ok"
 
     @log_func
     @tl_typechecked
     def close_position(
         self, order_id: int = 0, position_id: int = 0, close_quantity: float = 0
     ) -> None:
-        """Closes a position.
+        """Places an order to closee a position.
 
         Either the order_id or the position_id needs to be provided. If both are
         provided, the order_id will be used and the position_id will be ignored.
 
+        IMPORTANT: Isn't guaranteed to close the position, or close it immediately.
+        Will attempt to place an IOC, then GTC closing order, so the execution might be delayed.
+
         Args:
             order_id (int, optional): The order id. Defaults to 0.
             position_id (int, optional): The position id. Defaults to 0.
             close_quantity (float, optional): If a value bigger than 0 is provided the size of the position will be reduced by the given amount. Defaults to 0.
 
         Raises:
             ValueError: Will be raised if no order_id or position_id was provided
@@ -677,16 +758,16 @@
         response_json = self._get_response_json(response)
 
         self.log.info("Successfully refreshed authentication tokens")
 
         self._access_token = get_nested_key(response_json, ["accessToken"], str)
         self._refresh_token = get_nested_key(response_json, ["refreshToken"], str)
 
-    @log_func
     @lru_cache(maxsize=1)
+    @log_func
     @tl_typechecked
     def get_all_accounts(self) -> pd.DataFrame:
         """Returns all accounts associated with the account used for authentication.
 
         Raises:
             Exception: Will be raised if account informations could not be fetched
 
@@ -706,22 +787,22 @@
             self.log.critical("Failed to fetch user's accounts")
             raise Exception("Failed to fetch user's accounts")
 
         return accounts
 
     ############################## CONFIG ROUTES ##########################
 
-    @log_func
     @lru_cache(maxsize=1)
+    @log_func
     @tl_typechecked
     def get_config(self) -> ConfigType:
         """Returns the user's configuration.
 
         Returns:
-            _ConfigType: The configuration
+            ConfigType: The configuration
         """
         route_url = f"{self._base_url}/trade/config"
         response_json = self._request_get(route_url)
         config_dict: ConfigType = get_nested_key(response_json, ["d"], ConfigType)
         return config_dict
 
     ############################## ACCOUNT ROUTES ##########################
@@ -730,15 +811,15 @@
     @tl_typechecked
     def get_trade_accounts(self) -> TradeAccountsType:
         """Returns the account information.
 
         The account is defined by the acc_num used in constructor.
 
         Returns:
-            _TradeAccountsType: The account details
+            TradeAccountsType: The account details
         """
         route_url = f"{self._base_url}/trade/accounts"
 
         response_json = self._request_get(route_url)
 
         trade_accounts: TradeAccountsType = get_nested_key(
             response_json, ["d"], TradeAccountsType
@@ -762,16 +843,16 @@
         all_executions = pd.DataFrame(
             get_nested_key(response_json, ["d", "executions"]), columns=column_names
         )
         self._apply_typing(all_executions, ExecutionsColumns)
 
         return all_executions
 
-    @log_func
     @lru_cache(maxsize=1)
+    @log_func
     def get_all_instruments(self) -> pd.DataFrame:
         """Returns all available instruments for account.
 
         Returns:
             pd.DataFrame[InstrumentsColumnsTypes]: DataFrame with all available instruments
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/instruments"
@@ -878,18 +959,18 @@
     def get_instrument_details(
         self, instrument_id: int, locale: LocaleType = "en"
     ) -> InstrumentDetailsType:
         """Returns instrument details for a given instrument Id.
 
         Args:
             instrument_id (int): The instrument Id
-            locale (_LocaleType, optional): Locale (language) id. Defaults to "en".
+            locale (LocaleType, optional): Locale (language) id. Defaults to "en".
 
         Returns:
-            _InstrumentDetailsType: The instrument details
+            InstrumentDetailsType: The instrument details
         """
         route_url = f"{self._base_url}/trade/instruments/{instrument_id}"
 
         params: RequestsMappingType = self._get_params(
             {"routeId": self._get_info_route_id(instrument_id), "locale": locale}
         )
 
@@ -904,15 +985,15 @@
     def get_session_details(self, session_id: int) -> SessionDetailsType:
         """Returns details about the session defined by session_id.
 
         Args:
             session_id (int): Session id
 
         Returns:
-            _SessionDetailsType: Session details
+            SessionDetailsType: Session details
         """
         route_url = f"{self._base_url}/trade/sessions/{session_id}"
 
         response_json = self._request_get(route_url)
         session_details: SessionDetailsType = get_nested_key(
             response_json, ["d"], SessionDetailsType
         )
@@ -925,15 +1006,15 @@
     ) -> SessionStatusDetailsType:
         """Returns details about the session status.
 
         Args:
             session_status_id (int): Session id
 
         Returns:
-            _SessionStatusDetailsType: Session details
+            SessionStatusDetailsType: Session details
         """
         route_url = f"{self._base_url}/trade/sessionStatuses/{session_status_id}"
 
         response_json = self._request_get(route_url)
         session_status_details: SessionStatusDetailsType = get_nested_key(
             response_json, ["d"], SessionStatusDetailsType
         )
@@ -949,15 +1030,15 @@
         """Returns daily candle data for requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
             bar_type (Literal[BID, ASK, TRADE], optional): The type of candle data to return. Defaults to "ASK".
 
         Returns:
-            _DailyBarType: Daily candle data
+            DailyBarType: Daily candle data
         """
         route_url = f"{self._base_url}/trade/dailyBar"
 
         params: RequestsMappingType = self._get_params(
             {
                 "tradableInstrumentId": instrument_id,
                 "routeId": self._get_info_route_id(instrument_id),
@@ -975,15 +1056,15 @@
     def get_market_depth(self, instrument_id: int) -> MarketDepthlistType:
         """Returns market depth information for the requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
-            _MarketDepthlistType: Market depth data
+            MarketDepthlistType: Market depth data
         """
         route_url = f"{self._base_url}/trade/depth"
 
         params: RequestsMappingType = self._get_params(
             {
                 "tradableInstrumentId": instrument_id,
                 "routeId": self._get_info_route_id(instrument_id),
@@ -1006,15 +1087,15 @@
         start_timestamp: int = 0,  # timestamps are in miliseconds!
         end_timestamp: int = 0,
     ) -> pd.DataFrame:
         """Returns price history data for the requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
-            resolution (_ResolutionType, optional): Data resolution. Defaults to "15m".
+            resolution (ResolutionType, optional): Data resolution. Defaults to "15m".
             lookback_period (str, optional): Lookback period (for example "5m"). Defaults to "".
             start_timestamp (int, optional): Start timestamp (in ms). Defaults to 0.
             end_timestamp: (int, optional): End timestamp (in ms). Defaults to 0.
 
         Raises:
             ValueError: Will be raised on a invalid response
 
@@ -1024,17 +1105,17 @@
         route_url = f"{self._base_url}/trade/history"
 
         start_timestamp, end_timestamp = resolve_lookback_and_timestamps(
             lookback_period, start_timestamp, end_timestamp
         )
 
         history_size = estimate_history_size(start_timestamp, end_timestamp, resolution)
-        if history_size > _MAX_HISTORY_ROWS:
+        if history_size > self._get_max_history_rows():
             raise ValueError(
-                f"No. of requested rows ({history_size}) larger than max allowed ({_MAX_HISTORY_ROWS})."
+                f"No. of requested rows ({history_size}) larger than max allowed ({self._get_max_history_rows()})."
                 "Try splitting your request in smaller chunks."
             )
 
         params: RequestsMappingType = self._get_params(
             {
                 "tradableInstrumentId": instrument_id,
                 "routeId": self._get_info_route_id(instrument_id),
@@ -1060,15 +1141,14 @@
 
         self._apply_typing(bar_details, PriceHistoryColumns)
 
         return bar_details
 
     @log_func
     @tl_typechecked
-    # TODO: should be replaced with "get_latest_asking_price"
     def get_latest_asking_price(self, instrument_id: int) -> float:
         """Returns latest price informations for requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
@@ -1085,15 +1165,15 @@
     def get_quotes(self, instrument_id: int) -> QuotesType:
         """Returns price quotes for requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
-            _QuotesType: Price quotes for instrument
+            QuotesType: Price quotes for instrument
         """
         route_url = f"{self._base_url}/trade/quotes"
 
         params: RequestsMappingType = self._get_params(
             {
                 "tradableInstrumentId": instrument_id,
                 "routeId": self._get_info_route_id(instrument_id),
@@ -1112,15 +1192,15 @@
         """Closes opposite orders (smallest first) to net against the new order.
 
         Sorts the opposite orders by quantity (ascending) and closes them one by one until
         the total quantity of the new order is netted.
 
         Args:
             instrument_id (int): Instrument Id
-            new_position_side (_SideType): Side to which we want to increase the position
+            new_position_side (SideType): Side to which we want to increase the position
             quantity (float): Order size
 
         Returns:
             float: Total amount that was netted
 
         """
         opposite_side: str = "sell" if (new_position_side == "buy") else "buy"
@@ -1166,30 +1246,32 @@
         instrument_id: int,
         quantity: float,
         side: SideType,
         price: float = 0,
         type_: OrderTypeType = "market",
         validity: Optional[ValidityType] = None,
         position_netting: bool = False,
-        position_id: int = 0,
-    ) -> int | str:
+        stop_loss: Optional[float] = None,
+        take_profit: Optional[float] = None,
+    ) -> Optional[int]:
         """Creates an order.
 
         Args:
             instrument_id (int): Instrument Id
             quantity (float): Order size
-            side (_SideType): Order side
+            side (SideType): Order side
             price (float, optional): Price for non-market orders. Defaults to 0.
-            type_ (_OrderTypeType, optional): Order type. Defaults to "market".
-            validity (_ValidityType, optional): Validity type of order. Defaults to "IOC".
+            type_ (OrderTypeType, optional): Order type. Defaults to "market".
+            validity (ValidityType, optional): Validity type of order. Defaults to "IOC".
             position_netting (bool, optional): Should position netting be used. Defaults to False.
-            position_id (int, optional): Position Id. Defaults to 0.
+            stop_loss (float, optional): Stop Loss. Defaults to None.
+            take_profit (float, optional): Take Profit. Defaults to None.
 
         Returns:
-            int|str: order_id or "" if order could not be placed
+            Optional[int]: order_id or None if order could not be placed
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/orders"
 
         if type_ == "market" and price != 0:
             self.log.warning("Price specified for a market order. Ignoring the price.")
             price = 0
 
@@ -1232,45 +1314,45 @@
             )
 
         # If the quantity is smaller than the minimum lot size, return
         if quantity < _MIN_LOT_SIZE:
             self.log.warning(
                 "Unable to place an order with quantity smaller than min lot size of {_MIN_LOT_SIZE}"
             )
-            return ""
+            return None
 
         request_body: dict[str, str] = {
             "price": str(price),
             "qty": str(quantity),
             "routeId": self._get_trade_route_id(instrument_id),
             "side": side,
             "validity": validity,
             "tradableInstrumentId": str(instrument_id),
             "type": type_,
+            "stopLoss": stop_loss,
+            "takeProfit": take_profit,
         }
 
-        if position_id != 0:
-            request_body["positionId"] = position_id
-        elif position_netting:
+        if position_netting:
             # Try finding opposite orders to net against
-            if type_ != "market":
-                self.log.warning(
-                    "Order netting is only supported for market orders. Continuing without netting."
-                )
-            else:
+            if type_ == "market":
                 total_netted = self._perform_order_netting(
                     instrument_id, side, quantity
                 )
                 # Reduce the necessary quantity by the total_amount that was netted
                 request_body["qty"] = str(float(request_body["qty"]) - total_netted)
                 if float(request_body["qty"]) < _MIN_LOT_SIZE:
                     self.log.info(
                         "Not placing a new order after closing sufficient opposite orders due to netting."
                     )
-                    return ""
+                    return None
+            else:
+                self.log.warning(
+                    "Order netting is only supported for market orders. Continuing without netting."
+                )
 
         # Place the order
         response = requests.post(
             url=route_url,
             headers=self._get_headers({"Content-type": "application/json"}),
             json=request_body,
             timeout=_TIMEOUT,
@@ -1278,15 +1360,15 @@
         response_json = self._get_response_json(response)
         try:
             order_id: int = int(get_nested_key(response_json, ["d", "orderId"], str))
             self.log.info(f"Order {request_body} placed with order_id: {order_id}")
             return order_id
         except KeyError as err:
             self.log.error(f"Unable to place order {request_body}. Error: {err}")
-            return ""
+            return None
 
     @log_func
     @tl_typechecked
     def delete_order(self, order_id: int) -> bool:
         """Deletes a pending order.
 
         Args:
@@ -1310,23 +1392,22 @@
         self.log.info(f"Order deletion response: {response.json()}")
         response_status: str = get_nested_key(response_json, ["s"], str)
 
         return response_status == "ok"
 
     @log_func
     @tl_typechecked
-    # TODO: this should probably be further expanded / validated
     def modify_order(
         self, order_id: int, modification_params: ModificationParamsType
     ) -> bool:
-        """Modifies a pending order.
+        """Modifies a pending order -- a thin wrapper around PATCH /trade/orders/{order_id}.
 
         Args:
             order_id (int): Order Id
-            modification_params (_ModificationParamsType): Order modification details
+            modification_params (ModificationParamsType): Order modification details
 
         Returns:
             bool: True on success, False on error
         """
         route_url = f"{self._base_url}/trade/orders/{order_id}"
 
         self.log.info(f"Modifying the order with id {order_id}")
```

### Comparing `tradelocker-0.39.0/src/tradelocker/types.py` & `tradelocker-0.40.0/src/tradelocker/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,28 @@
     "accountDetailsConfig",
 ]
 ConfigColumnType: TA = list[dict[Literal["id", "description"], str]]
 ColumnConfigValuesType: TA = (
     dict[Literal["id", "title"], str] | dict[Literal["columns"], ConfigColumnType]
 )
 
+LimitsType: TA = dict[Literal["limitType", "limit"], str | int | float]
+RateLimitsType: TA = dict[
+    Literal["rateLimitType", "measure", "intervalNum", "limit"],
+    str | int | float,
+]
+
 ConfigType: TA = (
     dict[Literal["customerAccess"], dict[str, bool]]
     | dict[ColumnConfigKeysType, ColumnConfigValuesType]
+    | dict[Literal["limits"], list[LimitsType]]
+    | dict[
+        Literal["rateLimits"],
+        list[RateLimitsType],
+    ]
 )
 
 ResolutionType: TA = Literal["1M", "1W", "1D", "4H", "1H", "30m", "15m", "5m", "1m"]
 ModificationParamsType: TA = dict[
     str, str | StopLossType | TakeProfitType | ValidityType
 ]
 LocaleType: TA = Literal[
```

### Comparing `tradelocker-0.39.0/src/tradelocker/utils.py` & `tradelocker-0.40.0/src/tradelocker/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,76 +57,78 @@
         "debug": logging.DEBUG,
         "info": logging.INFO,
         "warning": logging.WARNING,
         "error": logging.ERROR,
         "critical": logging.CRITICAL,
     }
 
-    def __init__(self, module_name: str, log_level: LogLevelType = "debug"):
-        self.module_name = module_name
-        self.log_level = log_level
+    def __init__(self, log_level: LogLevelType = "debug"):
+        self.logger = logging.getLogger()
 
-        logger = logging.getLogger(module_name)
-
-        if log_level not in self.LOG_LEVELS.keys():
-            raise ValueError(
-                f"log_level ({log_level}) not among {list(self.LOG_LEVELS.keys())}"
-            )
-
-        logger.setLevel(self.LOG_LEVELS[log_level])
+        # remove all handlers from the new logger
+        for handler in self.logger.handlers[:]:
+            self.logger.removeHandler(handler)
 
         handler = logging.StreamHandler()
         handler.setFormatter(
             colorlog.ColoredFormatter(
-                f"%(log_color)s \n[%(levelname)s] {module_name} %(asctime)s %(module)s %(funcName)s: %(lineno)d %(message)s",
+                f"%(log_color)s [%(levelname)s %(asctime)s %(name)s.%(module)s.%(funcName)s:%(lineno)d]: %(message)s",
                 datefmt=None,
                 reset=True,
                 log_colors={
                     "DEBUG": "thin_white",
                     "INFO": "green",
                     "WARNING": "yellow",
                     "ERROR": "red",
                     "CRITICAL": "red,bg_white",
                 },
                 secondary_log_colors={},
                 style="%",
             )
         )
 
-        logger.addHandler(handler)
-        self.logger = logger
+        self.logger.addHandler(handler)
+        self.set_log_level(log_level)
 
     def get_logger(self) -> logging.Logger:
         return self.logger
 
+    def set_log_level(self, log_level: LogLevelType) -> None:
+        if log_level not in self.LOG_LEVELS.keys():
+            raise ValueError(
+                f"log_level ({log_level}) not among {list(self.LOG_LEVELS.keys())}"
+            )
+
+        self.logger.setLevel(self.LOG_LEVELS[log_level])
+
+
+color_logger = ColorLogger(log_level="debug").get_logger()
+
 
 # This decorator logs the function call and its arguments
 def log_func(func: Callable[..., RT]) -> Callable[..., RT]:
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> RT:
         args_repr = [repr(a) for a in args]
         kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]
         signature = ", ".join(args_repr + kwargs_repr)
 
-        # TODO: using ColorLogger does not work -- debugging needed
-        # log = args[0].log
-        # log.debug(f"**** CALLING {func.__name__}({signature})")
-        # print(f"**** CALLING {func.__name__}({signature})")
+        log = args[0].log
+        log.debug(f"**** CALLING {func.__name__}({signature})")
 
         return_value = func(*args, **kwargs)
 
         max_return_string_length = 1000
         return_string = repr(return_value)
         if len(return_string) > max_return_string_length:
             return_string = (
                 return_string[:max_return_string_length]
                 + "    ...   ===<< TRUNCATED DUE TO LENGTH >>===   "
             )
-        # print(f"**** RETURN from {func.__name__}({signature}):\n{return_string}")
-        # log.debug(f"**** RETURN from {func.__name__}({signature}):\n{return_string}")
+        log.debug(f"**** RETURN from {func.__name__}({signature}):\n{return_string}")
 
         return return_value
 
     return cast(Callable[..., RT], wrapper)
 
 
 def retry(func: Callable[..., RT], delay: float = 1) -> Callable[..., RT]:
@@ -214,21 +216,21 @@
         )
 
     if start_timestamp != 0 and end_timestamp != 0 and start_timestamp <= end_timestamp:
         return start_timestamp, end_timestamp
 
     try:
         start_timestamp, end_timestamp = timestamps_from_lookback(lookback_period)
-        # ColorLogger(__name__, "debug").get_logger(__name__, "debug").warning(
+        # color_logger.warning(
         #     "Both valid lookback_period and start_timestamp/end_timestamp were provided.\n"
         #     "Continuing with only the start_timestamp/end_timestamp"
         # )
     except Exception as err:
         pass
-        # ColorLogger(__name__, "debug").get_logger(__name__, "debug").warning(
+        # color_logger.warning(
         #     f"Invalid lookback_period provided: {err}\nContinuing with only the start_timestamp/end_timestamp"
         # )
 
     return start_timestamp, end_timestamp
 
 
 @tl_typechecked
@@ -239,25 +241,29 @@
     coeff = int(resolution[:-1]) * RESOLUTION_COEFF_MS[resolution[-1]]
     total_bars: int = int(total_miliseconds / coeff)
     return total_bars
 
 
 @tl_typechecked
 def time_to_token_expiry(access_token: str) -> float:
-    # TODO: start verifying the signature
+    if not access_token:
+        logging.warning(f"invalid access token: |{access_token}|")
+        return 0
+
+    # No explicit need to verify the signature as there is a direct https connection between the client and the server
     decoded_payload: dict[str, Any] = jwt.decode(
         access_token, options={"verify_signature": False}
     )
     expiration_time: float = decoded_payload["exp"]
     remaining_time: float = expiration_time - datetime.datetime.now().timestamp()
     return remaining_time
 
 
 @tl_typechecked
-# Should be called with    callers_file = __file__
+# Should be called with callers_file = __file__
 def load_env_config(callers_file: str, backup_env_file=".env") -> dict[str, str | int]:
     # Get the current script's directory
     basedir = os.path.abspath(os.path.dirname(callers_file))
 
     env_var_name = "ENV_FILE_PATH"
 
     # read the "$(env_var_name)" environment variable if it exists, otherwise use .env or .env-test
```

### Comparing `tradelocker-0.39.0/PKG-INFO` & `tradelocker-0.40.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradelocker
-Version: 0.39.0
+Version: 0.40.0
 Summary: TradeLocker Trading API support for Python
 License: MIT
 Keywords: tradelocker,api,rest,trading,exchange,algotrading,algo,bots,strategies
 Author: TradeLocker
 Author-email: admin@tradelocker.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyJWT (==2.8.0)
 Requires-Dist: Requests (==2.31.0)
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: pandas (==2.1.1)
 Requires-Dist: python-dotenv (==1.0.0)
-Requires-Dist: typeguard (==4.1.5)
 Project-URL: Issues, https://github.com/tradelocker/tradelocker-python/issues
 Project-URL: Source, https://github.com/tradelocker/tradelocker-python/
 Description-Content-Type: text/markdown
 
 # TradeLocker Python API Wrapper
 
 This project provides a Python wrapper for TradeLocker's public API. It simplifies the process of making requests to the API by providing Pythonic interfaces.
```

