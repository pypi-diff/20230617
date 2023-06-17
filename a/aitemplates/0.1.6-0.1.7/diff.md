# Comparing `tmp/aitemplates-0.1.6.tar.gz` & `tmp/aitemplates-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitemplates-0.1.6.tar", max compression
+gzip compressed data, was "aitemplates-0.1.7.tar", max compression
```

## Comparing `aitemplates-0.1.6.tar` & `aitemplates-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      414 2023-06-17 00:43:43.133041 aitemplates-0.1.6/aitemplates/__init__.py
--rw-r--r--   0        0        0     3308 2023-06-12 21:37:15.017128 aitemplates-0.1.6/aitemplates/main.py
--rw-r--r--   0        0        0        0 2023-06-11 16:53:31.418163 aitemplates-0.1.6/aitemplates/oai/__init__.py
--rw-r--r--   0        0        0      191 2023-06-11 17:06:23.567459 aitemplates-0.1.6/aitemplates/oai/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3650 2023-06-15 20:56:48.878741 aitemplates-0.1.6/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2023-06-15 20:55:55.542968 aitemplates-0.1.6/aitemplates/oai/ApiManager.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:48.721024 aitemplates-0.1.6/aitemplates/oai/responses/__init__.py
--rw-r--r--   0        0        0      201 2023-06-11 17:06:23.571195 aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5621 2023-06-15 21:01:08.775227 aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc
--rw-r--r--   0        0        0     3623 2023-06-17 00:22:05.025665 aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc
--rw-r--r--   0        0        0     2295 2023-06-15 23:23:34.942772 aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc
--rw-r--r--   0        0        0     6755 2023-06-15 20:56:18.901134 aitemplates-0.1.6/aitemplates/oai/responses/async_chat_response.py
--rw-r--r--   0        0        0     4839 2023-06-17 04:15:49.699410 aitemplates-0.1.6/aitemplates/oai/responses/chat_response.py
--rw-r--r--   0        0        0     1999 2023-06-15 23:23:26.602357 aitemplates-0.1.6/aitemplates/oai/responses/embedding.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:43.818807 aitemplates-0.1.6/aitemplates/oai/types/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 17:06:26.080642 aitemplates-0.1.6/aitemplates/oai/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3755 2023-06-17 00:22:05.827507 aitemplates-0.1.6/aitemplates/oai/types/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    10358 2023-06-17 00:22:58.570034 aitemplates-0.1.6/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc
--rw-r--r--   0        0        0     5178 2023-06-16 22:54:06.939606 aitemplates-0.1.6/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc
--rw-r--r--   0        0        0     1368 2023-06-15 04:30:14.843709 aitemplates-0.1.6/aitemplates/oai/types/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0      756 2023-06-15 04:06:26.784850 aitemplates-0.1.6/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc
--rw-r--r--   0        0        0     2855 2023-06-17 00:21:19.676232 aitemplates-0.1.6/aitemplates/oai/types/base.py
--rw-r--r--   0        0        0     9137 2023-06-17 00:22:48.636433 aitemplates-0.1.6/aitemplates/oai/types/chat.py
--rw-r--r--   0        0        0     3690 2023-06-17 04:13:03.598521 aitemplates-0.1.6/aitemplates/oai/types/functions.py
--rw-r--r--   0        0        0     2260 2023-06-15 04:28:59.632351 aitemplates-0.1.6/aitemplates/oai/types/models.py
--rw-r--r--   0        0        0      403 2023-06-12 20:02:50.562326 aitemplates-0.1.6/aitemplates/oai/types/Singleton.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:56.058941 aitemplates-0.1.6/aitemplates/oai/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 17:06:23.576521 aitemplates-0.1.6/aitemplates/oai/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2628 2023-06-15 16:31:05.118939 aitemplates-0.1.6/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc
--rw-r--r--   0        0        0     2381 2023-06-12 21:18:51.833696 aitemplates-0.1.6/aitemplates/oai/utils/count_tokens.py
--rw-r--r--   0        0        0     2857 2023-06-15 16:26:32.681761 aitemplates-0.1.6/aitemplates/oai/utils/wrappers.py
--rw-r--r--   0        0        0     1090 2023-06-17 01:35:58.789843 aitemplates-0.1.6/LICENSE
--rw-r--r--   0        0        0      818 2023-06-17 04:16:26.580462 aitemplates-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3487 2023-06-17 00:47:21.338361 aitemplates-0.1.6/README.md
--rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 aitemplates-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      414 2023-06-17 00:43:43.133041 aitemplates-0.1.7/aitemplates/__init__.py
+-rw-r--r--   0        0        0     3308 2023-06-12 21:37:15.017128 aitemplates-0.1.7/aitemplates/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 16:53:31.418163 aitemplates-0.1.7/aitemplates/oai/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-11 17:06:23.567459 aitemplates-0.1.7/aitemplates/oai/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3650 2023-06-15 20:56:48.878741 aitemplates-0.1.7/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2023-06-15 20:55:55.542968 aitemplates-0.1.7/aitemplates/oai/ApiManager.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:48.721024 aitemplates-0.1.7/aitemplates/oai/responses/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-11 17:06:23.571195 aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5621 2023-06-15 21:01:08.775227 aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc
+-rw-r--r--   0        0        0     3623 2023-06-17 00:22:05.025665 aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc
+-rw-r--r--   0        0        0     2295 2023-06-15 23:23:34.942772 aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc
+-rw-r--r--   0        0        0     6922 2023-06-17 04:24:33.988894 aitemplates-0.1.7/aitemplates/oai/responses/async_chat_response.py
+-rw-r--r--   0        0        0     5006 2023-06-17 04:24:42.678098 aitemplates-0.1.7/aitemplates/oai/responses/chat_response.py
+-rw-r--r--   0        0        0     2166 2023-06-17 04:24:48.674679 aitemplates-0.1.7/aitemplates/oai/responses/embedding.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:43.818807 aitemplates-0.1.7/aitemplates/oai/types/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 17:06:26.080642 aitemplates-0.1.7/aitemplates/oai/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3755 2023-06-17 00:22:05.827507 aitemplates-0.1.7/aitemplates/oai/types/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    10358 2023-06-17 00:22:58.570034 aitemplates-0.1.7/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc
+-rw-r--r--   0        0        0     5178 2023-06-16 22:54:06.939606 aitemplates-0.1.7/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc
+-rw-r--r--   0        0        0     1368 2023-06-15 04:30:14.843709 aitemplates-0.1.7/aitemplates/oai/types/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0      756 2023-06-15 04:06:26.784850 aitemplates-0.1.7/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc
+-rw-r--r--   0        0        0     2855 2023-06-17 00:21:19.676232 aitemplates-0.1.7/aitemplates/oai/types/base.py
+-rw-r--r--   0        0        0     9137 2023-06-17 00:22:48.636433 aitemplates-0.1.7/aitemplates/oai/types/chat.py
+-rw-r--r--   0        0        0     3690 2023-06-17 04:13:03.598521 aitemplates-0.1.7/aitemplates/oai/types/functions.py
+-rw-r--r--   0        0        0     2260 2023-06-15 04:28:59.632351 aitemplates-0.1.7/aitemplates/oai/types/models.py
+-rw-r--r--   0        0        0      403 2023-06-12 20:02:50.562326 aitemplates-0.1.7/aitemplates/oai/types/Singleton.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:56.058941 aitemplates-0.1.7/aitemplates/oai/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 17:06:23.576521 aitemplates-0.1.7/aitemplates/oai/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2628 2023-06-15 16:31:05.118939 aitemplates-0.1.7/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc
+-rw-r--r--   0        0        0     2381 2023-06-12 21:18:51.833696 aitemplates-0.1.7/aitemplates/oai/utils/count_tokens.py
+-rw-r--r--   0        0        0     2857 2023-06-15 16:26:32.681761 aitemplates-0.1.7/aitemplates/oai/utils/wrappers.py
+-rw-r--r--   0        0        0     1090 2023-06-17 01:35:58.789843 aitemplates-0.1.7/LICENSE
+-rw-r--r--   0        0        0      840 2023-06-17 04:25:25.268729 aitemplates-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3487 2023-06-17 00:47:21.338361 aitemplates-0.1.7/README.md
+-rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 aitemplates-0.1.7/PKG-INFO
```

### Comparing `aitemplates-0.1.6/aitemplates/main.py` & `aitemplates-0.1.7/aitemplates/main.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/ApiManager.py` & `aitemplates-0.1.7/aitemplates/oai/ApiManager.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/responses/async_chat_response.py` & `aitemplates-0.1.7/aitemplates/oai/responses/async_chat_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from aiohttp import ClientSession
 from tqdm.asyncio import tqdm_asyncio
 
 from aitemplates.oai.types.base import ResponseDict
 from aitemplates.oai.types.chat import ChatConversation, FunctionsAvailable, ChatPair
 from aitemplates.oai.ApiManager import ApiManager
 
-load_dotenv()
+dotenv_path = os.path.join(os.getcwd(), '.env')  # get the path to .env file in current working directory
+load_dotenv(dotenv_path)  # load environment variables from the .env file
 
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
 
 if OPENAI_API_KEY is None:
     raise Exception("API key not found in environment variables")
 
 openai.api_key = OPENAI_API_KEY
```

### Comparing `aitemplates-0.1.6/aitemplates/oai/responses/chat_response.py` & `aitemplates-0.1.7/aitemplates/oai/responses/chat_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import openai
 from aitemplates.oai.ApiManager import ApiManager
 
 from aitemplates.oai.utils.wrappers import retry_openai_api
 from aitemplates.oai.types.chat import ChatSequence, FunctionsAvailable, ChatConversation, Message
 
-load_dotenv()
+dotenv_path = os.path.join(os.getcwd(), '.env')  # get the path to .env file in current working directory
+load_dotenv(dotenv_path)  # load environment variables from the .env file
 
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
 
 if OPENAI_API_KEY is None:
     raise Exception("API key not found in environment variables")
 
 openai.api_key = OPENAI_API_KEY
```

### Comparing `aitemplates-0.1.6/aitemplates/oai/responses/embedding.py` & `aitemplates-0.1.7/aitemplates/oai/responses/embedding.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from dotenv import load_dotenv
 
 import openai
 
 from aitemplates.oai.utils.wrappers import retry_openai_api
 from aitemplates.oai.ApiManager import ApiManager
 
-load_dotenv()
+dotenv_path = os.path.join(os.getcwd(), '.env')  # get the path to .env file in current working directory
+load_dotenv(dotenv_path)  # load environment variables from the .env file
 
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
 
 if OPENAI_API_KEY is None:
     raise Exception("API key not found in environment variables")
 
 openai.api_key = OPENAI_API_KEY
```

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/__pycache__/base.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/types/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/__pycache__/models.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/types/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/base.py` & `aitemplates-0.1.7/aitemplates/oai/types/base.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/chat.py` & `aitemplates-0.1.7/aitemplates/oai/types/chat.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/functions.py` & `aitemplates-0.1.7/aitemplates/oai/types/functions.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/types/models.py` & `aitemplates-0.1.7/aitemplates/oai/types/models.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc` & `aitemplates-0.1.7/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/utils/count_tokens.py` & `aitemplates-0.1.7/aitemplates/oai/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/aitemplates/oai/utils/wrappers.py` & `aitemplates-0.1.7/aitemplates/oai/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/LICENSE` & `aitemplates-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/pyproject.toml` & `aitemplates-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aitemplates"
-version = "0.1.6"
+version = "0.1.7"
 description = "Designed to streamline and simplify your AI workflows, it offers Python typing support, error checking, and a smart usage meter to manage API costs efficiently. Plus, it features built-in examples with ChromaDB and efficient tools for prompt engineering."
 authors = ["Silen Naihin <silen.naihin@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aitemplates"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,14 +12,15 @@
 openai = "^0.27.8"
 aiolimiter = "^1.1.0"
 aiohttp = "^3.8.4"
 nbformat = "^5.9.0"
 argparse = "^1.4.0"
 pydantic = "^1.10.9"
 jsonschema = "^4.17.3"
+termcolor = "^2.3.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `aitemplates-0.1.6/README.md` & `aitemplates-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.6/PKG-INFO` & `aitemplates-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitemplates
-Version: 0.1.6
+Version: 0.1.7
 Summary: Designed to streamline and simplify your AI workflows, it offers Python typing support, error checking, and a smart usage meter to manage API costs efficiently. Plus, it features built-in examples with ChromaDB and efficient tools for prompt engineering.
 Author: Silen Naihin
 Author-email: silen.naihin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,15 @@
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: chromadb (>=0.3.26,<0.4.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: nbformat (>=5.9.0,<6.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ##### Library is up to date with function calling. Reference oai_examples.ipynb to see functionality. All other docs including ipynb, templates, readme still need to be updated
 
 # aitemplates
 
 aitemplates is a Python package designed to simplify and streamline your work with the OpenAI API. It provides Python typing support, error checking, and a usage meter to help manage API costs. Additionally, aitemplates offers built-in examples of using ChromaDB and tools for efficient prompt engineering with OpenAI.
```

