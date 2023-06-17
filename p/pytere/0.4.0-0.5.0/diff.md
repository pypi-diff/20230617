# Comparing `tmp/pytere-0.4.0.tar.gz` & `tmp/pytere-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytere-0.4.0.tar", last modified: Wed Jan 25 15:07:54 2023, max compression
+gzip compressed data, was "pytere-0.5.0.tar", last modified: Sat Jun 17 11:27:19 2023, max compression
```

## Comparing `pytere-0.4.0.tar` & `pytere-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 15:07:54.730461 pytere-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-25 15:07:45.000000 pytere-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-01-25 15:07:54.730461 pytere-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-25 15:07:45.000000 pytere-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-25 15:07:45.000000 pytere-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 15:07:54.730461 pytere-0.4.0/pytere/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-25 15:07:45.000000 pytere-0.4.0/pytere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 15:07:54.730461 pytere-0.4.0/pytere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-01-25 15:07:54.000000 pytere-0.4.0/pytere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-25 15:07:54.000000 pytere-0.4.0/pytere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 15:07:54.000000 pytere-0.4.0/pytere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-25 15:07:54.000000 pytere-0.4.0/pytere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-25 15:07:54.000000 pytere-0.4.0/pytere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 15:07:54.730461 pytere-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-25 15:07:45.000000 pytere-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:27:19.250197 pytere-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-17 11:27:17.000000 pytere-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-17 11:27:19.250197 pytere-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-17 11:27:17.000000 pytere-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-17 11:27:17.000000 pytere-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:27:19.246197 pytere-0.5.0/pytere/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-17 11:27:17.000000 pytere-0.5.0/pytere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:27:19.250197 pytere-0.5.0/pytere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-17 11:27:19.000000 pytere-0.5.0/pytere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-17 11:27:19.000000 pytere-0.5.0/pytere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:27:19.000000 pytere-0.5.0/pytere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-17 11:27:19.000000 pytere-0.5.0/pytere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 11:27:19.000000 pytere-0.5.0/pytere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 11:27:19.250197 pytere-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-17 11:27:17.000000 pytere-0.5.0/setup.py
```

### Comparing `pytere-0.4.0/LICENSE` & `pytere-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytere-0.4.0/PKG-INFO` & `pytere-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytere
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python Template Repository
 Home-page: https://github.com/astariul/pytere
 Author: Nicolas REMOND
 Author-email: remondnicola@gmail.com
 License: UNKNOWN
 Description: <h1 align="center">pytere</h1>
         <p align="center">
@@ -14,18 +14,16 @@
         <p align="center">
             <a href="https://github.com/astariul/pytere/releases"><img src="https://img.shields.io/github/release/astariul/pytere.svg" alt="GitHub release" /></a>
             <a href="https://github.com/astariul/pytere/actions/workflows/pytest.yaml"><img src="https://github.com/astariul/pytere/actions/workflows/pytest.yaml/badge.svg" alt="Test status" /></a>
             <a href="https://github.com/astariul/pytere/actions/workflows/lint.yaml"><img src="https://github.com/astariul/pytere/actions/workflows/lint.yaml/badge.svg" alt="Lint status" /></a>
             <img src=".github/badges/coverage.svg" alt="Coverage status" />
             <a href="https://astariul.github.io/pytere"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https%3A%2F%2Fastariul.github.io%2Fpytere" alt="Docs" /></a>
             <br>
-            <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat" alt="isort" /></a>
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" /></a>
-            <a href="https://github.com/PyCQA/flake8"><img src="https://img.shields.io/badge/code%20style-flake8-blue" alt="flake8" /></a>
-            <a href="https://github.com/terrencepreilly/darglint"><img src="https://img.shields.io/badge/docstrings-darglint-blue" alt="darglint" /></a>
+            <a href="https://github.com/astral-sh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff" /></a>
             <a href="https://github.com/pre-commit/pre-commit"><img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white" alt="pre-commit"></a>
             <a href="https://github.com/astariul/pytere/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
         </p>
         
         <p align="center">
           <a href="#description">Description</a> •
           <a href="#install">Install</a> •
@@ -41,15 +39,15 @@
         <h2 align="center">Description</h2>
         
         **`pytere`** stands for **Py**thon **te**mplate **re**pository.
         
         It's just a template repository for python, with the following features :
         
         * 📚 Beautiful documentation with [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/), published as a Github page with [mike](https://github.com/jimporter/mike) automatically
-        * ✨ Code style checks with [isort](https://github.com/PyCQA/isort), [black](https://github.com/psf/black), [flake518](https://github.com/carstencodes/flake518), [darglint](https://github.com/terrencepreilly/darglint)
+        * ✨ Modern code style checks with [black](https://github.com/psf/black) and [ruff](https://github.com/astral-sh/ruff)
         * 🅿️ Easy development with [pre-commit hooks](https://pre-commit.com/)
         * ✅ Tests with [pytest](https://docs.pytest.org/) and coverage without external tools
         * :octocat: CI with [Github actions](https://github.com/features/actions)
         * 📝 Issues & PR templates
         * 🤖 Stale bot & Dependabot
         * 🚀 Releases automatically published to PyPi
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: pytere Version: 0.4.0 Summary: A Python Template
+Metadata-Version: 2.1 Name: pytere Version: 0.5.0 Summary: A Python Template
 Repository Home-page: https://github.com/astariul/pytere Author: Nicolas REMOND
 Author-email: remondnicola@gmail.com License: UNKNOWN Description:
                              ****** pytere ******
                           Python Template repository
     [GitHub_release] [Test_status] [Lint_status] [Coverage status] [Docs]
-          [isort] [black] [flake8] [darglint] [pre-commit] [licence]
+                     [black] [ruff] [pre-commit] [licence]
 Description â¢ Install â¢ Usage â¢ Use_this_template â¢ FAQ â¢ Contribute
                                  Documentation
                             ***** Description *****
 **`pytere`** stands for **Py**thon **te**mplate **re**pository. It's just a
 template repository for python, with the following features : * ð Beautiful
 documentation with [Material for Mkdocs](https://squidfunk.github.io/mkdocs-
 material/), published as a Github page with [mike](https://github.com/
-jimporter/mike) automatically * â¨ Code style checks with [isort](https://
-github.com/PyCQA/isort), [black](https://github.com/psf/black), [flake518]
-(https://github.com/carstencodes/flake518), [darglint](https://github.com/
-terrencepreilly/darglint) * ð¿ï¸ Easy development with [pre-commit hooks]
-(https://pre-commit.com/) * â Tests with [pytest](https://docs.pytest.org/
-) and coverage without external tools * :octocat: CI with [Github actions]
-(https://github.com/features/actions) * ð Issues & PR templates * ð¤ Stale
-bot & Dependabot * ð Releases automatically published to PyPi
+jimporter/mike) automatically * â¨ Modern code style checks with [black]
+(https://github.com/psf/black) and [ruff](https://github.com/astral-sh/ruff) *
+ð¿ï¸ Easy development with [pre-commit hooks](https://pre-commit.com/) * â
+Tests with [pytest](https://docs.pytest.org/) and coverage without external
+tools * :octocat: CI with [Github actions](https://github.com/features/actions)
+* ð Issues & PR templates * ð¤ Stale bot & Dependabot * ð Releases
+automatically published to PyPi
                               ***** Install *****
 Install `pytere` by running : ``` pip install pytere ``` --- For development,
 you can install it locally by first cloning the repository : ``` git clone
 https://github.com/astariul/pytere.git cd pytere pip install -e . ```
                                ***** Usage *****
 `pytere` does not contain any useful code because it's a template repository.
 But you can check if the package is correctly installed with : ```python from
```

### Comparing `pytere-0.4.0/README.md` & `pytere-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 <p align="center">
     <a href="https://github.com/astariul/pytere/releases"><img src="https://img.shields.io/github/release/astariul/pytere.svg" alt="GitHub release" /></a>
     <a href="https://github.com/astariul/pytere/actions/workflows/pytest.yaml"><img src="https://github.com/astariul/pytere/actions/workflows/pytest.yaml/badge.svg" alt="Test status" /></a>
     <a href="https://github.com/astariul/pytere/actions/workflows/lint.yaml"><img src="https://github.com/astariul/pytere/actions/workflows/lint.yaml/badge.svg" alt="Lint status" /></a>
     <img src=".github/badges/coverage.svg" alt="Coverage status" />
     <a href="https://astariul.github.io/pytere"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https%3A%2F%2Fastariul.github.io%2Fpytere" alt="Docs" /></a>
     <br>
-    <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat" alt="isort" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" /></a>
-    <a href="https://github.com/PyCQA/flake8"><img src="https://img.shields.io/badge/code%20style-flake8-blue" alt="flake8" /></a>
-    <a href="https://github.com/terrencepreilly/darglint"><img src="https://img.shields.io/badge/docstrings-darglint-blue" alt="darglint" /></a>
+    <a href="https://github.com/astral-sh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff" /></a>
     <a href="https://github.com/pre-commit/pre-commit"><img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white" alt="pre-commit"></a>
     <a href="https://github.com/astariul/pytere/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
 </p>
 
 <p align="center">
   <a href="#description">Description</a> •
   <a href="#install">Install</a> •
@@ -33,15 +31,15 @@
 <h2 align="center">Description</h2>
 
 **`pytere`** stands for **Py**thon **te**mplate **re**pository.
 
 It's just a template repository for python, with the following features :
 
 * 📚 Beautiful documentation with [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/), published as a Github page with [mike](https://github.com/jimporter/mike) automatically
-* ✨ Code style checks with [isort](https://github.com/PyCQA/isort), [black](https://github.com/psf/black), [flake518](https://github.com/carstencodes/flake518), [darglint](https://github.com/terrencepreilly/darglint)
+* ✨ Modern code style checks with [black](https://github.com/psf/black) and [ruff](https://github.com/astral-sh/ruff)
 * 🅿️ Easy development with [pre-commit hooks](https://pre-commit.com/)
 * ✅ Tests with [pytest](https://docs.pytest.org/) and coverage without external tools
 * :octocat: CI with [Github actions](https://github.com/features/actions)
 * 📝 Issues & PR templates
 * 🤖 Stale bot & Dependabot
 * 🚀 Releases automatically published to PyPi
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
                              ****** pytere ******
                           Python Template repository
     [GitHub_release] [Test_status] [Lint_status] [Coverage status] [Docs]
-          [isort] [black] [flake8] [darglint] [pre-commit] [licence]
+                     [black] [ruff] [pre-commit] [licence]
 Description â¢ Install â¢ Usage â¢ Use_this_template â¢ FAQ â¢ Contribute
                                  Documentation
                             ***** Description *****
 **`pytere`** stands for **Py**thon **te**mplate **re**pository. It's just a
 template repository for python, with the following features : * ð Beautiful
 documentation with [Material for Mkdocs](https://squidfunk.github.io/mkdocs-
 material/), published as a Github page with [mike](https://github.com/
-jimporter/mike) automatically * â¨ Code style checks with [isort](https://
-github.com/PyCQA/isort), [black](https://github.com/psf/black), [flake518]
-(https://github.com/carstencodes/flake518), [darglint](https://github.com/
-terrencepreilly/darglint) * ð¿ï¸ Easy development with [pre-commit hooks]
-(https://pre-commit.com/) * â Tests with [pytest](https://docs.pytest.org/
-) and coverage without external tools * :octocat: CI with [Github actions]
-(https://github.com/features/actions) * ð Issues & PR templates * ð¤ Stale
-bot & Dependabot * ð Releases automatically published to PyPi
+jimporter/mike) automatically * â¨ Modern code style checks with [black]
+(https://github.com/psf/black) and [ruff](https://github.com/astral-sh/ruff) *
+ð¿ï¸ Easy development with [pre-commit hooks](https://pre-commit.com/) * â
+Tests with [pytest](https://docs.pytest.org/) and coverage without external
+tools * :octocat: CI with [Github actions](https://github.com/features/actions)
+* ð Issues & PR templates * ð¤ Stale bot & Dependabot * ð Releases
+automatically published to PyPi
                               ***** Install *****
 Install `pytere` by running : ``` pip install pytere ``` --- For development,
 you can install it locally by first cloning the repository : ``` git clone
 https://github.com/astariul/pytere.git cd pytere pip install -e . ```
                                ***** Usage *****
 `pytere` does not contain any useful code because it's a template repository.
 But you can check if the package is correctly installed with : ```python from
```

### Comparing `pytere-0.4.0/pytere.egg-info/PKG-INFO` & `pytere-0.5.0/pytere.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytere
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python Template Repository
 Home-page: https://github.com/astariul/pytere
 Author: Nicolas REMOND
 Author-email: remondnicola@gmail.com
 License: UNKNOWN
 Description: <h1 align="center">pytere</h1>
         <p align="center">
@@ -14,18 +14,16 @@
         <p align="center">
             <a href="https://github.com/astariul/pytere/releases"><img src="https://img.shields.io/github/release/astariul/pytere.svg" alt="GitHub release" /></a>
             <a href="https://github.com/astariul/pytere/actions/workflows/pytest.yaml"><img src="https://github.com/astariul/pytere/actions/workflows/pytest.yaml/badge.svg" alt="Test status" /></a>
             <a href="https://github.com/astariul/pytere/actions/workflows/lint.yaml"><img src="https://github.com/astariul/pytere/actions/workflows/lint.yaml/badge.svg" alt="Lint status" /></a>
             <img src=".github/badges/coverage.svg" alt="Coverage status" />
             <a href="https://astariul.github.io/pytere"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https%3A%2F%2Fastariul.github.io%2Fpytere" alt="Docs" /></a>
             <br>
-            <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat" alt="isort" /></a>
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" /></a>
-            <a href="https://github.com/PyCQA/flake8"><img src="https://img.shields.io/badge/code%20style-flake8-blue" alt="flake8" /></a>
-            <a href="https://github.com/terrencepreilly/darglint"><img src="https://img.shields.io/badge/docstrings-darglint-blue" alt="darglint" /></a>
+            <a href="https://github.com/astral-sh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff" /></a>
             <a href="https://github.com/pre-commit/pre-commit"><img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white" alt="pre-commit"></a>
             <a href="https://github.com/astariul/pytere/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
         </p>
         
         <p align="center">
           <a href="#description">Description</a> •
           <a href="#install">Install</a> •
@@ -41,15 +39,15 @@
         <h2 align="center">Description</h2>
         
         **`pytere`** stands for **Py**thon **te**mplate **re**pository.
         
         It's just a template repository for python, with the following features :
         
         * 📚 Beautiful documentation with [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/), published as a Github page with [mike](https://github.com/jimporter/mike) automatically
-        * ✨ Code style checks with [isort](https://github.com/PyCQA/isort), [black](https://github.com/psf/black), [flake518](https://github.com/carstencodes/flake518), [darglint](https://github.com/terrencepreilly/darglint)
+        * ✨ Modern code style checks with [black](https://github.com/psf/black) and [ruff](https://github.com/astral-sh/ruff)
         * 🅿️ Easy development with [pre-commit hooks](https://pre-commit.com/)
         * ✅ Tests with [pytest](https://docs.pytest.org/) and coverage without external tools
         * :octocat: CI with [Github actions](https://github.com/features/actions)
         * 📝 Issues & PR templates
         * 🤖 Stale bot & Dependabot
         * 🚀 Releases automatically published to PyPi
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: pytere Version: 0.4.0 Summary: A Python Template
+Metadata-Version: 2.1 Name: pytere Version: 0.5.0 Summary: A Python Template
 Repository Home-page: https://github.com/astariul/pytere Author: Nicolas REMOND
 Author-email: remondnicola@gmail.com License: UNKNOWN Description:
                              ****** pytere ******
                           Python Template repository
     [GitHub_release] [Test_status] [Lint_status] [Coverage status] [Docs]
-          [isort] [black] [flake8] [darglint] [pre-commit] [licence]
+                     [black] [ruff] [pre-commit] [licence]
 Description â¢ Install â¢ Usage â¢ Use_this_template â¢ FAQ â¢ Contribute
                                  Documentation
                             ***** Description *****
 **`pytere`** stands for **Py**thon **te**mplate **re**pository. It's just a
 template repository for python, with the following features : * ð Beautiful
 documentation with [Material for Mkdocs](https://squidfunk.github.io/mkdocs-
 material/), published as a Github page with [mike](https://github.com/
-jimporter/mike) automatically * â¨ Code style checks with [isort](https://
-github.com/PyCQA/isort), [black](https://github.com/psf/black), [flake518]
-(https://github.com/carstencodes/flake518), [darglint](https://github.com/
-terrencepreilly/darglint) * ð¿ï¸ Easy development with [pre-commit hooks]
-(https://pre-commit.com/) * â Tests with [pytest](https://docs.pytest.org/
-) and coverage without external tools * :octocat: CI with [Github actions]
-(https://github.com/features/actions) * ð Issues & PR templates * ð¤ Stale
-bot & Dependabot * ð Releases automatically published to PyPi
+jimporter/mike) automatically * â¨ Modern code style checks with [black]
+(https://github.com/psf/black) and [ruff](https://github.com/astral-sh/ruff) *
+ð¿ï¸ Easy development with [pre-commit hooks](https://pre-commit.com/) * â
+Tests with [pytest](https://docs.pytest.org/) and coverage without external
+tools * :octocat: CI with [Github actions](https://github.com/features/actions)
+* ð Issues & PR templates * ð¤ Stale bot & Dependabot * ð Releases
+automatically published to PyPi
                               ***** Install *****
 Install `pytere` by running : ``` pip install pytere ``` --- For development,
 you can install it locally by first cloning the repository : ``` git clone
 https://github.com/astariul/pytere.git cd pytere pip install -e . ```
                                ***** Usage *****
 `pytere` does not contain any useful code because it's a template repository.
 But you can check if the package is correctly installed with : ```python from
```

### Comparing `pytere-0.4.0/setup.py` & `pytere-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
 
 reqs = []
 
 extras_require = {
     "test": ["pytest~=7.0", "pytest-cov~=3.0", "coverage-badge~=1.0"],
     "hook": ["pre-commit~=3.0"],
-    "lint": ["isort~=5.9", "black~=22.1", "flake518~=1.2", "darglint~=1.8"],
+    "lint": ["black~=23.1", "ruff~=0.0.272"],
     "docs": ["mkdocs-material~=9.0", "mkdocstrings[python]~=0.18", "mike~=1.1"],
 }
 extras_require["all"] = sum(extras_require.values(), [])
 extras_require["dev"] = (
     extras_require["test"] + extras_require["hook"] + extras_require["lint"] + extras_require["docs"]
 )
 
 setuptools.setup(
     name="pytere",
-    version="0.4.0",
+    version="0.5.0",
     author="Nicolas REMOND",
     author_email="remondnicola@gmail.com",
     description="A Python Template Repository",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/astariul/pytere",
     packages=setuptools.find_packages(),
```

