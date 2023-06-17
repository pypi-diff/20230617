# Comparing `tmp/gpteasy-0.0.4.tar.gz` & `tmp/gpteasy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-0.0.4.tar", last modified: Sat Jun 17 09:11:53 2023, max compression
+gzip compressed data, was "gpteasy-1.0.1.tar", last modified: Sat Jun 17 13:37:38 2023, max compression
```

## Comparing `gpteasy-0.0.4.tar` & `gpteasy-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 09:11:53.758711 gpteasy-0.0.4/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-0.0.4/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 09:11:53.758383 gpteasy-0.0.4/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 09:11:45.000000 gpteasy-0.0.4/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 09:11:53.755452 gpteasy-0.0.4/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-0.0.4/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4289 2023-06-16 09:38:51.000000 gpteasy-0.0.4/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-0.0.4/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    12500 2023-06-17 08:13:14.000000 gpteasy-0.0.4/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1192 2023-06-16 09:38:41.000000 gpteasy-0.0.4/gpteasy/repl.py
--rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-0.0.4/gpteasy/settings.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 09:11:53.757880 gpteasy-0.0.4/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      296 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)       52 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1066 2023-06-17 09:11:45.000000 gpteasy-0.0.4/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 09:11:53.758804 gpteasy-0.0.4/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 13:37:38.532147 gpteasy-1.0.1/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.0.1/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 13:37:38.531856 gpteasy-1.0.1/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 13:37:30.000000 gpteasy-1.0.1/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 13:37:38.529192 gpteasy-1.0.1/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.0.1/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.0.1/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.0.1/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    12654 2023-06-17 13:35:36.000000 gpteasy-1.0.1/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.0.1/gpteasy/repl.py
+-rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-1.0.1/gpteasy/settings.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 13:37:38.531459 gpteasy-1.0.1/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      296 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)       52 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1052 2023-06-17 13:37:30.000000 gpteasy-1.0.1/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 13:37:38.532229 gpteasy-1.0.1/setup.cfg
```

### Comparing `gpteasy-0.0.4/LICENSE` & `gpteasy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.4/PKG-INFO` & `gpteasy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 0.0.4
+Version: 1.0.1
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 0.0.4
+Current version: 1.0.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-0.0.4/README.md` & `gpteasy-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 0.0.4
+Current version: 1.0.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-0.0.4/gpteasy/commands.py` & `gpteasy-1.0.1/gpteasy/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
         self.add_command('quit', self.handle_quit, ":quit - Quit the program")
         self.add_command('load', self.handle_load, ":load name - loads the saved conversation with the specified name")
         self.add_command('save', self.handle_save, ":save name - saves the conversation under the specified name")
 
         self.add_command('input', self.handle_input, ":input filename - loads an input from the specified file")
         self.add_command('model', self.handle_gpt_attribute, ":model gpt-4 - Sets the AI model")
         self.add_command('max_tokens', self.handle_gpt_attribute,
-                        ":max_tokens 800 - The maximum number of tokens to generate in the completion")
+                         ":max_tokens 800 - The maximum number of tokens to generate in the completion")
         self.add_command('temperature', self.handle_gpt_attribute, ":temperature 0.9 - What sampling temperature to " +
                                                                    "use, between 0 and 2")
         self.add_command('n', self.handle_gpt_attribute, ":n 1 - Specifies the number answers given")
         self.add_command('stop', self.handle_gpt_attribute, ':stop ["\\n", " Human:", " AI:"] - Up to 4 sequences ' +
                                                             'where the API will stop generating further tokens')
         self.add_command('bye', self.handle_bye, ":bye - quits but saves the conversation first")
         self.add_command('help', self.handle_help, ":help - shows this help message")
         for attr in dir(self.gpt):
-            if attr[0] != '_' and not attr in self.commands:
+            if attr[0] != '_' and attr not in self.commands:
                 self.add_command(attr, self.handle_gpt_attribute, "")
 
     def add_command(self, command, handler, description):
         self.commands[command] = (handler, description)
 
     def handle_quit(self):
         return False
@@ -64,29 +64,32 @@
         self.gpt.chat('bye')
         return False
 
     def handle_maxmessages(self, param):
         self.gpt.message_memory = int(param)
 
     def handle_gpt_attribute(self, attr, value):
+        if not value:
+            value = getattr(self.gpt, attr)
+            color_print(f"{attr} is currently {value}\n", color=SYSTEM_COLOR)
+            return True
         try:
             value = eval(value)
         except (SyntaxError, NameError):
             pass  # Treat param as a string
         setattr(self.gpt, attr, value)
         color_print(f"{attr} set to {value}\n", color=SYSTEM_COLOR)
         return True
 
     def handle_help(self):
         for (_, description) in self.commands.values():
             if description:
                 color_print(description, color=SYSTEM_COLOR)
         return True
 
-
     def handle_command(self, command: str):
         # Commands can be things like
         # :load filename
         # :save [filename]
         # :quit
         # :max_tokens=1000
         # :temperature=0.8
```

### Comparing `gpteasy-0.0.4/gpteasy/display.py` & `gpteasy-1.0.1/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.4/gpteasy/gpt.py` & `gpteasy-1.0.1/gpteasy/gpt.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 from openai.error import APIConnectionError, APIError, RateLimitError
 
 from .display import print_message, color_print, SYSTEM_COLOR, ERROR_COLOR
 from .settings import get_settings
 
 BASE_SYSTEM = "You are ChatGPT, a large language model trained by OpenAI."
 
+
 class GptFunction:
-    def __init__(self, name:str, description:str, callback=None):
+    def __init__(self, name: str, description: str, callback=None):
         self.name = name
         self.description = description
         self.parameters = {}  # name: (type, description, required, enum)
         self.callback = callback
 
-    def add_param(self, name:str, type:str, description:str=None, required:bool=False, enum:list=None):
+    def add_param(self, name: str, type: str, description: str = None, required: bool = False, enum: list = None):
         self.parameters[name] = (type, description, required, enum)
 
     def __call__(self, **kwargs):
         return self.callback(**kwargs)
 
     def in_completion_format(self) -> dict:
         """{
@@ -70,20 +71,19 @@
 class GPT:
     def __init__(self):
         # Authentication
         if not os.getenv("OPENAI_API_KEY"):
             load_dotenv()  # Load the .env file into the environment
         openai.api_key = os.getenv("OPENAI_API_KEY")
         if not openai.api_key:
-            print_message("No OpenAI API key found. Create one at https://platform.openai.com/account/api-keys and " +\
-                          "set it in the .env file like OPENAI_API_KEY=here_comes_your_key.", color=ERROR_COLOR)
-        #openai.organization = os.getenv("OPENAI_ORGANIZATION")
-        self.functions = {} # Callable GPT functions
+            color_print("No OpenAI API key found. Create one at https://platform.openai.com/account/api-keys and " +
+                        "set it in the .env file like OPENAI_API_KEY=here_comes_your_key.", color=ERROR_COLOR)
+        self.functions = {}  # Callable GPT functions
 
-        self.system = lambda: BASE_SYSTEM
+        self.system_message = BASE_SYSTEM
 
         # Model parameters
         self.model = "gpt-4"  # "gpt-3.5-turbo"
 
         # The maximum number of tokens to generate in the completion.
         # Defaults to 16
         # The token count of your prompt plus max_tokens cannot exceed the model's context length.
@@ -130,14 +130,17 @@
         self.name = ''  # Name of the current conversation
         self.save_dir = Path(__file__).resolve().parent / 'saves'
         self.save_dir.mkdir(exist_ok=True)
 
         self.message_memory = 20  # Number of messages to remember. Limits token usage.
         self.messages = []
 
+    def system(self):  # This function can be overwritten by child classes to make the system message dynamic
+        return self.system_message
+
     def reset(self):
         self.name = ''
         self.messages = []
 
     def get_messages(self):
         result = [{'role': 'system', 'content': self.system()}]
         for m in self.messages[-self.message_memory:]:
@@ -145,18 +148,18 @@
             if m.name:  # Function name in case the model called a function
                 message['name'] = m.name
             if m.content:  # Function result in case the model called a function
                 message['content'] = m.content
             result.append(message)
         return result
 
-    def add_function(self, function:GptFunction):
+    def add_function(self, function: GptFunction):
         self.functions[function.name] = function
 
-    def remove_funtion(self, name:str):
+    def remove_funtion(self, name: str):
         del self.functions[name]
 
     def get_functions(self):
         return [f.in_completion_format() for f in self.functions.values()] if self.functions else None
 
     def chat(self, prompt, add_to_messages=True):
 
@@ -173,15 +176,15 @@
                         top_p=self.top_p,
                         frequency_penalty=self.frequency_penalty,
                         presence_penalty=self.presence_penalty,
                         stop=self.stop,
                         functions=self.get_functions(),
                         function_call="auto" if self.functions else None  # auto is default, but we'll be explicit
                     )
-                else: # Version for models without the possibility to use functions
+                else:  # Version for models without the possibility to use functions
                     completion = openai.ChatCompletion.create(
                         model=self.model,
                         messages=self.get_messages(),
                         temperature=self.temperature,
                         max_tokens=self.max_tokens,
                         n=self.n,
                         top_p=self.top_p,
@@ -196,29 +199,27 @@
             except APIError as e:
                 color_print("API error", color=SYSTEM_COLOR)
                 return e
             except RateLimitError as e:
                 color_print(f"{get_settings()['model']} is overloaded", color=SYSTEM_COLOR)
                 return e
 
-
         if self.messages and not self.name:
             self.name = re.sub(r'\W+', '', self.messages[0].text).replace(' ', '_')[:20]
         self.messages += [Message('user', prompt)]
 
         completion = chat_completion_request()
 
         while completion["choices"][0]['finish_reason'] == 'function_call':
             message = completion["choices"][0]["message"]
             function_call = message["function_call"]
             function_to_call = self.functions[function_call["name"]]
             kwargs = json.loads(function_call["arguments"])
             function_response = function_to_call(**kwargs)
 
-            #self.messages += [Message('assistant', completion)]
             self.messages += [Message('function', name=function_call["name"], content=function_response)]
 
             # get a new response from GPT where it can see the function response
             completion = chat_completion_request()
 
         message = Message('assistant', completion)
         if add_to_messages:
@@ -236,40 +237,41 @@
         with open((self.save_dir / self.name).with_suffix('.txt'), "w") as f:
             f.write(f"system: {self.system()}\n")
             for message in self.messages:
                 f.write(f"{message.role}: {message.text}\n")
 
     def load(self, name):
         def save_message(msg):
-            if msg['role'] == 'system':
-                self.system = lambda: msg['content']
+            if msg.role == 'system':
+                self.system_message = msg.text
             else:
                 self.messages += [msg]
 
         self.messages = []
         self.name = name
         if not name.endswith('.txt'):
             name += '.txt'
         filename = self.save_dir / name
         if not os.path.isfile(filename):
             color_print(f"New conversation:  {filename}", color=SYSTEM_COLOR)
             return
         with open(filename, "r") as f:
             message = Message()
+            assert not message
             for line in f.readlines():
                 line = line[:-1]
                 try:
-                    role, content = line.split(': ', 1)
+                    role, text = line.split(': ', 1)
                 except ValueError:
                     message.text += '\n' + line
                     continue
-                if role in ['system', 'user', 'assistant']:
+                if role in ['system', 'user', 'assistant', 'function']:
                     if message:
                         save_message(message)
-                    message = {'role': role, 'content': content}
+                    message = Message(role=role, text_or_completion=text)
                 else:
                     message.text += '\n' + line
             if message:
                 save_message(message)
         print_message(Message('system', self.system()))
         for message in self.messages:
             print_message(message)
@@ -297,7 +299,10 @@
         try:
             return json.loads(self.raw_completion['choices'][0]['message']['content'])
         except json.decoder.JSONDecodeError:
             return {'type': 'other', 'response': self.raw_completion['choices'][0]['message']['content']}
 
     def tokens(self):
         return self.raw_completion['usage']['total_tokens']
+
+    def __bool__(self):
+        return bool(self.raw_completion) or bool(self.text)
```

### Comparing `gpteasy-0.0.4/gpteasy/repl.py` & `gpteasy-1.0.1/gpteasy/repl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Class to handle the interactivity to the model and setting model system parameters """
 from .display import print_message
 from .gpt import GPT
 
 
 class Repl:
-    def __init__(self, gpt: GPT, command_handler:callable):
+    def __init__(self, gpt: GPT, command_handler: callable):
         self.gpt = gpt
         self.command_handler = command_handler
         self.show_token_count = False
 
     def run(self, first_prompt=''):
         while True:
             if first_prompt:  # If we have a first prompt, use it instead of asking the user first
```

### Comparing `gpteasy-0.0.4/gpteasy/settings.py` & `gpteasy-1.0.1/gpteasy/settings.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.4/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.0.1/gpteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 0.0.4
+Version: 1.0.1
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 0.0.4
+Current version: 1.0.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-0.0.4/pyproject.toml` & `gpteasy-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "0.0.4"
+version = "1.0.1"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -24,9 +24,9 @@
 
 [project.urls]
 Homepage = "https://github.com/hpharmsen/gpteasy"
 
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["gpteasy"]  # package names should match these glob patterns (["*"] by default)
-exclude = ["test_gpteasy"]  # exclude packages matching these glob patterns (empty by default)
+exclude = []  # exclude packages matching these glob patterns (empty by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
```

