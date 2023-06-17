# Comparing `tmp/ofscraper-2.4.3.tar.gz` & `tmp/ofscraper-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.4.3.tar", max compression
+gzip compressed data, was "ofscraper-2.4.4.tar", max compression
```

## Comparing `ofscraper-2.4.3.tar` & `ofscraper-2.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1067 2023-06-16 18:24:54.342140 ofscraper-2.4.3/LICENSE
--rw-r--r--   0        0        0     5201 2023-06-16 18:24:54.342140 ofscraper-2.4.3/README.md
--rw-r--r--   0        0        0      607 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     7066 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/archive.py
--rw-r--r--   0        0        0     3944 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/init.py
--rw-r--r--   0        0        0     2343 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/me.py
--rw-r--r--   0        0        0     6592 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/messages.py
--rw-r--r--   0        0        0     8529 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/paid.py
--rw-r--r--   0        0        0     4576 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11162 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3593 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3047 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     7712 2023-06-16 18:24:54.346140 ofscraper-2.4.3/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    31071 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/commands/check.py
--rwxr-xr-x   0        0        0    14029 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     5769 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     1364 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompt model.md
--rw-r--r--   0        0        0      696 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     6754 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27230 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      679 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     9292 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9035 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     6158 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10680 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    19690 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3155 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     5622 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9870 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7654 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3073 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     6042 2023-06-16 18:24:54.350140 ofscraper-2.4.3/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1520 2023-06-16 18:25:27.978646 ofscraper-2.4.3/pyproject.toml
--rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 ofscraper-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-16 23:04:00.166897 ofscraper-2.4.4/LICENSE
+-rw-r--r--   0        0        0     5450 2023-06-16 23:04:00.166897 ofscraper-2.4.4/README.md
+-rw-r--r--   0        0        0      607 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     7066 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     3944 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2343 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/me.py
+-rw-r--r--   0        0        0     6592 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     8529 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     4576 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11162 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3593 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3047 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     7712 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    31071 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/commands/check.py
+-rwxr-xr-x   0        0        0    14029 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     5769 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     1364 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/prompt model.md
+-rw-r--r--   0        0        0      696 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     6754 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27230 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      679 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     9292 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9035 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     6158 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10680 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    19690 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3155 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     5622 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9870 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7654 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3073 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     6042 2023-06-16 23:04:00.174895 ofscraper-2.4.4/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1520 2023-06-16 23:04:32.082997 ofscraper-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 ofscraper-2.4.4/PKG-INFO
```

### Comparing `ofscraper-2.4.3/LICENSE` & `ofscraper-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/README.md` & `ofscraper-2.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,53 +21,72 @@
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
 
 
-## Installation
+# Installation
 
 ### Recommended python3.9 or python3.10
 
 
-# Windows: 
-## stable
+## Windows: 
+### stable
 ```
 pip install ofscraper
 ```
 or 
-## development
+### development
 ```
 pip install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 or 
-## specific version
+### specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
 
 
-#  macOS/Linux
+##  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
 pip3 install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 
 or 
-## specific version
+### specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
 
+## Upgrade
+Not uninstalling has caused user issues in the past
+```
+pip3 uninstall ofscraper
+```
+
+Then run one of the install commands above
+
+```
+pip3 install ofscraper --upgrade
+```
+or 
+
+```
+pip3 install ofscraper==latest version number
+```
+
+
+
 ## Authentication
 
 You'll need to retrive your auth information 
     
 https://github.com/datawhores/OF-Scraper/wiki/Auth
```

### Comparing `ofscraper-2.4.3/ofscraper/__init__.py` & `ofscraper-2.4.4/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/__version__.py` & `ofscraper-2.4.4/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/archive.py` & `ofscraper-2.4.4/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/highlights.py` & `ofscraper-2.4.4/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/init.py` & `ofscraper-2.4.4/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/me.py` & `ofscraper-2.4.4/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/messages.py` & `ofscraper-2.4.4/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/paid.py` & `ofscraper-2.4.4/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/pinned.py` & `ofscraper-2.4.4/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/posts.py` & `ofscraper-2.4.4/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/profile.py` & `ofscraper-2.4.4/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/subscriptions.py` & `ofscraper-2.4.4/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/api/timeline.py` & `ofscraper-2.4.4/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/commands/check.py` & `ofscraper-2.4.4/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/commands/scraper.py` & `ofscraper-2.4.4/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/constants.py` & `ofscraper-2.4.4/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/db/operations.py` & `ofscraper-2.4.4/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/db/queries.py` & `ofscraper-2.4.4/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/interaction/like.py` & `ofscraper-2.4.4/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/prompt model.md` & `ofscraper-2.4.4/ofscraper/prompt model.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.4.4/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.4.4/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/prompts/prompts.py` & `ofscraper-2.4.4/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/start.py` & `ofscraper-2.4.4/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/args.py` & `ofscraper-2.4.4/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/auth.py` & `ofscraper-2.4.4/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/binaries.py` & `ofscraper-2.4.4/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/config.py` & `ofscraper-2.4.4/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/dates.py` & `ofscraper-2.4.4/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/download.py` & `ofscraper-2.4.4/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/encoding.py` & `ofscraper-2.4.4/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/exit.py` & `ofscraper-2.4.4/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/filters.py` & `ofscraper-2.4.4/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/logger.py` & `ofscraper-2.4.4/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/of.py` & `ofscraper-2.4.4/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/paths.py` & `ofscraper-2.4.4/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/profiles.py` & `ofscraper-2.4.4/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/separate.py` & `ofscraper-2.4.4/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/stdout.py` & `ofscraper-2.4.4/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/ofscraper/utils/userselector.py` & `ofscraper-2.4.4/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4.3/pyproject.toml` & `ofscraper-2.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.4.3"
+version = "2.4.4"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.4.3/PKG-INFO` & `ofscraper-2.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.4.3
+Version: 2.4.4
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -56,53 +56,72 @@
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
 
 
-## Installation
+# Installation
 
 ### Recommended python3.9 or python3.10
 
 
-# Windows: 
-## stable
+## Windows: 
+### stable
 ```
 pip install ofscraper
 ```
 or 
-## development
+### development
 ```
 pip install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 or 
-## specific version
+### specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
 
 
-#  macOS/Linux
+##  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
 pip3 install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 
 or 
-## specific version
+### specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
 
+## Upgrade
+Not uninstalling has caused user issues in the past
+```
+pip3 uninstall ofscraper
+```
+
+Then run one of the install commands above
+
+```
+pip3 install ofscraper --upgrade
+```
+or 
+
+```
+pip3 install ofscraper==latest version number
+```
+
+
+
 ## Authentication
 
 You'll need to retrive your auth information 
     
 https://github.com/datawhores/OF-Scraper/wiki/Auth
```

