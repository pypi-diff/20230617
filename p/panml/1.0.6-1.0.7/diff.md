# Comparing `tmp/panml-1.0.6.tar.gz` & `tmp/panml-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-1.0.6.tar", last modified: Thu Jun 15 12:38:30 2023, max compression
+gzip compressed data, was "panml-1.0.7.tar", last modified: Sat Jun 17 04:41:07 2023, max compression
```

## Comparing `panml-1.0.6.tar` & `panml-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-15 12:38:30.417726 panml-1.0.6/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.6/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-15 12:38:30.418068 panml-1.0.6/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.6/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-15 12:38:30.411833 panml-1.0.6/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.6/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-15 12:38:30.414306 panml-1.0.6/panml/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.6/panml/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9463 2023-06-15 12:36:48.000000 panml-1.0.6/panml/clustering/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.6/panml/constants.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.6/panml/environments.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-15 12:38:30.415993 panml-1.0.6/panml/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.6/panml/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    24501 2023-06-15 12:36:48.000000 panml-1.0.6/panml/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-14 02:30:39.000000 panml-1.0.6/panml/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.6/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.6/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-15 12:38:30.413542 panml-1.0.6/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-15 12:38:30.000000 panml-1.0.6/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-15 12:38:30.000000 panml-1.0.6/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-15 12:38:30.000000 panml-1.0.6/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-15 12:38:30.000000 panml-1.0.6/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-15 12:38:30.000000 panml-1.0.6/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-15 12:38:30.419240 panml-1.0.6/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-15 12:36:48.000000 panml-1.0.6/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-15 12:38:30.417198 panml-1.0.6/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.6/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    12552 2023-06-15 12:36:48.000000 panml-1.0.6/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.215625 panml-1.0.7/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.7/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-17 04:41:07.215939 panml-1.0.7/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.7/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.209970 panml-1.0.7/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.7/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.212626 panml-1.0.7/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.7/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9448 2023-06-17 04:40:13.000000 panml-1.0.7/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.7/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.7/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.214082 panml-1.0.7/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.7/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    24501 2023-06-15 12:36:48.000000 panml-1.0.7/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-14 02:30:39.000000 panml-1.0.7/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.7/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.7/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.211812 panml-1.0.7/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-17 04:41:07.216999 panml-1.0.7/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-17 04:40:13.000000 panml-1.0.7/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.215102 panml-1.0.7/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.7/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    12552 2023-06-15 12:36:48.000000 panml-1.0.7/test/test_VectorEngine.py
```

### Comparing `panml-1.0.6/LICENSE` & `panml-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/PKG-INFO` & `panml-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.6
+Version: 1.0.7
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.6/README.md` & `panml-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml/clustering/faiss.py` & `panml-1.0.7/panml/clustering/faiss.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             self.model_emb = None # Embedding model not required with third party API functions
             if api_key is None:
                 raise ValueError('api key has not been specified for OpenAI model call')
             openai.api_key = api_key # Set API key
         else:
             raise ValueError('Embedding model is not recognised or currently supported')
         self.corpus = None
-        self.stored_vectors = None
+        self.vectors = None
         
     def _get_openai_embedding(self, text: str, model: str) -> list[str]:
         text = text.replace('\n', ' ')
         return openai.Embedding.create(input=[text], model=model)['data'][0]['embedding']
     
     def _get_embedding(self, corpus: list[str], model_emb_source: str) -> np.array:
         if model_emb_source == 'huggingface':
@@ -146,15 +146,15 @@
         if not isinstance(corpus_dir, str):
             raise TypeError('Input corpus dir needs to be of type: str')
         else:
             if not corpus_dir.lower().endswith('pkl'):
                 raise ValueError('Input corpus directory needs to end with .pkl')
         
         # Load the vectors and corpus
-        self.stored_vectors = faiss.read_index(f"{vectors_dir}") # load vectors
+        self.vectors = faiss.read_index(f"{vectors_dir}") # load vectors
         with open(f"{corpus_dir}", "rb") as f: # load corpus
             self.corpus = pickle.load(f)
 
     # Perform vector search of query against stored vectors and retrieve top k results
     def search(self, query: str, k: int, return_index: bool=False) -> Union[list[str], dict[str, str]]:
         '''
         Runs vector search of input query against the stored vectors.
@@ -182,10 +182,10 @@
             
         if k > len(self.corpus):
             k = len(self.corpus) # cap the max k to the maximum number of documents in the corpus store
         query_vector = self._get_embedding([query], self.model_emb_source) # embed input vector
         _, I = self.vectors.search(query_vector, k) # perform vector search
 
         if return_index:
-            return {'sample': list(np.array(self.corpus)[I][0]), 'idx': list(I[0])} # return samples and idx
+            return {'sample': list(np.array(self.corpus)[I][0]), 'id': list(I[0])} # return samples and idx
         else:
             return list(np.array(self.corpus)[I][0]) # return samples only
```

### Comparing `panml-1.0.6/panml/constants.py` & `panml-1.0.7/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml/environments.py` & `panml-1.0.7/panml/environments.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml/llm/huggingface.py` & `panml-1.0.7/panml/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml/llm/openai.py` & `panml-1.0.7/panml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml/models.py` & `panml-1.0.7/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml/search.py` & `panml-1.0.7/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/panml.egg-info/PKG-INFO` & `panml-1.0.7/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.6
+Version: 1.0.7
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.6/setup.py` & `panml-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '1.0.6', # version
+  version = '1.0.7', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-1.0.6/test/test_ModelPack.py` & `panml-1.0.7/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.6/test/test_VectorEngine.py` & `panml-1.0.7/test/test_VectorEngine.py`

 * *Files identical despite different names*

