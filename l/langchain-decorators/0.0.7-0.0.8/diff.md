# Comparing `tmp/langchain-decorators-0.0.7.tar.gz` & `tmp/langchain-decorators-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.0.7.tar", last modified: Thu Jun 15 13:37:39 2023, max compression
+gzip compressed data, was "langchain-decorators-0.0.8.tar", last modified: Fri Jun 16 23:04:47 2023, max compression
```

## Comparing `langchain-decorators-0.0.7.tar` & `langchain-decorators-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.090661 langchain-decorators-0.0.7/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.7/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 13:37:39.090448 langchain-decorators-0.0.7/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16253 2023-06-14 19:55:04.000000 langchain-decorators-0.0.7/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.7/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-15 13:37:39.090714 langchain-decorators-0.0.7/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.7/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.083658 langchain-decorators-0.0.7/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.088773 langchain-decorators-0.0.7/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      301 2023-06-15 13:37:22.000000 langchain-decorators-0.0.7/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5927 2023-06-15 12:29:03.000000 langchain-decorators-0.0.7/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     7347 2023-06-15 12:40:52.000000 langchain-decorators-0.0.7/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13112 2023-06-15 12:37:50.000000 langchain-decorators-0.0.7/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17436 2023-06-13 08:10:19.000000 langchain-decorators-0.0.7/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    20072 2023-06-15 12:48:53.000000 langchain-decorators-0.0.7/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15009 2023-06-14 00:48:45.000000 langchain-decorators-0.0.7/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2572 2023-06-11 18:59:03.000000 langchain-decorators-0.0.7/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2088 2023-06-14 14:15:48.000000 langchain-decorators-0.0.7/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1624 2023-06-15 12:53:20.000000 langchain-decorators-0.0.7/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.090169 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.480293 langchain-decorators-0.0.8/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.8/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17654 2023-06-16 23:04:47.479292 langchain-decorators-0.0.8/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17299 2023-06-16 23:01:41.000000 langchain-decorators-0.0.8/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.8/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-16 23:04:47.480361 langchain-decorators-0.0.8/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.8/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.472641 langchain-decorators-0.0.8/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.477703 langchain-decorators-0.0.8/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      365 2023-06-16 22:26:59.000000 langchain-decorators-0.0.8/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     7431 2023-06-16 22:48:34.000000 langchain-decorators-0.0.8/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     7738 2023-06-16 22:36:28.000000 langchain-decorators-0.0.8/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    14968 2023-06-16 22:33:40.000000 langchain-decorators-0.0.8/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    18570 2023-06-16 21:45:20.000000 langchain-decorators-0.0.8/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21194 2023-06-16 22:50:18.000000 langchain-decorators-0.0.8/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15906 2023-06-16 19:41:06.000000 langchain-decorators-0.0.8/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4023 2023-06-16 21:33:53.000000 langchain-decorators-0.0.8/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2836 2023-06-16 22:52:56.000000 langchain-decorators-0.0.8/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1624 2023-06-15 12:53:20.000000 langchain-decorators-0.0.8/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.478994 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17654 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.0.7/LICENSE` & `langchain-decorators-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.7/PKG-INFO` & `langchain-decorators-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: langchain-decorators
-Version: 0.0.7
-Summary: syntactic sugar for langchain
-Home-page: https://github.com/ju-bezdek/langchain-decorators
-Author: Juraj Bezdek
-Author-email: juraj.bezdek@blip.solutions
-License: MIT License
-Keywords: langchain
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LangChain Decorators ✨
 
 lanchchain decorators is a layer on the top op LangChain that provides syntactic sugar 🍭 for writing custom langchain prompts and chains
 
 > **Note:** This is an unofficial addon to langchain library. It's not trying to compete, just to make using it easier. Lot's of ideas here are totally opinionated 
 
 Main principles and benefits:
@@ -258,14 +245,19 @@
 if result.is_function_call:
     result.execute()
 else:
     print(result.output_text)
 
 ```
 
+> Additionally you can also add a `function_call` argument to your LLM prompt to control GPT behavior.
+> - if you set the value to "none" - it will disable the function call for the moment, but it can still see them (useful do to some reasoning/planning before calling the function)
+> - if you set the value to "auto" - GPT will choose to use or to to use the functions
+> - if you set the value to a name of function / or the function it self (decorators will handle resolving the same name as used in schema) it will force GPT to use that function
+
 
 If you use functions argument, the output will be always `OutputWithFunctionCall`
 
 ``` python
 class OutputWithFunctionCall(BaseModel):
     output_text:str
     output:T
@@ -291,26 +283,39 @@
        ...
         
     def execute(self):
         """ Executes the function synchronously. 
         If the function is async, it will be executed in a event loop.
         """
         ...
+     def to_function_message(self, result=None):
+        """
+        Converts the result to a FunctionMessage... 
+        you can override the result collected via execute with your own
+        """
+        ...
 ```
 
 If you want to see how to schema has been build, you can use `get_function_schema` method that is added to the function by the decorator:
 ```python
+from langchain_decorators import get_function_schema
 @llm_function
 def my_func(arg1:str):
     ...
 
-print(my_func.get_function_schema())
+f_schema = get_function_schema(my_func.get_function_schema) 
+print(f_schema)
 
 ```
 
+In order to add the result to memory / agent_scratchpad you can use `to_function_message` to generate an FunctionMessage that LLM will interpret as a Tool/Function result
+
+
+## Using functions
+
 
 # Defining other parameters
 Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
 
 
 Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
 Here is how it works:
@@ -508,8 +513,8 @@
 
 # Contributing
 feedback, contributions and PR are welcomed 🙏
 
 
 # Others
 - this project is dependant on [langchain](https://github.com/hwchase17/langchain) (obviously) 
-- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts... 
+- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts...
```

### Comparing `langchain-decorators-0.0.7/README.md` & `langchain-decorators-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: langchain-decorators
+Version: 0.0.8
+Summary: syntactic sugar for langchain
+Home-page: https://github.com/ju-bezdek/langchain-decorators
+Author: Juraj Bezdek
+Author-email: juraj.bezdek@blip.solutions
+License: MIT License
+Keywords: langchain
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LangChain Decorators ✨
 
 lanchchain decorators is a layer on the top op LangChain that provides syntactic sugar 🍭 for writing custom langchain prompts and chains
 
 > **Note:** This is an unofficial addon to langchain library. It's not trying to compete, just to make using it easier. Lot's of ideas here are totally opinionated 
 
 Main principles and benefits:
@@ -245,14 +258,19 @@
 if result.is_function_call:
     result.execute()
 else:
     print(result.output_text)
 
 ```
 
+> Additionally you can also add a `function_call` argument to your LLM prompt to control GPT behavior.
+> - if you set the value to "none" - it will disable the function call for the moment, but it can still see them (useful do to some reasoning/planning before calling the function)
+> - if you set the value to "auto" - GPT will choose to use or to to use the functions
+> - if you set the value to a name of function / or the function it self (decorators will handle resolving the same name as used in schema) it will force GPT to use that function
+
 
 If you use functions argument, the output will be always `OutputWithFunctionCall`
 
 ``` python
 class OutputWithFunctionCall(BaseModel):
     output_text:str
     output:T
@@ -278,26 +296,39 @@
        ...
         
     def execute(self):
         """ Executes the function synchronously. 
         If the function is async, it will be executed in a event loop.
         """
         ...
+     def to_function_message(self, result=None):
+        """
+        Converts the result to a FunctionMessage... 
+        you can override the result collected via execute with your own
+        """
+        ...
 ```
 
 If you want to see how to schema has been build, you can use `get_function_schema` method that is added to the function by the decorator:
 ```python
+from langchain_decorators import get_function_schema
 @llm_function
 def my_func(arg1:str):
     ...
 
-print(my_func.get_function_schema())
+f_schema = get_function_schema(my_func.get_function_schema) 
+print(f_schema)
 
 ```
 
+In order to add the result to memory / agent_scratchpad you can use `to_function_message` to generate an FunctionMessage that LLM will interpret as a Tool/Function result
+
+
+## Using functions
+
 
 # Defining other parameters
 Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
 
 
 Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
 Here is how it works:
@@ -495,8 +526,8 @@
 
 # Contributing
 feedback, contributions and PR are welcomed 🙏
 
 
 # Others
 - this project is dependant on [langchain](https://github.com/hwchase17/langchain) (obviously) 
-- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts... 
+- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts...
```

### Comparing `langchain-decorators-0.0.7/setup.py` & `langchain-decorators-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/chains.py` & `langchain-decorators-0.0.8/src/langchain_decorators/chains.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from langchain.callbacks.manager import CallbackManagerForChainRun, AsyncCallbackManagerForChainRun
 from langchain.tools.base import BaseTool
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts.chat import  ChatPromptValue
 from langchain.schema import PromptValue, ChatGeneration
 from pydantic import root_validator
+
+from .function_decorator import get_function_schema
 try:
     from langchain.tools.convert_to_openai import format_tool_to_openai_function
 except ImportError:
     pass
 
 MODELS_WITH_FUNCTIONS_SUPPORT=["gpt-3.5-turbo-0613","gpt-4-0613"]
 
@@ -43,16 +45,18 @@
         llm = values.get("llm",None)
         if functions:
             function_schemas=[None for _ in functions]
             for i,f in enumerate(functions):
                 if isinstance(f, BaseTool):
                     function_schemas[i] = format_tool_to_openai_function(f)
                 elif callable(f) and hasattr(f,"get_function_schema"):
-                    if hasattr(f,"get_function_schema"):
-                        function_schemas[i] = f.get_function_schema()
+                    schema = get_function_schema(f)
+                    if not schema:
+                        raise ValueError(f"Invalid item value in functions. Unable to retrieve schema from function {f}")
+                    function_schemas[i] =schema
                 else:
                     raise ValueError(f"Invalid item value in functions. Only Tools or functions decorated with @llm_function are allowed. Got: {f}")
             values["function_schemas"] = function_schemas
         if not llm:
             raise ValueError("llm must be defined")
         elif functions:
             if not isinstance(llm,ChatOpenAI):
@@ -61,56 +65,81 @@
                 if llm.model_name not in MODELS_WITH_FUNCTIONS_SUPPORT:
                     # keeping this as a warning to keep it future proof
                     logging.warn(f"WARNING! Model {llm.model_name} likely does not support functions. Functions will be likely ignored!)")
 
         return values
     
 
+    def preprocess_inputs(self, input_list):
+        additional_kwargs={}
+        if "function_call" in input_list[0]:
+            for input in input_list:
+                function_call=input.pop("function_call")
+            # function call should be only one... and the same for all inputs... there shouldn't be more anyway
+            if not isinstance(function_call,str):
+                #find the index of the function in self.functions
+                function_index = self.functions.index(function_call)
+                if function_index == -1:
+                    raise ValueError(f"Invalid function call. Function {function_call} is not defined in this chain")
+                function_call = {"name": self.function_schemas[function_index]["name"]}
+            elif function_call not in ["none","auto"]:
+                function_call = {"name": function_call}
+
+            additional_kwargs["function_call"]=function_call 
+        return additional_kwargs
 
 
 
     def generate(
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
+        
+        additional_kwargs = self.preprocess_inputs(input_list)
+           
         prompts, stop = self.prep_prompts(input_list, run_manager=run_manager)
         if self.functions:
+            
             chat_model:BaseChatModel=self.llm
           
             messages = [prompt.to_messages() for prompt in prompts]
              
             result =  chat_model.generate(messages=messages, 
                                         stop=stop, callbacks=run_manager.get_child() if run_manager else None,
-                                        functions=self.function_schemas)
+                                        functions=self.function_schemas,
+                                        **additional_kwargs
+                                        )
             return result
         else:
             return self.llm.generate_prompt(
                 prompts, stop, callbacks=run_manager.get_child() if run_manager else None
             )
 
     async def agenerate(
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
-        prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
-        
+        additional_kwargs = self.preprocess_inputs(input_list)
     
+        prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
         if self.functions:
             chat_model:BaseChatModel=self.llm
             if len(prompts)!=1:
                 raise ValueError("Only one prompt is supported when using functions")
             messages = [prompt.to_messages() for prompt in prompts]
              
             return  await chat_model.agenerate(messages=messages, 
                                          stop=stop, callbacks=run_manager.get_child() if run_manager else None,
-                                         functions=self.function_schemas)
+                                         functions=self.function_schemas,
+                                         **additional_kwargs
+                                         )
         else:
             return await self.llm.agenerate_prompt(
                 prompts, stop, callbacks=run_manager.get_child() if run_manager else None
             )
         
     def _create_output(self,generation):
         res = {
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/common.py` & `langchain-decorators-0.0.8/src/langchain_decorators/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,48 +109,55 @@
     def as_verbose(self):
         return PromptTypeSettings(llm=self.llm, color=self.color, log_level=100, capture_stream=self.capture_stream)
 
 
 class PromptTypes:
     UNDEFINED: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.BLACK_AND_WHITE, log_level=logging.DEBUG)
+    BIG_CONTEXT: PromptTypeSettings = PromptTypeSettings(
+        llm=ChatOpenAI(temperature=0.0, model="gpt-3.5-turbo-16k"), 
+        color=LogColors.BLACK_AND_WHITE, log_level=logging.DEBUG)
+        
     AGENT_REASONING: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.GREEN, log_level=logging.INFO)
     TOOL: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.BLUE, log_level=logging.INFO)
     FINAL_OUTPUT: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.YELLOW, log_level=logging.INFO)
 
 
 def get_func_return_type(func: callable)->Tuple:
     return_type = func.__annotations__.get("return",None)
     if inspect.iscoroutinefunction(func):
         if return_type:
             if is_generic_type(return_type):
                 return_type_origin = get_origin(return_type)
-                if issubclass(return_type_origin, Coroutine):
+                if return_type_origin and issubclass(return_type_origin, Coroutine):
                     return_type_args = getattr(return_type, '__args__', None)
                     if return_type_args and len(return_type_args) == 3:
-                        return return_type_args[2]
+                        return_type = return_type_args[2]
                     else:
                         raise Exception(f"Invalid Coroutine annotation {return_type}. Expected Coroutine[ any , any, <return_type>] or just <return_type>")
                 else:
-                    return return_type_origin
-            elif is_union_type(return_type):
-                return_type_args = getattr(return_type, '__args__', None)
-                if return_type_args and len(return_type_args) == 2 and return_type_args[1] == type(None):
-                    return return_type_args[0]
-                else:
-                    raise Exception(f"Invalid Union annotation {return_type}. Expected Union[ <return_type>, None] or just <return_type>")
+                    return_type = return_type_origin
+        else:
+            
+            if issubclass(return_type, Coroutine):
+                return None
             else:
-                
-                if issubclass(return_type, Coroutine):
-                    return None
-                else:
-                    return return_type
+                return_type = return_type
+    
+    if return_type and is_union_type(return_type):
+        return_type_args = getattr(return_type, '__args__', None)
+        if return_type_args and len(return_type_args) == 2 and return_type_args[1] == type(None):
+            return return_type_args[0]
+        else:
+            raise Exception(f"Invalid Union annotation {return_type}. Expected Union[ <return_type>, None] or just <return_type>")
+    else:
+        return return_type
             
             
 def get_function_docs(func: callable)->Tuple:
     if not func.__doc__:
         return None
     fist_line, rest = func.__doc__.split('\n', 1) if '\n' in func.__doc__ else (func.__doc__, "")
     # we dedent the first line separately,because its common that it often starts right after """
@@ -169,14 +176,16 @@
 
 def get_arguments_as_pydantic_fields(func) -> Dict[str, ModelField]:
     argument_types = {}
     model_config = BaseConfig()
     for arg_name, arg_desc in inspect.signature(func).parameters.items():
         if arg_name != "self":
             default = arg_desc.default if arg_desc.default!=inspect.Parameter.empty else None
+            if arg_desc.annotation==inspect._empty:
+                raise Exception(f"Argument '{arg_name}' of function {func.__name__} has no type annotation")
             argument_types[arg_name] = ModelField(
                 class_validators=None,
                 model_config=model_config,
                 name=arg_name, 
                 type_=arg_desc.annotation,
                 default=default,
                 required= arg_desc.default==inspect.Parameter.empty
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/function_decorator.py` & `langchain-decorators-0.0.8/src/langchain_decorators/function_decorator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,151 +1,201 @@
-from functools import wraps
+import re
 import inspect
-from textwrap import dedent
-from typing import Callable, Dict, Union, Type
+from enum import Enum
+from functools import wraps
+from typing import Callable,  Union, Type
 from pydantic import BaseModel
 from pydantic.fields import ModelField
-import re
-from enum import Enum
+from pydantic.schema import  field_schema
+import copy
 
+from .pydantic_helpers import sanitize_pydantic_schema
 from .common import  get_arguments_as_pydantic_fields, get_function_docs, get_function_full_name
 
 class DocstringsFormat(Enum):
     AUTO = "auto"
     GOOGLE = "google"
     SPHINX = "sphinx"
     NUMPY = "numpy"
 
+def get_function_schema(func):
+    if callable(func) and hasattr(func,"get_function_schema"):
+        return func.get_function_schema(func)
+    else:
+        return None
+
 
 def llm_function(
-       argument_schema:Union[str, Type[BaseModel], dict]="auto",
-       validate_docstrings:bool=True,
-       docstring_format:str="auto",
+        function_name:str=None,
+        argument_schema:Union[str, Type[BaseModel], dict]="auto",
+        validate_docstrings:bool=True,
+        docstring_format:str="auto",
         ):
     """
     Decorator for functions that take a language model as first argument.
 
-     - argument_schema
-        - `auto` (default): the schema is automatically inferred from the function signature. If docstrings are provided, they will be used to enhance function description
-        - `pydantic` -  expects a pydantic model as first and only argument ('self' being ignored) - allows for controllable schema
-        - `docstring` - parses the schema ONLY from the docstring
-
-        or define pydantic model:
-        ```
-        @llm_function(argument_schema=MyFunctionPydanticArgsSchema)
-        def my_function(self, question:str)->bool:
-            ...
-        ```
 
-        or define a simple dict with descriptions:
-        ```
-        @llm_function(argument_schema={"question": "Question to ask"})
-        def my_function(self, question:str)->bool:
-            ...
-        ```
-    - validate_docstrings: if True, the docstrings will be parsed and validated against function. If parsing or validation fails, an error will be raised
+    Args:
+        - function_name: the name of the function for LLM. If not provided, the name of the function will be used
 
-    - docstring_format: the format of the docstring
-        -  `auto` (default): the format is automatically inferred from the docstring
-        -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
-        -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
-        -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
+        - argument_schema
+            - `auto` (default): the schema is automatically inferred from the function signature. If docstrings are provided, they will be used to enhance function description
+            - `pydantic` -  expects a pydantic model as first and only argument ('self' being ignored) - allows for controllable schema
+            - `docstring` - parses the schema ONLY from the docstring
+
+            or define pydantic model:
+            ```
+            @llm_function(argument_schema=MyFunctionPydanticArgsSchema)
+            def my_function(self, question:str)->bool:
+                ...
+            ```
+
+            or define a simple dict with descriptions:
+            ```
+            @llm_function(argument_schema={"question": "Question to ask"})
+            def my_function(self, question:str)->bool:
+                ...
+            ```
+
+        - validate_docstrings: if True, the docstrings will be parsed and validated against function. If parsing or validation fails, an error will be raised
+
+        - docstring_format: the format of the docstring
+            -  `auto` (default): the format is automatically inferred from the docstring
+            -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
+            -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
+            -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
 
     Examples:
-    Google style docstrings:
-    ```python
-    @llm_function
-    def function_with_google_docstrings(self, question:str)->bool:
-        \"\"\"
-        This is a function with google docstrings
-        Args:  # but accepts also Parameters, Arguments
-            question (str): Question to ask
-        \"\"\"
-    ```
-
-    ```python
-    @llm_function
-    def function_with_numpy_docstrings(self, question:str)->bool:
-        \"\"\"
-        This is a function with google docstrings
-        Parameters # but accepts also Args, Arguments
-        ----------
-            question :int
-                Question to ask
-            
-        \"\"\"
-    ```
+    
+        Google style docstrings:
+        ```python
+        @llm_function
+        def function_with_google_docstrings(self, question:str)->bool:
+            \"\"\"
+            This is a function with google docstrings
+            Args:  # but accepts also Parameters, Arguments
+                question (str): Question to ask
+            \"\"\"
+        ```
 
-    ```python
-    @llm_function
-    def function_with_sphinx_docstrings(self, question:str)->bool:
-        \"\"\"
-        This is a function with google docstrings
-        :param question: Question to ask
-            
-        \"\"\"
-    ```
+        ```python
+        @llm_function
+        def function_with_numpy_docstrings(self, question:str)->bool:
+            \"\"\"
+            This is a function with google docstrings
+            Parameters # but accepts also Args, Arguments
+            ----------
+                question :int
+                    Question to ask
+                
+            \"\"\"
+        ```
 
-    Note: The fact whether the parameter is optional is inferred from the function signature. You can also document it, but it will be just part of the description. If typing annotations are used (i.e. Optional[str]), this will be stripped to native type.
+        ```python
+        @llm_function
+        def function_with_sphinx_docstrings(self, question:str)->bool:
+            \"\"\"
+            This is a function with google docstrings
+            :param question: Question to ask
+                
+            \"\"\"
+        ```
+
+    Note: 
+        The fact whether the parameter is optional is inferred from the function signature. You can also document it, but it will be just part of the description. If typing annotations are used (i.e. Optional[str]), this will be stripped to native type.
     
     """
     
-    if callable(argument_schema):
+    if callable(function_name):
         # this is the case when the decorator is called without arguments
         # we initialize params with default values
-        func = argument_schema
-        argument_schema = "auto"
+        func = function_name
+        function_name=None
     else:
         func = None
+
+
+    def get_function_schema(_func, _validate_docstrings=validate_docstrings):
+            return build_func_schema(_func, 
+                                            function_name = function_name, 
+                                            format=docstring_format, 
+                                            validate_docstrings=_validate_docstrings
+                                          )
     
     def decorator(func):
         
         is_async = inspect.iscoroutinefunction(func)
 
         if not is_async:
             @wraps(func)
             def func_wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
             
         else:
             @wraps(func)
             async def func_wrapper(*args, **kwargs):
                 return await func(*args, **kwargs)
-        def get_function_schema(_validate_docstrings=validate_docstrings):
-            return build_func_description(func, format=docstring_format, validate_docstrings=_validate_docstrings)
+        
+        
+        
+       
+
         func_wrapper.get_function_schema=get_function_schema
         return func_wrapper
     
     if func:
         return decorator(func)
     else:
         return decorator
     
 
+class LllFunctionWithModifiedSchema:
+    def __init__(self, func, modified_schema:dict):
+        self.func = func
+        self._function_schema = modified_schema
+
+
+    def __call__(self, *args, **kwargs):
+        return self.func(*args, **kwargs)
+
+    def get_function_schema(self):
+        return self._function_schema
+        
+         
 
 
 
-from pydantic.schema import get_field_info_schema, field_schema
-def build_func_description(func:Callable, format:Union[DocstringsFormat,str]="auto", validate_docstrings:bool=True):
+def build_func_schema(
+        func:Callable, 
+        function_name:str=None, 
+        format:Union[DocstringsFormat,str]="auto", 
+        validate_docstrings:bool=True
+        ):
     
     if isinstance(format,str):
         format = DocstringsFormat(format)
 
     func_docs = get_function_docs(func)  
-    func_name= get_function_full_name(func)
-    
 
+    if function_name and not re.match(r"^[a-zA-Z_][a-zA-Z0-9_]*$", function_name):
+        raise ValueError(f"Invalid function name: {function_name} for {get_function_full_name(func)}. Only letters, numbers and underscores are allowed. The name must start with a letter or an underscore.")
+   
+    func_name =  function_name or func.__name__
     arguments_fields = get_arguments_as_pydantic_fields(func)
     
     args_schema = None
     if len(arguments_fields)==1:
         first_param:ModelField = list(arguments_fields.values())[0]
-        if first_param.required == True and issubclass(first_param.type_, BaseModel):
+            
+        if first_param.type_==first_param.outer_type_ and first_param.required == True and issubclass(first_param.type_, BaseModel):
+            if first_param.type_==BaseModel:
+                raise ValueError(f"Invalid argument type for {get_function_full_name(func)}. The argument type cannot be pydantic BaseModel. Please use a subclass of BaseModel.")
             # the one and only argument is a pydantic model
             args_schema =  first_param.type_.schema()
+            sanitize_pydantic_schema(args_schema)
             args_schema={
                 "type":"object",
                 "properties":args_schema["properties"],
                 "required":args_schema["required"]
             }
     
     if not args_schema:
@@ -198,16 +248,17 @@
         #title is autogenerated by pydantic and will just costs us tokens....
         if "title" in schema:
             del schema["title"]
         return schema
     args_schema["properties"] = {prop:pop_prop_title(prop_schema) for prop, prop_schema in args_schema["properties"].items()}
     
     description = parse_function_description_from_docstrings(func_docs) if func_docs else None
+
     if not description:
-        raise ValueError(f"LLM Function {func_name} has no description in docstrings")
+        raise ValueError(f"LLM Function {get_function_full_name(func)} has no description in docstrings")
     return {
         "name":func_name,
         "description":description,
         "parameters":args_schema
     }
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.0.8/src/langchain_decorators/output_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import datetime
 import logging
-from textwrap import dedent, indent
+from textwrap import dedent
 from typing import Dict, List, Type, TypeVar, Union
 from langchain.output_parsers import PydanticOutputParser
 from langchain.schema import BaseOutputParser, OutputParserException
 
 import re
 import json
 import yaml
 from pydantic import BaseModel, ValidationError
 from pydantic.fields import ModelField
+from .function_decorator import llm_function
 from .pydantic_helpers import *
 
 
 class OutputParserExceptionWithOriginal(OutputParserException):
     """Exception raised when an output parser fails to parse the output of an LLM call."""
 
     def __init__(self, message: str, original: str, original_prompt_needed_on_retry:bool=False) -> None:
@@ -194,14 +195,45 @@
         """Instructions on how the LLM output should be formatted."""
         if not self.instructions_as_json_example:
             return "Return result as a valid JSON that matched this json schema definition:\n" + yaml.safe_dump(self.model.schema())
         else:
 
             return dedent(f"""```json\n{self.get_json_example_description(self.model)}\n```""").strip()
 
+class OpenAIFunctionsPydanticOutputParser(BaseOutputParser[T]):
+    model: Type[T]
+
+    @property
+    def _type(self) -> str:
+        return "opanai_functions_pydantic"
+    
+    def __init__(self, model: Type[T]):
+        super().__init__(model=model)
+
+    def parse(self, function_call_arguments:dict ) -> T:
+        try:
+            return self.model.parse_obj(function_call_arguments)
+        except ValidationError as e:
+            err_msg =humanize_pydantic_validation_error(e)
+            serialized= json.dumps(function_call_arguments)
+            raise OutputParserExceptionWithOriginal(f"Function call arguments are not in correct format: {serialized}Errors: {err_msg}",serialized)
+        
+
+    def get_format_instructions(self) -> str:
+        return "" # will be handled by openai
+    
+    
+    def build_llm_function(self):
+        @llm_function()
+        def generate_response( output:self.model) -> T:
+            """ Use this to transform the data into desired format. """
+            #above is a description for LLM...
+            return output
+        return generate_response
+
 
 class CheckListParser(ListOutputParser):
     """Parses list a a dictionary... assume this format:
         - KeyParma1: Value1
         - KeyPara2: Value2
         ...
     """
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.0.8/src/langchain_decorators/prompt_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,28 @@
     Note that the code of the function will never be executed... 
 
     Args:
         `prompt_type`: (Optional[PromptTypeSettings]) - This allows you mark your prompt with one of the predefined prompt types (see PromptTypes class - but you can subclass it!) to predefine some settings like LLM or style and color of logging into console.
 
         `template_format` (Optional[str]): one of [ `f-string` | `f-string-extra` ] ... f-string-extra is a superset of f-string template formats, enabling for optional sections.
 
-        `output_formatting` (Optional[str]): one of [ `auto` | `json` | `str` | `list` ] or `None` or langchain OutputParser object - you can control how will the output be parsed. 
+        `output_parser` (Optional[str]): one of [ `auto` | `json` | `str` | `list` ] or `None` or langchain OutputParser object - you can control how will the output be parsed. 
         
             `auto` - default - determine the output type automatically based on output type annotations
 
             `str` or `None` - will return plain string output
 
             `list` - will parse bullet or numbered list (each item on a new line) as a list
 
             `boolean` - will parse the output as boolean. Expects clear Yes/No in the output
 
             `json` - will parse the output as json
 
+            `functions` - will use the OpenAI functions to generate the output in desired format ... only for pydataic models and ChatOpenAI model
+
             `markdown` - will parse the output as markdown sections, the name of each section will be returned as a key and the content as a value. For nested sections, the value will be a dict with the same structure.
 
             `pydantic` - will parse the output as json and then convert into a pydantic model
 
 
         `stop_tokens` (Optional[List[str]]): list of stop tokens to instruct the LLM to stop generating text when it encounters any of these tokens. If not provided, the default stop tokens of the LLM will be used.
 
@@ -186,20 +188,25 @@
             else:
                 memory=None
 
             if "functions" in kwargs:
                 functions=kwargs.pop("functions")
             else:
                 functions=None
+
                 
             if functions:
                 llmChain = LLMChainWithFunctionSupport(llm=prompt_llm, prompt=prompt_template,  memory=memory, functions=functions)
+            elif isinstance(prompt_template.output_parser, OpenAIFunctionsPydanticOutputParser):
+                function=prompt_template.output_parser.build_llm_function()
+                kwargs["function_call"] = function
+                llmChain = LLMChainWithFunctionSupport(llm=prompt_llm, prompt=prompt_template,  memory=memory, functions=[function])
             else:
                 llmChain = LLMChain(llm=prompt_llm, prompt=prompt_template,  memory=memory)
-            other_supported_kwargs={"stop","callbacks"}
+            other_supported_kwargs={"stop","callbacks","function_call"}
             unexpected_inputs = [key for key in kwargs if key not in prompt_template.input_variables and key not in other_supported_kwargs ]
             if unexpected_inputs:
                 raise TypeError(f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}\nHint: Make sure that you've used all the inputs in the template")
             
             missing_inputs = [key for key in prompt_template.input_variables if key not in kwargs ]
             if format_instructions_parameter_key in missing_inputs:
                 missing_inputs.remove(format_instructions_parameter_key)
@@ -222,16 +229,19 @@
                 else:
                     raise TypeError(f"{full_name}: missing 1 required keyword-only argument: {missing_inputs}")
                 
             
             if stop_tokens:
                 kwargs["stop"]=stop_tokens
             call_args = {"inputs":kwargs, "return_only_outputs":True, "callbacks":callbacks}
+           
             return llmChain, call_args
         
+        
+        
         def get_retry_parse_call_args(prompt_template:PromptDecoratorTemplate, exception:OutputParserExceptionWithOriginal, get_original_prompt:Callable):
             logging.warning(msg=f"Failed to parse output for {full_name}: {exception}\nRetrying...")
             if format_instructions_parameter_key not in prompt_str:
                 logging.warning(f"Please note that we didn't find a {format_instructions_parameter_key} parameter in the prompt string. If you don't include it in your prompt template, you need to provide your custom formatting instructions.")    
             if exception.original_prompt_needed_on_retry:
                 original_prompt=get_original_prompt()
             else:
@@ -244,17 +254,24 @@
             if not format_instructions:
                 raise Exception(f"Failed to get format instructions for {full_name} from output parser {prompt_template.output_parser}.")
             call_kwargs = {"original_prompt":original_prompt, "original":exception.original, "format_instructions":format_instructions}
             return retryChain, call_kwargs
         
         def process_results(llmChain, result_data, result, is_function_call):
             log_results(result_data, result, is_function_call, verbose, prompt_type)
-            if llmChain.prompt.output_parser:
-                if result or not is_function_call:
-                    result = llmChain.prompt.output_parser.parse(result)
+            if llmChain.prompt.output_parser:    
+                if isinstance(llmChain.prompt.output_parser, OpenAIFunctionsPydanticOutputParser):
+                    # there is no result probably, but if there is, we ignore it... we are interested only in tha data in function_call_info
+                    result = llmChain.prompt.output_parser.parse(result_data["function_call_info"]["arguments"])
+                    result_data.pop("function_call_info") # we don't need it anymore, and later in the code we check it its here to create OutputWithFunctionCall
+                    result_data.pop("function")
+
+                else:
+                    if result:
+                        result = llmChain.prompt.output_parser.parse(result)
             return result
 
         if not is_async:
 
             @wraps(func)
             def wrapper(*args, **kwargs):
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.0.8/src/langchain_decorators/prompt_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from langchain import PromptTemplate
 from langchain.prompts import StringPromptTemplate
 from langchain.prompts.chat import  MessagesPlaceholder, ChatMessagePromptTemplate, ChatPromptTemplate, ChatPromptValue
 from langchain.schema import PromptValue, BaseOutputParser
 
 from promptwatch import register_prompt_template
-
+from .schema import OutputWithFunctionCall
 from .common import LogColors, PromptTypeSettings, get_func_return_type, get_function_docs, get_function_full_name, print_log
 from .output_parsers import *
 
 
 def parse_prompts_from_docs(docs:str):
     prompts = []
     for i, prompt_block in enumerate(re.finditer(r"```[^\S\n]*<prompt(?P<role>:\w+)?>\n(?P<prompt>.*?)\n```[ |\t]*\n", docs, re.MULTILINE | re.DOTALL)):
@@ -218,14 +218,16 @@
                 output_parser = "str"
             elif return_type==dict:
                 output_parser = "json"
             elif return_type==list:
                 output_parser = "list"
             elif return_type==bool:
                 output_parser = "boolean"
+            elif issubclass(return_type, OutputWithFunctionCall):
+                return_type = "str"
             elif issubclass(return_type,BaseModel):
                 output_parser = PydanticOutputParser(model=return_type)
             else:
                 raise Exception(f"Unsupported return type {return_type}")
         if isinstance(output_parser,str):
             if output_parser=="str":
                 output_parser = None
@@ -243,14 +245,26 @@
             elif  output_parser == "pydantic":
                 if issubclass(return_type,BaseModel):
                     output_parser = PydanticOutputParser(model=return_type)
                 elif return_type==None:
                     raise Exception(f"You must annotate the return type for pydantic output parser, so that we can infer the model")
                 else:
                     raise Exception(f"Unsupported return type {return_type} for pydantic output parser")
+            elif output_parser=="functions":
+                if not return_type:
+                    raise Exception(f"You must annotate the return type for functions output parser, so that we can infer the model")
+                elif not issubclass(return_type,OutputWithFunctionCall):
+                    if issubclass(return_type,BaseModel):
+                        output_parser = OpenAIFunctionsPydanticOutputParser(model=return_type)
+                    else:
+                        raise Exception(f"Functions output parser only supports return type pydantic models, got {return_type}")
+                else:
+                    output_parser=None
+            else:
+                raise Exception(f"Unsupported output parser {output_parser}")
 
         
         default_values = {k:v.default for k,v in inspect.signature(func).parameters.items() if v.default!=inspect.Parameter.empty}
 
         return cls.build(
             template_string=template_string,
             template_name=template_name,
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.0.8/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.0.8/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.7
+Version: 0.0.8
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
@@ -258,14 +258,19 @@
 if result.is_function_call:
     result.execute()
 else:
     print(result.output_text)
 
 ```
 
+> Additionally you can also add a `function_call` argument to your LLM prompt to control GPT behavior.
+> - if you set the value to "none" - it will disable the function call for the moment, but it can still see them (useful do to some reasoning/planning before calling the function)
+> - if you set the value to "auto" - GPT will choose to use or to to use the functions
+> - if you set the value to a name of function / or the function it self (decorators will handle resolving the same name as used in schema) it will force GPT to use that function
+
 
 If you use functions argument, the output will be always `OutputWithFunctionCall`
 
 ``` python
 class OutputWithFunctionCall(BaseModel):
     output_text:str
     output:T
@@ -291,26 +296,39 @@
        ...
         
     def execute(self):
         """ Executes the function synchronously. 
         If the function is async, it will be executed in a event loop.
         """
         ...
+     def to_function_message(self, result=None):
+        """
+        Converts the result to a FunctionMessage... 
+        you can override the result collected via execute with your own
+        """
+        ...
 ```
 
 If you want to see how to schema has been build, you can use `get_function_schema` method that is added to the function by the decorator:
 ```python
+from langchain_decorators import get_function_schema
 @llm_function
 def my_func(arg1:str):
     ...
 
-print(my_func.get_function_schema())
+f_schema = get_function_schema(my_func.get_function_schema) 
+print(f_schema)
 
 ```
 
+In order to add the result to memory / agent_scratchpad you can use `to_function_message` to generate an FunctionMessage that LLM will interpret as a Tool/Function result
+
+
+## Using functions
+
 
 # Defining other parameters
 Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
 
 
 Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
 Here is how it works:
```

### Comparing `langchain-decorators-0.0.7/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.0.8/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

