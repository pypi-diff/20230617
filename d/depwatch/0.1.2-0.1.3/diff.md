# Comparing `tmp/depwatch-0.1.2.tar.gz` & `tmp/depwatch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depwatch-0.1.2.tar", last modified: Fri Apr  7 00:06:06 2023, max compression
+gzip compressed data, was "depwatch-0.1.3.tar", last modified: Sat Jun 17 04:32:49 2023, max compression
```

## Comparing `depwatch-0.1.2.tar` & `depwatch-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-04-07 00:05:48.622200 depwatch-0.1.2/LICENSE
--rw-r--r--   0        0        0     2071 2023-04-07 00:05:48.622200 depwatch-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/__init__.py
--rw-r--r--   0        0        0      689 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/command.py
--rw-r--r--   0        0        0     1568 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/deployment.py
--rw-r--r--   0        0        0       45 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/exception.py
--rw-r--r--   0        0        0     2047 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/history.py
--rw-r--r--   0        0        0      519 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/main.py
--rw-r--r--   0        0        0     1293 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/repository.py
--rw-r--r--   0        0        0      731 2023-04-07 00:05:48.622200 depwatch-0.1.2/depwatch/writer.py
--rw-r--r--   0        0        0     1209 2023-04-07 00:05:48.622200 depwatch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 00:05:48.622200 depwatch-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1631 2023-04-07 00:05:48.626200 depwatch-0.1.2/tests/test_command.py
--rw-r--r--   0        0        0     4466 2023-04-07 00:05:48.626200 depwatch-0.1.2/tests/test_deployment.py
--rw-r--r--   0        0        0     2837 2023-04-07 00:05:48.626200 depwatch-0.1.2/tests/test_history.py
--rw-r--r--   0        0        0     3217 2023-04-07 00:05:48.626200 depwatch-0.1.2/tests/test_repository.py
--rw-r--r--   0        0        0     1820 2023-04-07 00:05:48.626200 depwatch-0.1.2/tests/test_writer.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 depwatch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-17 04:32:33.281063 depwatch-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2071 2023-06-17 04:32:33.281063 depwatch-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 04:32:33.281063 depwatch-0.1.3/depwatch/__init__.py
+-rw-r--r--   0        0        0     1046 2023-06-17 04:32:33.281063 depwatch-0.1.3/depwatch/command.py
+-rw-r--r--   0        0        0     1553 2023-06-17 04:32:33.281063 depwatch-0.1.3/depwatch/date_utils.py
+-rw-r--r--   0        0        0     1356 2023-06-17 04:32:33.285063 depwatch-0.1.3/depwatch/deployment.py
+-rw-r--r--   0        0        0       45 2023-06-17 04:32:33.285063 depwatch-0.1.3/depwatch/exception.py
+-rw-r--r--   0        0        0     3379 2023-06-17 04:32:33.285063 depwatch-0.1.3/depwatch/history.py
+-rw-r--r--   0        0        0     1006 2023-06-17 04:32:33.285063 depwatch-0.1.3/depwatch/main.py
+-rw-r--r--   0        0        0     1919 2023-06-17 04:32:33.285063 depwatch-0.1.3/depwatch/repository.py
+-rw-r--r--   0        0        0      731 2023-06-17 04:32:33.285063 depwatch-0.1.3/depwatch/writer.py
+-rw-r--r--   0        0        0     1180 2023-06-17 04:32:33.285063 depwatch-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2126 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_command.py
+-rw-r--r--   0        0        0     1387 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_date_utils.py
+-rw-r--r--   0        0        0     3256 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_deployment.py
+-rw-r--r--   0        0        0    16701 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_history.py
+-rw-r--r--   0        0        0     1296 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_main.py
+-rw-r--r--   0        0        0     6444 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_repository.py
+-rw-r--r--   0        0        0     1820 2023-06-17 04:32:33.285063 depwatch-0.1.3/tests/test_writer.py
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 depwatch-0.1.3/PKG-INFO
```

### Comparing `depwatch-0.1.2/LICENSE` & `depwatch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `depwatch-0.1.2/README.md` & `depwatch-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `depwatch-0.1.2/depwatch/command.py` & `depwatch-0.1.3/depwatch/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 from dotenv import load_dotenv
+from depwatch.date_utils import DateRange
 
-from depwatch.history import create_histories
+from depwatch.history import (
+    convert_repository_history_to_workflow_ids,
+    create_histories,
+)
 from depwatch.repository import get_main_branch, get_repository_history
 from depwatch.deployment import get_deployment_history
 from depwatch.writer import write_histories
 
 
-def generate_histories(name: str, code_only: bool, limit: int):
+def generate_histories(
+    name: str,
+    code_only: bool,
+    limit: int,
+    created_at: DateRange | None = None,
+    workflow_name: str | None = None,
+) -> None:
     load_dotenv()
 
     base = get_main_branch(name)
 
-    repository_histories = get_repository_history(name, base, limit)
+    repository_histories = get_repository_history(name, base, limit, created_at)
 
     # CircleCI
     deployment_histories = []
     if not code_only:
-        deployment_histories = get_deployment_history(name, base, limit)
+        workflow_ids = convert_repository_history_to_workflow_ids(
+            repository_histories, workflow_name
+        )
+        deployment_histories = get_deployment_history(workflow_ids)
 
     write_histories(
-        "output.csv", create_histories(repository_histories, deployment_histories)
+        "output.csv",
+        create_histories(repository_histories, deployment_histories, workflow_name),
     )
```

### Comparing `depwatch-0.1.2/depwatch/writer.py` & `depwatch-0.1.3/depwatch/writer.py`

 * *Files identical despite different names*

### Comparing `depwatch-0.1.2/pyproject.toml` & `depwatch-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "depwatch"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Simple command-line tool for collecting the times of various events in a project's lifecycle"
 authors = [
     { name = "hamakou108", email = "hamakou108@gmail.com" },
 ]
 dependencies = [
-    "typer[all]>=0.7.0",
-    "PyGithub>=1.58.0",
-    "python-dotenv>=0.21.1",
-    "pycircleci>=0.6.1",
-    "requests>=2.28.2",
-    "types-requests>=2.28.11.15",
+    "typer[all]>=0.9",
+    "PyGithub>=1.58",
+    "python-dotenv>=1.0",
+    "pycircleci>=0.7",
+    "requests>=2.31",
+    "types-requests>=2.31",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
@@ -23,22 +23,22 @@
 text = "MIT"
 
 [project.scripts]
 depwatch = "depwatch.main:main_cli"
 
 [tool.pdm.dev-dependencies]
 test = [
-    "pytest>=7.2.1",
-    "pytest-mock>=3.10.0",
+    "pytest>=7.3",
+    "pytest-mock>=3.10",
 ]
 linter = [
-    "mypy>=1.0.1",
-    "flake8>=6.0.0",
-    "Flake8-pyproject>=1.2.2",
-    "black>=23.1.0",
+    "mypy>=1.3",
+    "flake8>=6.0",
+    "Flake8-pyproject>=1.2",
+    "black>=23.3",
 ]
 
 [tool.pdm.scripts]
 check_type = "mypy depwatch tests"
 check_lint = "flake8 depwatch tests"
 check_format = "black --check depwatch tests"
 test = "pytest tests"
```

### Comparing `depwatch-0.1.2/tests/test_command.py` & `depwatch-0.1.3/tests/test_command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 from unittest.mock import patch, Mock
 
 from depwatch import command
 from depwatch.command import generate_histories
+from depwatch.date_utils import DateRange
 
 
 class TestCommand:
     @patch.object(command, "write_histories")
     @patch.object(command, "get_deployment_history", return_value=[])
+    @patch.object(
+        command, "convert_repository_history_to_workflow_ids", return_value=[]
+    )
     @patch.object(command, "get_repository_history", return_value=[])
     @patch.object(command, "get_main_branch", return_value="main")
     def test_generate_histories(
         self,
         get_main_branch_mock: Mock,
         get_repository_history_mock: Mock,
+        convert_repository_history_to_workflow_ids_mock: Mock,
         get_deployment_history_mock: Mock,
         write_histories_mock: Mock,
     ):
-        generate_histories("hamakou108/my_project", False, 100)
+        generate_histories(
+            "hamakou108/my_project",
+            False,
+            100,
+            DateRange.from_str("2023-01-01..2023-03-31"),
+            "workflow",
+        )
 
         get_main_branch_mock.assert_called_once_with("hamakou108/my_project")
         get_repository_history_mock.assert_called_once_with(
-            "hamakou108/my_project", "main", 100
+            "hamakou108/my_project",
+            "main",
+            100,
+            DateRange.from_str("2023-01-01..2023-03-31"),
         )
-        get_deployment_history_mock.assert_called_once_with(
-            "hamakou108/my_project", "main", 100
+        convert_repository_history_to_workflow_ids_mock.assert_called_once_with(
+            [], "workflow"
         )
+        get_deployment_history_mock.assert_called_once_with([])
         write_histories_mock.assert_called()
 
     @patch.object(command, "write_histories")
     @patch.object(command, "get_deployment_history", return_value=[])
     @patch.object(command, "get_repository_history", return_value=[])
     @patch.object(command, "get_main_branch", return_value="main")
     def test_generate_histories_with_code_only(
         self,
         get_main_branch_mock: Mock,
         get_repository_history_mock: Mock,
         get_deployment_history_mock: Mock,
         write_histories_mock: Mock,
     ):
-        generate_histories("hamakou108/my_project", True, 100)
+        generate_histories("hamakou108/my_project", True, 100, None, None)
 
         get_deployment_history_mock.assert_not_called()
```

### Comparing `depwatch-0.1.2/tests/test_writer.py` & `depwatch-0.1.3/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `depwatch-0.1.2/PKG-INFO` & `depwatch-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depwatch
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Simple command-line tool for collecting the times of various events in a project's lifecycle
 License: MIT
 Author-email: hamakou108 <hamakou108@gmail.com>
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

