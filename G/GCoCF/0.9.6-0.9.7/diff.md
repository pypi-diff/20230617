# Comparing `tmp/gcocf-0.9.6.tar.gz` & `tmp/gcocf-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcocf-0.9.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcocf-0.9.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcocf-0.9.6.tar` & `gcocf-0.9.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      124 2023-06-17 07:19:16.828575 gcocf-0.9.6/.example.envrc
--rw-r--r--   0        0        0      669 2023-06-17 07:19:16.828575 gcocf-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2023-06-17 07:19:16.828575 gcocf-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      501 2023-06-17 07:19:16.828575 gcocf-0.9.6/.github/dependabot.yml
--rw-r--r--   0        0        0     1076 2023-06-17 07:19:16.828575 gcocf-0.9.6/.github/pull_request_template.md
--rw-r--r--   0        0        0     1691 2023-06-17 07:19:16.828575 gcocf-0.9.6/.github/workflows/Testing.yml
--rw-r--r--   0        0        0      103 2023-06-17 07:19:16.828575 gcocf-0.9.6/.gitignore
--rw-r--r--   0        0        0     5224 2023-06-17 07:19:16.828575 gcocf-0.9.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      203 2023-06-17 07:19:16.828575 gcocf-0.9.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      273 2023-06-17 07:19:16.828575 gcocf-0.9.6/Dockerfile
--rw-r--r--   0        0        0      144 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/__init__.py
--rwxr-xr-x   0        0        0    10649 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/__main__.py
--rw-r--r--   0        0        0     2224 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/api.py
--rw-r--r--   0        0        0    10419 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/formatters.py
--rw-r--r--   0        0        0     2369 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/locales/messages.pot
--rw-r--r--   0        0        0    12638 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/models.py
--rw-r--r--   0        0        0     1009 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/notifiers.py
--rw-r--r--   0        0        0     1378 2023-06-17 07:19:16.828575 gcocf-0.9.6/GCoCF/utils.py
--rw-r--r--   0        0        0     1070 2023-06-17 07:19:16.828575 gcocf-0.9.6/LICENSE.txt
--rw-r--r--   0        0        0     1307 2023-06-17 07:19:16.828575 gcocf-0.9.6/README.md
--rw-r--r--   0        0        0     2495 2023-06-17 07:19:16.828575 gcocf-0.9.6/SECURITY.md
--rw-r--r--   0        0        0    41692 2023-06-17 07:19:16.828575 gcocf-0.9.6/data/full_destruction.json
--rw-r--r--   0        0        0    77643 2023-06-17 07:19:16.828575 gcocf-0.9.6/data/inWar_40.json
--rw-r--r--   0        0        0     1059 2023-06-17 07:19:16.828575 gcocf-0.9.6/data/notInWar.json
--rw-r--r--   0        0        0    24207 2023-06-17 07:19:16.828575 gcocf-0.9.6/data/op_full_destruction.json
--rw-r--r--   0        0        0    98300 2023-06-17 07:19:16.828575 gcocf-0.9.6/data/warEnded_50.json
--rw-r--r--   0        0        0      832 2023-06-17 07:19:16.828575 gcocf-0.9.6/pyproject.toml
--rw-r--r--   0        0        0       54 2023-06-17 07:19:16.828575 gcocf-0.9.6/requirements.txt
--rw-r--r--   0        0        0    13950 2023-06-17 07:19:16.828575 gcocf-0.9.6/test_everything.py
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 gcocf-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-06-17 07:48:15.940287 gcocf-0.9.7/.example.envrc
+-rw-r--r--   0        0        0      669 2023-06-17 07:48:15.940287 gcocf-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      644 2023-06-17 07:48:15.940287 gcocf-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      501 2023-06-17 07:48:15.940287 gcocf-0.9.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     1076 2023-06-17 07:48:15.940287 gcocf-0.9.7/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1691 2023-06-17 07:48:15.940287 gcocf-0.9.7/.github/workflows/Testing.yml
+-rw-r--r--   0        0        0      103 2023-06-17 07:48:15.940287 gcocf-0.9.7/.gitignore
+-rw-r--r--   0        0        0     5224 2023-06-17 07:48:15.940287 gcocf-0.9.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      203 2023-06-17 07:48:15.940287 gcocf-0.9.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      273 2023-06-17 07:48:15.940287 gcocf-0.9.7/Dockerfile
+-rw-r--r--   0        0        0      144 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/__init__.py
+-rwxr-xr-x   0        0        0    10649 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/__main__.py
+-rw-r--r--   0        0        0     2224 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/api.py
+-rw-r--r--   0        0        0    10419 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/formatters.py
+-rw-r--r--   0        0        0     2369 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/locales/messages.pot
+-rw-r--r--   0        0        0    12638 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/models.py
+-rw-r--r--   0        0        0     1009 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/notifiers.py
+-rw-r--r--   0        0        0     1378 2023-06-17 07:48:15.940287 gcocf-0.9.7/GCoCF/utils.py
+-rw-r--r--   0        0        0     1070 2023-06-17 07:48:15.940287 gcocf-0.9.7/LICENSE.txt
+-rw-r--r--   0        0        0     1317 2023-06-17 07:48:15.940287 gcocf-0.9.7/README.md
+-rw-r--r--   0        0        0     2495 2023-06-17 07:48:15.940287 gcocf-0.9.7/SECURITY.md
+-rw-r--r--   0        0        0    41692 2023-06-17 07:48:15.940287 gcocf-0.9.7/data/full_destruction.json
+-rw-r--r--   0        0        0    77643 2023-06-17 07:48:15.940287 gcocf-0.9.7/data/inWar_40.json
+-rw-r--r--   0        0        0     1059 2023-06-17 07:48:15.944287 gcocf-0.9.7/data/notInWar.json
+-rw-r--r--   0        0        0    24207 2023-06-17 07:48:15.944287 gcocf-0.9.7/data/op_full_destruction.json
+-rw-r--r--   0        0        0    98300 2023-06-17 07:48:15.944287 gcocf-0.9.7/data/warEnded_50.json
+-rw-r--r--   0        0        0      832 2023-06-17 07:48:15.944287 gcocf-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-06-17 07:48:15.944287 gcocf-0.9.7/requirements.txt
+-rw-r--r--   0        0        0    13950 2023-06-17 07:48:15.944287 gcocf-0.9.7/test_everything.py
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 gcocf-0.9.7/PKG-INFO
```

### Comparing `gcocf-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md` & `gcocf-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md` & `gcocf-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/.github/pull_request_template.md` & `gcocf-0.9.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/.github/workflows/Testing.yml` & `gcocf-0.9.7/.github/workflows/Testing.yml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/CODE_OF_CONDUCT.md` & `gcocf-0.9.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/__main__.py` & `gcocf-0.9.7/GCoCF/__main__.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/api.py` & `gcocf-0.9.7/GCoCF/api.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/formatters.py` & `gcocf-0.9.7/GCoCF/formatters.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/locales/messages.pot` & `gcocf-0.9.7/GCoCF/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/models.py` & `gcocf-0.9.7/GCoCF/models.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/notifiers.py` & `gcocf-0.9.7/GCoCF/notifiers.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/GCoCF/utils.py` & `gcocf-0.9.7/GCoCF/utils.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/LICENSE.txt` & `gcocf-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/README.md` & `gcocf-0.9.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
 ```bash
 GCoCF --coc-token {token_here} --clan-tag {tag_here} --webhook-url {url_here}
 ```
 
 ### Extra Options
 
-- ```--mute-attacks```: Mutes notification for every attack
-- ```--warlog```: Logs war activity
+- ```--mute-attacks```: Mutes notification for attacks
+- ```--warlog```: Path to warlog.db
 - ```--loglevel```: Sets the logging level
-- ```--dryrun```: Runs the bot without sending notifications
+- ```--dryrun```: Runs the bot without sending notifications or saving data
 
 ## Running Tests
 
 You can run the test cases by using the following command:
 
 ```bash
 pytest test_everything.py -v --capture=no
```

### Comparing `gcocf-0.9.6/SECURITY.md` & `gcocf-0.9.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/data/full_destruction.json` & `gcocf-0.9.7/data/full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/data/inWar_40.json` & `gcocf-0.9.7/data/inWar_40.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/data/notInWar.json` & `gcocf-0.9.7/data/notInWar.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/data/op_full_destruction.json` & `gcocf-0.9.7/data/op_full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/data/warEnded_50.json` & `gcocf-0.9.7/data/warEnded_50.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/pyproject.toml` & `gcocf-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/test_everything.py` & `gcocf-0.9.7/test_everything.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.6/PKG-INFO` & `gcocf-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCoCF
-Version: 0.9.6
+Version: 0.9.7
 Summary: Clash of Clans war moniting for Discord.
 Home-page: https://github.com/GILLESMaster/GCoCF
 Keywords: coc clashofclans discord
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -71,18 +71,18 @@
 
 ```bash
 GCoCF --coc-token {token_here} --clan-tag {tag_here} --webhook-url {url_here}
 ```
 
 ### Extra Options
 
-- ```--mute-attacks```: Mutes notification for every attack
-- ```--warlog```: Logs war activity
+- ```--mute-attacks```: Mutes notification for attacks
+- ```--warlog```: Path to warlog.db
 - ```--loglevel```: Sets the logging level
-- ```--dryrun```: Runs the bot without sending notifications
+- ```--dryrun```: Runs the bot without sending notifications or saving data
 
 ## Running Tests
 
 You can run the test cases by using the following command:
 
 ```bash
 pytest test_everything.py -v --capture=no
```

