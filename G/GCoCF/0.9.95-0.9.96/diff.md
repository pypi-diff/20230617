# Comparing `tmp/gcocf-0.9.95.tar.gz` & `tmp/gcocf-0.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcocf-0.9.95.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcocf-0.9.96.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcocf-0.9.95.tar` & `gcocf-0.9.96.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      124 2023-06-17 11:13:55.009268 gcocf-0.9.95/.example.envrc
--rw-r--r--   0        0        0      669 2023-06-17 11:13:55.009268 gcocf-0.9.95/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2023-06-17 11:13:55.009268 gcocf-0.9.95/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      501 2023-06-17 11:13:55.009268 gcocf-0.9.95/.github/dependabot.yml
--rw-r--r--   0        0        0     1076 2023-06-17 11:13:55.009268 gcocf-0.9.95/.github/pull_request_template.md
--rw-r--r--   0        0        0     2476 2023-06-17 11:13:55.009268 gcocf-0.9.95/.github/workflows/Testing.yml
--rw-r--r--   0        0        0      118 2023-06-17 11:13:55.009268 gcocf-0.9.95/.gitignore
--rw-r--r--   0        0        0     5224 2023-06-17 11:13:55.009268 gcocf-0.9.95/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      203 2023-06-17 11:13:55.009268 gcocf-0.9.95/CONTRIBUTING.md
--rw-r--r--   0        0        0      273 2023-06-17 11:13:55.009268 gcocf-0.9.95/Dockerfile
--rw-r--r--   0        0        0      145 2023-06-17 11:13:55.009268 gcocf-0.9.95/GCoCF/__init__.py
--rwxr-xr-x   0        0        0    10649 2023-06-17 11:13:55.009268 gcocf-0.9.95/GCoCF/__main__.py
--rw-r--r--   0        0        0     2224 2023-06-17 11:13:55.009268 gcocf-0.9.95/GCoCF/api.py
--rw-r--r--   0        0        0    10419 2023-06-17 11:13:55.009268 gcocf-0.9.95/GCoCF/formatters.py
--rw-r--r--   0        0        0     2369 2023-06-17 11:13:55.009268 gcocf-0.9.95/GCoCF/locales/messages.pot
--rw-r--r--   0        0        0    12638 2023-06-17 11:13:55.013268 gcocf-0.9.95/GCoCF/models.py
--rw-r--r--   0        0        0     1009 2023-06-17 11:13:55.013268 gcocf-0.9.95/GCoCF/notifiers.py
--rw-r--r--   0        0        0     1378 2023-06-17 11:13:55.013268 gcocf-0.9.95/GCoCF/utils.py
--rw-r--r--   0        0        0     1603 2023-06-17 11:13:55.013268 gcocf-0.9.95/GCoCF_Bot/database.py
--rw-r--r--   0        0        0     2532 2023-06-17 11:13:55.013268 gcocf-0.9.95/GCoCF_Bot/service_bot.py
--rw-r--r--   0        0        0     1070 2023-06-17 11:13:55.013268 gcocf-0.9.95/LICENSE.txt
--rw-r--r--   0        0        0     1317 2023-06-17 11:13:55.013268 gcocf-0.9.95/README.md
--rw-r--r--   0        0        0     2495 2023-06-17 11:13:55.013268 gcocf-0.9.95/SECURITY.md
--rw-r--r--   0        0        0    41692 2023-06-17 11:13:55.013268 gcocf-0.9.95/data/full_destruction.json
--rw-r--r--   0        0        0    77643 2023-06-17 11:13:55.013268 gcocf-0.9.95/data/inWar_40.json
--rw-r--r--   0        0        0     1059 2023-06-17 11:13:55.013268 gcocf-0.9.95/data/notInWar.json
--rw-r--r--   0        0        0    24207 2023-06-17 11:13:55.013268 gcocf-0.9.95/data/op_full_destruction.json
--rw-r--r--   0        0        0    98300 2023-06-17 11:13:55.013268 gcocf-0.9.95/data/warEnded_50.json
--rw-r--r--   0        0        0      832 2023-06-17 11:13:55.013268 gcocf-0.9.95/pyproject.toml
--rw-r--r--   0        0        0       54 2023-06-17 11:13:55.013268 gcocf-0.9.95/requirements.txt
--rw-r--r--   0        0        0    13950 2023-06-17 11:13:55.013268 gcocf-0.9.95/test_everything.py
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 gcocf-0.9.95/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-06-17 11:16:38.821978 gcocf-0.9.96/.example.envrc
+-rw-r--r--   0        0        0      669 2023-06-17 11:16:38.821978 gcocf-0.9.96/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      644 2023-06-17 11:16:38.821978 gcocf-0.9.96/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      501 2023-06-17 11:16:38.821978 gcocf-0.9.96/.github/dependabot.yml
+-rw-r--r--   0        0        0     1076 2023-06-17 11:16:38.821978 gcocf-0.9.96/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2476 2023-06-17 11:16:38.821978 gcocf-0.9.96/.github/workflows/Testing.yml
+-rw-r--r--   0        0        0      118 2023-06-17 11:16:38.821978 gcocf-0.9.96/.gitignore
+-rw-r--r--   0        0        0     5224 2023-06-17 11:16:38.825978 gcocf-0.9.96/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      203 2023-06-17 11:16:38.825978 gcocf-0.9.96/CONTRIBUTING.md
+-rw-r--r--   0        0        0      273 2023-06-17 11:16:38.825978 gcocf-0.9.96/Dockerfile
+-rw-r--r--   0        0        0      145 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/__init__.py
+-rwxr-xr-x   0        0        0    10649 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/__main__.py
+-rw-r--r--   0        0        0     2224 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/api.py
+-rw-r--r--   0        0        0    10419 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/formatters.py
+-rw-r--r--   0        0        0     2369 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/locales/messages.pot
+-rw-r--r--   0        0        0    12638 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/models.py
+-rw-r--r--   0        0        0     1009 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/notifiers.py
+-rw-r--r--   0        0        0     1378 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF/utils.py
+-rw-r--r--   0        0        0     1603 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF_Bot/database.py
+-rw-r--r--   0        0        0     2532 2023-06-17 11:16:38.825978 gcocf-0.9.96/GCoCF_Bot/service_bot.py
+-rw-r--r--   0        0        0     1070 2023-06-17 11:16:38.825978 gcocf-0.9.96/LICENSE.txt
+-rw-r--r--   0        0        0     1317 2023-06-17 11:16:38.825978 gcocf-0.9.96/README.md
+-rw-r--r--   0        0        0     2495 2023-06-17 11:16:38.825978 gcocf-0.9.96/SECURITY.md
+-rw-r--r--   0        0        0    41692 2023-06-17 11:16:38.825978 gcocf-0.9.96/data/full_destruction.json
+-rw-r--r--   0        0        0    77643 2023-06-17 11:16:38.825978 gcocf-0.9.96/data/inWar_40.json
+-rw-r--r--   0        0        0     1059 2023-06-17 11:16:38.825978 gcocf-0.9.96/data/notInWar.json
+-rw-r--r--   0        0        0    24207 2023-06-17 11:16:38.825978 gcocf-0.9.96/data/op_full_destruction.json
+-rw-r--r--   0        0        0    98300 2023-06-17 11:16:38.825978 gcocf-0.9.96/data/warEnded_50.json
+-rw-r--r--   0        0        0      832 2023-06-17 11:16:38.825978 gcocf-0.9.96/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-06-17 11:16:38.825978 gcocf-0.9.96/requirements.txt
+-rw-r--r--   0        0        0    13950 2023-06-17 11:16:38.825978 gcocf-0.9.96/test_everything.py
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 gcocf-0.9.96/PKG-INFO
```

### Comparing `gcocf-0.9.95/.github/ISSUE_TEMPLATE/bug_report.md` & `gcocf-0.9.96/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/.github/ISSUE_TEMPLATE/feature_request.md` & `gcocf-0.9.96/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/.github/pull_request_template.md` & `gcocf-0.9.96/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/.github/workflows/Testing.yml` & `gcocf-0.9.96/.github/workflows/Testing.yml`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
           password: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Build and push Docker image
         uses: docker/build-push-action@v2
         with:
           context: .
           push: true
-          tags: ghcr.io/gcocf/GCoCF:latest
+          tags: ghcr.io/gcocf/gcocf:latest
           
   send-summary:
     runs-on: ubuntu-latest
     if: always()
     needs:
       - build-and-test
       - build-and-publish
```

### Comparing `gcocf-0.9.95/CODE_OF_CONDUCT.md` & `gcocf-0.9.96/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/__main__.py` & `gcocf-0.9.96/GCoCF/__main__.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/api.py` & `gcocf-0.9.96/GCoCF/api.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/formatters.py` & `gcocf-0.9.96/GCoCF/formatters.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/locales/messages.pot` & `gcocf-0.9.96/GCoCF/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/models.py` & `gcocf-0.9.96/GCoCF/models.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/notifiers.py` & `gcocf-0.9.96/GCoCF/notifiers.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF/utils.py` & `gcocf-0.9.96/GCoCF/utils.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF_Bot/database.py` & `gcocf-0.9.96/GCoCF_Bot/database.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/GCoCF_Bot/service_bot.py` & `gcocf-0.9.96/GCoCF_Bot/service_bot.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/LICENSE.txt` & `gcocf-0.9.96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/README.md` & `gcocf-0.9.96/README.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/SECURITY.md` & `gcocf-0.9.96/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/data/full_destruction.json` & `gcocf-0.9.96/data/full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/data/inWar_40.json` & `gcocf-0.9.96/data/inWar_40.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/data/notInWar.json` & `gcocf-0.9.96/data/notInWar.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/data/op_full_destruction.json` & `gcocf-0.9.96/data/op_full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/data/warEnded_50.json` & `gcocf-0.9.96/data/warEnded_50.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/pyproject.toml` & `gcocf-0.9.96/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/test_everything.py` & `gcocf-0.9.96/test_everything.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.95/PKG-INFO` & `gcocf-0.9.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCoCF
-Version: 0.9.95
+Version: 0.9.96
 Summary: Clash of Clans war moniting for Discord.
 Home-page: https://github.com/GILLESMaster/GCoCF
 Keywords: coc clashofclans discord
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

