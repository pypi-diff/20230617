# Comparing `tmp/llm-0.4.tar.gz` & `tmp/llm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-0.4.tar", last modified: Sat Jun 17 08:47:04 2023, max compression
+gzip compressed data, was "llm-0.4.1.tar", last modified: Sat Jun 17 21:41:31 2023, max compression
```

## Comparing `llm-0.4.tar` & `llm-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-17 08:46:44.000000 llm-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-17 08:47:04.872565 llm-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-17 08:46:44.000000 llm-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 08:46:44.000000 llm-0.4/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 08:46:44.000000 llm-0.4/llm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-06-17 08:46:44.000000 llm-0.4/llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-17 08:46:44.000000 llm-0.4/llm/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 08:47:04.872565 llm-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-17 08:46:44.000000 llm-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-17 08:46:44.000000 llm-0.4/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-17 08:46:44.000000 llm-0.4/tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 08:46:44.000000 llm-0.4/tests/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-17 08:46:44.000000 llm-0.4/tests/test_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-17 21:41:16.000000 llm-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-17 21:41:31.631900 llm-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-17 21:41:16.000000 llm-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 21:41:16.000000 llm-0.4.1/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 21:41:16.000000 llm-0.4.1/llm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-17 21:41:16.000000 llm-0.4.1/llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-17 21:41:16.000000 llm-0.4.1/llm/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 21:41:31.631900 llm-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-17 21:41:16.000000 llm-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_templates.py
```

### Comparing `llm-0.4/LICENSE` & `llm-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-0.4/PKG-INFO` & `llm-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.4
+Version: 0.4.1
 Summary: Access large language models from the command-line
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
-Project-URL: Documentation, https://llm.datasette.io/
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
 Project-URL: Changelog, https://github.com/simonw/llm/releases
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# llm
+# LLM
 
 [![PyPI](https://img.shields.io/pypi/v/llm.svg)](https://pypi.org/project/llm/)
-[![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://github.com/simonw/llm/releases)
+[![Documentation](https://readthedocs.org/projects/llm/badge/?version=latest)](https://llm.datasette.io/)
+[![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://llm.datasette.io/en/stable/changelog.html)
 [![Tests](https://github.com/simonw/llm/workflows/Test/badge.svg)](https://github.com/simonw/llm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm/blob/master/LICENSE)
 
 Access large language models from the command-line
 
+Full documentation: **[llm.datasette.io](https://llm.datasette.io/)**
+
 See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
 
 ## Installation
 
 Install this tool using `pip`:
 
     pip install llm
 
-[Detailed installation instructions](https://llm.datasette.io/en/stable/installation.html).
+Or using [Homebrew](https://brew.sh/):
+
+    brew install simonw/llm/llm
+
+[Detailed installation instructions](https://llm.datasette.io/en/stable/setup.html).
 
 ## Getting started
 
 First, create an OpenAI API key and save it to the tool like this:
 
 ```
 llm keys set openai
@@ -54,15 +60,15 @@
 ```
 1. Waddles
 2. Pebbles
 3. Bubbles
 4. Flappy
 5. Chilly
 ```
-Read the [usage instructions](https://llm.datasette.io/en/stable/usage.html) for more.
+Read the [usage instructions](https://llm.datasette.io/en/latest/usage.html) for more.
 
 ## Help
 
 For help, run:
 
     llm --help
```

### Comparing `llm-0.4/README.md` & `llm-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-# llm
+# LLM
 
 [![PyPI](https://img.shields.io/pypi/v/llm.svg)](https://pypi.org/project/llm/)
-[![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://github.com/simonw/llm/releases)
+[![Documentation](https://readthedocs.org/projects/llm/badge/?version=latest)](https://llm.datasette.io/)
+[![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://llm.datasette.io/en/stable/changelog.html)
 [![Tests](https://github.com/simonw/llm/workflows/Test/badge.svg)](https://github.com/simonw/llm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm/blob/master/LICENSE)
 
 Access large language models from the command-line
 
+Full documentation: **[llm.datasette.io](https://llm.datasette.io/)**
+
 See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
 
 ## Installation
 
 Install this tool using `pip`:
 
     pip install llm
 
-[Detailed installation instructions](https://llm.datasette.io/en/stable/installation.html).
+Or using [Homebrew](https://brew.sh/):
+
+    brew install simonw/llm/llm
+
+[Detailed installation instructions](https://llm.datasette.io/en/stable/setup.html).
 
 ## Getting started
 
 First, create an OpenAI API key and save it to the tool like this:
 
 ```
 llm keys set openai
@@ -38,15 +45,15 @@
 ```
 1. Waddles
 2. Pebbles
 3. Bubbles
 4. Flappy
 5. Chilly
 ```
-Read the [usage instructions](https://llm.datasette.io/en/stable/usage.html) for more.
+Read the [usage instructions](https://llm.datasette.io/en/latest/usage.html) for more.
 
 ## Help
 
 For help, run:
 
     llm --help
```

### Comparing `llm-0.4/llm/__init__.py` & `llm-0.4.1/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-0.4/llm/cli.py` & `llm-0.4.1/llm/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,15 +288,22 @@
 def templates_list():
     "List available prompt templates"
     path = template_dir()
     pairs = []
     for file in path.glob("*.yaml"):
         name = file.stem
         template = load_template(name)
-        pairs.append((name, template.prompt or ""))
+        text = []
+        if template.system:
+            text.append(f"system: {template.system}")
+            if template.prompt:
+                text.append(f" prompt: {template.prompt}")
+        else:
+            text = [template.prompt]
+        pairs.append((name, "".join(text).replace("\n", " ")))
     max_name_len = max(len(p[0]) for p in pairs)
     fmt = "{name:<" + str(max_name_len) + "} : {prompt}"
     for name, prompt in sorted(pairs):
         text = fmt.format(name=name, prompt=prompt)
         click.echo(display_truncated(text))
```

### Comparing `llm-0.4/llm/migrations.py` & `llm-0.4.1/llm/migrations.py`

 * *Files identical despite different names*

### Comparing `llm-0.4/llm.egg-info/PKG-INFO` & `llm-0.4.1/llm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.4
+Version: 0.4.1
 Summary: Access large language models from the command-line
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
-Project-URL: Documentation, https://llm.datasette.io/
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
 Project-URL: Changelog, https://github.com/simonw/llm/releases
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# llm
+# LLM
 
 [![PyPI](https://img.shields.io/pypi/v/llm.svg)](https://pypi.org/project/llm/)
-[![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://github.com/simonw/llm/releases)
+[![Documentation](https://readthedocs.org/projects/llm/badge/?version=latest)](https://llm.datasette.io/)
+[![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://llm.datasette.io/en/stable/changelog.html)
 [![Tests](https://github.com/simonw/llm/workflows/Test/badge.svg)](https://github.com/simonw/llm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm/blob/master/LICENSE)
 
 Access large language models from the command-line
 
+Full documentation: **[llm.datasette.io](https://llm.datasette.io/)**
+
 See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
 
 ## Installation
 
 Install this tool using `pip`:
 
     pip install llm
 
-[Detailed installation instructions](https://llm.datasette.io/en/stable/installation.html).
+Or using [Homebrew](https://brew.sh/):
+
+    brew install simonw/llm/llm
+
+[Detailed installation instructions](https://llm.datasette.io/en/stable/setup.html).
 
 ## Getting started
 
 First, create an OpenAI API key and save it to the tool like this:
 
 ```
 llm keys set openai
@@ -54,15 +60,15 @@
 ```
 1. Waddles
 2. Pebbles
 3. Bubbles
 4. Flappy
 5. Chilly
 ```
-Read the [usage instructions](https://llm.datasette.io/en/stable/usage.html) for more.
+Read the [usage instructions](https://llm.datasette.io/en/latest/usage.html) for more.
 
 ## Help
 
 For help, run:
 
     llm --help
```

### Comparing `llm-0.4/setup.py` & `llm-0.4.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4"
+VERSION = "0.4.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -16,15 +16,14 @@
     name="llm",
     description="Access large language models from the command-line",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Simon Willison",
     url="https://github.com/simonw/llm",
     project_urls={
-        "Documentation": "https://llm.datasette.io/",
         "Issues": "https://github.com/simonw/llm/issues",
         "CI": "https://github.com/simonw/llm/actions",
         "Changelog": "https://github.com/simonw/llm/releases",
     },
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["llm"],
```

### Comparing `llm-0.4/tests/test_keys.py` & `llm-0.4.1/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `llm-0.4/tests/test_llm.py` & `llm-0.4.1/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `llm-0.4/tests/test_migrate.py` & `llm-0.4.1/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `llm-0.4/tests/test_templates.py` & `llm-0.4.1/tests/test_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,19 +32,29 @@
 
 def test_templates_list(templates_path):
     (templates_path / "one.yaml").write_text("template one", "utf-8")
     (templates_path / "two.yaml").write_text("template two", "utf-8")
     (templates_path / "three.yaml").write_text(
         "template three is very long " * 4, "utf-8"
     )
+    (templates_path / "four.yaml").write_text(
+        "'this one\n\nhas newlines in it'", "utf-8"
+    )
+    (templates_path / "both.yaml").write_text(
+        "system: summarize this\nprompt: $input", "utf-8"
+    )
+    (templates_path / "sys.yaml").write_text("system: Summarize this", "utf-8")
     runner = CliRunner()
     result = runner.invoke(cli, ["templates", "list"])
     assert result.exit_code == 0
     assert result.output == (
+        "both  : system: summarize this prompt: $input\n"
+        "four  : this one has newlines in it\n"
         "one   : template one\n"
+        "sys   : system: Summarize this\n"
         "three : template three is very long template three is very long template thre...\n"
         "two   : template two\n"
     )
 
 
 @mock.patch.dict(os.environ, {"OPENAI_API_KEY": "X"})
 @pytest.mark.parametrize(
```

