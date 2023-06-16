# Comparing `tmp/vercel_llm_api-0.1.1-py3-none-any.whl.zip` & `tmp/vercel_llm_api-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 17943 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4639 b- defN 23-Jun-16 18:58 vercel_ai.py
--rw-r--r--  2.0 unx    35148 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6599 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      491 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/RECORD
-6 files, 46979 bytes uncompressed, 17053 bytes compressed:  63.7%
+Zip file size: 18446 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     5781 b- defN 23-Jun-16 22:02 vercel_ai.py
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7598 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      491 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/RECORD
+6 files, 49120 bytes uncompressed, 17556 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vercel_ai.py
 Comment: 
 
-Filename: vercel_llm_api-0.1.1.dist-info/LICENSE
+Filename: vercel_llm_api-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: vercel_llm_api-0.1.1.dist-info/METADATA
+Filename: vercel_llm_api-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: vercel_llm_api-0.1.1.dist-info/WHEEL
+Filename: vercel_llm_api-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: vercel_llm_api-0.1.1.dist-info/top_level.txt
+Filename: vercel_llm_api-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vercel_llm_api-0.1.1.dist-info/RECORD
+Filename: vercel_llm_api-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vercel_ai.py

```diff
@@ -2,28 +2,31 @@
 import logging
 import re
 import json
 import base64
 import quickjs
 import queue
 import threading
+import uuid
+import random
 from curl_cffi import requests
 
 logging.basicConfig()
 logger = logging.getLogger()
 
 class Client:
   base_url = "https://play.vercel.ai"
   token_url = base_url + "/openai.jpeg" #nice try vercel
   generate_url = base_url + "/api/prompt"
+  chat_url = base_url + "/api/generate"
 
   def __init__(self):
-    self.session = requests.Session(impersonate="chrome110")
+    self.session = requests.Session(impersonate="chrome107")
     self.headers = {
-      "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110 Safari/537.36",
+      "User-Agent": f"Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.{random.randint(0,9999)}.{random.randint(0,99)} Safari/537.36",
       "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
       "Accept-Encoding": "gzip, deflate, br",
       "Accept-Language": "en-US,en;q=0.5",
       "Te": "trailers",
       "Upgrade-Insecure-Requests": "1"
     }
     self.session.headers.update(self.headers)
@@ -41,31 +44,44 @@
     separator_regex = r'"\]\)<\/script><script>self\.__next_f\.push\(\[.,"'
 
     paths = re.findall(paths_regex, html)
     for i in range(len(paths)):
       paths[i] = re.sub(separator_regex, "", paths[i])
     paths = list(set(paths))
 
-    for path in paths:
-      script_url = f"{self.base_url}/_next/{path}"
-      logger.info(f"Downloading and parsing {script_url}...")
+    scripts = []
+    threads = []
 
+    logger.info(f"Downloading and parsing scripts...")
+    def download_thread(path):
+      script_url = f"{self.base_url}/_next/{path}"
       script = self.session.get(script_url).text
+      scripts.append(script)
+      
+    for path in paths:
+      thread = threading.Thread(target=download_thread, args=(path,), daemon=True)
+      thread.start()
+      threads.append(thread)
+    
+    for thread in threads:
+      thread.join()
+    
+    for script in scripts:
       models_regex = r'let .="\\n\\nHuman:\",r=(.+?),.='
       matches = re.findall(models_regex, script)
 
       if matches:
         models_str = matches[0]
         stop_sequences_regex = r'(?<=stopSequences:{value:\[)\D(?<!\])'
         models_str = re.sub(stop_sequences_regex, re.escape('"\\n\\nHuman:"'), models_str)
 
         context = quickjs.Context()
         json_str = context.eval(f"({models_str})").json()
         return json.loads(json_str)
-    
+
     return []
 
   def get_token(self):
     logger.info("Fetching token from "+self.token_url)
     b64 = self.session.get(self.token_url).text
     data = json.loads(base64.b64decode(b64))
 
@@ -86,69 +102,92 @@
   def get_default_params(self, model_id):
     model = self.models[model_id]
     defaults = {}
     for key, param in model["parameters"].items():
       defaults[key] = param["value"]
     return defaults
 
-  def generate(self, model_id, prompt, params={}):
-    logger.info(f"Sending to {model_id}: {prompt}")
-
-    token = self.get_token()
-    defaults = self.get_default_params(model_id)
-    payload = {**defaults, **params, **{
-      "prompt": prompt,
-      "model": model_id,
-    }}
-
-    headers = {**self.headers, **{
-      "Accept-Encoding": "gzip, deflate, br",
-      "Custom-Encoding": token,
-      "Host": "play.vercel.ai",
-      "Origin": "https://play.vercel.ai",
-      "Referrer": "https://play.vercel.ai",
-      "Sec-Fetch-Dest": "empty",
-      "Sec-Fetch-Mode": "cors",
-      "Sec-Fetch-Site": "same-origin",
-    }}
-
-    #bad streaming workaround cause the tls library doesn't support it
-    logger.info(f"Waiting for server response")
-
+  #bad streaming workaround cause the tls library doesn't support it
+  def stream_request(self, method, *args, **kwargs):
     chunks_queue = queue.Queue()
     error = None
     response = None
 
     def callback(data):
       chunks_queue.put(data.decode())
     def request_thread():
       nonlocal response, error
       try:
-        response = self.session.post(self.generate_url, json=payload, headers=headers, content_callback=callback)
+        response = self.session.post(*args, **kwargs, content_callback=callback)
         response.raise_for_status()
       except Exception as e:
         error = e
     
     thread = threading.Thread(target=request_thread, daemon=True)
     thread.start()
     
-    text = ""
-    index = 0
     while True:
       try:
-        chunk = chunks_queue.get(block=True, timeout=0.1)
+        chunk = chunks_queue.get(block=True, timeout=0.01)
       except queue.Empty:
         if error:
           raise error
         elif response:
           break
         else:
           continue
+      
+      yield chunk
+  
+  def get_headers(self):
+    token = self.get_token()
+
+    headers = {**self.headers, **{
+      "Accept-Encoding": "gzip, deflate, br",
+      "Custom-Encoding": token,
+      "Host": "play.vercel.ai",
+      "Origin": "https://play.vercel.ai",
+      "Referrer": "https://play.vercel.ai",
+      "Sec-Fetch-Dest": "empty",
+      "Sec-Fetch-Mode": "cors",
+      "Sec-Fetch-Site": "same-origin",
+    }}
+
+    return headers
 
+  def generate(self, model_id, prompt, params={}):
+    logger.info(f"Sending to {model_id}: {prompt}")
+
+    defaults = self.get_default_params(model_id)
+    payload = {**defaults, **params, **{
+      "prompt": prompt,
+      "model": model_id,
+    }}
+    headers = self.get_headers()
+
+    logger.info("Waiting for response")
+    text = ""
+    index = 0
+    for chunk in self.stream_request(self.session.post, self.generate_url, headers=headers, json=payload):
       text += chunk
       lines = text.split("\n")
 
       if len(lines) - 1 > index:
         new = lines[index:-1]
         for word in new:
           yield json.loads(word)
-        index = len(lines) - 1
+        index = len(lines) - 1
+  
+  def chat(self, model_id, messages, params={}):
+    logger.info(f"Sending to {model_id}: {len(messages)} messages")
+
+    defaults = self.get_default_params(model_id)
+    payload = {**defaults, **params, **{
+      "chatIndex": 0, 
+      "messages": messages,
+      "model": model_id,
+      "playgroundId": str(uuid.uuid4())
+    }}
+    headers = self.get_headers()
+    
+    logger.info("Waiting for response")
+    return self.stream_request(self.session.post, self.chat_url, headers=headers, json=payload)
```

## Comparing `vercel_llm_api-0.1.1.dist-info/LICENSE` & `vercel_llm_api-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vercel_llm_api-0.1.1.dist-info/METADATA` & `vercel_llm_api-0.2.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vercel-llm-api
-Version: 0.1.1
+Version: 0.2.0
 Summary: A reverse engineered API for the Vercel AI playground.
 Home-page: https://github.com/ading2210/vercel-llm-api
 Author: ading2210
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -24,24 +24,26 @@
 - [Features](#features)
 - [Limitations](#limitations)
 - [Installation](#installation)
 - [Documentation](#documentation)
   * [Using the Client](#using-the-client)
     + [Downloading the Available Models](#downloading-the-available-models)
     + [Generating Text](#generating-text)
+    + [Generating Chat Messages](#generating-chat-messages)
   * [Misc](#misc)
     + [Changing the Logging Level](#changing-the-logging-level)
 - [Copyright](#copyright)
   * [Copyright Notice](#copyright-notice)
 
 *Table of contents generated with [markdown-toc](http://ecotrust-canada.github.io/markdown-toc).*
 
 ## Features:
  - Download the available models
  - Generate text
+ - Generate chat messages
  - Set custom parameters
  - Stream the responses
 
 ## Limitations:
  - User-agent is hardcoded
  - No auth support
  - No proxy support
@@ -158,14 +160,34 @@
 ```python
 result = ""
 for chunk in client.generate("openai:gpt-3.5-turbo", "Summarize the GNU GPL v3"):
   result += chunk
 print(result)
 ```
 
+#### Generating Chat Messages:
+To generate chat messages, use the `client.chat` function, which accepts the following arguments:
+ - `model` - The ID of the model you want to use.
+ - `messages` - A list of messages. The format for this is identical to how you would use the official OpenAI API.
+ - `params = {}` - A dict of optional parameters. See the "Downloading the Available Models" section for how to find these.
+
+The function is a generator which returns the newly generated text as a string.
+
+```python
+messages = [
+  {"role": "system", "content": "You are a helpful assistant."},
+  {"role": "user", "content": "Who won the world series in 2020?"},
+  {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
+  {"role": "user", "content": "Where was it played?"}
+]
+for chunk in client.chat("openai:gpt-3.5-turbo", messages):
+  print(chunk, end="", flush=True)
+print()
+```
+
 ### Misc:
 
 #### Changing the Logging Level:
 If you want to show the debug messages, simply call `vercel_ai.logger.setLevel`.
 
 ```python
 import vercel_ai
```

