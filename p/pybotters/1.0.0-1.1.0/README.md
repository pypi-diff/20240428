# Comparing `tmp/pybotters-1.0.0.tar.gz` & `tmp/pybotters-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotters-1.0.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pybotters-1.0.0.tar` & `pybotters-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,68 @@
--rw-r--r--   0        0        0     8462 2024-01-31 11:54:15.876526 pybotters-1.0.0/README.md
--rw-r--r--   0        0        0     1460 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/__init__.py
--rw-r--r--   0        0        0    17237 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/auth.py
--rw-r--r--   0        0        0    10844 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/client.py
--rw-r--r--   0        0        0        0 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/__init__.py
--rw-r--r--   0        0        0    31567 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/binance.py
--rw-r--r--   0        0        0     3919 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/bitbank.py
--rw-r--r--   0        0        0    16374 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/bitflyer.py
--rw-r--r--   0        0        0     9356 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/bitget.py
--rw-r--r--   0        0        0     4349 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/bitmex.py
--rw-r--r--   0        0        0    11398 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/bybit.py
--rw-r--r--   0        0        0     3627 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/coincheck.py
--rw-r--r--   0        0        0     8305 2024-01-31 11:54:15.880526 pybotters-1.0.0/pybotters/models/gmocoin.py
--rw-r--r--   0        0        0    25507 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/models/kucoin.py
--rw-r--r--   0        0        0    20486 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/models/legacy/gmocoin.py
--rw-r--r--   0        0        0    14133 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/models/okx.py
--rw-r--r--   0        0        0    11654 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/models/phemex.py
--rw-r--r--   0        0        0     1396 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/request.py
--rw-r--r--   0        0        0    12718 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/store.py
--rw-r--r--   0        0        0      309 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/typedefs.py
--rw-r--r--   0        0        0    24022 2024-01-31 11:54:15.884526 pybotters-1.0.0/pybotters/ws.py
--rw-r--r--   0        0        0     1424 2024-01-31 11:54:15.884526 pybotters-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9780 1970-01-01 00:00:00.000000 pybotters-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pybotters-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 pybotters-1.1.0/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/release.yml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pybotters-1.1.0/.vscode/extensions.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pybotters-1.1.0/.vscode/hatch_config.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pybotters-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/advanced.rst
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/contributing.rst
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/examples.rst
+-rw-r--r--   0        0        0    16099 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/exchanges.rst
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/favicon.ico
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0    52834 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/logo.png
+-rw-r--r--   0        0        0    16737 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/logo_150.png
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/reference.rst
+-rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/user-guide.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/binance.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bitbank.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bitflyer.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bitget.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bybit.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/coincheck.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/gmocoin.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/kucoin.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/okx.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/phemex.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/requirements.txt
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/trading-bot/bitflyer.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/__version__.py
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/auth.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/client.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/request.py
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/store.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/typedefs.py
+-rw-r--r--   0        0        0    25768 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/ws.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/__init__.py
+-rw-r--r--   0        0        0    31433 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/binance.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitbank.py
+-rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitflyer.py
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitget.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitmex.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bybit.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/coincheck.py
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/gmocoin.py
+-rw-r--r--   0        0        0    25200 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/kucoin.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/okx.py
+-rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/phemex.py
+-rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/legacy/gmocoin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    43212 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_auth.py
+-rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_client.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_request.py
+-rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_store.py
+-rw-r--r--   0        0        0    45820 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_ws.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pybotters-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pybotters-1.1.0/LICENCE
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pybotters-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 pybotters-1.1.0/PKG-INFO
```

### Comparing `pybotters-1.0.0/README.md` & `pybotters-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [
   ![PyPI](https://img.shields.io/pypi/v/pybotters)
   ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pybotters)
   ![PyPI - License](https://img.shields.io/pypi/l/pybotters)
 ](https://pypi.org/project/pybotters/)
 [![Downloads](https://static.pepy.tech/badge/pybotters)](https://pepy.tech/project/pybotters)
 
-[![pytest](https://github.com/pybotters/pybotters/actions/workflows/pytest.yml/badge.svg)](https://github.com/pybotters/pybotters/actions/workflows/pytest.yml)
+[![CI](https://github.com/pybotters/pybotters/actions/workflows/ci.yml/badge.svg)](https://github.com/pybotters/pybotters/actions/workflows/ci.yml)
 [![publish](https://github.com/pybotters/pybotters/actions/workflows/publish.yml/badge.svg)](https://github.com/pybotters/pybotters/actions/workflows/publish.yml)
 [![codecov](https://codecov.io/gh/pybotters/pybotters/graph/badge.svg?token=ARR29R726W)](https://codecov.io/gh/pybotters/pybotters)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/pybotters/badge/?version=latest)](https://pybotters.readthedocs.io/ja/latest/?badge=latest)
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/pybotters/pybotters?style=social)](https://github.com/pybotters/pybotters/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/pybotters/pybotters?style=social)](https://github.com/pybotters/pybotters/network/members)
 [![Discord](https://img.shields.io/discord/832651305155297331?label=Discord&logo=discord&style=social)](https://discord.com/invite/CxuWSX9U69)
 [![GitHub Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23db61a2.svg?&logo=github&logoColor=181717&&style=flat-square&labelColor=white)](https://github.com/sponsors/MtkN1)
 
 
 # pybotters
 
-![pybotters logo](docs/logo_150.png)
+![pybotters logo](https://raw.githubusercontent.com/pybotters/pybotters/main/docs/logo_150.png)
 
 An advanced API client for python botters. This project is in Japanese.
 
 ## 📌 Description
 
 `pybotters` is a Python library for [仮想通貨 botter (crypto bot traders)](https://medium.com/perpdex/botter-the-crypto-bot-trader-in-japan-2f5f2a65856f).
```

### Comparing `pybotters-1.0.0/pybotters/__init__.py` & `pybotters-1.1.0/pybotters/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from __future__ import annotations
 
-from importlib.metadata import version
-
-__version__ = version(__package__)
-
+from .__version__ import __version__
 from .auth import Auth
 from .client import Client, FetchResult, NotJSONContent
 from .models.binance import (
     BinanceCOINMDataStore,
     BinanceSpotDataStore,
     BinanceUSDSMDataStore,
 )
@@ -21,14 +18,16 @@
 from .models.kucoin import KuCoinDataStore
 from .models.okx import OKXDataStore
 from .models.phemex import PhemexDataStore
 from .store import DataStore, DataStoreCollection, StoreChange, StoreStream
 from .ws import WebSocketApp, WebSocketQueue
 
 __all__: tuple[str, ...] = (
+    # version
+    "__version__",
     # client
     "Client",
     "FetchResult",
     "NotJSONContent",
     # ws
     "WebSocketApp",
     "WebSocketQueue",
```

### Comparing `pybotters-1.0.0/pybotters/auth.py` & `pybotters-1.1.0/pybotters/auth.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/client.py` & `pybotters-1.1.0/pybotters/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dataclasses import dataclass
 from typing import Any, Literal, Mapping
 
 import aiohttp
 from aiohttp import hdrs
 from aiohttp.client import _RequestContextManager
 
-from . import __version__
+from .__version__ import __version__
 from .auth import Auth
 from .request import ClientRequest
 from .typedefs import WsBytesHandler, WsJsonHandler, WsStrHandler
 from .ws import ClientWebSocketResponse, WebSocketApp
 
 logger = logging.getLogger(__name__)
 
@@ -237,14 +237,15 @@
         send_str: str | list[str] | None = None,
         send_bytes: bytes | list[bytes] | None = None,
         send_json: dict | list[dict] | None = None,
         hdlr_str: WsStrHandler | list[WsStrHandler] | None = None,
         hdlr_bytes: WsBytesHandler | list[WsBytesHandler] | None = None,
         hdlr_json: WsJsonHandler | list[WsJsonHandler] | None = None,
         backoff: tuple[float, float, float, float] = WebSocketApp._DEFAULT_BACKOFF,
+        autoping: bool = True,
         heartbeat: float = 10.0,
         auth: Auth | None = Auth,
         **kwargs: Any,
     ) -> WebSocketApp:
         """WebSocket request.
 
         Args:
@@ -252,14 +253,15 @@
             send_str: 送信する WebSocket メッセージ (文字列)
             send_bytes: 送信する WebSocket メッセージ (バイト)
             send_json: 送信する WebSocket メッセージ (JSON)
             hdlr_str: WebSocket メッセージをハンドリングするコールバック (文字列)
             hdlr_bytes: WebSocket メッセージをハンドリングするコールバック (バイト)
             hdlr_json: WebSocket メッセージをハンドリングするコールバック (JSON)
             backoff: 再接続の指数バックオフ (最小、最大、係数、初期値)
+            autoping: Ping に対する自動 Pong 応答 (デフォルト True)
             heartbeat: WebSocket ハートビート (デフォルト 10.0 秒)
             auth: 認証オプション (デフォルトで有効、None で無効)
             **kwargs: aiohttp.ClientSession.ws_connect にバイパスされる引数
 
         Returns:
             WebSocketApp
 
@@ -271,14 +273,15 @@
             send_str=send_str,
             send_bytes=send_bytes,
             send_json=send_json,
             hdlr_str=hdlr_str,
             hdlr_bytes=hdlr_bytes,
             hdlr_json=hdlr_json,
             backoff=backoff,
+            autoping=autoping,
             heartbeat=heartbeat,
             auth=auth,
             **kwargs,
         )
 
     @staticmethod
     def _load_apis(apis: dict[str, list[str]] | str | None) -> dict[str, list[str]]:
```

### Comparing `pybotters-1.0.0/pybotters/models/binance.py` & `pybotters-1.1.0/pybotters/models/binance.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         - GET /fapi/v2/balance, /dapi/v1/balance (:attr:`.BinanceCOINMDataStore.balance`)
         - GET /fapi/v2/positionRisk, /dapi/v1/positionRisk (:attr:`.BinanceCOINMDataStore.position`)
 
         USDⓈ-M
         - GET /fapi/v1/indexInfo (:attr:`.BinanceUSDSMDataStore.compositeindex`)
 
 
-        """  # noqa
+        """
         for f in asyncio.as_completed(aws):
             resp = await f
             data = await resp.json()
             endpoint = resp.url.path
             if self._is_target_endpoint(self._ORDERBOOK_INIT_ENDPOINT, endpoint):
                 self._initialize_orderbook(resp, data)
             elif self._is_target_endpoint(self._ORDER_INIT_ENDPOINT, endpoint):
@@ -191,28 +191,28 @@
         * Spot
             * https://binance-docs.github.io/apidocs/spot/en/#aggregate-trade-streams
             * https://binance-docs.github.io/apidocs/spot/en/#trade-streams
         * USDⓈ-M
             * https://binance-docs.github.io/apidocs/futures/en/#aggregate-trade-streams
         * COIN-M
             * https://binance-docs.github.io/apidocs/delivery/en/#aggregate-trade-streams
-        """  # noqa: E501
+        """
         return self._get("trade", Trade)
 
     @property
     def kline(self) -> "Kline":
         """kline stream.
 
         * Spot
             * https://binance-docs.github.io/apidocs/spot/en/#kline-candlestick-streams
         * USDⓈ-M
             * https://binance-docs.github.io/apidocs/futures/en/#kline-candlestick-streams
         * COIN-M
             * https://binance-docs.github.io/apidocs/delivery/en/#kline-candlestick-streams
-        """  # noqa: E501
+        """
         return self._get("kline", Kline)
 
     @property
     def ticker(self) -> "Ticker":
         """24hrMiniTicker/24hrTicker stream.
 
         * Spot
@@ -220,41 +220,41 @@
             * https://binance-docs.github.io/apidocs/spot/en/#individual-symbol-ticker-streams
         * USDⓈ-M
             * https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-mini-ticker-stream
             * https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-ticker-streams
         * COIN-M
             * https://binance-docs.github.io/apidocs/delivery/en/#individual-symbol-mini-ticker-stream
             * https://binance-docs.github.io/apidocs/delivery/en/#individual-symbol-ticker-streams
-        """  # noqa: E501
+        """
         return self._get("ticker", Ticker)
 
     @property
     def bookticker(self) -> "BookTicker":
         """bookTicker stream.
 
         * Spot
             * https://binance-docs.github.io/apidocs/spot/en/#individual-symbol-book-ticker-streams
         * USDⓈ-M
             * https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-book-ticker-streams
         * COIN-M
             * https://binance-docs.github.io/apidocs/delivery/en/#individual-symbol-book-ticker-streams
-        """  # noqa: E501
+        """
         return self._get("bookticker", BookTicker)
 
     @property
     def orderbook(self) -> "OrderBook":
         """depthUpdate stream.
 
         * Spot
             * https://binance-docs.github.io/apidocs/spot/en/#diff-depth-stream
         * USDⓈ-M
             * https://binance-docs.github.io/apidocs/futures/en/#diff-book-depth-streams
         * COIN-M
             * https://binance-docs.github.io/apidocs/delivery/en/#diff-book-depth-streams
-        """  # noqa: E501
+        """
         return self._get("orderbook", OrderBook)
 
     @property
     def order(self) -> "Order":
         """executionReport/ORDER_TRADE_UPDATE from User Data Streams.
 
         アクティブオーダーのみデータが格納されます。 キャンセル、約定済みなどは削除されます。
@@ -335,42 +335,42 @@
 
     @property
     def continuouskline(self) -> "ContinuousKline":
         """continuous_kline stream.
 
         * https://binance-docs.github.io/apidocs/futures/en/#continuous-contract-kline-candlestick-data
         * https://binance-docs.github.io/apidocs/delivery/en/#continuous-contract-kline-candlestick-data
-        """  # noqa: E501
+        """
         return self._get("continuouskline", ContinuousKline)
 
     @property
     def liquidation(self) -> "Liquidation":
         """forceOrder stream.
 
         * https://binance-docs.github.io/apidocs/futures/en/#liquidation-order-streams
         * https://binance-docs.github.io/apidocs/delivery/en/#all-market-liquidation-order-streams
-        """  # noqa: E501
+        """
         return self._get("liquidation", Liquidation)
 
     @property
     def balance(self) -> "Balance":
         """ACCOUNT_UPDATE from User Data Streams.
 
         * https://binance-docs.github.io/apidocs/futures/en/#event-balance-and-position-update
         * https://binance-docs.github.io/apidocs/delivery/en/#event-balance-and-position-update
-        """  # noqa: E501
+        """
         return self._get("balance", Balance)
 
     @property
     def position(self) -> "Position":
         """ACCOUNT_UPDATE from User Data Streams.
 
         * https://binance-docs.github.io/apidocs/futures/en/#event-balance-and-position-update
         * https://binance-docs.github.io/apidocs/delivery/en/#event-balance-and-position-update
-        """  # noqa: E501
+        """
         return self._get("position", Position)
 
 
 class BinanceSpotDataStore(BinanceDataStoreBase):
     """Binance Spot の DataStoreCollection クラス"""
 
     _ORDERBOOK_INIT_ENDPOINT = "/api/v3/depth"
```

### Comparing `pybotters-1.0.0/pybotters/models/bitbank.py` & `pybotters-1.1.0/pybotters/models/bitbank.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,32 +28,32 @@
                 self.ticker._onmessage(room_name, data)
 
     @property
     def transactions(self) -> "Transactions":
         """transactions channel.
 
         https://github.com/bitbankinc/bitbank-api-docs/blob/master/public-stream.md#transactions
-        """  # noqa: E501
+        """
         return self._get("transactions", Transactions)
 
     @property
     def depth(self) -> "Depth":
         """depth channel.
 
         * https://github.com/bitbankinc/bitbank-api-docs/blob/master/public-stream.md#depth-diff
         * https://github.com/bitbankinc/bitbank-api-docs/blob/master/public-stream.md#depth-whole
-        """  # noqa: E501
+        """
         return self._get("depth", Depth)
 
     @property
     def ticker(self) -> "Ticker":
         """ticker channel.
 
         https://github.com/bitbankinc/bitbank-api-docs/blob/master/public-stream.md#ticker
-        """  # noqa: E501
+        """
         return self._get("ticker", Ticker)
 
 
 class Transactions(DataStore):
     _MAXLEN = 99999
 
     def _onmessage(self, room_name: str, data: list[Item]) -> None:
```

### Comparing `pybotters-1.0.0/pybotters/models/bitflyer.py` & `pybotters-1.1.0/pybotters/models/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/models/bitget.py` & `pybotters-1.1.0/pybotters/models/bitget.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/models/bitmex.py` & `pybotters-1.1.0/pybotters/models/bitmex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/models/bybit.py` & `pybotters-1.1.0/pybotters/models/bybit.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,27 @@
                     f"URL: {resp.url}\n"
                     f"Data: {data}"
                 )
 
             if resp.url.path in self._MAP_PATH_TOPIC:
                 topic = self._MAP_PATH_TOPIC[resp.url.path]
                 if topic in self:
-                    getattr(self[topic], "_onresponse")(resp.url, data)
+                    self[topic]._onresponse(resp.url, data)
 
     def _onmessage(self, msg: Item, ws: ClientWebSocketResponse) -> None:
         if "success" in msg:
             if not msg["success"]:
                 logger.warning(msg)
 
         if "topic" in msg:
             dot_topic: str = msg["topic"]
             topic, *topic_ext = dot_topic.split(".")
 
             if topic in self:
-                getattr(self[topic], "_onmessage")(msg, topic_ext)
+                self[topic]._onmessage(msg, topic_ext)
 
     @property
     def orderbook(self) -> "OrderBook":
         """orderbook topic.
 
         https://bybit-exchange.github.io/docs/v5/websocket/public/orderbook
         """
@@ -249,24 +249,21 @@
 class Liquidation(DataStore):
     _MAXLEN = 99999
 
     def _onmessage(self, msg: Item, topic_ext: list[str]) -> None:
         self._insert([msg["data"]])
 
 
-class LTKline(Kline):
-    ...
+class LTKline(Kline): ...
 
 
-class LTTicker(Ticker):
-    ...
+class LTTicker(Ticker): ...
 
 
-class LTNav(Ticker):
-    ...
+class LTNav(Ticker): ...
 
 
 class Position(DataStore):
     _KEYS = ["symbol", "positionIdx"]
 
     def _onresponse(self, url: URL, data: Item) -> None:
         self._update(data["result"]["list"])
```

### Comparing `pybotters-1.0.0/pybotters/models/coincheck.py` & `pybotters-1.1.0/pybotters/models/coincheck.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/models/gmocoin.py` & `pybotters-1.1.0/pybotters/models/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/models/kucoin.py` & `pybotters-1.1.0/pybotters/models/kucoin.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     @property
     def ticker(self) -> "Ticker":
         """/market/ticker, /contractMarket/tickerV2, /contractMarket/ticker topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/public-channels/ticker
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/get-ticker-v2
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/get-ticker
-        """  # noqa: E501
+        """
         return self._get("ticker", Ticker)
 
     @property
     def kline(self) -> "Kline":
         """/market/candles topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/public-channels/klines
@@ -164,172 +164,172 @@
         return self._get("kline", Kline)
 
     @property
     def symbolsnapshot(self) -> "SymbolSnapshot":
         """/market/snapshot topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/public-channels/symbol-snapshot
-        """  # noqa: E501
+        """
         return self._get("symbolsnapshot", SymbolSnapshot)
 
     @property
     def orderbook5(self) -> "TopKOrderBook":
         """/spotMarket/level2Depth50, /contractMarket/level2Depth5 topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/public-channels/level2-5-best-ask-bid-orders
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/level2-5-best-ask-bid-orders
-        """  # noqa: E501
+        """
         return self._get("orderbook5", TopKOrderBook)
 
     @property
     def orderbook50(self) -> "TopKOrderBook":
         """/spotMarket/level2Depth50, /contractMarket/level2Depth50 topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/public-channels/level2-50-best-ask-bid-orders
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/level2-50-best-ask-bid-orders
-        """  # noqa: E501
+        """
         return self._get("orderbook50", TopKOrderBook)
 
     @property
     def execution(self) -> "Execution":
         """/market/match, /contractMarket/execution topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/public-channels/match-execution-data
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/match-execution-data
-        """  # noqa: E501
+        """
         return self._get("execution", Execution)
 
     @property
     def indexprice(self) -> "IndexPrice":
         """/indicator/index topic.
 
         * https://www.kucoin.com/docs/websocket/margin-trading/public-channels/index-price
-        """  # noqa: E501
+        """
         return self._get("indexprice", IndexPrice)
 
     @property
     def markprice(self) -> "MarkPrice":
         """/indicator/markPrice topic.
 
         * https://www.kucoin.com/docs/websocket/margin-trading/public-channels/mark-price
-        """  # noqa: E501
+        """
         return self._get("markprice", MarkPrice)
 
     @property
     def orderevents(self) -> "OrderEvents":
         """/spotMarket/tradeOrders, /spotMarket/advancedOrders, /contractMarket/tradeOrders, /contractMarket/advancedOrders topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/private-channels/private-order-change
         * https://www.kucoin.com/docs/websocket/spot-trading/private-channels/stop-order-event
         * https://www.kucoin.com/docs/websocket/futures-trading/private-channels/trade-orders
         * https://www.kucoin.com/docs/websocket/futures-trading/private-channels/stop-order-lifecycle-event
-        """  # noqa: E501
+        """
         return self._get("orderevents", OrderEvents)
 
     @property
     def orders(self) -> "Orders":
         """tradeOrders/advancedOrders topic.
 
         アクティブオーダーのみデータが格納されます。 キャンセル、約定済みなどは削除されます。
 
         * https://www.kucoin.com/docs/websocket/spot-trading/private-channels/private-order-change
         * https://www.kucoin.com/docs/websocket/spot-trading/private-channels/stop-order-event
         * https://www.kucoin.com/docs/websocket/futures-trading/private-channels/trade-orders
         * https://www.kucoin.com/docs/websocket/futures-trading/private-channels/stop-order-lifecycle-event
-        """  # noqa: E501
+        """
         return self._get("orders", Orders)
 
     @property
     def balance(self) -> "Balance":
         """/account/balance topic.
 
         * https://www.kucoin.com/docs/websocket/spot-trading/private-channels/account-balance-change
-        """  # noqa: E501
+        """
         return self._get("balance", Balance)
 
     @property
     def marginfundingbook(self) -> "MarginFundingBook":
         """/margin/fundingBook topic.
 
         * https://www.kucoin.com/docs/websocket/margin-trading/public-channels/margin-funding-order-book-change
-        """  # noqa: E501
+        """
         return self._get("marginfundingbook", MarginFundingBook)
 
     @property
     def marginpositions(self) -> "MarginPositions":
         """/margin/position topic.
 
         * https://www.kucoin.com/docs/websocket/margin-trading/private-channels/cross-margin-position-event
-        """  # noqa: E501
+        """
         return self._get("marginpositions", MarginPositions)
 
     @property
     def marginpositionevents(self) -> "MarginPositionEvents":
         """/margin/position topic.
 
         * https://www.kucoin.com/docs/websocket/margin-trading/private-channels/cross-margin-position-event
-        """  # noqa: E501
+        """
         return self._get("marginpositionevents", MarginPositionEvents)
 
     @property
     def marginorderevents(self) -> "MarginOrderEvents":
         """/margin/loan topic.
 
         * https://www.kucoin.com/docs/websocket/margin-trading/private-channels/margin-trade-order-event
-        """  # noqa: E501
+        """
         return self._get("marginorderevents", MarginOrderEvents)
 
     @property
     def marginorders(self) -> "MarginOrders":
         """/margin/loan topic.
 
         アクティブオーダーのみデータが格納されます。 キャンセル、約定済みなどは削除されます。
 
         * https://www.kucoin.com/docs/websocket/margin-trading/private-channels/margin-trade-order-event
-        """  # noqa: E501
+        """
         return self._get("marginorders", MarginOrders)
 
     @property
     def instrument(self) -> "Instrument":
         """/contract/instrument topic.
 
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/contract-market-data
-        """  # noqa: E501
+        """
         return self._get("instrument", Instrument)
 
     @property
     def announcements(self) -> "Announcements":
         """/contract/announcement topic.
 
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/funding-fee-settlement
-        """  # noqa: E501
+        """
         return self._get("announcements", Announcements)
 
     @property
     def transactionstats(self) -> "TransactionStats":
         """/contractMarket/snapshot topic.
 
         * https://www.kucoin.com/docs/websocket/futures-trading/public-channels/transaction-statistics-timer-event
-        """  # noqa: E501
+        """
         return self._get("transactionstats", TransactionStats)
 
     @property
     def balanceevents(self) -> "BalanceEvents":
         """/contractAccount/wallet topic.
 
         * https://www.kucoin.com/docs/websocket/futures-trading/private-channels/account-balance-events
-        """  # noqa: E501
+        """
         return self._get("balanceevents", BalanceEvents)
 
     @property
     def positions(self) -> "Positions":
         """/contract/position topic.
 
         * https://www.kucoin.com/docs/websocket/futures-trading/private-channels/position-change-events
-        """  # noqa: E501
+        """
         return self._get("positions", Positions)
 
     @property
     def endpoint(self):
         """Retrieved KuCoin WebSocket endpoint."""
 
         if self._endpoint is None:
@@ -427,16 +427,16 @@
     """
 
     # Spot
     - https://docs.kucoin.com/#level2-5-best-ask-bid-orders
     - https://docs.kucoin.com/#level2-50-best-ask-bid-orders
 
     # Future
-    - https://docs.kucoin.com/futures/message-channel-for-the-5-best-ask-bid-full-data-of-level-2  # noqa: E501
-    - https://docs.kucoin.com/futures/message-channel-for-the-50-best-ask-bid-full-data-of-level-2 # noqa: E501
+    - https://docs.kucoin.com/futures/message-channel-for-the-5-best-ask-bid-full-data-of-level-2
+    - https://docs.kucoin.com/futures/message-channel-for-the-50-best-ask-bid-full-data-of-level-2
     """
 
     _KEYS = ["symbol", "side", "price"]
 
     def __init__(self, *args, **kwargs):
         super(TopKOrderBook, self).__init__(*args, **kwargs)
```

### Comparing `pybotters-1.0.0/pybotters/models/legacy/gmocoin.py` & `pybotters-1.1.0/pybotters/models/legacy/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/models/okx.py` & `pybotters-1.1.0/pybotters/models/okx.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     async def initialize(self, *aws: Awaitable[aiohttp.ClientResponse]) -> None:
         """Initialize DataStore from HTTP response data.
 
         対応エンドポイント
 
         - GET /api/v5/trade/orders-pending (:attr:`.OKXDataStore.orders`)
         - GET /api/v5/trade/orders-algo-pending (:attr:`.OKXDataStore.ordersalgo` :attr:`.OKXDataStore.algoadvance`)
-        """  # noqa: E501
+        """
         for f in asyncio.as_completed(aws):
             resp = await f
             data = await resp.json()
             if data["code"] != "0":
                 logger.warning(f"Invalid response: {data}")
             if resp.url.path == "/api/v5/trade/orders-pending":
                 self.orders._onresponse(data["data"])
@@ -275,48 +275,40 @@
     _LIST_KEYS = ["ts", "o", "h", "l", "c"]
 
     def _onmessage(self, msg: dict[str, Any]) -> None:
         for item in msg["data"]:
             self._update([{**msg["arg"], **dict(zip(self._LIST_KEYS, item))}])
 
 
-class Instruments(_UpdateStore):
-    ...
+class Instruments(_UpdateStore): ...
 
 
-class Tickers(_UpdateStore):
-    ...
+class Tickers(_UpdateStore): ...
 
 
-class OpenInterest(_UpdateStore):
-    ...
+class OpenInterest(_UpdateStore): ...
 
 
 class Candle(_CandleStore):
     _LIST_KEYS = ["ts", "o", "h", "l", "c", "vol", "volCcy"]
 
 
-class Trades(_InsertStore):
-    ...
+class Trades(_InsertStore): ...
 
 
-class EstimatedPrice(_UpdateStore):
-    ...
+class EstimatedPrice(_UpdateStore): ...
 
 
-class MarkPrice(_UpdateStore):
-    ...
+class MarkPrice(_UpdateStore): ...
 
 
-class MarkPriceCandle(_CandleStore):
-    ...
+class MarkPriceCandle(_CandleStore): ...
 
 
-class PriceLimit(_UpdateStore):
-    ...
+class PriceLimit(_UpdateStore): ...
 
 
 class Books(DataStore):
     _KEYS = ["instId", "side", "px"]
     _LIST_KEYS = ["px", "sz", "liqSz", "ordSz"]
 
     def _init(self) -> None:
@@ -353,32 +345,27 @@
                     else:
                         self._delete([item])
             if "checksum" in book:
                 self.checksum[msg["arg"]["instId"]] = book["checksum"]
             self.ts = book["ts"]
 
 
-class OptSummary(_UpdateStore):
-    ...
+class OptSummary(_UpdateStore): ...
 
 
-class FundingRate(_UpdateStore):
-    ...
+class FundingRate(_UpdateStore): ...
 
 
-class IndexCandle(_CandleStore):
-    ...
+class IndexCandle(_CandleStore): ...
 
 
-class IndexTickers(_UpdateStore):
-    ...
+class IndexTickers(_UpdateStore): ...
 
 
-class Status(_InsertStore):
-    ...
+class Status(_InsertStore): ...
 
 
 class Account(DataStore):
     def _onmessage(self, msg: dict[str, Any]) -> None:
         self._clear()
         self._insert(msg["data"])
 
@@ -463,13 +450,12 @@
         for item in msg["data"]:
             if item["state"] in ("live", "partially_filled"):
                 self._update([item])
             else:
                 self._delete([item])
 
 
-class LiquidationWarning(_UpdateStore):
-    ...
+class LiquidationWarning(_UpdateStore): ...
 
 
 class AccountGreeks(_UpdateStore):
     _KEYS = ["ccy"]
```

### Comparing `pybotters-1.0.0/pybotters/models/phemex.py` & `pybotters-1.1.0/pybotters/models/phemex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/request.py` & `pybotters-1.1.0/pybotters/request.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.0.0/pybotters/store.py` & `pybotters-1.1.0/pybotters/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self._keys: tuple[str, ...] = tuple(keys if keys else self._KEYS)
         self._events: list[asyncio.Event] = []
         self._queues: list[asyncio.Queue] = []
         if data is None:
             data = []
         self._insert(data)
         if hasattr(self, "_init"):
-            getattr(self, "_init")()
+            self._init()
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __iter__(self) -> Iterator[Item]:
         return iter(self._data.values())
 
@@ -157,15 +157,15 @@
     def get(self, item: Item) -> Item | None:
         """DataStore から Item を取得します。
 
         Args:
             item: DataStore のキー (:attr:`.DataStore._KES`) を指定する辞書
 
         Returns:
-            キーに一致するアイテムがアイテムがあればそのアイテムを返します。
+            キーに一致するアイテムがあればそのアイテムを返します。
             なければ None を返します
         """
         if self._keys:
             try:
                 keyitem = {k: item[k] for k in self._keys}
             except KeyError:
                 pass
@@ -350,15 +350,15 @@
     """
 
     def __init__(self) -> None:
         self._stores: dict[str, DataStore] = {}
         self._events: list[asyncio.Event] = []
         self._iscorofunc = asyncio.iscoroutinefunction(self._onmessage)
         if hasattr(self, "_init"):
-            getattr(self, "_init")()
+            self._init()
 
     def __getitem__(self, name: str) -> DataStore | None:
         return self._stores[name]
 
     def __contains__(self, name: str) -> bool:
         return name in self._stores
```

### Comparing `pybotters-1.0.0/pybotters/ws.py` & `pybotters-1.1.0/pybotters/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import base64
 import datetime
 import hashlib
 import hmac
 import inspect
 import logging
 import random
+import struct
 import time
 import uuid
 from dataclasses import dataclass
 from secrets import token_hex
 from typing import Any, AsyncIterator, Generator
 
 import aiohttp
@@ -61,14 +62,17 @@
         self._session = session
         self._url = url
 
         self._loop = session._loop
         self._current_ws: aiohttp.ClientWebSocketResponse | None = None
         self._event = asyncio.Event()
 
+        self._autoping = kwargs.pop("autoping", True)
+        self._pings: dict[bytes, asyncio.Event] = {}
+
         if send_str is None:
             send_str = []
         elif isinstance(send_str, str):
             send_str = [send_str]
 
         if send_bytes is None:
             send_bytes = []
@@ -91,15 +95,15 @@
             hdlr_bytes = [hdlr_bytes]
 
         if hdlr_json is None:
             hdlr_json = []
         elif callable(hdlr_json):
             hdlr_json = [hdlr_json]
 
-        self._task = asyncio.create_task(
+        self._task = self._loop.create_task(
             self._run_forever(
                 send_str=send_str,
                 send_bytes=send_bytes,
                 send_json=send_json,
                 hdlr_str=hdlr_str,
                 hdlr_bytes=hdlr_bytes,
                 hdlr_json=hdlr_json,
@@ -153,28 +157,28 @@
                     send_bytes=send_bytes,
                     send_json=send_json,
                     hdlr_str=hdlr_str,
                     hdlr_bytes=hdlr_bytes,
                     hdlr_json=hdlr_json,
                     **kwargs,
                 )
-            # From https://github.com/python-websockets/websockets/blob/12.0/src/websockets/legacy/client.py#L600-L624  # noqa: E501
+            # From https://github.com/python-websockets/websockets/blob/12.0/src/websockets/legacy/client.py#L600-L624
             # Licensed under the BSD-3-Clause
             except Exception as e:
                 logger.warning(f"{pretty_modulename(e)}: {e}")
                 if backoff_delay == BACKOFF_MIN:
                     initial_delay = random.random() * BACKOFF_INITIAL
                     await asyncio.sleep(initial_delay)
                 else:
                     await asyncio.sleep(int(backoff_delay))
                 backoff_delay = backoff_delay * BACKOFF_FACTOR
                 backoff_delay = min(backoff_delay, BACKOFF_MAX)
             else:
                 backoff_delay = BACKOFF_MIN
-            # End https://github.com/python-websockets/websockets/blob/12.0/src/websockets/legacy/client.py#L600-L624  # noqa: E501
+            # End https://github.com/python-websockets/websockets/blob/12.0/src/websockets/legacy/client.py#L600-L624
             finally:
                 self._current_ws = None
                 self._event.clear()
 
     async def _ws_connect(
         self,
         *,
@@ -182,15 +186,15 @@
         send_bytes: list[bytes],
         send_json: list[dict],
         hdlr_str: list[WsStrHandler],
         hdlr_bytes: list[WsBytesHandler],
         hdlr_json: list[WsJsonHandler],
         **kwargs: Any,
     ) -> None:
-        async with self._session.ws_connect(self._url, **kwargs) as ws:
+        async with self._session.ws_connect(self._url, autoping=False, **kwargs) as ws:
             self._current_ws = ws
             self._event.set()
 
             await self._ws_send(ws, send_str, send_bytes, send_json)
 
             await self._ws_receive(ws, hdlr_str, hdlr_bytes, hdlr_json)
 
@@ -226,29 +230,68 @@
         hdlr_str: list[WsStrHandler],
         hdlr_bytes: list[WsBytesHandler],
         hdlr_json: list[WsJsonHandler],
     ) -> None:
         if msg.type == aiohttp.WSMsgType.TEXT:
             for hdlr in hdlr_str:
                 self._loop.call_soon(hdlr, msg.data, ws)
-
-        if msg.type == aiohttp.WSMsgType.BINARY:
+        elif msg.type == aiohttp.WSMsgType.BINARY:
             for hdlr in hdlr_bytes:
                 self._loop.call_soon(hdlr, msg.data, ws)
 
         if hdlr_json:
             try:
                 data = msg.json()
             except json.JSONDecodeError as e:
                 if msg.data not in {"ping", "pong"}:
                     logger.warning(f"{pretty_modulename(e)}: {e} {e.doc}")
             else:
                 for hdlr in hdlr_json:
                     self._loop.call_soon(hdlr, data, ws)
 
+        if msg.type == aiohttp.WSMsgType.PING and self._autoping:
+            self._loop.create_task(ws.pong(msg.data))
+        elif msg.type == aiohttp.WSMsgType.PONG:
+            data = bytes(msg.data)
+            if data in self._pings:
+                self._pings[data].set()
+
+    async def heartbeat(self, timeout: float = 10.0) -> None:
+        """Ensure WebSocket connection is open with Ping-Pong.
+
+        WebSocket の Ping-Pong で接続の疎通を確認します。
+        ユーザーコード内で WebSocket のデータを利用する前にこのコルーチンを待機することで、
+        WebSocket の接続性を保証するのに役に立ちます。
+
+        一定時間 Pong が返ってこない場合は再接続を試みます。
+        このメソッドは疎通が確認されるまで待機します。
+
+        Args:
+            timeout: WebSocket Ping-Pong ハートビート (デフォルト 10.0 秒)
+        """
+        while True:
+            await self._wait_handshake()
+
+            ping = struct.pack("!I", random.getrandbits(32))
+            self._pings[ping] = asyncio.Event()
+            if self._current_ws:
+                await self._current_ws.ping(ping)
+
+            try:
+                await asyncio.wait_for(self._pings[ping].wait(), timeout=timeout)
+            except asyncio.TimeoutError:
+                if self._current_ws:
+                    self._current_ws._pong_not_received()
+                    self._current_ws = None
+                    self._event.clear()
+            else:
+                return
+            finally:
+                del self._pings[ping]
+
     async def wait(self) -> None:
         """Wait WebSocketApp.
 
         WebSocketApp の待機を待ちます。
         ただし WebSocketApp は自動再接続の機構を備えるので、実質的に無限待機です。
         プログラムの終了を防ぐのに役に立ちます。
         """
```

### Comparing `pybotters-1.0.0/PKG-INFO` & `pybotters-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,88 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pybotters
-Version: 1.0.0
-Summary: An advanced API client for python botters.
-Home-page: https://github.com/pybotters/pybotters
-License: MIT
-Author: MtkN1
-Author-email: 51289448+MtkN1@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
+Version: 1.1.0
+Summary: An advanced API client for python crypto bot traders
+Project-URL: Documentation, https://pybotters.readthedocs.io/ja/stable/
+Project-URL: Repository, https://github.com/pybotters/pybotters
+Author-email: MtkN1 <51289448+MtkN1@users.noreply.github.com>
+License-Expression: MIT
+License-File: LICENCE
+Keywords: aiohttp,crypto,exchange,trading
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Typing :: Typed
-Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
-Project-URL: Documentation, https://pybotters.readthedocs.io/ja/stable/
-Project-URL: Repository, https://github.com/pybotters/pybotters
+Requires-Python: >=3.8
+Requires-Dist: aiohttp>=3.7.0
+Provides-Extra: dev
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-aiohttp; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-freezer; extra == 'dev'
+Requires-Dist: pytest-mock; extra == 'dev'
+Requires-Dist: rich; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-autobuild; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-new-tab-link; extra == 'docs'
+Provides-Extra: lint
+Requires-Dist: ruff; extra == 'lint'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-aiohttp; extra == 'test'
+Requires-Dist: pytest-asyncio; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-freezer; extra == 'test'
+Requires-Dist: pytest-mock; extra == 'test'
 Description-Content-Type: text/markdown
 
 [
   ![PyPI](https://img.shields.io/pypi/v/pybotters)
   ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pybotters)
   ![PyPI - License](https://img.shields.io/pypi/l/pybotters)
 ](https://pypi.org/project/pybotters/)
 [![Downloads](https://static.pepy.tech/badge/pybotters)](https://pepy.tech/project/pybotters)
 
-[![pytest](https://github.com/pybotters/pybotters/actions/workflows/pytest.yml/badge.svg)](https://github.com/pybotters/pybotters/actions/workflows/pytest.yml)
+[![CI](https://github.com/pybotters/pybotters/actions/workflows/ci.yml/badge.svg)](https://github.com/pybotters/pybotters/actions/workflows/ci.yml)
 [![publish](https://github.com/pybotters/pybotters/actions/workflows/publish.yml/badge.svg)](https://github.com/pybotters/pybotters/actions/workflows/publish.yml)
 [![codecov](https://codecov.io/gh/pybotters/pybotters/graph/badge.svg?token=ARR29R726W)](https://codecov.io/gh/pybotters/pybotters)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/pybotters/badge/?version=latest)](https://pybotters.readthedocs.io/ja/latest/?badge=latest)
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/pybotters/pybotters?style=social)](https://github.com/pybotters/pybotters/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/pybotters/pybotters?style=social)](https://github.com/pybotters/pybotters/network/members)
 [![Discord](https://img.shields.io/discord/832651305155297331?label=Discord&logo=discord&style=social)](https://discord.com/invite/CxuWSX9U69)
 [![GitHub Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23db61a2.svg?&logo=github&logoColor=181717&&style=flat-square&labelColor=white)](https://github.com/sponsors/MtkN1)
 
 
 # pybotters
 
-![pybotters logo](docs/logo_150.png)
+![pybotters logo](https://raw.githubusercontent.com/pybotters/pybotters/main/docs/logo_150.png)
 
 An advanced API client for python botters. This project is in Japanese.
 
 ## 📌 Description
 
 `pybotters` is a Python library for [仮想通貨 botter (crypto bot traders)](https://medium.com/perpdex/botter-the-crypto-bot-trader-in-japan-2f5f2a65856f).
 
@@ -299,8 +326,7 @@
 X:
 
 [![X (formerly Twitter) Follow](https://img.shields.io/twitter/follow/MtkN1XBt)](https://twitter.com/MtkN1XBt)
 
 Discord:
 
 [![Discord Widget](https://discord.com/api/guilds/832651305155297331/widget.png?style=banner3)](https://discord.com/invite/CxuWSX9U69)
-
```

