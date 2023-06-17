# Comparing `tmp/phylodm-2.2.1.tar.gz` & `tmp/phylodm-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylodm-2.2.1.tar", last modified: Mon Jan  9 03:46:18 2023, max compression
+gzip compressed data, was "phylodm-3.0.0.tar", last modified: Sat Jun 17 03:50:35 2023, max compression
```

## Comparing `phylodm-2.2.1.tar` & `phylodm-3.0.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:46:18.345982 phylodm-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-01-09 03:46:07.000000 phylodm-2.2.1/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-09 03:46:07.000000 phylodm-2.2.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-09 03:46:07.000000 phylodm-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-09 03:46:07.000000 phylodm-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-01-09 03:46:18.345982 phylodm-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-01-09 03:46:07.000000 phylodm-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:46:18.341982 phylodm-2.2.1/phylodm/
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-01-09 03:46:07.000000 phylodm-2.2.1/phylodm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:46:18.345982 phylodm-2.2.1/phylodm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-01-09 03:46:18.000000 phylodm-2.2.1/phylodm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-09 03:46:18.000000 phylodm-2.2.1/phylodm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 03:46:18.000000 phylodm-2.2.1/phylodm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 03:46:18.000000 phylodm-2.2.1/phylodm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-09 03:46:18.000000 phylodm-2.2.1/phylodm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-09 03:46:18.000000 phylodm-2.2.1/phylodm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-09 03:46:07.000000 phylodm-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 03:46:18.345982 phylodm-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-09 03:46:07.000000 phylodm-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:46:18.345982 phylodm-2.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18817 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/pdm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/python.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:46:18.345982 phylodm-2.2.1/src/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/tree/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/tree/node.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/tree/types.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-01-09 03:46:07.000000 phylodm-2.2.1/src/util.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:46:18.345982 phylodm-2.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-01-09 03:46:07.000000 phylodm-2.2.1/test/test_phylodm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:50:35.322643 phylodm-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-17 03:50:25.000000 phylodm-3.0.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-17 03:50:26.000000 phylodm-3.0.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 03:50:25.000000 phylodm-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 03:50:25.000000 phylodm-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-17 03:50:35.322643 phylodm-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-17 03:50:25.000000 phylodm-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:50:35.322643 phylodm-3.0.0/phylodm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-17 03:50:25.000000 phylodm-3.0.0/phylodm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:50:35.322643 phylodm-3.0.0/phylodm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-17 03:50:35.000000 phylodm-3.0.0/phylodm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-17 03:50:35.000000 phylodm-3.0.0/phylodm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 03:50:35.000000 phylodm-3.0.0/phylodm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 03:50:35.000000 phylodm-3.0.0/phylodm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 03:50:35.000000 phylodm-3.0.0/phylodm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 03:50:35.000000 phylodm-3.0.0/phylodm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-17 03:50:25.000000 phylodm-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 03:50:35.322643 phylodm-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-17 03:50:25.000000 phylodm-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:50:35.322643 phylodm-3.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/pdm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/python.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:50:35.322643 phylodm-3.0.0/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/tree/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/tree/node.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/tree/types.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-17 03:50:25.000000 phylodm-3.0.0/src/util.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:50:35.322643 phylodm-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-17 03:50:25.000000 phylodm-3.0.0/test/test_phylodm.py
```

### Comparing `phylodm-2.2.1/Cargo.lock` & `phylodm-3.0.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "ahash"
-version = "0.7.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
-dependencies = [
- "getrandom 0.2.8",
- "once_cell",
- "version_check",
-]
-
-[[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "ansi_term"
 version = "0.12.1"
@@ -92,17 +81,17 @@
  "quote",
  "rustc_version",
  "syn",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "env_logger"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a19187fea3ac7e84da7dacf48de0c45d63c6a76f9490dae389aead16c243fce3"
 dependencies = [
@@ -123,26 +112,15 @@
 name = "getrandom"
 version = "0.1.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8fc3cb4d91f53b50155bdcfd23f6a4c39ae1969c2ae85982b135750cccaf5fce"
 dependencies = [
  "cfg-if",
  "libc",
- "wasi 0.9.0+wasi-snapshot-preview1",
-]
-
-[[package]]
-name = "getrandom"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
-dependencies = [
- "cfg-if",
- "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
 ]
 
 [[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
@@ -163,17 +141,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
@@ -184,72 +162,70 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "light_phylogeny"
-version = "2.1.2"
+version = "2.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06bc709bf2c0458e2cc280d25a47d6173bacf889e045cc8f1fc679b88ab2dbaa"
+checksum = "b05b6cc82499caacbc149f9a79c29564151f93c45f049999f0da7657fa4c10ad"
 dependencies = [
  "env_logger",
  "getopt",
  "log",
  "random_color",
  "roxmltree",
  "structopt",
  "svg",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -261,17 +237,17 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
@@ -289,59 +265,59 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.17.2"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a462c1af5ba1fddec1488c4646993a23ae7931f9e170ccba23e9c7c834277797"
+checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
 dependencies = [
- "ahash",
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
+ "rustc-hash",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "phylodm"
-version = "2.2.0"
+version = "2.2.1"
 dependencies = [
  "derive_more",
  "itertools",
  "light_phylogeny",
  "ndarray",
  "numpy",
  "pyo3",
@@ -375,97 +351,97 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a6b1679d49b24bbfe0c803429aa1874472f50d9b363131f0e89fc356b544d03"
 dependencies = [
- "getrandom 0.1.16",
+ "getrandom",
  "libc",
  "rand_chacha",
  "rand_core",
  "rand_hc",
  "rand_pcg",
 ]
 
@@ -481,15 +457,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90bde5296fc891b0cef12a6d03ddccc162ce7b2aff54160af9338f8d40df6d19"
 dependencies = [
- "getrandom 0.1.16",
+ "getrandom",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -519,48 +495,54 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.0"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "roxmltree"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "921904a62e410e37e215c40381b7117f830d9d89ba60ab5236170541dd25646b"
 dependencies = [
  "xmlparser",
 ]
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
@@ -569,17 +551,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "semver"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58bc9567378fc7690d6b2addae4e60ac2eeea07becb2c64b9f218b53865cba2a"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
@@ -611,40 +593,40 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "svg"
-version = "0.8.2"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdb25a4593d6656239319426f4025f7a658157e25e89f0e0319d7516d46042d"
+checksum = "02d815ad337e8449d2374d4248448645edfe74e699343dd5719139d93fa87112"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.11.0"
@@ -652,23 +634,23 @@
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.0"
+version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fdbf052a0783de01e944a6ce7a8cb939e295b1e7be835a1112c3b9a7f047a5a"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
@@ -693,20 +675,14 @@
 [[package]]
 name = "wasi"
 version = "0.9.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
 
 [[package]]
-name = "wasi"
-version = "0.11.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
-
-[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -730,68 +706,68 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "xmlparser"
 version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
```

### Comparing `phylodm-2.2.1/Cargo.toml` & `phylodm-3.0.0/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "phylodm"
-version = "2.2.1"
+version = "3.0.0"
 authors = ["Aaron Mussig <aaronmussig@gmail.com>"]
 edition = "2021"
 description = "Efficient calculation of phylogenetic distance matrices."
 readme = "README.md"
 repository = "https://github.com/aaronmussig/PhyloDM"
 license = "GPL-3.0"
 
@@ -14,16 +14,16 @@
 [features]
 python = ["pyo3", "numpy"]
 
 [dependencies]
 light_phylogeny = "2.1"
 derive_more = "0.99"
 itertools = "0.10"
-pyo3 = { version = "0.17", features = ["extension-module"], optional = true }
-numpy = { version = "0.17", optional = true }
+pyo3 = { version = "0.19.0", features = ["extension-module"], optional = true }
+numpy = { version = "0.19.0", optional = true }
 ndarray = "0.15"
 
 [profile.release]
 lto = true
 codegen-units = 1
 opt-level = 3
 strip = true
```

### Comparing `phylodm-2.2.1/LICENSE` & `phylodm-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phylodm-2.2.1/PKG-INFO` & `phylodm-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylodm
-Version: 2.2.1
+Version: 3.0.0
 Summary: Efficient calculation of phylogenetic distance matrices.
 Home-page: https://github.com/aaronmussig/PhyloDM
 Author: Aaron Mussig
 Author-email: aaronmussig@gmail.com
 License: GPL3
 Project-URL: Bug Tracker, https://github.com/aaronmussig/PhyloDM/issues
 Project-URL: Documentation, https://github.com/aaronmussig/PhyloDM
```

### Comparing `phylodm-2.2.1/README.md` & `phylodm-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `phylodm-2.2.1/phylodm/__init__.py` & `phylodm-3.0.0/phylodm/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Optional, List
 from typing import TYPE_CHECKING
 
+import dendropy
+
 if TYPE_CHECKING:
-    import dendropy
     import numpy as np
 
 from .pdm import PhyloDM as PDM
 
 
 class PhyloDM:
 
@@ -19,17 +20,24 @@
     @classmethod
     def load_from_newick_path(cls, path: str) -> 'PhyloDM':
         """Load a tree from a Newick file.
 
         Args:
             path: The path to the Newick file.
         """
-        pdm = cls()
-        pdm._rs.load_from_newick_path(path=path)
-        return pdm
+        try:
+            pdm = cls()
+            pdm._rs.load_from_newick_path(path=path)
+            return pdm
+        except Exception as e:
+            print(f'Unable to load newick tree using light_phylogeny (Rust). '
+                  f'This is likely due to it not supporting the extended Newick format... '
+                  f'falling back to DendroPy to load the tree.')
+            tree = dendropy.Tree.get(path=path, schema='newick')
+            return cls.load_from_dendropy(tree)
 
     @classmethod
     def load_from_dendropy(cls, tree: dendropy.Tree) -> 'PhyloDM':
         """Load a tree from a Dendropy tree object.
 
         Args:
             tree: The Dendropy tree object.
```

### Comparing `phylodm-2.2.1/phylodm.egg-info/PKG-INFO` & `phylodm-3.0.0/phylodm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylodm
-Version: 2.2.1
+Version: 3.0.0
 Summary: Efficient calculation of phylogenetic distance matrices.
 Home-page: https://github.com/aaronmussig/PhyloDM
 Author: Aaron Mussig
 Author-email: aaronmussig@gmail.com
 License: GPL3
 Project-URL: Bug Tracker, https://github.com/aaronmussig/PhyloDM/issues
 Project-URL: Documentation, https://github.com/aaronmussig/PhyloDM
```

### Comparing `phylodm-2.2.1/setup.py` & `phylodm-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,13 +59,13 @@
           'Programming Language :: Python :: 3.11',
           'Programming Language :: Rust',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
       ],
       keywords='phylogenetic distance matrix symmetric',
       packages=['phylodm'],
       install_requires=['numpy'],
-      setup_requires=['setuptools-rust', 'setuptools', 'wheel'],
+      setup_requires=['setuptools-rust', 'setuptools', 'wheel', 'dendropy'],
       python_requires='>=3.7',
       data_files=[("", ["LICENSE"])],
       rust_extensions=[RustExtension("phylodm.pdm", binding=Binding.PyO3, features=['python'])],
       zip_safe=False,
       )
```

### Comparing `phylodm-2.2.1/src/pdm.rs` & `phylodm-3.0.0/src/pdm.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 use std::collections::HashMap;
+use std::panic;
 
 use itertools::Itertools;
 use light_phylogeny::ArenaTree as LpTree;
 use light_phylogeny::read_newick;
 use ndarray::Array2;
 
+use crate::error::PhyloErr;
 use crate::tree::{Edge, NodeDepth, NodeId, Taxon};
 use crate::tree::Node;
 use crate::util::{create_row_vec_from_mat_dims, row_idx_from_mat_coords, row_vec_to_symmat};
 
 /// Create and manipulate the Phylogenetic Distance Matrix.
 ///
 /// # Examples
 ///
 /// ```
 /// use phylodm::PDM;
 ///
 /// let mut tree = PDM::default();
 /// tree.load_from_newick_path("examples/example.tree");
 ///
-/// let (taxa, dm) = tree.matrix(true);
+/// let (taxa, dm) = tree.matrix(true).unwrap();
 /// ```
 #[derive(Default)]
 pub struct PDM {
     pub(crate) nodes: Vec<Node>,
     pub(crate) taxon_to_node_id: HashMap<Taxon, NodeId>,
     pub(crate) leaf_idx_to_row_idx: HashMap<NodeId, usize>,
     pub(crate) leaf_idx_to_row_idx_vec: Vec<usize>,
@@ -36,42 +38,52 @@
     /// Return the number of nodes (leaf + internal) in the tree.
     #[must_use]
     fn n_nodes(&self) -> usize {
         self.nodes.len()
     }
 
     /// Return all leaf nodes in the tree.
-    #[must_use]
-    pub fn leaf_nodes(&self) -> Vec<Taxon> {
+    ///
+    /// # Errors
+    /// In the event that a leaf node has no taxon, this function will return an error.
+    /// This case should never happen, but is possible due to the way the tree is constructed.
+    pub fn leaf_nodes(&self) -> Result<Vec<Taxon>, PhyloErr> {
         let mut out = Vec::with_capacity(self.row_idx_to_leaf_idx.len());
         for leaf_idx in &self.row_idx_to_leaf_idx {
             let leaf = self.get_node(*leaf_idx);
-            out.push(leaf.taxon.clone().expect("Leaf node has no taxon! Please report this error."));
+            let Some(taxon) = &leaf.taxon else {
+                return Err(PhyloErr("Leaf node has no taxon! Please report this error.".to_string()));
+            };
+            out.push(taxon.clone());
         }
-        out
+        Ok(out)
     }
 
     /// Return the sum of all branches in the tree.
     #[must_use]
     pub fn length(&self) -> Edge {
         self.nodes
             .iter()
             .map(|n| n.parent_distance.unwrap_or(Edge(0.0)))
             .sum()
     }
 
-    /// Returns a vector of node indices at a specific depth. Panics if depth doesn't exist.
-    #[must_use]
-    fn get_node_idxs_at_depth(&self, depth: NodeDepth) -> Vec<NodeId> {
-        let nodes_at_depth = self.nodes_at_depth.get(&depth).expect("No nodes at depth!");
+    /// Returns a vector of node indices at a specific depth. Errors if depth doesn't exist.
+    fn get_node_idxs_at_depth(&self, depth: NodeDepth) -> Result<Vec<NodeId>, PhyloErr> {
+        if self.nodes_at_depth.get(&depth).is_none() {
+            return Err(PhyloErr("No nodes at depth! Please report this error.".to_string()));
+        }
+        let Some(nodes_at_depth) = self.nodes_at_depth.get(&depth) else {
+            return Err(PhyloErr("No nodes at depth! Please report this error.".to_string()));
+        };
         let mut nodes: Vec<NodeId> = Vec::with_capacity(nodes_at_depth.len());
         for node_id in nodes_at_depth {
             nodes.push(*node_id);
         }
-        nodes
+        Ok(nodes)
     }
 
     /// Return the number of leaf nodes in the tree.
     #[must_use]
     pub fn n_leaf_nodes(&self) -> usize {
         self.leaf_idx_to_row_idx.len()
     }
@@ -89,41 +101,41 @@
         let i_idx = self.get_row_vec_idx_from_leaf_idx(i);
         let j_idx = self.get_row_vec_idx_from_leaf_idx(j);
         row_idx_from_mat_coords(n_taxa, i_idx, j_idx)
     }
 
     /// Add a new leaf node to the tree.
     /// Returns the ID of the new node.
-    fn add_leaf_node(&mut self, taxon: &Taxon) -> NodeId {
+    fn add_leaf_node(&mut self, taxon: &Taxon) -> Result<NodeId, PhyloErr> {
         // Panic if the taxon is already in the tree.
-        assert!(!self.taxon_to_node_id.contains_key(taxon),
-                "Taxon already exists in the tree: '{:?}'", taxon);
+        if self.taxon_to_node_id.contains_key(taxon) {
+            return Err(PhyloErr(format!("Taxon already exists in the tree: '{taxon:?}'")));
+        }
 
         // Create the new node, and place it in the tree.
         let node_id = NodeId(self.n_nodes());
         self.taxon_to_node_id.insert(taxon.clone(), node_id);
         self.leaf_idx_to_row_idx.insert(node_id, self.leaf_idx_to_row_idx.len());
         self.row_idx_to_leaf_idx.push(node_id);
         self.nodes.push(Node::new(node_id, Some(taxon.clone())));
-        return self.nodes.last().unwrap().id;
+        return Ok(self.nodes.last().unwrap().id);
     }
 
     /// Add a new internal node to the tree.
     fn add_internal_node(&mut self) -> NodeId {
         let node_id = NodeId(self.n_nodes());
         self.nodes.push(Node::new(node_id, None));
         return self.nodes.last().unwrap().id;
     }
 
     /// Add a node to the tree.
-    // TODO: Remove this method.
-    pub(crate) fn add_node(&mut self, taxon: Option<&Taxon>) -> NodeId {
+    pub(crate) fn add_node(&mut self, taxon: Option<&Taxon>) -> Result<NodeId, PhyloErr> {
         match taxon {
             Some(t) => self.add_leaf_node(t),
-            None => self.add_internal_node(),
+            None => Ok(self.add_internal_node()),
         }
     }
 
     /// Retrieve a node from the tree.
     #[must_use]
     fn get_node(&self, node_id: NodeId) -> &Node {
         &self.nodes[node_id.0]
@@ -145,33 +157,37 @@
     ///
     pub(crate) fn add_edge(&mut self, parent: NodeId, child: NodeId, length: Edge) {
         self.get_node_mut(parent).add_child(child);
         self.get_node_mut(child).set_parent(parent, length);
     }
 
     /// Set the depth of each node in the tree.
-    fn assign_node_depth(&mut self) {
+    fn assign_node_depth(&mut self) -> Result<(), PhyloErr> {
         // Iterate over each node to make sure there is only one root node.
         let mut root = None;
-        self.nodes.iter().for_each(|node| {
+        for node in &self.nodes {
             if node.is_root() {
-                assert!(root.is_none(), "Multiple root nodes detected!");
+                if root.is_some() {
+                    return Err(PhyloErr("Multiple root nodes detected!".to_string()));
+                }
                 root = Some(node.id);
             }
-        });
+        }
 
-        // Panic if no root node could be found.
-        assert!(root.is_some(), "No root node found!");
+        if root.is_none() {
+            return Err(PhyloErr("No root node detected!".to_string()));
+        }
 
         // Set the depth of all nodes
-        self.set_node_depth_dfs(root.unwrap());
+        self.set_node_depth_dfs(root.unwrap())?;
+        Ok(())
     }
 
     /// Set the depth of all nodes using a depth first search.
-    fn set_node_depth_dfs(&mut self, root_id: NodeId) {
+    fn set_node_depth_dfs(&mut self, root_id: NodeId) -> Result<(), PhyloErr> {
         let mut nodes_at_depth: HashMap<NodeDepth, Vec<NodeId>> = HashMap::new();
 
         // Seed the stack with the root node.
         let mut stack = vec![(root_id, NodeDepth(0))];
 
         // Iterate over the stack.
         while let Some((node_id, depth)) = stack.pop() {
@@ -188,41 +204,45 @@
             // Add the children to the stack
             node.children.iter().for_each(|child_id| {
                 stack.push((*child_id, depth + NodeDepth(1)));
             });
         }
 
         // Check that the root is the only node at depth 0.
-        let nodes_at_depth_0 = nodes_at_depth.get(&NodeDepth(0)).expect("Root node not found!");
-        assert!(
-            !(nodes_at_depth_0.len() != 1 && nodes_at_depth_0[0] != root_id),
-            "Root node not found!"
-        );
+        if nodes_at_depth.get(&NodeDepth(0)).is_none() {
+            return Err(PhyloErr("Root node not found!".to_string()));
+        }
+        let Some(nodes_at_depth_0) = nodes_at_depth.get(&NodeDepth(0)) else {
+            return Err(PhyloErr("No nodes were found at depth 0, report this error.".to_string()));
+        };
+        if nodes_at_depth_0.len() != 1 && nodes_at_depth_0[0] != root_id {
+            return Err(PhyloErr("Root node not found!".to_string()));
+        }
 
         // Check that the deepest nodes have no children.
         let deepest_node_depth = NodeDepth(nodes_at_depth.len() - 1);
-        nodes_at_depth
-            .get(&deepest_node_depth)
-            .into_iter()
-            .for_each(|nodes| {
-                for node_id in nodes.iter() {
-                    let node = self.get_node(*node_id);
-                    assert!(node.is_leaf(), "Node has children: {:?}", node_id);
-                }
-            });
+        let Some(deepest_nodes) = nodes_at_depth.get(&deepest_node_depth) else {
+            return Err(PhyloErr("No nodes were found at depth max, report this error.".to_string()));
+        };
+        for node_id in deepest_nodes {
+            let node = self.get_node(*node_id);
+            if !node.is_leaf() {
+                return Err(PhyloErr("Node has children!".to_string()));
+            }
+        }
 
         // Save the hashmap
         self.nodes_at_depth = nodes_at_depth;
+        Ok(())
     }
 
     /// Wrapper method to calculate the pairwise distances at a given depth.
-    fn calculate_distances_at_depth(&mut self, depth: NodeDepth, row_vec: &mut [f64]) {
+    fn calculate_distances_at_depth(&mut self, depth: NodeDepth, row_vec: &mut [f64]) -> Result<(), PhyloErr> {
         // Iterate over all nodes a this depth
-
-        for &node_id in &self.get_node_idxs_at_depth(depth) {
+        for &node_id in &self.get_node_idxs_at_depth(depth)? {
             let node = self.get_node(node_id);
 
             // This is a leaf node, set the child distances to 0
             if node.is_leaf() {
                 self.get_node_mut(node_id).set_desc_distances_as_leaf();
             } else if node.children.len() == 1 {
                 // This only happens with malformed trees, bring forward the distances.
@@ -232,61 +252,28 @@
                         child_node.desc_distances.as_ref().unwrap().clone();
                     for edge in new_desc_distances.values_mut() {
                         *edge = *edge + node.parent_distance.unwrap_or(Edge(0.0));
                     }
                     self.get_node_mut(node_id)
                         .set_desc_distances(&Some(new_desc_distances));
                 } else {
-                    panic!("Unknown error, please report this.")
+                    return Err(PhyloErr("Unknown error, please report this.".to_string()));
                 }
             } else {
                 // 1. Set the descendant distances for this node.
                 self.set_node_descendant_distance(node_id);
 
                 // 2. Calculate the pairwise distances for the leaf nodes.
                 self.calc_pairwise_distances_to_leaf_nodes(node_id, row_vec);
 
                 // Free un-used memory
                 self.unset_node_child_distances(node_id);
             }
         }
-
-        // self.get_node_idxs_at_depth(depth)
-        //     .into_iter()
-        //     .for_each(|node_id| {
-        //         let node = self.get_node(node_id);
-        //
-        //         // This is a leaf node, set the child distances to 0
-        //         if node.is_leaf() {
-        //             self.get_node_mut(node_id).set_desc_distances_as_leaf();
-        //         } else if node.children.len() == 1 {
-        //             // This only happens with malformed trees, bring forward the distances.
-        //             let child_node = self.get_node(node.children[0]);
-        //             if child_node.desc_distances.is_some() {
-        //                 let mut new_desc_distances =
-        //                     child_node.desc_distances.as_ref().unwrap().clone();
-        //                 for edge in new_desc_distances.values_mut() {
-        //                     *edge = *edge + node.parent_distance.unwrap_or(Edge(0.0));
-        //                 }
-        //                 self.get_node_mut(node_id)
-        //                     .set_desc_distances(&Some(new_desc_distances));
-        //             } else {
-        //                 panic!("Unknown error, please report this.")
-        //             }
-        //         } else {
-        //             // 1. Set the descendant distances for this node.
-        //             self.set_node_descendant_distance(node_id);
-        //
-        //             // 2. Calculate the pairwise distances for the leaf nodes.
-        //             self.calc_pairwise_distances_to_leaf_nodes(node_id, row_vec);
-        //
-        //             // Free un-used memory
-        //             self.unset_node_child_distances(node_id);
-        //         }
-        //     });
+        Ok(())
     }
 
     /// For a given node, iterate over its children and unset the descendant distances.
     /// This is mainly to free memory during distance matrix calculation.
     fn unset_node_child_distances(&mut self, node_id: NodeId) {
         self.get_node(node_id)
             .children
@@ -389,75 +376,97 @@
         self.leaf_idx_to_row_idx_vec = new_row_idx_to_leaf_idx_vec;
     }
 
     /// Return the symmetrical pairwise distance matrix.
     ///
     /// # Arguments
     /// * `norm` - True if the result should be normalized by the sum of all branches in the tree.
-    pub fn matrix(&mut self, norm: bool) -> (Vec<Taxon>, Array2<f64>) {
-        self.compute_row_vec();
+    ///
+    /// # Errors
+    /// If any errors are encountered due to unexpected tree structures, an error will be raised.
+    pub fn matrix(&mut self, norm: bool) -> Result<(Vec<Taxon>, Array2<f64>), PhyloErr> {
+        self.compute_row_vec()?;
 
         let mut array = row_vec_to_symmat(self.row_vec.as_ref().unwrap());
 
         if norm {
             let tree_length = self.length();
             array.mapv_inplace(|x| x / tree_length.0);
         }
-        (self.leaf_nodes(), array)
+        Ok((self.leaf_nodes()?, array))
     }
 
     /// Initialise the PDM from a newick file.
-    pub fn load_from_newick_path(&mut self, path: &str) {
-        let mut lp_tree: LpTree<String> = LpTree::default();
-        read_newick(path.to_string(), &mut lp_tree);
+    ///
+    /// # Errors
+    /// If any errors are encountered due to unexpected tree structures, an error will be raised.
+    pub fn load_from_newick_path(&mut self, path: &str) -> Result<(), PhyloErr> {
+        // Catch any errors that light_phylogeny may throw
+        // Suppress the stderr message
+        let prev_hook = panic::take_hook();
+        panic::set_hook(Box::new(|_| {}));
+        let newick_ok = panic::catch_unwind(|| {
+            let mut lp_tree: LpTree<String> = LpTree::default();
+            read_newick(path.to_string(), &mut lp_tree);
+            lp_tree
+        });
+        panic::set_hook(prev_hook);
+        if newick_ok.is_err() {
+            return Err(PhyloErr("Error reading newick file".to_string()));
+        }
+        let lp_tree = newick_ok.unwrap();
+
+        // Import the tree
         for cur_node in &lp_tree.arena {
             if cur_node.name.is_empty() {
-                self.add_node(None);
+                self.add_node(None)?;
             } else {
-                self.add_node(Some(&Taxon(cur_node.name.clone())));
+                self.add_node(Some(&Taxon(cur_node.name.clone())))?;
             }
         }
         for cur_node in &lp_tree.arena {
             if cur_node.parent.is_some() {
                 let parent_node = cur_node.parent.unwrap();
                 self.add_edge(
                     NodeId(parent_node),
                     NodeId(cur_node.idx),
                     Edge(cur_node.l as f64),
                 );
             }
         }
-        self.compute_row_vec();
+        self.compute_row_vec()?;
+        Ok(())
     }
 
     /// Computes the row vector. Required if the PDM was manually created (i.e. not from a newick file).
-    pub fn compute_row_vec(&mut self) {
+    pub fn compute_row_vec(&mut self) -> Result<(), PhyloErr> {
         // For reproducibility, order the taxa
         self.order_leaf_node_idx();
 
         // Create the output row matrix
         let num_leaf = self.n_leaf_nodes();
         let mut row_vec = create_row_vec_from_mat_dims(num_leaf);
 
         // Compute the depth of each node
         // TODO: No need to do this again if no new nodes have been added.
-        self.assign_node_depth();
+        self.assign_node_depth()?;
 
         // Process the deepest nodes first
         let depths = self
             .nodes_at_depth
             .keys()
             .sorted()
             .rev()
             .copied()
             .collect::<Vec<_>>();
         for cur_depth in depths {
-            self.calculate_distances_at_depth(cur_depth, &mut row_vec);
+            self.calculate_distances_at_depth(cur_depth, &mut row_vec)?;
         }
         self.row_vec = Some(row_vec);
+        Ok(())
     }
 
     fn get_taxon_node_idx(&self, taxon: &Taxon) -> NodeId {
         self.taxon_to_node_id[taxon]
     }
 
     /// Return the distance between two taxa.
```

### Comparing `phylodm-2.2.1/src/python.rs` & `phylodm-3.0.0/src/python.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use numpy::{PyArray2, ToPyArray};
 use pyo3::{Py, pyclass, pymethods, pymodule, PyResult, Python, types::PyModule};
+use pyo3::exceptions::PyValueError;
 
 use crate::pdm::PDM as RustPhyloDM;
 use crate::tree::{Edge, NodeId, Taxon};
 
 #[pyclass]
 struct PhyloDM {
     tree: RustPhyloDM,
@@ -14,24 +15,31 @@
     #[new]
     fn new() -> Self {
         Self {
             tree: RustPhyloDM::default(),
         }
     }
 
-    pub fn load_from_newick_path(&mut self, path: &str) {
-        self.tree.load_from_newick_path(path);
+    pub fn load_from_newick_path(&mut self, path: &str) -> PyResult<()> {
+        let result = self.tree.load_from_newick_path(path);
+        if result.is_err() {
+            return Err(PyValueError::new_err("Unable to load newick."));
+        }
+        Ok(())
     }
 
-    pub fn add_node(&mut self, taxon: Option<&str>) -> usize {
-        match taxon {
+    pub fn add_node(&mut self, taxon: Option<&str>) -> PyResult<usize> {
+        let out = match taxon {
             Some(taxon) => self.tree.add_node(Some(&Taxon(taxon.to_string()))),
             None => self.tree.add_node(None),
+        };
+        if out.is_err() {
+            return Err(PyValueError::new_err("Unable to add node."));
         }
-            .0
+        Ok(out.unwrap().0)
     }
 
     pub fn add_edge(&mut self, parent_id: usize, child_id: usize, length: f64) {
         self.tree.add_edge(
             NodeId(parent_id),
             NodeId(child_id),
             Edge(length),
@@ -42,37 +50,48 @@
         let mut out = Vec::new();
         for node in &self.tree.nodes {
             out.push(node.id.0);
         }
         out
     }
 
-    pub fn dm(&mut self, norm: bool) -> Py<PyArray2<f64>> {
-        let (_, array) = self.tree.matrix(norm);
-        Python::with_gil(|py| {
+    pub fn dm(&mut self, norm: bool) -> PyResult<Py<PyArray2<f64>>> {
+        let matrix = self.tree.matrix(norm);
+        if matrix.is_err() {
+            return Err(PyValueError::new_err("Unable to compute distance matrix."));
+        }
+        let (_, array) = matrix.unwrap();
+        Ok(Python::with_gil(|py| {
             return Py::from(array.to_pyarray(py));
-        })
+        }))
     }
 
-    pub fn taxa(&self) -> Vec<String> {
+    pub fn taxa(&self) -> PyResult<Vec<String>> {
         let mut out: Vec<String> = Vec::new();
-        for taxon in self.tree.leaf_nodes() {
+        let taxa = self.tree.leaf_nodes();
+        if taxa.is_err() {
+            return Err(PyValueError::new_err("Unable to get taxa."));
+        }
+        for taxon in taxa.unwrap() {
             out.push(taxon.0);
         }
-        out
+        Ok(out)
     }
 
     pub fn length(&self) -> f64 {
         self.tree.length().0
     }
-    
-    pub fn compute_row_vec(&mut self) {
-        self.tree.compute_row_vec();
+
+    pub fn compute_row_vec(&mut self) -> PyResult<()> {
+        if self.tree.compute_row_vec().is_err() {
+            return Err(PyValueError::new_err("Unable to compute row vector."));
+        }
+        Ok(())
     }
-    
+
     pub fn distance(&self, a: &str, b: &str, norm: bool) -> f64 {
         let taxon_a = Taxon(a.to_string());
         let taxon_b = Taxon(b.to_string());
         self.tree.distance(&taxon_a, &taxon_b, norm)
     }
 }
```

### Comparing `phylodm-2.2.1/src/tree/node.rs` & `phylodm-3.0.0/src/tree/node.rs`

 * *Files identical despite different names*

### Comparing `phylodm-2.2.1/src/tree/types.rs` & `phylodm-3.0.0/src/tree/types.rs`

 * *Files identical despite different names*

### Comparing `phylodm-2.2.1/src/util.rs` & `phylodm-3.0.0/src/util.rs`

 * *Files identical despite different names*

### Comparing `phylodm-2.2.1/test/test_phylodm.py` & `phylodm-3.0.0/test/test_phylodm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import tempfile
 import unittest
+from pathlib import Path
 
 import dendropy
 import numpy as np
 from dendropy.simulate import treesim
 
 from phylodm import PhyloDM
 
@@ -140,7 +141,17 @@
         dm = pdm.dm(norm=False)
         delta = test_tree['pd_mat'] - dm
 
         self.assertTrue(np.all(delta < 1e-6))
         self.assertAlmostEqual(pdm.length(), test_tree['length'], places=6)
         self.assertTrue(test_tree['taxa'] == tuple(pdm.taxa()))
         return
+
+    # def test_tree_with_bootstraps_from_newick(self):
+    #     with tempfile.TemporaryDirectory() as tmp_dir:
+    #         tmp_dir = Path(tmp_dir)
+    #         path_newick = tmp_dir / 'newick.tree'
+    #
+    #         # Download the GTDB archaeal newick tree
+    #         url = 'https://data.gtdb.ecogenomic.org/releases/release89/89.0/ar122_r89.tree'
+    #         os.system(f'wget {url} -O {path_newick}')
+    #         PhyloDM.load_from_newick_path(str(path_newick))
```

