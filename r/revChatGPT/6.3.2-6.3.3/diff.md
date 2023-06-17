# Comparing `tmp/revChatGPT-6.3.2.tar.gz` & `tmp/revChatGPT-6.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.3.2.tar", last modified: Fri Jun 16 08:50:47 2023, max compression
+gzip compressed data, was "revChatGPT-6.3.3.tar", last modified: Sat Jun 17 02:23:23 2023, max compression
```

## Comparing `revChatGPT-6.3.2.tar` & `revChatGPT-6.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-16 08:50:47.000000 revChatGPT-6.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:50:47.489462 revChatGPT-6.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58784 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-16 08:50:47.000000 revChatGPT-6.3.2/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-16 08:50:47.000000 revChatGPT-6.3.2/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:50:47.000000 revChatGPT-6.3.2/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 08:50:47.000000 revChatGPT-6.3.2/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 08:50:47.000000 revChatGPT-6.3.2/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:50:47.493462 revChatGPT-6.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 08:50:17.000000 revChatGPT-6.3.2/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.729875 revChatGPT-6.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58838 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/tests/test_recipient.py
```

### Comparing `revChatGPT-6.3.2/LICENSE` & `revChatGPT-6.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/PKG-INFO` & `revChatGPT-6.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.2
+Version: 6.3.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.3.2/README.md` & `revChatGPT-6.3.3/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/setup.py` & `revChatGPT-6.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.3.2",
+    version="6.3.3",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.3.2/src/revChatGPT/V1.py` & `revChatGPT-6.3.3/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,14 +452,15 @@
             self.conversation_id = cid
 
         if not (auto_continue and finish_details == "max_tokens"):
             return
         message = message.strip("\n")
         for i in self.continue_write(
             conversation_id=cid,
+            model=model,
             timeout=timeout,
             auto_continue=False,
         ):
             i["message"] = message + i["message"]
             yield i
 
     @logger(is_timed=True)
@@ -1032,14 +1033,15 @@
                 self.conversation_id = cid
 
             if not (auto_continue and finish_details == "max_tokens"):
                 return
             message = message.strip("\n")
             async for i in self.continue_write(
                 conversation_id=cid,
+                model=model,
                 timeout=timeout,
                 auto_continue=False,
             ):
                 i["message"] = message + i["message"]
                 yield i
 
     async def post_messages(
```

### Comparing `revChatGPT-6.3.2/src/revChatGPT/V3.py` & `revChatGPT-6.3.3/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/src/revChatGPT/__init__.py` & `revChatGPT-6.3.3/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/src/revChatGPT/__main__.py` & `revChatGPT-6.3.3/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.3.3/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/src/revChatGPT/typings.py` & `revChatGPT-6.3.3/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/src/revChatGPT/utils.py` & `revChatGPT-6.3.3/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.2/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.3.3/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.2
+Version: 6.3.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.3.2/tests/test_recipient.py` & `revChatGPT-6.3.3/tests/test_recipient.py`

 * *Files identical despite different names*

