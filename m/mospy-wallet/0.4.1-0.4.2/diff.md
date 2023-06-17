# Comparing `tmp/mospy_wallet-0.4.1.tar.gz` & `tmp/mospy_wallet-0.4.2.tar.gz`

## Comparing `mospy_wallet-0.4.1.tar` & `mospy_wallet-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/requirements.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/setup.cfg
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/CNAME
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/account.md
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/examples.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/index.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/transaction.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/clients/grpcclient.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/clients/httpclient.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/clients/index.md
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/docs/transaction/types.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/examples/builtin_staking.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/examples/delegate.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/examples/evmos_transfer.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/examples/ibc_transfer.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/examples/osmosis_trade.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/examples/set_withdraw_address.py
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/Account.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/Transaction.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/utils.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/_transactions/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/_transactions/_delegate.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/_transactions/_transfer.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/_transactions/_undelegate.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/_transactions/_withdraw_reward.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/clients/GRPCClient.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/clients/HTTPClient.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/clients/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/src/mospy/exceptions/clients.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/tests/test_account.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/tests/test_eth.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/tests/test_transaction.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/tests/clients/test_grpcclient.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/tests/clients/test_httpclient.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/.gitignore
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 mospy_wallet-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/requirements.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/setup.cfg
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/CNAME
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/account.md
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/examples.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/index.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/transaction.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/clients/grpcclient.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/clients/httpclient.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/clients/index.md
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/docs/transaction/types.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/examples/builtin_staking.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/examples/delegate.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/examples/evmos_transfer.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/examples/ibc_transfer.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/examples/osmosis_trade.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/examples/set_withdraw_address.py
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/Account.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/Transaction.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/utils.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/_transactions/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/_transactions/_delegate.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/_transactions/_transfer.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/_transactions/_undelegate.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/_transactions/_withdraw_reward.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/clients/GRPCClient.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/clients/HTTPClient.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/clients/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/src/mospy/exceptions/clients.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/tests/test_account.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/tests/test_eth.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/tests/test_transaction.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/tests/clients/test_grpcclient.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/tests/clients/test_httpclient.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/.gitignore
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/README.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 mospy_wallet-0.4.2/PKG-INFO
```

### Comparing `mospy_wallet-0.4.1/.github/workflows/tests.yaml` & `mospy_wallet-0.4.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/docs/examples.md` & `mospy_wallet-0.4.2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/docs/index.md` & `mospy_wallet-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/docs/transaction/types.md` & `mospy_wallet-0.4.2/docs/transaction/types.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/examples/builtin_staking.py` & `mospy_wallet-0.4.2/examples/builtin_staking.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/examples/delegate.py` & `mospy_wallet-0.4.2/examples/delegate.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/examples/evmos_transfer.py` & `mospy_wallet-0.4.2/examples/evmos_transfer.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/examples/ibc_transfer.py` & `mospy_wallet-0.4.2/examples/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/examples/osmosis_trade.py` & `mospy_wallet-0.4.2/examples/osmosis_trade.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/examples/set_withdraw_address.py` & `mospy_wallet-0.4.2/examples/set_withdraw_address.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/Account.py` & `mospy_wallet-0.4.2/src/mospy/Account.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/Transaction.py` & `mospy_wallet-0.4.2/src/mospy/Transaction.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/utils.py` & `mospy_wallet-0.4.2/src/mospy/utils.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/_transactions/_delegate.py` & `mospy_wallet-0.4.2/src/mospy/_transactions/_delegate.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/_transactions/_transfer.py` & `mospy_wallet-0.4.2/src/mospy/_transactions/_transfer.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/_transactions/_undelegate.py` & `mospy_wallet-0.4.2/src/mospy/_transactions/_undelegate.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/_transactions/_withdraw_reward.py` & `mospy_wallet-0.4.2/src/mospy/_transactions/_withdraw_reward.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/clients/GRPCClient.py` & `mospy_wallet-0.4.2/src/mospy/clients/GRPCClient.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/src/mospy/clients/HTTPClient.py` & `mospy_wallet-0.4.2/src/mospy/clients/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/tests/test_account.py` & `mospy_wallet-0.4.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/tests/test_eth.py` & `mospy_wallet-0.4.2/tests/test_eth.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/tests/test_transaction.py` & `mospy_wallet-0.4.2/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/tests/clients/test_grpcclient.py` & `mospy_wallet-0.4.2/tests/clients/test_grpcclient.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/tests/clients/test_httpclient.py` & `mospy_wallet-0.4.2/tests/clients/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/README.md` & `mospy_wallet-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.4.1/pyproject.toml` & `mospy_wallet-0.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mospy-wallet"
-version = "0.4.1"
+version = "0.4.2"
 description = "This package is a fork of cosmospy and is a light framework for the cosmos ecosystem"
 authors = [
     { name = "ctrl-felix", email = "dev@ctrl-felix.de" },
 ]
 readme = "README.md"
 keywords = ["cosmospy", "mospy", "cosmos"]
 license = {text = "BSD 3-Clause License"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "protobuf==4.22.1",
+    "protobuf~=4.22.1",
     "grpcio~=1.51.3",
     "httpx~=0.23.0",
     "cosmospy-protobuf>=0.2.0",
     "ecdsa==0.17.0",
     "bech32==1.2.0",
     "mnemonic==0.20",
     "hdwallets==0.1.2",
```

### Comparing `mospy_wallet-0.4.1/PKG-INFO` & `mospy_wallet-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mospy-wallet
-Version: 0.4.1
+Version: 0.4.2
 Summary: This package is a fork of cosmospy and is a light framework for the cosmos ecosystem
 Project-URL: Homepage, https://github.com/ctrl-Felix/mospy/
 Project-URL: Bug Tracker, https://github.com/ctrl-Felix/mospy/issues
 Author-email: ctrl-felix <dev@ctrl-felix.de>
 License: BSD 3-Clause License
 Keywords: cosmos,cosmospy,mospy
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Requires-Dist: bech32==1.2.0
 Requires-Dist: cosmospy-protobuf>=0.2.0
 Requires-Dist: ecdsa==0.17.0
 Requires-Dist: grpcio~=1.51.3
 Requires-Dist: hdwallets==0.1.2
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: mnemonic==0.20
-Requires-Dist: protobuf==4.22.1
+Requires-Dist: protobuf~=4.22.1
 Requires-Dist: pysha3==1.0.2; python_version < '3.9'
 Requires-Dist: safe-pysha3==1.0.3; python_version >= '3.9'
 Description-Content-Type: text/markdown
 
 # MosPy
 
 MosPy is a fork of the cosmospy library and aims to be a versatile transaction signing library for the whole cosmos ecosystem.
```

