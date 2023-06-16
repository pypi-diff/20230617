# Comparing `tmp/tree-sitter-apertium-0.1.4.tar.gz` & `tmp/tree-sitter-apertium-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-apertium-0.1.4.tar", last modified: Thu Jun 15 06:10:57 2023, max compression
+gzip compressed data, was "tree-sitter-apertium-0.1.5.tar", last modified: Thu Jun 15 22:25:05 2023, max compression
```

## Comparing `tree-sitter-apertium-0.1.4.tar` & `tree-sitter-apertium-0.1.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.700563 tree-sitter-apertium-0.1.4/
--rw-r--r--   0 root         (0) root         (0)      168 2022-12-25 12:19:26.000000 tree-sitter-apertium-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-15 06:10:57.700191 tree-sitter-apertium-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-25 12:19:26.000000 tree-sitter-apertium-0.1.4/README
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 06:10:57.700786 tree-sitter-apertium-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-15 06:10:32.000000 tree-sitter-apertium-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.624670 tree-sitter-apertium-0.1.4/test/
--rw-r--r--   0 root         (0) root         (0)     1463 2022-12-25 13:46:09.000000 tree-sitter-apertium-0.1.4/test/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.625557 tree-sitter-apertium-0.1.4/tree_sitter_apertium/
--rw-r--r--   0 root         (0) root         (0)     1367 2022-12-25 13:46:09.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.620823 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.615716 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.635926 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/
--rw-r--r--   0 root         (0) root         (0)    92560 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/grammar.json
--rw-r--r--   0 root         (0) root         (0)    50961 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/node-types.json
--rw-r--r--   0 root         (0) root         (0)  2066617 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/parser.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.651175 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/tree_sitter/
--rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/tree_sitter/parser.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.616600 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.654962 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/
--rw-r--r--   0 root         (0) root         (0)    24418 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/grammar.json
--rw-r--r--   0 root         (0) root         (0)    12484 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/node-types.json
--rw-r--r--   0 root         (0) root         (0)  1121499 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/parser.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.662607 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/tree_sitter/
--rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/tree_sitter/parser.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.617340 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.667058 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/
--rw-r--r--   0 root         (0) root         (0)    34495 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/grammar.json
--rw-r--r--   0 root         (0) root         (0)    15336 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/node-types.json
--rw-r--r--   0 root         (0) root         (0)   228399 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/parser.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.669372 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/tree_sitter/
--rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/tree_sitter/parser.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.618088 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.673145 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/
--rw-r--r--   0 root         (0) root         (0)    67526 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/grammar.json
--rw-r--r--   0 root         (0) root         (0)    25402 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/node-types.json
--rw-r--r--   0 root         (0) root         (0)   394563 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/parser.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.678597 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/tree_sitter/
--rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/tree_sitter/parser.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.619304 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.682006 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/
--rw-r--r--   0 root         (0) root         (0)    20876 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/grammar.json
--rw-r--r--   0 root         (0) root         (0)    12702 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/node-types.json
--rw-r--r--   0 root         (0) root         (0)   140281 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/parser.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.684455 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/tree_sitter/
--rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 06:10:35.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/tree_sitter/parser.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.621245 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.688594 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/
--rw-r--r--   0 root         (0) root         (0)    18628 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/grammar.json
--rw-r--r--   0 root         (0) root         (0)     9158 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/node-types.json
--rw-r--r--   0 root         (0) root         (0)  1561147 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/parser.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.699243 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/tree_sitter/
--rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 06:10:34.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/tree_sitter/parser.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 06:10:57.631435 tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-15 06:10:57.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1574 2023-06-15 06:10:57.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 06:10:57.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 06:10:57.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 06:10:57.000000 tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.613845 tree-sitter-apertium-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      168 2022-12-25 12:19:26.000000 tree-sitter-apertium-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-15 22:25:05.613478 tree-sitter-apertium-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-25 12:19:26.000000 tree-sitter-apertium-0.1.5/README
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 22:25:05.614057 tree-sitter-apertium-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-15 22:24:41.000000 tree-sitter-apertium-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.534458 tree-sitter-apertium-0.1.5/test/
+-rw-r--r--   0 root         (0) root         (0)     1463 2022-12-25 13:46:09.000000 tree-sitter-apertium-0.1.5/test/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.535347 tree-sitter-apertium-0.1.5/tree_sitter_apertium/
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-06-15 22:24:41.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.530101 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.524957 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.546622 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/
+-rw-r--r--   0 root         (0) root         (0)    92560 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/grammar.json
+-rw-r--r--   0 root         (0) root         (0)    50961 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/node-types.json
+-rw-r--r--   0 root         (0) root         (0)  2066617 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/parser.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.562611 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/tree_sitter/
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/tree_sitter/parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.525925 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.566561 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/
+-rw-r--r--   0 root         (0) root         (0)    24418 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/grammar.json
+-rw-r--r--   0 root         (0) root         (0)    12484 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/node-types.json
+-rw-r--r--   0 root         (0) root         (0)  1121499 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/parser.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.575145 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/tree_sitter/
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/tree_sitter/parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.526703 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.578621 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/
+-rw-r--r--   0 root         (0) root         (0)    34495 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/grammar.json
+-rw-r--r--   0 root         (0) root         (0)    15336 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/node-types.json
+-rw-r--r--   0 root         (0) root         (0)   228399 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/parser.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.581094 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/tree_sitter/
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/tree_sitter/parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.527429 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.586099 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/
+-rw-r--r--   0 root         (0) root         (0)    67526 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/grammar.json
+-rw-r--r--   0 root         (0) root         (0)    25402 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/node-types.json
+-rw-r--r--   0 root         (0) root         (0)   394563 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/parser.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.589457 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/tree_sitter/
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/tree_sitter/parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.528580 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.594643 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/
+-rw-r--r--   0 root         (0) root         (0)    20876 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/grammar.json
+-rw-r--r--   0 root         (0) root         (0)    12702 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/node-types.json
+-rw-r--r--   0 root         (0) root         (0)   140281 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/parser.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.596589 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/tree_sitter/
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 22:24:44.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/tree_sitter/parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.530531 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.600260 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/
+-rw-r--r--   0 root         (0) root         (0)    18628 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/grammar.json
+-rw-r--r--   0 root         (0) root         (0)     9158 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/node-types.json
+-rw-r--r--   0 root         (0) root         (0)  1561147 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/parser.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.612103 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/tree_sitter/
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-06-15 22:24:43.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/tree_sitter/parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:25:05.542131 tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-15 22:25:05.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-06-15 22:25:05.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 22:25:05.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 22:25:05.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 22:25:05.000000 tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/top_level.txt
```

### Comparing `tree-sitter-apertium-0.1.4/PKG-INFO` & `tree-sitter-apertium-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-apertium
-Version: 0.1.4
+Version: 0.1.5
 Summary: tree-sitter grammars for Apertium formats
 Home-page: https://github.com/apertium/tree-sitter-apertium
 Author: Daniel Swanson
 Author-email: awesomeevildudes@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tree-sitter-apertium-0.1.4/setup.py` & `tree-sitter-apertium-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class BD(Distribution):
     def has_ext_modules(self):
         return True
 
 setup(
     name='tree-sitter-apertium',
-    version='0.1.4',
+    version='0.1.5',
     description='tree-sitter grammars for Apertium formats',
     url='https://github.com/apertium/tree-sitter-apertium',
     author='Daniel Swanson',
     author_email='awesomeevildudes@gmail.com',
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
```

### Comparing `tree-sitter-apertium-0.1.4/test/test.py` & `tree-sitter-apertium-0.1.5/test/test.py`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/__init__.py` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,55 @@
     LEXC = Language(path, 'lexc')
     LEXD = Language(path, 'lexd')
     RTX = Language(path, 'rtx')
     TWOLC = Language(path, 'twolc')
     XFST = Language(path, 'xfst')
 
 def parse_bytes(b, lang):
+    '''
+    parse_bytes(b: bytes, lang: tree_sitter.Language) -> tree_sitter.Node
+    Create a parser for lang and use it to parse b.
+    Return the root node of the resulting tree.
+    '''
     p = Parser()
     p.set_language(lang)
     return p.parse(b).root_node
 
 def parse_file(fname, lang):
+    '''
+    parse_file(fname: str, lang: tree_sitter.Language)
+      -> (bytes, tree_sitter.Node)
+    Open file at path fname and parse it with lang.
+    Return the file contents as a bytestring and the root node of the tree.
+    '''
     with open(fname, 'rb') as fin:
         byt = fin.read()
         return byt, parse_bytes(byt, lang)
 
 def text(byt, node, offset=0):
+    '''
+    text(byt: bytes, node: tree_sitter.Node, offset: int = 0) -> str
+    Extract and decode the string corresponding to a particular node.
+    If byt is not the entire original text, offset specifies the starting
+    index of the slice it corresponds to.
+    '''
     return byt[node.start_byte-offset:node.end_byte-offset].decode('utf-8')
 
 def line(node):
+    '''
+    line(node: tree_sitter.Node) -> int
+    Return the human-readable (1-indexed) line number a node starts on.
+    '''
     return node.start_point[0]+1
 
 def end_comment(node):
+    '''
+    end_comment(node: tree_sitter.Node) -> Optional[tree_sitter.Node]
+    Return the comment on the same line as node, if one exists, otherwise None.
+    '''
     if node.type == 'comment':
         return node
     com = node.child_by_field_name('comment')
     if com is not None:
         return com
     cur = node
     ln = node.end_point[0]
```

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/grammar.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/node-types.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/parser.c` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/cg/src/tree_sitter/parser.h` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/cg/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/grammar.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/node-types.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/parser.c` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexc/src/tree_sitter/parser.h` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexc/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/grammar.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/node-types.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/parser.c` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/lexd/src/tree_sitter/parser.h` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/lexd/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/grammar.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/node-types.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/parser.c` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/rtx/src/tree_sitter/parser.h` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/rtx/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/grammar.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/node-types.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/parser.c` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/twolc/src/tree_sitter/parser.h` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/twolc/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/grammar.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/node-types.json` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/parser.c` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium/grammars/xfst/src/tree_sitter/parser.h` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium/grammars/xfst/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/PKG-INFO` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-apertium
-Version: 0.1.4
+Version: 0.1.5
 Summary: tree-sitter grammars for Apertium formats
 Home-page: https://github.com/apertium/tree-sitter-apertium
 Author: Daniel Swanson
 Author-email: awesomeevildudes@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tree-sitter-apertium-0.1.4/tree_sitter_apertium.egg-info/SOURCES.txt` & `tree-sitter-apertium-0.1.5/tree_sitter_apertium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

