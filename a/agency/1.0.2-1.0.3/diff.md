# Comparing `tmp/agency-1.0.2.tar.gz` & `tmp/agency-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.0.2.tar", max compression
+gzip compressed data, was "agency-1.0.3.tar", max compression
```

## Comparing `agency-1.0.2.tar` & `agency-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 agency-1.0.2/LICENSE
--rw-r--r--   0        0        0    25690 2023-06-15 19:41:44.309956 agency-1.0.2/README.md
--rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 agency-1.0.2/agency/__init__.py
--rw-r--r--   0        0        0    10347 2023-06-15 19:59:59.343889 agency-1.0.2/agency/agent.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 agency-1.0.2/agency/agents/__init__.py
--rw-r--r--   0        0        0     2791 2023-06-12 21:57:53.079991 agency-1.0.2/agency/agents/chattyai.py
--rw-r--r--   0        0        0     2202 2023-06-12 20:36:46.457242 agency-1.0.2/agency/agents/host.py
--rw-r--r--   0        0        0     2729 2023-06-14 13:13:25.937150 agency-1.0.2/agency/agents/openai_completion_agent.py
--rw-r--r--   0        0        0     7797 2023-06-14 13:13:25.937407 agency-1.0.2/agency/agents/openai_function_agent.py
--rw-r--r--   0        0        0     1519 2023-06-12 20:36:46.457203 agency-1.0.2/agency/agents/prompt_methods.py
--rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 agency-1.0.2/agency/schema.py
--rwxr-xr-x   0        0        0     3261 2023-06-14 13:13:25.937665 agency-1.0.2/agency/space.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 agency-1.0.2/agency/spaces/__init__.py
--rw-r--r--   0        0        0     6646 2023-06-14 13:13:25.937925 agency-1.0.2/agency/spaces/templates/index.html
--rw-r--r--   0        0        0     4027 2023-06-14 13:13:25.938200 agency-1.0.2/agency/spaces/web_app.py
--rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 agency-1.0.2/agency/util.py
--rw-r--r--   0        0        0      557 2023-06-15 20:21:51.900010 agency-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    26529 1970-01-01 00:00:00.000000 agency-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-17 00:45:31.301980 agency-1.0.3/LICENSE
+-rw-r--r--   0        0        0    24997 2023-06-17 00:45:31.301980 agency-1.0.3/README.md
+-rw-r--r--   0        0        0       40 2023-06-17 00:45:31.301980 agency-1.0.3/agency/__init__.py
+-rw-r--r--   0        0        0    10347 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agent.py
+-rw-r--r--   0        0        0        0 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/__init__.py
+-rw-r--r--   0        0        0     2791 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/chattyai.py
+-rw-r--r--   0        0        0     2202 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/host.py
+-rw-r--r--   0        0        0     2729 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/openai_completion_agent.py
+-rw-r--r--   0        0        0     7797 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/openai_function_agent.py
+-rw-r--r--   0        0        0     1519 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/prompt_methods.py
+-rw-r--r--   0        0        0      801 2023-06-17 00:45:31.301980 agency-1.0.3/agency/schema.py
+-rwxr-xr-x   0        0        0     3261 2023-06-17 00:45:31.301980 agency-1.0.3/agency/space.py
+-rw-r--r--   0        0        0        0 2023-06-17 00:45:31.301980 agency-1.0.3/agency/spaces/__init__.py
+-rw-r--r--   0        0        0     6646 2023-06-17 00:45:31.301980 agency-1.0.3/agency/spaces/templates/index.html
+-rw-r--r--   0        0        0     4027 2023-06-17 00:45:31.301980 agency-1.0.3/agency/spaces/web_app.py
+-rw-r--r--   0        0        0     4280 2023-06-17 00:45:31.301980 agency-1.0.3/agency/util.py
+-rw-r--r--   0        0        0      554 2023-06-17 00:45:34.749985 agency-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    25833 1970-01-01 00:00:00.000000 agency-1.0.3/PKG-INFO
```

### Comparing `agency-1.0.2/LICENSE` & `agency-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/README.md` & `agency-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,32 @@
+Metadata-Version: 2.1
+Name: agency
+Version: 1.0.3
+Summary: A fast and minimal actor model framework for building agent-integrated systems
+License: GPL-3.0
+Author: Daniel Rodriguez
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Flask-SocketIO (>=5.3,<6.0)
+Requires-Dist: asyncio (>=3.4,<4.0)
+Requires-Dist: colorama (>=0.4,<0.5)
+Requires-Dist: eventlet (>=0.33,<0.34)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pydantic (>=1.8,<2.0)
+Requires-Dist: torch (>=2.0,<3.0)
+Requires-Dist: transformers (>=4.29,<5.0)
+Description-Content-Type: text/markdown
+
 # `agency`
 
-A fast and minimal foundation for unifying human, AI, and other computing
-systems, in python
+A fast and minimal actor model framework for building agent-integrated systems
 
 
 ## What is `agency`?
 
 `agency` defines a common communication and action framework for integrating
 AI agents, humans, and traditional computing systems.
 
@@ -54,17 +75,16 @@
 of the `Agent` class. This includes all humans, software, and AI-driven agents.
 
 The `Agent` class is a base class similar to "Object" in many object-oriented
 languages. All agents may expose "actions" that other agents can discover and
 invoke at run time. Actions also specify an access policy, allowing you to
 monitor and control actions to ensure safety.
 
-A `Space` is also an `Agent` and is used to group multiple agents together.
-
-A space can be thought of as both a collection of agents and a "router" for
+A `Space` is also an `Agent` and is used to group multiple agents together. A
+space can be thought of as both a collection of agents and a facilitator for
 their communication. An agent cannot communicate with others until it is first
 added to a space.
 
 Spaces may be nested, allowing for namespacing and hierarchical organization of
 the agents in your application.
 
 To summarize, the two classes of `Agent` and `Space` together create a simple
@@ -72,17 +92,62 @@
 systems, in a way that is intended for all to equally understand and use.
 
 Let's walk through a thorough example to see how this works in practice.
 
 
 # Example Walkthrough
 
-> Please note that the example classes used in this walkthrough are implemented
-for you to explore and try out, but should be considered "proof of concept"
-quality at this time.
+> Please note that the example agent classes used in this walkthrough are
+implemented for you to explore and try out, but should be considered "proof of
+concept" quality at this time.
+
+The following snippet is the full resulting implementation (minus imports) of
+the example walkthrough that you can try out on your own, including two OpenAI
+agent examples and the HuggingFace based `ChattyAI`. Note that `Space.run()`
+starts a thread, so we simply keep the application alive with a while loop.
+
+```python
+# demo.py
+
+if __name__ == '__main__':
+
+    space = Space("DemoSpace")
+
+    space.add(
+        WebApp("WebApp",
+            demo_user_id="Dan", # hardcoded for simplicity
+            port='8080'))
+
+    space.add(
+        ChattyAI("Chatty",
+            model="EleutherAI/gpt-neo-125m"))
+
+    space.add(
+        Host("Host"))
+
+    space.add(
+        OpenAIFunctionAgent("FunctionAI",
+            model="gpt-3.5-turbo-16k",
+            openai_api_key=os.getenv("OPENAI_API_KEY"),
+            # user_id determines the "user" role in the OpenAI chat
+            user_id="Dan.WebApp.DemoSpace"))
+
+    space.add(
+        OpenAICompletionAgent("CompletionAI",
+            model="text-davinci-003",
+            openai_api_key=os.getenv("OPENAI_API_KEY")))
+
+    space.run()
+
+    print("pop!")
+
+    # keep alive
+    while True:
+        time.sleep(1)
+```
 
 
 ## Creating a `Space`
 
 Let's start by instantiating a demo space.
 
 ```python
@@ -156,17 +221,17 @@
     }
 })
 ```
 
 This is a simple implementation that demonstrates the basic idea of how to
 invoke an action on another agent.
 
-When an agent receives a message, it invokes the action method specified in by
-the `"action"` field of the message, passing the `"args"` to the action method
-as keyword arguments.
+When an agent receives a message, it invokes the action method specified by the
+`"action"` field of the message, passing the `"args"` to the action method as
+keyword arguments.
 
 So here we see that Chatty is invoking the `say` action on the sender of the
 original message, passing the response as the `"content"` argument.
 
 
 ## The Common Message Schema
 
@@ -293,17 +358,14 @@
 user may expose to others.
 
 Using the `asyncio` library you'll see that we simply forward messages as-is to
 the `React` frontend, and allow the client code to handle rendering and parsing
 of input as actions back to the `Flask` application, which forwards them to
 their intended receiver in the space.
 
-This way, we allow individual web users to appear as individual agents to others
-in the space.
-
 
 ## Namespacing and Adding the Web Application
 
 Now that we've defined our new `WebApp` class, we can add it to `DemoSpace`
 with:
 
 ```python
@@ -326,14 +388,17 @@
 
 Users of the web application, as they log in or out, may be added dynamically
 under the `"WebApp"` namespace allowing them to be addressed with a fully
 qualified `id` of, for example:
 
 - `"Dan.WebApp.DemoSpace"`.
 
+This way, we allow individual web users to appear as individual agents to others
+in the space.
+
 _(Note that login/out functionality is not implemented as of this writing.)_
 
 
 ## Adding OS Access with the `Host` class
 
 At this point, we have a system where human users of the web application can
 chat with `ChattyAI`, using just a single action called `"say"` that both
@@ -346,16 +411,16 @@
 space.add(Host("Host"))
 ```
 
 The `Host` class allows access to the host operating system where the python
 application is running. It exposes actions such as `read_file` and
 `shell_command` which allow other agents to interact with the host.
 
-This class is a good example of one with potentially dangerous actions that need
-to be accessed with care. You'll notice that all the methods in the `Host` class
+This class is a good example of one with potentially dangerous actions that must
+be accessed with care. You'll notice that all the methods in the `Host` class
 have been given the access policy:
 
 ```python
 @access_policy(ACCESS_REQUESTED)
 ```
 
 By declaring this access policy, all actions on the host will require a
@@ -406,22 +471,14 @@
         "to": "Host.DemoSpace",
         "action": "list_files",
         "thoughts": "List files in a directory",
         "args": {
           "directory_path": "str"
         }
     },
-    {
-        "to": "ChattyAI.DemoSpace",
-        "action": "say",
-        "thoughts": "Use this action to say something to Chatty",
-        "args": {
-          "content": "str"
-        }
-    },
     ...
 ]
 ```
 
 Notice that each action lists the fully qualified `id` of the agent in the
 `"to"` field, the docstring of the action's method in the `"thoughts"` field,
 and each argument along with its type in the `"args"` field.
@@ -433,20 +490,20 @@
 /list_files to:Host.DemoSpace directory_path:/app
 ```
 
 This will send the `list_files` action to the `Host` agent who will (after being
 granted permission) return the results back to `"Dan.WebApp.DemoSpace"`
 rendering it to the web user interface as a message.
 
-Note the use of the fully qualified `id` of `Host.DemoSpace` used with the `to:`
-field.
-
 
 ## Broadcast vs Point-to-Point Messaging
 
+Note the use of the fully qualified `id` of `Host.DemoSpace` used with the `to:`
+field.
+
 If we omit the `to:Host.DemoSpace` portion of the command above, the message
 will be broadcast, and any agents who implement a `list_files` action will
 respond.
 
 This is also how the `/help` command works. If you want to request help from
 just a single agent you can use something like:
 
@@ -488,77 +545,33 @@
 to the chat API. Since the chat API is limited to a predefined set of roles, we
 need to indicate which is the main "user".
 
 For an implementation that uses a plain text completion API, see
 [`OpenAICompletionAgent`](./agency/agents/openai_completion_agent.py).
 
 
-## Complete Demo Implementation
-
-The following is the full implementation (minus imports) of the above
-walkthrough that you can try out on your own, including both OpenAI agent
-examples and the HuggingFace based "Chatty". Note that `Space.run()` starts a
-thread, so we simply keep the application alive with a while loop.
-
-```python
-# demo.py
-
-if __name__ == '__main__':
-
-    space = Space("DemoSpace") 
-
-    space.add(
-        WebApp("WebApp",
-            demo_user_id="Dan", # hardcoded for simplicity
-            port='8080'))
+## Running the Example
 
-    space.add(
-        ChattyAI("Chatty",
-            model="EleutherAI/gpt-neo-125m"))
-
-    space.add(
-        Host("Host"))
-
-    space.add(
-        OpenAIFunctionAgent("FunctionAI",
-            model="gpt-3.5-turbo-16k",
-            openai_api_key=os.getenv("OPENAI_API_KEY"),
-            # user_id determines the "user" role in the OpenAI chat
-            user_id="Dan.WebApp.DemoSpace"))
-
-    space.add(
-        OpenAICompletionAgent("CompletionAI",
-            model="text-davinci-003",
-            openai_api_key=os.getenv("OPENAI_API_KEY")))
-
-    space.run()
-
-    print("pop!")
-
-    # keep alive
-    while True:
-        time.sleep(1)
-```
-
-If you run the above python script, after a short boot time you can visit the
-web app at `http://localhost:8080` and you should see a simple chat interface.
+If you run the python script provided at the beginning of this walkthrough,
+after a short boot time you can visit the web app at `http://localhost:8080` and
+you should see a simple chat interface.
 
 The following is a screenshot of a conversation that showcases all the agents
 intelligently interacting and following orders.
 
 Note that my messages are broadcasted in the below conversation, which explains
 why all three respond to each message. There is an obvious difference in
 quality, of course.
 
 I also demonstrate the results of rejecting an action and directing an agent to
 use a different approach.
 
 After I explained my rejection of the `read_file` action (which happened behind
 the scenes on the terminal), "FunctionAI" appropriately used the `shell_command`
-action with `wc -l Dockerfile`. The Dockerfile indeed has 73 lines.
+action with `wc -l Dockerfile`. The Dockerfile indeed had 73 lines.
 
 CompletionAI used that command on the first try. Anecdotally as of this writing,
 `CompletionAI` seems to be more accurate, even though it is using the text
 completion API vs the function calling feature of the chat API. This may be due
 to the implementation or issues arising from the translation into roles
 discussed elsewhere.
 
@@ -655,33 +668,34 @@
 So, `agency` is a more general framework intended to support agent development
 and to ultimately enable agents to safely integrate with anything, in any way
 imaginable.
 
 ## What are some known limitations or issues?
 
 * It's a new project, so keep that in mind in terms of completeness, but see
-the plans below for where this is heading. Core functionality is pretty
-well tested at the moment.
+  [the issues page](https://github.com/operand/agency/issues) for what is
+  currently planned. Core functionality is pretty well tested at the moment.
 
 * This library makes use of threads for each individual agent. Multithreading
-is limited by python's GIL, meaning if you run a CPU bound model other agents
-will have to wait for their "turn". This goes for anything else you might define
-as an "agent", if it is CPU heavy it will block other agents. Note that I/O does
-not block, so networked backends or services will execute in parallel.  Other
-forms of multiprocessing to avoid the GIL may eventually be considered.
+  is limited by python's GIL, meaning if you run a CPU bound model other agents
+  will have to wait for their "turn". This goes for anything else you might
+  define as an "agent", if it is CPU heavy it will block other agents. Note that
+  I/O does not block, so networked backends or services will execute in
+  parallel.
+
+  Other forms of multiprocessing to avoid the GIL will be considered.
 
 * This API does NOT assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
-  of representing many things uniquely and independently.
-
-  This is a core feature of `agency`: that all things are treated the same and
-  may be interacted with through common means.
+  of representing many things uniquely and independently. This is a core feature
+  of `agency`: that all things are treated the same and may be interacted with
+  through common means.
 
   The lack of roles introduces some challenges in integrating with role based
   APIs. See the implementation of
   [`OpenAIFunctionAgent`](./agency/agents/openai_function_agent.py) for an
   example.
 
 * There is not much by way of storage support. That is mostly left up to you and
@@ -691,17 +705,14 @@
   APIs may be considered in the future.
 
 
 # Contributing
 
 Please do!
 
-If you have any questions, suggestions, or problems, please open an
-[issue](https://github.com/operand/agency/issues).
-
 
 ## Development Installation
 
 ```bash
 git clone git@github.com:operand/agency.git
 cd agency
 poetry install
@@ -724,38 +735,28 @@
 human, artificial, and other computing systems together, with the following
 priorities.
 
 
 ## Priorities
 - **Speed**:
   Performance is always a concern. If it's not performant, it's not practical.
-  Currently the limitations of python multi-threading are a bottleneck.
+  Currently the limitations of python multi-threading are a bottleneck and a
+  priority to address.
 - **Access Control and Safety**:
   An effective access control solution for agent-integrated systems is
   fundamental to ensure safety. I believe I've included a sane first step at
   such a pattern, but further development will be a focus of this project.
 - **Compatibility and Usability**:
   In general, I believe this is a fair start in defining a set of patterns for
   creating agent systems. I hope to ensure the API is kept small, and
   compatible with a wide variety of use cases.
 - **Documentation**:
   I hope to ensure documentation is kept organized, clear, and accurate. This
   readme serves as a start.
 
 
 ## Planned Work
-- Add web app multimodal i/o examples
-  - image
-  - audio
-  - video
-- Add multimodal model integration example
-- Add message broker/networking support (RabbitMQ)
-- Add integration example for [mlc-llm](https://github.com/mlc-ai/mlc-llm)
-- Add integration example for [gorilla](https://github.com/ShishirPatil/gorilla)
-- Add integration example for LangChain
-- Add model training example
-- Consider alternative multiprocessing approaches
-- Consider adding a storage API
-- Consider prior work on distributed access control
-- Add docker assets to encourage using it
-- [_feel free to make
-suggestions_](https://github.com/operand/agency/issues)
+
+[Please see the issues page.](https://github.com/operand/agency/issues)
+
+If you have any suggestions or otherwise, feel free to add an issue!
+
```

### Comparing `agency-1.0.2/agency/agent.py` & `agency-1.0.3/agency/agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/agents/chattyai.py` & `agency-1.0.3/agency/agents/chattyai.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/agents/host.py` & `agency-1.0.3/agency/agents/host.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/agents/openai_completion_agent.py` & `agency-1.0.3/agency/agents/openai_completion_agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/agents/openai_function_agent.py` & `agency-1.0.3/agency/agents/openai_function_agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/agents/prompt_methods.py` & `agency-1.0.3/agency/agents/prompt_methods.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/schema.py` & `agency-1.0.3/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/space.py` & `agency-1.0.3/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/spaces/templates/index.html` & `agency-1.0.3/agency/spaces/templates/index.html`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/spaces/web_app.py` & `agency-1.0.3/agency/spaces/web_app.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/agency/util.py` & `agency-1.0.3/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.2/pyproject.toml` & `agency-1.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "agency"
-version = "1.0.2"
-description = "A fast and minimal foundation for unifying human, AI, and other computing systems"
+version = "1.0.3"
+description = "A fast and minimal actor model framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncio = "^3.4"
```

### Comparing `agency-1.0.2/PKG-INFO` & `agency-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,10 @@
-Metadata-Version: 2.1
-Name: agency
-Version: 1.0.2
-Summary: A fast and minimal foundation for unifying human, AI, and other computing systems
-License: GPL-3.0
-Author: Daniel Rodriguez
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Flask-SocketIO (>=5.3,<6.0)
-Requires-Dist: asyncio (>=3.4,<4.0)
-Requires-Dist: colorama (>=0.4,<0.5)
-Requires-Dist: eventlet (>=0.33,<0.34)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (>=1.8,<2.0)
-Requires-Dist: torch (>=2.0,<3.0)
-Requires-Dist: transformers (>=4.29,<5.0)
-Description-Content-Type: text/markdown
-
 # `agency`
 
-A fast and minimal foundation for unifying human, AI, and other computing
-systems, in python
+A fast and minimal actor model framework for building agent-integrated systems
 
 
 ## What is `agency`?
 
 `agency` defines a common communication and action framework for integrating
 AI agents, humans, and traditional computing systems.
 
@@ -76,17 +53,16 @@
 of the `Agent` class. This includes all humans, software, and AI-driven agents.
 
 The `Agent` class is a base class similar to "Object" in many object-oriented
 languages. All agents may expose "actions" that other agents can discover and
 invoke at run time. Actions also specify an access policy, allowing you to
 monitor and control actions to ensure safety.
 
-A `Space` is also an `Agent` and is used to group multiple agents together.
-
-A space can be thought of as both a collection of agents and a "router" for
+A `Space` is also an `Agent` and is used to group multiple agents together. A
+space can be thought of as both a collection of agents and a facilitator for
 their communication. An agent cannot communicate with others until it is first
 added to a space.
 
 Spaces may be nested, allowing for namespacing and hierarchical organization of
 the agents in your application.
 
 To summarize, the two classes of `Agent` and `Space` together create a simple
@@ -94,17 +70,62 @@
 systems, in a way that is intended for all to equally understand and use.
 
 Let's walk through a thorough example to see how this works in practice.
 
 
 # Example Walkthrough
 
-> Please note that the example classes used in this walkthrough are implemented
-for you to explore and try out, but should be considered "proof of concept"
-quality at this time.
+> Please note that the example agent classes used in this walkthrough are
+implemented for you to explore and try out, but should be considered "proof of
+concept" quality at this time.
+
+The following snippet is the full resulting implementation (minus imports) of
+the example walkthrough that you can try out on your own, including two OpenAI
+agent examples and the HuggingFace based `ChattyAI`. Note that `Space.run()`
+starts a thread, so we simply keep the application alive with a while loop.
+
+```python
+# demo.py
+
+if __name__ == '__main__':
+
+    space = Space("DemoSpace")
+
+    space.add(
+        WebApp("WebApp",
+            demo_user_id="Dan", # hardcoded for simplicity
+            port='8080'))
+
+    space.add(
+        ChattyAI("Chatty",
+            model="EleutherAI/gpt-neo-125m"))
+
+    space.add(
+        Host("Host"))
+
+    space.add(
+        OpenAIFunctionAgent("FunctionAI",
+            model="gpt-3.5-turbo-16k",
+            openai_api_key=os.getenv("OPENAI_API_KEY"),
+            # user_id determines the "user" role in the OpenAI chat
+            user_id="Dan.WebApp.DemoSpace"))
+
+    space.add(
+        OpenAICompletionAgent("CompletionAI",
+            model="text-davinci-003",
+            openai_api_key=os.getenv("OPENAI_API_KEY")))
+
+    space.run()
+
+    print("pop!")
+
+    # keep alive
+    while True:
+        time.sleep(1)
+```
 
 
 ## Creating a `Space`
 
 Let's start by instantiating a demo space.
 
 ```python
@@ -178,17 +199,17 @@
     }
 })
 ```
 
 This is a simple implementation that demonstrates the basic idea of how to
 invoke an action on another agent.
 
-When an agent receives a message, it invokes the action method specified in by
-the `"action"` field of the message, passing the `"args"` to the action method
-as keyword arguments.
+When an agent receives a message, it invokes the action method specified by the
+`"action"` field of the message, passing the `"args"` to the action method as
+keyword arguments.
 
 So here we see that Chatty is invoking the `say` action on the sender of the
 original message, passing the response as the `"content"` argument.
 
 
 ## The Common Message Schema
 
@@ -315,17 +336,14 @@
 user may expose to others.
 
 Using the `asyncio` library you'll see that we simply forward messages as-is to
 the `React` frontend, and allow the client code to handle rendering and parsing
 of input as actions back to the `Flask` application, which forwards them to
 their intended receiver in the space.
 
-This way, we allow individual web users to appear as individual agents to others
-in the space.
-
 
 ## Namespacing and Adding the Web Application
 
 Now that we've defined our new `WebApp` class, we can add it to `DemoSpace`
 with:
 
 ```python
@@ -348,14 +366,17 @@
 
 Users of the web application, as they log in or out, may be added dynamically
 under the `"WebApp"` namespace allowing them to be addressed with a fully
 qualified `id` of, for example:
 
 - `"Dan.WebApp.DemoSpace"`.
 
+This way, we allow individual web users to appear as individual agents to others
+in the space.
+
 _(Note that login/out functionality is not implemented as of this writing.)_
 
 
 ## Adding OS Access with the `Host` class
 
 At this point, we have a system where human users of the web application can
 chat with `ChattyAI`, using just a single action called `"say"` that both
@@ -368,16 +389,16 @@
 space.add(Host("Host"))
 ```
 
 The `Host` class allows access to the host operating system where the python
 application is running. It exposes actions such as `read_file` and
 `shell_command` which allow other agents to interact with the host.
 
-This class is a good example of one with potentially dangerous actions that need
-to be accessed with care. You'll notice that all the methods in the `Host` class
+This class is a good example of one with potentially dangerous actions that must
+be accessed with care. You'll notice that all the methods in the `Host` class
 have been given the access policy:
 
 ```python
 @access_policy(ACCESS_REQUESTED)
 ```
 
 By declaring this access policy, all actions on the host will require a
@@ -428,22 +449,14 @@
         "to": "Host.DemoSpace",
         "action": "list_files",
         "thoughts": "List files in a directory",
         "args": {
           "directory_path": "str"
         }
     },
-    {
-        "to": "ChattyAI.DemoSpace",
-        "action": "say",
-        "thoughts": "Use this action to say something to Chatty",
-        "args": {
-          "content": "str"
-        }
-    },
     ...
 ]
 ```
 
 Notice that each action lists the fully qualified `id` of the agent in the
 `"to"` field, the docstring of the action's method in the `"thoughts"` field,
 and each argument along with its type in the `"args"` field.
@@ -455,20 +468,20 @@
 /list_files to:Host.DemoSpace directory_path:/app
 ```
 
 This will send the `list_files` action to the `Host` agent who will (after being
 granted permission) return the results back to `"Dan.WebApp.DemoSpace"`
 rendering it to the web user interface as a message.
 
-Note the use of the fully qualified `id` of `Host.DemoSpace` used with the `to:`
-field.
-
 
 ## Broadcast vs Point-to-Point Messaging
 
+Note the use of the fully qualified `id` of `Host.DemoSpace` used with the `to:`
+field.
+
 If we omit the `to:Host.DemoSpace` portion of the command above, the message
 will be broadcast, and any agents who implement a `list_files` action will
 respond.
 
 This is also how the `/help` command works. If you want to request help from
 just a single agent you can use something like:
 
@@ -510,77 +523,33 @@
 to the chat API. Since the chat API is limited to a predefined set of roles, we
 need to indicate which is the main "user".
 
 For an implementation that uses a plain text completion API, see
 [`OpenAICompletionAgent`](./agency/agents/openai_completion_agent.py).
 
 
-## Complete Demo Implementation
-
-The following is the full implementation (minus imports) of the above
-walkthrough that you can try out on your own, including both OpenAI agent
-examples and the HuggingFace based "Chatty". Note that `Space.run()` starts a
-thread, so we simply keep the application alive with a while loop.
-
-```python
-# demo.py
-
-if __name__ == '__main__':
-
-    space = Space("DemoSpace") 
-
-    space.add(
-        WebApp("WebApp",
-            demo_user_id="Dan", # hardcoded for simplicity
-            port='8080'))
-
-    space.add(
-        ChattyAI("Chatty",
-            model="EleutherAI/gpt-neo-125m"))
-
-    space.add(
-        Host("Host"))
-
-    space.add(
-        OpenAIFunctionAgent("FunctionAI",
-            model="gpt-3.5-turbo-16k",
-            openai_api_key=os.getenv("OPENAI_API_KEY"),
-            # user_id determines the "user" role in the OpenAI chat
-            user_id="Dan.WebApp.DemoSpace"))
-
-    space.add(
-        OpenAICompletionAgent("CompletionAI",
-            model="text-davinci-003",
-            openai_api_key=os.getenv("OPENAI_API_KEY")))
+## Running the Example
 
-    space.run()
-
-    print("pop!")
-
-    # keep alive
-    while True:
-        time.sleep(1)
-```
-
-If you run the above python script, after a short boot time you can visit the
-web app at `http://localhost:8080` and you should see a simple chat interface.
+If you run the python script provided at the beginning of this walkthrough,
+after a short boot time you can visit the web app at `http://localhost:8080` and
+you should see a simple chat interface.
 
 The following is a screenshot of a conversation that showcases all the agents
 intelligently interacting and following orders.
 
 Note that my messages are broadcasted in the below conversation, which explains
 why all three respond to each message. There is an obvious difference in
 quality, of course.
 
 I also demonstrate the results of rejecting an action and directing an agent to
 use a different approach.
 
 After I explained my rejection of the `read_file` action (which happened behind
 the scenes on the terminal), "FunctionAI" appropriately used the `shell_command`
-action with `wc -l Dockerfile`. The Dockerfile indeed has 73 lines.
+action with `wc -l Dockerfile`. The Dockerfile indeed had 73 lines.
 
 CompletionAI used that command on the first try. Anecdotally as of this writing,
 `CompletionAI` seems to be more accurate, even though it is using the text
 completion API vs the function calling feature of the chat API. This may be due
 to the implementation or issues arising from the translation into roles
 discussed elsewhere.
 
@@ -677,33 +646,34 @@
 So, `agency` is a more general framework intended to support agent development
 and to ultimately enable agents to safely integrate with anything, in any way
 imaginable.
 
 ## What are some known limitations or issues?
 
 * It's a new project, so keep that in mind in terms of completeness, but see
-the plans below for where this is heading. Core functionality is pretty
-well tested at the moment.
+  [the issues page](https://github.com/operand/agency/issues) for what is
+  currently planned. Core functionality is pretty well tested at the moment.
 
 * This library makes use of threads for each individual agent. Multithreading
-is limited by python's GIL, meaning if you run a CPU bound model other agents
-will have to wait for their "turn". This goes for anything else you might define
-as an "agent", if it is CPU heavy it will block other agents. Note that I/O does
-not block, so networked backends or services will execute in parallel.  Other
-forms of multiprocessing to avoid the GIL may eventually be considered.
+  is limited by python's GIL, meaning if you run a CPU bound model other agents
+  will have to wait for their "turn". This goes for anything else you might
+  define as an "agent", if it is CPU heavy it will block other agents. Note that
+  I/O does not block, so networked backends or services will execute in
+  parallel.
+
+  Other forms of multiprocessing to avoid the GIL will be considered.
 
 * This API does NOT assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
-  of representing many things uniquely and independently.
-
-  This is a core feature of `agency`: that all things are treated the same and
-  may be interacted with through common means.
+  of representing many things uniquely and independently. This is a core feature
+  of `agency`: that all things are treated the same and may be interacted with
+  through common means.
 
   The lack of roles introduces some challenges in integrating with role based
   APIs. See the implementation of
   [`OpenAIFunctionAgent`](./agency/agents/openai_function_agent.py) for an
   example.
 
 * There is not much by way of storage support. That is mostly left up to you and
@@ -713,17 +683,14 @@
   APIs may be considered in the future.
 
 
 # Contributing
 
 Please do!
 
-If you have any questions, suggestions, or problems, please open an
-[issue](https://github.com/operand/agency/issues).
-
 
 ## Development Installation
 
 ```bash
 git clone git@github.com:operand/agency.git
 cd agency
 poetry install
@@ -746,39 +713,27 @@
 human, artificial, and other computing systems together, with the following
 priorities.
 
 
 ## Priorities
 - **Speed**:
   Performance is always a concern. If it's not performant, it's not practical.
-  Currently the limitations of python multi-threading are a bottleneck.
+  Currently the limitations of python multi-threading are a bottleneck and a
+  priority to address.
 - **Access Control and Safety**:
   An effective access control solution for agent-integrated systems is
   fundamental to ensure safety. I believe I've included a sane first step at
   such a pattern, but further development will be a focus of this project.
 - **Compatibility and Usability**:
   In general, I believe this is a fair start in defining a set of patterns for
   creating agent systems. I hope to ensure the API is kept small, and
   compatible with a wide variety of use cases.
 - **Documentation**:
   I hope to ensure documentation is kept organized, clear, and accurate. This
   readme serves as a start.
 
 
 ## Planned Work
-- Add web app multimodal i/o examples
-  - image
-  - audio
-  - video
-- Add multimodal model integration example
-- Add message broker/networking support (RabbitMQ)
-- Add integration example for [mlc-llm](https://github.com/mlc-ai/mlc-llm)
-- Add integration example for [gorilla](https://github.com/ShishirPatil/gorilla)
-- Add integration example for LangChain
-- Add model training example
-- Consider alternative multiprocessing approaches
-- Consider adding a storage API
-- Consider prior work on distributed access control
-- Add docker assets to encourage using it
-- [_feel free to make
-suggestions_](https://github.com/operand/agency/issues)
 
+[Please see the issues page.](https://github.com/operand/agency/issues)
+
+If you have any suggestions or otherwise, feel free to add an issue!
```

