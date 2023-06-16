# Comparing `tmp/gitmopy-0.2.0.tar.gz` & `tmp/gitmopy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.2.0.tar", max compression
+gzip compressed data, was "gitmopy-0.3.0.tar", max compression
```

## Comparing `gitmopy-0.2.0.tar` & `gitmopy-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-06-14 14:26:54.760147 gitmopy-0.2.0/LICENSE
--rw-r--r--   0        0        0     3933 2023-06-15 02:01:47.793731 gitmopy-0.2.0/README.md
--rw-r--r--   0        0        0       73 2023-06-14 23:40:00.987257 gitmopy-0.2.0/gitmopy/__init__.py
--rw-r--r--   0        0        0     6968 2023-06-15 02:01:47.796240 gitmopy-0.2.0/gitmopy/cli.py
--rw-r--r--   0        0        0     3655 2023-06-15 02:01:47.796721 gitmopy-0.2.0/gitmopy/history.py
--rw-r--r--   0        0        0     7161 2023-06-15 02:01:47.797318 gitmopy-0.2.0/gitmopy/prompt.py
--rw-r--r--   0        0        0    18938 2023-06-15 02:01:47.797724 gitmopy-0.2.0/gitmopy/utils.py
--rw-r--r--   0        0        0      572 2023-06-15 02:01:47.798925 gitmopy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4833 1970-01-01 00:00:00.000000 gitmopy-0.2.0/setup.py
--rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 gitmopy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 14:26:54.760147 gitmopy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6463 2023-06-16 20:29:37.545684 gitmopy-0.3.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.0/gitmopy/__init__.py
+-rw-r--r--   0        0        0    11998 2023-06-16 20:28:22.684270 gitmopy-0.3.0/gitmopy/cli.py
+-rw-r--r--   0        0        0     3434 2023-06-16 19:39:04.305856 gitmopy-0.3.0/gitmopy/git.py
+-rw-r--r--   0        0        0     2989 2023-06-16 20:28:43.708911 gitmopy-0.3.0/gitmopy/history.py
+-rw-r--r--   0        0        0     8032 2023-06-16 19:39:04.307150 gitmopy-0.3.0/gitmopy/prompt.py
+-rw-r--r--   0        0        0    19754 2023-06-16 19:39:04.307687 gitmopy-0.3.0/gitmopy/utils.py
+-rw-r--r--   0        0        0      578 2023-06-16 19:59:45.699347 gitmopy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7429 1970-01-01 00:00:00.000000 gitmopy-0.3.0/setup.py
+-rw-r--r--   0        0        0     7091 1970-01-01 00:00:00.000000 gitmopy-0.3.0/PKG-INFO
```

### Comparing `gitmopy-0.2.0/LICENSE` & `gitmopy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.2.0/gitmopy/prompt.py` & `gitmopy-0.3.0/gitmopy/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,42 @@
+"""
+Module handling user prompts.
+
+Prompts typically parameterize the commit message or ``gitmopy``'s behavior.
+"""
+
 from typing import Any, Dict, List, Optional
 
 from InquirerPy import inquirer
-from InquirerPy.base.control import Choice, Separator
+from InquirerPy.base.control import Choice
 from prompt_toolkit.completion import Completer, Completion
 from prompt_toolkit.document import Document
 
 from gitmopy import history as gmp_history
-from gitmopy.utils import APP_PATH, DEFAULT_CHOICES, GITMOJIS, load_config, save_config
+from gitmopy.utils import (
+    APP_PATH,
+    DEFAULT_CHOICES,
+    GITMOJIS,
+    load_config,
+    save_config,
+    separator,
+)
 
 
 class GMPCompleter(Completer):
     def __init__(self, key: str, max_results: Optional[int] = 10):
         """
         A completer that completes a text prompt from the user's history.
+
         Completions are sorted by most recent first.
         Returns up to ``self.max_results`` results.
 
         Args:
             key (str): Key to complete from. Must be one of "scope", "title", "message".
+            max_results (int): Maximum number of results to return. Defaults to 10.
         """
         self.key = key
         self.max_results = max_results
         self.candidates = {}
         for c in gmp_history.HISTORY:
             if c[key] not in self.candidates:
                 self.candidates[c[key]] = c["timestamp"]
@@ -57,33 +72,28 @@
         )
         for m in matched[: self.max_results]:
             yield Completion(m[0], start_position=-len(document.text))
 
 
 def commit_prompt(config: Dict[str, bool]) -> Dict[str, str]:
     """
-    Prompt the user for a commit message in up to 4 steps:
-    - Select gitmoji
-    - Select scope
-    - Enter title
-    - Enter message
+    Prompt the user for emoji, scope title and message to make a commit message.
 
     Scope and message are optional.
     Scope and message can be bypassed from the config (run ``gitmopy config``)
     Scope, title and message are completed from the user's history if
         ``config["enable_history"]`` is ``True``.
 
     Args:
         config (dict): Configuration dictionary, from ``gitmopy config``.
 
     Returns:
         dict: User-specified commit as a dict with keys
             ``"emoji"``, ``"scope"``, ``"title"``, ``"message"``.
     """
-
     # get the commit's gitmoji
     emoji = (
         inquirer.fuzzy(
             message="Select gitmoji:",
             choices=GITMOJIS,
             multiselect=False,
             max_height="70%",
@@ -154,14 +164,15 @@
         "message": message,
     }
 
 
 def config_prompt() -> None:
     """
     Prompt the user for configuration options.
+
     Will setup:
     - Whether to skip scope
     - Whether to skip message
     - Whether to capitalize title
     - Whether to enable history
 
     Will save the configuration in ``${APP_PATH}/config.yaml``.
@@ -203,20 +214,23 @@
     Args:
         status (dict): Dictionary of files grouped by status.
 
     Returns:
         list: List of all the files selected by the user.
     """
     choices = []
+    if len(status["unstaged"]) > 0:
+        choices.append(separator("Unstaged files"))
     for s in status["unstaged"]:
-        choices.append(Choice(s, f"{s} -- unstaged", True))
-    if len(choices) > 0:
-        choices.append(Separator())
+        choices.append(Choice(s, s, True))
+
+    if len(status["untracked"]) > 0:
+        choices.append(separator("Untracked files"))
     for s in status["untracked"]:
-        choices.append(Choice(s, f"{s} -- untracked", True))
+        choices.append(Choice(s, s, True))
 
     selected = inquirer.checkbox(
         message="Select files to add for the commit.",
         instruction="Use 'space' to (de-)select, 'enter' to validate.",
         choices=choices,
         cycle=True,
         transformer=lambda result: "",
@@ -224,19 +238,46 @@
         amark="✓",
     ).execute()
 
     return selected
 
 
 def choose_remote_prompt(remotes: List[str]) -> List[str]:
+    """
+    Prompt the user to select remotes to push to.
+
+    Args:
+        remotes (List[str]): Available remotes.
+
+    Returns:
+        List[str]: Selected remotes.
+    """
     choices = [Choice(r.name, r.name, True) for r in remotes]
     selected = inquirer.checkbox(
         "Select remotes to push to:",
         instruction="Use 'space' to (de-)select, 'enter' to validate.",
         choices=choices,
         cycle=True,
         qmark="❓",
         amark="✓",
         transformer=lambda result: "Pushing to " + ", ".join(result),
     ).execute()
 
     return selected
+
+
+def set_upstream_prompt(remote_name: str) -> bool:
+    """
+    Prompt the user to set the upstream branch for a remote.
+
+    Args:
+        remote_name (str): Remote name.
+
+    Returns:
+        bool: Whether or not to set the upstream branch.
+    """
+    return inquirer.confirm(
+        f"Do you want to set the upstream branch for '{remote_name}' now?",
+        qmark="❓",
+        amark="✓",
+        default=True,
+    ).execute()
```

### Comparing `gitmopy-0.2.0/gitmopy/utils.py` & `gitmopy-0.3.0/gitmopy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+"""
+Utility functions and constants for ``gitmopy``.
+"""
 from os.path import expandvars
 from pathlib import Path
 from typing import Dict, List, Union
 
 import typer
 from rich import print
 from yaml import safe_dump, safe_load
+from InquirerPy.separator import Separator
 
 
 def resolve_path(path: Union[str, Path]) -> Path:
     """
     Resolve a path with ``expandvars``, ``expanduser`` and ``resolve``.
 
     Args:
@@ -66,28 +70,30 @@
 Default gitmopy configuration.
 """
 
 
 def load_config() -> Dict[str, bool]:
     """
     Load the configuration from ``${APP_PATH}/config.yaml``.
+
     Returns the default configuration if the file does not exist.
 
     Returns:
         Dict[str, bool]: User gitmopy configuration.
     """
     yaml_path = APP_PATH / "config.yaml"
     if yaml_path.exists():
         return {**DEFAULT_CONFIG, **safe_load(yaml_path.read_text())}
     return DEFAULT_CONFIG
 
 
 def save_config(config: Dict[str, bool]) -> None:
     """
     Save the configuration to ``${APP_PATH}/config.yaml``.
+
     Creates the parent directory if it does not exist.
 
     Args:
         config (Dict[str, bool]): Current gitmopy configuration.
     """
     yaml_path = APP_PATH / "config.yaml"
     if not yaml_path.exists():
@@ -108,15 +114,15 @@
     s = "" if nst == 1 else "s"
     print(f"[green3]Currently {nst} staged file{s} for commit:[/green3]")
     for f in staged:
         print(f"  [grey66]- {f}[/grey66]")
 
 
 def message_from_commit_dict(commit_dict: Dict[str, str]) -> str:
-    """
+    r"""
     Create a commit message from a commit dictionary.
 
     Depending on whether ``scope`` is set, will look like
 
     * ``{emoji} ({scope}): {title}``
     * ``{emoji}: {title}``
 
@@ -132,14 +138,37 @@
     message = f"{commit_dict['emoji']} "
     if commit_dict["scope"]:
         message += f"({commit_dict['scope']}): "
     message += f"{commit_dict['title']}\n\n{commit_dict['message']}"
     return message.strip()
 
 
+def separator(title: str = "", width: int = 30, sep: str = "-") -> Separator:
+    """
+    Create an InquirerPy separator with a title.
+
+    Args:
+        title (str, optional): Title in-between separator characters.
+            Defaults to ``""``.
+        width (int, optional): Total length of sperator line. Defaults to 30.
+        sep (str, optional): Character to use around the ``title``. Defaults to ``"-"``.
+
+    Returns:
+        Separator: _description_
+    """
+    assert sep
+    assert width > 0
+    if len(title) > width - 4:
+        width = len(title) + 4
+
+    first = (width - len(title)) // 2
+    line = f"{sep * first} {title} {sep * (width - first - len(title) - 2)}"
+    return Separator(line)
+
+
 # https://github.com/carloscuesta/gitmoji/blob/master/packages/gitmojis/src/gitmojis.json
 GITMOJIS = [
     {
         "emoji": "🎨",
         "entity": "&#x1f3a8;",
         "code": ":art:",
         "description": "Improve structure / format of the code.",
```

### Comparing `gitmopy-0.2.0/pyproject.toml` & `gitmopy-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.2.0"
+version = "0.3.0"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-emoji = "^2.5.0"
 GitPython = "^3.1.31"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = ">=0.8.0"}
 pyyaml = "^6.0"
 inquirerpy = "^0.3.4"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 ipython = "^8.14.0"
+pydocstyle = "^6.3.0"
 
 [tool.poetry.scripts]
 gitmopy = "gitmopy.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

