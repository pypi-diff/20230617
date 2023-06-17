# Comparing `tmp/is_bot-0.2.2.tar.gz` & `tmp/is_bot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "is_bot-0.2.2.tar", last modified: Mon Mar 13 13:13:18 2023, max compression
+gzip compressed data, was "dist/is_bot-0.2.3.tar", last modified: Sat Jun 17 06:28:49 2023, max compression
```

## Comparing `is_bot-0.2.2.tar` & `is_bot-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 13:13:18.745293 is_bot-0.2.2/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2021-02-13 05:38:25.000000 is_bot-0.2.2/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2021-02-11 14:12:33.000000 is_bot-0.2.2/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     2354 2023-03-13 13:13:18.745293 is_bot-0.2.2/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     1971 2022-08-25 05:44:59.000000 is_bot-0.2.2/README.md
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 13:13:18.745293 is_bot-0.2.2/is_bot/
--rw-rw-r--   0 roman     (1000) roman     (1000)       70 2023-03-13 13:08:23.000000 is_bot-0.2.2/is_bot/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1388 2022-08-23 11:42:31.000000 is_bot-0.2.2/is_bot/_is_bot.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     4536 2023-03-13 12:51:05.000000 is_bot-0.2.2/is_bot/_patterns.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 13:13:18.745293 is_bot-0.2.2/is_bot.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     2354 2023-03-13 13:13:18.000000 is_bot-0.2.2/is_bot.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      284 2023-03-13 13:13:18.000000 is_bot-0.2.2/is_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-03-13 13:13:18.000000 is_bot-0.2.2/is_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       17 2023-03-13 13:13:18.000000 is_bot-0.2.2/is_bot.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        7 2023-03-13 13:13:18.000000 is_bot-0.2.2/is_bot.egg-info/top_level.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      135 2022-08-23 09:57:29.000000 is_bot-0.2.2/pyproject.toml
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-03-13 13:13:18.745293 is_bot-0.2.2/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1109 2022-08-23 08:33:05.000000 is_bot-0.2.2/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 13:13:18.745293 is_bot-0.2.2/tests/
--rw-rw-r--   0 roman     (1000) roman     (1000)     2543 2023-03-13 12:12:36.000000 is_bot-0.2.2/tests/test_is_bot.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-17 06:28:49.000000 is_bot-0.2.3/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2021-02-13 05:38:25.000000 is_bot-0.2.3/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2021-02-11 14:12:33.000000 is_bot-0.2.3/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2374 2023-06-17 06:28:49.000000 is_bot-0.2.3/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1971 2022-08-25 05:44:59.000000 is_bot-0.2.3/README.md
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       70 2023-06-17 05:52:29.000000 is_bot-0.2.3/is_bot/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1388 2022-08-23 11:42:31.000000 is_bot-0.2.3/is_bot/_is_bot.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3676 2023-06-17 05:50:09.000000 is_bot-0.2.3/is_bot/_patterns.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2374 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      263 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       17 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        7 2023-06-17 06:28:49.000000 is_bot-0.2.3/is_bot.egg-info/top_level.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      135 2023-06-17 06:14:33.000000 is_bot-0.2.3/pyproject.toml
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-06-17 06:28:49.000000 is_bot-0.2.3/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1109 2022-08-23 08:33:05.000000 is_bot-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `is_bot-0.2.2/LICENSE.txt` & `is_bot-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `is_bot-0.2.2/PKG-INFO` & `is_bot-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: is_bot
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package to detect bots/crawlers/spiders via user-agent
 Home-page: https://github.com/romis2012/is-bot
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: python bots crawlers web-crawlers user-agent user-agent-parser
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## is-bot
 
 [![CI](https://github.com/romis2012/is-bot/actions/workflows/ci.yml/badge.svg)](https://github.com/romis2012/is-bot/actions/workflows/ci.yml)
 [![Coverage Status](https://codecov.io/gh/romis2012/is-bot/branch/master/graph/badge.svg)](https://codecov.io/gh/romis2012/is-bot)
@@ -79,7 +80,9 @@
 #> Search
 
 # list all patterns that match the user agent string
 print(bots.matches(ua))
 #> ['(?<! (ya|yandex))search', '(?<! cu)bot']
 ```
 
+
+
```

### Comparing `is_bot-0.2.2/README.md` & `is_bot-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `is_bot-0.2.2/is_bot/_is_bot.py` & `is_bot-0.2.3/is_bot/_is_bot.py`

 * *Files identical despite different names*

### Comparing `is_bot-0.2.2/is_bot/_patterns.py` & `is_bot-0.2.3/is_bot/_patterns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,88 @@
+# https://github.com/omrilotan/isbot/tree/v3.6.3
 default_patterns = {
     " daum[ /]",
-    " DCV$",
     " deusu/",
     "(?:^| )site",
     "@[a-z]",
     "\\(at\\)[a-z]",
     "\\(github\\.com/",
     "\\[at\\][a-z]",
     "^12345",
     "^<",
-    "^[\\w \\.]+/v?\\d+(\\.\\d+)?(\\.\\d{1,10})?$",
-    "^[\\w\\-\\(\\)]+$",
+    "^[\\w \\.\\-\\(\\)]+(/v?\\d+(\\.\\d+)?(\\.\\d{1,10})?)?$",
     "^[^ ]{50,}$",
-    "^ace explorer",
-    "^acoon",
     "^active",
     "^ad muncher",
     "^anglesharp/",
     "^anonymous",
-    "^apple-pubsub/",
-    "^astute srm",
     "^avsdevicesdk/",
     "^axios/",
     "^bidtellect/",
     "^biglotron",
-    "^blackboard safeassign",
-    "^blocknote.net",
-    "^braze sender",
-    "^captivenetworksupport",
+    "^btwebclient/",
     "^castro",
-    "^cf-uc ",
     "^clamav[ /]",
+    "^client/",
     "^cobweb/",
     "^coccoc",
     "^custom",
-    "^dap ",
     "^ddg[_-]android",
     "^discourse",
     "^dispatch/\\d",
     "^downcast/",
     "^duckduckgo",
-    "^email",
-    "^enigma browser",
-    "^evernote clip resolver",
     "^facebook",
-    "^faraday",
     "^fdm[ /]\\d",
     "^getright/",
     "^gozilla/",
     "^hatena",
     "^hobbit",
     "^hotzonu",
     "^hwcdn/",
-    "^invision",
     "^jeode/",
-    "^jetbrains",
     "^jetty/",
     "^jigsaw",
     "^linkdex",
     "^lwp[-: ]",
-    "^mailchimp\\.com$",
     "^metauri",
     "^microsoft bits",
-    "^microsoft data",
-    "^microsoft office existence",
-    "^microsoft office protocol discovery",
-    "^microsoft windows network diagnostics",
-    "^microsoft-cryptoapi",
-    "^microsoft-webdav-miniredir",
     "^movabletype",
     "^mozilla/\\d\\.\\d \\(compatible;?\\)$",
     "^mozilla/\\d\\.\\d \\w*$",
-    "^my browser$",
     "^navermailapp",
     "^netsurf",
-    "^nginx\\W",
-    "^node-superagent",
-    "^octopus",
     "^offline explorer",
-    "^pagething",
-    "^panscient",
-    "^perimeterx",
     "^php",
     "^postman",
     "^postrank",
     "^python",
     "^read",
     "^reed",
     "^restsharp/",
-    "^shareaza",
-    "^shockwave flash",
     "^snapchat",
     "^space bison",
-    "^sprinklr",
     "^svn",
     "^swcd ",
-    "^t-online browser",
     "^taringa",
     "^test certificate info",
-    "^the knowledge ai",
-    "^thinklab",
     "^thumbor/",
-    "^traackr.com",
     "^tumblr/",
-    "^uptime",
-    "^vbulletin",
+    "^user-agent:mozilla",
+    "^valid",
     "^venus/fedoraplanet",
     "^w3c",
     "^webbandit/",
     "^webcopier",
     "^wget",
     "^whatsapp",
-    "^www-mechanize",
     "^xenu link sleuth",
     "^yahoo",
     "^yandex",
     "^zdm/\\d",
-    "^zeushdthree",
     "^zoom marketplace/",
     "^{{.*}}$",
     "adbeat\\.com",
     "appinsights",
     "archive",
     "ask jeeves/teoma",
     "bit\\.ly/",
@@ -129,18 +91,17 @@
     "browsex",
     "burpcollaborator",
     "capture",
     "catch",
     "check",
     "chrome-lighthouse",
     "chromeframe",
-    "client",
     "cloud",
     "crawl",
-    "daemon",
+    "cryptoapi",
     "dareboost",
     "datanyze",
     "dataprovider",
     "dejaclick",
     "dmbrowser",
     "download",
     "evc-batch/",
@@ -168,49 +129,46 @@
     "neustar wpm",
     "news",
     "nutch",
     "offbyone",
     "optimize",
     "pageburst",
     "pagespeed",
-    "parse",
     "perl",
     "phantom",
     "pingdom",
     "powermarks",
     "preview",
-    "probe",
     "proxy",
     "ptst[ /]\\d",
     "reader",
     "rexx;",
     "rigor",
     "rss",
     "scan",
     "scrape",
     "search",
     "serp ?reputation ?management",
     "server",
     "sogou",
     "sparkler/",
+    "speedcurve",
     "spider",
     "statuscake",
     "stumbleupon\\.com",
     "supercleaner",
     "synapse",
     "synthetic",
     "taginspector/",
-    "toolbar",
     "torrent",
     "tracemyfile",
     "transcoder",
     "trendsmapresolver",
     "twingly recon",
     "url",
-    "valid",
     "virtuoso",
     "wappalyzer",
     "webglance",
     "webkit2png",
     "websitemetadataretriever",
     "whatcms/",
     "wordpress",
```

### Comparing `is_bot-0.2.2/is_bot.egg-info/PKG-INFO` & `is_bot-0.2.3/is_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: is-bot
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package to detect bots/crawlers/spiders via user-agent
 Home-page: https://github.com/romis2012/is-bot
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: python bots crawlers web-crawlers user-agent user-agent-parser
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## is-bot
 
 [![CI](https://github.com/romis2012/is-bot/actions/workflows/ci.yml/badge.svg)](https://github.com/romis2012/is-bot/actions/workflows/ci.yml)
 [![Coverage Status](https://codecov.io/gh/romis2012/is-bot/branch/master/graph/badge.svg)](https://codecov.io/gh/romis2012/is-bot)
@@ -79,7 +80,9 @@
 #> Search
 
 # list all patterns that match the user agent string
 print(bots.matches(ua))
 #> ['(?<! (ya|yandex))search', '(?<! cu)bot']
 ```
 
+
+
```

### Comparing `is_bot-0.2.2/setup.py` & `is_bot-0.2.3/setup.py`

 * *Files identical despite different names*

