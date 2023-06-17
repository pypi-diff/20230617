# Comparing `tmp/auto-screener-0.1.2.tar.gz` & `tmp/auto-screener-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.1.2.tar", last modified: Fri Jun 16 12:15:57 2023, max compression
+gzip compressed data, was "auto-screener-0.2.0.tar", last modified: Sat Jun 17 10:42:21 2023, max compression
```

## Comparing `auto-screener-0.1.2.tar` & `auto-screener-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 12:15:57.382559 auto-screener-0.1.2/
--rw-rw-rw-   0        0        0       98 2023-06-16 12:15:57.000000 auto-screener-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-16 12:15:57.382559 auto-screener-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 12:15:57.377535 auto-screener-0.1.2/auto_screener/
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.1.2/auto_screener/base.py
--rw-rw-rw-   0        0        0    17233 2023-06-15 21:24:06.000000 auto-screener-0.1.2/auto_screener/collect.py
--rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-0.1.2/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-0.1.2/auto_screener/document.py
--rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-0.1.2/auto_screener/exchanges.py
--rw-rw-rw-   0        0        0    26687 2023-06-16 12:15:07.000000 auto-screener-0.1.2/auto_screener/feed.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.1.2/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.1.2/auto_screener/interval.py
--rw-rw-rw-   0        0        0    26820 2023-06-16 12:11:56.000000 auto-screener-0.1.2/auto_screener/screener.py
--rw-rw-rw-   0        0        0    24728 2023-06-13 13:49:29.000000 auto-screener-0.1.2/auto_screener/screening.py
--rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-0.1.2/auto_screener/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:15:57.381559 auto-screener-0.1.2/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.1.2/build.py
--rw-rw-rw-   0        0        0      645 2023-06-16 12:15:57.000000 auto-screener-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       59 2023-05-24 20:12:53.000000 auto-screener-0.1.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 19:47:16.000000 auto-screener-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 12:15:57.382559 auto-screener-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-06-16 12:15:48.000000 auto-screener-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:42:21.932310 auto-screener-0.2.0/
+-rw-rw-rw-   0        0        0       98 2023-06-17 10:42:21.000000 auto-screener-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-17 10:42:21.931313 auto-screener-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 10:42:21.926311 auto-screener-0.2.0/auto_screener/
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.2.0/auto_screener/base.py
+-rw-rw-rw-   0        0        0    17233 2023-06-15 21:24:06.000000 auto-screener-0.2.0/auto_screener/collect.py
+-rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-0.2.0/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-0.2.0/auto_screener/document.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-0.2.0/auto_screener/exchanges.py
+-rw-rw-rw-   0        0        0    26654 2023-06-17 10:31:17.000000 auto-screener-0.2.0/auto_screener/feed.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.2.0/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.2.0/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    33759 2023-06-17 10:31:17.000000 auto-screener-0.2.0/auto_screener/screener.py
+-rw-rw-rw-   0        0        0    32301 2023-06-17 10:33:08.000000 auto-screener-0.2.0/auto_screener/screening.py
+-rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-0.2.0/auto_screener/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:42:21.930310 auto-screener-0.2.0/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.2.0/build.py
+-rw-rw-rw-   0        0        0      645 2023-06-17 10:42:21.000000 auto-screener-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-0.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 10:42:21.932310 auto-screener-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-06-17 10:42:08.000000 auto-screener-0.2.0/setup.py
```

### Comparing `auto-screener-0.1.2/PKG-INFO` & `auto-screener-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.1.2
+Version: 0.2.0
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.1.2/README.md` & `auto-screener-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener/base.py` & `auto-screener-0.2.0/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener/collect.py` & `auto-screener-0.2.0/auto_screener/collect.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener/dataset.py` & `auto-screener-0.2.0/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener/document.py` & `auto-screener-0.2.0/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener/feed.py` & `auto-screener-0.2.0/auto_screener/screening.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,491 +1,703 @@
-# feed.py
+# screening.py
 
-import threading
-import asyncio
 import time
+import asyncio
 import warnings
-from functools import partial
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any,
-    Union, Callable, List, Type
+    Optional, Union, Dict, Iterable, Any, List
 )
 
 import pandas as pd
+import numpy as np
 
-from represent import Modifiers, BaseModel
+import ccxt
+import ccxt.pro as ccxtpro
+import ccxt.async_support as async_ccxt
 
-from cryptofeed import FeedHandler
-from cryptofeed.feed import Feed
-from cryptofeed.types import OrderBook
-from cryptofeed.defines import L2_BOOK
+from represent import Modifiers
 
+from multithreading import Caller, Callers, multi_threaded_calls
+
+from auto_screener.hints import Number
 from auto_screener.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
+    OPEN, HIGH, LOW, CLOSE, VOLUME, BIDS, ASKS,
+    DATE_TIME, OHLCV_COLUMNS
 )
-from auto_screener.symbols import Separator, adjust_symbol
+from auto_screener.interval import interval_to_total_time
 from auto_screener.screener import (
-    BaseScreener, BaseMultiScreener, create_market_dataframe
-)
-from auto_screener.hints import Number
-from auto_screener.exchanges import EXCHANGES
-from auto_screener.collect import (
-    find_name, validate_exchange, validate_symbol
+    wait_for_update, BaseMultiScreener, structure_screener_datasets,
+    BaseScreener, MarketRecorder, create_market_dataframe
 )
 
 __all__ = [
-    "MarketRecorder",
-    "MarketHandler",
-    "MarketScreener",
-    "add_feeds",
-    "create_market",
-    "market_screener",
-    "market_recorder",
-    "create_orderbook_dataframe"
+    "OHLCVScreener",
+    "MarketOHLCVScreener",
+    "market_ohlcv_recorder",
+    "MarketOHLCVRecorder",
+    "market_ohlcv_screener",
+    "create_ohlcv_market",
+    "create_ohlcv_dataframe"
 ]
 
-Market = Dict[str, Dict[str, pd.DataFrame]]
-RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
-
-def create_orderbook_dataframe() -> pd.DataFrame:
+def configure_exchange(
+        exchange: str,
+        pro: Optional[bool] = True,
+        options: Optional[Dict[str, Any]] = None
+) -> async_ccxt.Exchange:
     """
-    Creates a dataframe for the order book data.
+    Validates the exchange source value.
 
-    :return: The dataframe.
+    :param exchange: The name of the exchange platform.
+    :param pro: The value for the pro interface.
+    :param options: The ccxt options.
+
+    :return: The validates source.
     """
 
-    return create_market_dataframe(
-        columns=MarketRecorder.COLUMNS
-    )
-# end create_orderbook_dataframe
+    try:
+        exchange_service = getattr(
+            (ccxtpro if pro else async_ccxt), exchange
+        )(options)
 
-def create_market(data: Dict[str, Iterable[str]]) -> Dict[str, Dict[str, pd.DataFrame]]:
-    """
-    Creates the dataframes of the market data.
+    except AttributeError:
+        raise ValueError(f"Unrecognized exchange name: {exchange}.")
+        # end try
 
-    :param data: The market data.
+    if not (
+        hasattr(exchange_service, "watch_tickers") or
+        hasattr(exchange_service, "fetch_tickers")
+    ):
+        raise ValueError(
+            f"Exchange {exchange_service} must have at least one of the "
+            f"methods 'fetch_tickers', or 'watch_tickers'."
+        )
+        # end if
+    # end if
 
-    :return: The dataframes of the market data.
+    return exchange_service
+# end configure_exchange
+
+class OHLCVScreener(BaseScreener):
     """
+    A class to represent a live asset data builder.
 
-    return {
-        exchange.lower(): {
-            symbol: create_orderbook_dataframe()
-            for symbol in data[exchange]
-        } for exchange in data
-    }
-# end create_market
+    Using this class, you can create a screener object to
+    screen the market ask and bid data for a specific asset in
+    a specific exchange at real time.
 
-class MarketRecorder(BaseModel):
-    """
-    A class to represent a crypto data feed recorder.
-    This object passes the record method to the handler object to record
-    the data fetched by the handler.
+    You can also use it to build real time datasets of Open
+    High Low Close Volume, with Bids and Asks.
 
     Parameters:
 
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
+    - symbol:
+        The symbol of an asset to screen.
+
+    - exchange:
+        The name of the exchange platform to screen data from.
+
+    - locaion:
+        The saving location for the saved data of the screener.
 
-    >>> from auto_screener.feed import market_recorder
+    - interval:
+        The interval for the time between data points in the dataset.
+
+    - delay:
+        The delay to wait between each data fetching.
+
+    - screener:
+        The screener object to connect to for creating the dataset.
+
+    - length:
+        An initial dataset length to start with.
+
+    - pro:
+        The value to use the pro interface.
+
+    - options:
+        The ccxt options for the backend screening process.
+
+    - cencel:
+        The time to cancel screening process after no new data is fetched.
+
+    >>> from auto_screener.screening import OHLCVScreener
+    >>> from auto_screener.screener import wait_for_initialization
+    >>> from auto_screener.interval import interval_to_total_time
     >>>
-    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
+    >>> interval = "1m"
     >>>
-    >>> recorder = market_recorder(data=market)
-
+    >>> dataset = OHLCVScreener(
+    >>>     symbol="BTC/USD", exchange="binance", interval=interval
+    >>> )
+    >>>
+    >>> dataset.run(wait=True)
+    >>>
+    >>> print(dataset.market.iloc[-1].splitlines()[0])
+    >>>
+    >>> while True:
+    >>>     print(dataset.market.iloc[-1].splitlines()[-1])
+    >>>
+    >>>     wait_for_update(dataset, delay=interval_to_total_time(interval))
     """
 
-    modifiers = Modifiers(**BaseModel.modifiers)
-    modifiers.excluded.append("market")
+    modifiers = Modifiers(**BaseScreener.modifiers)
+    modifiers.excluded.append('task')
+
+    __slots__ = "interval", "pro", "market", "options", "task"
+
+    INTERVAL = "1m"
+
+    PRO = False
+
+    OPTIONS = {}
+
+    LENGTH = 0
 
-    __slots__ = "market"
+    BIDS = BIDS
+    ASKS = ASKS
 
-    COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
+    COLUMNS = (
+        OPEN, HIGH, LOW, CLOSE,
+        ASKS, BIDS, VOLUME
+    )
 
-    def __init__(self, market: Optional[Market] = None) -> None:
+    def __init__(
+            self,
+            symbol: str,
+            exchange: str,
+            interval: Optional[str] = None,
+            pro: Optional[bool] = True,
+            data: Optional[pd.DataFrame] = None,
+            length: Optional[Union[bool, int]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
+            location: Optional[str] = None,
+            options: Optional[Dict[str, Any]] = None,
+            cancel: Optional[Union[Number, dt.timedelta]] = None
+    ) -> None:
         """
         Defines the class attributes.
 
-        :param market: The object to fill with the crypto feed record.
+        :param symbol: The symbol of the asset.
+        :param exchange: The exchange to get source data from.
+        :param interval: The interval for the data.
+        :param data: The base dataset of the asset to add to.
+        :param length: The length of the base dataset.
+        :param location: The saving location for the data.
+        :param delay: The delay for the process.
+        :param pro: The value for the pro interface.
+        :param options: The ccxt options.
+        :param cancel: The time to cancel the waiting.
         """
 
-        if market is None:
-            market = {}
+        super().__init__(
+            symbol=symbol, exchange=exchange, delay=delay,
+            location=location, cancel=cancel
+        )
+
+        if pro is None:
+            pro = self.PRO
         # end if
 
-        self.market: Market = market
+        if length is None:
+            length = self.LENGTH
+        # end if
+
+        self.pro = pro
+        self.interval = interval or self.INTERVAL
+        self.options = options or {}
+
+        self.task = None
+
+        self.market = self.validate_data(data, length=length)
     # end __init__
 
-    def structure(self) -> Dict[str, List[str]]:
+    def __getstate__(self) -> Dict[str, Any]:
         """
-        Returns the structure of the market data.
+        Returns the data of the object.
 
-        :return: The structure of the market.
+        :return: The state of the object.
         """
 
-        return {
-            exchange: list(symbols.keys())
-            for exchange, symbols in self.market.items()
-        }
-    # end structure
+        data = super().__getstate__()
 
-    def parameters(self) -> RecorderParameters:
-        """
-        Returns the order book parameters.
+        data["task"] = None
 
-        :return: The order book parameters.
+        return data
+    # end __getstate__
+
+    def validate_data(self, data: Any, length: Optional[int]) -> pd.DataFrame:
         """
+        Validates the asset data value.
 
-        return dict(
-            channels=[L2_BOOK],
-            callbacks={L2_BOOK: self.record},
-            max_depth=2
-        )
-    # end parameters
+        :param data: The asset data.
+        :param length: The length of the data to add.
 
-    async def record(self, data: OrderBook, timestamp: float) -> None:
+        :return: The validates source.
         """
-        Records the data from the crypto feed into the dataset.
 
-        :param data: The data from the exchange.
-        :param timestamp: The time of the request.
-        """
+        if not all(
+            hasattr(self, name) for name in ["exchange", "interval"]
+        ):
+            raise AttributeError(
+                "Source and interval attributes must be defined "
+                "before attempting to validate the data parameter data."
+            )
+        # end if
 
-        exchange = find_name(
-            name=data.exchange, names=self.market.keys()
-        )
-        symbol = find_name(
-            name=adjust_symbol(
-                symbol=data.symbol,
-                separator=Separator.value
-            ),
-            names=exchange
-        )
+        if (
+            (data is None) and
+            (
+                (length is None) or
+                (length == 0) or
+                (length is False) or
+                (
+                    isinstance(length, int) and
+                    not (0 < length <= 500)
+                )
+            )
+        ):
+            data = pd.DataFrame(
+                {column: [] for column in self.COLUMNS},
+                index=[]
+            )
 
-        dataset = (
-            self.market.
-            setdefault(exchange, {}).
-            setdefault(symbol, create_orderbook_dataframe())
-        )
+        elif (data is None) and (isinstance(length, int)):
+            if 0 < length <= 500:
+                try:
+                    exchange = getattr(ccxt, self.exchange)(self.options)
+
+                    data = self.data_to_dataset(
+                        exchange.fetch_ohlcv(
+                            symbol=self.symbol,
+                            timeframe=self.interval,
+                            limit=length
+                        )
+                    )
 
-        bids = data.book.bids.to_list()
-        asks = data.book.asks.to_list()
+                except Exception as e:
+                    warnings.warn(str(e))
 
-        try:
-            dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
-                BIDS: float(bids[0][0]),
-                ASKS: float(asks[0][0]),
-                BIDS_VOLUME: float(bids[0][1]),
-                ASKS_VOLUME: float(asks[0][1])
-            }
+                    data = pd.DataFrame(
+                        {column: [] for column in self.COLUMNS},
+                        index=[]
+                    )
+                # end try
 
-        except IndexError:
-            pass
-        # end try
-    # end record
+            else:
+                raise ValueError(
+                    f"Length must be a positive int between "
+                    f"{1} and {500} when data is not defined, "
+                    f"not: {length}."
+                )
+            # end if
+        # end if
+
+        return data
+    # end validate_data
 
-    def data(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def data_to_dataset(self, data: Iterable[Iterable]) -> pd.DataFrame:
         """
-        Returns the market data of the symbol from the exchange.
+        Adjusts the dataset to an asset Open, High, Low, Close, Bids, Asks, Volume dataset.
 
-        :param exchange: The source name of the exchange.
-        :param symbol: The symbol of the pair.
+        :param data: The data to adjust.
 
-        :return: The dataset of the spread data.
+        :return: The asset dataset.
         """
 
-        exchange = find_name(name=exchange, names=self.market.keys())
+        data = pd.DataFrame(data)
 
-        validate_exchange(
-            exchange=exchange,
-            exchanges=self.market.keys(),
-            provider=self
-        )
+        index_column_name = list(data.columns)[0]
 
-        validate_symbol(
-            symbol=symbol,
-            exchange=exchange,
-            exchanges=self.market.keys(),
-            symbols=self.market[exchange],
-            provider=self
-        )
+        data.index = pd.to_datetime(data[index_column_name], unit="ms")
+        del data[index_column_name]
+        data.index.name = DATE_TIME
+        data.columns = list(OHLCV_COLUMNS)
 
-        return self.market[exchange][symbol]
-    # end data
+        if len(self.market) == 0:
+            asks = [np.nan] * len(data)
+            bids = [np.nan] * len(data)
 
-    def screener(
-            self,
-            symbol: str,
-            exchange: str,
-            location: Optional[str] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None
-    ) -> BaseScreener:
+        else:
+            asks = (
+                self.market[self.ASKS].iloc
+                [-len(data):].values[:]
+            )
+            bids = (
+                self.market[self.BIDS].iloc
+                [-len(data):].values[:]
+            )
+        # end if
+
+        if self.ASKS in data:
+            data[self.ASKS].values[:] = asks
+
+        else:
+            data[self.ASKS] = asks
+        # end if
+
+        if self.BIDS in data:
+            data[self.BIDS].values[:] = bids
+
+        else:
+            data[self.BIDS] = bids
+        # end if
+
+        return data[list(self.COLUMNS)]
+    # end data_to_dataset
+
+    def dataset_path(self, location: Optional[str] = None) -> str:
         """
-        Defines the class attributes.
+        Creates the path to the saving file for the screener object.
 
-        :param symbol: The symbol of the asset.
-        :param exchange: The exchange to get source data from.
-        :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
+        :param location: The saving location of the dataset.
+
+        :return: The saving path for the dataset.
         """
 
-        screener = BaseScreener(
-            symbol=symbol, exchange=exchange, delay=delay,
-            location=location, cancel=cancel,
-            market=self.data(exchange=exchange, symbol=symbol)
+        return super().dataset_path(location=location).replace(
+            '.csv', f'_{self.interval}.csv'
         )
+    # end dataset_path
 
-        return screener
-    # end screener
-
-    def screeners(
-            self,
-            location: Optional[str] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None
-    ) -> List[BaseScreener]:
+    async def async_get_market(self) -> Dict[str, Number]:
         """
-        Defines the class attributes.
+        Gets the market data.
 
-        :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
+        :return: The bids and asks.
         """
 
-        base_screeners = []
+        exchange = configure_exchange(
+            exchange=self.exchange.lower(), pro=self.pro,
+            options=self.options
+        )
 
-        for exchange in self.market:
-            for symbol in self.market[exchange]:
-                base_screeners.append(
-                    self.screener(
-                        symbol=symbol, exchange=exchange, delay=delay,
-                        location=location, cancel=cancel
-                    )
-                )
-            # end for
-        # end for
+        method = None
 
-        return base_screeners
-    # end create_screeners
-# end MarketRecorder
+        if hasattr(exchange, "fetch_tickers"):
+            method = exchange.fetch_tickers
 
-class ExchangeFeed(Feed):
-    """A class to represent an exchange feed object."""
+        elif hasattr(exchange, "watch_tickers"):
+            method = exchange.watch_tickers
+        # end if
 
-    handler: Optional[FeedHandler] = None
+        data = await method(symbols=[self.symbol])
 
-    running: bool = False
+        ticker = list(data.keys())[0]
 
-    def stop(self) -> None:
-        """Stops the process."""
+        data[ticker][VOLUME.lower()] = data[ticker]["quoteVolume"]
+        data[ticker][self.ASKS.lower()] = data[ticker]["ask"]
+        data[ticker][self.BIDS.lower()] = data[ticker]["bid"]
 
-        self.running = False
+        data = {
+            key: data[ticker][key.lower()] for key in
+            self.COLUMNS
+        }
 
-        Feed.stop(self)
-    # end stop
+        if any(np.isnan(value) for value in data.values()):
+            ohlcv = await exchange.fetch_ohlcv(
+                self.symbol, timeframe='1m', limit=1
+            )
 
-    def start(self, loop: asyncio.AbstractEventLoop) -> None:
-        """
-        Create tasks for exchange interfaces and backends.
+            ohlcv = {
+                column: value for column, value in zip(
+                    [OPEN, HIGH, LOW, CLOSE, VOLUME], ohlcv
+                ) if np.isnan(data[column])
+            }
 
-        :param loop: The event loop for the process.
-        """
+            data.update(ohlcv)
+        # end if
+
+        await exchange.close()
+
+        return data
+    # end async_get_market
+
+    async def async_update_market(self) -> None:
+        """Updates the market data."""
+
+        data = await self.async_get_market()
+
+        self.market.loc[dt.datetime.now()] = data
+    # end async_update_market
+
+    def update_market(self) -> None:
+        """Updates the market data."""
+
+        asyncio.run(self.async_update_market())
+    # end update_market
+
+    def get_market(self) -> Dict[str, Number]:
+        """Gets the market data."""
+
+        return asyncio.run(self.async_get_market())
+    # end get_market
+
+    async def async_run_loop(self) -> None:
+        """Runs the processes of price screening."""
 
         self.running = True
 
-        Feed.start(self, loop=loop)
-    # end start
-# end ExchangeFeed
+        delay = interval_to_total_time(self.interval).seconds
 
-def add_feeds(
-        handler: FeedHandler,
-        data: Dict[str, Iterable[str]],
-        fixed: Optional[bool] = False,
-        amount: Optional[int] = 5,
-        separator: Optional[str] = Separator.value,
-        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-) -> None:
-    """
-    Adds the tickers to the handler for each exchange.
-
-    :param handler: The handler object.
-    :param data: The data of the exchanges and tickers to add.
-    :param parameters: The parameters for the exchanges.
-    :param fixed: The value for fixed parameters to all exchanges.
-    :param separator: The separator of the assets.
-    :param amount: The maximum amount of symbols for each feed.
-    """
-
-    base_parameters = None
-
-    if not fixed:
-        parameters = parameters or {}
-
-    else:
-        base_parameters = parameters or {}
-        parameters = {}
-    # end if
+        while self.running:
+            start = time.time()
+
+            try:
+                await self.async_update_market()
+
+            except Exception as e:
+                self.terminate()
+
+                raise RuntimeError(
+                    f"Could not complete task. {str(e)}"
+                ) from e
+            # end try
+
+            end = time.time()
+
+            if delay:
+                time.sleep(max([delay - (end - start), 0]))
+            # end if
+        # end while
+    # end async_run
+
+    def run_loop(self) -> None:
+        """Runs the process of the price screening."""
+
+        task = self.async_run_loop()
+
+        try:
+            loop = asyncio.new_event_loop()
+
+            self.task = loop.create_task(task)
+
+            if not loop.is_running():
+                loop.run_forever()
+            # end if
+
+        except RuntimeError:
+            asyncio.run(task)
+        # end try
+    # end run_loop
+
+    def run_new_loop(self) -> None:
+        """Runs the process of the price screening."""
+
+        task = self.async_run_loop()
+
+        try:
+            loop = asyncio.new_event_loop()
+
+            self.task = loop.create_task(task)
+
+            if not loop.is_running():
+                loop.run_forever()
+            # end if
+
+        except RuntimeError:
+            asyncio.run(task)
+        # end try
+    # end run_loop
 
-    for exchange, symbols in data.items():
-        exchange = find_name(name=exchange, names=EXCHANGES.keys())
+    def stop(self) -> None:
+        """Stops the screening process."""
 
-        symbols = [
-            symbol.replace(separator, '-')
-            for symbol in symbols
-        ]
+        super().stop()
 
-        if fixed:
-            parameters.setdefault(exchange, base_parameters)
+        if self.task is not None:
+            self.task.cancel()
         # end if
+    # end stop
+# end OHLCVScreener
 
-        EXCHANGES[exchange]: Type[ExchangeFeed]
+class MarketOHLCVRecorder(MarketRecorder):
+    """
+    A class to represent a crypto data feed recorder.
+    This object passes the record method to the handler object to record
+    the data fetched by the handler.
 
-        packets = []
+    Parameters:
 
-        for i in range(0, int(len(symbols) / amount) + len(symbols) % amount, amount):
-            packets.append(symbols[i:])
-        # end for
+    - market:
+        The market structure of the data to store the fetched data in.
+        This structure is a dictionary with exchange names as keys
+        and dictionaries as values, where their keys are symbols,
+        and their values are the dataframes to record the data.
 
-        for symbols_packet in packets:
-            feed = EXCHANGES[exchange](
-                symbols=symbols_packet,
-                **(
-                    parameters[exchange]
-                    if (
-                        (exchange in parameters) and
-                        isinstance(parameters[exchange], dict) and
-                        all(isinstance(key, str) for key in parameters)
+    >>> from auto_screener.screening import market_ohlcv_recorder
+    >>>
+    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
+    >>>
+    >>> recorder = market_ohlcv_recorder(data=market)
+    """
 
-                    ) else {}
-                )
-            )
+    COLUMNS = OHLCVScreener.COLUMNS
+# end MarketOHLCVRecorder
 
-            feed.start = partial(ExchangeFeed.start, feed)
-            feed.stop = partial(ExchangeFeed.stop, feed)
-            feed.handler = handler
-            feed.running = False
+def create_ohlcv_dataframe() -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
 
-            handler.add_feed(feed)
-        # end for
-    # end for
-# end add_feeds
+    :return: The dataframe.
+    """
+
+    return create_market_dataframe(
+        columns=MarketOHLCVRecorder.COLUMNS
+    )
+# end create_order_book_dataframe
 
-class MarketHandler(FeedHandler):
-    """A class to handle the market data feed."""
+def create_ohlcv_market(data: Dict[str, Iterable[str]]) -> Dict[str, Dict[str, pd.DataFrame]]:
+    """
+    Creates the dataframes of the market data.
 
-    def __init__(self) -> None:
-        """Defines the class attributes."""
+    :param data: The market data.
 
-        super().__init__(
-            config={'uvloop': False, 'log': {'disabled': True}}
-        )
-    # end __init__
-# end MarketHandler
+    :return: The dataframes of the market data.
+    """
+
+    return {
+        exchange.lower(): {
+            symbol.upper(): create_ohlcv_dataframe()
+            for symbol in data[exchange]
+        } for exchange in data
+    }
+# end create_ohlcv_market
+
+def market_ohlcv_recorder(data: Dict[str, Iterable[str]]) -> MarketOHLCVRecorder:
+    """
+    Creates the market recorder object for the data.
+
+    :param data: The market data.
+
+    :return: The market recorder object.
+    """
+
+    return MarketOHLCVRecorder(
+        market=create_ohlcv_market(data=data)
+    )
+# end market_ohlcv_recorder
 
-class MarketScreener(BaseMultiScreener):
+class MarketOHLCVScreener(BaseMultiScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
     Parameters:
 
-    - location:
-        The saving location for the saved data of the screener.
+    - exchanges:
+        The data of exchanges and their tickers to screen.
 
-    - cancel:
-        The time to cancel screening process after no new data is fetched.
+    - interval:
+        The interval for the time between data points in the dataset.
 
     - delay:
         The delay to wait between each data fetching.
 
-    - handler:
-        The handler object to handle the data feed.
+    - length:
+        An initial dataset length to start with.
+
+    - locaion:
+        The saving location for the saved data of the screener.
+
+    - pro:
+        The value to use the pro interface.
 
-    - recorder:
-        The recorder object to record the data of the market from the feed.
+    - options:
+        The ccxt options for the backend screening process.
+
+    - cencel:
+        The time to cancel screening process after no new data is fetched.
 
-    >>> from auto_screener.feed import market_screener
+    >>> from auto_screener.screening import MarketOHLCVScreener
+    >>> from auto_screener.screener import wait_for_initialization
     >>>
-    >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
+    >>> screener = MarketOHLCVScreener(
+    >>>     data={
+    >>>         "binance": ["BTC/USDT", "AAVE/EUR"],
+    >>>         "bittrex": ["GRT/USD", "BTC/USD"]
+    >>>     }
+    >>> )
     >>>
-    >>> screener = market_screener(data=structure)
-    >>> screener.run()
+    >>> screener.run(wait=True)
+    >>>
+    >>> while True:
+    >>>     screener.wait_for_update(delay=1)
     """
 
-    modifiers = Modifiers(**BaseMultiScreener.modifiers)
-    modifiers.excluded.extend(['update_process'])
+    __slots__ = "interval", "pro", "options", "task", "exchanges", "length"
 
-    __slots__ = (
-        "handler", "recorder", "updating",
-        "update_process", "loop", "limited",
-        "feeds_parameters", "screening_parameters"
-    )
+    INTERVAL = OHLCVScreener.INTERVAL
+
+    PRO = OHLCVScreener.PRO
 
-    DELAY = 10
-    AMOUNT = 5
+    OPTIONS = OHLCVScreener.OPTIONS
 
-    REFRESH = dt.timedelta(minutes=5)
+    ASKS = OHLCVScreener.ASKS
+    BIDS = OHLCVScreener.BIDS
+
+    LENGTH = OHLCVScreener.LENGTH
+    CANCEL = OHLCVScreener.CANCEL
+
+    COLUMNS = OHLCVScreener.COLUMNS
+
+    screeners: List[OHLCVScreener]
 
     def __init__(
             self,
+            interval: Optional[str] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
+            length: Optional[Union[int, bool]] = None,
             location: Optional[str] = None,
+            pro: Optional[bool] = None,
+            options: Optional[Dict[str, Any]] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
-            refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
-            limited: Optional[bool] = None,
-            handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None,
+            screeners: Optional[Iterable[OHLCVScreener]] = None,
             recorder: Optional[MarketRecorder] = None
     ) -> None:
         """
-        Creates the class attributes.
+        Defines the class attributes.
 
+        :param interval: The interval of the data to load.
+        :param pro: The value to use the pro interface.
         :param location: The saving location for the data.
-        :param delay: The delay for the process.
-        :param cancel: The cancel time for the loops.
-        :param limited: The value to limit the screeners to active only.
-        :param refresh: The refresh time for rerunning.
-        :param handler: The handler object for the market data.
-        :param amount: The maximum amount of symbols for each feed.
+        :param delay: The delay between each data fetching request.
+        :param length: The length of the data to get in each request.
+        :param options: The ccxt options.
+        :param cancel: The time it takes to cancel a non-updating screener.
+        :param screeners: The create_screeners for the multi-screener object.
         :param recorder: The recorder object for recording the data.
         """
 
         super().__init__(
-            location=location, cancel=cancel, delay=delay
+            delay=delay, cancel=cancel,
+            location=location, recorder=recorder or MarketOHLCVRecorder(
+                market=structure_screener_datasets(screeners=screeners)
+            )
         )
 
-        if refresh is True:
-            refresh = self.REFRESH
+        if pro is None:
+            pro = self.PRO
         # end if
 
-        self.handler = handler or MarketHandler()
-        self.recorder = recorder or MarketRecorder()
-        self.limited = limited or False
-        self.amount = amount or self.AMOUNT
-        self.refresh = refresh
-
-        self.screeners: List[BaseScreener] = self.create_screeners()
+        if length is None:
+            length = self.LENGTH
+        # end if
 
-        self.updating = False
+        self.options = options or self.OPTIONS
+        self.interval = interval or self.INTERVAL
+        self.pro = pro
+        self.length = length
 
-        self.update_process: Optional[threading.Thread] = None
-        self.loop: Optional[asyncio.AbstractEventLoop] = None
-
-        self.feeds_parameters: Optional[Dict[str, Any]] = None
-        self.screening_parameters: Optional[Dict[str, Any]] = None
-    # end __init__
+        self.screeners[:] = list(screeners or []) or self.create_screeners()
+    # end Screener
 
     @property
     def market(self) -> Dict[str, Dict[str, pd.DataFrame]]:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
@@ -494,411 +706,370 @@
         return self.recorder.market
     # end market
 
     def create_screener(
             self,
             symbol: str,
             exchange: str,
+            pro: Optional[bool] = True,
+            length: Optional[Union[bool, int]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
             location: Optional[str] = None,
+            options: Optional[Dict[str, Any]] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None
-    ) -> BaseScreener:
+            container: Optional[Dict[str, Dict[str, OHLCVScreener]]] = None
+    ) -> OHLCVScreener:
         """
-        Defines the class attributes.
+        Creates the screener and inserts it into the container.
 
-        :param symbol: The symbol of the asset.
-        :param exchange: The exchange to get source data from.
+        :param container: The container to contain the new screener.
+        :param symbol: The symbol of the screener.
+        :param exchange: The source of the data.
+        :param pro: The value to use the pro interface.
         :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
+        :param delay: The delay between each data fetching request.
+        :param length: The length of the data to get in each request.
+        :param options: The ccxt options.
+        :param cancel: The time it takes to cancel a non-updating screener.
         """
 
-        return self.recorder.screener(
-            symbol=symbol, exchange=exchange, location=location or self.location,
-            cancel=cancel or self.cancel, delay=delay or self.delay
+        if container is None:
+            container = {}
+        # end if
+
+        if pro is None:
+            pro = self.pro
+        # end if
+
+        if length is None:
+            length = self.length
+        # end if
+
+        if cancel is None:
+            cancel = self.cancel
+        # end if
+
+        if delay is None:
+            delay = self.delay
+        # end if
+
+        container.setdefault(exchange, {})[symbol] = OHLCVScreener(
+            symbol=symbol, exchange=exchange,
+            options=options, interval=self.interval,
+            pro=pro, delay=delay, length=length,
+            location=location or self.location, cancel=cancel
         )
+
+        return container[exchange][symbol]
     # end create_screener
 
-    def create_screeners(
+    def _create_screener(
             self,
+            symbol: str,
+            exchange: str,
+            pro: Optional[bool] = True,
+            length: Optional[Union[bool, int]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
             location: Optional[str] = None,
+            options: Optional[Dict[str, Any]] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None
-    ) -> List[BaseScreener]:
+            container: Optional[Dict[str, Dict[str, Optional[OHLCVScreener]]]] = None,
+    ) -> OHLCVScreener:
         """
-        Defines the class attributes.
+        Creates the screener and inserts it into the container.
 
+        :param container: The container to contain the new screener.
+        :param symbol: The symbol of the screener.
+        :param exchange: The source of the data.
+        :param pro: The value to use the pro interface.
         :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
-        """
-
-        return self.recorder.screeners(
-            location=location or self.location,
-            cancel=cancel or self.cancel, delay=delay or self.delay
-        )
-    # end create_screeners
-
-    def add_feeds(
-            self,
-            data: Dict[str, Iterable[str]],
-            fixed: Optional[bool] = True,
-            separator: Optional[str] = Separator.value,
-            amount: Optional[int] = None,
-            parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-    ) -> None:
-        """
-        Adds the tickers to the handler for each exchange.
-
-        :param data: The data of the exchanges and tickers to add.
-        :param parameters: The parameters for the exchanges.
-        :param fixed: The value for fixed parameters to all exchanges.
-        :param amount: The maximum amount of symbols for each feed.
-        :param separator: The separator of the assets.
+        :param delay: The delay between each data fetching request.
+        :param length: The length of the data to get in each request.
+        :param options: The ccxt options.
+        :param cancel: The time it takes to cancel a non-updating screener.
         """
 
-        self.feeds_parameters = dict(
-            data=data, fixed=fixed, separator=separator, parameters=parameters
-        )
-
-        feed_params = self.recorder.parameters()
-        feed_params.update(parameters or {})
-
-        add_feeds(
-            self.handler, data=data, fixed=fixed, separator=separator,
-            parameters=feed_params, amount=amount or self.amount
-        )
-    # end add_feeds
-
-    def refresh_feeds(self) -> None:
-        """Refreshes the feed objects."""
-
-        if self.feeds_parameters is None:
-            warnings.warn(
-                "Cannot refresh feeds as there was "
-                "no feeds initialization to repeat."
-            )
-
-            return
+        if container is None:
+            container = {}
         # end if
 
-        self.handler.feeds.clear()
-
-        self.add_feeds(**self.feeds_parameters)
-    # end refresh
-
-    def rerun(self) -> None:
-        """Refreshes the process."""
-
-        if self.screening_parameters is None:
-            warnings.warn(
-                "Cannot rerun as there was "
-                "no initial process to repeat."
+        try:
+            return self.create_screener(
+                symbol=symbol, exchange=exchange,
+                container=container, pro=pro, length=length,
+                delay=delay, location=location,
+                options=options, cancel=cancel
             )
 
-            return
-        # end if
-
-        self.terminate()
-        self.refresh_feeds()
-        self.run(**self.screening_parameters)
-    # end rerun
-
-    def data(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source name of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
+        except ValueError as e:
+            warnings.warn(str(e))
 
-        return self.recorder.data(exchange=exchange, symbol=symbol)
-    # end data
+            container[symbol] = None
+        # end try
+    # end _create_screener
 
-    def run_loop(
+    def _create_screeners(
             self,
-            start: Optional[bool] = True,
-            loop: Optional[asyncio.AbstractEventLoop] = None
-    ) -> None:
-        """
-        Runs the process of the price screening.
-
-        :param start: The value to start the loop.
-        :param loop: The event loop.
+            symbols: Iterable[str],
+            exchange: str,
+            pro: Optional[bool] = True,
+            length: Optional[Union[bool, int]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
+            location: Optional[str] = None,
+            options: Optional[Dict[str, Any]] = None,
+            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            container: Optional[Dict[str, Dict[str, Optional[OHLCVScreener]]]] = None,
+            wait: Optional[bool] = True
+    ) -> Dict[str, Optional[OHLCVScreener]]:
+        """
+        Creates the screener and inserts it into the container.
+
+        :param container: The container to contain the new screener.
+        :param symbols: The symbol of the screener.
+        :param exchange: The source of the data.
+        :param wait: The value to wait for the creation of the screeners.
+        :param pro: The value to use the pro interface.
+        :param location: The saving location for the data.
+        :param delay: The delay between each data fetching request.
+        :param length: The length of the data to get in each request.
+        :param options: The ccxt options.
+        :param cancel: The time it takes to cancel a non-updating screener.
         """
 
-        if loop is None:
-            loop = asyncio.new_event_loop()
+        if container is None:
+            container = {}
         # end if
 
-        self.loop = loop
-
-        asyncio.set_event_loop(loop)
-
-        self.running = True
-
-        self.handler.run(
-            start_loop=start and (not loop.is_running()),
-            install_signal_handlers=False
-        )
-    # end run_loop
+        symbols = list(symbols)
 
-    def saving_loop(self) -> None:
-        """Runs the process of the price screening."""
+        callers = []
 
-        for screener in self.screeners or self.create_screeners():
-            screener.saving_process = threading.Thread(
-                target=screener.saving_loop
+        for symbol in symbols:
+            callers.append(
+                Caller(
+                    caller=self._create_screener,
+                    kwargs=dict(
+                        container=container,
+                        symbol=symbol, exchange=exchange,
+                        pro=pro, length=length,
+                        delay=delay, location=location,
+                        options=options, cancel=cancel
+                    )
+                )
             )
-            screener.saving_process.start()
         # end for
-    # end saving_loop
-
-    def update_loop(self) -> None:
-        """Updates the state of the screeners."""
 
-        self.updating = True
+        multi_threaded_calls(
+            callers=Callers(callers=callers), wait=wait
+        )
 
-        refresh = self.refresh
+        return container
+    # end _create_screeners
 
-        if isinstance(refresh, dt.timedelta):
-            refresh = refresh.total_seconds()
-        # end if
+    def create_screeners(
+            self,
+            pro: Optional[bool] = True,
+            length: Optional[Union[bool, int]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
+            location: Optional[str] = None,
+            options: Optional[Dict[str, Any]] = None,
+            cancel: Optional[Union[Number, dt.timedelta]] = None,
+    ) -> List[OHLCVScreener]:
+        """
+        Initializes the create_screeners.
 
-        start = time.time()
+        :param pro: The value to use the pro interface.
+        :param location: The saving location for the data.
+        :param delay: The delay between each data fetching request.
+        :param length: The length of the data to get in each request.
+        :param options: The ccxt options.
+        :param cancel: The time it takes to cancel a non-updating screener.
+
+        :return: The created screener objects.
+        """
+
+        market: Dict[str, Dict[str, OHLCVScreener]] = {}
+
+        callers = []
+
+        for exchange, symbols in self.recorder.structure().items():
+            market.setdefault(exchange, {})
+
+            callers.append(
+                Caller(
+                    caller=self._create_screeners,
+                    kwargs=dict(
+                        container=market, symbols=symbols,
+                        exchange=exchange, wait=False,
+                        pro=pro, length=length,
+                        delay=delay, location=location,
+                        options=options, cancel=cancel
+                    )
+                )
+            )
+        # end for
 
-        while self.updating:
-            if self.running:
-                self.update()
+        multi_threaded_calls(callers=Callers(callers=callers))
 
-                current = time.time()
+        screeners = []
 
-                if refresh and ((current - start) >= refresh):
-                    self.rerun()
+        for exchange in market.values():
+            for symbol, screener in exchange.copy().items():
+                if isinstance(screener, OHLCVScreener):
+                    screeners.append(screener)
 
-                    start = current
+                else:
+                    exchange.pop(symbol)
                 # end if
-            # end if
+            # end for
+        # end for
 
-            time.sleep(self.delay)
-        # end while
-    # end update_loop
+        return screeners
+    # end create_screeners
+
+    async def async_get_market(self) -> Dict[str, Dict[str, Dict[str, Number]]]:
+        """Gets the market data."""
 
-    def save(self) -> None:
-        """Runs the data handling loop."""
+        market = {exchange: {} for exchange in self.exchanges}
 
-        for screener in self.screeners or self.create_screeners():
-            threading.Thread(
-                target=screener.save_dataset,
-                kwargs=dict(location=self.location)
-            ).start()
+        for screener in self.screeners:
+            market[screener.exchange][screener.symbol] = (
+                await screener.async_get_market()
+            )
         # end for
-    # end run
 
-    def update(self) -> None:
-        """Updates the state of the screeners."""
+        return market
+    # end async_get_market
 
-        for screener in self.screeners:
-            for feed in self.handler.feeds:
-                feed: ExchangeFeed
+    async def async_update_market(self) -> None:
+        """Updates the market data."""
 
-                if (
-                    self.limited and
-                    (screener.exchange.lower() == feed.id.lower()) and
-                    (not feed.running)
-                ):
-                    screener.stop()
-                # end if
-            # end for
+        for screener in self.screeners:
+            await screener.async_update_market()
         # end for
-    # end update
+    # end async_update_market
 
-    def stop(self) -> None:
-        """Stops the data handling loop."""
+    def update_market(self) -> None:
+        """Updates the market data."""
 
-        super().stop()
+        asyncio.run(self.async_update_market())
+    # end update_market
 
-        self.running = False
+    def get_market(self) -> Dict[str, Dict[str, Dict[str, Number]]]:
+        """Gets the market data."""
 
-        if self.loop is None:
-            return
-        # end if
+        return asyncio.run(self.async_get_market())
+    # end get_market
 
-        if (
-            self.updating and
-            isinstance(self.update_process, threading.Thread) and
-            self.update_process.is_alive()
-        ):
-            self.updating = False
+    def stop(self) -> None:
+        """Stops the screening process."""
 
-            self.update_process = None
-        # end if
+        super().stop()
 
-        self.loop: asyncio.AbstractEventLoop
+        for screener in self.screeners:
+            screener.stop()
+        # end for
+    # end stop
 
-        async def stop() -> None:
-            self.handler.stop(self.loop)
-            self.handler.close(self.loop)
-        # end stop
+    def terminate(self) -> None:
+        """Stops the screening process."""
 
-        self.loop.create_task(stop())
+        super().terminate()
 
-        for task in asyncio.all_tasks(self.loop):
-            task.cancel()
+        for screener in self.screeners:
+            screener.terminate()
         # end for
+    # end terminate
 
-        self.loop = None
+    def blocking(self) -> bool:
+        """
+        returns the value of the process being blocked.
 
-        self.handler.running = False
-    # end stop
+        :return: The value.
+        """
+
+        return self.block
+    # end blocking
 
     def run(
             self,
+            start: Optional[bool] = True,
             save: Optional[bool] = True,
             block: Optional[bool] = False,
-            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None,
             update: Optional[bool] = True,
-            start: Optional[bool] = True,
-            loop: Optional[asyncio.AbstractEventLoop] = None
-    ) -> threading.Thread:
+            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
+            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+    ) -> None:
         """
-        Runs the program.
+        Runs the process of the price screening.
 
+        :param start: The value to start the screening.
         :param save: The value to save the data.
         :param wait: The value to wait after starting to run the process.
         :param block: The value to block the execution.
-        :param timeout: The valur to add a timeout to the process.
         :param update: The value to update the screeners.
-        :param start: The value to start the loop.
-        :param loop: The event loop.
-
-        :return: The timeout process.
+        :param timeout: The valur to add a timeout to the process.
         """
 
         if self.running:
             warnings.warn(f"Screener is already running.")
 
-            return self.screening_process
-        # end if
-
-        self.running = True
-
-        self.screening_parameters = dict(
-            save=save, block=block, wait=wait, loop=loop,
-            timeout=timeout, update=update, start=start
-        )
-
-        if save:
-            self.saving_process = threading.Thread(
-                target=self.saving_loop
-            )
-
-            self.saving_process.start()
-        # end if
-
-        if update:
-            self.update_process = threading.Thread(
-                target=self.update_loop
-            )
-
-            self.update_process.start()
-        # end if
-
-        if timeout:
-            self.timeout(duration=timeout)
-        # end if
-
-        if not block:
-            self.screening_process = threading.Thread(
-                target=lambda: self.run_loop(loop=loop, start=start)
-            )
-
-            self.screening_process.start()
-
-        else:
-            self.run_loop(loop=loop, start=start)
-        # end if
-
-        if isinstance(wait, dt.datetime):
-            wait = wait - dt.datetime.now()
-        # end if
-
-        if isinstance(wait, dt.timedelta):
-            wait = wait.total_seconds()
+            return
         # end if
 
-        if isinstance(wait, bool) and wait:
-            self.wait_for_initialization()
-
-        elif isinstance(wait, (int, float)):
-            time.sleep(wait)
+        if start:
+            for screener in self.screeners:
+                screener.run(
+                    timeout=timeout, wait=False,
+                    block=False, save=save
+                )
+            # end for
         # end if
 
-        return self.screening_process
+        super().run(
+            start=start, save=save, block=block,
+            update=update, wait=wait, timeout=timeout
+        )
     # end run
-# end MarketScreener
-
-def market_recorder(data: Dict[str, Iterable[str]]) -> MarketRecorder:
-    """
-    Creates the market recorder object for the data.
-
-    :param data: The market data.
-
-    :return: The market recorder object.
-    """
+# end Screener
 
-    return MarketRecorder(market=create_market(data=data))
-# end market_recorder
+Market = Dict[str, Dict[str, pd.DataFrame]]
 
-def market_screener(
+def market_ohlcv_screener(
         data: Dict[str, Iterable[str]],
+        interval: Optional[str] = None,
+        delay: Optional[Union[Number, dt.timedelta]] = None,
+        length: Optional[Union[int, bool]] = None,
         location: Optional[str] = None,
+        pro: Optional[bool] = None,
+        options: Optional[Dict[str, Any]] = None,
         cancel: Optional[Union[Number, dt.timedelta]] = None,
-        delay: Optional[Union[Number, dt.timedelta]] = None,
-        limited: Optional[bool] = None,
-        handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
-        amount: Optional[int] = None,
-        refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
-        recorder: Optional[MarketRecorder] = None,
-        fixed: Optional[bool] = True,
-        separator: Optional[str] = Separator.value,
-        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-) -> MarketScreener:
+        recorder: Optional[MarketOHLCVRecorder] = None,
+) -> MarketOHLCVScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
-    :param handler: The handler object for the market data.
-    :param limited: The value to limit the screeners to active only.
-    :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
-    :param fixed: The value for fixed parameters to all exchanges.
-    :param refresh: The refresh time for rerunning.
-    :param amount: The maximum amount of symbols for each feed.
-    :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
+    :param interval: The interval of the data to load.
+    :param pro: The value to use the pro interface.
     :param location: The saving location for the data.
-    :param delay: The delay for the process.
-    :param cancel: The cancel time for the loops.
+    :param delay: The delay between each data fetching request.
+    :param length: The length of the data to get in each request.
+    :param options: The ccxt options.
+    :param cancel: The time it takes to cancel a non-updating screener.
 
     :return: The market screener object.
     """
 
-    screener = MarketScreener(
-        recorder=recorder or MarketRecorder(
-            market=market or create_market(data=data)
+    screener = MarketOHLCVScreener(
+        recorder=recorder or MarketOHLCVRecorder(
+            market=market or create_ohlcv_market(data=data)
         ),
-        handler=handler, location=location, amount=amount,
-        cancel=cancel, delay=delay, limited=limited, refresh=refresh
-    )
-
-    screener.add_feeds(
-        data=screener.recorder.structure(), fixed=fixed,
-        separator=separator, parameters=parameters
+        location=location, cancel=cancel, delay=delay,
+        options=options, pro=pro, interval=interval, length=length
     )
 
     return screener
-# end market_recorder
+# end market_order_book_recorder
```

### Comparing `auto-screener-0.1.2/auto_screener/interval.py` & `auto-screener-0.2.0/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener/screener.py` & `auto-screener-0.2.0/auto_screener/screener.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 # screener.py
 
-import os
 import warnings
 import datetime as dt
 import time
 from abc import ABCMeta
 import threading
 from typing import (
     Optional, Union, Dict, Iterable, Any, List
 )
 
 import pandas as pd
 
 from represent import BaseModel, Modifiers
 
+from multithreading import Caller, Callers, multi_threaded_calls
+
 from auto_screener.dataset import (
     DATE_TIME, save_dataset, load_dataset
 )
 from auto_screener.hints import Number
-from auto_screener.collect import validate_symbol
+from auto_screener.collect import (
+    find_name, validate_exchange, validate_symbol
+)
 
 __all__ = [
     "BaseScreener",
     "wait_for_update",
     "wait_for_initialization",
     "WaitingState",
     "DataCollector",
     "collect_screeners",
     "wait_for_dynamic_update",
     "wait_for_dynamic_initialization",
     "BaseMultiScreener",
     "live_screeners",
     "create_market_dataframe",
     "structure_screeners",
-    "find_screeners"
+    "find_screeners",
+    "MarketRecorder",
+    "structure_screeners_datasets",
+    "structure_screener_datasets",
+    "validate_market"
 ]
 
 class WaitingState(BaseModel):
     """A class to represent the waiting state of screener objects."""
 
     modifiers = Modifiers(excluded=["create_screeners"])
 
@@ -108,26 +115,36 @@
         Defines the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         """
 
-        self.cancel = cancel or self.CANCEL
-        self.delay = delay or self.DELAY
+        if delay is None:
+            delay = self.DELAY
+        # end if
+
+        if cancel is None:
+            cancel = self.CANCEL
+        # end if
+
+        self.cancel = cancel
+        self.delay = delay
 
         self.location = location or self.LOCATION
 
         self.running = False
         self.block = False
         self.saving = False
+        self.updating = False
 
         self.screening_process = None
         self.timeout_process = None
         self.saving_process = None
+        self.update_process = None
     # end __init__
 
     def __getstate__(self) -> Dict[str, Any]:
         """
         Returns the data of the object.
 
         :return: The state of the object.
@@ -158,14 +175,18 @@
         """Runs the process of the price screening."""
     # end run_loop
 
     def saving_loop(self) -> None:
         """Runs the process of the price screening."""
     # end saving_loop
 
+    def update_loop(self) -> None:
+        """Updates the state of the screeners."""
+    # end update_loop
+
     def wait_for_initialization(
             self,
             delay: Optional[Union[Number, dt.timedelta]] = None,
             once: Optional[bool] = False,
             stop: Optional[Union[bool, int]] = False,
             cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
     ) -> WaitingState:
@@ -212,50 +233,68 @@
             self, delay=delay, once=once,
             stop=stop, cancel=cancel or self.cancel
         )
     # end wait_for_update
 
     def run(
             self,
+            start: Optional[bool] = True,
             save: Optional[bool] = True,
             block: Optional[bool] = False,
+            update: Optional[bool] = True,
             wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
             timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
-    ) -> threading.Thread:
+    ) -> None:
         """
         Runs the process of the price screening.
 
+        :param start: The value to start the screening.
         :param save: The value to save the data.
         :param wait: The value to wait after starting to run the process.
         :param block: The value to block the execution.
+        :param update: The value to update the screeners.
         :param timeout: The valur to add a timeout to the process.
         """
 
         if self.running:
             warnings.warn(f"Screener object {self} is already running.")
 
             return self.screening_process
         # end if
 
-        self.running = True
+        if start:
+            self.running = True
 
-        self.screening_process = threading.Thread(target=self.run_loop)
+            self.screening_process = threading.Thread(
+                target=self.run_loop
+            )
 
-        self.screening_process.start()
+            self.screening_process.start()
+        # end if
 
         if save:
             self.saving = True
 
             self.saving_process = threading.Thread(
                 target=self.saving_loop
             )
 
             self.saving_process.start()
         # end if
 
+        if update:
+            self.updating = True
+
+            self.update_process = threading.Thread(
+                target=self.update_loop
+            )
+
+            self.update_process.start()
+        # end if
+
         if timeout:
             self.timeout(timeout)
         # end if
 
         if block:
             self.block = block
 
@@ -274,16 +313,14 @@
 
         if isinstance(wait, bool) and wait:
             self.wait_for_initialization()
 
         elif isinstance(wait, (int, float)):
             time.sleep(wait)
         # end if
-
-        return self.screening_process
     # end run
 
     def timeout(
             self, duration: Union[Number, dt.timedelta, dt.datetime]
     ) -> threading.Thread:
         """
         Runs a timeout for the process.
@@ -503,19 +540,167 @@
         while self.saving:
             start = time.time()
 
             self.save_dataset()
 
             end = time.time()
 
-            time.sleep(max(delay - (end - start), 0) or 1)
+            time.sleep(max(delay - (end - start), 1))
         # end while
     # end run_loop
 # end BaseScreener
 
+Market = Dict[str, Dict[str, pd.DataFrame]]
+
+def validate_market(data: Any) -> Dict[str, Iterable[str]]:
+    """
+    Validates the data.
+
+    :param data: The data to validate.
+
+    :return: The valid data.
+    """
+
+    if data is None:
+        return {}
+    # end if
+
+    try:
+        if not isinstance(data, dict):
+            raise ValueError
+        # end if
+
+        new_data = {}
+
+        for key, values in data.items():
+            if not (
+                isinstance(key, str) and
+                all(isinstance(value, str) for value in values)
+            ):
+                raise ValueError
+            # end if
+        # end for
+
+    except (TypeError, ValueError):
+        raise ValueError(
+            f"Exchanges data must be a dictionary of "
+            f"exchange names as keys and iterables of "
+            f"symbol names as values, not {data}."
+        )
+    # end try
+
+    return new_data
+# end validate_market
+
+class MarketRecorder(BaseModel):
+    """
+    A class to represent a crypto data feed recorder.
+    This object passes the record method to the handler object to record
+    the data fetched by the handler.
+
+    Parameters:
+
+    - market:
+        The market structure of the data to store the fetched data in.
+        This structure is a dictionary with exchange names as keys
+        and dictionaries as values, where their keys are symbols,
+        and their values are the dataframes to record the data.
+
+    >>> from auto_screener.feed import market_order_book_recorder
+    >>>
+    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
+    >>>
+    >>> recorder = market_order_book_recorder(data=market)
+
+    """
+
+    modifiers = Modifiers(**BaseModel.modifiers)
+    modifiers.excluded.append("market")
+
+    __slots__ = "market"
+
+    def __init__(self, market: Optional[Market] = None) -> None:
+        """
+        Defines the class attributes.
+
+        :param market: The object to fill with the crypto feed record.
+        """
+
+        if market is None:
+            market = {}
+        # end if
+
+        validate_market(data=market)
+
+        self.market: Market = market
+    # end __init__
+
+    def structure(self) -> Dict[str, List[str]]:
+        """
+        Returns the structure of the market data.
+
+        :return: The structure of the market.
+        """
+
+        return {
+            exchange: list(symbols.keys())
+            for exchange, symbols in self.market.items()
+        }
+    # end structure
+
+    def data(self, exchange: str, symbol: str) -> pd.DataFrame:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
+        """
+
+        exchange = find_name(name=exchange, names=self.market.keys())
+
+        validate_exchange(
+            exchange=exchange,
+            exchanges=self.market.keys(),
+            provider=self
+        )
+
+        validate_symbol(
+            symbol=symbol,
+            exchange=exchange,
+            exchanges=self.market.keys(),
+            symbols=self.market[exchange],
+            provider=self
+        )
+
+        return self.market[exchange][symbol]
+    # end data
+
+    def in_market(self, exchange: str, symbol: str) -> bool:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
+        """
+
+        try:
+            self.data(exchange=exchange, symbol=symbol)
+
+            return True
+
+        except ValueError:
+            return False
+        # end try
+    # end in_market
+# end MarketRecorder
+
 class BaseMultiScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
@@ -538,14 +723,15 @@
     screeners: List[BaseScreener]
 
     __slots__ = "screeners", "location", "cancel", "delay"
 
     def __init__(
             self,
             screeners: Optional[Iterable[BaseScreener]] = None,
+            recorder: Optional[MarketRecorder] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
             delay: Optional[Union[Number, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -553,54 +739,85 @@
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         """
 
         super().__init__(location=location, cancel=cancel, delay=delay)
 
         self.screeners = list(screeners or [])
+
+        self.recorder = recorder or MarketRecorder(
+            market=structure_screener_datasets(screeners=self.screeners)
+        )
     # end __init__
 
-    def load_datasets(self, location: Optional[str] = None) -> None:
+    @property
+    def market(self) -> Dict[str, Dict[str, pd.DataFrame]]:
         """
-        Loads the datasets of the create_screeners.
+        Returns the market to hold the recorder data.
 
-        :param location: The saving or loading path for the dataset.
+        :return: The market object.
         """
 
+        return self.recorder.market
+    # end market
+
+    def connect_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+
         for screener in self.screeners:
-            if os.path.exists(screener.dataset_path() or location):
-                try:
-                    screener.load_dataset(
-                        location=location or self.location or screener.location
-                    )
-
-                except Exception as e:
-                    warnings.warn(str(e))
-                # end try
-            # end if
+            screener.market = self.recorder.data(
+                exchange=screener.exchange, symbol=screener.symbol
+            )
         # end for
-    # end load_datasets
+    # end connect_screeners
 
     def save_datasets(self, location: Optional[str] = None) -> None:
         """
-        Saves the datasets of the create_screeners.
+        Runs the data handling loop.
 
-        :param location: The saving or loading path for the dataset.
+        :param location: The saving location.
         """
 
+        callers = []
+
         for screener in self.screeners:
-            try:
-                screener.save_dataset(
-                    location=location or self.location or screener.location
+            location = location or screener.location or self.location
+
+            callers.append(
+                Caller(
+                    caller=screener.save_dataset,
+                    kwargs=dict(location=location)
                 )
+            )
+        # end for
+
+        multi_threaded_calls(callers=Callers(callers=callers))
+    # end save_datasets
+
+    def load_datasets(self, location: Optional[str] = None) -> None:
+        """
+        Runs the data handling loop.
+
+        :param location: The saving location.
+        """
+
+        callers = []
 
-            except Exception as e:
-                warnings.warn(str(e))
-            # end try
+        for screener in self.screeners:
+            location = location or screener.location or self.location
+
+            callers.append(
+                Caller(
+                    caller=screener.load_dataset,
+                    kwargs=dict(location=location)
+                )
+            )
         # end for
+
+        multi_threaded_calls(callers=Callers(callers=callers))
     # end load_datasets
 # end BaseScreener
 
 def collect_screeners(
         symbol: str,
         exchange: str,
         screeners: Iterable[BaseScreener]
@@ -919,14 +1136,62 @@
             setdefault(screener.symbol, [])
         ).append(screener)
     # end for
 
     return structure
 # end structure_screeners
 
+def structure_screeners_datasets(
+        screeners: Iterable[BaseScreener]
+) -> Dict[str, Dict[str, List[pd.DataFrame]]]:
+    """
+    Structures the screener objects by exchanges and symbols
+
+    :param screeners: The screeners to structure.
+
+    :return: The structure of the screeners.
+    """
+
+    structure: Dict[str, Dict[str, List[pd.DataFrame]]] = {}
+
+    for screener in screeners:
+        (
+            structure.
+            setdefault(screener.exchange, {}).
+            setdefault(screener.symbol, [])
+        ).append(screener.market)
+    # end for
+
+    return structure
+# end structure_screeners_datasets
+
+def structure_screener_datasets(
+        screeners: Iterable[BaseScreener]
+) -> Dict[str, Dict[str, pd.DataFrame]]:
+    """
+    Structures the screener objects by exchanges and symbols
+
+    :param screeners: The screeners to structure.
+
+    :return: The structure of the screeners.
+    """
+
+    structure: Dict[str, Dict[str, pd.DataFrame]] = {}
+
+    for screener in screeners:
+        (
+            structure.
+            setdefault(screener.exchange, {}).
+            setdefault(screener.symbol, screener.market)
+        )
+    # end for
+
+    return structure
+# end structure_screener_datasets
+
 def find_screeners(
         screeners: Iterable[BaseScreener], exchange: str, symbol: str
 ) -> List[BaseScreener]:
     """
     Finds all the screeners with the matching exchange and symbol name.
 
     :param screeners: The screeners to process.
```

### Comparing `auto-screener-0.1.2/auto_screener/symbols.py` & `auto-screener-0.2.0/auto_screener/symbols.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.2.0/auto_screener.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.1.2
+Version: 0.2.0
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.1.2/auto_screener.egg-info/SOURCES.txt` & `auto-screener-0.2.0/auto_screener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/build.py` & `auto-screener-0.2.0/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.2/pyproject.toml` & `auto-screener-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.1.2'
+version = '0.2.0'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.1.2/setup.py` & `auto-screener-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.1.2',
+        version='0.2.0',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

