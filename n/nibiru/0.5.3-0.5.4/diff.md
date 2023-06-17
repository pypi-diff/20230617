# Comparing `tmp/nibiru-0.5.3.tar.gz` & `tmp/nibiru-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibiru-0.5.3.tar", max compression
+gzip compressed data, was "nibiru-0.5.4.tar", max compression
```

## Comparing `nibiru-0.5.3.tar` & `nibiru-0.5.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     1068 2022-08-17 16:39:30.962967 nibiru-0.5.3/LICENSE
--rw-r--r--   0        0        0    12371 2022-11-14 13:19:46.688702 nibiru-0.5.3/README.md
--rw-r--r--   0        0        0      771 2022-10-12 16:20:34.476374 nibiru-0.5.3/nibiru/__init__.py
--rw-r--r--   0        0        0    10943 2022-11-09 14:43:26.898239 nibiru-0.5.3/nibiru/client.py
--rw-r--r--   0        0        0     3024 2022-08-19 17:44:11.896543 nibiru-0.5.3/nibiru/common.py
--rw-r--r--   0        0        0     2615 2022-10-10 19:20:10.728865 nibiru-0.5.3/nibiru/event_specs.py
--rw-r--r--   0        0        0      167 2022-08-23 20:38:16.358079 nibiru-0.5.3/nibiru/exceptions.py
--rw-r--r--   0        0        0      390 2022-08-19 17:44:11.897007 nibiru-0.5.3/nibiru/msg/__init__.py
--rw-r--r--   0        0        0     2628 2022-10-03 12:16:20.731294 nibiru-0.5.3/nibiru/msg/bank.py
--rw-r--r--   0        0        0     3337 2022-08-19 17:44:11.897471 nibiru-0.5.3/nibiru/msg/dex.py
--rw-r--r--   0        0        0     3908 2022-08-19 17:44:11.897736 nibiru-0.5.3/nibiru/msg/perp.py
--rw-r--r--   0        0        0      906 2022-08-19 17:44:11.897921 nibiru-0.5.3/nibiru/msg/pricefeed.py
--rw-r--r--   0        0        0     4267 2022-10-28 19:59:36.231312 nibiru-0.5.3/nibiru/network.py
--rw-r--r--   0        0        0      452 2022-10-03 12:16:20.731520 nibiru-0.5.3/nibiru/query_clients/__init__.py
--rw-r--r--   0        0        0     1111 2022-09-13 20:03:55.356892 nibiru-0.5.3/nibiru/query_clients/auth.py
--rw-r--r--   0        0        0    11700 2022-08-23 20:38:16.358399 nibiru-0.5.3/nibiru/query_clients/dex.py
--rw-r--r--   0        0        0     1289 2022-09-13 20:04:19.533702 nibiru-0.5.3/nibiru/query_clients/epoch.py
--rw-r--r--   0        0        0     3047 2022-11-14 13:19:36.268078 nibiru-0.5.3/nibiru/query_clients/perp.py
--rw-r--r--   0        0        0     1337 2022-08-23 20:38:16.358860 nibiru-0.5.3/nibiru/query_clients/pricefeed.py
--rw-r--r--   0        0        0     5074 2022-10-03 12:16:20.731703 nibiru-0.5.3/nibiru/query_clients/staking.py
--rw-r--r--   0        0        0     7552 2022-11-14 13:19:46.690708 nibiru-0.5.3/nibiru/query_clients/util.py
--rw-r--r--   0        0        0     1753 2022-10-10 19:20:10.728955 nibiru-0.5.3/nibiru/query_clients/vpool.py
--rw-r--r--   0        0        0     5204 2022-11-14 13:19:36.269185 nibiru-0.5.3/nibiru/sdk.py
--rw-r--r--   0        0        0     5659 2022-08-23 20:38:16.359772 nibiru-0.5.3/nibiru/transaction.py
--rw-r--r--   0        0        0     5836 2022-10-12 16:20:34.477572 nibiru-0.5.3/nibiru/tx.py
--rw-r--r--   0        0        0     8486 2022-10-12 16:20:34.478490 nibiru-0.5.3/nibiru/utils.py
--rw-r--r--   0        0        0    11263 2022-08-19 17:44:11.901224 nibiru-0.5.3/nibiru/wallet.py
--rw-r--r--   0        0        0     7018 2022-10-11 09:18:58.820587 nibiru-0.5.3/nibiru/websocket.py
--rw-r--r--   0        0        0     1488 2022-11-14 14:08:56.483225 nibiru-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    13878 2022-11-14 14:09:04.717413 nibiru-0.5.3/setup.py
--rw-r--r--   0        0        0    13949 2022-11-14 14:09:04.717949 nibiru-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-08-17 16:39:30.962967 nibiru-0.5.4/LICENSE
+-rw-r--r--   0        0        0    12371 2022-11-14 13:19:46.688702 nibiru-0.5.4/README.md
+-rw-r--r--   0        0        0      771 2022-10-12 16:20:34.476374 nibiru-0.5.4/nibiru/__init__.py
+-rw-r--r--   0        0        0    10943 2022-11-09 14:43:26.898239 nibiru-0.5.4/nibiru/client.py
+-rw-r--r--   0        0        0     3024 2022-08-19 17:44:11.896543 nibiru-0.5.4/nibiru/common.py
+-rw-r--r--   0        0        0        0 2022-11-28 13:19:10.232273 nibiru-0.5.4/nibiru/crypto/__init__.py
+-rw-r--r--   0        0        0    12881 2022-11-28 13:19:10.232784 nibiru-0.5.4/nibiru/crypto/ripemd160.py
+-rw-r--r--   0        0        0     2615 2022-10-10 19:20:10.728865 nibiru-0.5.4/nibiru/event_specs.py
+-rw-r--r--   0        0        0      167 2022-08-23 20:38:16.358079 nibiru-0.5.4/nibiru/exceptions.py
+-rw-r--r--   0        0        0      390 2022-08-19 17:44:11.897007 nibiru-0.5.4/nibiru/msg/__init__.py
+-rw-r--r--   0        0        0     2628 2022-10-03 12:16:20.731294 nibiru-0.5.4/nibiru/msg/bank.py
+-rw-r--r--   0        0        0     3337 2022-08-19 17:44:11.897471 nibiru-0.5.4/nibiru/msg/dex.py
+-rw-r--r--   0        0        0     3908 2022-08-19 17:44:11.897736 nibiru-0.5.4/nibiru/msg/perp.py
+-rw-r--r--   0        0        0      906 2022-08-19 17:44:11.897921 nibiru-0.5.4/nibiru/msg/pricefeed.py
+-rw-r--r--   0        0        0     4267 2022-10-28 19:59:36.231312 nibiru-0.5.4/nibiru/network.py
+-rw-r--r--   0        0        0      452 2022-10-03 12:16:20.731520 nibiru-0.5.4/nibiru/query_clients/__init__.py
+-rw-r--r--   0        0        0     1111 2022-09-13 20:03:55.356892 nibiru-0.5.4/nibiru/query_clients/auth.py
+-rw-r--r--   0        0        0    11700 2022-08-23 20:38:16.358399 nibiru-0.5.4/nibiru/query_clients/dex.py
+-rw-r--r--   0        0        0     1289 2022-09-13 20:04:19.533702 nibiru-0.5.4/nibiru/query_clients/epoch.py
+-rw-r--r--   0        0        0     3047 2022-11-14 13:19:36.268078 nibiru-0.5.4/nibiru/query_clients/perp.py
+-rw-r--r--   0        0        0     1337 2022-08-23 20:38:16.358860 nibiru-0.5.4/nibiru/query_clients/pricefeed.py
+-rw-r--r--   0        0        0     5074 2022-10-03 12:16:20.731703 nibiru-0.5.4/nibiru/query_clients/staking.py
+-rw-r--r--   0        0        0     7552 2022-11-14 13:19:46.690708 nibiru-0.5.4/nibiru/query_clients/util.py
+-rw-r--r--   0        0        0     1753 2022-10-10 19:20:10.728955 nibiru-0.5.4/nibiru/query_clients/vpool.py
+-rw-r--r--   0        0        0     5204 2022-11-14 13:19:36.269185 nibiru-0.5.4/nibiru/sdk.py
+-rw-r--r--   0        0        0     5659 2022-08-23 20:38:16.359772 nibiru-0.5.4/nibiru/transaction.py
+-rw-r--r--   0        0        0     5836 2022-10-12 16:20:34.477572 nibiru-0.5.4/nibiru/tx.py
+-rw-r--r--   0        0        0     8486 2022-10-12 16:20:34.478490 nibiru-0.5.4/nibiru/utils.py
+-rw-r--r--   0        0        0    11286 2022-11-28 13:19:10.233325 nibiru-0.5.4/nibiru/wallet.py
+-rw-r--r--   0        0        0     7018 2022-10-11 09:18:58.820587 nibiru-0.5.4/nibiru/websocket.py
+-rw-r--r--   0        0        0     1488 2022-11-28 13:24:51.941699 nibiru-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    13895 2022-11-28 13:24:55.329198 nibiru-0.5.4/setup.py
+-rw-r--r--   0        0        0    13949 2022-11-28 13:24:55.329743 nibiru-0.5.4/PKG-INFO
```

### Comparing `nibiru-0.5.3/LICENSE` & `nibiru-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/README.md` & `nibiru-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/__init__.py` & `nibiru-0.5.4/nibiru/__init__.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/client.py` & `nibiru-0.5.4/nibiru/client.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/common.py` & `nibiru-0.5.4/nibiru/common.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/event_specs.py` & `nibiru-0.5.4/nibiru/event_specs.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/msg/bank.py` & `nibiru-0.5.4/nibiru/msg/bank.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/msg/dex.py` & `nibiru-0.5.4/nibiru/msg/dex.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/msg/perp.py` & `nibiru-0.5.4/nibiru/msg/perp.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/msg/pricefeed.py` & `nibiru-0.5.4/nibiru/msg/pricefeed.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/network.py` & `nibiru-0.5.4/nibiru/network.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/auth.py` & `nibiru-0.5.4/nibiru/query_clients/auth.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/dex.py` & `nibiru-0.5.4/nibiru/query_clients/dex.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/epoch.py` & `nibiru-0.5.4/nibiru/query_clients/epoch.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/perp.py` & `nibiru-0.5.4/nibiru/query_clients/perp.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/pricefeed.py` & `nibiru-0.5.4/nibiru/query_clients/pricefeed.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/staking.py` & `nibiru-0.5.4/nibiru/query_clients/staking.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/util.py` & `nibiru-0.5.4/nibiru/query_clients/util.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/query_clients/vpool.py` & `nibiru-0.5.4/nibiru/query_clients/vpool.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/sdk.py` & `nibiru-0.5.4/nibiru/sdk.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/transaction.py` & `nibiru-0.5.4/nibiru/transaction.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/tx.py` & `nibiru-0.5.4/nibiru/tx.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/utils.py` & `nibiru-0.5.4/nibiru/utils.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/nibiru/wallet.py` & `nibiru-0.5.4/nibiru/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from bech32 import bech32_decode, bech32_encode, convertbits
 from bip32 import BIP32
 from ecdsa import BadSignatureError, SECP256k1, SigningKey, VerifyingKey
 from ecdsa.util import sigencode_string_canonize
 from mnemonic import Mnemonic
 from nibiru_proto.proto.cosmos.crypto.secp256k1.keys_pb2 import PubKey as PubKeyProto
 
+from nibiru.crypto.ripemd160 import ripemd160
+
 BECH32_PUBKEY_ACC_PREFIX = "nibipub"
 BECH32_PUBKEY_VAL_PREFIX = "nibivaloperpub"
 BECH32_PUBKEY_CONS_PREFIX = "nibivalconspub"
 
 BECH32_ADDR_ACC_PREFIX = "nibi"
 BECH32_ADDR_VAL_PREFIX = "nibivaloper"
 BECH32_ADDR_CONS_PREFIX = "nibivalcons"
@@ -179,15 +181,15 @@
         # k = sha3.keccak_256()
         # k.update(pubkey[1:])
         # addr = k.digest()[12:]
         # return Address(addr)
 
         pubkey = self.verify_key.to_string("compressed")
         s = hashlib.new("sha256", pubkey).digest()
-        r = hashlib.new("ripemd160", s).digest()
+        r = ripemd160(s)
         return Address(r)
 
     def verify(self, msg: bytes, sig: bytes) -> bool:
         """
         Verify a signature made from the given message.
 
         :param msg: data signed by the `signature`, will be hashed using sha256 function
```

### Comparing `nibiru-0.5.3/nibiru/websocket.py` & `nibiru-0.5.4/nibiru/websocket.py`

 * *Files identical despite different names*

### Comparing `nibiru-0.5.3/pyproject.toml` & `nibiru-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nibiru"
-version = "0.5.3"
+version = "0.5.4"
 description = "Python SDK for interacting with Nibiru."
 authors = ["Nibiru Chain <dev@nibiru.fi>"]
 license = "MIT"
 maintainers = [
   "NibiruHeisenberg <dev@nibiru.fi>",
   "matthiasmat <dev@nibiru.fi>",
   "onikonychev <dev@nibiru.fi>",
```

### Comparing `nibiru-0.5.3/setup.py` & `nibiru-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['nibiru', 'nibiru.msg', 'nibiru.query_clients']
+['nibiru', 'nibiru.crypto', 'nibiru.msg', 'nibiru.query_clients']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiocron>=1.8,<2.0',
  'aiohttp>=3.8.3,<4.0.0',
@@ -24,15 +24,15 @@
  'python-dotenv>=0.21.0,<0.22.0',
  'requests>=2.28.1,<3.0.0',
  'shutup>=0.2.0,<0.3.0',
  'websocket-client>=1.4.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'nibiru',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'Python SDK for interacting with Nibiru.',
     'long_description': '# Nibiru Python SDK - `nibiru`                           <!-- omit in toc -->\n\n> Python-based client for interacting with the Nibiru blockchain.\n\n<!-- Badges -->\n\n[![Nibiru Test workflow][tests-badge]][tests-workflow]\n[![PyPI Version][pypi-image]][pypi-url]\n[![][documentation-image]][documentation-url]\n[![][discord-badge]][discord-url]\n[![][stars-image]][stars-url]\n[![MIT license][license-badge]][license-link]\n\n<!-- Badges links -->\n\n<!-- pypi -->\n[pypi-image]: https://img.shields.io/pypi/v/nibiru\n[pypi-url]: https://pypi.org/project/nibiru/\n[stars-image]: https://img.shields.io/github/stars/NibiruChain?style=social\n[stars-url]: https://github.com/NibiruChain\n[documentation-image]: https://readthedocs.org/projects/nibiru-py/badge/?version=latest\n[documentation-url]: https://nibiru-py.readthedocs.io/en/latest/?badge=latest\n[discord-badge]: https://img.shields.io/badge/Nibiru%20Chain-%237289DA.svg?style=&logo=discord&logoColor=white\n[discord-url]: https://discord.gg/sgPw8ZYfpQ\n[license-badge]: https://img.shields.io/badge/License-MIT-blue.svg\n[license-link]: https://github.com/NibiruChain/py-sdk/blob/master/LICENSE\n[tests-badge]: https://github.com/NibiruChain/py-sdk/actions/workflows/pytests.yml/badge.svg\n[tests-workflow]: https://github.com/NibiruChain/py-sdk/actions/workflows/pytests.yml\n\nThe `nibiru` package allows you to index, query, and send transactions on the Nibiru Blockchain using Python. It provides access to market data for analysis, visualization, indicator development, algorithmic trading, strategy backtesting, bot programming, and related software engineering.\n\nThe package is intended to be used by coders, developers, technically-skilled traders and  data-scientists for building trading algorithms.\n\n## Python SDK Tutorial          <!-- omit in toc -->\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)][Colab link]\n\n[Colab link]: https://colab.research.google.com/github/NibiruChain/py-sdk/blob/master/examples/collab_notebook.ipynb\n\n#### README Contents\n\n- [User Guidelines](#user-guidelines)\n  - [Documentation Website](#documentation-website)\n  - [Installation from `PyPI`](#installation-from-pypi)\n- [Development Guidelines](#development-guidelines)\n  - [Setting up a professional dev environment with `pyenv` and `poetry`](#setting-up-a-professional-dev-environment-with-pyenv-and-poetry)\n    - [Pyenv for managing multiple Python interpreters](#pyenv-for-managing-multiple-python-interpreters)\n  - [Installing `poetry` for dependency resolution and publishing packages](#installing-poetry-for-dependency-resolution-and-publishing-packages)\n  - [Installing external dependencies](#installing-external-dependencies)\n  - [Running tests](#running-tests)\n  - [Makefile and Protocol Buffers](#makefile-and-protocol-buffers)\n  - [Linting](#linting)\n  - [Gotchas](#gotchas)\n  - [Usage instructions for publishing.](#usage-instructions-for-publishing)\n\n# User Guidelines\n\n## Documentation Website\n\nDocumentation can be found here: [Nibiru-py documentation](https://nibiru-py.readthedocs.io/en/latest/index.html)\n\n- Learn more about opening and managing your spot and perp positions [here](https://nibiru-py.readthedocs.io/en/latest/nibiru.sdks.tx.html#nibiru-sdks-tx-package)\n- Learn about querying the chain using the Sdk [here](https://nibiru-py.readthedocs.io/en/latest/nibiru.clients.html#nibiru-clients-package)\n\n## Installation from `PyPI`\n\n```sh\npip install nibiru  # requires Python 3.9\n```\n\nYou may need to update `pip` to get this to run:\n\n```sh\npython -m pip install --upgrade pip\n```\n\n---\n\n# Development Guidelines\n\nOur recommended setup is `pyenv` in combination with `poetry`.\n\n- `pyenv` is a tool for installing and managing Python interpreters. This will let you seamlessly switch between Python versions.\n- `poetry` is used for managing virtual environments, dependency resolution, package installations, package building, and package publishing.\n- We assume you\'re on a Unix machine such as WSL2 Ubuntu, MacOS, or a common Linux distro.\n\nCurrently, `nibiru` is created with Python 3.9.13. It may be compatible with higher versions, but we only run end-to-end tests in 3.9.13.\n\n## Setting up a professional dev environment with `pyenv` and `poetry`\n\n### Pyenv for managing multiple Python interpreters\n\nIf you\'re on MacOS or a common Linux distro, you can install `pyenv` with brew.\n\n```sh\nbrew install pyenv\n```\n\nYou\'ll then need to add the following snippet to your shell config, e.g. your `.bash_profile`, `.bashrc`, or `.zshrc`.\n\n```sh\nexport PYENV_ROOT="$HOME/.pyenv"\nexport PATH="$PYENV_ROOT/bin:$PATH"\neval "$(pyenv init -)"\neval "$(pyenv init --path)"\n```\n\nAfter using `source` on your config or restarting the shell, you should have the `pyenv` root command.\n\nThe command use to install any version of python is `pyenv install`. Display additional info for this command with `pyenv install --help`.\n\n```sh\npyenv install 3.9.13 # example for nibiru\n```\n\nOnce you have a version installed, you can print out the versions on your machine with:\n\n```sh\npyenv versions\n```\n\n```\n# example output\n  system\n* 3.9.13 (set by /home/realu/.python-version)\n  3.10.4\n```\n\nIn this example, I have 2 different interpreters installed on my machine. The one with the `*` is currently set as my **global interpreter**. This is set manually using the `pyenv global` command.\n\n```sh\npyenv global 3.10.4   # switches the global interpreter to 3.10.4\n```\n\nYou can verify this works as expected using `python --version`. You may be familiar with using `python3` as the command instead of `python`. With `pyenv`, this is not necessary.\n\nAdditional usage and installation instructions can be found in the [pyenv repo](https://github.com/pyenv/pyenv).\n\n## Installing `poetry` for dependency resolution and publishing packages\n\nReference: [Poetry docs](https://python-poetry.org/docs/)\n\nPoetry can be installed with both `curl` and `pip`. We recommended using `curl` so that it will be global to your machine.\n\nNOTE We highly, highly, highly recommend that you DO NOT use `brew` to install `poetry`.\nIf you use `brew`, it\'s going to install directly to your system, which prevents you from being able to leverage `pyenv` to seamlessly switch between Python interpreters.\n\n```bash\n# installation with pip: recommended option in tandem with pyenv\npip install poetry\n```\n\n```bash\n# For UNIX systems - installation with curl\ncurl -sSL https://install.python-poetry.org/ | python -\n```\n\nAfter this installation command, add the `poetry` binary to the path in your shell config (if it\'s not done automatically).\n\n```bash\nexport PATH=$PATH:$HOME/.poetry/bin\n```\n\n## Installing external dependencies\n\nThe `nibiru` project is defined by its `pyproject.toml`. At the root of the repo, simply call:\n\n```bash\npoetry install\n```\n\nThis will resolve dependencies between each of the project\'s packages and install them into a virtual environment.\n\n## Running tests\n\n#### Setting environment variables\n\nThere\'s currently a "devnet" running in GCP that the CI workflows use. You can find these secrets at [this notion page](https://www.notion.so/nibiru/Resources-and-Repo-Configs-b31aa8074a2b419d80b0c946ed5efab0) if you have access to it or contact one of the `CODEOWNERS` (@Unique-Divine, @matthiasmatt, @nibiruheisenberg).\nThis is useful so that you can run every part of the package code without needing to visit other repositories.\n\nYou\'ll need to set up a `.env` configuration file to set environment variables for the tests.\n\n#### Environment Variables - Local\n\n\n```bash\n# Example configuration for the Nibiry Python SDK\nHOST="..."\nVALIDATOR_MNEMONIC="..."\nORACLE_MNEMONIC="..."\nTENDERMINT_RPC_ENDPOINT="http://...:26657"\nLCD_ENDPOINT="http://...:1317"\nGRPC_ENDPOINT="...:9090"\nWEBSOCKET_ENDPOINT="ws://...:26657/websocket"\nCHAIN_ID="..."\nNETWORK_INSECURE=true\n```\n\n#### Environment variables in GitHub Actions\n\nThe variables used in the CI build can be found in the `env` section of the [`pytests.yml` workflow](.github/workflows/pytests.yml):\n\n```yaml\njobs:\n  tests:\n    env:\n      # https://www.notion.so/nibiru/Resources-and-Repo-Configs-b31aa8074a2b419d80b0c946ed5efab0\n      CHAIN_ID: ${{ secrets.CHAIN_ID }}\n      HOST: ${{ secrets.HOST }}\n      VALIDATOR_MNEMONIC: ${{ secrets.VALIDATOR_MNEMONIC }}\n      GRPC_PORT: ${{ secrets.GRPC_PORT }}\n      LCD_PORT: ${{ secrets.LCD_PORT }}\n```\n\nYou\'ll need an `.env` configuration like this.\n\n#### Running the tests with `poetry` + `pytest`\n\nAfter following the instructions for setting up `poetry`, you can run the tests with `poetry run pytest`:\n\n```bash\npoetry run pytest -p no:warnings # silences warnings\n```\n\n#### (option B). Install the `nibiru` package with `pip`\n\n  ```bash\n  # from local\n  # build and install\n  pip install .\n\n  # from local build\n  pip uninstall nibiru\n  pip install nibiru --no-index --find-links /path/to/nibiru/py-sdk/dist\n\n  # from pypi\n  pip uninstall nibiru\n  pip install nibiru\n  ```\n\n## Makefile and Protocol Buffers\n\nSee the [NibiruChain/sdk-proto-gen repository](https://github.com/NibiruChain/sdk-proto-gen).\n\nAfter cloning `sdk-proto-gen` and the proto files for `nibiru`, you only need to run `make proto-gen`:\n\n```bash\ngit clone git@github.com:NibiruChain/sdk-proto-gen.git\ngit clone git@github.com:NibiruChain/nibiru.git\n```\n\n```bash\ncd sdk-proto-gen\nmake proto-gen\n```\n\nIf you get a permissions error such as\n\n```\nrm: cannot remove \'proto/proto/epochs/query.proto\': Permission denied\n```\n\ncall `sudo chown -R [USER-NAME] proto` using the name of user directory.\nYou can find the value for `[USER-NAME]` quickly by running `whoami`. In other words, this should work:\n\n```sh\nsudo chown -R $(whoami) proto\n```\n\nYou\'re done generating types once you\'ve successfully called\n\n```sh\nmake proto-gen\npoetry build # equivalently, you can run `python -m build`\n```\n\n## Linting\n\nEnable git hook which will perform linting before each commit:\n\n```shell\npoetry run pre-commit install\n```\n\nThis will keep your code clean.\n\n## Gotchas\n\nThe `protobuf` package must be version 3.20.x or lower. Otherwise, the following error appears at runtime.\n\n```\nnibiru/clients/__init__.py:1: in <module>\n    from nibiru.clients.dex import Dex  # noqa\nnibiru/clients/dex.py:8: in <module>\n    from nibiru.proto.dex.v1 import query_pb2 as dex_type\nnibiru/proto/dex/v1/query_pb2.py:16: in <module>\n    from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2\n../../../anaconda3/envs/divine/lib/python3.9/site-packages/google/api/annotations_pb2.py:30: in <module>\n    from google.api import http_pb2 as google_dot_api_dot_http__pb2\n../../../anaconda3/envs/divine/lib/python3.9/site-packages/google/api/http_pb2.py:48: in <module>\n    _descriptor.FieldDescriptor(\n../../../anaconda3/envs/divine/lib/python3.9/site-packages/google/protobuf/descriptor.py:560: in __new__\n    _message.Message._CheckCalledFromGeneratedFile()\nE   TypeError: Descriptors cannot not be created directly.\nE   If this call came from a _pb2.py file, your generated code is out of date and must be regenerated with protoc >= 3.19.0.\nE   If you cannot immediately regenerate your protos, some other possible workarounds are:\nE    1. Downgrade the protobuf package to 3.20.x or lower.\nE    2. Set PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python (but this will use pure-Python parsing and will be much slower).\nE\nE   More information: https://developers.google.com/protocol-buffers/docs/news/2022-05-06#python-updates\n```\n\n## Usage instructions for publishing.\n\nYou specify updates to publish using the commit (or PR) title with `bump-[version-keyword]`.\nFor the `poetry version` command, ysing any bump rule with a valid semver string will change the version inside `pyproject.toml`. For example,\n\n```\npoetry version patch # moves from x.y.14 to x.y.15\npoetry version minor # moves from x.5.z to x.6.0\npoetry version major # moves from 3.y.z to 4.0.0\n```\nThe list of bump rules includes:\npatch, minor, major, prepatch, preminor, premajor, prerelease.\n\nSo the list of available keywords you an put in a PR includes\n- `bump-patch`:\n- `bump-patch`: 0.0.0 → 0.0.1\n- `bump-minor`: 0.0.* → 0.1.0\n- `bump-major`: 0.*.* → 1.0.0\n- `bump-prepatch`: 0.0.0 → 0.0.1-alpha0\n- `bump-prerelease`: equivalent to `bump-prepatch`\n- `bump-preminor`: 0.0.* → 0.1.0-alpha0\n- `bump-premajor`: 0.*.* → 1.0.0-alpha0\n\nThese guidelines are in the release.yml for future reference.\n',
     'author': 'Nibiru Chain',
     'author_email': 'dev@nibiru.fi',
     'maintainer': 'NibiruHeisenberg',
     'maintainer_email': 'dev@nibiru.fi',
     'url': 'https://github.com/NibiruChain/sdk-py',
```

### Comparing `nibiru-0.5.3/PKG-INFO` & `nibiru-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibiru
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python SDK for interacting with Nibiru.
 Home-page: https://github.com/NibiruChain/sdk-py
 License: MIT
 Keywords: nibiru,blockchain,sdk,python,cosmos
 Author: Nibiru Chain
 Author-email: dev@nibiru.fi
 Maintainer: NibiruHeisenberg
```

