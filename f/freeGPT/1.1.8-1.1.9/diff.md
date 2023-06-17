# Comparing `tmp/freeGPT-1.1.8.tar.gz` & `tmp/freeGPT-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.1.8.tar", last modified: Mon Jun 12 19:28:35 2023, max compression
+gzip compressed data, was "freeGPT-1.1.9.tar", last modified: Sat Jun 17 19:34:37 2023, max compression
```

## Comparing `freeGPT-1.1.8.tar` & `freeGPT-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 19:28:35.920948 freeGPT-1.1.8/
--rw-rw-rw-   0        0        0    35149 2023-06-12 19:26:41.000000 freeGPT-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       96 2023-06-12 19:26:41.000000 freeGPT-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4211 2023-06-12 19:28:35.918949 freeGPT-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3080 2023-06-12 19:26:41.000000 freeGPT-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 19:28:35.881950 freeGPT-1.1.8/freeGPT/
--rw-rw-rw-   0        0        0     2319 2023-06-12 19:26:41.000000 freeGPT-1.1.8/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:28:35.910949 freeGPT-1.1.8/freeGPT/alpaca_7b/
--rw-rw-rw-   0        0        0     1545 2023-06-12 19:26:41.000000 freeGPT-1.1.8/freeGPT/alpaca_7b/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:28:35.912949 freeGPT-1.1.8/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5009 2023-06-12 19:26:41.000000 freeGPT-1.1.8/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:28:35.915948 freeGPT-1.1.8/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6759 2023-06-12 19:26:41.000000 freeGPT-1.1.8/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:28:35.908949 freeGPT-1.1.8/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     4211 2023-06-12 19:28:35.000000 freeGPT-1.1.8/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-12 19:28:35.000000 freeGPT-1.1.8/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 19:28:35.000000 freeGPT-1.1.8/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-12 19:28:35.000000 freeGPT-1.1.8/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 19:28:35.000000 freeGPT-1.1.8/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 19:28:35.920948 freeGPT-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1577 2023-06-12 19:26:41.000000 freeGPT-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.527489 freeGPT-1.1.9/
+-rw-rw-rw-   0        0        0    35149 2023-06-17 19:31:12.000000 freeGPT-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       96 2023-06-17 19:31:12.000000 freeGPT-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4247 2023-06-17 19:34:37.526492 freeGPT-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3110 2023-06-17 19:31:12.000000 freeGPT-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.372011 freeGPT-1.1.9/freeGPT/
+-rw-rw-rw-   0        0        0     2319 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.517521 freeGPT-1.1.9/freeGPT/alpaca_7b/
+-rw-rw-rw-   0        0        0     1590 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/alpaca_7b/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.521509 freeGPT-1.1.9/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5094 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.523502 freeGPT-1.1.9/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2467 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.509559 freeGPT-1.1.9/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4247 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 19:34:37.528485 freeGPT-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1533 2023-06-17 19:31:12.000000 freeGPT-1.1.9/setup.py
```

### Comparing `freeGPT-1.1.8/LICENSE` & `freeGPT-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.8/PKG-INFO` & `freeGPT-1.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.8
-Summary: freeGPT is a Python package that gives free access to GPT and more models.
+Version: 1.1.9
+Summary: freeGPT is a Python package that gives access to GPT and more models for free.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Project-URL: Discord, http://dsc.gg/ruu3fstudio
-Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,alpaca-7b,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
+Project-URL: Discord, https://dsc.gg/ruu3fstudio
+Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,model,free,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,36 +30,37 @@
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
 ***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
 
 ## Source:
-*Both GPT models have internet access.*
+*GPT-3 has internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
-| gpt3              | [you.com](https://you.com)                           |
-| gpt4              | [forefront.ai](https://chat.forefront.ai)            |
+| gpt3              | [you.com](https://you.com/)                          |
+| gpt4              | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/)|
 | alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
 
 ### TODO-List:
-- [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
-- [ ] Add a text to image generation model.
+- [ ] Add a image generation model.
 
 ## Support me:
-- Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
-- Star this repository :D
+- Star this repository! :D
+- Join my [Discord Server](https://discord.gg/NcQ26PrNDp):
+
+[![DiscordWidget](https://discordapp.com/api/guilds/1084505055476056184/widget.png?style=banner2)](https://discord.gg/NcQ26PrNDp)
 
 ## Discord bot:
 - Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
 - This bot has ALL the models in this repository available.
 - Its interactive, fast and overall easy to use.
 - And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
 
@@ -80,19 +81,18 @@
         print(f"🤖 > {str(e)}")
 ```
 #### GPT-4:
 ```python
 from freeGPT import gpt4
 
 while True:
-    token = gpt4.Account.create(logging=True)
     prompt = input("👦 > ")
     try:
-        resp = gpt4.Completion.create(prompt=prompt, token=token)
-        print(f"🤖 > {str(resp.text)}")
+        resp = gpt4.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp)}")
     except Exception as e:
         print(f"🤖 > {str(e)}")
 ```
 
 #### Alpaca-7b:
 ```python
 from freeGPT import alpaca_7b
```

### Comparing `freeGPT-1.1.8/README.md` & `freeGPT-1.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
 ***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
 
 ## Source:
-*Both GPT models have internet access.*
+*GPT-3 has internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
-| gpt3              | [you.com](https://you.com)                           |
-| gpt4              | [forefront.ai](https://chat.forefront.ai)            |
+| gpt3              | [you.com](https://you.com/)                          |
+| gpt4              | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/)|
 | alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
 
 ### TODO-List:
-- [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
-- [ ] Add a text to image generation model.
+- [ ] Add a image generation model.
 
 ## Support me:
-- Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
-- Star this repository :D
+- Star this repository! :D
+- Join my [Discord Server](https://discord.gg/NcQ26PrNDp):
+
+[![DiscordWidget](https://discordapp.com/api/guilds/1084505055476056184/widget.png?style=banner2)](https://discord.gg/NcQ26PrNDp)
 
 ## Discord bot:
 - Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
 - This bot has ALL the models in this repository available.
 - Its interactive, fast and overall easy to use.
 - And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
 
@@ -57,19 +58,18 @@
         print(f"🤖 > {str(e)}")
 ```
 #### GPT-4:
 ```python
 from freeGPT import gpt4
 
 while True:
-    token = gpt4.Account.create(logging=True)
     prompt = input("👦 > ")
     try:
-        resp = gpt4.Completion.create(prompt=prompt, token=token)
-        print(f"🤖 > {str(resp.text)}")
+        resp = gpt4.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp)}")
     except Exception as e:
         print(f"🤖 > {str(e)}")
 ```
 
 #### Alpaca-7b:
 ```python
 from freeGPT import alpaca_7b
```

### Comparing `freeGPT-1.1.8/freeGPT/__init__.py` & `freeGPT-1.1.9/freeGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.8/freeGPT/alpaca_7b/__init__.py` & `freeGPT-1.1.9/freeGPT/alpaca_7b/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,17 @@
             "Sec-Ch-Ua-Mobile": "?0",
             "Sec-Ch-Ua-Platform": "Windows",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "cross-site",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36",
         }
-        resp = requests.post(
-            "https://us-central1-arched-keyword-306918.cloudfunctions.net/run-inference-1",
-            headers=headers,
-            json={"prompt": prompt},
-        ).json()
         try:
-            return resp["completion"]
-        except KeyError:
+            resp = requests.post(
+                "https://us-central1-arched-keyword-306918.cloudfunctions.net/run-inference-1",
+                headers=headers,
+                json={"prompt": prompt},
+            ).json()
+        except requests.exceptions.RequestException:
             raise Exception("Unable to fetch the response.")
+
+        return resp["completion"]
```

### Comparing `freeGPT-1.1.8/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.9/freeGPT/gpt3/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import os, re, json
-
-try:
-    from tls_client import Session
-except ImportError:
-    os.system("pip install tls_client --no-cache-dir")
+import re, json
+import subprocess
 from uuid import uuid4
 from fake_useragent import UserAgent
 from typing import Optional, List
 
 
 class Completion:
     """A class that provides methods for creating completion requests."""
@@ -16,50 +12,56 @@
     def create(
         prompt: str,
         page: int = 1,
         count: int = 10,
         safe_search: str = "Off",
         on_shopping_page: bool = False,
         mkt: str = "",
-        response_filter: str = "WebPages,Translations,TimeZone,Computation,RelatedSearches",
+        response_filter: str = "WebPages, Translations, Computation, RelatedSearches",
         domain: str = "youchat",
-        query_trace_id: str = None,
-        chat: List[str] = None,
+        query_trace_id: Optional[str] = None,
+        chat: Optional[List[str]] = None,
         include_links: bool = False,
         detailed: bool = False,
         proxies: Optional[str] = None,
     ) -> dict:
         """
         Creates a completion request.
 
         Args:
             prompt (str): The prompt text for the completion.
             page (int, optional): The page number for pagination. Defaults to 1.
             count (int, optional): The number of results per page. Defaults to 10.
-            safe_search (str, optional): The safe search level. Defaults to 'Moderate'.
+            safe_search (str, optional): The safe search level. Defaults to 'Off'.
             on_shopping_page (bool, optional): Indicates if the completion is on a shopping page. Defaults to False.
             mkt (str, optional): The market for the completion. Defaults to ''.
             response_filter (str, optional): The filter for the response. Defaults to 'WebPages,Translations,TimeZone,Computation,RelatedSearches'.
             domain (str, optional): The domain for the completion. Defaults to 'youchat'.
             query_trace_id (str, optional): The trace ID for the query. Defaults to None.
             chat (list, optional): A list of chat messages. Defaults to None.
             include_links (bool, optional): Indicates if links should be included in the response. Defaults to False.
             detailed (bool, optional): Indicates if detailed results should be included in the response. Defaults to False.
-            proxy (str, optional): The proxy server to use. Defaults to None.
+            proxies (str, optional): The proxy server to use. Defaults to None.
 
         Returns:
             dict: The completion response as a dictionary.
 
         Raises:
             Exception: If unable to get the response.
         """
         if chat is None:
             chat = []
 
-        client = Session(client_identifier="chrome_108")
+        try:
+            import tls_client
+        except ImportError:
+            subprocess.run(["pip", "install", "tls_client", "--no-cache-dir"])
+            import tls_client
+
+        client = tls_client.Session(client_identifier="chrome_108")
         client.headers = Completion.__get_headers()
         client.proxies = proxies
 
         response = client.get(
             "https://you.com/api/streamingSearch",
             params={
                 "q": prompt,
@@ -117,17 +119,17 @@
             dict: The headers as a dictionary.
         """
         return {
             "authority": "you.com",
             "accept": "text/event-stream",
             "accept-language": "en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3",
             "cache-control": "no-cache",
-            "referer": "https://you.com/search?q=who+are+you&tbm=youchat",
+            "referer": "https://you.com/search?q=hi&tbm=youchat",
             "sec-ch-ua": '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
             "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Windows"',
+            "sec-ch-ua-platform": '"Linux"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
-            "cookie": f"safesearch_guest=Moderate; uuid_guest={str(uuid4())}",
+            "cookie": f"safesearch_guest=Off; uuid_guest={str(uuid4())}",
             "user-agent": UserAgent().random,
         }
```

### Comparing `freeGPT-1.1.8/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.9/freeGPT.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.8
-Summary: freeGPT is a Python package that gives free access to GPT and more models.
+Version: 1.1.9
+Summary: freeGPT is a Python package that gives access to GPT and more models for free.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Project-URL: Discord, http://dsc.gg/ruu3fstudio
-Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,alpaca-7b,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
+Project-URL: Discord, https://dsc.gg/ruu3fstudio
+Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,model,free,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,36 +30,37 @@
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
 ***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
 
 ## Source:
-*Both GPT models have internet access.*
+*GPT-3 has internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
-| gpt3              | [you.com](https://you.com)                           |
-| gpt4              | [forefront.ai](https://chat.forefront.ai)            |
+| gpt3              | [you.com](https://you.com/)                          |
+| gpt4              | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/)|
 | alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
 
 ### TODO-List:
-- [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
-- [ ] Add a text to image generation model.
+- [ ] Add a image generation model.
 
 ## Support me:
-- Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
-- Star this repository :D
+- Star this repository! :D
+- Join my [Discord Server](https://discord.gg/NcQ26PrNDp):
+
+[![DiscordWidget](https://discordapp.com/api/guilds/1084505055476056184/widget.png?style=banner2)](https://discord.gg/NcQ26PrNDp)
 
 ## Discord bot:
 - Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
 - This bot has ALL the models in this repository available.
 - Its interactive, fast and overall easy to use.
 - And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
 
@@ -80,19 +81,18 @@
         print(f"🤖 > {str(e)}")
 ```
 #### GPT-4:
 ```python
 from freeGPT import gpt4
 
 while True:
-    token = gpt4.Account.create(logging=True)
     prompt = input("👦 > ")
     try:
-        resp = gpt4.Completion.create(prompt=prompt, token=token)
-        print(f"🤖 > {str(resp.text)}")
+        resp = gpt4.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp)}")
     except Exception as e:
         print(f"🤖 > {str(e)}")
 ```
 
 #### Alpaca-7b:
 ```python
 from freeGPT import alpaca_7b
```

### Comparing `freeGPT-1.1.8/setup.py` & `freeGPT-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.8",
-    description="freeGPT is a Python package that gives free access to GPT and more models.",
+    version="1.1.9",
+    description="freeGPT is a Python package that gives access to GPT and more models for free.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
         "ai-models",
         "chatllama",
-        "alpaca-7b",
         "gpt4free",
         "freegpt",
         "chatgpt",
         "python",
         "alpaca",
         "openai",
+        "model",
+        "free",
         "gpt3",
         "gpt4",
         "gpt",
         "py",
         "ai",
     ],
     python_requires=">=3.6",
@@ -39,19 +40,16 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(),
     install_requires=[
-        "pydantic",
-        "pymailtm",
-        "curl_cffi",
         "requests",
         "fake-useragent",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
         "Issues": "https://github.com/Ruu3f/freeGPT/issues",
-        "Discord": "http://dsc.gg/ruu3fstudio",
+        "Discord": "https://dsc.gg/ruu3fstudio",
     },
 )
```

