# Comparing `tmp/gcocf-0.9.91.tar.gz` & `tmp/gcocf-0.9.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcocf-0.9.91.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcocf-0.9.94.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcocf-0.9.91.tar` & `gcocf-0.9.94.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0      124 2023-06-17 08:11:24.753582 gcocf-0.9.91/.example.envrc
--rw-r--r--   0        0        0      669 2023-06-17 08:11:24.753582 gcocf-0.9.91/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2023-06-17 08:11:24.753582 gcocf-0.9.91/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      501 2023-06-17 08:11:24.753582 gcocf-0.9.91/.github/dependabot.yml
--rw-r--r--   0        0        0     1076 2023-06-17 08:11:24.753582 gcocf-0.9.91/.github/pull_request_template.md
--rw-r--r--   0        0        0     1883 2023-06-17 08:11:24.753582 gcocf-0.9.91/.github/workflows/Testing.yml
--rw-r--r--   0        0        0      103 2023-06-17 08:11:24.753582 gcocf-0.9.91/.gitignore
--rw-r--r--   0        0        0     5224 2023-06-17 08:11:24.753582 gcocf-0.9.91/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      203 2023-06-17 08:11:24.753582 gcocf-0.9.91/CONTRIBUTING.md
--rw-r--r--   0        0        0      273 2023-06-17 08:11:24.753582 gcocf-0.9.91/Dockerfile
--rw-r--r--   0        0        0      145 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/__init__.py
--rwxr-xr-x   0        0        0    10649 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/__main__.py
--rw-r--r--   0        0        0     2224 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/api.py
--rw-r--r--   0        0        0    10419 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/formatters.py
--rw-r--r--   0        0        0     2369 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/locales/messages.pot
--rw-r--r--   0        0        0    12638 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/models.py
--rw-r--r--   0        0        0     1009 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/notifiers.py
--rw-r--r--   0        0        0     1378 2023-06-17 08:11:24.753582 gcocf-0.9.91/GCoCF/utils.py
--rw-r--r--   0        0        0     1070 2023-06-17 08:11:24.753582 gcocf-0.9.91/LICENSE.txt
--rw-r--r--   0        0        0     1317 2023-06-17 08:11:24.753582 gcocf-0.9.91/README.md
--rw-r--r--   0        0        0     2495 2023-06-17 08:11:24.753582 gcocf-0.9.91/SECURITY.md
--rw-r--r--   0        0        0    41692 2023-06-17 08:11:24.757582 gcocf-0.9.91/data/full_destruction.json
--rw-r--r--   0        0        0    77643 2023-06-17 08:11:24.757582 gcocf-0.9.91/data/inWar_40.json
--rw-r--r--   0        0        0     1059 2023-06-17 08:11:24.757582 gcocf-0.9.91/data/notInWar.json
--rw-r--r--   0        0        0    24207 2023-06-17 08:11:24.757582 gcocf-0.9.91/data/op_full_destruction.json
--rw-r--r--   0        0        0    98300 2023-06-17 08:11:24.757582 gcocf-0.9.91/data/warEnded_50.json
--rw-r--r--   0        0        0      832 2023-06-17 08:11:24.757582 gcocf-0.9.91/pyproject.toml
--rw-r--r--   0        0        0       54 2023-06-17 08:11:24.757582 gcocf-0.9.91/requirements.txt
--rw-r--r--   0        0        0    13950 2023-06-17 08:11:24.757582 gcocf-0.9.91/test_everything.py
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 gcocf-0.9.91/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-06-17 11:08:57.785350 gcocf-0.9.94/.example.envrc
+-rw-r--r--   0        0        0      669 2023-06-17 11:08:57.785350 gcocf-0.9.94/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      644 2023-06-17 11:08:57.785350 gcocf-0.9.94/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      501 2023-06-17 11:08:57.785350 gcocf-0.9.94/.github/dependabot.yml
+-rw-r--r--   0        0        0     1076 2023-06-17 11:08:57.785350 gcocf-0.9.94/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2495 2023-06-17 11:08:57.785350 gcocf-0.9.94/.github/workflows/Testing.yml
+-rw-r--r--   0        0        0      118 2023-06-17 11:08:57.785350 gcocf-0.9.94/.gitignore
+-rw-r--r--   0        0        0     5224 2023-06-17 11:08:57.785350 gcocf-0.9.94/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      203 2023-06-17 11:08:57.785350 gcocf-0.9.94/CONTRIBUTING.md
+-rw-r--r--   0        0        0      273 2023-06-17 11:08:57.785350 gcocf-0.9.94/Dockerfile
+-rw-r--r--   0        0        0      145 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/__init__.py
+-rwxr-xr-x   0        0        0    10649 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/__main__.py
+-rw-r--r--   0        0        0     2224 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/api.py
+-rw-r--r--   0        0        0    10419 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/formatters.py
+-rw-r--r--   0        0        0     2369 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/locales/messages.pot
+-rw-r--r--   0        0        0    12638 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/models.py
+-rw-r--r--   0        0        0     1009 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/notifiers.py
+-rw-r--r--   0        0        0     1378 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF/utils.py
+-rw-r--r--   0        0        0     1603 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF_Bot/database.py
+-rw-r--r--   0        0        0     2532 2023-06-17 11:08:57.785350 gcocf-0.9.94/GCoCF_Bot/service_bot.py
+-rw-r--r--   0        0        0     1070 2023-06-17 11:08:57.785350 gcocf-0.9.94/LICENSE.txt
+-rw-r--r--   0        0        0     1317 2023-06-17 11:08:57.785350 gcocf-0.9.94/README.md
+-rw-r--r--   0        0        0     2495 2023-06-17 11:08:57.785350 gcocf-0.9.94/SECURITY.md
+-rw-r--r--   0        0        0    41692 2023-06-17 11:08:57.785350 gcocf-0.9.94/data/full_destruction.json
+-rw-r--r--   0        0        0    77643 2023-06-17 11:08:57.785350 gcocf-0.9.94/data/inWar_40.json
+-rw-r--r--   0        0        0     1059 2023-06-17 11:08:57.785350 gcocf-0.9.94/data/notInWar.json
+-rw-r--r--   0        0        0    24207 2023-06-17 11:08:57.785350 gcocf-0.9.94/data/op_full_destruction.json
+-rw-r--r--   0        0        0    98300 2023-06-17 11:08:57.785350 gcocf-0.9.94/data/warEnded_50.json
+-rw-r--r--   0        0        0      832 2023-06-17 11:08:57.785350 gcocf-0.9.94/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-06-17 11:08:57.789350 gcocf-0.9.94/requirements.txt
+-rw-r--r--   0        0        0    13950 2023-06-17 11:08:57.789350 gcocf-0.9.94/test_everything.py
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 gcocf-0.9.94/PKG-INFO
```

### Comparing `gcocf-0.9.91/.github/ISSUE_TEMPLATE/bug_report.md` & `gcocf-0.9.94/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/.github/ISSUE_TEMPLATE/feature_request.md` & `gcocf-0.9.94/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/.github/pull_request_template.md` & `gcocf-0.9.94/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/.github/workflows/Testing.yml` & `gcocf-0.9.94/.github/workflows/Testing.yml`

 * *Files 10% similar despite different names*

```diff
@@ -45,38 +45,59 @@
         with:
           python-version: '3.11'
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flit
-          pip install pyarmor
+        #  pip install pyarmor
 
-      - name: Obfuscate code
-        run: |
-          pyarmor init GCoCF/
-          pyarmor build GCoCF/
-          pyarmor obfuscate GCoCF/
+      #- name: Obfuscate code
+      #  run: |
+      #    pyarmor gen -r GCoCF/
 
       - name: Build package
         run: |
           flit build
 
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
 
+  build-and-contain:
+    needs: [build-and-test, build-and-publish]
+    runs-on: ubuntu-latest
+    if: github.event_name == 'push' && github.ref == 'refs/heads/master'
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Log in to GitHub Container Registry
+        uses: docker/login-action@v1
+        with:
+          registry: ghcr.io
+          username: ${{ github.actor }}
+          password: ${{ secrets.GITHUB_TOKEN }}
+
+      - name: Build and push Docker image
+        uses: docker/build-push-action@v2
+        with:
+          context: .
+          push: true
+          tags: ghcr.io/${{ github.repository }}/GCoCF:latest
+          
   send-summary:
     runs-on: ubuntu-latest
     if: always()
     needs:
       - build-and-test
       - build-and-publish
+      - build-and-contain
 
     steps:
       - name: Send Test Summary
         uses: CalmDownVal/webhook-summary@v1
         with:
           token: ${{ secrets.TOKEN }}
           url: ${{ secrets.WEBHOOK_URL }}
```

### Comparing `gcocf-0.9.91/CODE_OF_CONDUCT.md` & `gcocf-0.9.94/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/__main__.py` & `gcocf-0.9.94/GCoCF/__main__.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/api.py` & `gcocf-0.9.94/GCoCF/api.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/formatters.py` & `gcocf-0.9.94/GCoCF/formatters.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/locales/messages.pot` & `gcocf-0.9.94/GCoCF/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/models.py` & `gcocf-0.9.94/GCoCF/models.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/notifiers.py` & `gcocf-0.9.94/GCoCF/notifiers.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/GCoCF/utils.py` & `gcocf-0.9.94/GCoCF/utils.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/LICENSE.txt` & `gcocf-0.9.94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/README.md` & `gcocf-0.9.94/README.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/SECURITY.md` & `gcocf-0.9.94/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/data/full_destruction.json` & `gcocf-0.9.94/data/full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/data/inWar_40.json` & `gcocf-0.9.94/data/inWar_40.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/data/notInWar.json` & `gcocf-0.9.94/data/notInWar.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/data/op_full_destruction.json` & `gcocf-0.9.94/data/op_full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/data/warEnded_50.json` & `gcocf-0.9.94/data/warEnded_50.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/pyproject.toml` & `gcocf-0.9.94/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/test_everything.py` & `gcocf-0.9.94/test_everything.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.91/PKG-INFO` & `gcocf-0.9.94/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCoCF
-Version: 0.9.91
+Version: 0.9.94
 Summary: Clash of Clans war moniting for Discord.
 Home-page: https://github.com/GILLESMaster/GCoCF
 Keywords: coc clashofclans discord
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

