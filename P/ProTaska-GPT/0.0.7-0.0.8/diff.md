# Comparing `tmp/ProTaska-GPT-0.0.7.tar.gz` & `tmp/ProTaska-GPT-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.7.tar", last modified: Sat Jun 17 16:49:10 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.8.tar", last modified: Sat Jun 17 16:57:49 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.7.tar` & `ProTaska-GPT-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:49:10.336125 ProTaska-GPT-0.0.7/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:49:10.317832 ProTaska-GPT-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:49:10.115134 ProTaska-GPT-0.0.7/ProTaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.7/ProTaska/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:49:10.224990 ProTaska-GPT-0.0.7/ProTaska/data/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.7/ProTaska/data/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.7/ProTaska/data/data_utils.py
--rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.7/ProTaska/data/ingestion.py
--rw-rw-rw-   0        0        0     5317 2023-06-17 15:32:34.000000 ProTaska-GPT-0.0.7/ProTaska/data/loader.py
--rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.7/ProTaska/describer.py
--rw-rw-rw-   0        0        0     3323 2023-06-17 16:48:44.000000 ProTaska-GPT-0.0.7/ProTaska/ideate.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:49:10.311403 ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:49:09.000000 ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-17 16:49:10.000000 ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:49:09.000000 ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-17 16:49:09.000000 ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 16:49:09.000000 ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 16:49:10.336125 ProTaska-GPT-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-06-17 16:48:49.000000 ProTaska-GPT-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.718547 ProTaska-GPT-0.0.8/ProTaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.8/ProTaska/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.721425 ProTaska-GPT-0.0.8/ProTaska/data/
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.8/ProTaska/data/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.8/ProTaska/data/data_utils.py
+-rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.8/ProTaska/data/ingestion.py
+-rw-rw-rw-   0        0        0     5357 2023-06-17 16:57:15.000000 ProTaska-GPT-0.0.8/ProTaska/data/loader.py
+-rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.8/ProTaska/describer.py
+-rw-rw-rw-   0        0        0     3323 2023-06-17 16:48:44.000000 ProTaska-GPT-0.0.8/ProTaska/ideate.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-06-17 16:57:21.000000 ProTaska-GPT-0.0.8/setup.py
```

### Comparing `ProTaska-GPT-0.0.7/LICENSE` & `ProTaska-GPT-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.7/PKG-INFO` & `ProTaska-GPT-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.7/ProTaska/data/data_utils.py` & `ProTaska-GPT-0.0.8/ProTaska/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.7/ProTaska/data/ingestion.py` & `ProTaska-GPT-0.0.8/ProTaska/data/ingestion.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.7/ProTaska/data/loader.py` & `ProTaska-GPT-0.0.8/ProTaska/data/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,18 @@
                     'absolute_path': absolute_path,
                     'memory_size': str(round(memory_size, 4))+"mb"
                 })
         dataset = self.get_meta_data(dataset)
         dataset = self.reformat_dataset(dataset)
         self.dataset = "\n\n".join(dataset)
 
-    def ingest(self, llm, chunk_size=500):
+    def ingest(self, llm, chunk_size=500, verbose=False):
         details = self.dataset
-        print(colorama.Fore.BLUE+"Going to summarize:\n"+colorama.Fore.RESET,colorama.Fore.GREEN+str(details)+colorama.Fore.RESET)
+        if verbose:
+            print(colorama.Fore.BLUE+"Going to summarize:\n"+colorama.Fore.RESET,colorama.Fore.GREEN+str(details)+colorama.Fore.RESET)
         llm_chain = IngestionChain(llm=llm)
         out = None
         while len(details) > 0:
             chunk = details[:chunk_size]
             details = details[chunk_size:]
             if out is None:
                 out = llm_chain.run(self.prompt_prefix+chunk)
```

### Comparing `ProTaska-GPT-0.0.7/ProTaska/describer.py` & `ProTaska-GPT-0.0.8/ProTaska/describer.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.7/ProTaska/ideate.py` & `ProTaska-GPT-0.0.8/ProTaska/ideate.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.7/ProTaska_GPT.egg-info/PKG-INFO` & `ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.7/README.md` & `ProTaska-GPT-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.7/setup.py` & `ProTaska-GPT-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ProTaska-GPT',
-    version='0.0.7',
+    version='0.0.8',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=find_packages(exclude=["notebooks", "docs"]),
     url='https://github.com/AmanPriyanshu/protaska-gpt',
```

