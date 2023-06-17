# Comparing `tmp/portable_wisdom-0.9.tar.gz` & `tmp/portable_wisdom-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portable_wisdom-0.9.tar", last modified: Sat Jan 14 18:08:06 2023, max compression
+gzip compressed data, was "portable_wisdom-1.0.tar", last modified: Sat Jun 17 19:54:31 2023, max compression
```

## Comparing `portable_wisdom-0.9.tar` & `portable_wisdom-1.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.130766 portable_wisdom-0.9/
--rw-r--r--   0 jacobbudin   (501) staff       (20)      233 2019-04-24 15:19:43.000000 portable_wisdom-0.9/.editorconfig
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.123367 portable_wisdom-0.9/.github/
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.125629 portable_wisdom-0.9/.github/workflows/
--rw-r--r--   0 jacobbudin   (501) staff       (20)      575 2023-01-14 16:59:49.000000 portable_wisdom-0.9/.github/workflows/test.yml
--rw-r--r--   0 jacobbudin   (501) staff       (20)      135 2023-01-13 04:54:31.000000 portable_wisdom-0.9/.gitignore
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1072 2019-04-30 01:53:56.000000 portable_wisdom-0.9/LICENSE
--rw-r--r--   0 jacobbudin   (501) staff       (20)     3912 2023-01-14 18:08:06.130629 portable_wisdom-0.9/PKG-INFO
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2973 2023-01-11 04:40:49.000000 portable_wisdom-0.9/README.md
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.128005 portable_wisdom-0.9/portable_wisdom/
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-04-24 01:31:59.000000 portable_wisdom-0.9/portable_wisdom/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)       20 2023-01-14 18:07:04.000000 portable_wisdom-0.9/portable_wisdom/__version__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      263 2019-04-21 22:33:45.000000 portable_wisdom-0.9/portable_wisdom/article.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      883 2019-05-27 19:10:38.000000 portable_wisdom-0.9/portable_wisdom/cache.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      973 2023-01-04 01:16:31.000000 portable_wisdom-0.9/portable_wisdom/config.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      672 2023-01-08 02:31:39.000000 portable_wisdom-0.9/portable_wisdom/epub.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.128821 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/
--rw-r--r--   0 jacobbudin   (501) staff       (20)     3912 2023-01-14 18:08:06.000000 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1016 2023-01-14 18:08:06.000000 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)        1 2023-01-14 18:08:06.000000 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)       64 2023-01-14 18:08:06.000000 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/entry_points.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)      141 2023-01-14 18:08:06.000000 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/requires.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)       99 2023-01-14 18:08:06.000000 portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/top_level.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2131 2023-01-04 01:20:39.000000 portable_wisdom-0.9/portable_wisdom/source.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.129028 portable_wisdom-0.9/portable_wisdom/sources/
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-05-02 01:19:01.000000 portable_wisdom-0.9/portable_wisdom/sources/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1136 2023-01-13 04:06:30.000000 portable_wisdom-0.9/portable_wisdom/sources/instapaper.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.129343 portable_wisdom-0.9/portable_wisdom/styles/
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1067 2019-05-11 16:01:48.000000 portable_wisdom-0.9/portable_wisdom/styles/nook-glowlight-3.css
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.130382 portable_wisdom-0.9/portable_wisdom/tests/
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-04-28 19:21:20.000000 portable_wisdom-0.9/portable_wisdom/tests/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      491 2019-05-02 01:48:20.000000 portable_wisdom-0.9/portable_wisdom/tests/test_article.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1014 2019-05-02 01:48:52.000000 portable_wisdom-0.9/portable_wisdom/tests/test_cache.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      783 2019-05-02 01:51:39.000000 portable_wisdom-0.9/portable_wisdom/tests/test_source.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-04-28 19:22:00.000000 portable_wisdom-0.9/portable_wisdom/tests/test_wisdom.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-01-14 18:08:06.130470 portable_wisdom-0.9/portable_wisdom/tmp/
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2023-01-13 04:06:18.000000 portable_wisdom-0.9/portable_wisdom/tmp/.keep
--rw-r--r--   0 jacobbudin   (501) staff       (20)     4717 2023-01-04 01:33:37.000000 portable_wisdom-0.9/portable_wisdom/transformers.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2994 2023-01-13 05:08:23.000000 portable_wisdom-0.9/portable_wisdom/wisdom.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)    62768 2019-05-11 16:07:11.000000 portable_wisdom-0.9/preview.jpg
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1682 2023-01-14 17:48:38.000000 portable_wisdom-0.9/pyproject.toml
--rw-r--r--   0 jacobbudin   (501) staff       (20)       38 2023-01-14 18:08:06.130801 portable_wisdom-0.9/setup.cfg
--rw-r--r--   0 jacobbudin   (501) staff       (20)       92 2023-01-14 17:36:59.000000 portable_wisdom-0.9/setup.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      334 2023-01-14 16:59:49.000000 portable_wisdom-0.9/tox.ini
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.143673 portable_wisdom-1.0/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      233 2019-04-24 15:19:43.000000 portable_wisdom-1.0/.editorconfig
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.138388 portable_wisdom-1.0/.github/
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.140555 portable_wisdom-1.0/.github/workflows/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      646 2023-06-10 22:54:31.000000 portable_wisdom-1.0/.github/workflows/lint.yml
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      665 2023-06-10 22:54:31.000000 portable_wisdom-1.0/.github/workflows/test.yml
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      135 2023-01-13 04:54:31.000000 portable_wisdom-1.0/.gitignore
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      368 2023-06-10 23:28:03.000000 portable_wisdom-1.0/Dockerfile
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1072 2019-04-30 01:53:56.000000 portable_wisdom-1.0/LICENSE
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     4661 2023-06-17 19:54:31.143523 portable_wisdom-1.0/PKG-INFO
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     3709 2023-06-17 19:41:09.000000 portable_wisdom-1.0/README.md
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.141738 portable_wisdom-1.0/portable_wisdom/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-04-24 01:31:59.000000 portable_wisdom-1.0/portable_wisdom/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       20 2023-06-17 19:51:45.000000 portable_wisdom-1.0/portable_wisdom/__version__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      263 2019-04-21 22:33:45.000000 portable_wisdom-1.0/portable_wisdom/article.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      883 2019-05-27 19:10:38.000000 portable_wisdom-1.0/portable_wisdom/cache.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      979 2023-06-17 19:38:26.000000 portable_wisdom-1.0/portable_wisdom/config.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      672 2023-01-15 00:55:16.000000 portable_wisdom-1.0/portable_wisdom/epub.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.142431 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     4661 2023-06-17 19:54:31.000000 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1054 2023-06-17 19:54:31.000000 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        1 2023-06-17 19:54:31.000000 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       64 2023-06-17 19:54:31.000000 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/entry_points.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      141 2023-06-17 19:54:31.000000 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/requires.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       99 2023-06-17 19:54:31.000000 portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2131 2023-01-04 01:20:39.000000 portable_wisdom-1.0/portable_wisdom/source.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.142628 portable_wisdom-1.0/portable_wisdom/sources/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-05-02 01:19:01.000000 portable_wisdom-1.0/portable_wisdom/sources/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1394 2023-06-17 19:50:56.000000 portable_wisdom-1.0/portable_wisdom/sources/instapaper.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.142750 portable_wisdom-1.0/portable_wisdom/styles/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1067 2019-05-11 16:01:48.000000 portable_wisdom-1.0/portable_wisdom/styles/nook-glowlight-3.css
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.143262 portable_wisdom-1.0/portable_wisdom/tests/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-04-28 19:21:20.000000 portable_wisdom-1.0/portable_wisdom/tests/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      491 2019-05-02 01:48:20.000000 portable_wisdom-1.0/portable_wisdom/tests/test_article.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1014 2019-05-02 01:48:52.000000 portable_wisdom-1.0/portable_wisdom/tests/test_cache.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      783 2019-05-02 01:51:39.000000 portable_wisdom-1.0/portable_wisdom/tests/test_source.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2019-04-28 19:22:00.000000 portable_wisdom-1.0/portable_wisdom/tests/test_wisdom.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-06-17 19:54:31.143354 portable_wisdom-1.0/portable_wisdom/tmp/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2023-01-13 04:06:18.000000 portable_wisdom-1.0/portable_wisdom/tmp/.keep
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     4717 2023-01-04 01:33:37.000000 portable_wisdom-1.0/portable_wisdom/transformers.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     4150 2023-06-17 19:48:20.000000 portable_wisdom-1.0/portable_wisdom/wisdom.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)    62768 2019-05-11 16:07:11.000000 portable_wisdom-1.0/preview.jpg
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1695 2023-06-17 19:52:21.000000 portable_wisdom-1.0/pyproject.toml
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       38 2023-06-17 19:54:31.143706 portable_wisdom-1.0/setup.cfg
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       92 2023-01-14 17:36:59.000000 portable_wisdom-1.0/setup.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      334 2023-01-14 16:59:49.000000 portable_wisdom-1.0/tox.ini
```

### Comparing `portable_wisdom-0.9/LICENSE` & `portable_wisdom-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/PKG-INFO` & `portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: portable_wisdom
-Version: 0.9
+Name: portable-wisdom
+Version: 1.0
 Summary: Generate EPUB files from unread Instapaper articles
 Author-email: Jacob Budin <self@jacobbudin.com>
 License: MIT
 Project-URL: Source, https://github.com/jacobbudin/portable-wisdom
 Keywords: cli,ebook,reading,epub,instapaper
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -37,28 +37,47 @@
 - Retrieves unread articles from Instapaper
 - Finds and downloads articles' images from the web, downsizes them, converts them to greyscale, and embeds them into the file
 - Caches articles and images, runs fast for frequent users
 - Creates well-formatted EPUB files tailored for your ereader
 
 ## Quick Start
 
-1. Download and install Portable Wisdom from PyPI:
+Before you begin, you'll need to [request an Instapaper API key](https://www.instapaper.com/main/request_oauth_consumer_token) or copy one from a friend.
+
+### Python
+
+1. Download and install Portable Wisdom [from PyPI](https://pypi.org/project/portable-wisdom/):
 
 		$ pip install portable-wisdom
 
-2. [Request an Instapaper API key.](https://www.instapaper.com/main/request_oauth_consumer_token) (Or copy one from a friend.)
-4. Run Portable Wisdom from the command line:
+2. Run Portable Wisdom from the command line:
 
-		$ portable-wisdom --instapaper-key KEY \
-			--instapaper-secret SECRET \
+		$ portable-wisdom \
+			--instapaper-api-key KEY \
+			--instapaper-api-secret SECRET \
 			--instapaper-login USER \
 			--instapaper-password PASS
 
 On success, the script will print the output filename. To view all of the options, run `$ portable-wisdom -h`.
 
+### Docker
+
+Alternatively, using [Docker](https://www.docker.com/get-started/), to download and execute Portable Wisdom [from Docker Hub](https://hub.docker.com/repository/docker/jacobbudin/portable-wisdom/general), run:
+
+	$ docker pull jacobbudin/portable-wisdom:latest
+	$ docker run jacobbudin/portable-wisdom:latest \
+		--instapaper-api-key KEY \
+		--instapaper-api-secret SECRET \
+		--instapaper-login USER \
+		--instapaper-password PASS
+
+## Environment
+
+Alternatively, you can supply the Instapaper credentials via environment variables: `INSTAPAPER_API_KEY`, `INSTAPAPER_API_SECRET`, `INSTAPAPER_LOGIN`, and `INSTAPAPER_PASSWORD`.
+
 ## Transformers
 
 Transformers are functions that modify the EPUB before writing the file to disk. There are many built-in transformers including:
 - `beautify_hr` — converts lines of asterisks to horizontal rules
 - `remove_duplicative_blockquotes` — removes magazine-style "pull quotes"
 - `strip_emojis` — replaces emojis with shortcodes
 - `strip_links` — removes `a` elements
```

### Comparing `portable_wisdom-0.9/README.md` & `portable_wisdom-1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,47 @@
 - Retrieves unread articles from Instapaper
 - Finds and downloads articles' images from the web, downsizes them, converts them to greyscale, and embeds them into the file
 - Caches articles and images, runs fast for frequent users
 - Creates well-formatted EPUB files tailored for your ereader
 
 ## Quick Start
 
-1. Download and install Portable Wisdom from PyPI:
+Before you begin, you'll need to [request an Instapaper API key](https://www.instapaper.com/main/request_oauth_consumer_token) or copy one from a friend.
+
+### Python
+
+1. Download and install Portable Wisdom [from PyPI](https://pypi.org/project/portable-wisdom/):
 
 		$ pip install portable-wisdom
 
-2. [Request an Instapaper API key.](https://www.instapaper.com/main/request_oauth_consumer_token) (Or copy one from a friend.)
-4. Run Portable Wisdom from the command line:
+2. Run Portable Wisdom from the command line:
 
-		$ portable-wisdom --instapaper-key KEY \
-			--instapaper-secret SECRET \
+		$ portable-wisdom \
+			--instapaper-api-key KEY \
+			--instapaper-api-secret SECRET \
 			--instapaper-login USER \
 			--instapaper-password PASS
 
 On success, the script will print the output filename. To view all of the options, run `$ portable-wisdom -h`.
 
+### Docker
+
+Alternatively, using [Docker](https://www.docker.com/get-started/), to download and execute Portable Wisdom [from Docker Hub](https://hub.docker.com/repository/docker/jacobbudin/portable-wisdom/general), run:
+
+	$ docker pull jacobbudin/portable-wisdom:latest
+	$ docker run jacobbudin/portable-wisdom:latest \
+		--instapaper-api-key KEY \
+		--instapaper-api-secret SECRET \
+		--instapaper-login USER \
+		--instapaper-password PASS
+
+## Environment
+
+Alternatively, you can supply the Instapaper credentials via environment variables: `INSTAPAPER_API_KEY`, `INSTAPAPER_API_SECRET`, `INSTAPAPER_LOGIN`, and `INSTAPAPER_PASSWORD`.
+
 ## Transformers
 
 Transformers are functions that modify the EPUB before writing the file to disk. There are many built-in transformers including:
 - `beautify_hr` — converts lines of asterisks to horizontal rules
 - `remove_duplicative_blockquotes` — removes magazine-style "pull quotes"
 - `strip_emojis` — replaces emojis with shortcodes
 - `strip_links` — removes `a` elements
```

### Comparing `portable_wisdom-0.9/portable_wisdom/cache.py` & `portable_wisdom-1.0/portable_wisdom/cache.py`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/config.py` & `portable_wisdom-1.0/portable_wisdom/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     'remove_duplicative_blockquotes',
     'embed_images',
     'strip_emojis',
     'strip_links',
     'beautify_hr'
 )
 
-# Instapaper configuration
-INSTAPAPER_KEY = ''
-INSTAPAPER_SECRET = ''
+# Instapaper credentials
+INSTAPAPER_API_KEY = ''
+INSTAPAPER_API_SECRET = ''
 INSTAPAPER_LOGIN = ''
 INSTAPAPER_PASSWORD = ''
 
 # Maximum number of articles to include
 ARTICLE_LIMIT = 25
 
 # Whether to convert images to greyscale
```

### Comparing `portable_wisdom-0.9/portable_wisdom/epub.py` & `portable_wisdom-1.0/portable_wisdom/epub.py`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/PKG-INFO` & `portable_wisdom-1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: portable-wisdom
-Version: 0.9
+Name: portable_wisdom
+Version: 1.0
 Summary: Generate EPUB files from unread Instapaper articles
 Author-email: Jacob Budin <self@jacobbudin.com>
 License: MIT
 Project-URL: Source, https://github.com/jacobbudin/portable-wisdom
 Keywords: cli,ebook,reading,epub,instapaper
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -37,28 +37,47 @@
 - Retrieves unread articles from Instapaper
 - Finds and downloads articles' images from the web, downsizes them, converts them to greyscale, and embeds them into the file
 - Caches articles and images, runs fast for frequent users
 - Creates well-formatted EPUB files tailored for your ereader
 
 ## Quick Start
 
-1. Download and install Portable Wisdom from PyPI:
+Before you begin, you'll need to [request an Instapaper API key](https://www.instapaper.com/main/request_oauth_consumer_token) or copy one from a friend.
+
+### Python
+
+1. Download and install Portable Wisdom [from PyPI](https://pypi.org/project/portable-wisdom/):
 
 		$ pip install portable-wisdom
 
-2. [Request an Instapaper API key.](https://www.instapaper.com/main/request_oauth_consumer_token) (Or copy one from a friend.)
-4. Run Portable Wisdom from the command line:
+2. Run Portable Wisdom from the command line:
 
-		$ portable-wisdom --instapaper-key KEY \
-			--instapaper-secret SECRET \
+		$ portable-wisdom \
+			--instapaper-api-key KEY \
+			--instapaper-api-secret SECRET \
 			--instapaper-login USER \
 			--instapaper-password PASS
 
 On success, the script will print the output filename. To view all of the options, run `$ portable-wisdom -h`.
 
+### Docker
+
+Alternatively, using [Docker](https://www.docker.com/get-started/), to download and execute Portable Wisdom [from Docker Hub](https://hub.docker.com/repository/docker/jacobbudin/portable-wisdom/general), run:
+
+	$ docker pull jacobbudin/portable-wisdom:latest
+	$ docker run jacobbudin/portable-wisdom:latest \
+		--instapaper-api-key KEY \
+		--instapaper-api-secret SECRET \
+		--instapaper-login USER \
+		--instapaper-password PASS
+
+## Environment
+
+Alternatively, you can supply the Instapaper credentials via environment variables: `INSTAPAPER_API_KEY`, `INSTAPAPER_API_SECRET`, `INSTAPAPER_LOGIN`, and `INSTAPAPER_PASSWORD`.
+
 ## Transformers
 
 Transformers are functions that modify the EPUB before writing the file to disk. There are many built-in transformers including:
 - `beautify_hr` — converts lines of asterisks to horizontal rules
 - `remove_duplicative_blockquotes` — removes magazine-style "pull quotes"
 - `strip_emojis` — replaces emojis with shortcodes
 - `strip_links` — removes `a` elements
```

### Comparing `portable_wisdom-0.9/portable_wisdom/portable_wisdom.egg-info/SOURCES.txt` & `portable_wisdom-1.0/portable_wisdom/portable_wisdom.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .editorconfig
 .gitignore
+Dockerfile
 LICENSE
 README.md
 preview.jpg
 pyproject.toml
 setup.py
 tox.ini
+.github/workflows/lint.yml
 .github/workflows/test.yml
 portable_wisdom/__init__.py
 portable_wisdom/__version__.py
 portable_wisdom/article.py
 portable_wisdom/cache.py
 portable_wisdom/config.py
 portable_wisdom/epub.py
```

### Comparing `portable_wisdom-0.9/portable_wisdom/source.py` & `portable_wisdom-1.0/portable_wisdom/source.py`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/sources/instapaper.py` & `portable_wisdom-1.0/portable_wisdom/sources/instapaper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import logging
 from ..cache import cache
 from ..article import Article
-from ..config import INSTAPAPER_KEY, INSTAPAPER_SECRET, \
-                     INSTAPAPER_LOGIN, INSTAPAPER_PASSWORD, ARTICLE_LIMIT
+from ..config import INSTAPAPER_API_KEY, INSTAPAPER_API_SECRET, \
+    INSTAPAPER_LOGIN, INSTAPAPER_PASSWORD, ARTICLE_LIMIT
 from ..source import Source
 from pyinstapaper.instapaper import Instapaper as PInstapaper
 
 
 class Instapaper(Source):
     name = 'Instapaper'
 
     def get_articles(self):
         """Produce a list of Articles"""
-        instapaper = PInstapaper(INSTAPAPER_KEY, INSTAPAPER_SECRET)
-        instapaper.login(INSTAPAPER_LOGIN, INSTAPAPER_PASSWORD)
+        instapaper = PInstapaper(INSTAPAPER_API_KEY, INSTAPAPER_API_SECRET)
+
+        try:
+            instapaper.login(INSTAPAPER_LOGIN, INSTAPAPER_PASSWORD)
+        except KeyError as e:
+            if 'oauth_token' in str(e):
+                logging.critical(
+                    'Instapaper authentication failed; '
+                    'check your API and user credentials')
+
+            raise e
 
         # Enforce 25 article maximum
         limit = 25
 
         if ARTICLE_LIMIT:
             limit = min(limit, ARTICLE_LIMIT)
```

### Comparing `portable_wisdom-0.9/portable_wisdom/styles/nook-glowlight-3.css` & `portable_wisdom-1.0/portable_wisdom/styles/nook-glowlight-3.css`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/tests/test_cache.py` & `portable_wisdom-1.0/portable_wisdom/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/tests/test_source.py` & `portable_wisdom-1.0/portable_wisdom/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/transformers.py` & `portable_wisdom-1.0/portable_wisdom/transformers.py`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/portable_wisdom/wisdom.py` & `portable_wisdom-1.0/portable_wisdom/wisdom.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,28 +3,40 @@
 # Generate EPUB from Instapaper
 
 import argparse
 import datetime
 from ebooklib import epub
 import logging
 from . import config
+from .__version__ import __version__ as version
 import sys
+import os
 
 
 def main():
     """Generate EPUB from Instapaper"""
     # Support CLI
     parser = argparse.ArgumentParser(
-        description='Generate EPUB from Instapaper')
-    parser.add_argument('--instapaper-key', help='Instapaper API key')
-    parser.add_argument('--instapaper-secret', help='Instapaper API secret')
-    parser.add_argument('--instapaper-login',
-                        help='Instapaper account username or email address')
-    parser.add_argument('--instapaper-password',
-                        help='Instapaper account password')
+        description='Generate EPUB files from unread Instapaper articles')
+    parser.add_argument(
+        '--instapaper-api-key',
+        help='Instapaper API key',
+        default=os.environ.get('INSTAPAPER_API_KEY'))
+    parser.add_argument(
+        '--instapaper-api-secret',
+        help='Instapaper API secret',
+        default=os.environ.get('INSTAPAPER_API_SECRET'))
+    parser.add_argument(
+        '--instapaper-login',
+        help='Instapaper account username or email address',
+        default=os.environ.get('INSTAPAPER_LOGIN'))
+    parser.add_argument(
+        '--instapaper-password',
+        help='Instapaper account password',
+        default=os.environ.get('INSTAPAPER_PASSWORD'))
     parser.add_argument('-o', '--output', default=config.OUTPUT,
                         metavar='FILE', help='output filename')
     parser.add_argument('-s', '--style', default=config.STYLE,
                         metavar='PRESET|FILE', help='stylesheet to use')
     parser.add_argument('-t', '--transform', default=config.TRANSFORM,
                         nargs='+', metavar='FUNCTION',
                         help='transformer functions')
@@ -34,17 +46,44 @@
     parser.add_argument('-q', '--quiet', default=False,
                         action='store_true',
                         help='do not print standard output')
     parser.add_argument('-v', '--verbose', default=False,
                         action='store_true', help='verbose mode')
     parser.add_argument('-d', '--debug', default=False,
                         action='store_true', help='debug mode')
+    parser.add_argument('-V', '--version', default=False,
+                        action='store_true', help='print version number')
 
     args = parser.parse_args()
 
+    if args.version:
+        print(version)
+        sys.exit(0)
+
+    # Check for mandatory arguments
+    mandatory_arguments = (
+        'instapaper_api_key',
+        'instapaper_api_secret',
+        'instapaper_login',
+        'instapaper_password')
+    absent_arguments = []
+    for arg in mandatory_arguments:
+        try:
+            value = getattr(args, arg)
+            if value is None or len(value) == 0:
+                raise AttributeError
+        except AttributeError:
+            absent_arguments.append(arg)
+
+    if len(absent_arguments):
+        logging.critical(
+            'Instapaper credentials not provided: %s' %
+            ', '.join(absent_arguments))
+        sys.exit(1)
+
     # Where an option is provided, override its configuration value
     for option, value in vars(args).items():
         if value:
             setattr(config, option.upper(), value)
 
     logging_level = logging.CRITICAL
     if config.VERBOSE or config.DEBUG:
```

### Comparing `portable_wisdom-0.9/preview.jpg` & `portable_wisdom-1.0/preview.jpg`

 * *Files identical despite different names*

### Comparing `portable_wisdom-0.9/pyproject.toml` & `portable_wisdom-1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "Generate EPUB files from unread Instapaper articles"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["cli", "ebook", "reading", "epub", "instapaper"]
 license = {text = "MIT"}
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

