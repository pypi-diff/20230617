# Comparing `tmp/skale.py-5.8b2.tar.gz` & `tmp/skale.py-6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skale.py-5.8b2.tar", last modified: Fri Jun 16 16:26:49 2023, max compression
+gzip compressed data, was "dist/skale.py-6.0.dev0.tar", last modified: Wed Jun  7 19:06:23 2023, max compression
```

## Comparing `skale.py-5.8b2.tar` & `skale.py-6.0.dev0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-16 16:25:21.000000 skale.py-5.8b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 16:25:21.000000 skale.py-5.8b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-16 16:26:49.000000 skale.py-5.8b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-16 16:25:21.000000 skale.py-5.8b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:26:49.000000 skale.py-5.8b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-16 16:26:49.000000 skale.py-5.8b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/contracts/allocator/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/allocator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/allocator/allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/allocator/escrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/base_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/contract_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/contracts/ima/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/ima/linker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/contracts/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/bounty_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/constants_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/contracts/manager/delegation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/delegation_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/delegation_period_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/distributor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/slashing_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/token_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/delegation/validator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/dkg.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/node_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/punisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/schains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/schains_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/sync_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/contracts/manager/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/test/time_helpers_with_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/contracts/manager/wallets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/dataclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/dataclasses/delegation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/dataclasses/node_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/dataclasses/schain_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/dataclasses/skaled_ports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/schain_config/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/schain_config/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/schain_config/ports_allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/schain_config/rotation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/skale_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/skale_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/skale_ima.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/skale_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/transactions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/transactions/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/transactions/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/abi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/account_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contract_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contract_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/utils/contracts_provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contracts_provision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contracts_provision/allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contracts_provision/fake_multisig_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contracts_provision/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/contracts_provision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/utils/random_names/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/random_names/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/random_names/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/random_names/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale/wallets/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/ledger_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/redis_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/rpc_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/sgx_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-16 16:25:21.000000 skale.py-5.8b2/skale/wallets/web3_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 16:26:49.000000 skale.py-5.8b2/skale.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:49.000000 skale.py-5.8b2/tests/schain_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:21.000000 skale.py-5.8b2/tests/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 16:25:21.000000 skale.py-5.8b2/tests/schain_config/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-16 16:25:21.000000 skale.py-5.8b2/tests/schain_config/ports_allocation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-07 19:06:22.000000 skale.py-6.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/contracts/allocator/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/allocator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/allocator/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/allocator/escrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/base_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/contract_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/contracts/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/ima/linker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/contracts/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/bounty_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/constants_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/delegation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/delegation_period_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/distributor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/slashing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/token_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/delegation/validator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/dkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/node_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/punisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/schains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/schains_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/sync_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/contracts/manager/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/test/time_helpers_with_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/contracts/manager/wallets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/dataclasses/delegation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/dataclasses/node_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/dataclasses/schain_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/dataclasses/skaled_ports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/schain_config/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/schain_config/ports_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/schain_config/rotation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/skale_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/skale_ima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/skale_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/transactions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/transactions/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/transactions/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/abi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/account_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contract_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contract_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/utils/contracts_provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contracts_provision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contracts_provision/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contracts_provision/fake_multisig_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contracts_provision/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/contracts_provision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/utils/random_names/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/random_names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/random_names/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/random_names/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale/wallets/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/ledger_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/redis_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/rpc_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/sgx_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/skale/wallets/web3_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/skale.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:06:23.000000 skale.py-6.0.dev0/tests/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/tests/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/tests/schain_config/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-07 19:04:44.000000 skale.py-6.0.dev0/tests/schain_config/ports_allocation_test.py
```

### Comparing `skale.py-5.8b2/LICENSE` & `skale.py-6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/PKG-INFO` & `skale.py-6.0.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 5.8b2
+Version: 6.0.dev0
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: skale
```

### Comparing `skale.py-5.8b2/README.md` & `skale.py-6.0.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![codecov](https://codecov.io/gh/skalenetwork/skale.py/branch/develop/graph/badge.svg?token=XHiZ15ijpa)](https://codecov.io/gh/skalenetwork/skale.py)
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/skalenetwork/skale.py)
 [![Discord](https://img.shields.io/discord/534485763354787851.svg)](https://discord.gg/vvUtWJB)
 
 Python client library used in SKALE network components.
 
 - Python 3.7+ support
-- Compatibility with `web3.py` v5
+- Compatibility with `web3.py` v6
 
 ### Installation
 
 ```bash
 pip install skale.py
 ```
```

### Comparing `skale.py-5.8b2/setup.py` & `skale.py-6.0.dev0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,44 +12,44 @@
         "importlib-metadata<5.0"
     ],
     'dev': [
         "bumpversion==0.6.0",
         "click==7.1.2",
         "freezegun==1.2.2",
         "mock==4.0.2",
-        "pytest==5.4.3",
+        "pytest==7.1.3",
         "pytest-cov==2.8.1",
         "Random-Word==1.0.4",
-        "twine==4.0.2",
+        "twine==3.1.1",
         "when-changed"
     ],
     'hw-wallet': [
         "ledgerblue==0.1.47"
     ]
 }
 
 extras_require['dev'] = (
     extras_require['linter'] + extras_require['dev'] + extras_require['hw-wallet']
 )
 
 setup(
     name='skale.py',
-    version='5.8b2',
+    version='6.0dev0',
     description='SKALE client tools',
     long_description_markdown_filename='README.md',
     author='SKALE Labs',
     author_email='support@skalelabs.com',
     url='https://github.com/skalenetwork/skale.py',
     include_package_data=True,
     install_requires=[
-        "web3==5.31.1",
         "asyncio==3.4.3",
         "pyyaml==6.0",
-        "sgx.py==0.8dev7",
-        "redis==4.3.4"
+        "sgx.py==0.9dev0",
+        "redis==4.4.4",
+        "web3==6.3.0"
     ],
 
     python_requires='>=3.7,<4',
     extras_require=extras_require,
 
     keywords='skale',
     packages=find_packages(exclude=['tests']),
```

### Comparing `skale.py-5.8b2/skale/config.py` & `skale.py-6.0.dev0/skale/config.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/allocator/allocator.py` & `skale.py-6.0.dev0/skale/contracts/allocator/allocator.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE Allocator Core Escrow methods """
 
 from enum import IntEnum
 
 from skale.contracts.base_contract import BaseContract, transaction_method
+from skale.transactions.exceptions import ContractLogicError
 from skale.transactions.result import TxRes
 from skale.utils.helper import format_fields
 
 
 PLAN_FIELDS = [
     'totalVestingDuration',
     'vestingCliff',
@@ -153,15 +154,15 @@
     def get_all_plans(self) -> dict:
         plans = []
         for i in range(1, MAX_NUM_OF_PLANS):
             try:
                 plan = self.get_plan(i)
                 plan['planId'] = i
                 plans.append(plan)
-            except ValueError:
+            except (ContractLogicError, ValueError):
                 break
         return plans
 
     def calculate_vested_amount(self, address: str) -> int:
         return self.contract.functions.calculateVestedAmount(address).call()
 
     def get_finish_vesting_time(self, address: str) -> int:
```

### Comparing `skale.py-5.8b2/skale/contracts/allocator/escrow.py` & `skale.py-6.0.dev0/skale/contracts/allocator/escrow.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/base_contract.py` & `skale.py-6.0.dev0/skale/contracts/base_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     return wrapper
 
 
 class BaseContract:
     def __init__(self, skale, name, address, abi):
         self.skale = skale
         self.name = name
-        self.address = Web3.toChecksumAddress(address)
+        self.address = Web3.to_checksum_address(address)
         self.contract = skale.web3.eth.contract(address=self.address, abi=abi)
 
     def __getattr__(self, attr):
         """Fallback for contract calls"""
         logger.debug("Calling contract function: %s", attr)
 
         def wrapper(*args, **kw):
```

### Comparing `skale.py-5.8b2/skale/contracts/contract_manager.py` & `skale.py-6.0.dev0/skale/contracts/contract_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/ima/linker.py` & `skale.py-6.0.dev0/skale/contracts/ima/linker.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/__init__.py` & `skale.py-6.0.dev0/skale/contracts/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/bounty_v2.py` & `skale.py-6.0.dev0/skale/contracts/manager/bounty_v2.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/constants_holder.py` & `skale.py-6.0.dev0/skale/contracts/manager/constants_holder.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/delegation/delegation_controller.py` & `skale.py-6.0.dev0/skale/contracts/manager/delegation/delegation_controller.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/delegation/delegation_period_manager.py` & `skale.py-6.0.dev0/skale/contracts/manager/delegation/delegation_period_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/delegation/distributor.py` & `skale.py-6.0.dev0/skale/contracts/manager/delegation/distributor.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/delegation/slashing_table.py` & `skale.py-6.0.dev0/skale/contracts/manager/delegation/slashing_table.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/delegation/token_state.py` & `skale.py-6.0.dev0/skale/contracts/manager/delegation/token_state.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/delegation/validator_service.py` & `skale.py-6.0.dev0/skale/contracts/manager/delegation/validator_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.registerValidator(
             name, description, fee_rate, min_delegation_amount)
 
     def get_link_node_signature(self, validator_id: int) -> str:
-        unsigned_hash = Web3.soliditySha3(['uint256'], [validator_id])
+        unsigned_hash = Web3.solidity_keccak(['uint256'], [validator_id])
         signed_hash = self.skale.wallet.sign_hash(unsigned_hash.hex())
         return signed_hash.signature.hex()
 
     @transaction_method
     def link_node_address(self, node_address: str, signature: str) -> TxRes:
         """Link node address to your validator account.
```

### Comparing `skale.py-5.8b2/skale/contracts/manager/dkg.py` & `skale.py-6.0.dev0/skale/contracts/manager/dkg.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/groups.py` & `skale.py-6.0.dev0/skale/contracts/manager/groups.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/key_storage.py` & `skale.py-6.0.dev0/skale/contracts/manager/key_storage.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/manager.py` & `skale.py-6.0.dev0/skale/contracts/manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE manager operations """
 
 
 import logging
 import socket
 
-from eth_abi import encode_abi
+from eth_abi import encode
 
 from skale.contracts.base_contract import BaseContract, transaction_method
 from skale.utils import helper
 from skale.transactions.result import TxRes
 from skale.dataclasses.schain_options import (
     SchainOptions, get_default_schain_options
 )
@@ -79,15 +79,15 @@
         skale_nonce = helper.generate_nonce()
 
         if schain_originator is None:
             schain_originator = self.skale.wallet.address
         if not options:
             options = get_default_schain_options()
 
-        tx_data = encode_abi(
+        tx_data = encode(
             ['(uint,uint8,uint16,string,address,(string,bytes)[])'],
             [(lifetime, type_of_nodes, skale_nonce, name, schain_originator, options.to_tuples())]
         )
 
         return self.skale.token.contract.functions.send(
             self.address,
             deposit,
```

### Comparing `skale.py-5.8b2/skale/contracts/manager/node_rotation.py` & `skale.py-6.0.dev0/skale/contracts/manager/node_rotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     def is_finish_ts_reached(self, schain_name) -> bool:
         rotation = self.skale.node_rotation.get_rotation_obj(schain_name)
         schain_finish_ts = self.get_schain_finish_ts(rotation.leaving_node_id, schain_name)
 
         if not schain_finish_ts:
             schain_finish_ts = 0
 
-        latest_block = self.skale.web3.eth.getBlock('latest')
+        latest_block = self.skale.web3.eth.get_block('latest')
         current_ts = latest_block['timestamp']
 
         logger.info(f'current_ts: {current_ts}, schain_finish_ts: {schain_finish_ts}')
         return current_ts > schain_finish_ts
 
     def wait_for_new_node(self, schain_name):
         schain_id = self.schains.name_to_id(schain_name)
@@ -129,11 +129,11 @@
     def debugger_role(self):
         return self.contract.functions.DEBUGGER_ROLE().call()
 
     def get_previous_node(self, schain_name: str, node_id: int) -> int:
         schain_id = self.schains.name_to_id(schain_name)
         try:
             return self.contract.functions.getPreviousNode(schain_id, node_id).call()
-        except ContractLogicError as e:
+        except (ContractLogicError, ValueError) as e:
             if NO_PREVIOUS_NODE_EXCEPTION_TEXT in str(e):
                 return None
             raise e
```

### Comparing `skale.py-5.8b2/skale/contracts/manager/nodes.py` & `skale.py-6.0.dev0/skale/contracts/manager/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ Nodes.sol functions """
 
 import socket
 from enum import IntEnum
 
 from Crypto.Hash import keccak
-from web3.exceptions import BadFunctionCallOutput
+from web3.exceptions import BadFunctionCallOutput, ContractLogicError
 
 from skale.contracts.base_contract import BaseContract, transaction_method
 from skale.transactions.result import TxRes
 
 from skale.utils.exceptions import InvalidNodeIdError
 from skale.utils.helper import format_fields
 
@@ -43,15 +43,15 @@
     IN_MAINTENANCE = 3
 
 
 class Nodes(BaseContract):
     def __get_raw(self, node_id):
         try:
             return self.contract.functions.nodes(node_id).call()
-        except (ValueError, BadFunctionCallOutput):
+        except (ContractLogicError, ValueError, BadFunctionCallOutput):
             raise InvalidNodeIdError(node_id)
 
     def __get_raw_w_pk(self, node_id):
         raw_node_struct = self.__get_raw(node_id)
         raw_node_struct.append(self.get_node_public_key(node_id))
         return raw_node_struct
 
@@ -87,15 +87,15 @@
             self.get(node_id)['ip']
             for node_id in range(0, nodes_number)
             if self.get_node_status(node_id) == NodeStatus.ACTIVE
         ]
 
     def name_to_id(self, name):
         keccak_hash = keccak.new(data=name.encode("utf8"), digest_bits=256)
-        return keccak_hash.hexdigest()
+        return keccak_hash.digest()
 
     def is_node_name_available(self, name):
         node_id = self.name_to_id(name)
         return not self.contract.functions.nodesNameCheck(node_id).call()
 
     def is_node_ip_available(self, ip):
         ip_bytes = socket.inet_aton(ip)
@@ -104,33 +104,33 @@
     def node_name_to_index(self, name):
         name_hash = self.name_to_id(name)
         return self.contract.functions.nodesNameToIndex(name_hash).call()
 
     def get_node_status(self, node_id):
         try:
             return self.contract.functions.getNodeStatus(node_id).call()
-        except (ValueError, BadFunctionCallOutput):
+        except (ContractLogicError, ValueError, BadFunctionCallOutput):
             raise InvalidNodeIdError(node_id)
 
     def get_node_finish_time(self, node_id):
         try:
             return self.contract.functions.getNodeFinishTime(node_id).call()
-        except (ValueError, BadFunctionCallOutput):
+        except (ContractLogicError, ValueError, BadFunctionCallOutput):
             raise InvalidNodeIdError(node_id)
 
     def __get_node_public_key_raw(self, node_id):
         try:
             return self.contract.functions.getNodePublicKey(node_id).call()
-        except (ValueError, BadFunctionCallOutput):
+        except (ContractLogicError, ValueError, BadFunctionCallOutput):
             raise InvalidNodeIdError(node_id)
 
     def get_node_public_key(self, node_id):
         raw_key = self.__get_node_public_key_raw(node_id)
         key_bytes = raw_key[0] + raw_key[1]
-        return self.skale.web3.toHex(key_bytes)
+        return self.skale.web3.to_hex(key_bytes)
 
     def get_validator_node_indices(self, validator_id: int) -> list:
         """Returns list of node indices to the validator
 
         :returns: List of trusted node indices
         :rtype: list
         """
```

### Comparing `skale.py-5.8b2/skale/contracts/manager/punisher.py` & `skale.py-6.0.dev0/skale/contracts/manager/punisher.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/schains.py` & `skale.py-6.0.dev0/skale/contracts/manager/schains.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/schains_internal.py` & `skale.py-6.0.dev0/skale/contracts/manager/schains_internal.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/sync_manager.py` & `skale.py-6.0.dev0/skale/contracts/manager/sync_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/test/time_helpers_with_debug.py` & `skale.py-6.0.dev0/skale/contracts/manager/test/time_helpers_with_debug.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/token.py` & `skale.py-6.0.dev0/skale/contracts/manager/token.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/contracts/manager/wallets.py` & `skale.py-6.0.dev0/skale/contracts/manager/wallets.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/dataclasses/__init__.py` & `skale.py-6.0.dev0/skale/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/dataclasses/delegation_status.py` & `skale.py-6.0.dev0/skale/dataclasses/delegation_status.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/dataclasses/node_info.py` & `skale.py-6.0.dev0/skale/dataclasses/node_info.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/dataclasses/schain_options.py` & `skale.py-6.0.dev0/skale/dataclasses/schain_options.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/dataclasses/skaled_ports.py` & `skale.py-6.0.dev0/skale/dataclasses/skaled_ports.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,8 +27,7 @@
     HTTP_JSON = 3
     BINARY_CONSENSUS = 4
     ZMQ_BROADCAST = 5
     IMA_MONITORING = 6
     WSS_JSON = 7
     HTTPS_JSON = 8
     INFO_HTTP_JSON = 9
-    IMA_RPC = 10
```

### Comparing `skale.py-5.8b2/skale/schain_config/__init__.py` & `skale.py-6.0.dev0/skale/schain_config/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/schain_config/generator.py` & `skale.py-6.0.dev0/skale/schain_config/generator.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/schain_config/ports_allocation.py` & `skale.py-6.0.dev0/skale/schain_config/ports_allocation.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/schain_config/rotation_history.py` & `skale.py-6.0.dev0/skale/schain_config/rotation_history.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/skale_allocator.py` & `skale.py-6.0.dev0/skale/skale_allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/skale_base.py` & `skale.py-6.0.dev0/skale/skale_base.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/skale_ima.py` & `skale.py-6.0.dev0/skale/skale_ima.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/skale_manager.py` & `skale.py-6.0.dev0/skale/skale_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/transactions/result.py` & `skale.py-6.0.dev0/skale/transactions/result.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/transactions/tools.py` & `skale.py-6.0.dev0/skale/transactions/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 def estimate_gas(web3, method, opts):
     try:
         block_gas_limit = get_block_gas_limit(web3)
     except AttributeError:
         block_gas_limit = get_block_gas_limit(web3)
 
-    estimated_gas = method.estimateGas(
+    estimated_gas = method.estimate_gas(
         opts,
         block_identifier='latest'
     )
     normalized_estimated_gas = int(
         estimated_gas * config.DEFAULT_GAS_MULTIPLIER
     )
     if normalized_estimated_gas > block_gas_limit:
@@ -83,15 +83,15 @@
 block gas limit, going to use block_gas_limit ({block_gas_limit}) for this transaction')
         return block_gas_limit
     return normalized_estimated_gas
 
 
 def build_tx_dict(method, *args, **kwargs):
     base_fields = compose_base_fields(*args, **kwargs)
-    return method.buildTransaction(base_fields)
+    return method.build_transaction(base_fields)
 
 
 def compose_base_fields(
     nonce: int,
     gas_limit: int,
     gas_price: Optional[int] = None,
     max_fee_per_gas: Optional[int] = None,
```

### Comparing `skale.py-5.8b2/skale/utils/abi_utils.py` & `skale.py-6.0.dev0/skale/utils/abi_utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/account_tools.py` & `skale.py-6.0.dev0/skale/utils/account_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     **kwargs
 ):
     logger.info(
         f'Sending {amount} SKALE tokens from {skale.wallet.address} => '
         f'{receiver_address}'
     )
 
-    wei_amount = skale.web3.toWei(amount, 'ether')
+    wei_amount = skale.web3.to_wei(amount, 'ether')
     return skale.token.transfer(
         receiver_address,
         wei_amount,
         *args,
         **kwargs
     )
 
@@ -79,15 +79,15 @@
     priority: Optional[int] = None,
     **kwargs
 ):
     logger.info(
         f'Sending {amount} ETH from {wallet.address} => '
         f'{receiver_address}'
     )
-    wei_amount = web3.toWei(amount, 'ether')
+    wei_amount = web3.to_wei(amount, 'ether')
     gas_price = gas_price or default_gas_price(web3)
     tx = compose_eth_transfer_tx(
         web3=web3,
         *args,
         gas_price=gas_price,
         from_address=wallet.address,
         to_address=receiver_address,
@@ -107,28 +107,28 @@
             confirmation_blocks
         )
     check_receipt(receipt)
     return receipt
 
 
 def account_eth_balance_wei(web3, address):
-    return web3.eth.getBalance(address)
+    return web3.eth.get_balance(address)
 
 
 def check_ether_balance(web3, address):
     balance_wei = account_eth_balance_wei(web3, address)
-    balance = web3.fromWei(balance_wei, 'ether')
+    balance = web3.from_wei(balance_wei, 'ether')
 
     logger.info(f'{address} balance: {balance} ETH')
     return balance
 
 
 def check_skale_balance(skale, address):
     balance_wei = skale.token.get_balance(address)
-    balance = skale.web3.fromWei(balance_wei, 'ether')
+    balance = skale.web3.from_wei(balance_wei, 'ether')
     logger.info(f'{address} balance: {balance} SKALE')
     return balance
 
 
 def generate_account(web3):
     account = web3.eth.account.create()
     private_key = account.key.hex()
```

### Comparing `skale.py-5.8b2/skale/utils/constants.py` & `skale.py-6.0.dev0/skale/utils/constants.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/contract_info.py` & `skale.py-6.0.dev0/skale/utils/contract_info.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/contract_types.py` & `skale.py-6.0.dev0/skale/utils/contract_types.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/contracts_provision/__init__.py` & `skale.py-6.0.dev0/skale/utils/contracts_provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/contracts_provision/allocator.py` & `skale.py-6.0.dev0/skale/utils/contracts_provision/allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/contracts_provision/fake_multisig_contract.py` & `skale.py-6.0.dev0/skale/utils/contracts_provision/fake_multisig_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     print('Going to deploy simple payable contract')
     FakeMultisigContract = web3.eth.contract(abi=FAKE_MULTISIG_ABI, bytecode=FAKE_MULTISIG_BYTECODE)
     constructor = FakeMultisigContract.constructor()
     constructor.fn_name = 'fake_multisig_constructor'
     tx = transaction_from_method(
         constructor,
         nonce=get_eth_nonce(web3, wallet.address),
+        gas_price=3 * 10 ** 9,
         gas_limit=FAKE_MULTISIG_CONSTRUCTOR_GAS
     )
     tx_hash = wallet.sign_and_send(tx)
     receipt = wait_for_receipt_by_blocks(web3, tx_hash)
     print(f'Sample contract successfully deployed: {receipt.contractAddress}')
     content = {
         'address': receipt.contractAddress,
```

### Comparing `skale.py-5.8b2/skale/utils/contracts_provision/main.py` & `skale.py-6.0.dev0/skale/utils/contracts_provision/main.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/contracts_provision/utils.py` & `skale.py-6.0.dev0/skale/utils/contracts_provision/utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/exceptions.py` & `skale.py-6.0.dev0/skale/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/helper.py` & `skale.py-6.0.dev0/skale/utils/helper.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/random_names/generator.py` & `skale.py-6.0.dev0/skale/utils/random_names/generator.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/random_names/vocabulary.py` & `skale.py-6.0.dev0/skale/utils/random_names/vocabulary.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/utils/web3_utils.py` & `skale.py-6.0.dev0/skale/utils/web3_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         saved_number: {saved_number}, state_path: {state_path}'
 
 
 def make_client_checking_middleware(allowed_ts_diff: int,
                                     state_path: str = None):
     def eth_client_checking_middleware(make_request, web3):
         def middleware(method, params):
-            if method in ('eth_blockNumber', 'eth_getBlockByNumber'):
+            if method in ('eth_block_number', 'eth_getBlockByNumber'):
                 response = make_request(method, params)
             else:
                 latest_block = web3.eth.get_block('latest')
                 current_time = time.time()
 
                 ts_diff = current_time - latest_block['timestamp']
                 if not is_test_env():
@@ -174,26 +174,26 @@
     web3,
     tx,
     blocks_to_wait=DEFAULT_BLOCKS_TO_WAIT,
     timeout=MAX_WAITING_TIME
 ):
     blocks_to_wait = blocks_to_wait or DEFAULT_BLOCKS_TO_WAIT
     timeout = timeout or MAX_WAITING_TIME
-    previous_block = web3.eth.blockNumber
+    previous_block = web3.eth.block_number
     current_block = previous_block
     wait_start_time = time.time()
     while time.time() - wait_start_time < timeout and \
             current_block <= previous_block + blocks_to_wait:
         try:
             receipt = get_receipt(web3, tx)
         except TransactionNotFound:
             receipt = None
         if receipt is not None:
             return receipt
-        current_block = web3.eth.blockNumber
+        current_block = web3.eth.block_number
         time.sleep(3)
     raise TransactionNotMinedError(
         f'Transaction with hash: {tx} not found in {blocks_to_wait} blocks.'
     )
 
 
 def wait_receipt(web3, tx, retries=30, timeout=5):
@@ -223,44 +223,44 @@
 
 def wait_for_confirmation_blocks(
     web3,
     blocks_to_wait,
     timeout=MAX_WAITING_TIME,
     request_timeout=5
 ):
-    current_block = start_block = web3.eth.blockNumber
+    current_block = start_block = web3.eth.block_number
     logger.info(
         f'Current block number is {current_block}, '
         f'waiting for {blocks_to_wait} confimration blocks to be mined'
     )
     wait_start_time = time.time()
     while time.time() - wait_start_time < timeout and \
             current_block <= start_block + blocks_to_wait:
-        current_block = web3.eth.blockNumber
+        current_block = web3.eth.block_number
         time.sleep(request_timeout)
 
 
 def private_key_to_public(pr):
-    pr_bytes = Web3.toBytes(hexstr=pr)
+    pr_bytes = Web3.to_bytes(hexstr=pr)
     pk = keys.PrivateKey(pr_bytes)
     return pk.public_key
 
 
 def public_key_to_address(pk):
     hash = Web3.keccak(hexstr=str(pk))
-    return Web3.toHex(hash[-20:])
+    return Web3.to_hex(hash[-20:])
 
 
 def private_key_to_address(pr):
     pk = private_key_to_public(pr)
     return public_key_to_address(pk)
 
 
 def to_checksum_address(address):
-    return Web3.toChecksumAddress(address)
+    return Web3.to_checksum_address(address)
 
 
 def wallet_to_public_key(wallet):
     if isinstance(wallet, dict):
         return private_key_to_public(wallet['private_key'])
     else:
         return wallet['public_key']
```

### Comparing `skale.py-5.8b2/skale/wallets/common.py` & `skale.py-6.0.dev0/skale/wallets/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Dict, Optional
 
 from skale.utils.exceptions import ChainIdError
 
 
 def ensure_chain_id(tx_dict, web3):
     if not tx_dict.get('chainId'):
-        tx_dict['chainId'] = web3.eth.chainId
+        tx_dict['chainId'] = web3.eth.chain_id
     if not tx_dict.get('chainId'):
         raise ChainIdError('chainId must be in tx_dict (see EIP-155)')
 
 
 class BaseWallet(ABC):
     @abstractmethod
     def sign(self, tx):
```

### Comparing `skale.py-5.8b2/skale/wallets/ledger_wallet.py` & `skale.py-6.0.dev0/skale/wallets/ledger_wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,30 +156,30 @@
         return exchange_result
 
     def sign(self, tx_dict):
         ensure_chain_id(tx_dict, self._web3)
         if config.ENV == 'dev':  # fix for big chainId in ganache
             tx_dict['chainId'] = None
         if tx_dict.get('nonce') is None:
-            tx_dict['nonce'] = self._web3.eth.getTransactionCount(self.address)
+            tx_dict['nonce'] = self._web3.eth.get_transaction_count(self.address)
         tx = tx_from_dict(tx_dict)
         payload = self.make_payload(tx)
         exchange_result = self.exchange_sign_payload_by_chunks(payload)
         return LedgerWallet.parse_sign_result(tx, exchange_result)
 
     def sign_and_send(
         self,
         tx: Dict,
         multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
         priority: int = config.DEFAULT_PRIORITY,
         method: Optional[str] = None,
         meta: Optional[Dict] = None
     ) -> str:
         signed_tx = self.sign(tx)
-        return self._web3.eth.sendRawTransaction(
+        return self._web3.eth.send_raw_transaction(
             signed_tx.rawTransaction
         ).hex()
 
     def sign_hash(self, unsigned_hash: str):
         raise NotImplementedError(
             'sign_hash is not implemented for hardware wallet'
         )
@@ -216,17 +216,17 @@
             timeout=timeout
         )
 
 
 def hardware_sign_and_send(web3, method, gas_amount, wallet) -> str:
     address_from = wallet['address']
     eth_nonce = get_eth_nonce(web3, address_from)
-    tx_dict = method.buildTransaction({
+    tx_dict = method.build_transaction({
         'gas': gas_amount,
         'nonce': eth_nonce
     })
     signed_txn = wallet.sign(tx_dict)
-    tx = web3.eth.sendRawTransaction(signed_txn.rawTransaction).hex()
+    tx = web3.eth.send_raw_transaction(signed_txn.rawTransaction).hex()
     logger.info(
-        f'{method.__class__.__name__} - transaction_hash: {web3.toHex(tx)}'
+        f'{method.__class__.__name__} - transaction_hash: {web3.to_hex(tx)}'
     )
     return tx
```

### Comparing `skale.py-5.8b2/skale/wallets/redis_wallet.py` & `skale.py-6.0.dev0/skale/wallets/redis_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/wallets/rpc_wallet.py` & `skale.py-6.0.dev0/skale/wallets/rpc_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/skale/wallets/sgx_wallet.py` & `skale.py-6.0.dev0/skale/wallets/sgx_wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         tx_dict: Dict,
         multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
         priority: int = config.DEFAULT_PRIORITY,
         method: Optional[str] = None,
         meta: Optional[Dict] = None
     ) -> str:
         signed_tx = self.sign(tx_dict)
-        return self._web3.eth.sendRawTransaction(
+        return self._web3.eth.send_raw_transaction(
             signed_tx.rawTransaction
         ).hex()
 
     def sign_hash(self, unsigned_hash: str):
         if unsigned_hash.startswith('0x'):
             unsigned_hash = unsigned_hash[2:]
```

### Comparing `skale.py-5.8b2/skale/wallets/web3_wallet.py` & `skale.py-6.0.dev0/skale/wallets/web3_wallet.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 
 import skale.config as config
 from skale.utils.web3_utils import get_eth_nonce, wait_for_receipt_by_blocks
 from skale.wallets.common import BaseWallet, ensure_chain_id
 
 
 def private_key_to_public(pr):
-    pr_bytes = Web3.toBytes(hexstr=pr)
+    pr_bytes = Web3.to_bytes(hexstr=pr)
     pk = keys.PrivateKey(pr_bytes)
     return pk.public_key
 
 
 def public_key_to_address(pk):
     hash = Web3.keccak(hexstr=str(pk))
-    return to_checksum_address(Web3.toHex(hash[-20:]))
+    return to_checksum_address(Web3.to_hex(hash[-20:]))
 
 
 def private_key_to_address(pr):
     pk = private_key_to_public(pr)
     return public_key_to_address(pk)
 
 
 def to_checksum_address(address):
-    return Web3.toChecksumAddress(address)
+    return Web3.to_checksum_address(address)
 
 
 def generate_wallet(web3):
     account = web3.eth.account.create()
     private_key = account.key.hex()
     return Web3Wallet(private_key, web3)
 
@@ -82,15 +82,15 @@
         tx_dict: Dict,
         multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
         priority: int = config.DEFAULT_PRIORITY,
         method: Optional[str] = None,
         meta: Optional[Dict] = None
     ) -> str:
         signed_tx = self.sign(tx_dict)
-        return self._web3.eth.sendRawTransaction(
+        return self._web3.eth.send_raw_transaction(
             signed_tx.rawTransaction
         ).hex()
 
     @property
     def address(self):
         return self._address
```

### Comparing `skale.py-5.8b2/skale.py.egg-info/PKG-INFO` & `skale.py-6.0.dev0/skale.py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 5.8b2
+Version: 6.0.dev0
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: skale
```

### Comparing `skale.py-5.8b2/skale.py.egg-info/SOURCES.txt` & `skale.py-6.0.dev0/skale.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/tests/schain_config/generator_test.py` & `skale.py-6.0.dev0/tests/schain_config/generator_test.py`

 * *Files identical despite different names*

### Comparing `skale.py-5.8b2/tests/schain_config/ports_allocation_test.py` & `skale.py-6.0.dev0/tests/schain_config/ports_allocation_test.py`

 * *Files identical despite different names*

