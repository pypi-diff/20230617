# Comparing `tmp/sankaku-1.0.2.tar.gz` & `tmp/sankaku-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sankaku-1.0.2.tar", last modified: Wed May 31 04:28:53 2023, max compression
+gzip compressed data, was "sankaku-1.0.3.tar", last modified: Sat Jun 17 19:01:45 2023, max compression
```

## Comparing `sankaku-1.0.2.tar` & `sankaku-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.115640 sankaku-1.0.2/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.2/LICENSE
--rw-r--r--   0 moldus    (1000) moldus    (1000)       90 2023-05-31 03:19:49.000000 sankaku-1.0.2/MANIFEST.in
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3250 2023-05-31 04:28:53.115640 sankaku-1.0.2/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2447 2023-05-31 03:56:32.000000 sankaku-1.0.2/README.md
--rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.2/pyproject.toml
--rw-r--r--   0 moldus    (1000) moldus    (1000)       13 2023-05-31 03:19:49.000000 sankaku-1.0.2/requirements-socks.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)      126 2023-05-31 03:19:49.000000 sankaku-1.0.2/requirements-test.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       79 2023-05-31 03:19:49.000000 sankaku-1.0.2/requirements.txt
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.112640 sankaku-1.0.2/sankaku/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-29 15:50:51.000000 sankaku-1.0.2/sankaku/__init__.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.113641 sankaku-1.0.2/sankaku/clients/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.2/sankaku/clients/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1228 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/clients/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    15472 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/clients/clients.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3258 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/clients/http_client.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1325 2023-05-31 03:19:49.000000 sankaku-1.0.2/sankaku/constants.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/errors.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.114641 sankaku-1.0.2/sankaku/models/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.2/sankaku/models/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1906 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/books.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/http.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      268 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/pages.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3464 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/posts.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     4250 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/tags.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2137 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/users.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.115640 sankaku-1.0.2/sankaku/paginators/
--rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.2/sankaku/paginators/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      829 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/paginators/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    10560 2023-05-31 04:05:29.000000 sankaku-1.0.2/sankaku/paginators/paginators.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      380 2023-05-31 04:05:29.000000 sankaku-1.0.2/sankaku/typedefs.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/types.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2049 2023-05-31 04:17:38.000000 sankaku-1.0.2/sankaku/utils.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.113641 sankaku-1.0.2/sankaku.egg-info/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3250 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)      750 2023-05-31 04:28:53.000000 sankaku-1.0.2/sankaku.egg-info/SOURCES.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/dependency_links.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)      241 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/requires.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/top_level.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-05-31 04:28:53.115640 sankaku-1.0.2/setup.cfg
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1631 2023-05-31 04:26:03.000000 sankaku-1.0.2/setup.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.919839 sankaku-1.0.3/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.3/LICENSE
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       90 2023-06-17 14:43:33.000000 sankaku-1.0.3/MANIFEST.in
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3248 2023-06-17 19:01:45.919839 sankaku-1.0.3/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2445 2023-06-17 18:44:48.000000 sankaku-1.0.3/README.md
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.3/pyproject.toml
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       13 2023-05-31 03:19:49.000000 sankaku-1.0.3/requirements-socks.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      126 2023-06-17 14:43:33.000000 sankaku-1.0.3/requirements-test.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       80 2023-06-01 19:36:49.000000 sankaku-1.0.3/requirements.txt
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.916839 sankaku-1.0.3/sankaku/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-29 15:50:51.000000 sankaku-1.0.3/sankaku/__init__.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.917839 sankaku-1.0.3/sankaku/clients/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.3/sankaku/clients/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1228 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/clients/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    15472 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/clients/clients.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3258 2023-06-01 20:18:47.000000 sankaku-1.0.3/sankaku/clients/http_client.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1325 2023-05-31 03:19:49.000000 sankaku-1.0.3/sankaku/constants.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/errors.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.918839 sankaku-1.0.3/sankaku/models/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.3/sankaku/models/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      202 2023-06-17 18:03:24.000000 sankaku-1.0.3/sankaku/models/base.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1935 2023-06-17 17:20:37.000000 sankaku-1.0.3/sankaku/models/books.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/models/http.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      268 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/models/pages.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3657 2023-06-17 17:35:06.000000 sankaku-1.0.3/sankaku/models/posts.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     4418 2023-06-17 17:43:40.000000 sankaku-1.0.3/sankaku/models/tags.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2469 2023-06-17 17:14:26.000000 sankaku-1.0.3/sankaku/models/users.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.919839 sankaku-1.0.3/sankaku/paginators/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.3/sankaku/paginators/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      829 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/paginators/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    10560 2023-05-31 04:05:29.000000 sankaku-1.0.3/sankaku/paginators/paginators.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      380 2023-05-31 04:05:29.000000 sankaku-1.0.3/sankaku/typedefs.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/types.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2049 2023-06-17 15:58:03.000000 sankaku-1.0.3/sankaku/utils.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.917839 sankaku-1.0.3/sankaku.egg-info/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3248 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      773 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/SOURCES.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/dependency_links.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      242 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/requires.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/top_level.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-06-17 19:01:45.919839 sankaku-1.0.3/setup.cfg
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1631 2023-06-17 19:00:05.000000 sankaku-1.0.3/setup.py
```

### Comparing `sankaku-1.0.2/LICENSE` & `sankaku-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/PKG-INFO` & `sankaku-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sankaku
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asynchronous API wrapper for Sankaku Complex.
 Home-page: https://github.com/zerex290/sankaku
 Author: zerex290
 Author-email: zerex290@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/zerex290/sankaku/issues
 Keywords: sankaku,sankakucomplex,api
@@ -56,15 +56,15 @@
 ## Requirements
 
 - Python 3.7+
 - aiohttp
 - pydantic
 - loguru
 - aiohttp-retry
-- typing_extensions; python_version < '3.9'
+- typing_extensions; python_version < '3.10'
 
 ## Installation
 
 To install sankaku via pip write following line of code in your terminal:
 
 ```commandline
 pip install sankaku
@@ -82,15 +82,15 @@
 
 Open a command prompt. Navigate to the directory where you want
 to install Sankaku. Type the following command:
 
 ```commandline
 git clone https://github.com/zerex290/sankaku.git
 cd sankaku
-docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3 bash
 ```
 
 ## Usage example
 
 It's very simple to use and doesn't require to always keep opened browser page
 with documentation because all methods are self-explanatory:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sankaku Version: 1.0.2 Summary: Asynchronous API
+Metadata-Version: 2.1 Name: sankaku Version: 1.0.3 Summary: Asynchronous API
 wrapper for Sankaku Complex. Home-page: https://github.com/zerex290/sankaku
 Author: zerex290 Author-email: zerex290@gmail.com License: MIT Project-URL:
 Issue Tracker, https://github.com/zerex290/sankaku/issues Keywords:
 sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -17,25 +17,25 @@
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
 API request parameters to provide better user experience > For instance, you
 can type `types.TagType.ARTIST` instead of `types[]=1` --- Documentation:
 https://zerex290.github.io/sankaku API Reference: https://zerex290.github.io/
 sankaku/api Source code: https://github.com/zerex290/sankaku --- ##
 Requirements - Python 3.7+ - aiohttp - pydantic - loguru - aiohttp-retry -
-typing_extensions; python_version < '3.9' ## Installation To install sankaku
+typing_extensions; python_version < '3.10' ## Installation To install sankaku
 via pip write following line of code in your terminal: ```commandline pip
 install sankaku ``` To install the sankaku via Docker, you can follow these
 steps: ###### Step 1: Install Docker Ensure that Docker is installed on your
 machine. If Docker is not already installed, you can download and install it
 from the official [Docker website](https://www.docker.com/get-started). ######
 Step 2: Use docker to install sankaku Open a command prompt. Navigate to the
 directory where you want to install Sankaku. Type the following command:
 ```commandline git clone https://github.com/zerex290/sankaku.git cd sankaku
-docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash ``` ##
-Usage example It's very simple to use and doesn't require to always keep opened
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3 bash ``` ## Usage
+example It's very simple to use and doesn't require to always keep opened
 browser page with documentation because all methods are self-explanatory: ```py
 import asyncio from sankaku import SankakuClient async def main(): client =
 SankakuClient() post = await client.get_post(25742064) print(f"Rating:
 {post.rating} | Created: {post.created_at}") # "Rating: Rating.QUESTIONABLE |
 Created: 2021-08-01 23:18:52+03:00" await client.login(access_token="token") #
 Or you can authorize by credentials: # await client.login(login="nickname or
 email", password="password") async for book in client.get_recently_read_books
```

### Comparing `sankaku-1.0.2/README.md` & `sankaku-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## Requirements
 
 - Python 3.7+
 - aiohttp
 - pydantic
 - loguru
 - aiohttp-retry
-- typing_extensions; python_version < '3.9'
+- typing_extensions; python_version < '3.10'
 
 ## Installation
 
 To install sankaku via pip write following line of code in your terminal:
 
 ```commandline
 pip install sankaku
@@ -59,15 +59,15 @@
 
 Open a command prompt. Navigate to the directory where you want
 to install Sankaku. Type the following command:
 
 ```commandline
 git clone https://github.com/zerex290/sankaku.git
 cd sankaku
-docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3 bash
 ```
 
 ## Usage example
 
 It's very simple to use and doesn't require to always keep opened browser page
 with documentation because all methods are self-explanatory:
```

#### html2text {}

```diff
@@ -6,25 +6,25 @@
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
 API request parameters to provide better user experience > For instance, you
 can type `types.TagType.ARTIST` instead of `types[]=1` --- Documentation:
 https://zerex290.github.io/sankaku API Reference: https://zerex290.github.io/
 sankaku/api Source code: https://github.com/zerex290/sankaku --- ##
 Requirements - Python 3.7+ - aiohttp - pydantic - loguru - aiohttp-retry -
-typing_extensions; python_version < '3.9' ## Installation To install sankaku
+typing_extensions; python_version < '3.10' ## Installation To install sankaku
 via pip write following line of code in your terminal: ```commandline pip
 install sankaku ``` To install the sankaku via Docker, you can follow these
 steps: ###### Step 1: Install Docker Ensure that Docker is installed on your
 machine. If Docker is not already installed, you can download and install it
 from the official [Docker website](https://www.docker.com/get-started). ######
 Step 2: Use docker to install sankaku Open a command prompt. Navigate to the
 directory where you want to install Sankaku. Type the following command:
 ```commandline git clone https://github.com/zerex290/sankaku.git cd sankaku
-docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash ``` ##
-Usage example It's very simple to use and doesn't require to always keep opened
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3 bash ``` ## Usage
+example It's very simple to use and doesn't require to always keep opened
 browser page with documentation because all methods are self-explanatory: ```py
 import asyncio from sankaku import SankakuClient async def main(): client =
 SankakuClient() post = await client.get_post(25742064) print(f"Rating:
 {post.rating} | Created: {post.created_at}") # "Rating: Rating.QUESTIONABLE |
 Created: 2021-08-01 23:18:52+03:00" await client.login(access_token="token") #
 Or you can authorize by credentials: # await client.login(login="nickname or
 email", password="password") async for book in client.get_recently_read_books
```

### Comparing `sankaku-1.0.2/sankaku/clients/abc.py` & `sankaku-1.0.3/sankaku/clients/abc.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/clients/clients.py` & `sankaku-1.0.3/sankaku/clients/clients.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/clients/http_client.py` & `sankaku-1.0.3/sankaku/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/constants.py` & `sankaku-1.0.3/sankaku/constants.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/errors.py` & `sankaku-1.0.3/sankaku/errors.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/models/books.py` & `sankaku-1.0.3/sankaku/models/books.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Optional, List
 
-from pydantic import BaseModel
-
 from sankaku import types
+from .base import SankakuResponseModel
 from .posts import Post
 from .tags import PostTag
 from .users import Author
 
 
 __all__ = ["PageBook", "Book"]
 
 
-class BookState(BaseModel):
+class BookState(SankakuResponseModel):
     current_page: int
     sequence: int
     post_id: int
     series_id: Optional[int]
     created_at: datetime
     updated_at: datetime
     percent: int
 
 
-class PageBook(BaseModel):
+class PageBook(SankakuResponseModel):
     """Model that describes books on book pages."""
     id: int
     name_en: Optional[str]
     name_ja: Optional[str]
     description: str
     description_en: Optional[str]
     description_ja: Optional[str]
```

### Comparing `sankaku-1.0.2/sankaku/models/posts.py` & `sankaku-1.0.3/sankaku/models/posts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Optional, List
 
-from pydantic import BaseModel, Field, validator
+from pydantic import Field, validator
 
 from sankaku import types
 from sankaku.utils import convert_ts_to_datetime
+from .base import SankakuResponseModel
 from .tags import PostTag
 from .users import Author
 
 
 __all__ = ["Comment", "Post", "AIPost"]
 
 
-class GenerationDirectives(BaseModel):
+class GenerationDirectives(SankakuResponseModel):
     """Model that describes additional fields for AI-generated posts."""
     width: int
     height: int
     prompt: str
     batch_size: int
     batch_count: int
     sampling_steps: int
     negative_prompt: str
 
+    # The following fields can be missing in server JSON response
+    version: Optional[str] = None  # https://imgur.com/a/aMJ7fR2
 
-class BasePost(BaseModel):
+
+class BasePost(SankakuResponseModel):
     """Model that contains minimum amount of information that all posts have."""
     id: int
     created_at: datetime
     rating: types.Rating
     status: str
     author: Author
     file_url: Optional[str]
@@ -61,15 +65,15 @@
     )
 
     @validator("extension", pre=True)
     def get_extension(cls, v) -> Optional[str]:  # noqa
         return v.split("/")[-1] if v else None
 
 
-class Comment(BaseModel):
+class Comment(SankakuResponseModel):
     """Model that describes comments related to posts if they are exist."""
     id: int
     created_at: datetime
     post_id: int
     author: Author
     body: str
     score: int
```

### Comparing `sankaku-1.0.2/sankaku/models/tags.py` & `sankaku-1.0.3/sankaku/models/tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from datetime import datetime
 from typing import Optional, List
 
-from pydantic import BaseModel, Field, validator
+from pydantic import Field, validator
 
 from sankaku import types
 from sankaku.utils import convert_ts_to_datetime
+from .base import SankakuResponseModel
 from .users import Author
 
 
 __all__ = ["PostTag", "PageTag", "Wiki", "WikiTag"]
 
 
-class BaseTag(BaseModel):
+class BaseTag(SankakuResponseModel):
     """Model that contains minimum amount of information that all tags have."""
     id: int
     name: str
     name_en: str
     name_ja: Optional[str]
     type: types.TagType
     post_count: int
     pool_count: int
     series_count: int
     rating: Optional[types.Rating]
 
 
-class TagMixin(BaseModel):
+class TagMixin(SankakuResponseModel):
     """Additional data that certain tags have."""
     count: int
     tag_name: str = Field(alias="tagName")
     total_post_count: int
     total_pool_count: int
 
 
@@ -75,15 +76,15 @@
         tag_ids = v.split(",") if "," in v else v.split()
         try:
             return [int(tag_id) for tag_id in tag_ids]
         except ValueError:
             return None
 
 
-class BaseTranslations(BaseModel):
+class BaseTranslations(SankakuResponseModel):
     """Model that contain minimum information about tag translations."""
     lang: str
     translation: str
 
 
 class PageTagTranslations(BaseTranslations):
     """Model that describes page tag translations."""
@@ -91,24 +92,27 @@
 
 
 class WikiTagTranslations(BaseTranslations):
     """Model that describes wiki tag translations."""
     status: int
     opacity: float
 
+    # The following fields can be missing in server JSON response
+    id: Optional[int] = None
+
 
 class PageTag(PostTag):
     """Model that describes tags on tag page."""
     translations: List[PageTagTranslations]
     related_tags: List[NestedTag]
     child_tags: List[NestedTag]
     parent_tags: List[NestedTag]
 
 
-class Wiki(BaseModel):
+class Wiki(SankakuResponseModel):
     """Model that describes wiki information for specific tag."""
     id: int
     title: str
     body: str
     created_at: datetime
     updated_at: Optional[datetime]
     author: Author = Field(alias="user")
```

### Comparing `sankaku-1.0.2/sankaku/models/users.py` & `sankaku-1.0.3/sankaku/models/users.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
 from typing import Optional, List
 
-from pydantic import BaseModel, Field, validator
+from pydantic import Field, validator
 
 from sankaku import types
+from .base import SankakuResponseModel
 
 
 __all__ = ["Author", "User", "ExtendedUser"]
 
 
-class BaseUser(BaseModel):
+class BaseUser(SankakuResponseModel):
     """User profile with a minimum amount of information."""
     id: int
     name: str
     avatar: str
     avatar_rating: types.Rating
 
 
@@ -37,37 +38,41 @@
     note_update_count: int
     wiki_update_count: int
     forum_post_count: int
     pool_update_count: int
     series_update_count: int
     tag_update_count: int
     artist_update_count: int
-    show_popup_version: int
-    credits: int
-    credits_subs: int
-    is_ai_beta: bool
 
-    # The following fields can be missing in API json response
+    # The following fields can be missing in server JSON response
     last_logged_in_at: Optional[datetime] = None
     favorite_count: Optional[int] = None
     post_favorite_count: Optional[int]
     pool_favorite_count: Optional[int]
     vote_count: Optional[int] = None
     post_vote_count: Optional[int] = None
     pool_vote_count: Optional[int] = None
     recommended_posts_for_user: Optional[int] = None
     subscriptions: List[str] = []
 
+    # The following fields was removed from server JSON response
+    # TODO: Remove in future versions
+    show_popup_version: Optional[int] = None  # Still present in ExtendedUser
+    credits: Optional[int] = None  # Still present in ExtendedUser
+    credits_subs: Optional[int] = None  # Still present in ExtendedUser
+    is_ai_beta: Optional[bool] = None
+
 
 class ExtendedUser(User):
     """Profile of the currently logged-in user."""
     email: str
     hide_ads: bool
     subscription_level: int
     filter_content: bool
+    has_mail: bool
     receive_dmails: bool
     email_verification_status: str
     is_verified: bool
     verifications_count: int
     blacklist_is_hidden: bool
     blacklisted_tags: List[str]
     blacklisted: List[str]
```

### Comparing `sankaku-1.0.2/sankaku/paginators/abc.py` & `sankaku-1.0.3/sankaku/paginators/abc.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/paginators/paginators.py` & `sankaku-1.0.3/sankaku/paginators/paginators.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/types.py` & `sankaku-1.0.3/sankaku/types.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku/utils.py` & `sankaku-1.0.3/sankaku/utils.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.2/sankaku.egg-info/PKG-INFO` & `sankaku-1.0.3/sankaku.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sankaku
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asynchronous API wrapper for Sankaku Complex.
 Home-page: https://github.com/zerex290/sankaku
 Author: zerex290
 Author-email: zerex290@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/zerex290/sankaku/issues
 Keywords: sankaku,sankakucomplex,api
@@ -56,15 +56,15 @@
 ## Requirements
 
 - Python 3.7+
 - aiohttp
 - pydantic
 - loguru
 - aiohttp-retry
-- typing_extensions; python_version < '3.9'
+- typing_extensions; python_version < '3.10'
 
 ## Installation
 
 To install sankaku via pip write following line of code in your terminal:
 
 ```commandline
 pip install sankaku
@@ -82,15 +82,15 @@
 
 Open a command prompt. Navigate to the directory where you want
 to install Sankaku. Type the following command:
 
 ```commandline
 git clone https://github.com/zerex290/sankaku.git
 cd sankaku
-docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3 bash
 ```
 
 ## Usage example
 
 It's very simple to use and doesn't require to always keep opened browser page
 with documentation because all methods are self-explanatory:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sankaku Version: 1.0.2 Summary: Asynchronous API
+Metadata-Version: 2.1 Name: sankaku Version: 1.0.3 Summary: Asynchronous API
 wrapper for Sankaku Complex. Home-page: https://github.com/zerex290/sankaku
 Author: zerex290 Author-email: zerex290@gmail.com License: MIT Project-URL:
 Issue Tracker, https://github.com/zerex290/sankaku/issues Keywords:
 sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -17,25 +17,25 @@
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
 API request parameters to provide better user experience > For instance, you
 can type `types.TagType.ARTIST` instead of `types[]=1` --- Documentation:
 https://zerex290.github.io/sankaku API Reference: https://zerex290.github.io/
 sankaku/api Source code: https://github.com/zerex290/sankaku --- ##
 Requirements - Python 3.7+ - aiohttp - pydantic - loguru - aiohttp-retry -
-typing_extensions; python_version < '3.9' ## Installation To install sankaku
+typing_extensions; python_version < '3.10' ## Installation To install sankaku
 via pip write following line of code in your terminal: ```commandline pip
 install sankaku ``` To install the sankaku via Docker, you can follow these
 steps: ###### Step 1: Install Docker Ensure that Docker is installed on your
 machine. If Docker is not already installed, you can download and install it
 from the official [Docker website](https://www.docker.com/get-started). ######
 Step 2: Use docker to install sankaku Open a command prompt. Navigate to the
 directory where you want to install Sankaku. Type the following command:
 ```commandline git clone https://github.com/zerex290/sankaku.git cd sankaku
-docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash ``` ##
-Usage example It's very simple to use and doesn't require to always keep opened
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3 bash ``` ## Usage
+example It's very simple to use and doesn't require to always keep opened
 browser page with documentation because all methods are self-explanatory: ```py
 import asyncio from sankaku import SankakuClient async def main(): client =
 SankakuClient() post = await client.get_post(25742064) print(f"Rating:
 {post.rating} | Created: {post.created_at}") # "Rating: Rating.QUESTIONABLE |
 Created: 2021-08-01 23:18:52+03:00" await client.login(access_token="token") #
 Or you can authorize by credentials: # await client.login(login="nickname or
 email", password="password") async for book in client.get_recently_read_books
```

### Comparing `sankaku-1.0.2/sankaku.egg-info/SOURCES.txt` & `sankaku-1.0.3/sankaku.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 sankaku.egg-info/requires.txt
 sankaku.egg-info/top_level.txt
 sankaku/clients/__init__.py
 sankaku/clients/abc.py
 sankaku/clients/clients.py
 sankaku/clients/http_client.py
 sankaku/models/__init__.py
+sankaku/models/base.py
 sankaku/models/books.py
 sankaku/models/http.py
 sankaku/models/pages.py
 sankaku/models/posts.py
 sankaku/models/tags.py
 sankaku/models/users.py
 sankaku/paginators/__init__.py
```

### Comparing `sankaku-1.0.2/setup.py` & `sankaku-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     item.group(1): _load_req(item.group(0))
     for item in [_REQ_PATTERN.fullmatch(reqpath) for reqpath in os.listdir()]
     if item
 }
 
 setuptools.setup(
     name="sankaku",
-    version="1.0.2",
+    version="1.0.3",
     author="zerex290",
     author_email="zerex290@gmail.com",
     description="Asynchronous API wrapper for Sankaku Complex.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="sankaku sankakucomplex api".split(),
     url="https://github.com/zerex290/sankaku",
```

