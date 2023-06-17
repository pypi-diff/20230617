# Comparing `tmp/ProTaska-GPT-0.0.5.tar.gz` & `tmp/ProTaska-GPT-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.5.tar", last modified: Sat Jun 17 16:39:16 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.6.tar", last modified: Sat Jun 17 16:47:42 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.5.tar` & `ProTaska-GPT-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:39:15.809784 ProTaska-GPT-0.0.5/ProTaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.5/ProTaska/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:39:15.873554 ProTaska-GPT-0.0.5/ProTaska/data/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.5/ProTaska/data/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.5/ProTaska/data/data_utils.py
--rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.5/ProTaska/data/ingestion.py
--rw-rw-rw-   0        0        0     5317 2023-06-17 15:32:34.000000 ProTaska-GPT-0.0.5/ProTaska/data/loader.py
--rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.5/ProTaska/describer.py
--rw-rw-rw-   0        0        0     3151 2023-06-17 16:38:49.000000 ProTaska-GPT-0.0.5/ProTaska/ideate.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-06-17 16:35:03.000000 ProTaska-GPT-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:47:42.892117 ProTaska-GPT-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:47:42.892117 ProTaska-GPT-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 16:47:42.671483 ProTaska-GPT-0.0.6/ProTaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.6/ProTaska/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:47:42.781370 ProTaska-GPT-0.0.6/ProTaska/data/
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.6/ProTaska/data/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.6/ProTaska/data/data_utils.py
+-rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.6/ProTaska/data/ingestion.py
+-rw-rw-rw-   0        0        0     5317 2023-06-17 15:32:34.000000 ProTaska-GPT-0.0.6/ProTaska/data/loader.py
+-rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.6/ProTaska/describer.py
+-rw-rw-rw-   0        0        0     3280 2023-06-17 16:46:46.000000 ProTaska-GPT-0.0.6/ProTaska/ideate.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:47:42.892117 ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:47:42.000000 ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-17 16:47:42.000000 ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:47:42.000000 ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-17 16:47:42.000000 ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 16:47:42.000000 ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:47:42.892117 ProTaska-GPT-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-06-17 16:47:18.000000 ProTaska-GPT-0.0.6/setup.py
```

### Comparing `ProTaska-GPT-0.0.5/LICENSE` & `ProTaska-GPT-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.5/PKG-INFO` & `ProTaska-GPT-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.5/ProTaska/data/data_utils.py` & `ProTaska-GPT-0.0.6/ProTaska/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.5/ProTaska/data/ingestion.py` & `ProTaska-GPT-0.0.6/ProTaska/data/ingestion.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.5/ProTaska/data/loader.py` & `ProTaska-GPT-0.0.6/ProTaska/data/loader.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.5/ProTaska/describer.py` & `ProTaska-GPT-0.0.6/ProTaska/describer.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.5/ProTaska/ideate.py` & `ProTaska-GPT-0.0.6/ProTaska/ideate.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,9 +56,12 @@
 def main(openai_key, dataset_description):
     chat_bot = ChatBotWrapper(openai_key, dataset_description)
     print("ProTaska:\t", chat_bot.first_output)
     print("ProTaska-Source:\t", chat_bot.second_output)
     print()
     while True:
         human_input = input("Human:\t")
+        if human_input=='exit' or human_input=='break':
+            print("ProTaska:\tStopping Execution!")
+            break
         print("ProTaska:\t", chat_bot(human_input))
         print()
```

### Comparing `ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/PKG-INFO` & `ProTaska-GPT-0.0.6/ProTaska_GPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.5/README.md` & `ProTaska-GPT-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.5/setup.py` & `ProTaska-GPT-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ProTaska-GPT',
-    version='0.0.5',
+    version='0.0.6',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=find_packages(exclude=["notebooks", "docs"]),
     url='https://github.com/AmanPriyanshu/protaska-gpt',
```

