# Comparing `tmp/chia_py_rpc-0.0.6.tar.gz` & `tmp/chia_py_rpc-0.0.7.tar.gz`

## Comparing `chia_py_rpc-0.0.6.tar` & `chia_py_rpc-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/.vscode/launch.json
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/src/chia_py_rpc/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/src/chia_py_rpc/rpc_connect.py
--rw-r--r--   0        0        0    80559 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/src/chia_py_rpc/wallet.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/LICENSE
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/README.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/src/chia_py_rpc/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/src/chia_py_rpc/rpc_connect.py
+-rw-r--r--   0        0        0    80546 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/src/chia_py_rpc/wallet.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.7/PKG-INFO
```

### Comparing `chia_py_rpc-0.0.6/src/chia_py_rpc/rpc_connect.py` & `chia_py_rpc-0.0.7/src/chia_py_rpc/rpc_connect.py`

 * *Files identical despite different names*

### Comparing `chia_py_rpc-0.0.6/src/chia_py_rpc/wallet.py` & `chia_py_rpc-0.0.7/src/chia_py_rpc/wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,16 +413,16 @@
             "excluded_coins": excluded_coins,
             "max_coin_amount": max_coin_amount,
             "exclude_coin_amounts": exclude_coin_amounts
         }
         result = self.__chia_rpc__.submit("select_coins", json.dumps(data))
         return json.loads(result)
 
-    def take_offer(self, offer, fee, min_coin_amount,
-                   max_coin_amount=None, solver=None, reuse_puzhash=True):
+    def take_offer(self, offer, fee, min_coin_amount=0,
+                   max_coin_amount=0, solver=None, reuse_puzhash=True):
         """Takes an offer in CAT Wallet using RPC.
 
         Args:
             offer (str): Trade ID of the offer to take
             fee (int): Fee to offer in addition to the original offer
             min_coin_amount (int): Minimum amount of coins to use for solving the puzzle
             max_coin_amount (int): Maximum amount of coins to use for solving the puzzle (default: None)
@@ -2126,17 +2126,17 @@
 
         # Use the submit method of WalletRPCConnect instance to make the Chia
         # RPC call with the payload
         result = self.__chia_rpc__.submit("nft_add_uri", json.dumps(payload))
 
         # Parse the JSON response and return the result
         return json.loads(result)
-    
-    
-    
+
+
+
 
 
 class Coins:
     def __init__(self, url: str = None, cert: str = None):
         """
         Initialize Coins instance.
```

### Comparing `chia_py_rpc-0.0.6/LICENSE` & `chia_py_rpc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chia_py_rpc-0.0.6/README.md` & `chia_py_rpc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chia_py_rpc-0.0.6/pyproject.toml` & `chia_py_rpc-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chia_py_rpc"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="L4bb3rs", email="king@the300.net" },
 ]
 description = "Chia-Py-RPC is a Python library that provides a convenient way to interact with the Chia blockchain using the Chia RPC (Remote Procedure Call) protocol."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `chia_py_rpc-0.0.6/PKG-INFO` & `chia_py_rpc-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia_py_rpc
-Version: 0.0.6
+Version: 0.0.7
 Summary: Chia-Py-RPC is a Python library that provides a convenient way to interact with the Chia blockchain using the Chia RPC (Remote Procedure Call) protocol.
 Project-URL: Homepage, https://github.com/L4bb3rs/Chia-Py-RPC
 Project-URL: Bug Tracker, https://github.com/L4bb3rs/Chia-Py-RPC
 Author-email: L4bb3rs <king@the300.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

