# Comparing `tmp/pynamer-2.1.5.tar.gz` & `tmp/pynamer-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.1.5.tar", last modified: Tue Jun 13 14:26:33 2023, max compression
+gzip compressed data, was "pynamer-2.1.6.tar", last modified: Sat Jun 17 20:20:17 2023, max compression
```

## Comparing `pynamer-2.1.5.tar` & `pynamer-2.1.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:26:33.111858 pynamer-2.1.5/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.5/AUTHORS.md
--rw-rw-rw-   0        0        0    11151 2023-06-13 14:26:08.000000 pynamer-2.1.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.5/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    19498 2023-06-13 14:26:33.111858 pynamer-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    17533 2023-06-13 14:25:10.000000 pynamer-2.1.5/README.md
--rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.5/pyproject.toml
--rw-rw-rw-   0        0        0     2288 2023-06-13 14:26:33.111858 pynamer-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.721209 pynamer-2.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.830616 pynamer-2.1.5/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.5/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-13 14:26:08.000000 pynamer-2.1.5/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.5/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.5/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.5/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.846211 pynamer-2.1.5/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.5/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7909 2023-06-12 20:06:37.000000 pynamer-2.1.5/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.5/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.5/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.5/src/pynamer/utils.py
--rw-rw-rw-   0        0        0    11394 2023-06-12 20:09:06.000000 pynamer-2.1.5/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.846211 pynamer-2.1.5/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    19498 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 14:26:33.096211 pynamer-2.1.5/tests/
--rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.5/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.5/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2822 2023-06-07 13:04:42.000000 pynamer-2.1.5/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.5/tests/test_get_homepage.py
--rw-rw-rw-   0        0        0     2025 2023-06-12 20:09:06.000000 pynamer-2.1.5/tests/test_github_meta.py
--rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.5/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.5/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.5/tests/test_utils_search_json.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.5/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.534263 pynamer-2.1.6/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.6/AUTHORS.md
+-rw-rw-rw-   0        0        0    11759 2023-06-17 20:20:04.000000 pynamer-2.1.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    19547 2023-06-17 20:20:17.535265 pynamer-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    17582 2023-06-17 19:07:40.000000 pynamer-2.1.6/README.md
+-rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0     2288 2023-06-17 20:20:17.540269 pynamer-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.289270 pynamer-2.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.398264 pynamer-2.1.6/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.6/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-17 20:20:04.000000 pynamer-2.1.6/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.6/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.6/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.6/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.418274 pynamer-2.1.6/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.6/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7935 2023-06-17 17:24:20.000000 pynamer-2.1.6/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.6/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.6/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    11098 2023-06-14 17:55:57.000000 pynamer-2.1.6/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    11810 2023-06-15 11:17:11.000000 pynamer-2.1.6/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.411273 pynamer-2.1.6/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    19547 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.531263 pynamer-2.1.6/tests/
+-rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.6/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.6/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2900 2023-06-15 11:28:35.000000 pynamer-2.1.6/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1484 2023-06-14 19:03:12.000000 pynamer-2.1.6/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.6/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     2025 2023-06-12 20:09:06.000000 pynamer-2.1.6/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.6/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.6/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1325 2023-06-14 17:55:57.000000 pynamer-2.1.6/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.6/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_write_output_file.py
```

### Comparing `pynamer-2.1.5/CHANGELOG.md` & `pynamer-2.1.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.6 (2023-06-17)
+### Fix
+* Error message regarding pypirc file before registration ([`ded4143`](https://github.com/Stephen-RA-King/pynamer/commit/ded4143062a1e2fb5cf74c2912dea692d64fac17))
+
+### Documentation
+* Update logo ([`6be0f9a`](https://github.com/Stephen-RA-King/pynamer/commit/6be0f9ae77e6b63f382e1a490b57153a589a8920))
+* Add missing docstrings ([`1377322`](https://github.com/Stephen-RA-King/pynamer/commit/1377322620a7894bc036021c9cde50bcd4cc732b))
+* Update help screen image ([`7ce744b`](https://github.com/Stephen-RA-King/pynamer/commit/7ce744b6ad94610ebe0eee5158b46db359f73d85))
+
 ## v2.1.5 (2023-06-13)
 ### Fix
 * Typeerror for github license ([`bb7bd2a`](https://github.com/Stephen-RA-King/pynamer/commit/bb7bd2aafef6a78db971e6fda7c4e93978088c9e))
 
 ### Documentation
 * Minor updates ([`e4e3721`](https://github.com/Stephen-RA-King/pynamer/commit/e4e3721ec3e8e541aa1fc5d746cf048e5c157f28))
```

### Comparing `pynamer-2.1.5/LICENSE` & `pynamer-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/PKG-INFO` & `pynamer-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.5
+Version: 2.1.6
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -50,15 +50,15 @@
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
 
 As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
-![](assets/pynamer.png)
+![](assets/pynamer1.png)
 
 # Contents
 
 -   [tl;dr](#TLDR)
 -   [Introduction](#Introduction)
 -   [Quick Start](#Quick-Start)
     -   [Prerequisites](#Prerequisites)
@@ -157,19 +157,19 @@
 ---
 
 -   [x] Python >= 3.9.
 
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
--   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
+-   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API token.
 
     or
 
--   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+-   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables).
 
 Your .pypirc file should contain the following and be on your PATH:
 
 ```file
 [distutils]
 index-servers =
     pypi
@@ -227,33 +227,32 @@
 Display the help menu with the `-h` argument
 
 ```bash
 ~ $ pynamer -h
 ```
 
 ```bash
-usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [-f FILENAME] [-o FILENAME] [--version] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
-  projects              Optional - one or more project names
+  projects          Optional - one or more project names
 
-options:
-  -h, --help            show this help message and exit
-  -r, --register        register the name on PyPi if the name is available
-  -v, --verbose         display information about similar projects
-  -g, --generate        generate a new PyPI index file
-  -m, --meta            input new meta data when registering (Author and email address)
-  -s, --stats           display GitHub stats if available
-  -w, --webbrowser      open the project on PyPI in a webbrowser
-  --version             display version number
-  -f FILE, --file FILE  file containing a list of projects to analyze
-  -o OUTPUT, --output OUTPUT
-                        file to store the test results
+optional arguments:
+  -h, --help        show this help message and exit
+  -r, --register    register the name on PyPi if the name is available
+  -v, --verbose     display information about similar projects
+  -g, --generate    generate a new PyPI index file
+  -m, --meta        input new meta data when registering (Author and email address)
+  -s, --stats       display GitHub stats if available
+  -w, --webbrowser  open the project on PyPI in a webbrowser
+  -f FILENAME       file containing a list of project names to analyze
+  -o FILENAME       file to save the test results
+  --version         display version number
 ```
 
 ## Specifying multiple names
 
 You can specify as many names as you like from the command line e.g.
 
 ```bash
@@ -432,17 +431,18 @@
 
 -   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
 
 ## Meta
 
 ---
 
-[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
+[![Linkedin](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![PyPI repository](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/pynamer)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
```

### Comparing `pynamer-2.1.5/README.md` & `pynamer-2.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
 
 As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
-![](assets/pynamer.png)
+![](assets/pynamer1.png)
 
 # Contents
 
 -   [tl;dr](#TLDR)
 -   [Introduction](#Introduction)
 -   [Quick Start](#Quick-Start)
     -   [Prerequisites](#Prerequisites)
@@ -125,19 +125,19 @@
 ---
 
 -   [x] Python >= 3.9.
 
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
--   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
+-   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API token.
 
     or
 
--   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+-   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables).
 
 Your .pypirc file should contain the following and be on your PATH:
 
 ```file
 [distutils]
 index-servers =
     pypi
@@ -195,33 +195,32 @@
 Display the help menu with the `-h` argument
 
 ```bash
 ~ $ pynamer -h
 ```
 
 ```bash
-usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [-f FILENAME] [-o FILENAME] [--version] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
-  projects              Optional - one or more project names
+  projects          Optional - one or more project names
 
-options:
-  -h, --help            show this help message and exit
-  -r, --register        register the name on PyPi if the name is available
-  -v, --verbose         display information about similar projects
-  -g, --generate        generate a new PyPI index file
-  -m, --meta            input new meta data when registering (Author and email address)
-  -s, --stats           display GitHub stats if available
-  -w, --webbrowser      open the project on PyPI in a webbrowser
-  --version             display version number
-  -f FILE, --file FILE  file containing a list of projects to analyze
-  -o OUTPUT, --output OUTPUT
-                        file to store the test results
+optional arguments:
+  -h, --help        show this help message and exit
+  -r, --register    register the name on PyPi if the name is available
+  -v, --verbose     display information about similar projects
+  -g, --generate    generate a new PyPI index file
+  -m, --meta        input new meta data when registering (Author and email address)
+  -s, --stats       display GitHub stats if available
+  -w, --webbrowser  open the project on PyPI in a webbrowser
+  -f FILENAME       file containing a list of project names to analyze
+  -o FILENAME       file to save the test results
+  --version         display version number
 ```
 
 ## Specifying multiple names
 
 You can specify as many names as you like from the command line e.g.
 
 ```bash
@@ -400,17 +399,18 @@
 
 -   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
 
 ## Meta
 
 ---
 
-[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
+[![Linkedin](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![PyPI repository](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/pynamer)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
```

### Comparing `pynamer-2.1.5/pyproject.toml` & `pynamer-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/setup.cfg` & `pynamer-2.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/src/pynamer/__init__.py` & `pynamer-2.1.6/src/pynamer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.1.5"
+__version__ = "2.1.6"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
@@ -64,14 +64,14 @@
 else:  # pragma: no cover
     raise SystemExit("The package has a structural problem")
 
 
 if project_count_file_trv.is_file():
     project_count = pickle.loads(project_count_file_trv.read_bytes())
 else:  # pragma: no cover
-    project_count = 455256
+    project_count = 460705
 
 
 if meta_file_trv.is_file():
     meta = pickle.loads(meta_file_trv.read_bytes())
 else:  # pragma: no cover
     meta = {}
```

### Comparing `pynamer-2.1.5/src/pynamer/builder.py` & `pynamer-2.1.6/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/src/pynamer/cli.py` & `pynamer-2.1.6/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/src/pynamer/config.py` & `pynamer-2.1.6/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/src/pynamer/pynamer.py` & `pynamer-2.1.6/src/pynamer/pynamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             )
             _build_dist()
             if args.dryrun is False:
                 _upload_dist(new_project)
             else:
                 _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
             _cleanup(new_project)
-        elif config.pypirc is None:
+        elif args.register is True and config.pypirc is None:
             _feedback(
                 ".pypirc file cannot be located ... wont attempt to 'register'",
                 "error",
             )
         elif sum(test_results) > 0 and args.register is True:
             _feedback("Project already exists ... wont attempt to 'register'", "error")
```

### Comparing `pynamer-2.1.5/src/pynamer/utils.py` & `pynamer-2.1.6/src/pynamer/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,296 @@
-#!/usr/bin/env python3
-"""Collection of package support utilities."""
-# Core Library modules
-import json
-import os
-import pickle
-import re
-from importlib.resources import as_file
-from pathlib import Path
-from typing import Any, Union
-
-# Third party modules
-import requests
-from colorama import Back, Fore, Style
-from packaging import version
-from tqdm import tqdm
-
-# First party modules
-import pynamer
-
-# Local modules
-from . import logger, project_count_file_trv, pypi_index_file_trv
-from .config import config
-
-
-def _check_integrity() -> None:
-    pass  # pragma: no cover
-
-
-def _reset() -> None:
-    pass  # pragma: no cover
-
-
-def _feedback(message: str, feedback_type: str) -> None:
-    """Generates a formatted messages appropriate to the message type.
-
-    Args:
-        message:        Text to be echoed.
-        feedback_type:  identifies type of message to display.
-    """
-    if feedback_type not in ["null", "nominal", "warning", "error"]:
-        return
-    if config.idlemode == 1:
-        print(message)
-    else:
-        if feedback_type == "null":
-            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "nominal":
-            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "warning":
-            print(
-                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
-            )
-        elif feedback_type == "error":
-            print(
-                Fore.RED
-                + Back.BLACK
-                + Style.BRIGHT
-                + f"ERROR: {message}"
-                + Style.RESET_ALL
-            )
-
-
-def _search_json(json_data: dict, project_name: str) -> list:
-    github_links = []
-    pattern = re.compile(r"https?://github.com/[\w\-/]+")
-
-    def check_value(value: dict) -> None:
-        if isinstance(value, str):
-            match = pattern.search(value)
-            if match and value.endswith(project_name):
-                github_links.append(match.group(0))
-                return
-
-        elif isinstance(value, list):
-            for item in value:
-                check_value(item)
-
-        elif isinstance(value, dict):
-            for val in value.values():
-                check_value(val)
-
-    check_value(json_data)
-    return github_links
-
-
-def _find_pypirc_file(filename: str = ".pypirc") -> None:
-    """Function to iterate over paths in the PATH environment variable to find a file.
-
-     Designed to find a .pypirc file starting with the current working directory.
-     If identified will update the config.pypirc variable, so it can be used elsewhere.
-
-    Args:
-        filename:       filename to find.
-    """
-    system_path = os.getenv("PATH")
-    if system_path is not None:
-        path_directories = [os.getcwd()]
-        path_directories.extend(system_path.split(os.pathsep))
-        for directory in path_directories:
-            file_path = Path(directory) / filename
-            if file_path.exists():
-                logger.debug(
-                    "%s is present in the system's PATH at %s", filename, directory
-                )
-                config.pypirc = file_path
-                break
-    logger.debug("%s is not present in the system's PATH.", filename)
-
-
-def _generate_pypi_index() -> None:
-    """Generates a list of projects in PyPI's simple index - writes results to a file.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-
-    Notes:
-        A potentially expensive operation as there are almost 500,000 projects to
-        process. Can take 2-3 seconds. Look to improve performance at a later date:
-        look at asyncio, asyncio.http etc.
-        An improvement is to automatically periodically run this in the background.
-    """
-    new_count = 0
-    pattern = re.compile(r">([\w\W]*?)<")
-    with as_file(pypi_index_file_trv) as pypi_index_file:
-        if pypi_index_file.exists():
-            pypi_index_file.unlink(missing_ok=True)
-
-    progress_bar = tqdm(total=config.project_count)
-
-    try:
-        index_object_raw = requests.get(config.pypi_simple_index_url, timeout=5)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    with pypi_index_file_trv.open("a") as file:
-        for line in index_object_raw.iter_lines():
-            line = str(line)
-            project_text = re.search(pattern, line)
-            if project_text is not None:
-                new_count += 1
-                progress_bar.update(1)
-                project = "".join([project_text.group(1), " \n"])
-                file.write(project)
-    progress_bar.close()
-    with project_count_file_trv.open("wb") as f:
-        pickle.dump(new_count, f)
-
-    if config.project_count > 0:
-        diff = new_count - config.project_count
-        if diff > 0:  # pragma: no cover
-            _feedback(
-                f"Project count has increased by {diff} since last index generation",
-                "warning",
-            )
-        elif diff < 0:  # pragma: no cover
-            _feedback(
-                f"Project count has decreased by {diff} since last index generation",
-                "warning",
-            )
-
-
-def _check_version() -> None:
-    """Utility function to compare package version against latest version on PyPI.
-
-    Returns:
-        current_version:    version of the installed package.
-        str:                Message concerning the result of the comparison.
-        bool:               True: if the installed package is up-to-date.
-                            False: if there is a newer version on PyPI.
-    """
-    url_json = "".join([config.pypi_json_url, "pynamer", "/json"])
-    current_version = version.parse(pynamer.__version__)
-    try:
-        project_json_raw = requests.get(url_json, timeout=5)
-    except requests.RequestException:
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-        pypi_version = version.parse(project_json["info"]["version"])
-        if pypi_version > current_version:
-            message = f"(There is a newer version available: {pypi_version})"
-            _feedback(f"{current_version} : {message}", "warning")
-        elif pypi_version == current_version:
-            message = "(You have the most recent version)"
-            _feedback(f"{current_version} : {message}", "nominal")
-
-
-def _process_input_file(file: str) -> list[Union[str, Any]]:
-    """Processes the contents of the file to a list of strings.
-
-    Args:
-        file:           simple string for the file.
-
-    Raises:
-        SystemExit:     If the file is found to not exist.
-
-    Notes:
-        file contents should contain any number of space separated strings on any
-        number of lines.
-    """
-    file_path = Path(file)
-    try:
-        with file_path.open(mode="r") as f:
-            file_contents = f.read()
-            projects = file_contents.split()
-            return list(set(projects))
-    except FileNotFoundError:  # pragma: no cover
-        _feedback(f"The file {file} does not exist", "warning")
-        raise SystemExit()
-    except PermissionError:  # pragma: no cover
-        _feedback(f"Permission denied to file: {file}", "warning")
-        raise SystemExit()
-    except IsADirectoryError:  # pragma: no cover
-        _feedback(f"{file} is a directory not a file", "warning")
-        raise SystemExit()
-    except OSError:  # pragma: no cover
-        _feedback(f"A general IO error has occurred opening file: {file}", "warning")
-        raise SystemExit()
-    except Exception as e:  # pragma: no cover
-        _feedback(f"An error occurred:, {str(e)}", "warning")
-        raise SystemExit()
-
-
-def _write_output_file(file_name: str, results: dict) -> None:
-    """Write the results to a file
-
-    Args:
-        file_name:      Name of file to save as a simple string.
-        results:        Dictionary containing the test results e.g.
-                        {"pynball": [1, 1, 1]}
-    """
-    header_width = 83
-    truncation_width = 25
-    file_path = Path(file_name)
-    title = "Results from pynamer PyPI utility\n"
-    title = "".join([title, "=" * header_width, "\n\n"])
-    title = "".join(
-        [
-            title,
-            "Test 1 - Basic url lookup on PyPI\n",
-            "Test 2 - Search of PyPIs simple index\n",
-            "Test 3 - Search using an request to PyPIs search 'API'\n\n",
-        ]
-    )
-    header = f"{'Project':30}{'Test1':12}{'Test2':12}{'Test3':12}{'Conclusion'}\n"
-    header = "".join([header, "=" * header_width, "\n"])
-    projects_results: str = ""
-    for project in results:
-        project_name = (
-            project
-            if len(project) <= truncation_width
-            else project[: truncation_width - 3] + "..."
-        )
-        projects_results = "".join([projects_results, f"{project_name:30}"])
-        for test in results[project]:
-            test = "Found" if test == 1 else "Not Found"
-            projects_results = "".join([projects_results, f"{test:12}"])
-        conclusion = "Not Available" if sum(results[project]) > 0 else "Available"
-        projects_results = "".join([projects_results, f"{conclusion}"])
-        projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
-
-    final_output_text = "".join([title, header, projects_results])
-
-    try:  # pragma: no cover
-        with file_path.open(mode="w") as f:
-            f.write(final_output_text)
-    except PermissionError:  # pragma: no cover
-        _feedback(f"Permission denied to file: {file_path.open}", "warning")
-        raise SystemExit()
-    except FileExistsError:  # pragma: no cover
-        _feedback(f"File {file_path.open} already exists", "warning")
-        raise SystemExit()
-    except IsADirectoryError:  # pragma: no cover
-        _feedback(f"{file_path.open} is a directory not a file", "warning")
-        raise SystemExit()
-    except OSError:  # pragma: no cover
-        _feedback("General IO error has occurred", "warning")
-        raise SystemExit()
-    except Exception as e:  # pragma: no cover
-        _feedback(f"An error occurred:, {str(e)}", "warning")
-        raise SystemExit()
+#!/usr/bin/env python3
+"""Collection of package support utilities."""
+# Core Library modules
+import json
+import os
+import pickle
+import re
+from importlib.resources import as_file
+from pathlib import Path
+from typing import Any, Union
+
+# Third party modules
+import requests
+from colorama import Back, Fore, Style
+from packaging import version
+from tqdm import tqdm
+
+# First party modules
+import pynamer
+
+# Local modules
+from . import logger, project_count_file_trv, pypi_index_file_trv
+from .config import config
+
+
+def _check_integrity() -> None:
+    pass  # pragma: no cover
+
+
+def _reset() -> None:
+    pass  # pragma: no cover
+
+
+def _feedback(message: str, feedback_type: str) -> None:
+    """Generates a formatted messages appropriate to the message type.
+
+    Args:
+        message:        text to be echoed.
+        feedback_type:  identifies type of message to display.
+    """
+    if feedback_type not in ["null", "nominal", "warning", "error"]:
+        return
+    if config.idlemode == 1:
+        print(message)
+    else:
+        if feedback_type == "null":
+            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "nominal":
+            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "warning":
+            print(
+                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
+            )
+        elif feedback_type == "error":
+            print(
+                Fore.RED
+                + Back.BLACK
+                + Style.BRIGHT
+                + f"ERROR: {message}"
+                + Style.RESET_ALL
+            )
+
+
+def _search_json(json_data: dict, project_name: str) -> str:
+    """Searches a json data structure for a GitHub project URL.
+
+    The json data is found from the PyPI json URL: "https://pypi.org/pypi/package_name".
+    The function searches for the GitHub homepage URL:
+     "https://github.com/{owner}/{package_name} and returns upon first match.
+
+     Args:
+         json_data:     json found from PyPI.
+         project_name:  the package name under test.
+
+    Returns:
+        str:           the GitHub homepage URL if found else an empty string.
+    """
+    homepage = ""
+    pattern = re.compile(r"https?://github.com/[\w\-/]+")
+
+    def check_value(value: dict) -> None:
+        if isinstance(value, str):
+            match = pattern.search(value)
+            if match and value.endswith(project_name):
+                nonlocal homepage
+                homepage = match.group(0)
+                return
+
+        elif isinstance(value, list):
+            for item in value:
+                check_value(item)
+
+        elif isinstance(value, dict):
+            for val in value.values():
+                check_value(val)
+
+    check_value(json_data)
+    return homepage
+
+
+def _find_pypirc_file(filename: str = ".pypirc") -> None:
+    """Function to iterate over paths in the PATH environment variable to find a file.
+
+     Designed to find a .pypirc file starting with the current working directory.
+     If identified will update the config.pypirc variable, so it can be used elsewhere.
+
+    Args:
+        filename:       filename to find.
+    """
+    system_path = os.getenv("PATH")
+    if system_path is not None:
+        path_directories = [os.getcwd()]
+        path_directories.extend(system_path.split(os.pathsep))
+        for directory in path_directories:
+            file_path = Path(directory) / filename
+            if file_path.exists():
+                logger.debug(
+                    "%s is present in the system's PATH at %s", filename, directory
+                )
+                config.pypirc = file_path
+                break
+    logger.debug("%s is not present in the system's PATH.", filename)
+
+
+def _generate_pypi_index() -> None:
+    """Generates a list of projects in PyPI's simple index - writes results to a file.
+
+    Raises:
+        SystemExit:     if any requests.RequestException occurs.
+
+    Notes:
+        A potentially expensive operation as there are almost 500,000 projects to
+        process. Can take 2-3 seconds. Look to improve performance at a later date:
+        look at asyncio, asyncio.http etc.
+        An improvement is to automatically periodically run this in the background.
+    """
+    new_count = 0
+    pattern = re.compile(r">([\w\W]*?)<")
+    with as_file(pypi_index_file_trv) as pypi_index_file:
+        if pypi_index_file.exists():
+            pypi_index_file.unlink(missing_ok=True)
+
+    progress_bar = tqdm(total=config.project_count)
+
+    try:
+        index_object_raw = requests.get(config.pypi_simple_index_url, timeout=5)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    with pypi_index_file_trv.open("a") as file:
+        for line in index_object_raw.iter_lines():
+            line = str(line)
+            project_text = re.search(pattern, line)
+            if project_text is not None:
+                new_count += 1
+                progress_bar.update(1)
+                project = "".join([project_text.group(1), " \n"])
+                file.write(project)
+    progress_bar.close()
+    with project_count_file_trv.open("wb") as f:
+        pickle.dump(new_count, f)
+
+    if config.project_count > 0:
+        diff = new_count - config.project_count
+        if diff > 0:  # pragma: no cover
+            _feedback(
+                f"Project count has increased by {diff} since last index generation",
+                "warning",
+            )
+        elif diff < 0:  # pragma: no cover
+            _feedback(
+                f"Project count has decreased by {diff} since last index generation",
+                "warning",
+            )
+
+
+def _check_version() -> None:
+    """Utility function to compare package version against latest version on PyPI.
+
+    Returns:
+        current_version:    version of the installed package.
+        str:                message concerning the result of the comparison.
+        bool:               True: if the installed package is up-to-date.
+                            False: if there is a newer version on PyPI.
+    """
+    url_json = "".join([config.pypi_json_url, "pynamer", "/json"])
+    current_version = version.parse(pynamer.__version__)
+    try:
+        project_json_raw = requests.get(url_json, timeout=5)
+    except requests.RequestException:
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+        pypi_version = version.parse(project_json["info"]["version"])
+        if pypi_version > current_version:
+            message = f"(There is a newer version available: {pypi_version})"
+            _feedback(f"{current_version} : {message}", "warning")
+        elif pypi_version == current_version:
+            message = "(You have the most recent version)"
+            _feedback(f"{current_version} : {message}", "nominal")
+
+
+def _process_input_file(file: str) -> list[Union[str, Any]]:
+    """Processes the contents of the file to a list of strings.
+
+    Args:
+        file:           simple string for the file.
+
+    Raises:
+        SystemExit:     if the file is found to not exist.
+
+    Notes:
+        File contents should contain any number of space separated strings on any
+        number of lines.
+    """
+    file_path = Path(file)
+    try:
+        with file_path.open(mode="r") as f:
+            file_contents = f.read()
+            projects = file_contents.split()
+            return list(set(projects))
+    except FileNotFoundError:  # pragma: no cover
+        _feedback(f"The file {file} does not exist", "warning")
+        raise SystemExit()
+    except PermissionError:  # pragma: no cover
+        _feedback(f"Permission denied to file: {file}", "warning")
+        raise SystemExit()
+    except IsADirectoryError:  # pragma: no cover
+        _feedback(f"{file} is a directory not a file", "warning")
+        raise SystemExit()
+    except OSError:  # pragma: no cover
+        _feedback(f"A general IO error has occurred opening file: {file}", "warning")
+        raise SystemExit()
+    except Exception as e:  # pragma: no cover
+        _feedback(f"An error occurred:, {str(e)}", "warning")
+        raise SystemExit()
+
+
+def _write_output_file(file_name: str, results: dict) -> None:
+    """Write the results to a file.
+
+    Args:
+        file_name:      name of file to save as a simple string.
+        results:        dictionary containing the test results e.g.
+                        {"pynball": [1, 1, 1]}
+    """
+    header_width = 83
+    truncation_width = 25
+    file_path = Path(file_name)
+    title = "Results from pynamer PyPI utility\n"
+    title = "".join([title, "=" * header_width, "\n\n"])
+    title = "".join(
+        [
+            title,
+            "Test 1 - Basic url lookup on PyPI\n",
+            "Test 2 - Search of PyPIs simple index\n",
+            "Test 3 - Search using an request to PyPIs search 'API'\n\n",
+        ]
+    )
+    header = f"{'Project':30}{'Test1':12}{'Test2':12}{'Test3':12}{'Conclusion'}\n"
+    header = "".join([header, "=" * header_width, "\n"])
+    projects_results: str = ""
+    for project in results:
+        project_name = (
+            project
+            if len(project) <= truncation_width
+            else project[: truncation_width - 3] + "..."
+        )
+        projects_results = "".join([projects_results, f"{project_name:30}"])
+        for test in results[project]:
+            test = "Found" if test == 1 else "Not Found"
+            projects_results = "".join([projects_results, f"{test:12}"])
+        conclusion = "Not Available" if sum(results[project]) > 0 else "Available"
+        projects_results = "".join([projects_results, f"{conclusion}"])
+        projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
+
+    final_output_text = "".join([title, header, projects_results])
+
+    try:  # pragma: no cover
+        with file_path.open(mode="w") as f:
+            f.write(final_output_text)
+    except PermissionError:  # pragma: no cover
+        _feedback(f"Permission denied to file: {file_path.open}", "warning")
+        raise SystemExit()
+    except FileExistsError:  # pragma: no cover
+        _feedback(f"File {file_path.open} already exists", "warning")
+        raise SystemExit()
+    except IsADirectoryError:  # pragma: no cover
+        _feedback(f"{file_path.open} is a directory not a file", "warning")
+        raise SystemExit()
+    except OSError:  # pragma: no cover
+        _feedback("General IO error has occurred", "warning")
+        raise SystemExit()
+    except Exception as e:  # pragma: no cover
+        _feedback(f"An error occurred:, {str(e)}", "warning")
+        raise SystemExit()
```

### Comparing `pynamer-2.1.5/src/pynamer/validators.py` & `pynamer-2.1.6/src/pynamer/validators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,304 +1,326 @@
-#!/usr/bin/env python3
-"""Collection of functions to test availability of a package name on PyPI"""
-# Core Library modules
-import json
-import re
-import string
-from datetime import datetime
-from typing import Any, Union
-
-# Third party modules
-import requests
-from bs4 import BeautifulSoup
-from dateutil.parser import isoparse
-from rich.console import Console
-from rich.table import Table
-
-# Local modules
-from . import logger, pypi_index_file_trv
-from .config import config
-from .utils import _generate_pypi_index, _search_json
-
-
-def _is_valid_package_name(project_name: str) -> bool:
-    """Function does a basic check of project name validity.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the name passes the basic check
-        False:          If the name fails the basic check
-    """
-    pattern = re.compile("^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.I)
-    if re.match(pattern, project_name) is not None:
-        return True
-    else:
-        return False
-
-
-def _get_homepage(project_json: dict, project_name: str) -> tuple[str, str]:
-    home_url = project_json["info"]["home_page"]
-
-    if "github.com" in home_url and home_url.endswith(project_name):
-        return "".join(["Homepage: ", home_url]), home_url
-
-    if "github.io" in home_url:
-        for item in (".github.io", "https://"):
-            home_url = home_url.replace(item, "")
-        home_url = home_url.rstrip("/")
-        home_url = "".join([config.github_base_url, home_url])
-        return "".join(["Homepage: ", home_url]), home_url
-
-    homepages = _search_json(project_json, project_name)
-    for home_url in homepages:
-        if "github.com" in home_url and home_url.endswith(project_name):
-            return "".join(["Homepage: ", home_url]), home_url
-
-    if home_url != "":
-        return "".join(["Homepage: ", home_url]), home_url
-
-    return "Homepage: None", ""
-
-
-def _github_meta(url: str) -> str:
-    return_text = "\n\nGitHub Stats\n------------\n"
-    repo_api_url = "".join(
-        [config.github_api_url, url.replace(r"https://github.com/", "")]
-    )
-    try:
-        json_raw = requests.get(repo_api_url, timeout=5)
-    except requests.RequestException:
-        return "".join([return_text, "GitHub can not be contacted"])
-
-    if json_raw.status_code == 200:
-        repo_json = json_raw.json()
-
-        license_name = (
-            repo_json["license"]["name"] if repo_json["license"] is not None else "None"
-        )
-
-        return "".join(
-            [
-                return_text,
-                f"stars:    {repo_json['stargazers_count']}",
-                "\n",
-                f"forks:    {repo_json['forks']}",
-                "\n",
-                f"issues:   {repo_json['open_issues']}",
-                "\n",
-                f"license:  {license_name}",
-                "\n",
-                f"watching: {repo_json['subscribers_count']}",
-                "\n",
-                f"created:  {isoparse(repo_json['created_at']).date()}",
-                "\n",
-                f"updated:  {isoparse(repo_json['updated_at']).date()}",
-            ]
-        )
-    if json_raw.status_code == 404:
-        return "".join([return_text, "repository does not exist"])
-    return ""
-
-
-def _ping_project(project_name: str) -> bool:
-    """Determines if the URL to the project exists in PyPIs project area.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the URLs response code is 200
-        False:          If the URLs response code is not 200
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_project = "".join([config.pypi_project_url, project_name, "/"])
-    logger.debug("attempting to get url %s", url_project)
-    try:
-        project_ping = requests.get(url_project, timeout=5)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_ping.status_code == 200:
-        logger.debug("%s FOUND in the project area of PyPI", project_name)
-        return True
-    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
-    return False
-
-
-def _ping_json(project_name: str, stats: bool = False) -> str:
-    """Collects some details about the project if it exists.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_json = "".join([config.pypi_json_url, project_name, "/json"])
-    logger.debug("attempting to get url %s", url_json)
-    try:
-        project_json_raw = requests.get(url_json, timeout=5)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-
-        homepage_text, homepage_url = _get_homepage(project_json, project_name)
-
-        author = (
-            "".join(["Author:   ", project_json["info"]["author"]])
-            if project_json["info"]["author"]
-            else "Author:   None"
-        )
-        version = (
-            "".join(["Version:  ", project_json["info"]["version"]])
-            if project_json["info"]["version"]
-            else "Version:  None"
-        )
-        email = (
-            "".join(["Email:    ", project_json["info"]["author_email"]])
-            if project_json["info"]["author_email"]
-            else "Email:    None"
-        )
-        summary = (
-            "".join(["Summary:  ", project_json["info"]["summary"]])
-            if project_json["info"]["summary"]
-            else "Summary:  None"
-        )
-        result = "".join(
-            [summary, "\n", author, "\n", email, "\n", version, "\n", homepage_text]
-        )
-
-        if "github" in homepage_url and stats is True:
-            result = "".join([result, _github_meta(homepage_url)])
-        return result
-    logger.debug("No response from JSON URL")
-    return ""
-
-
-def _pypi_search_index(project_name: str) -> bool:
-    """Open the generated index file and search for the project name.
-
-    Args:
-        project_name:   the name of the project currently under test.
-
-    Returns:
-        True:           A match was found.
-        False:          A match was not found.
-    """
-    if not pypi_index_file_trv.is_file():
-        _generate_pypi_index()
-
-    projects = pypi_index_file_trv.read_text(encoding="utf-8")
-    if project_name in projects:
-        logger.debug("%s FOUND in the PyPI simple index", project_name)
-        return True
-    logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
-    return False
-
-
-def _pypi_search(
-    search_project: str,
-) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
-    """Performs a get request to PyPI's search API for the project name.
-
-    Args:
-        search_project:   The name of the project currently under test.
-
-    Returns:
-        match:          A list of projects matching name comprising:
-                            [project_name, version, released, description]
-        others:         A list of projects not matching but PyPI thinks are relevant.
-                            [project_name, version, released, description]
-        others_total:   A str representation of total projects found (minus matches).
-    """
-    pattern = re.compile(r">([\d,+]*?)<")
-    s = requests.Session()
-    projects_raw: list = []
-    match: list[list[str]] = []
-    others: list[list[str]] = []
-    params = {"q": {search_project}, "page": 1}
-    r = s.get(config.pypi_search_url, params=params)  # type: ignore
-    soup = BeautifulSoup(r.text, "html.parser")
-    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
-    for project_raw in projects_raw:
-        project_name = project_raw.select_one(
-            'span[class*="package-snippet__name"]'
-        ).text.strip()
-        version = project_raw.select_one(
-            'span[class*="package-snippet__version"]'
-        ).text.strip()
-        released_iso_8601 = project_raw.select_one(
-            'span[class*="package-snippet__created"]'
-        ).find("time")["datetime"]
-        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
-            "%Y-%m-%d"
-        )
-        description = project_raw.select_one(
-            'p[class*="package-snippet__description"]'
-        ).text.strip()
-        if project_name.lower() == search_project.lower():
-            match.append([project_name, version, released, description])
-        else:
-            others.append([project_name, version, released, description])
-
-    total_div_raw = soup.select(
-        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
-    )
-    total_raw = re.search(pattern, str(total_div_raw))
-    if total_raw is not None:
-        total_string = total_raw.group(1)
-        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
-        others_total = (
-            "".join([str(total), "+"])
-            if total == 10000
-            else (str(int(total) - len(match)))
-        )
-    else:
-        others_total = "0"
-    return match, others, others_total
-
-
-def _final_analysis(pattern: list[int]) -> None:
-    """Displays a rich console table displaying the conclusion of the test results
-
-    Args:
-        pattern:    A list of the test results:
-                    1 - A 'negative' result, indicating the project has been found.
-                    0 - A 'positive' result, indicating the project was not found.
-    """
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    if pattern == [0, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "It can only be found by searching the simple index which is not available "
-            "through the web interface.\n\n"
-            "The most likely cause is an abandoned or deleted project by the owner.\n\n"
-            "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
-            "to name transfer"
-        )
-    elif pattern == [1, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "However if appears in the simple index and can be displayed by simply"
-            " browsing "
-            "to the projects URL"
-        )
-    elif sum(pattern) >= 1:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row("The package name was found in at least one place")
-    elif sum(pattern) == 0:
-        table.add_row("[green]AVAILABLE![/green]\n")
-        table.add_row("The package name was not found in any part of PyPI")
-
-    console = Console()
-    console.print(table)
+#!/usr/bin/env python3
+"""Collection of functions to test availability of a package name on PyPI"""
+# Core Library modules
+import json
+import re
+import string
+from datetime import datetime
+from typing import Any, Union
+
+# Third party modules
+import requests
+from bs4 import BeautifulSoup
+from dateutil.parser import isoparse
+from rich.console import Console
+from rich.table import Table
+
+# Local modules
+from . import logger, pypi_index_file_trv
+from .config import config
+from .utils import _generate_pypi_index, _search_json
+
+
+def _is_valid_package_name(project_name: str) -> bool:
+    """Function does a basic check of project name validity.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the name passes the basic check
+        False:          If the name fails the basic check
+    """
+    pattern = re.compile("^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.I)
+    if re.match(pattern, project_name) is not None:
+        return True
+    else:
+        return False
+
+
+def _get_homepage(project_json: dict, project_name: str) -> tuple[str, str]:
+    """Finds the GitHub homepage from the PyPI json data.
+
+    With this function we are trying to ultimately find the GitHub 'homepage':
+    https://github.com/{username}/{project_name}.
+    Unfortunately not everyone agrees what the homepage should be. Some people for
+    example use 'readthedocs' or 'github.io' etc.
+
+    Args:
+        project_json:       json data from PyPI json URL.
+        project_name:       package name under test.
+
+    Returns:
+        tuple[str, str]:    strings containing found homepage URL.
+    """
+    home_url = project_json["info"]["home_page"]
+
+    if "github.com" in home_url and home_url.endswith(project_name):
+        return "".join(["Homepage: ", home_url]), home_url
+
+    if "github.io" in home_url:
+        for item in (".github.io", "https://"):
+            home_url = home_url.replace(item, "")
+        home_url = home_url.rstrip("/")
+        home_url = "".join([config.github_base_url, home_url])
+        return "".join(["Homepage: ", home_url]), home_url
+
+    homepage = _search_json(project_json, project_name)
+    if homepage:
+        return "".join(["Homepage: ", homepage]), homepage
+
+    if home_url != "":
+        return "".join(["Homepage: ", home_url]), home_url
+
+    return "Homepage: None", ""
+
+
+def _github_meta(url: str) -> str:
+    """Finds GitHub statistics given a GitHub Homepage URL.
+
+    Args:
+        url:    GitHub homepage URL.
+
+    Returns:
+        str:    a string containing all the pertinent statistics:
+    """
+    return_text = "\n\nGitHub Stats\n------------\n"
+    repo_api_url = "".join(
+        [config.github_api_url, url.replace(r"https://github.com/", "")]
+    )
+    try:
+        json_raw = requests.get(repo_api_url, timeout=5)
+    except requests.RequestException:
+        return "".join([return_text, "GitHub can not be contacted"])
+
+    if json_raw.status_code == 200:
+        repo_json = json_raw.json()
+
+        license_name = (
+            repo_json["license"]["name"] if repo_json["license"] is not None else "None"
+        )
+
+        return "".join(
+            [
+                return_text,
+                f"stars:    {repo_json['stargazers_count']}",
+                "\n",
+                f"forks:    {repo_json['forks']}",
+                "\n",
+                f"issues:   {repo_json['open_issues']}",
+                "\n",
+                f"license:  {license_name}",
+                "\n",
+                f"watching: {repo_json['subscribers_count']}",
+                "\n",
+                f"created:  {isoparse(repo_json['created_at']).date()}",
+                "\n",
+                f"updated:  {isoparse(repo_json['updated_at']).date()}",
+            ]
+        )
+    if json_raw.status_code == 404:
+        return "".join([return_text, "repository does not exist"])
+    return ""
+
+
+def _ping_project(project_name: str) -> bool:
+    """Determines if the URL to the project exists in PyPIs project area.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           if the URLs response code is 200.
+        False:          if the URLs response code is not 200.
+
+    Raises:
+        SystemExit:     if any requests.RequestException occurs.
+    """
+    url_project = "".join([config.pypi_project_url, project_name, "/"])
+    logger.debug("attempting to get url %s", url_project)
+    try:
+        project_ping = requests.get(url_project, timeout=5)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_ping.status_code == 200:
+        logger.debug("%s FOUND in the project area of PyPI", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
+    return False
+
+
+def _ping_json(project_name: str, stats: bool = False) -> str:
+    """Collects some details about the project if it exists.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Raises:
+        SystemExit:     if any requests.RequestException occurs.
+    """
+    url_json = "".join([config.pypi_json_url, project_name, "/json"])
+    logger.debug("attempting to get url %s", url_json)
+    try:
+        project_json_raw = requests.get(url_json, timeout=5)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+
+        homepage_text, homepage_url = _get_homepage(project_json, project_name)
+
+        author = (
+            "".join(["Author:   ", project_json["info"]["author"]])
+            if project_json["info"]["author"]
+            else "Author:   None"
+        )
+        version = (
+            "".join(["Version:  ", project_json["info"]["version"]])
+            if project_json["info"]["version"]
+            else "Version:  None"
+        )
+        email = (
+            "".join(["Email:    ", project_json["info"]["author_email"]])
+            if project_json["info"]["author_email"]
+            else "Email:    None"
+        )
+        summary = (
+            "".join(["Summary:  ", project_json["info"]["summary"]])
+            if project_json["info"]["summary"]
+            else "Summary:  None"
+        )
+        result = "".join(
+            [summary, "\n", author, "\n", email, "\n", version, "\n", homepage_text]
+        )
+
+        if "github" in homepage_url and stats is True:
+            result = "".join([result, _github_meta(homepage_url)])
+        return result
+    logger.debug("No response from JSON URL")
+    return ""
+
+
+def _pypi_search_index(project_name: str) -> bool:
+    """Open the generated index file and search for the project name.
+
+    Args:
+        project_name:   the name of the project currently under test.
+
+    Returns:
+        True:           a match was found.
+        False:          a match was not found.
+    """
+    if not pypi_index_file_trv.is_file():
+        _generate_pypi_index()
+
+    projects = pypi_index_file_trv.read_text(encoding="utf-8")
+    if project_name in projects:
+        logger.debug("%s FOUND in the PyPI simple index", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
+    return False
+
+
+def _pypi_search(
+    search_project: str,
+) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
+    """Performs a get request to PyPI's search API for the project name.
+
+    Args:
+        search_project:   the name of the project currently under test.
+
+    Returns:
+        match:          a list of projects matching name comprising:
+                            [project_name, version, released, description]
+        others:         a list of projects not matching but PyPI thinks are relevant.
+                            [project_name, version, released, description]
+        others_total:   a str representation of total projects found (minus matches).
+    """
+    pattern = re.compile(r">([\d,+]*?)<")
+    s = requests.Session()
+    projects_raw: list = []
+    match: list[list[str]] = []
+    others: list[list[str]] = []
+    params = {"q": {search_project}, "page": 1}
+    r = s.get(config.pypi_search_url, params=params)  # type: ignore
+    soup = BeautifulSoup(r.text, "html.parser")
+    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
+    for project_raw in projects_raw:
+        project_name = project_raw.select_one(
+            'span[class*="package-snippet__name"]'
+        ).text.strip()
+        version = project_raw.select_one(
+            'span[class*="package-snippet__version"]'
+        ).text.strip()
+        released_iso_8601 = project_raw.select_one(
+            'span[class*="package-snippet__created"]'
+        ).find("time")["datetime"]
+        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
+            "%Y-%m-%d"
+        )
+        description = project_raw.select_one(
+            'p[class*="package-snippet__description"]'
+        ).text.strip()
+        if project_name.lower() == search_project.lower():
+            match.append([project_name, version, released, description])
+        else:
+            others.append([project_name, version, released, description])
+
+    total_div_raw = soup.select(
+        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
+    )
+    total_raw = re.search(pattern, str(total_div_raw))
+    if total_raw is not None:
+        total_string = total_raw.group(1)
+        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
+        others_total = (
+            "".join([str(total), "+"])
+            if total == 10000
+            else (str(int(total) - len(match)))
+        )
+    else:
+        others_total = "0"
+    return match, others, others_total
+
+
+def _final_analysis(pattern: list[int]) -> None:
+    """Displays a rich console table displaying the conclusion of the test results
+
+    Args:
+        pattern:    a list of the test results:
+                    1 - a 'negative' result, indicating the project has been found.
+                    0 - a 'positive' result, indicating the project was not found.
+    """
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    if pattern == [0, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "It can only be found by searching the simple index which is not available "
+            "through the web interface.\n\n"
+            "The most likely cause is an abandoned or deleted project by the owner.\n\n"
+            "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
+            "to name transfer.\n"
+            "https://peps.python.org/pep-0541/#how-to-request-a-name-transfer"
+        )
+    elif pattern == [1, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "However if appears in the simple index and can be displayed by simply"
+            " browsing "
+            "to the projects URL"
+        )
+    elif sum(pattern) >= 1:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row("The package name was found in at least one place")
+    elif sum(pattern) == 0:
+        table.add_row("[green]AVAILABLE![/green]\n")
+        table.add_row("The package name was not found in any part of PyPI")
+
+    console = Console()
+    console.print(table)
```

### Comparing `pynamer-2.1.5/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.6/src/pynamer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.5
+Version: 2.1.6
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -50,15 +50,15 @@
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
 
 As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
-![](assets/pynamer.png)
+![](assets/pynamer1.png)
 
 # Contents
 
 -   [tl;dr](#TLDR)
 -   [Introduction](#Introduction)
 -   [Quick Start](#Quick-Start)
     -   [Prerequisites](#Prerequisites)
@@ -157,19 +157,19 @@
 ---
 
 -   [x] Python >= 3.9.
 
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
--   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
+-   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API token.
 
     or
 
--   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+-   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables).
 
 Your .pypirc file should contain the following and be on your PATH:
 
 ```file
 [distutils]
 index-servers =
     pypi
@@ -227,33 +227,32 @@
 Display the help menu with the `-h` argument
 
 ```bash
 ~ $ pynamer -h
 ```
 
 ```bash
-usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [-f FILENAME] [-o FILENAME] [--version] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
-  projects              Optional - one or more project names
+  projects          Optional - one or more project names
 
-options:
-  -h, --help            show this help message and exit
-  -r, --register        register the name on PyPi if the name is available
-  -v, --verbose         display information about similar projects
-  -g, --generate        generate a new PyPI index file
-  -m, --meta            input new meta data when registering (Author and email address)
-  -s, --stats           display GitHub stats if available
-  -w, --webbrowser      open the project on PyPI in a webbrowser
-  --version             display version number
-  -f FILE, --file FILE  file containing a list of projects to analyze
-  -o OUTPUT, --output OUTPUT
-                        file to store the test results
+optional arguments:
+  -h, --help        show this help message and exit
+  -r, --register    register the name on PyPi if the name is available
+  -v, --verbose     display information about similar projects
+  -g, --generate    generate a new PyPI index file
+  -m, --meta        input new meta data when registering (Author and email address)
+  -s, --stats       display GitHub stats if available
+  -w, --webbrowser  open the project on PyPI in a webbrowser
+  -f FILENAME       file containing a list of project names to analyze
+  -o FILENAME       file to save the test results
+  --version         display version number
 ```
 
 ## Specifying multiple names
 
 You can specify as many names as you like from the command line e.g.
 
 ```bash
@@ -432,17 +431,18 @@
 
 -   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
 
 ## Meta
 
 ---
 
-[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
+[![Linkedin](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![PyPI repository](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/pynamer)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
```

### Comparing `pynamer-2.1.5/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.6/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_args.py` & `pynamer-2.1.6/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_build_dist.py` & `pynamer-2.1.6/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_cleanup.py` & `pynamer-2.1.6/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_create_setup_file.py` & `pynamer-2.1.6/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_defaults.py` & `pynamer-2.1.6/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_delete_director.py` & `pynamer-2.1.6/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_feedback.py` & `pynamer-2.1.6/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_final_analysis.py` & `pynamer-2.1.6/tests/test_final_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     table.add_row(
         "A Gotcha!, whereby the package is not found even with PyPI's own search"
         " facility.\n"
         "It can only be found by searching the simple index which is not available "
         "through the web interface.\n\n"
         "The most likely cause is an abandoned or deleted project by the owner.\n\n"
         "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
-        "to name transfer"
+        "to name transfer.\n"
+        "https://peps.python.org/pep-0541/#how-to-request-a-name-transfer"
     )
     console = Console()
     console.print(table)
     captured_expected = capsys.readouterr()
 
     pynamer._final_analysis([0, 1, 0])
     captured_actual = capsys.readouterr()
```

### Comparing `pynamer-2.1.5/tests/test_find_pypirc_file.py` & `pynamer-2.1.6/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_generate_pypi_index.py` & `pynamer-2.1.6/tests/test_generate_pypi_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 
 
 def test_generate_pypi_index_error(monkeypatch, project_path_mock):
     def mock_requests_error(*args, **kwargs):
         raise ConnectTimeout("Connection timed out")
 
     monkeypatch.setattr(requests, "get", mock_requests_error)
+    monkeypatch.setattr(utils, "pypi_index_file_trv", BASE_DIR / "pypi_index")
 
     with pytest.raises(SystemExit) as excinfo:
-        pynamer._generate_pypi_index()
+        utils._generate_pypi_index()
     assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-2.1.5/tests/test_get_homepage.py` & `pynamer-2.1.6/tests/test_get_homepage.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_github_meta.py` & `pynamer-2.1.6/tests/test_github_meta.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_ping_json.py` & `pynamer-2.1.6/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_ping_project.py` & `pynamer-2.1.6/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_process_input_file.py` & `pynamer-2.1.6/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_pypi_search.py` & `pynamer-2.1.6/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_pypi_search_index.py` & `pynamer-2.1.6/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_rename_project_dir.py` & `pynamer-2.1.6/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_upload_dist.py` & `pynamer-2.1.6/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_utils_search_json.py` & `pynamer-2.1.6/tests/test_utils_search_json.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#!/usr/bin/env python3
-# Core Library modules
-import json
-import pickle
-from pathlib import Path
-
-# First party modules
-import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_search_json_black():
-    pickle_file = BASE_DIR / "resources" / "requests_get_json_black.pickle"
-    pickle_bytes = pickle_file.read_bytes()
-    request_object = pickle.loads(pickle_bytes)
-    project_json = json.loads(request_object.content)
-
-    urls = pynamer.utils._search_json(project_json, "black")
-
-    assert urls == ["https://github.com/psf/black"]
-
-
-def test_search_json_isort():
-    pickle_file = BASE_DIR / "resources" / "requests_get_json_isort.pickle"
-    pickle_bytes = pickle_file.read_bytes()
-    request_object = pickle.loads(pickle_bytes)
-    project_json = json.loads(request_object.content)
-
-    urls = pynamer.utils._search_json(project_json, "isort")
-
-    assert urls == ["https://github.com/pycqa/isort"]
-
-
-def test_search_json_requests():
-    pickle_file = BASE_DIR / "resources" / "requests_get_json_requests.pickle"
-    pickle_bytes = pickle_file.read_bytes()
-    request_object = pickle.loads(pickle_bytes)
-    project_json = json.loads(request_object.content)
-
-    urls = pynamer.utils._search_json(project_json, "requests")
-
-    assert urls == ["https://github.com/psf/requests"]
+#!/usr/bin/env python3
+# Core Library modules
+import json
+import pickle
+from pathlib import Path
+
+# First party modules
+import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_search_json_black():
+    pickle_file = BASE_DIR / "resources" / "requests_get_json_black.pickle"
+    pickle_bytes = pickle_file.read_bytes()
+    request_object = pickle.loads(pickle_bytes)
+    project_json = json.loads(request_object.content)
+
+    url = pynamer.utils._search_json(project_json, "black")
+
+    assert url == "https://github.com/psf/black"
+
+
+def test_search_json_isort():
+    pickle_file = BASE_DIR / "resources" / "requests_get_json_isort.pickle"
+    pickle_bytes = pickle_file.read_bytes()
+    request_object = pickle.loads(pickle_bytes)
+    project_json = json.loads(request_object.content)
+
+    url = pynamer.utils._search_json(project_json, "isort")
+
+    assert url == "https://github.com/pycqa/isort"
+
+
+def test_search_json_requests():
+    pickle_file = BASE_DIR / "resources" / "requests_get_json_requests.pickle"
+    pickle_bytes = pickle_file.read_bytes()
+    request_object = pickle.loads(pickle_bytes)
+    project_json = json.loads(request_object.content)
+
+    url = pynamer.utils._search_json(project_json, "requests")
+
+    assert url == "https://github.com/psf/requests"
```

### Comparing `pynamer-2.1.5/tests/test_utils_version.py` & `pynamer-2.1.6/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.5/tests/test_write_output_file.py` & `pynamer-2.1.6/tests/test_write_output_file.py`

 * *Files identical despite different names*

