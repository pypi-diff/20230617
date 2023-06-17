# Comparing `tmp/talkytrend-1.3.1.tar.gz` & `tmp/talkytrend-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.3.1.tar", max compression
+gzip compressed data, was "talkytrend-1.3.2.tar", max compression
```

## Comparing `talkytrend-1.3.1.tar` & `talkytrend-1.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-15 19:54:26.676061 talkytrend-1.3.1/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-15 19:54:26.676061 talkytrend-1.3.1/README.md
--rw-r--r--   0        0        0     1720 2023-06-15 19:54:41.769239 talkytrend-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-15 19:54:41.769239 talkytrend-1.3.1/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-15 19:54:26.676061 talkytrend-1.3.1/talkytrend/config.py
--rw-r--r--   0        0        0      951 2023-06-15 19:54:26.676061 talkytrend-1.3.1/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6121 2023-06-15 19:54:26.676061 talkytrend-1.3.1/talkytrend/main.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-17 12:42:45.764912 talkytrend-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-17 12:42:45.764912 talkytrend-1.3.2/README.md
+-rw-r--r--   0        0        0     1720 2023-06-17 12:43:03.493221 talkytrend-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-17 12:43:03.493221 talkytrend-1.3.2/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-17 12:42:45.764912 talkytrend-1.3.2/talkytrend/config.py
+-rw-r--r--   0        0        0      932 2023-06-17 12:42:45.764912 talkytrend-1.3.2/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6121 2023-06-17 12:42:45.764912 talkytrend-1.3.2/talkytrend/main.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.3.2/PKG-INFO
```

### Comparing `talkytrend-1.3.1/LICENSE` & `talkytrend-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.1/README.md` & `talkytrend-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.1/pyproject.toml` & `talkytrend-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.3.1"
+version = "1.3.2"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.3.1/talkytrend/config.py` & `talkytrend-1.3.2/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.1/talkytrend/default_settings.toml` & `talkytrend-1.3.2/talkytrend/default_settings.toml`

 * *Files 26% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 enable_news = true
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
-live_tv_url = "https://bloomberg-bloombergtv-1.samsung.wurl.com/manifest/playlist.m3u8"
+live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 
 [testing]
 VALUE = "On Testing"
```

### Comparing `talkytrend-1.3.1/talkytrend/main.py` & `talkytrend-1.3.2/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.1/PKG-INFO` & `talkytrend-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.3.1
+Version: 1.3.2
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

