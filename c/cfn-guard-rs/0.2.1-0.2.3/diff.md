# Comparing `tmp/cfn_guard_rs-0.2.1.tar.gz` & `tmp/cfn_guard_rs-0.2.3.tar.gz`

## Comparing `cfn_guard_rs-0.2.1.tar` & `cfn_guard_rs-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 cfn_guard_rs-0.2.1/Cargo.toml
--rw-r--r--   0     1001      121      691 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/.gitignore
--rw-r--r--   0     1001      121      155 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/CHANGELOG.md
--rw-r--r--   0     1001      121      413 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/README.md
--rw-r--r--   0     1001      121      280 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/mypy.ini
--rw-r--r--   0     1001      121      353 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/pyproject.toml
--rw-r--r--   0     1001      121       85 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/pytest.ini
--rw-r--r--   0     1001      121      307 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/cfn_guard_rs/__init__.py
--rw-r--r--   0     1001      121     1630 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/cfn_guard_rs/api.py
--rw-r--r--   0     1001      121      447 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/cfn_guard_rs/errors.py
--rw-r--r--   0     1001      121     2228 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/cfn_guard_rs/interface.py
--rw-r--r--   0     1001      121        0 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/cfn_guard_rs/py.typed
--rw-r--r--   0     1001      121       32 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/__init__.py
--rw-r--r--   0     1001      121       69 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/rules/invalid_format.guard
--rw-r--r--   0     1001      121      360 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/rules/invalid_missing_value.guard
--rw-r--r--   0     1001      121       71 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/rules/s3_bucket_name.guard
--rw-r--r--   0     1001      121     1124 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/rules/s3_bucket_public_access.guard
--rw-r--r--   0     1001      121       85 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/templates/s3_bucket_name_invalid.yaml
--rw-r--r--   0     1001      121       90 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/templates/s3_bucket_name_valid.yaml
--rw-r--r--   0     1001      121      241 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/templates/s3_bucket_public_access_invalid.yaml
--rw-r--r--   0     1001      121      240 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/fixtures/templates/s3_bucket_public_access_valid.yaml
--rw-r--r--   0     1001      121     5708 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/python/tests/test_cfn_guard_rs.py
--rw-r--r--   0     1001      121       19 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/requirements-dev.txt
--rw-r--r--   0     1001      121       43 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/requirements.txt
--rw-r--r--   0     1001      121     3621 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/src/errors.rs
--rw-r--r--   0     1001      121     2235 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/src/lib.rs
--rw-r--r--   0     1001      121      218 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/tox.ini
--rw-r--r--   0     1001      121    25522 2022-11-02 15:41:10.000000 cfn_guard_rs-0.2.1/Cargo.lock
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 cfn_guard_rs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 cfn_guard_rs-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123      691 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/.gitignore
+-rw-r--r--   0     1001      123      155 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/CHANGELOG.md
+-rw-r--r--   0     1001      123      413 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/README.md
+-rw-r--r--   0     1001      123      280 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/mypy.ini
+-rw-r--r--   0     1001      123      353 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123       85 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/pytest.ini
+-rw-r--r--   0     1001      123      307 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/cfn_guard_rs/__init__.py
+-rw-r--r--   0     1001      123     1689 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/cfn_guard_rs/api.py
+-rw-r--r--   0     1001      123      447 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/cfn_guard_rs/errors.py
+-rw-r--r--   0     1001      123     2228 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/cfn_guard_rs/interface.py
+-rw-r--r--   0     1001      123        0 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/cfn_guard_rs/py.typed
+-rw-r--r--   0     1001      123       32 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/__init__.py
+-rw-r--r--   0     1001      123       69 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/rules/invalid_format.guard
+-rw-r--r--   0     1001      123      360 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/rules/invalid_missing_value.guard
+-rw-r--r--   0     1001      123       71 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/rules/s3_bucket_name.guard
+-rw-r--r--   0     1001      123     1124 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/rules/s3_bucket_public_access.guard
+-rw-r--r--   0     1001      123       85 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/templates/s3_bucket_name_invalid.yaml
+-rw-r--r--   0     1001      123       90 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/templates/s3_bucket_name_valid.yaml
+-rw-r--r--   0     1001      123      241 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/templates/s3_bucket_public_access_invalid.yaml
+-rw-r--r--   0     1001      123      240 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/fixtures/templates/s3_bucket_public_access_valid.yaml
+-rw-r--r--   0     1001      123     5971 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/python/tests/test_cfn_guard_rs.py
+-rw-r--r--   0     1001      123       19 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/requirements-dev.txt
+-rw-r--r--   0     1001      123       43 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/requirements.txt
+-rw-r--r--   0     1001      123     3621 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/src/errors.rs
+-rw-r--r--   0     1001      123     2235 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123      215 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/tox.ini
+-rw-r--r--   0     1001      123    26051 2023-06-17 17:08:55.000000 cfn_guard_rs-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 cfn_guard_rs-0.2.3/PKG-INFO
```

### Comparing `cfn_guard_rs-0.2.1/.gitignore` & `cfn_guard_rs-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cfn_guard_rs-0.2.1/python/cfn_guard_rs/api.py` & `cfn_guard_rs-0.2.3/python/cfn_guard_rs/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
   Defines the api for cfn_guard_rs
 
   Supports running the non-verbose version of
   run_checks from CloudFormation Guard
 """
 import logging
 import json
-from .interface import DataOutput
+from cfn_guard_rs.interface import DataOutput
 
 # pylint: disable=no-name-in-module
-from .cfn_guard_rs import (
+from cfn_guard_rs.cfn_guard_rs import (
     CfnGuardParseError,
     CfnGuardMissingValue,
     run_checks_rs,
 )
 
 from . import errors
 
@@ -35,24 +35,24 @@
 
     Returns
     -------
     DataOuptut
         DataOutput representation of the result of running guard
     """
     try:
-        output = json.loads(run_checks_rs(json.dumps(data), rules, False))
-
+        raw_output = run_checks_rs(json.dumps(data), rules, False)
+        output = json.loads(raw_output)
         # remove the lib set items and replace with our defaults
         result = DataOutput(**output)
 
         return result
     except json.JSONDecodeError as err:
         LOG.debug(
             "JSON decoding error when processing return value [%s] got error: %s",
-            output,
+            raw_output,
             err,
         )
         raise err
     except CfnGuardMissingValue as err:
         raise errors.MissingValueError(str(err))
     except CfnGuardParseError as err:
         raise errors.ParseError(str(err))
```

### Comparing `cfn_guard_rs-0.2.1/python/cfn_guard_rs/interface.py` & `cfn_guard_rs-0.2.3/python/cfn_guard_rs/interface.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_rs-0.2.1/python/tests/fixtures/rules/s3_bucket_public_access.guard` & `cfn_guard_rs-0.2.3/python/tests/fixtures/rules/s3_bucket_public_access.guard`

 * *Files identical despite different names*

### Comparing `cfn_guard_rs-0.2.1/python/tests/test_cfn_guard_rs.py` & `cfn_guard_rs-0.2.3/python/tests/test_cfn_guard_rs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
     Test cfn_guard_rs
 """
 from unittest.mock import patch
+import json
 import yaml
 import pytest
 import cfn_guard_rs.errors
 from cfn_guard_rs import Comparison, run_checks, DataOutput, NameInfo
 
 
 @pytest.mark.parametrize(
@@ -136,14 +137,24 @@
     with pytest.raises(parent_error, match=message):
         run_checks(template_str, rules)
 
     with pytest.raises(cfn_guard_rs.errors.GuardError, match=message):
         run_checks(template_str, rules)
 
 
+@patch("cfn_guard_rs.api.run_checks_rs")
+def test_json_decode_error(mock_run_check_rs):
+    """Test JSON Decode errors"""
+
+    mock_run_check_rs.return_value = '{ "bad": }'
+
+    with pytest.raises(json.JSONDecodeError):
+        run_checks("{}", "")
+
+
 def test_run_unknown_errors():
     """Test unknown errors"""
 
     template_filename = "python/tests/fixtures/templates/s3_bucket_name_valid.yaml"
     rules_filename = "python/tests/fixtures/rules/s3_bucket_name.guard"
     with open(template_filename, encoding="utf8") as file:
         template_str = yaml.safe_load(file)
```

### Comparing `cfn_guard_rs-0.2.1/src/errors.rs` & `cfn_guard_rs-0.2.3/src/errors.rs`

 * *Files identical despite different names*

### Comparing `cfn_guard_rs-0.2.1/src/lib.rs` & `cfn_guard_rs-0.2.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cfn_guard_rs-0.2.1/Cargo.lock` & `cfn_guard_rs-0.2.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4f55bd91a0978cbfd91c457a164bab8b4001c833b7f323132c0a4e1922dd44e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "ansi_term"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "arrayvec"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
 
 [[package]]
 name = "atty"
@@ -71,20 +80,20 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cfn-guard"
-version = "2.1.0"
-source = "git+https://github.com/aws-cloudformation/cloudformation-guard?branch=main#5481fa7265eab3dfdbb932df3fee4936dd4a4497"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c30bced6fce7c1040b223362681668004589dfb95d2ceac40d404b18a63cdb7"
 dependencies = [
  "Inflector",
  "clap",
- "clap_complete",
  "colored 2.0.0",
  "enumflags2",
  "enumflags2_derive",
  "grep-matcher",
  "grep-regex",
  "grep-searcher",
  "heck",
@@ -103,49 +112,33 @@
  "unsafe-libyaml",
  "urlencoding",
  "walkdir",
 ]
 
 [[package]]
 name = "cfn_guard_rs"
-version = "0.2.1"
+version = "0.2.3"
 dependencies = [
  "cfn-guard",
  "pyo3",
 ]
 
 [[package]]
 name = "clap"
-version = "4.0.18"
+version = "2.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "335867764ed2de42325fafe6d18b8af74ba97ee0c590fa016f157535b42ab04b"
+checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
 dependencies = [
+ "ansi_term",
  "atty",
  "bitflags",
- "clap_lex",
  "strsim",
- "termcolor",
-]
-
-[[package]]
-name = "clap_complete"
-version = "4.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfe581a2035db4174cdbdc91265e1aba50f381577f0510d0ad36c7bc59cc84a3"
-dependencies = [
- "clap",
-]
-
-[[package]]
-name = "clap_lex"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d4198f73e42b4936b35b5bb248d81d2b595ecb170da0bac7655c54eedfa8da8"
-dependencies = [
- "os_str_bytes",
+ "textwrap",
+ "unicode-width",
+ "vec_map",
 ]
 
 [[package]]
 name = "colored"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4ffc801dacf156c5854b9df4f425a626539c3a6ef7893cc0c5084a23f0b6c59"
@@ -182,30 +175,30 @@
 checksum = "1cc3c5651fb62ab8aa3103998dade57efdd028544bd300516baa31840c252a83"
 dependencies = [
  "encoding_rs",
 ]
 
 [[package]]
 name = "enumflags2"
-version = "0.7.5"
+version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e75d4cd21b95383444831539909fbb14b9dc3fdceb2a6f5d36577329a1f55ccb"
+checksum = "c041f5090df68b32bcd905365fd51769c8b9d553fe87fde0b683534f10c01bd2"
 dependencies = [
  "enumflags2_derive",
 ]
 
 [[package]]
 name = "enumflags2_derive"
-version = "0.7.4"
+version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f58dc3c5e468259f19f2d46304a6b28f1c3d034442e14b322d2b850e36f6d5ae"
+checksum = "5e9a1f9f7d83e59740248a6e14ecf93929ade55027844dfcea78beafccc15745"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures"
 version = "0.3.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38390104763dc37a5145a53c29c63c1290b5d316d6086ec32c293f6736051bb0"
@@ -256,15 +249,15 @@
 name = "futures-macro"
 version = "0.3.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdfb8ce053d86b91919aad980c220b1fb8401a9394410e1c289ed7e66b61835d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.103",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39c15cf1a4aa79df40f1bb462fb39676d0ad9e366c2a33b590d7c66f4f81fcf9"
@@ -447,14 +440,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95af15f345b17af2efc8ead6080fb8bc376f8cec1b35277b935637595fe77498"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "nom"
 version = "5.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffb4262d26ed83a1c0a33a38fe2bb15797329c85770da05e6b828ddb782627af"
 dependencies = [
  "lexical-core",
  "memchr",
@@ -484,20 +486,14 @@
 [[package]]
 name = "once_cell"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3baf96e39c5359d2eb0dd6ccb42c62b91d9678aa68160d261b9e0ccbf9e9dea9"
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -526,85 +522,86 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.16.6"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0220c44442c9b239dd4357aa856ac468a4f5e1f0df19ddb89b2522952eb4c6ca"
+checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.16.6"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c819d397859445928609d0ec5afc2da5204e0d0f73d6bf9e153b04e83c9cdc2"
+checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.16.6"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca882703ab55f54702d7bfe1189b41b0af10272389f04cae38fe4cd56c65f75f"
+checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.16.6"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "568749402955ad7be7bad9a09b8593851cd36e549ac90bfd44079cea500f3f21"
+checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.103",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.16.6"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "611f64e82d98f447787e82b8e7b0ebc681e1eb78fc1252668b2c605ffb4e1eb8"
+checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.103",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -655,15 +652,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5015e68a0685a95ade3eee617ff7101ab6a3fc689203101ca16ebc16f2b89c66"
 dependencies = [
  "cfg-if",
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.103",
 ]
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
@@ -711,15 +708,15 @@
 name = "serde_derive"
 version = "1.0.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f1d362ca8fc9c3e3a7484440752472d68a6caa98f1ab81d99b5dfe517cec852"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.103",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ce777b7b150d76b9cf60d28b55f5847135a003f7d7350c6be7a773508ce7d45"
@@ -781,42 +778,53 @@
 name = "string-builder"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2bd10a070fb1f2796a288abec42695db4682a82b6f12ffacd60fb8d5ad3a4a12"
 
 [[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
 
 [[package]]
 name = "syn"
 version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a864042229133ada95abf3b54fdc62ef5ccabe9515b64717bcb9a1919e59445d"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
 
 [[package]]
-name = "termcolor"
-version = "1.1.3"
+name = "textwrap"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
- "winapi-util",
+ "unicode-width",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
@@ -862,14 +870,20 @@
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fdbf052a0783de01e944a6ce7a8cb939e295b1e7be835a1112c3b9a7f047a5a"
 
 [[package]]
+name = "unicode-width"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+
+[[package]]
 name = "unindent"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
 
 [[package]]
 name = "unsafe-libyaml"
@@ -880,14 +894,20 @@
 [[package]]
 name = "urlencoding"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
 
 [[package]]
+name = "vec_map"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
```

### Comparing `cfn_guard_rs-0.2.1/PKG-INFO` & `cfn_guard_rs-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn_guard_rs
-Version: 0.2.1
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyyaml>=5.0.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

