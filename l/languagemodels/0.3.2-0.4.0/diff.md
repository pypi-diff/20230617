# Comparing `tmp/languagemodels-0.3.2.tar.gz` & `tmp/languagemodels-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.3.2.tar", last modified: Thu Jun  8 01:45:08 2023, max compression
+gzip compressed data, was "languagemodels-0.4.0.tar", last modified: Sat Jun 17 13:08:58 2023, max compression
```

## Comparing `languagemodels-0.3.2.tar` & `languagemodels-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-08 01:45:08.791806 languagemodels-0.3.2/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8872 2023-06-08 01:45:08.791806 languagemodels-0.3.2/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-08 01:45:08.791806 languagemodels-0.3.2/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10565 2023-06-08 01:43:41.000000 languagemodels-0.3.2/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4580 2023-06-08 01:33:35.000000 languagemodels-0.3.2/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7860 2023-06-08 01:43:41.000000 languagemodels-0.3.2/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-08 01:45:08.791806 languagemodels-0.3.2/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8872 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       53 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-08 01:45:08.791806 languagemodels-0.3.2/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      792 2023-06-08 01:44:57.000000 languagemodels-0.3.2/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 13:08:58.337436 languagemodels-0.4.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8928 2023-06-17 13:08:58.333436 languagemodels-0.4.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 13:08:58.333436 languagemodels-0.4.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10516 2023-06-17 13:06:52.000000 languagemodels-0.4.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4577 2023-06-17 01:38:19.000000 languagemodels-0.4.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7105 2023-06-17 12:18:09.000000 languagemodels-0.4.0/languagemodels/inference.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4078 2023-06-17 01:38:19.000000 languagemodels-0.4.0/languagemodels/models.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 13:08:58.333436 languagemodels-0.4.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8928 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      306 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       61 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-17 13:08:58.000000 languagemodels-0.4.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-17 13:08:58.337436 languagemodels-0.4.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      800 2023-06-17 13:08:46.000000 languagemodels-0.4.0/setup.py
```

### Comparing `languagemodels-0.3.2/PKG-INFO` & `languagemodels-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.3.2
+Version: 0.4.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -41,19 +41,14 @@
         >>> import languagemodels as lm
         >>> lm.do("What color is the sky?")
         'The color of the sky is blue.'
         ```
         
         This will require downloading a significant amount of data (~250MB) on the first run. Models will be cached for later use and subsequent calls should be quick.
         
-        Model Performance
-        -----------------
-        
-        The underlying models used by this package were selected as the best in their size class. These models are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
-        
         Example Usage
         -------------
         
         Here are some usage examples as Python REPL sessions. This should work in the REPL, notebooks, or in traditional scripts and applications.
         
         ### Text Completions
         
@@ -92,18 +87,18 @@
         ### External Retrieval
         
         Helper functions are provided to retrieve text from external sources that can be used to augment prompt context.
         
         ```python
         >>> import languagemodels as lm
         
-        >>> lm.fetch_wiki('Chemistry')
+        >>> lm.get_wiki('Chemistry')
         'Chemistry is the scientific study...
         
-        >>> lm.fetch_weather(41.8, -87.6)
+        >>> lm.get_weather(41.8, -87.6)
         'Partly cloudy with a chance of rain...
         
         >>> lm.get_date()
         'Friday, May 12, 2023 at 09:27AM'
         ```
         
         Here's an example showing how this can be used (compare to previous chat example):
@@ -133,37 +128,49 @@
         ```
         
         This can also be used to get a blend of context from stored documents:
         
         ```python
         >>> import languagemodels as lm
         
-        >>> lm.store_doc(lm.fetch_wiki("Python"))
-        >>> lm.store_doc(lm.fetch_wiki("C++"))
-        >>> lm.store_doc(lm.fetch_wiki("Javascript"))
-        >>> lm.store_doc(lm.fetch_wiki("Fortran"))
+        >>> lm.store_doc(lm.get_wiki("Python"))
+        >>> lm.store_doc(lm.get_wiki("C++"))
+        >>> lm.store_doc(lm.get_wiki("Javascript"))
+        >>> lm.store_doc(lm.get_wiki("Fortran"))
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
         'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
         
         C, or c, is the third letter in the Latin alphabet, used in the modern English alphabet, the alphabets of other western European languages and others worldwide. Its name in English is cee (pronounced ), plural cees.
         
         a measure of the popularity of programming languages.'
         ```
         
+        ### Performance
+        
+        The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
+        
+        The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
+        
+        ```python
+        >>> import languagemodels as lm
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'You have 8 apples.'
+        >>> lm.set_max_ram('4gb')
+        4.0
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'I have 2 apples left.'
+        ```
+        
         [Full documentation](https://languagemodels.netlify.app/)
         
         Advanced Usage
         --------------
         
         This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face. For integrating language models in more complex ways, [LangChain](https://github.com/hwchase17/langchain) or [guidance](https://github.com/microsoft/guidance) may be helpful.
         
-        ### Large models
-        
-        The default model used for inference is around 250M parameters. There is a larger model that can be used if you don't mind things working a little more slowly. It can be enabled by setting the `LANGUAGEMODELS_SIZE` environment variable to `large`. This model isn't large by modern standards and should still work quickly in most environments (but not the lowest tier repl.it instance).
-        
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
         - CLI Chatbot (see examples/chat.py)
         - Streamlit chatbot (see examples/streamlitchat.py)
```

### Comparing `languagemodels-0.3.2/languagemodels/__init__.py` & `languagemodels-0.4.0/languagemodels/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,18 @@
 import requests
 import datetime
 import json
 
+from languagemodels.models import set_max_ram
 from languagemodels.inference import generate_instruct, parse_chat, list_tokens
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
 
 
-def print_tokens(prompt: str) -> None:
-    """Prints a list of tokens in a prompt
-
-    This function is provided for exploratory purposes only. It may return
-    different tokens than the underlying model and may not match the
-    tokenization of any backend API being used.
-
-    :param prompt: Prompt to use as input to tokenizer
-    :return: Nothing
-
-    Examples:
-
-    >>> print_tokens("Hello world")
-    ' Hello' (token 8774)
-    ' world' (token 296)
-
-    >>> print_tokens("Hola mundo")
-    ' Hol' (token 5838)
-    'a' (token 9)
-    ' mun' (token 13844)
-    'd' (token 26)
-    'o' (token 32)
-    """
-
-    tokens = list_tokens(prompt)
-
-    for token in tokens:
-        print(f"'{token[0].replace('▁',' ')}' (token {token[1]})")
-
-
-def count_tokens(prompt: str) -> None:
-    """Counts tokens in a prompt
-
-    This function is provided for exploratory purposes only. It may return
-    slightly different counts than the underlying model and may not match the
-    tokenization of any backend API being used.
-
-    :param prompt: Prompt to use as input to tokenizer
-    :return: Nothing
-
-    Examples:
-
-    >>> count_tokens("Hello world")
-    2
-
-    >>> count_tokens("Hola mundo")
-    5
-    """
-
-    return len(list_tokens(prompt))
-
-
 def complete(prompt: str) -> str:
     """Provide one completion for a given open-ended prompt
 
     :param prompt: Prompt to use as input to the model
     :return: Completion returned from the language model
 
     Examples:
@@ -96,21 +45,29 @@
     :return: Completion returned from the language model
 
     Examples:
 
     >>> do("Translate Spanish to English: Hola mundo!")
     'Hello world!'
 
-    >>> do("Pick the sport: baseball, texas, chemistry")
+    >>> do("Pick the sport from the list: baseball, texas, chemistry")
     'Baseball.'
 
     >>> do("Is the following positive or negative: I love Star Trek.")
     'Positive.'
     """
-    return generate_instruct(prompt, max_tokens=200)
+    result = generate_instruct(prompt, max_tokens=200, topk=1)
+
+    if len(result.split()) == 1:
+        result = result.title()
+
+        if result[-1] not in (".", "!", "?"):
+            result = result + "."
+
+    return result
 
 
 def chat(prompt: str) -> str:
     """Get new message from chat-optimized language model
 
     The `prompt` for this model is provided as a series of messages as a single
     plain-text string. Several special tokens are used to delineate chat
@@ -137,14 +94,16 @@
     ```
 
     The completion from the language model is returned.
 
     :param message: Prompt using formatting described above
     :return: Completion returned from the language model
 
+    Examples:
+
     >>> chat('''
     ...      System: Respond as a helpful assistant. It is 5:15pm.
     ...
     ...      User: What time is it?
     ...
     ...      Assistant:
     ...      ''')
@@ -163,18 +122,18 @@
     # Suppress all user messages to avoid repeating them
     suppress += [m["content"] for m in messages if m["role"] == "user"]
 
     system_msgs = [m for m in messages if m["role"] == "system"]
     assistant_msgs = [m for m in messages if m["role"] == "assistant"]
     user_msgs = [m for m in messages if m["role"] == "user"]
 
+    # The current model is tuned on instructions and tends to get
+    # lost if it sees too many questions
     # Use only the most recent user and assistant message for context
     # Keep all system messages
-    # The current model is really tuned on instructions and tends to get
-    # lost if it sees too many questions
     messages = system_msgs + assistant_msgs[-1:] + user_msgs[-1:]
 
     rolemap = {
         "system": "System",
         "user": "Question",
         "assistant": "Assistant",
     }
@@ -209,18 +168,20 @@
     It may not always be a correct or meaningful answer, but it will never be
     an arbitrary hallucination.
 
     :param question: A question to answer using knowledge from context
     :param context: Knowledge used to answer the question
     :return: Answer to the question.
 
+    Examples:
+
     >>> context = "There is a green ball and a red box"
     >>> extract_answer("What color is the ball?", context) #doctest: +SKIP
     'green'
-    >>> extract_answer("Who created Python?", fetch_wiki('Python')) #doctest: +SKIP
+    >>> extract_answer("Who created Python?", get_wiki('Python')) #doctest: +SKIP
     'Guido van Rossum'
     """
 
     return generate_instruct(f"{context}\n\n{question}")
 
 
 def classify(doc: str, label1: str, label2: str) -> str:
@@ -228,45 +189,55 @@
 
     :param doc: A plain text input document to classify
     :param label1: The first label to classify against
     :param label2: The second label to classify against
     :return: The closest matching class. The return value will always be
     `label1` or `label2`
 
-    >>> classify("I love you!","positive","negative") #doctest: +SKIP
+    Examples:
+
+    >>> classify("I love you!","positive","negative")
     'positive'
-    >>> classify("That book was fine.","positive","negative") #doctest: +SKIP
+    >>> classify("That book was good.","positive","negative")
     'positive'
-    >>> classify("That movie was terrible.","positive","negative") #doctest: +SKIP
+    >>> classify("That movie was terrible.","positive","negative")
     'negative'
-    >>> classify("The submarine is diving", "ocean", "space") #doctest: +SKIP
+    >>> classify("The submarine is diving", "ocean", "land")
     'ocean'
     """
 
-    return generate_instruct(f"Classify as {label1} or {label2}: {doc}", max_tokens=5)
+    result = generate_instruct(
+        f"Classify as {label1} or {label2}: {doc}\n\nClassification:", max_tokens=5
+    )
+
+    return result.lower().rstrip(".")
 
 
 def store_doc(doc: str) -> None:
     """Store document for later retrieval
 
     :param doc: A plain text document to store.
 
+    Examples:
+
     >>> store_doc("The sky is blue.")
     """
     docs.store(doc)
 
 
 def load_doc(query: str) -> str:
     """Load a matching document
 
     A single document that best matches `query` will be returned.
 
     :param query: Query to compare to stored documents
     :return: Content of the closest matching document
 
+    Examples:
+
     >>> store_doc("Paris is in France.")
     >>> store_doc("The sky is blue.")
     >>> load_doc("Where is Paris?")
     'Paris is in France.'
     """
     return docs.get_match(query)
 
@@ -276,37 +247,41 @@
 
     A string representing the most relevant content from all stored documents
     will be returned. This may be a blend of chunks from multiple documents.
 
     :param query: Query to compare to stored documents
     :return: Up to 128 tokens of context
 
+    Examples:
+
     >>> store_doc("Paris is in France.")
     >>> store_doc("Paris is nice.")
     >>> store_doc("The sky is blue.")
     >>> get_doc_context("Where is Paris?")
     'Paris is in France.\\n\\nParis is nice.'
     """
     return docs.get_context(query)
 
 
-def fetch_wiki(topic: str) -> str:
+def get_wiki(topic: str) -> str:
     """
     Return Wikipedia summary for a topic
 
     This function ignores the complexity of disambiguation pages and simply
     returns the first result that is not a disambiguation page
 
     :param topic: Topic to search for on Wikipedia
     :return: Text content of the lead section of the most popular matching article
 
-    >>> fetch_wiki('Python')
+    Examples:
+
+    >>> get_wiki('Python')
     'Python is a high-level...'
 
-    >>> fetch_wiki('Chemistry')
+    >>> get_wiki('Chemistry')
     'Chemistry is the scientific study...'
     """
 
     url = "https://api.wikimedia.org/core/v1/wikipedia/en/search/title"
     response = requests.get(url, params={"q": topic, "limit": 5})
     response = json.loads(response.text)
 
@@ -322,25 +297,27 @@
 
         summary = first["extract"]
         return summary
     else:
         return "No matching wiki page found."
 
 
-def fetch_weather(latitude, longitude):
+def get_weather(latitude, longitude):
     """Fetch the current weather for a supplied longitude and latitude
 
     Weather is provided by the US government and this function only supports
     locations in the United States.
 
     :param latitude: Latitude value representing this location
     :param longitude: Longitude value representing this location
     :return: Plain text description of the current weather forecast
 
-    >>> fetch_weather(41.8, -87.6) # doctest: +SKIP
+    Examples:
+
+    >>> get_weather(41.8, -87.6) # doctest: +SKIP
     'Scattered showers and thunderstorms before 1pm with a high of 73.'
     """
 
     res = requests.get(f"https://api.weather.gov/points/{latitude},{longitude}")
     points = json.loads(res.text)
     forecast_url = points["properties"]["forecast"]
 
@@ -357,7 +334,51 @@
     >>> get_date() # doctest: +SKIP
     'Friday, May 12, 2023 at 09:27AM'
     """
 
     now = datetime.datetime.now()
 
     return now.strftime("%A, %B %d, %Y at %I:%M%p")
+
+
+def print_tokens(prompt: str) -> None:
+    """Prints a list of tokens in a prompt
+
+    :param prompt: Prompt to use as input to tokenizer
+    :return: Nothing
+
+    Examples:
+
+    >>> print_tokens("Hello world")
+    ' Hello' (token 8774)
+    ' world' (token 296)
+
+    >>> print_tokens("Hola mundo")
+    ' Hol' (token 5838)
+    'a' (token 9)
+    ' mun' (token 13844)
+    'd' (token 26)
+    'o' (token 32)
+    """
+
+    tokens = list_tokens(prompt)
+
+    for token in tokens:
+        print(f"'{token[0].replace('▁',' ')}' (token {token[1]})")
+
+
+def count_tokens(prompt: str) -> None:
+    """Counts tokens in a prompt
+
+    :param prompt: Prompt to use as input to tokenizer
+    :return: Nothing
+
+    Examples:
+
+    >>> count_tokens("Hello world")
+    2
+
+    >>> count_tokens("Hola mundo")
+    5
+    """
+
+    return len(list_tokens(prompt))
```

### Comparing `languagemodels-0.3.2/languagemodels/embeddings.py` & `languagemodels-0.4.0/languagemodels/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from languagemodels.inference import get_model
+from languagemodels.models import get_model
 
 
 def cosine_similarity(a, b):
     dot_product = sum(ai * bi for ai, bi in zip(a, b))
     magnitude_a = sum(ai ** 2 for ai in a) ** 0.5
     magnitude_b = sum(bi ** 2 for bi in b) ** 0.5
     return dot_product / (magnitude_a * magnitude_b)
```

### Comparing `languagemodels-0.3.2/languagemodels/inference.py` & `languagemodels-0.4.0/languagemodels/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import requests
-import os
-from huggingface_hub import hf_hub_download
-import ctranslate2
 import re
-import sentencepiece
-from tokenizers import Tokenizer
+import os
+
+from languagemodels.models import get_model
 
 
 class InferenceException(Exception):
     pass
 
 
-modelcache = {}
-
-
 def list_tokens(prompt):
     """Generates a list of tokens for a supplied prompt
 
     >>> list_tokens("Hello, world!")
     [('▁Hello', 8774), (',', 6), ('▁world', 296), ('!', 55)]
     """
     tokenizer, _ = get_model("instruct")
@@ -77,90 +72,78 @@
 
     try:
         return resp["choices"][0]["text"]
     except KeyError:
         raise InferenceException(f"OpenAI error: {resp}")
 
 
-def get_model(model_type):
-    if model_type == "instruct":
-        model_name = "jncraton/LaMini-Flan-T5-248M-ct2-int8"
-    elif model_type == "embedding":
-        model_name = "jncraton/all-MiniLM-L6-v2-ct2-int8"
-    else:
-        raise InferenceException(f"Invalid model: {model_type}")
+def chat_oa(engine, prompt, max_tokens=200, temperature=0):
+    """Generates a single text response for a prompt using OpenAI
 
-    if os.environ.get("LANGUAGEMODELS_SIZE") == "small":
-        model_name = model_name.replace("base", "small")
-        model_name = model_name.replace("248M", "77M")
-
-    if os.environ.get("LANGUAGEMODELS_SIZE") == "large":
-        model_name = model_name.replace("base", "large")
-        model_name = model_name.replace("248M", "783M")
-
-    if model_name not in modelcache:
-        hf_hub_download(model_name, "config.json")
-        model_path = hf_hub_download(model_name, "model.bin")
-        model_base_path = model_path[:-10]
-
-        if "minilm" in model_name.lower():
-            hf_hub_download(model_name, "vocabulary.txt")
-            tokenizer = Tokenizer.from_pretrained(model_name)
-            tokenizer.no_padding()
-            tokenizer.no_truncation()
-            modelcache[model_name] = (
-                tokenizer,
-                ctranslate2.Encoder(model_base_path),
-            )
-        else:
-            hf_hub_download(model_name, "shared_vocabulary.txt")
-            tokenizer_path = hf_hub_download(model_name, "spiece.model")
-
-            tokenizer = sentencepiece.SentencePieceProcessor()
-            tokenizer.Load(tokenizer_path)
-
-            modelcache[model_name] = (
-                tokenizer,
-                ctranslate2.Translator(model_base_path),
-            )
+    The server and API key are provided as environment variables:
+
+    LANGUAGEMODELS_OA_KEY is the API key
+    """
+    apikey = os.environ.get("LANGUAGEMODELS_OA_KEY")
+
+    response = requests.post(
+        "https://api.openai.com/v1/chat/completions",
+        headers={
+            "Authorization": f"Bearer {apikey}",
+            "Content-Type": "application/json",
+        },
+        json={
+            "model": engine,
+            "messages": [{"role": "user", "content": prompt}],
+            "max_tokens": max_tokens,
+            "temperature": temperature,
+        },
+    )
+    resp = response.json()
 
-    return modelcache[model_name]
+    try:
+        return resp["choices"][0]["message"]["content"]
+    except KeyError:
+        raise InferenceException(f"OpenAI error: {resp}")
 
 
 def generate_instruct(
     prompt,
     max_tokens=200,
     temperature=0.1,
+    topk=1,
     repetition_penalty=1.2,
     prefix="",
     suppress=[],
 ):
     """Generates one completion for a prompt using an instruction-tuned model
 
     This may use a local model, or it may make an API call to an external
     model if API keys are available.
     """
-    if os.environ.get("ts_key") or os.environ.get("ts_server"):
-        return generate_ts("flan_t5_xxl_q4", prompt, max_tokens)
+    if os.environ.get("LANGUAGEMODELS_TS_KEY") or os.environ.get(
+        "LANGUAGEMODELS_TS_SERVER"
+    ):
+        return generate_ts("flan_t5_xxl_q4", prompt, max_tokens).strip()
 
-    if os.environ.get("oa_key"):
-        return generate_oa("text-babbage-001", prompt, max_tokens)
+    if os.environ.get("LANGUAGEMODELS_OA_KEY"):
+        return chat_oa("gpt-3.5-turbo", prompt, max_tokens).strip()
 
     tokenizer, model = get_model("instruct")
 
     suppress = [tokenizer.EncodeAsPieces(s) for s in suppress]
 
     input_tokens = tokenizer.EncodeAsPieces(prompt) + ["</s>"]
     results = model.translate_batch(
         [input_tokens],
         target_prefix=[tokenizer.EncodeAsPieces(prefix)],
         repetition_penalty=repetition_penalty,
         max_decoding_length=max_tokens,
         sampling_temperature=temperature,
-        sampling_topk=40,
+        sampling_topk=topk,
         suppress_sequences=suppress,
         beam_size=2,
     )
 
     output_tokens = results[0].hypotheses[0]
 
     return tokenizer.DecodePieces(output_tokens)
```

### Comparing `languagemodels-0.3.2/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.4.0/languagemodels.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.3.2
+Version: 0.4.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -41,19 +41,14 @@
         >>> import languagemodels as lm
         >>> lm.do("What color is the sky?")
         'The color of the sky is blue.'
         ```
         
         This will require downloading a significant amount of data (~250MB) on the first run. Models will be cached for later use and subsequent calls should be quick.
         
-        Model Performance
-        -----------------
-        
-        The underlying models used by this package were selected as the best in their size class. These models are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
-        
         Example Usage
         -------------
         
         Here are some usage examples as Python REPL sessions. This should work in the REPL, notebooks, or in traditional scripts and applications.
         
         ### Text Completions
         
@@ -92,18 +87,18 @@
         ### External Retrieval
         
         Helper functions are provided to retrieve text from external sources that can be used to augment prompt context.
         
         ```python
         >>> import languagemodels as lm
         
-        >>> lm.fetch_wiki('Chemistry')
+        >>> lm.get_wiki('Chemistry')
         'Chemistry is the scientific study...
         
-        >>> lm.fetch_weather(41.8, -87.6)
+        >>> lm.get_weather(41.8, -87.6)
         'Partly cloudy with a chance of rain...
         
         >>> lm.get_date()
         'Friday, May 12, 2023 at 09:27AM'
         ```
         
         Here's an example showing how this can be used (compare to previous chat example):
@@ -133,37 +128,49 @@
         ```
         
         This can also be used to get a blend of context from stored documents:
         
         ```python
         >>> import languagemodels as lm
         
-        >>> lm.store_doc(lm.fetch_wiki("Python"))
-        >>> lm.store_doc(lm.fetch_wiki("C++"))
-        >>> lm.store_doc(lm.fetch_wiki("Javascript"))
-        >>> lm.store_doc(lm.fetch_wiki("Fortran"))
+        >>> lm.store_doc(lm.get_wiki("Python"))
+        >>> lm.store_doc(lm.get_wiki("C++"))
+        >>> lm.store_doc(lm.get_wiki("Javascript"))
+        >>> lm.store_doc(lm.get_wiki("Fortran"))
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
         'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
         
         C, or c, is the third letter in the Latin alphabet, used in the modern English alphabet, the alphabets of other western European languages and others worldwide. Its name in English is cee (pronounced ), plural cees.
         
         a measure of the popularity of programming languages.'
         ```
         
+        ### Performance
+        
+        The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
+        
+        The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
+        
+        ```python
+        >>> import languagemodels as lm
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'You have 8 apples.'
+        >>> lm.set_max_ram('4gb')
+        4.0
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'I have 2 apples left.'
+        ```
+        
         [Full documentation](https://languagemodels.netlify.app/)
         
         Advanced Usage
         --------------
         
         This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face. For integrating language models in more complex ways, [LangChain](https://github.com/hwchase17/langchain) or [guidance](https://github.com/microsoft/guidance) may be helpful.
         
-        ### Large models
-        
-        The default model used for inference is around 250M parameters. There is a larger model that can be used if you don't mind things working a little more slowly. It can be enabled by setting the `LANGUAGEMODELS_SIZE` environment variable to `large`. This model isn't large by modern standards and should still work quickly in most environments (but not the lowest tier repl.it instance).
-        
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
         - CLI Chatbot (see examples/chat.py)
         - Streamlit chatbot (see examples/streamlitchat.py)
```

### Comparing `languagemodels-0.3.2/setup.py` & `languagemodels-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.3.2",
+    version="0.4.0",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
@@ -18,11 +18,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     install_requires=[
         "sentencepiece",
         "huggingface_hub",
-        "ctranslate2",
+        "ctranslate2>=3.15.0",
         "tokenizers",
        ],
 )
```

