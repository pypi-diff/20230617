# Comparing `tmp/streamlit_chitchat-0.1.6.tar.gz` & `tmp/streamlit_chitchat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chitchat-0.1.6.tar", max compression
+gzip compressed data, was "streamlit_chitchat-0.1.7.tar", max compression
```

## Comparing `streamlit_chitchat-0.1.6.tar` & `streamlit_chitchat-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1453 2023-06-16 13:15:15.292597 streamlit_chitchat-0.1.6/README.md
--rw-r--r--   0        0        0      627 2023-06-16 18:14:09.093228 streamlit_chitchat-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-16 16:45:14.267359 streamlit_chitchat-0.1.6/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0     4317 2023-06-16 18:12:20.014253 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/chitchat.py
--rw-r--r--   0        0        0     1992 2023-06-16 17:24:05.212800 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/data.py
--rw-r--r--   0        0        0      793 2023-06-16 16:38:43.394926 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/utils.py
--rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit_chitchat-0.1.6/streamlit_chitchat/tests/__init__.py
--rw-r--r--   0        0        0     3508 2023-06-16 18:12:04.074404 streamlit_chitchat-0.1.6/streamlit_chitchat/tests/main.py
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 streamlit_chitchat-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1453 2023-06-17 18:36:51.919463 streamlit_chitchat-0.1.7/README.md
+-rw-r--r--   0        0        0      627 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0     4317 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/streamlit_chitchat/chitchat.py
+-rw-r--r--   0        0        0     1992 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/streamlit_chitchat/data.py
+-rw-r--r--   0        0        0     1140 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/streamlit_chitchat/utils.py
+-rw-r--r--   0        0        0        0 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/tests/__init__.py
+-rw-r--r--   0        0        0     3508 2023-06-17 18:36:51.923463 streamlit_chitchat-0.1.7/streamlit_chitchat/tests/main.py
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 streamlit_chitchat-0.1.7/PKG-INFO
```

### Comparing `streamlit_chitchat-0.1.6/README.md` & `streamlit_chitchat-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.6/pyproject.toml` & `streamlit_chitchat-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-chitchat"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["k4144 <github.k4144@gmail.com>"]
 readme = "README.md"
 packages = [{include = "streamlit_chitchat"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/chitchat.py` & `streamlit_chitchat-0.1.7/streamlit_chitchat/streamlit_chitchat/chitchat.py`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/data.py` & `streamlit_chitchat-0.1.7/streamlit_chitchat/streamlit_chitchat/data.py`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.6/streamlit_chitchat/tests/main.py` & `streamlit_chitchat-0.1.7/streamlit_chitchat/tests/main.py`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.6/PKG-INFO` & `streamlit_chitchat-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chitchat
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: k4144
 Author-email: github.k4144@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

