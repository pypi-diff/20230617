# Comparing `tmp/pandaxt-0.1.5.tar.gz` & `tmp/pandaxt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandaxt-0.1.5.tar", last modified: Mon Jan 28 19:44:42 2019, max compression
+gzip compressed data, was "dist/pandaxt-0.1.6.tar", last modified: Mon Jan 28 18:11:04 2019, max compression
```

## Comparing `pandaxt-0.1.5.tar` & `pandaxt-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 19:44:42.000000 pandaxt-0.1.5/
--rw-r--r--   0 godmin    (1001) godmin    (1001)      160 2019-01-28 19:06:39.000000 pandaxt-0.1.5/.gitignore
--rw-r-----   0 godmin    (1001) godmin    (1001)     1210 2018-11-09 14:44:11.000000 pandaxt-0.1.5/LICENSE
--rw-r--r--   0 godmin    (1001) godmin    (1001)      634 2019-01-28 19:44:42.000000 pandaxt-0.1.5/PKG-INFO
--rw-r--r--   0 godmin    (1001) godmin    (1001)     1143 2019-01-28 18:53:13.000000 pandaxt-0.1.5/README.md
-drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 19:44:42.000000 pandaxt-0.1.5/doc/
--rw-r--r--   0 godmin    (1001) godmin    (1001)      815 2019-01-05 18:31:58.000000 pandaxt-0.1.5/doc/orders.md
-drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt/
--rw-r--r--   0 godmin    (1001) godmin    (1001)      613 2019-01-28 18:11:32.000000 pandaxt-0.1.5/pandaxt/__init__.py
--rw-r--r--   0 godmin    (1001) godmin    (1001)    28701 2019-01-28 19:08:25.000000 pandaxt-0.1.5/pandaxt/core.py
--rw-r--r--   0 godmin    (1001) godmin    (1001)     9502 2019-01-28 19:14:19.000000 pandaxt-0.1.5/pandaxt/utils.py
-drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt.egg-info/
--rw-r--r--   0 godmin    (1001) godmin    (1001)      634 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt.egg-info/PKG-INFO
--rw-r--r--   0 godmin    (1001) godmin    (1001)      285 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt.egg-info/SOURCES.txt
--rw-r--r--   0 godmin    (1001) godmin    (1001)       37 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt.egg-info/dependency_links.txt
--rw-r-----   0 godmin    (1001) godmin    (1001)       43 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt.egg-info/requires.txt
--rw-r--r--   0 godmin    (1001) godmin    (1001)        8 2019-01-28 19:44:42.000000 pandaxt-0.1.5/pandaxt.egg-info/top_level.txt
--rw-r--r--   0 godmin    (1001) godmin    (1001)       50 2019-01-27 19:33:37.000000 pandaxt-0.1.5/requirements.txt
--rw-r-----   0 godmin    (1001) godmin    (1001)      102 2019-01-28 19:44:42.000000 pandaxt-0.1.5/setup.cfg
--rw-r--r--   0 godmin    (1001) godmin    (1001)      975 2019-01-05 18:46:28.000000 pandaxt-0.1.5/setup.py
+drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 18:11:04.000000 pandaxt-0.1.6/
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      132 2019-01-28 18:09:52.000000 pandaxt-0.1.6/.gitignore
+-rw-r-----   0 godmin    (1001) godmin    (1001)     1210 2018-11-09 14:44:11.000000 pandaxt-0.1.6/LICENSE
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      634 2019-01-28 18:11:04.000000 pandaxt-0.1.6/PKG-INFO
+-rw-r--r--   0 godmin    (1001) godmin    (1001)     1143 2019-01-28 18:09:51.000000 pandaxt-0.1.6/README.md
+drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 18:11:04.000000 pandaxt-0.1.6/doc/
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      815 2019-01-05 18:31:58.000000 pandaxt-0.1.6/doc/orders.md
+drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 18:11:04.000000 pandaxt-0.1.6/pandaxt/
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      613 2019-01-28 18:10:44.000000 pandaxt-0.1.6/pandaxt/__init__.py
+-rw-r--r--   0 godmin    (1001) godmin    (1001)    31139 2019-01-27 23:06:28.000000 pandaxt-0.1.6/pandaxt/core.py
+-rw-r-----   0 godmin    (1001) godmin    (1001)     2004 2019-01-27 22:59:13.000000 pandaxt-0.1.6/pandaxt/decorators.py
+-rw-r--r--   0 godmin    (1001) godmin    (1001)     9320 2019-01-05 18:38:43.000000 pandaxt-0.1.6/pandaxt/utils.py
+drwxr-xr-x   0 godmin    (1001) godmin    (1001)        0 2019-01-28 18:11:04.000000 pandaxt-0.1.6/pandaxt.egg-info/
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      634 2019-01-28 18:11:03.000000 pandaxt-0.1.6/pandaxt.egg-info/PKG-INFO
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      307 2019-01-28 18:11:03.000000 pandaxt-0.1.6/pandaxt.egg-info/SOURCES.txt
+-rw-r--r--   0 godmin    (1001) godmin    (1001)       37 2019-01-28 18:11:03.000000 pandaxt-0.1.6/pandaxt.egg-info/dependency_links.txt
+-rw-r-----   0 godmin    (1001) godmin    (1001)       43 2019-01-28 18:11:03.000000 pandaxt-0.1.6/pandaxt.egg-info/requires.txt
+-rw-r--r--   0 godmin    (1001) godmin    (1001)        8 2019-01-28 18:11:03.000000 pandaxt-0.1.6/pandaxt.egg-info/top_level.txt
+-rw-r--r--   0 godmin    (1001) godmin    (1001)       50 2019-01-27 19:33:37.000000 pandaxt-0.1.6/requirements.txt
+-rw-r-----   0 godmin    (1001) godmin    (1001)      102 2019-01-28 18:11:04.000000 pandaxt-0.1.6/setup.cfg
+-rw-r--r--   0 godmin    (1001) godmin    (1001)      975 2019-01-05 18:46:28.000000 pandaxt-0.1.6/setup.py
```

### Comparing `pandaxt-0.1.5/LICENSE` & `pandaxt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pandaxt-0.1.5/PKG-INFO` & `pandaxt-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pandaxt
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 A Python 3 "ccxt" wrapper over "Pandas" lib.
 
 Home-page: https://github.com/havocesp/pandaxt
 Author: Daniel J. Umpierrez
 Author-email: umpierrez@pm.me
 License: UNLICENSE
```

### Comparing `pandaxt-0.1.5/README.md` & `pandaxt-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PandaXT
 
 A Python 3 "__ccxt__" wrapper over __Pandas__ lib.
 
  - Author: Daniel J. Umpierrez
  - License: UNLICENSE
- - Version: 0.1.5
+ - Version: 0.1.6
 
 ## Description
 
 Python ccxt multi-exchange lib mixed with pandas lib for data handling.
 
 ## Requirements
 
@@ -28,15 +28,15 @@
 
 ```
 
 ## Changelog
 
 Project changes over versions.
 
-### 0.1.5
+### 0.1.6
 - Many features added and many errors fixed
 
 ### 0.1.4
 - New "model" module.
 - Added dict2class in "utils" module.
 
 ### 0.1.3
```

### Comparing `pandaxt-0.1.5/doc/orders.md` & `pandaxt-0.1.6/doc/orders.md`

 * *Files identical despite different names*

### Comparing `pandaxt-0.1.5/pandaxt/__init__.py` & `pandaxt-0.1.6/pandaxt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pandaxt.core import PandaXT
 
 
 __project__ = 'PandaXT'
 __package__ = 'pandaxt'
 __author__ = 'Daniel J. Umpierrez'
 __license__ = 'UNLICENSE'
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 __description__ = __doc__
 __site__ = 'https://github.com/havocesp/{}'.format(__package__)
 __email__ = 'umpierrez@pm.me'
 __keywords__ = ['altcoins', 'altcoin', 'exchange', 'pandas', 'bitcoin', 'trading']
 
 __all__ = ['__description__', '__author__', '__license__', '__version__', '__package__', '__project__', '__site__',
            '__email__', '__keywords__', 'PandaXT']
```

### Comparing `pandaxt-0.1.5/pandaxt/core.py` & `pandaxt-0.1.6/pandaxt/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # -*- coding:utf-8 -*-
 """Core module."""
+import collections
 import functools
 import os
 import pathlib
 import warnings
 from collections import OrderedDict, UserDict, Iterable
 
 import ccxt
 import pandas as pd
 import tulipy
 from cctf import Symbol, Tickers, Currency, Balance, Wallet, Markets, Market, Ticker
 from diskcache import Cache
 from pandas.core.common import SettingWithCopyWarning
-from pandaxt.utils import load_dotenv, magic2num, get_tor_session
+# from cctf import Market, Symbol, Currency, Ticker, Markets, Wallet, Tickers
+from pandaxt.decorators import retry
+from pandaxt.utils import load_dotenv, magic2num, get_tor_session, error  # , find_nearest
 
 warnings.simplefilter(action='ignore', category=SettingWithCopyWarning)
 
-# noinspection PyUnusedName
+# log = Logger('PandaXT', 'INFO')
+_COLORS = ("red", "green", "yellow", "blue", "magenta", "cyan")
+
 pd.options.display.precision = 8
-# noinspection PyUnusedName
 pd.options.display.max_colwidth = -1
-# noinspection PyUnusedName
 pd.options.display.float_format = lambda n: '{:.8f}'.format(n).rstrip('0.') if n < 0.0 else '{:.8f}'.format(n)
 
 _OHLC_FIELDS = ['date', 'open', 'high', 'low', 'close', 'volume']
 _USER_DATA_DIR = pathlib.Path.home().joinpath('.local', 'share')
 _SETTINGS = dict(config=dict(timeout=25000, enableRateLimit=True, fetchTickersErrors=False))
 
-__all__ = ['PandaXT', 'Exchanges', 'Exchange']
+__all__ = ['PandaXT']
 
 
 def _get_version(exchange):
     """Exchange CCXT id validator an sanitizer.
 
     If exchange is found in CCXT supported exchange list and exchange has only one API api version, exchange value
     will be returned as is.
@@ -49,15 +52,16 @@
 
 
 # noinspection PyUnusedFunction,PySameParameterValue
 class PandaXT:
     """A "ccxt" exchanges wrapper class over Pandas lib."""
 
     def __init__(self, exchange, load_keys=True, tor=False, user_agent=None):
-        """Constructor.
+        """
+        Constructor.
 
         >>> markets = PandaXT('binance').markets
         >>> isinstance(markets, Markets)
         True
         >>> market = markets.get('BTC/USDT')  # type: Market
         >>> isinstance(market, Market)
         True
@@ -126,26 +130,26 @@
 
         :param str exchange: exchange name to be checked.
         """
         if isinstance(exchange or 0, str) and len(exchange) > 0:
             return any([str(exchange) == e for e in ccxt.exchanges])
         else:
             return False
-
     @property
     def id(self):
         """Exchange unique reference (also know as ID).
 
         >>> PandaXT('binance').id
         'binance'
 
         :return Text: exchange unique reference.
         """
         return self._api.id
 
+
     @property
     def timeframes(self):
         """Return valid exchange timeframes as list.
 
         >>> '15m' in PandaXT('binance').timeframes
         True
 
@@ -180,14 +184,15 @@
         'Binance'
 
         :return Text: exchange long name.
         """
         return getattr(self._api, 'name')
 
     @property
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def markets(self):
         """Get all exchange markets metadata.
 
         >>> isinstance(PandaXT('binance').markets, Markets)
         True
 
         :return Dict: all exchange markets metadata.
@@ -202,27 +207,28 @@
             self._cache.set('markets', data, (60.0 ** 2.0) * 6.0)
         if not len(self._symbols):
             self._symbols = [self.altname(s) for s in sorted(data)]
             self.basemarkets = list({s.quote for s in self._symbols})
             self.currencies = list({s.base for s in self._symbols})
         return Markets(**data) if not isinstance(data, Markets) else data
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def _fetch_ohlcv(self, symbol, timeframe='15m', since=None, limit=None, params=None):
         """See `Exchange` fetch_ohlcv from ccxt lib.
 
         :param symbol:
         :param timeframe:
         :param since:
         :param limit:
         :param params:
         :type symbol: Text or Symbol
         :type timeframe: Text
         :type limit: int
         :type params: Dict
-        :return list: OHLCV data as list
+        :return:
         """
         if not self._api.has['fetchTrades']:
             self._api.raise_error(ccxt.NotSupported, details='fetch_ohlcv() not implemented yet')
 
         timeframe2seconds = self._api.parse_timeframe(timeframe) * limit * 2
         trades = self._api.fetch_trades(symbol, since=timeframe2seconds * 1000, params=params or dict())
 
@@ -231,16 +237,18 @@
     def get_timeframe(self, timeframe):
         # timeframe = find_nearest(self._api.timeframes.values(), value)
         if isinstance(timeframe, int):
             timeframe = '{}m'.format(timeframe)
         # elif str(timeframe)[-1] in list('mhwMd'):
         return str(timeframe) in self.timeframes
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_ohlc(self, symbol, timeframe='5m', limit=25):
-        """Get OHLC data for specific symbol as pandas DataFrame type.
+        """
+        Get OHLC data for specific symbol as pandas DataFrame type.
 
         :param Text symbol: symbol name use at ohlc data request.
         :param Text timeframe: an exchange supported timeframe.
         :param int limit: max rows limit.
         :return pd.DataFrame: DataFrame with timestamps a index and columns: open, high, low, close, volume, qvolume
         """
 
@@ -282,52 +290,55 @@
         else:
             c = ccc(str(name))
             if c == 'BSV':
                 c = 'BCHSV'
             return Currency(c)
 
     def cost2precision(self, symbol, cost, to_str=True):
-        """Return cost rounded to symbol precision exchange specifications.
+        """
+        Return cost rounded to symbol precision exchange specifications.
 
         :param symbol: a valid exchange symbol.
         :type symbol: Text or Symbol
         :param float cost: cost to be rounded.
-        :param Bool to_str: True to return result as str, otherwise result will be returned as float
         :return float: cost rounded to specific symbol exchange specifications.
         """
         t = str if to_str else float
         return t(self._api.cost_to_precision(symbol, cost))
 
     def amount2precision(self, symbol, amount, to_str=True):
-        """Return amount rounded to symbol precision exchange specifications.
+        """
+        Return amount rounded to symbol precision exchange specifications.
 
         :param symbol: a valid exchange symbol.
         :type symbol: Text or Symbol
         :param amount: amount to be rounded.
-        :param Bool to_str: True to return result as str, otherwise result will be returned as float
+        :param bool to_str: True to return result as str, otherwise result will be returned as float
         :return: amount rounded to specific symbol exchange specifications.
         :rtype: float or Text
         """
         t = str if to_str else float
         return t(self._api.amount_to_precision(symbol, amount))
 
     def price2precision(self, symbol, price, to_str=True):
-        """Return price rounded to symbol precision exchange specifications.
+        """
+        Return price rounded to symbol precision exchange specifications.
 
         :param symbol: a valid exchange symbol.
         :type symbol: Text or Symbol
         :param price: price to be rounded.
         :param Bool to_str: True to return result as str, otherwise result will be returned as float
         :return float: price rounded to specific symbol exchange specifications.
         """
         m = self.markets.get(symbol)  # type: Market
         t = str if to_str else float
         template = '{:.@f}'.replace('@', str(m.precision.price))
         return t(template.format(float(price)))
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_orderbook(self, symbol, limit=5):
         """Get order book data for a symbol.
 
         >>> book_entries = PandaXT('binance').get_orderbook('MDA/BTC', 5)
         >>> isinstance(book_entries['ask'].values[-1], float)
         True
 
@@ -341,63 +352,72 @@
         raw = self._api.fetch_order_book(symbol, limit=int(limit))
 
         columns = ['ask', 'ask_vol', 'bid', 'bid_vol']
         data = [ask + bid for ask, bid in zip(raw['asks'], raw['bids'])]
         df = pd.DataFrame(data, columns=columns)
         return df.round({'ask': 8, 'bid': 8, 'ask_vol': 0, 'bid_vol': 0})
 
+    # @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_tickers(self, symbols, sorted_by=None):
         """Get tickers dict with symbol name as keys for all symbols specified as positional args.
 
         >>> exchange = PandaXT('binance')
         >>> ticker = exchange.get_tickers("ADA/BTC", sorted_by='percentage')
         >>> isinstance(ticker, Ticker)
         True
 
         :param symbols: list of valid exchange symbols.
         :type symbols: Iterable
         :param sorted_by: a valid ticker field like percentage, last, ask, bid, quoteVolume, ...
         :return: Ticker or Tickers instance with returned data.
         :rtype: Ticker or Tickers
         """
-        return_value = list()
+        result = list()
 
         if isinstance(symbols, Iterable) and len(symbols):
             symbols = [symbols] if isinstance(symbols, str) else list(symbols)
 
             for s in map(str, symbols):
                 if s not in self.markets:
-                    print(f'Symbol {s or "NULL"} is not listed in {self.name} exchange.')
+                    print('Symbol {} is not listed in {} exchange.'.format(s or 'NULL', self.name))
             try:
                 raw = self._api.fetch_tickers(symbols)
+                # if hitbtc in self.id:
+                #     raw['ask'] = raw['info']['ask']
+                #     raw['bid'] = raw['info']['bid']
+                #     raw['last'] = float((raw['ask'] + raw['bid'])/2.0)
                 if str(sorted_by) in list(raw.values())[0].keys():
                     raw = OrderedDict(sorted(raw.items(), key=lambda k: k[1][sorted_by], reverse=True))
-                return_value = Tickers(**raw)
-                return_value = return_value[symbols[0]] if len(symbols) == 1 else return_value
+                result = Tickers(**raw)
+                result = result[symbols[0]] if len(symbols) == 1 else result
             except ccxt.ExchangeError as err:
                 print(str(err))
 
-        return return_value
+        return result
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_indicators(self, indicators, symbol, timeframe='15m', limit=25, **kwargs):
         """Get technical indicators value for a symbol.
 
+        Indicators params should be supplied
+
         :param Dict indicators: indicators and their params as dict (params ara mandatory, there is no default values).
         :param Text symbol: a valid exchange symbol.
         :param Text timeframe: an exchange valid timeframe (default 15m).
         :param int limit: a valid exchange limit for returned rows (check exchange official API)
+        :param indicators_params: dict instance containing indicator / params key pair where params (if any) will be
         supplied as a param / value dict instance also. Example: "{'roc': {'period': 9}}"
         :param kwargs: if "ohlc" is set with OHLC data (DataFrame) it will be use for value calculations.
         :return Dict: dict type with indicators name/value pairs.
         """
         indicator_names = indicators.keys()
         indicators = {k.lower(): v for k, v in indicators.items()}
         symbol = Symbol(symbol)
-        return_value = OrderedDict.fromkeys(indicators.keys())
-        supported_ti = [_a for _a in dir(tulipy.lib) if _a[0].islower()]
+        result = OrderedDict.fromkeys(indicators.keys())
+        supported_ti = [a for a in dir(tulipy.lib) if a[0].islower()]
 
         functions = OrderedDict({i: getattr(tulipy, i) for i in indicators if i in supported_ti})
 
         data = kwargs.get('ohlc', self.get_ohlc(symbol, timeframe=timeframe, limit=limit))
 
         for n, fn in functions.items():
             inputs = ['close' if i in 'real' else i for i in fn.inputs]
@@ -410,86 +430,100 @@
             try:
                 raw = fn(*data[inputs].T.values, **indicator_params)
                 di = data.index
                 if n in 'roc':
                     raw = raw * 100.0
                 sr = pd.Series(raw, name=n.upper())
                 sr.index = di.values[-len(sr):]
-                return_value[n] = sr.copy(True)
+                result[n] = sr.copy(True)
 
             except tulipy.lib.InvalidOptionError as err:
                 print(str(err))
 
-        return {k: return_value[k.lower()] for k in indicator_names}
+        return {k: result[k.lower()] for k in indicator_names}
 
-    def create_market_order(self, symbol, side, amount=None):
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
+    def create_market_order(self, symbol, side):
         """Create a market order order.
 
-        :param symbol: a valid exchange symbol.
-        :type symbol: Text or Symbol
+        :param Text symbol: a valid exchange symbol.
         :param Text side: accepted values: "buy", "sell"
-        :param float amount: amount used in order creation.
         :return Dict: order creation result data as dict.
         """
-        return self.create_order(symbol, side=side, order_type='market', amount=amount)
+        symbol = Symbol(symbol)
+        side = str(side).lower()
+
+        if symbol not in self._symbols:
+            error('Invalid symbol: {}'.format(symbol))
+
+        if side not in ['buy', 'sell']:
+            error('Invalid side: {} (accepted values: "buy", "sell")'.format(side))
+
+        coin = quote if side in 'buy' else base
+        free = self.get_balance(coin, 'free') or dict()
+
+        return self._api.create_order(symbol, type='market', side=side, amount=magic2num(amount))
 
     def buy(self, symbol, amount=None, price=None):
-        """Create buy order.
+        """
+        Create buy order.
 
         :param symbol: a valid exchange symbol.
         :type symbol: str or Symbol
         :param float amount: amount to buy or None to auto-fill
         :param float price: buy price or None to auto-fill
         :return Dict: order creation result data as dict.
         """
         return self.create_order(symbol, order_type='limit', side='buy', amount=amount, price=price)
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def create_order(self, symbol, side, order_type=None, amount=None, price=None):
-        """Create a new order.
+        """
+        Create a new order.
 
         :param symbol: symbol to be use for order creation.
         :type symbol: str or Symbol
         :param Text side: order side: 'sell' or 'buy'
         :param Text order_type: order type (default 'limit')
         :param float amount: amount used in order creation.
         :param float price: price used in order creation.
-        :return Dict: order result info as dict.
+        :return Dict:
         """
         symbol = Symbol(symbol)
-        response = dict()
-        if symbol not in self._symbols:
-            raise ValueError('Invalid symbol: {}'.format(symbol))
-
-        if side not in ['buy', 'sell']:
-            raise ValueError('Invalid side: {} (accepted values: "buy", "sell")'.format(side))
-
-        currency = symbol.quote if side in 'buy' else symbol.base
-        balance_field = 'free' if side in 'buy' else 'total'
-        ticker_field = 'ask' if side in 'buy' else 'bid'
-
+        assert symbol in self._symbols, 'Invalid symbol: {}'.format(symbol)
+        base, quote = symbol.parts
+        if side in 'buy':
+            currency = quote
+            balance_field = 'free'
+            ticker_field = 'ask'
+        else:
+            balance_field = 'total'
+            ticker_field = 'bid'
+            currency = base
         amount = magic2num(amount or self.get_balances(balance_field).get(currency, 0.0))
-
         if amount > 0.0:
             price = magic2num(price or self.get_tickers(symbol).get(ticker_field))
             if side in 'buy':
                 amount = amount / price
-            response = self._api.create_order(symbol, type=order_type or 'limit', side=side, amount=amount, price=price)
-        return response
+            return self._api.create_order(symbol, type=str(order_type or 'limit'), side=side, amount=amount,
+                                          price=price)
 
     def sell(self, symbol, amount=None, price=None):
-        """Create sell order.
+        """
+        Create sell order.
 
         :param symbol: a valid exchange symbol.
         :type symbol: str or Symbol
         :param float amount: amount to sell or None to auto-fill
         :param float price: sell price or None to auto-fill
         :return dict: order creation result data as dict.
         """
         return self.create_order(symbol, order_type='limit', side='sell', amount=amount, price=price)
 
+    @retry(exceptions=ccxt.NetworkError)
     def get_balances(self, field=None):
         """Get balances.
 
         :param Text field: accepted values: if None all balances will be loaded, (values; "total", "used", "free")
         :return Wallet: positive balances.
         """
         raw = self._api.fetch_balance()
@@ -501,29 +535,48 @@
             if isinstance(v, float):
                 return v > 0.0
             else:
                 return v['total'] if 'total' in v else False
 
         return Wallet(**{str(k): v for k, v in data.items() if nonzero(v)})
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_balance(self, currency, field='total'):
         """Get balance for a currency.
 
         :param currency: a valid exchange currency.
         :type currency: Text or Currency
         :param Text field: accepted values: total, used, free
         :return Balance: currency with balance amount as float.
         """
+
         currency = Currency(str(currency))
 
         if currency not in self.currencies:
             raise ValueError('{} exchange do not support {} currency'.format(self.name.upper(), currency))
         balance_data = self.get_balances(field=field) or Balance(currency=currency, **{field: 0.0})
+        # balance_data = balance_data.get(currency, balance_data)
         return balance_data[currency]
 
+    def _calculate_fees(self, trades):
+        """
+
+        :param pd.DataFrame trades:
+        :return:
+        """
+        fee = trades.pop('fee')
+        if fee.any():
+            fee_currency = pd.Series(fee.apply(lambda v: v['currency']), index=trades.index.values, name='fee_currency')
+            trades['fee_currency'] = fee_currency
+            trades['fee_percent'] = trades.T.apply(lambda v: 0.05 if 'BNB' in v['fee_currency'] else 0.1).T
+            trades['fee_base'] = trades['fee_percent'] / 100. * trades['cost']
+            trades['total'] = trades.T.apply(
+                lambda v: v['cost'] - v['fee_base'] if v['side'] in 'sell' else v['cost'] + v['fee_base']).T
+
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_user_trades(self, symbol, limit=25):
         """Get user trades filter by symbol.
 
         :param symbol: a valid exchange symbol
         :type symbol: Text or Symbol
         :param int limit: a valid limit for rows return (please, refer to official exchange API manual for details)
         :return pd.DataFrame: user trades as pandas DataFrame type.
@@ -538,28 +591,30 @@
                 currency = fee_dict.pop('currency')
                 cost = fee_dict.pop('cost')
                 trades[idx].update(fee_currency=currency, fee_cost=cost)
             trades = pd.DataFrame(trades)
 
             return trades.sort_index(ascending=False)
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_trades(self, symbol, limit=25):
         """Get latest user trades for a symbol.
 
         :param symbol: a valid exchange symbol
         :param limit: a valid limit for rows return (please, refer to official exchange API manual for details)
         :return pd.DataFrame: latest trades for a symbol.
         """
         symbol = self.altname(symbol)
         trades = self._api.fetch_trades(symbol, limit=limit)
         if trades:
             trades = [{k: v for k, v in t.items() if k not in 'info'} for t in trades]
         trades = pd.DataFrame(trades)
         return trades.sort_index(ascending=False)
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_cost(self, symbol, **kwargs):
         """FIXME do not work well sometimes giving a bad result by unknown reason.
 
         Get weighted average (from buy trades data) cost for a symbol.
 
         >>> api = PandaXT('binance')
         >>> symbol_cost = api.get_cost('AGI/BTC')
@@ -572,65 +627,72 @@
         :return float: cost calculation result as float type.
         """
         symbol = self.altname(symbol)
         base, quote = symbol.parts if isinstance(symbol, Symbol) else Currency(symbol) + 'BTC'
 
         # reuse provided balance and trades data (for rate limit save)
         if 'balance' in kwargs:
-            cached_balance = kwargs.get('balance')  # type: Balance
-            balance = cached_balance[base] if isinstance(cached_balance, Wallet) else cached_balance
+            balance = kwargs.get('balance')  # type: Wallet
+            balance = balance[base] if isinstance(balance, Wallet) else balance
         else:
             balance = self.get_balance(base, field='total')  # type: Balance
 
-        total_balance = balance.total if balance and hasattr(balance, 'total') else balance
+        balance = balance.total if balance and hasattr(balance, 'total') else balance
 
-        if total_balance > 0.0:
+        if balance > 0.0:
+            # balance = balance.total
             trades = kwargs.get('trades', self.get_user_trades(symbol))
+
             buys = trades.query('side == "buy"')
+
+            # if "order" column is None replace it with "id" column
             if buys['order'].isna().all():
                 buys['order'].update(buys['id'])
 
             # groupby operations per column
             columns_op = dict(amount='sum', price='mean', cost='mean', timestamp='mean')
             buys = buys.groupby('order').agg(columns_op).sort_index(ascending=False)  # type: pd.DataFrame
             buys = buys[['price', 'amount']].reset_index(drop=True)
 
             for index, price, amount in buys.itertuples():
-                if total_balance - amount <= 0:
-                    if round(total_balance - amount, 8) != 0.0:
+                if balance - amount <= 0:
+                    if round(balance - amount, 8) != 0.0:
                         prices, amounts = buys[:index + 1].T.values
-                        amounts[-1] = total_balance
+                        amounts[-1] = balance
                     else:
                         prices, amounts = buys[:index + 1].T.values
                     return round(pd.np.average(prices, weights=amounts), 10)
                 else:
-                    total_balance -= amount
+                    balance -= amount
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_order_status(self, order_id, symbol=None):
         """Get order status by order_id.
 
         :param Text order_id: a valid order id.
         :param symbol: a valid exchange market
         :type symbol: str or Symbol or Market
         :return Text: order status as str. Possible values are: "closed",  "canceled", "open"
         """
         return self._api.fetch_order_status(order_id, symbol=symbol)
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_open_orders(self, symbol=None):
         """Get open orders.md for a symbol.
 
         :param symbol: symbol used in opened orders.md server query.
         :type symbol: str or Symbol
         :return List: list of open orders.md for specific symbol.
         """
         assert isinstance(symbol or 0, str) and symbol in self.symbols
         raw = self._api.fetch_open_orders(symbol)
 
         return [{Symbol(k): v for k, v in r.items() if k not in 'info'} for r in raw.copy()]
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def get_profit(self, currency):
         """Returns current profit for a currency and its weighted average buy cost.
 
         :param Text currency: a valid currency to use at profit and cost calc
         :return: current profit and weighted average buy cost as a tuple
         """
         currency = Currency(str(currency))
@@ -639,16 +701,18 @@
 
         if balance.used > 0.0:
             cost = self.get_cost(symbol=btc_symbol)
             return balance.to_btc - (cost * balance.total)
         else:
             return 0.0, 0.0
 
+    @retry(exceptions=(ccxt.NetworkError, ccxt.ExchangeError))
     def cancel_order(self, symbol, last_only=False):
-        """Cancel symbols open orders.md for a symbol.
+        """
+        Cancel symbols open orders.md for a symbol.
 
         :param symbol: the symbol with open orders.md.
         :type symbol: Bool or Symbol
         :param Bool last_only: if True, only last order sent will be cancelled.
         :return List: list of dict with data about cancellations.
         """
         symbol = Symbol(symbol)
@@ -657,18 +721,18 @@
         if len(pending_orders):
             if last_only:
                 return self._api.cancel_order(pending_orders[-1]['id'], symbol)
 
             else:
                 canceled_orders = list()
                 for p in pending_orders:
-                    return_value = self._api.cancel_order(p['id'], symbol)
+                    result = self._api.cancel_order(p['id'], symbol)
 
-                    if return_value and return_value.get('status', '') in 'cancel':
-                        canceled_orders.append({k: v for k, v in return_value.items() if v})
+                    if result and result.get('status', '') in 'cancel':
+                        canceled_orders.append({k: v for k, v in result.items() if v})
                     else:
                         self._api.cancel_order(p['id'], symbol)
                 return canceled_orders
 
     def __str__(self):
         """PandaXT instance as "str" type representation.
 
@@ -676,42 +740,41 @@
         'binance'
 
         :return Text: PandaXT instance as "str" type representation.
         """
         return self.id
 
     def __repr__(self):
-        """PandaXT instance as "str" type representation.
+        """
+        PandaXT instance as "str" type representation.
 
         >>> PandaXT('binance')
         binance
 
         :return str: PandaXT instance as "str" type representation.
         """
         return self.id
 
     def __contains__(self, item):
-        """Check if a symbol or currency is supported by exchange.
+        """
+        Check if a symbol or currency is supported by exchange.
 
         >>> exchange = PandaXT('cryptopia')
         >>> Currency('ETH') in exchange
         True
         >>> Currency('ETH/BTC') in exchange
         True
         >>> Currency('MyCOIN') in exchange
         False
 
         :param item: currency or symbol for supports checking on exchange.
         :type item: str or Currency or Symbol
         :return bool: True is item is supported, otherwise False.
         """
-        return str(item) in self.markets or str(item) in map(str, self.currencies)
-
-
-Exchange = PandaXT  # alias
+        return str(item) in self.markets.keys() or str(item) in map(str, self.currencies)
 
 
 class Exchanges(UserDict):
     """Dick like class to store multiple exchanges."""
 
     def __init__(self, **exchanges):
         """Constructor.
```

### Comparing `pandaxt-0.1.5/pandaxt/utils.py` & `pandaxt-0.1.6/pandaxt/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,21 @@
 from itertools import repeat, starmap
 
 import pandas as pd
 import requests
 
 
 def error(text=None):
-    """Print a formatted error text.
-
-    :param text: error message.
-    :type text: tp.Text
-    """
     print(' - [ERROR] {}'.format(text))
 
 
 def repeatfunc(func, times=None, *args):
     """Repeat calls to func with specified arguments.
 
     Example:  repeatfunc(random.random)
-
-    :param tp.Callable func:
-    :param int times:
     """
     if times is None:
         return starmap(func, repeat(args))
     return starmap(func, repeat(args, times))
 
 
 def get_timeframe(d, tf):
@@ -51,24 +43,22 @@
 
     by_unit = pd.np.asarray(d)
     idx = (pd.np.abs(by_unit - value)).argmin()
     return [idx]
 
 
 def whoami():
-    """Return function name where this function is called.
-
-    :return str: caller function name.
-    """
+    """Return function name where this function is called."""
     frame = inspect.currentframe()
     return inspect.getframeinfo(frame).function
 
 
 def drop_keys(it, *keys):
-    """Remove specified "keys" from any iterable type (tuple, list, dict, ...).
+    """
+    Remove specified "keys" from any iterable type (tuple, list, dict, ...).
 
     :param tp.Iterable it: iterable containing dict type instances (or similar)
     :param tp.List[tp.AnyStr] keys: keys to be dropped.
     :return tp:Iterable: iterable "it" after keys deletion.
     """
     if it is not None:
         if isinstance(it, col.Mapping) and len(it):
@@ -81,15 +71,16 @@
         elif isinstance(it, tp.Iterable):
             return [drop_keys(v) if isinstance(v, col.Mapping) else v for v in it]
     else:
         return it
 
 
 def flt(value, p=None, as_str=False):
-    """Float builtin wrapper for precision param initialization.
+    """
+    Float builtin wrapper for precision param initialization.
 
     >>> flt(4.13, 5, False)
     4.13
     >>> flt(4.13, 5, True)
     '4.13'
     >>> flt(4, 5, True)
     '4'
@@ -115,15 +106,16 @@
         except ValueError:
             return value
     else:
         return value
 
 
 def infer_precision(number):
-    """Infer precision base on number size.
+    """
+    Infer precision base on number size.
 
     >>> infer_precision(0.343)
     3
     >>> infer_precision(0.0001343)
     5
     >>> infer_precision(12300)
     0
@@ -150,24 +142,25 @@
         elif number < 1000.0:
             return 1
         else:
             return 0
 
 
 def num2str(n, precision=None):
-    """Numeric type infer and parser
+    """
+    Numeric type infer and parser
 
     Accept any Iterable (dict, list, tuple, set, ...) or built-in data types int, float, str, ... and try  to
     convert it a number data type (int, float)
 
     >>> num2str(['10.032', '10.32032', '11.392', '13'])
     [10.03, 10.32, 11.39, 13]
 
     :param n: number
-    :type n: float or int or Iterable
+    :type n: Number or tp.Iterable
     :param int precision:
     :return tp.Iterable:
     """
     if n is not None:
         if isinstance(n, str):
             backup = type(n)(n)
             try:
```

### Comparing `pandaxt-0.1.5/pandaxt.egg-info/PKG-INFO` & `pandaxt-0.1.6/pandaxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pandaxt
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 A Python 3 "ccxt" wrapper over "Pandas" lib.
 
 Home-page: https://github.com/havocesp/pandaxt
 Author: Daniel J. Umpierrez
 Author-email: umpierrez@pm.me
 License: UNLICENSE
```

### Comparing `pandaxt-0.1.5/setup.py` & `pandaxt-0.1.6/setup.py`

 * *Files identical despite different names*

