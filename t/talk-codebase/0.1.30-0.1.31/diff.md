# Comparing `tmp/talk_codebase-0.1.30.tar.gz` & `tmp/talk_codebase-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.30.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.31.tar", max compression
```

## Comparing `talk_codebase-0.1.30.tar` & `talk_codebase-0.1.31.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2866 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/README.md
--rw-r--r--   0        0        0      896 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/pyproject.toml
--rw-r--r--   0        0        0     4442 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2898 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/talk_codebase/cli.py
--rw-r--r--   0        0        0     1724 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/talk_codebase/consts.py
--rw-r--r--   0        0        0     2474 2023-06-14 11:24:17.670249 talk_codebase-0.1.30/talk_codebase/utils.py
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 talk_codebase-0.1.30/PKG-INFO
+-rw-r--r--   0        0        0     2874 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/README.md
+-rw-r--r--   0        0        0      896 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0     4442 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1724 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2474 2023-06-17 00:25:49.817072 talk_codebase-0.1.31/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.31/PKG-INFO
```

### Comparing `talk_codebase-0.1.30/README.md` & `talk_codebase-0.1.31/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,71 @@
-## talk-codebase: Tool for chatting with your codebase and docs using OpenAI, LlamaCpp, and GPT-4-All
-
+## talk-codebase 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
+* Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
+* It supports offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
+* Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
+
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
-## Description
-
-Talk-codebase is a tool that allows you to converse with your codebase using LLMs to answer your queries. It supports
-offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third
-parties, or you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and
-not for production use.
-
 ## Installation
 
-To install `talk-codebase`, you need to have Python 3.9 and an OpenAI API
-key [api-keys](https://platform.openai.com/account/api-keys).
-Additionally, if you want to use the GPT4All model, you need to download
-the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model. If you prefer a
-different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the configuration
-and specify its
-path in the configuration. If you want some files to be ignored, add them to .gitignore.
+To install talk-codebase, you need to have:
 
-To install `talk-codebase`, run the following command in your terminal:
+* Python 3.9
+* An OpenAI API [api-keys](https://platform.openai.com/account/api-keys)
+* (Optional) [GPT4All](https://gpt4all.io) model
 
 ```bash
+# Install talk-codebase
 pip install talk-codebase
-```
 
-Once `talk-codebase` is installed, you can use it to chat with your codebase by running the following command:
+# Configure talk-codebase
+talk-codebase configure
 
-```bash
-talk-codebase chat <path-to-your-codebase>
+# If you want some files to be ignored, add them to .gitignore.
+# Once `talk-codebase` is installed, you can use it to chat with your codebase in the current directory by running the following command:
+talk-codebase chat .
 ```
 
-If you need to configure or edit the configuration, you can run:
-
-```bash
-talk-codebase configure
-```
+## Advanced configuration
 
 You can also edit the configuration manually by editing the `~/.config.yaml` file.
 If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
 the path to the configuration file.
 
 ```yaml
 # The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
 api_key: sk-xxx
-# maximum overlap between chunks. It can be nice to have some overlap to maintain some continuity between chunks
-chunk_overlap: '50'
-# maximum size of a chunk
-chunk_size: '500'
-# number of samples to generate for each prompt.
-k: '4'
-# maximum tokens for the LLMs
-max_tokens: '1048'
-# token limit for the LLM model only OpenAI
+
+# Configuration for chunking
+chunk_overlap: 50
+chunk_size: 500
+
+# Configuration for sampling
+k: 4
+max_tokens: 1048
+
+# Configuration for the LLM model
 model_name: gpt-3.5-turbo
-# path to the llm file on disk.
 model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
-# type of the LLM model. It can be either local or openai
 model_type: openai
-
 ```
 
-## The supported extensions:
+## Supports the following extensions:
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
 - [x] `.epub`
 - [x] `.md`
 - [x] `.pdf`
 - [x] `.txt`
 - [x] `popular programming languages`
 
 ## Contributing
 
-Contributions are always welcome!
+* If you find a bug in talk-codebase, please report it on the project's issue tracker. When reporting a bug, please include as much information as possible, such as the steps to reproduce the bug, the expected behavior, and the actual behavior.
+* If you have an idea for a new feature for Talk-codebase, please open an issue on the project's issue tracker. When suggesting a feature, please include a brief description of the feature, as well as any rationale for why the feature would be useful.
+* You can contribute to talk-codebase by writing code. The project is always looking for help with improving the codebase, adding new features, and fixing bugs.
```

### Comparing `talk_codebase-0.1.30/pyproject.toml` & `talk_codebase-0.1.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.30"
+version = "0.1.31"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.30/talk_codebase/LLM.py` & `talk_codebase-0.1.31/talk_codebase/LLM.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.30/talk_codebase/cli.py` & `talk_codebase-0.1.31/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.30/talk_codebase/consts.py` & `talk_codebase-0.1.31/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.30/talk_codebase/utils.py` & `talk_codebase-0.1.31/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.30/PKG-INFO` & `talk_codebase-0.1.31/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.30
+Version: 0.1.31
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,88 +20,79 @@
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: unstructured (>=0.6.10,<0.7.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
-## talk-codebase: Tool for chatting with your codebase and docs using OpenAI, LlamaCpp, and GPT-4-All
-
+## talk-codebase 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
+* Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
+* It supports offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
+* Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
+
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
-## Description
-
-Talk-codebase is a tool that allows you to converse with your codebase using LLMs to answer your queries. It supports
-offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third
-parties, or you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and
-not for production use.
-
 ## Installation
 
-To install `talk-codebase`, you need to have Python 3.9 and an OpenAI API
-key [api-keys](https://platform.openai.com/account/api-keys).
-Additionally, if you want to use the GPT4All model, you need to download
-the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model. If you prefer a
-different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the configuration
-and specify its
-path in the configuration. If you want some files to be ignored, add them to .gitignore.
+To install talk-codebase, you need to have:
 
-To install `talk-codebase`, run the following command in your terminal:
+* Python 3.9
+* An OpenAI API [api-keys](https://platform.openai.com/account/api-keys)
+* (Optional) [GPT4All](https://gpt4all.io) model
 
 ```bash
+# Install talk-codebase
 pip install talk-codebase
-```
 
-Once `talk-codebase` is installed, you can use it to chat with your codebase by running the following command:
+# Configure talk-codebase
+talk-codebase configure
 
-```bash
-talk-codebase chat <path-to-your-codebase>
+# If you want some files to be ignored, add them to .gitignore.
+# Once `talk-codebase` is installed, you can use it to chat with your codebase in the current directory by running the following command:
+talk-codebase chat .
 ```
 
-If you need to configure or edit the configuration, you can run:
-
-```bash
-talk-codebase configure
-```
+## Advanced configuration
 
 You can also edit the configuration manually by editing the `~/.config.yaml` file.
 If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
 the path to the configuration file.
 
 ```yaml
 # The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
 api_key: sk-xxx
-# maximum overlap between chunks. It can be nice to have some overlap to maintain some continuity between chunks
-chunk_overlap: '50'
-# maximum size of a chunk
-chunk_size: '500'
-# number of samples to generate for each prompt.
-k: '4'
-# maximum tokens for the LLMs
-max_tokens: '1048'
-# token limit for the LLM model only OpenAI
+
+# Configuration for chunking
+chunk_overlap: 50
+chunk_size: 500
+
+# Configuration for sampling
+k: 4
+max_tokens: 1048
+
+# Configuration for the LLM model
 model_name: gpt-3.5-turbo
-# path to the llm file on disk.
 model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
-# type of the LLM model. It can be either local or openai
 model_type: openai
-
 ```
 
-## The supported extensions:
+## Supports the following extensions:
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
 - [x] `.epub`
 - [x] `.md`
 - [x] `.pdf`
 - [x] `.txt`
 - [x] `popular programming languages`
 
 ## Contributing
 
-Contributions are always welcome!
+* If you find a bug in talk-codebase, please report it on the project's issue tracker. When reporting a bug, please include as much information as possible, such as the steps to reproduce the bug, the expected behavior, and the actual behavior.
+* If you have an idea for a new feature for Talk-codebase, please open an issue on the project's issue tracker. When suggesting a feature, please include a brief description of the feature, as well as any rationale for why the feature would be useful.
+* You can contribute to talk-codebase by writing code. The project is always looking for help with improving the codebase, adding new features, and fixing bugs.
+
```

