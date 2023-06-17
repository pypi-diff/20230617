# Comparing `tmp/languagemodels-0.4.0.tar.gz` & `tmp/languagemodels-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.4.0.tar", last modified: Sat Jun 17 13:08:58 2023, max compression
+gzip compressed data, was "languagemodels-0.5.0.tar", last modified: Sat Jun 17 20:35:31 2023, max compression
```

## Comparing `languagemodels-0.4.0.tar` & `languagemodels-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 13:08:58.337436 languagemodels-0.4.0/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8928 2023-06-17 13:08:58.333436 languagemodels-0.4.0/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 13:08:58.333436 languagemodels-0.4.0/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10516 2023-06-17 13:06:52.000000 languagemodels-0.4.0/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4577 2023-06-17 01:38:19.000000 languagemodels-0.4.0/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7105 2023-06-17 12:18:09.000000 languagemodels-0.4.0/languagemodels/inference.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4078 2023-06-17 01:38:19.000000 languagemodels-0.4.0/languagemodels/models.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 13:08:58.333436 languagemodels-0.4.0/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8928 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      306 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       61 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-17 13:08:58.337436 languagemodels-0.4.0/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      800 2023-06-17 13:08:46.000000 languagemodels-0.4.0/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 20:35:31.764542 languagemodels-0.5.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8930 2023-06-17 20:35:31.764542 languagemodels-0.5.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 20:35:31.764542 languagemodels-0.5.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10532 2023-06-17 20:12:04.000000 languagemodels-0.5.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4577 2023-06-17 01:38:19.000000 languagemodels-0.5.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7105 2023-06-17 19:46:56.000000 languagemodels-0.5.0/languagemodels/inference.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4078 2023-06-17 01:38:19.000000 languagemodels-0.5.0/languagemodels/models.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 20:35:31.764542 languagemodels-0.5.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8930 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      306 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       61 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-17 20:35:31.764542 languagemodels-0.5.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      800 2023-06-17 20:06:30.000000 languagemodels-0.5.0/setup.py
```

### Comparing `languagemodels-0.4.0/PKG-INFO` & `languagemodels-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -64,15 +64,15 @@
         ```python
         >>> import languagemodels as lm
         
         >>> lm.do("Translate to English: Hola, mundo!")
         'Hello, world!'
         
         >>> lm.do("What is the capital of France?")
-        'paris'
+        'Paris.'
         ```
         
         ### Chat
         
         ```python
         >>> chat('''
         ...      System: Respond as a helpful assistant.
@@ -129,23 +129,21 @@
         
         This can also be used to get a blend of context from stored documents:
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.store_doc(lm.get_wiki("Python"))
-        >>> lm.store_doc(lm.get_wiki("C++"))
+        >>> lm.store_doc(lm.get_wiki("C language"))
         >>> lm.store_doc(lm.get_wiki("Javascript"))
         >>> lm.store_doc(lm.get_wiki("Fortran"))
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
         'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
         
-        C, or c, is the third letter in the Latin alphabet, used in the modern English alphabet, the alphabets of other western European languages and others worldwide. Its name in English is cee (pronounced ), plural cees.
-        
-        a measure of the popularity of programming languages.'
+        often incorporating third-party libraries. All major web browsers have a dedicated JavaScript engine to execute the code on users\' devices. JavaScript is a high-level, often just-in-time compiled language that conforms to the ECMAScript standard. It has dynamic typing, prototype'
         ```
         
         ### Performance
         
         The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
         
         The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
```

### Comparing `languagemodels-0.4.0/languagemodels/__init__.py` & `languagemodels-0.5.0/languagemodels/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """Follow a single-turn instructional prompt
 
     :param prompt: Instructional prompt to follow
     :return: Completion returned from the language model
 
     Examples:
 
-    >>> do("Translate Spanish to English: Hola mundo!")
+    >>> do("Translate Spanish to English: Hola mundo!") #doctest: +SKIP
     'Hello world!'
 
     >>> do("Pick the sport from the list: baseball, texas, chemistry")
     'Baseball.'
 
     >>> do("Is the following positive or negative: I love Star Trek.")
     'Positive.'
```

### Comparing `languagemodels-0.4.0/languagemodels/embeddings.py` & `languagemodels-0.5.0/languagemodels/embeddings.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.4.0/languagemodels/inference.py` & `languagemodels-0.5.0/languagemodels/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         [input_tokens],
         target_prefix=[tokenizer.EncodeAsPieces(prefix)],
         repetition_penalty=repetition_penalty,
         max_decoding_length=max_tokens,
         sampling_temperature=temperature,
         sampling_topk=topk,
         suppress_sequences=suppress,
-        beam_size=2,
+        beam_size=1,
     )
 
     output_tokens = results[0].hypotheses[0]
 
     return tokenizer.DecodePieces(output_tokens)
```

### Comparing `languagemodels-0.4.0/languagemodels/models.py` & `languagemodels-0.5.0/languagemodels/models.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.4.0/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.5.0/languagemodels.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -64,15 +64,15 @@
         ```python
         >>> import languagemodels as lm
         
         >>> lm.do("Translate to English: Hola, mundo!")
         'Hello, world!'
         
         >>> lm.do("What is the capital of France?")
-        'paris'
+        'Paris.'
         ```
         
         ### Chat
         
         ```python
         >>> chat('''
         ...      System: Respond as a helpful assistant.
@@ -129,23 +129,21 @@
         
         This can also be used to get a blend of context from stored documents:
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.store_doc(lm.get_wiki("Python"))
-        >>> lm.store_doc(lm.get_wiki("C++"))
+        >>> lm.store_doc(lm.get_wiki("C language"))
         >>> lm.store_doc(lm.get_wiki("Javascript"))
         >>> lm.store_doc(lm.get_wiki("Fortran"))
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
         'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
         
-        C, or c, is the third letter in the Latin alphabet, used in the modern English alphabet, the alphabets of other western European languages and others worldwide. Its name in English is cee (pronounced ), plural cees.
-        
-        a measure of the popularity of programming languages.'
+        often incorporating third-party libraries. All major web browsers have a dedicated JavaScript engine to execute the code on users\' devices. JavaScript is a high-level, often just-in-time compiled language that conforms to the ECMAScript standard. It has dynamic typing, prototype'
         ```
         
         ### Performance
         
         The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
         
         The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
```

### Comparing `languagemodels-0.4.0/setup.py` & `languagemodels-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.4.0",
+    version="0.5.0",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

