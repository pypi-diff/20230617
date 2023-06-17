# Comparing `tmp/ProTaska-GPT-0.0.4.tar.gz` & `tmp/ProTaska-GPT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.4.tar", last modified: Sat Jun 17 16:24:43 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.5.tar", last modified: Sat Jun 17 16:39:16 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.4.tar` & `ProTaska-GPT-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.903261 ProTaska-GPT-0.0.4/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:24:43.901078 ProTaska-GPT-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.736427 ProTaska-GPT-0.0.4/ProTaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.4/ProTaska/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.800058 ProTaska-GPT-0.0.4/ProTaska/data/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.4/ProTaska/data/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.4/ProTaska/data/data_utils.py
--rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.4/ProTaska/data/ingestion.py
--rw-rw-rw-   0        0        0     5317 2023-06-17 15:32:34.000000 ProTaska-GPT-0.0.4/ProTaska/data/loader.py
--rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.4/ProTaska/describer.py
--rw-rw-rw-   0        0        0     3143 2023-06-17 16:18:56.000000 ProTaska-GPT-0.0.4/ProTaska/ideate.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.889546 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 16:24:43.904309 ProTaska-GPT-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-06-17 16:24:33.000000 ProTaska-GPT-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 16:39:15.809784 ProTaska-GPT-0.0.5/ProTaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.5/ProTaska/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:39:15.873554 ProTaska-GPT-0.0.5/ProTaska/data/
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.5/ProTaska/data/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.5/ProTaska/data/data_utils.py
+-rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.5/ProTaska/data/ingestion.py
+-rw-rw-rw-   0        0        0     5317 2023-06-17 15:32:34.000000 ProTaska-GPT-0.0.5/ProTaska/data/loader.py
+-rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.5/ProTaska/describer.py
+-rw-rw-rw-   0        0        0     3151 2023-06-17 16:38:49.000000 ProTaska-GPT-0.0.5/ProTaska/ideate.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 16:39:15.000000 ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:39:16.031219 ProTaska-GPT-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-06-17 16:35:03.000000 ProTaska-GPT-0.0.5/setup.py
```

### Comparing `ProTaska-GPT-0.0.4/LICENSE` & `ProTaska-GPT-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.4/PKG-INFO` & `ProTaska-GPT-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.4
+Version: 0.0.5
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.4/ProTaska/data/data_utils.py` & `ProTaska-GPT-0.0.5/ProTaska/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.4/ProTaska/data/ingestion.py` & `ProTaska-GPT-0.0.5/ProTaska/data/ingestion.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.4/ProTaska/data/loader.py` & `ProTaska-GPT-0.0.5/ProTaska/data/loader.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.4/ProTaska/describer.py` & `ProTaska-GPT-0.0.5/ProTaska/describer.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.4/ProTaska/ideate.py` & `ProTaska-GPT-0.0.5/ProTaska/ideate.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         ),
         self.agent_chain = initialize_agent(tools=tools, 
             llm=self.llm, 
             agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION, 
             memory=self.memory,
             verbose=agent_verbose
         )
-        self.second_output = self.agent_chain.run("Find relevant sources from Wikipedia from the above techniques and advances you just said. Also include some TLDRs in front of those links. Be specific to the ML techniques previously mentioned.")
+        self.second_output = self.agent_chain.run(self.first_output+"\n\nFind relevant sources from Wikipedia from the above techniques and advances. Also include some TLDRs in front of those links. Be specific to the ML techniques previously mentioned.")
 
     def __call__(self, human_input):
         output = self.agent_chain.run(human_input)
         return output
 
 def main(openai_key, dataset_description):
     chat_bot = ChatBotWrapper(openai_key, dataset_description)
```

### Comparing `ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/PKG-INFO` & `ProTaska-GPT-0.0.5/ProTaska_GPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.4
+Version: 0.0.5
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.4/README.md` & `ProTaska-GPT-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.4/setup.py` & `ProTaska-GPT-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ProTaska-GPT',
-    version='0.0.4',
+    version='0.0.5',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=find_packages(exclude=["notebooks", "docs"]),
     url='https://github.com/AmanPriyanshu/protaska-gpt',
     install_requires=[
         'langchain',
         'numpy',
         'pandas',
         'colorama',
         'wikipedia',
         'openai',
+        'datasets',
+        'tiktoken'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

