# Comparing `tmp/cardano-nft-vending-machine-0.8.0.tar.gz` & `tmp/cardano-nft-vending-machine-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-k5fu8eyh/cardano-nft-vending-machine-0.8.0.tar", last modified: Sun May 28 19:08:37 2023, max compression
+gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-9qoro_1z/cardano-nft-vending-machine-0.8.1.tar", last modified: Sat Jun 17 14:39:26 2023, max compression
```

## Comparing `cardano-nft-vending-machine-0.8.0.tar` & `cardano-nft-vending-machine-0.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.781260 cardano-nft-vending-machine-0.8.0/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.8.0/LICENSE
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13178 2023-05-28 19:08:37.780821 cardano-nft-vending-machine-0.8.0/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12518 2023-05-27 01:38:09.000000 cardano-nft-vending-machine-0.8.0/README.md
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-28 02:54:06.000000 cardano-nft-vending-machine-0.8.0/pyproject.toml
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-28 19:08:37.781411 cardano-nft-vending-machine-0.8.0/setup.cfg
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.769776 cardano-nft-vending-machine-0.8.0/src/
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.772053 cardano-nft-vending-machine-0.8.0/src/cardano/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.8.0/src/cardano/__init__.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.774672 cardano-nft-vending-machine-0.8.0/src/cardano/wt/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5058 2023-05-27 01:37:27.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/blockfrost.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.775566 cardano-nft-vending-machine-0.8.0/src/cardano/wt/bonuses/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/bonuses/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/bonuses/bogo.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3935 2023-05-27 01:21:05.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/cardano_cli.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     6592 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/mint.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/network.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    15480 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/nft_vending_machine.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      888 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/utxo.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.778161 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/asset_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2511 2023-05-12 17:49:03.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/filesystem.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/no_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/wallet_whitelist.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.780333 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13178 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/requires.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/top_level.txt
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.114508 cardano-nft-vending-machine-0.8.1/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.8.1/LICENSE
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13178 2023-06-17 14:39:26.114246 cardano-nft-vending-machine-0.8.1/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12518 2023-05-27 01:38:09.000000 cardano-nft-vending-machine-0.8.1/README.md
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-06-17 14:38:31.000000 cardano-nft-vending-machine-0.8.1/pyproject.toml
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-06-17 14:39:26.114591 cardano-nft-vending-machine-0.8.1/setup.cfg
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.106834 cardano-nft-vending-machine-0.8.1/src/
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.108307 cardano-nft-vending-machine-0.8.1/src/cardano/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.8.1/src/cardano/__init__.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.110349 cardano-nft-vending-machine-0.8.1/src/cardano/wt/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5058 2023-05-27 01:37:27.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/blockfrost.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.110848 cardano-nft-vending-machine-0.8.1/src/cardano/wt/bonuses/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/bonuses/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/bonuses/bogo.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3935 2023-05-27 01:21:05.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/cardano_cli.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     6592 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/mint.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/network.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    15541 2023-06-17 14:38:12.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/nft_vending_machine.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      888 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/utxo.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.112398 cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/asset_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2511 2023-05-12 17:49:03.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/filesystem.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/no_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/wallet_whitelist.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-06-17 14:39:26.113886 cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13178 2023-06-17 14:39:26.000000 cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-06-17 14:39:26.000000 cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-06-17 14:39:26.000000 cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-06-17 14:39:26.000000 cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/requires.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-06-17 14:39:26.000000 cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/top_level.txt
```

### Comparing `cardano-nft-vending-machine-0.8.0/LICENSE` & `cardano-nft-vending-machine-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/PKG-INFO` & `cardano-nft-vending-machine-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.8.0 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.8.1 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
```

### Comparing `cardano-nft-vending-machine-0.8.0/README.md` & `cardano-nft-vending-machine-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/pyproject.toml` & `cardano-nft-vending-machine-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardano-nft-vending-machine"
-version = "0.8.0"
+version = "0.8.1"
 
 description = "Library to perform NFT mints automatically on the Cardano blockchain"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/blockfrost.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/blockfrost.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/cardano_cli.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/cardano_cli.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/mint.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/mint.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/nft_vending_machine.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/nft_vending_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         # PAY THE USER'S REBATE AFTER NFTs CALCULATED
         all_names = [name for name_lst in nft_policy_map.values() for name in name_lst]
         total_name_chars = sum([len(name) for name in all_names])
         user_rebate = Mint.RebateCalculator.calculate_rebate_for(len(nft_policy_map.keys()), len(all_names), total_name_chars)
         print(f"Minimum rebate to user is {user_rebate}")
 
         # DEDUCT REBATES AND FEES FROM PROFIT IF ADA-ONLY MINT, OTHERWISE FROM USER
+        print(f"Checkpoint [profit {profit_ada}]: {payees}")
         payees[input_addr][Balance.LOVELACE_POLICY] = user_rebate
         if profit_ada and len(payees[self.profit_addr]) == 1:
             payees[self.profit_addr][Balance.LOVELACE_POLICY] -= (user_rebate + fee)
         elif user_rebate > remaining_ada.lovelace:
             raise ValueError(f"USER SENT {remaining_ada.lovelace} WHICH CAN'T COVER REBATE OF {user_rebate} (FREE MINT?)")
         else:
             remaining_ada.lovelace -= (user_rebate + fee)
```

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/utxo.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/asset_whitelist.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/asset_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/filesystem.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/filesystem.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/no_whitelist.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/no_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/wallet_whitelist.py` & `cardano-nft-vending-machine-0.8.1/src/cardano/wt/whitelist/wallet_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO` & `cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.8.0 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.8.1 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
```

### Comparing `cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt` & `cardano-nft-vending-machine-0.8.1/src/cardano_nft_vending_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

