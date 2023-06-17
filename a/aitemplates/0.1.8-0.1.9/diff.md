# Comparing `tmp/aitemplates-0.1.8.tar.gz` & `tmp/aitemplates-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitemplates-0.1.8.tar", max compression
+gzip compressed data, was "aitemplates-0.1.9.tar", max compression
```

## Comparing `aitemplates-0.1.8.tar` & `aitemplates-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      414 2023-06-17 00:43:43.133041 aitemplates-0.1.8/aitemplates/__init__.py
--rw-r--r--   0        0        0     3308 2023-06-12 21:37:15.017128 aitemplates-0.1.8/aitemplates/main.py
--rw-r--r--   0        0        0        0 2023-06-11 16:53:31.418163 aitemplates-0.1.8/aitemplates/oai/__init__.py
--rw-r--r--   0        0        0      191 2023-06-11 17:06:23.567459 aitemplates-0.1.8/aitemplates/oai/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3650 2023-06-15 20:56:48.878741 aitemplates-0.1.8/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2023-06-15 20:55:55.542968 aitemplates-0.1.8/aitemplates/oai/ApiManager.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:48.721024 aitemplates-0.1.8/aitemplates/oai/responses/__init__.py
--rw-r--r--   0        0        0      201 2023-06-11 17:06:23.571195 aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5621 2023-06-15 21:01:08.775227 aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc
--rw-r--r--   0        0        0     3623 2023-06-17 00:22:05.025665 aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc
--rw-r--r--   0        0        0     2295 2023-06-15 23:23:34.942772 aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc
--rw-r--r--   0        0        0     6922 2023-06-17 04:24:33.988894 aitemplates-0.1.8/aitemplates/oai/responses/async_chat_response.py
--rw-r--r--   0        0        0     5034 2023-06-17 04:26:56.895455 aitemplates-0.1.8/aitemplates/oai/responses/chat_response.py
--rw-r--r--   0        0        0     2166 2023-06-17 04:24:48.674679 aitemplates-0.1.8/aitemplates/oai/responses/embedding.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:43.818807 aitemplates-0.1.8/aitemplates/oai/types/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 17:06:26.080642 aitemplates-0.1.8/aitemplates/oai/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3755 2023-06-17 00:22:05.827507 aitemplates-0.1.8/aitemplates/oai/types/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    10358 2023-06-17 00:22:58.570034 aitemplates-0.1.8/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc
--rw-r--r--   0        0        0     5178 2023-06-16 22:54:06.939606 aitemplates-0.1.8/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc
--rw-r--r--   0        0        0     1368 2023-06-15 04:30:14.843709 aitemplates-0.1.8/aitemplates/oai/types/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0      756 2023-06-15 04:06:26.784850 aitemplates-0.1.8/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc
--rw-r--r--   0        0        0     2855 2023-06-17 00:21:19.676232 aitemplates-0.1.8/aitemplates/oai/types/base.py
--rw-r--r--   0        0        0     9137 2023-06-17 00:22:48.636433 aitemplates-0.1.8/aitemplates/oai/types/chat.py
--rw-r--r--   0        0        0     3690 2023-06-17 04:13:03.598521 aitemplates-0.1.8/aitemplates/oai/types/functions.py
--rw-r--r--   0        0        0     2260 2023-06-15 04:28:59.632351 aitemplates-0.1.8/aitemplates/oai/types/models.py
--rw-r--r--   0        0        0      403 2023-06-12 20:02:50.562326 aitemplates-0.1.8/aitemplates/oai/types/Singleton.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:56.058941 aitemplates-0.1.8/aitemplates/oai/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 17:06:23.576521 aitemplates-0.1.8/aitemplates/oai/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2628 2023-06-15 16:31:05.118939 aitemplates-0.1.8/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc
--rw-r--r--   0        0        0     2381 2023-06-12 21:18:51.833696 aitemplates-0.1.8/aitemplates/oai/utils/count_tokens.py
--rw-r--r--   0        0        0     2857 2023-06-15 16:26:32.681761 aitemplates-0.1.8/aitemplates/oai/utils/wrappers.py
--rw-r--r--   0        0        0     1090 2023-06-17 01:35:58.789843 aitemplates-0.1.8/LICENSE
--rw-r--r--   0        0        0      840 2023-06-17 04:27:16.913351 aitemplates-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3487 2023-06-17 00:47:21.338361 aitemplates-0.1.8/README.md
--rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 aitemplates-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      414 2023-06-17 00:43:43.133041 aitemplates-0.1.9/aitemplates/__init__.py
+-rw-r--r--   0        0        0     3308 2023-06-12 21:37:15.017128 aitemplates-0.1.9/aitemplates/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 16:53:31.418163 aitemplates-0.1.9/aitemplates/oai/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-11 17:06:23.567459 aitemplates-0.1.9/aitemplates/oai/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3650 2023-06-15 20:56:48.878741 aitemplates-0.1.9/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2023-06-15 20:55:55.542968 aitemplates-0.1.9/aitemplates/oai/ApiManager.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:48.721024 aitemplates-0.1.9/aitemplates/oai/responses/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-11 17:06:23.571195 aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5621 2023-06-15 21:01:08.775227 aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc
+-rw-r--r--   0        0        0     3623 2023-06-17 00:22:05.025665 aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc
+-rw-r--r--   0        0        0     2295 2023-06-15 23:23:34.942772 aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc
+-rw-r--r--   0        0        0     6922 2023-06-17 04:24:33.988894 aitemplates-0.1.9/aitemplates/oai/responses/async_chat_response.py
+-rw-r--r--   0        0        0     5034 2023-06-17 04:26:56.895455 aitemplates-0.1.9/aitemplates/oai/responses/chat_response.py
+-rw-r--r--   0        0        0     2166 2023-06-17 04:24:48.674679 aitemplates-0.1.9/aitemplates/oai/responses/embedding.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:43.818807 aitemplates-0.1.9/aitemplates/oai/types/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 17:06:26.080642 aitemplates-0.1.9/aitemplates/oai/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3755 2023-06-17 00:22:05.827507 aitemplates-0.1.9/aitemplates/oai/types/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    10358 2023-06-17 00:22:58.570034 aitemplates-0.1.9/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc
+-rw-r--r--   0        0        0     5178 2023-06-16 22:54:06.939606 aitemplates-0.1.9/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc
+-rw-r--r--   0        0        0     1368 2023-06-15 04:30:14.843709 aitemplates-0.1.9/aitemplates/oai/types/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0      756 2023-06-15 04:06:26.784850 aitemplates-0.1.9/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc
+-rw-r--r--   0        0        0     2855 2023-06-17 00:21:19.676232 aitemplates-0.1.9/aitemplates/oai/types/base.py
+-rw-r--r--   0        0        0     9137 2023-06-17 00:22:48.636433 aitemplates-0.1.9/aitemplates/oai/types/chat.py
+-rw-r--r--   0        0        0     3690 2023-06-17 04:13:03.598521 aitemplates-0.1.9/aitemplates/oai/types/functions.py
+-rw-r--r--   0        0        0     2260 2023-06-15 04:28:59.632351 aitemplates-0.1.9/aitemplates/oai/types/models.py
+-rw-r--r--   0        0        0      403 2023-06-12 20:02:50.562326 aitemplates-0.1.9/aitemplates/oai/types/Singleton.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:56.058941 aitemplates-0.1.9/aitemplates/oai/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 17:06:23.576521 aitemplates-0.1.9/aitemplates/oai/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2628 2023-06-15 16:31:05.118939 aitemplates-0.1.9/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc
+-rw-r--r--   0        0        0     2381 2023-06-12 21:18:51.833696 aitemplates-0.1.9/aitemplates/oai/utils/count_tokens.py
+-rw-r--r--   0        0        0     3174 2023-06-17 04:33:31.367260 aitemplates-0.1.9/aitemplates/oai/utils/wrappers.py
+-rw-r--r--   0        0        0     1090 2023-06-17 01:35:58.789843 aitemplates-0.1.9/LICENSE
+-rw-r--r--   0        0        0      840 2023-06-17 04:33:50.253739 aitemplates-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3487 2023-06-17 00:47:21.338361 aitemplates-0.1.9/README.md
+-rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 aitemplates-0.1.9/PKG-INFO
```

### Comparing `aitemplates-0.1.8/aitemplates/main.py` & `aitemplates-0.1.9/aitemplates/main.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/ApiManager.py` & `aitemplates-0.1.9/aitemplates/oai/ApiManager.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/responses/async_chat_response.py` & `aitemplates-0.1.9/aitemplates/oai/responses/async_chat_response.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/responses/chat_response.py` & `aitemplates-0.1.9/aitemplates/oai/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/responses/embedding.py` & `aitemplates-0.1.9/aitemplates/oai/responses/embedding.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/__pycache__/base.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/types/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/types/__pycache__/chat.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/types/__pycache__/functions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/__pycache__/models.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/types/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/base.py` & `aitemplates-0.1.9/aitemplates/oai/types/base.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/chat.py` & `aitemplates-0.1.9/aitemplates/oai/types/chat.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/functions.py` & `aitemplates-0.1.9/aitemplates/oai/types/functions.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/types/models.py` & `aitemplates-0.1.9/aitemplates/oai/types/models.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc` & `aitemplates-0.1.9/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/utils/count_tokens.py` & `aitemplates-0.1.9/aitemplates/oai/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/aitemplates/oai/utils/wrappers.py` & `aitemplates-0.1.9/aitemplates/oai/utils/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,16 +55,21 @@
                     if not user_warned:
                         logging.warning(
                             """Please double check that you have setup a paid OpenAI API 
                               Account. You can read more here: https://docs.agpt.co/setup/#getting-an-api-key"""
                         )
                         user_warned = True
                 except InvalidRequestError as e:
-                    logging.error(f"OpenAI API Invalid Request: {e}")
-                    user_warned = True
+                    if 'not exist' in str(e):
+                        logging.warning(f"Requested model does not exist. Using default model gpt-3.5-turbo-0613.")
+                        kwargs['model'] = "gpt-3.5-turbo-0613"
+                        return func(*args, **kwargs)
+                    else:
+                        logging.error(f"OpenAI API Invalid Request: {e}")
+                        user_warned = True
                 except APIConnectionError as e:
                     logging.error(
                         f"OpenAI API Connection Error: {e}"
                     )
                     user_warned = True
                 except Timeout as e:
                     logging.error(f"OpenAI API Timeout Error: {e}")
```

### Comparing `aitemplates-0.1.8/LICENSE` & `aitemplates-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/pyproject.toml` & `aitemplates-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aitemplates"
-version = "0.1.8"
+version = "0.1.9"
 description = "Designed to streamline and simplify your AI workflows, it offers Python typing support, error checking, and a smart usage meter to manage API costs efficiently. Plus, it features built-in examples with ChromaDB and efficient tools for prompt engineering."
 authors = ["Silen Naihin <silen.naihin@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aitemplates"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `aitemplates-0.1.8/README.md` & `aitemplates-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.8/PKG-INFO` & `aitemplates-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitemplates
-Version: 0.1.8
+Version: 0.1.9
 Summary: Designed to streamline and simplify your AI workflows, it offers Python typing support, error checking, and a smart usage meter to manage API costs efficiently. Plus, it features built-in examples with ChromaDB and efficient tools for prompt engineering.
 Author: Silen Naihin
 Author-email: silen.naihin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

