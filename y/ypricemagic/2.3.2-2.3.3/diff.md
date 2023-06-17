# Comparing `tmp/ypricemagic-2.3.2.tar.gz` & `tmp/ypricemagic-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.3.2.tar", last modified: Fri Jun 16 18:01:36 2023, max compression
+gzip compressed data, was "ypricemagic-2.3.3.tar", last modified: Sat Jun 17 04:10:24 2023, max compression
```

## Comparing `ypricemagic-2.3.2.tar` & `ypricemagic-2.3.3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.755845 ypricemagic-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.735845 ypricemagic-2.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-16 18:01:36.755845 ypricemagic-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-16 18:01:36.755845 ypricemagic-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.743845 ypricemagic-2.3.2/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9930 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20162 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.747845 ypricemagic-2.3.2/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11225 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    22301 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.751845 ypricemagic-2.3.2/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.755845 ypricemagic-2.3.2/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.755845 ypricemagic-2.3.2/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-16 18:01:25.000000 ypricemagic-2.3.2/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 18:01:36.755845 ypricemagic-2.3.2/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-16 18:01:36.000000 ypricemagic-2.3.2/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-16 18:01:36.000000 ypricemagic-2.3.2/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 18:01:36.000000 ypricemagic-2.3.2/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-16 18:01:36.000000 ypricemagic-2.3.2/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-16 18:01:36.000000 ypricemagic-2.3.2/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.906909 ypricemagic-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.890908 ypricemagic-2.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.894908 ypricemagic-2.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-17 04:10:24.906909 ypricemagic-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-17 04:10:24.906909 ypricemagic-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.894908 ypricemagic-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.894908 ypricemagic-2.3.3/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.894908 ypricemagic-2.3.3/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.894908 ypricemagic-2.3.3/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20162 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.898908 ypricemagic-2.3.3/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19869 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22301 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.902908 ypricemagic-2.3.3/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.906909 ypricemagic-2.3.3/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.906909 ypricemagic-2.3.3/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-17 04:10:09.000000 ypricemagic-2.3.3/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 04:10:24.906909 ypricemagic-2.3.3/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-17 04:10:24.000000 ypricemagic-2.3.3/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-17 04:10:24.000000 ypricemagic-2.3.3/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-17 04:10:24.000000 ypricemagic-2.3.3/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-17 04:10:24.000000 ypricemagic-2.3.3/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-17 04:10:24.000000 ypricemagic-2.3.3/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.3.2/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.3.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/.github/workflows/pytest.yaml` & `ypricemagic-2.3.3/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/.github/workflows/release.yaml` & `ypricemagic-2.3.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/LICENSE.txt` & `ypricemagic-2.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/README.md` & `ypricemagic-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/setup.py` & `ypricemagic-2.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/classes/test_erc20.py` & `ypricemagic-2.3.3/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/classes/test_singleton.py` & `ypricemagic-2.3.3/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/fixtures.py` & `ypricemagic-2.3.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.3.3/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/lending/test_aave.py` & `ypricemagic-2.3.3/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/lending/test_compound.py` & `ypricemagic-2.3.3/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/test_chainlink.py` & `ypricemagic-2.3.3/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/test_magic.py` & `ypricemagic-2.3.3/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/test_popsicle.py` & `ypricemagic-2.3.3/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/test_synthetix.py` & `ypricemagic-2.3.3/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/test_yearn.py` & `ypricemagic-2.3.3/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/tests/prices/utils/test_buckets.py` & `ypricemagic-2.3.3/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/__init__.py` & `ypricemagic-2.3.3/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/classes/common.py` & `ypricemagic-2.3.3/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/classes/singleton.py` & `ypricemagic-2.3.3/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/constants.py` & `ypricemagic-2.3.3/y/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,16 @@
     Network.Avalanche:          "0xB31f66AA3C1e785363F0875A1B74E27b85FD66c7",
     Network.Heco:               "0x5545153CCFcA01fbd7Dd11C0b23ba694D9509A6F",
     Network.Harmony:            "0xcF664087a5bB0237a0BAd6742852ec6c8d69A27a",
     Network.Cronos:             "0x5C7F8A570d578ED84E63fdFA7b1eE72dEae1AE23",
     Network.Optimism:           "0x4200000000000000000000000000000000000006",
 }.get(chain.id)
 
+RAM_CACHE_TTL = int(os.environ.get("YPRICEMAGIC_CACHE_TTL", 60*60*24))  # 24h default
+
 thread_pool_executor = PruningThreadPoolExecutor(max_workers = int(os.environ.get("DOP", 128)))
 
 RECURSION_TIMEOUT = int(os.environ.get("YPRICEMAGIC_RECURSION_TIMEOUT", 60))
 recursion_logger_level = os.environ.get("YPRICEMAGIC_RECURSION_LOGGER_LEVEL", "debug").lower()
 log_possible_recursion_err = getattr(logging.getLogger("ypricemagic.recursion_logger"), recursion_logger_level)
 
 SKIP_YPRICEAPI = bool(os.environ.get("SKIP_YPRICEAPI"))
```

### Comparing `ypricemagic-2.3.2/y/contracts.py` & `ypricemagic-2.3.3/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/datatypes.py` & `ypricemagic-2.3.3/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/decorators.py` & `ypricemagic-2.3.3/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/erc20.py` & `ypricemagic-2.3.3/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/exceptions.py` & `ypricemagic-2.3.3/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/ERC20.py` & `ypricemagic-2.3.3/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.3.3/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/compound/unitroller.py` & `ypricemagic-2.3.3/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.3.3/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/multicall2.py` & `ypricemagic-2.3.3/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.3.3/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.3.3/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/networks.py` & `ypricemagic-2.3.3/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/band.py` & `ypricemagic-2.3.3/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/chainlink.py` & `ypricemagic-2.3.3/y/prices/chainlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         return convert.to_address(asset) in await self.__feeds__(sync=False)
 
     async def get_price(self, asset, block: Optional[Block] = None) -> UsdPrice:
         if block is None:
             block = chain.height
         return await self._get_price(asset, block)
 
-    alru_cache(maxsize=1000)
+    alru_cache(maxsize=1000, ttl=60*60*24)  # 24h ttl
     async def _get_price(self, asset, block: Block) -> Optional[UsdPrice]:
         asset = convert.to_address(asset)
         if asset == ZERO_ADDRESS:
             return None
         feed = await self.get_feed(asset, sync=False)
         if feed is None or (block is not None and block < await contract_creation_block_async(feed.address, True)):
             return None
```

### Comparing `ypricemagic-2.3.2/y/prices/convex.py` & `ypricemagic-2.3.3/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.3.3/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/balancer/v1.py` & `ypricemagic-2.3.3/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/balancer/v2.py` & `ypricemagic-2.3.3/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/genericamm.py` & `ypricemagic-2.3.3/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/mooniswap.py` & `ypricemagic-2.3.3/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.3.3/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.3.3/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.3.3/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.3.3/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.3.3/y/prices/dex/uniswap/v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         types = [type for _, type in zip(path, cycle(['address', 'uint24']))]
         return encode_abi_packed(types, path)
 
     def _undo_fees(self, path) -> float:
         fees = [1 - fee / FEE_DENOMINATOR for fee in path if isinstance(fee, int)]
         return math.prod(fees)
     
-    @a_sync.a_sync(cache_type='memory')
+    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
     async def get_price(self, token: Address, block: Optional[Block] = None) -> Optional[UsdPrice]:
         if block and block < await contract_creation_block_async(UNISWAP_V3_QUOTER, True):
             return None
 
         paths = [[token, fee, usdc.address] for fee in self.fee_tiers]
         if token != weth:
             paths += [
```

### Comparing `ypricemagic-2.3.2/y/prices/eth_derivs/creth.py` & `ypricemagic-2.3.3/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.3.3/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/gearbox.py` & `ypricemagic-2.3.3/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/lending/aave.py` & `ypricemagic-2.3.3/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/lending/compound.py` & `ypricemagic-2.3.3/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/lending/ib.py` & `ypricemagic-2.3.3/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/magic.py` & `ypricemagic-2.3.3/y/prices/magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         raise_if_exception_in(prices)
     else:
         for p in prices:
             if isinstance(p, Exception) and not isinstance(p, PriceError):
                 raise p
     return prices
 
-@a_sync.a_sync(cache_type='memory')
+@a_sync.a_sync(cache_type='memory', ram_cache_ttl=constants.RAM_CACHE_TTL)
 async def _get_price(
     token: AnyAddressType, 
     block: Block, 
     fail_to_None: bool = False, 
     silent: bool = False
     ) -> Optional[UsdPrice]:  # sourcery skip: remove-redundant-if
```

### Comparing `ypricemagic-2.3.2/y/prices/one_to_one.py` & `ypricemagic-2.3.3/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/popsicle.py` & `ypricemagic-2.3.3/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/stable_swap/belt.py` & `ypricemagic-2.3.3/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/stable_swap/curve.py` & `ypricemagic-2.3.3/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.3.3/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/stable_swap/froyo.py` & `ypricemagic-2.3.3/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.3.3/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/stable_swap/saddle.py` & `ypricemagic-2.3.3/y/prices/stable_swap/saddle.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 @a_sync.a_sync(default='sync', cache_type='memory')
 async def is_saddle_lp(token_address: AnyAddressType) -> bool:
     pool = await get_pool(token_address, sync=False)
     if pool:
         return await has_methods(pool, ('getVirtualPrice()(uint)', 'getA()(uint)','getAPrecise()(uint)'), sync=False)
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', ram_cache_ttl=60*60*24)  # 24h ttl
 async def get_pool(token_address: AnyAddressType) -> Address:
     convert.to_address(token_address)
     if chain.id == Network.Mainnet:
         if token_address == '0xc9da65931ABf0Ed1b74Ce5ad8c041C4220940368': # saddle aleth doesn't have swap() function
             return '0xa6018520EAACC06C30fF2e1B3ee2c7c22e64196a'
         elif token_address == '0xd48cF4D7FB0824CC8bAe055dF3092584d0a1726A': # saddle d4
             return '0xC69DDcd4DFeF25D8a793241834d4cc4b3668EAD6'
```

### Comparing `ypricemagic-2.3.2/y/prices/synthetix.py` & `ypricemagic-2.3.3/y/prices/synthetix.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         if await synthetix.get_currency_key(token, sync=False):
             return True
         if await has_method(token, 'target()(address)', sync=False):
             target = await Call(token, 'target()(address)').coroutine()
             return target in await synthetix.synths and await Call(target, 'proxy()(address)').coroutine() == token
         return False
     
-    @a_sync.a_sync(cache_type='memory')
+    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
     async def get_currency_key(self, token: AnyAddressType) -> Optional[HexString]:
         target = await Call(token, ['target()(address)']).coroutine() if await has_method(token, 'target()(address)', sync=False) else token
         return await Call(target, ['currencyKey()(bytes32)']).coroutine() if await has_method(token, 'currencyKey()(bytes32)', sync=False) else None
     
     async def get_price(self, token: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
         """
         Get a price of a synth in dollars.
```

### Comparing `ypricemagic-2.3.2/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.3.3/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.3.3/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.3.3/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.3.3/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/utils/buckets.py` & `ypricemagic-2.3.3/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/utils/sense_check.py` & `ypricemagic-2.3.3/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/utils/ypriceapi.py` & `ypricemagic-2.3.3/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/prices/yearn.py` & `ypricemagic-2.3.3/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/time.py` & `ypricemagic-2.3.3/y/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     client = get_ethereum_client()
     if client in ['tg', 'erigon']:
         header = web3.manager.request_blocking(f"{client}_getHeaderByNumber", [height])
         return int(header.timestamp, 16)
     else:
         return chain[height].timestamp
 
-@a_sync(cache_type='memory')
+@a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
 async def get_block_timestamp_async(height: int) -> int:
     client = await get_ethereum_client_async()
     if client in ['tg', 'erigon']:
         header = await dank_w3.manager.coro_request(f"{client}_getHeaderByNumber", [height])
         return int(header.timestamp, 16)
     else:
         block = await dank_w3.eth.get_block(height)
@@ -88,15 +88,15 @@
         except NoBlockFound:
             time.sleep(.2)
     check_node()
     block = _closest_block_after_timestamp_cached(timestamp)
     logger.debug(f'closest {Network.name()} block after timestamp {timestamp} -> {block}')
     return block
 
-@a_sync(cache_type='memory')
+@a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
 async def closest_block_after_timestamp_async(timestamp: Timestamp, wait_for_block_if_needed: bool = False) -> int:
     timestamp = _parse_timestamp(timestamp)
     while wait_for_block_if_needed:
         try:
             return await closest_block_after_timestamp_async(timestamp)
         except NoBlockFound:
             await asyncio.sleep(0.2)
@@ -140,8 +140,8 @@
 
 @alru_cache(ttl=60)
 async def check_node_async() -> None:
     latest = await dank_w3.eth.get_block('latest')
     node_timestamp = latest.timestamp
     current_time = time.time()
     if current_time - node_timestamp > 5 * 60:
-        raise NodeNotSynced(f"current time: {current_time}  latest block time: {node_timestamp}  discrepancy: {round((current_time - node_timestamp) / 60, 2)} minutes")
+        raise NodeNotSynced(f"current time: {current_time}  latest block time: {node_timestamp}  discrepancy: {round((current_time - node_timestamp) / 60, 2)} minutes")
```

### Comparing `ypricemagic-2.3.2/y/utils/client.py` & `ypricemagic-2.3.3/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/utils/events.py` & `ypricemagic-2.3.3/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/utils/fakes.py` & `ypricemagic-2.3.3/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/utils/logging.py` & `ypricemagic-2.3.3/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/utils/middleware.py` & `ypricemagic-2.3.3/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/utils/multicall.py` & `ypricemagic-2.3.3/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/y/utils/raw_calls.py` & `ypricemagic-2.3.3/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/ypricemagic/magic.py` & `ypricemagic-2.3.3/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.2/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.3.3/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

