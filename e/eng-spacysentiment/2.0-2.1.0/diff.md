# Comparing `tmp/eng_spacysentiment-2.0.tar.gz` & `tmp/eng_spacysentiment-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eng_spacysentiment-2.0.tar", last modified: Fri May  5 13:00:52 2023, max compression
+gzip compressed data, was "eng_spacysentiment-2.1.0.tar", last modified: Sat Jun 17 09:36:27 2023, max compression
```

## Comparing `eng_spacysentiment-2.0.tar` & `eng_spacysentiment-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:00:52.028613 eng_spacysentiment-2.0/
--rw-rw-rw-   0        0        0       34 2023-05-05 13:00:48.000000 eng_spacysentiment-2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      285 2023-05-05 13:00:52.028098 eng_spacysentiment-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 13:00:51.923319 eng_spacysentiment-2.0/eng_spacysentiment/
--rw-rw-rw-   0        0        0      245 2023-05-05 13:00:48.000000 eng_spacysentiment-2.0/eng_spacysentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:00:51.975225 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/
--rw-rw-rw-   0        0        0     2142 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/config.cfg
--rw-rw-rw-   0        0        0      613 2023-05-05 13:00:49.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/meta.json
-drwxrwxrwx   0        0        0        0 2023-05-05 13:00:51.991452 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/textcat/
--rw-rw-rw-   0        0        0      102 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/textcat/cfg
--rw-rw-rw-   0        0        0  2097777 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/textcat/model
--rw-rw-rw-   0        0        0    77663 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/tokenizer
-drwxrwxrwx   0        0        0        0 2023-05-05 13:00:52.026071 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/vocab/
--rw-rw-rw-   0        0        0        1 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/vocab/key2row
--rw-rw-rw-   0        0        0        1 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/vocab/lookups.bin
--rw-rw-rw-   0        0        0   325784 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/vocab/strings.json
--rw-rw-rw-   0        0        0      128 2023-05-05 12:24:06.000000 eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/vocab/vectors
--rw-rw-rw-   0        0        0      613 2023-05-05 13:00:49.000000 eng_spacysentiment-2.0/eng_spacysentiment/meta.json
-drwxrwxrwx   0        0        0        0 2023-05-05 13:00:51.950932 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/
--rw-rw-rw-   0        0        0      285 2023-05-05 13:00:50.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      885 2023-05-05 13:00:51.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:00:50.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-05 13:00:51.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-05 13:00:50.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-05 13:00:51.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 13:00:51.000000 eng_spacysentiment-2.0/eng_spacysentiment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      613 2023-05-05 13:00:48.000000 eng_spacysentiment-2.0/meta.json
--rw-rw-rw-   0        0        0       42 2023-05-05 13:00:52.029648 eng_spacysentiment-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1852 2023-05-05 13:00:48.000000 eng_spacysentiment-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:27.776538 eng_spacysentiment-2.1.0/
+-rw-rw-rw-   0        0        0       79 2023-06-17 09:36:25.000000 eng_spacysentiment-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      891 2023-06-17 09:36:27.776538 eng_spacysentiment-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-06-17 09:36:25.000000 eng_spacysentiment-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:27.701660 eng_spacysentiment-2.1.0/eng_spacysentiment/
+-rw-rw-rw-   0        0        0      247 2023-06-17 09:36:25.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:27.743261 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/
+-rw-rw-rw-   0        0        0      638 2023-06-17 09:36:25.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/README.md
+-rw-rw-rw-   0        0        0     2024 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/config.cfg
+-rw-rw-rw-   0        0        0      642 2023-06-17 09:36:26.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/meta.json
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:27.756207 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/textcat/
+-rw-rw-rw-   0        0        0       95 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/textcat/cfg
+-rw-rw-rw-   0        0        0  2097777 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/textcat/model
+-rw-rw-rw-   0        0        0    77663 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/tokenizer
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:27.774539 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/key2row
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/lookups.bin
+-rw-rw-rw-   0        0        0   968728 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/strings.json
+-rw-rw-rw-   0        0        0      128 2023-06-17 09:16:42.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/vectors
+-rw-rw-rw-   0        0        0      642 2023-06-17 09:36:26.000000 eng_spacysentiment-2.1.0/eng_spacysentiment/meta.json
+drwxrwxrwx   0        0        0        0 2023-06-17 09:36:27.728261 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/
+-rw-rw-rw-   0        0        0      891 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      967 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-17 09:36:27.000000 eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      642 2023-06-17 09:36:25.000000 eng_spacysentiment-2.1.0/meta.json
+-rw-rw-rw-   0        0        0       42 2023-06-17 09:36:27.777538 eng_spacysentiment-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2119 2023-06-17 09:36:25.000000 eng_spacysentiment-2.1.0/setup.py
```

### Comparing `eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/config.cfg` & `eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/config.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,127 @@
-00000000: 5b70 6174 6873 5d0d 0a74 7261 696e 203d  [paths]..train =
-00000010: 206e 756c 6c0d 0a64 6576 203d 206e 756c   null..dev = nul
-00000020: 6c0d 0a76 6563 746f 7273 203d 206e 756c  l..vectors = nul
-00000030: 6c0d 0a69 6e69 745f 746f 6b32 7665 6320  l..init_tok2vec 
-00000040: 3d20 6e75 6c6c 0d0a 0d0a 5b73 7973 7465  = null....[syste
-00000050: 6d5d 0d0a 7365 6564 203d 2030 0d0a 6770  m]..seed = 0..gp
-00000060: 755f 616c 6c6f 6361 746f 7220 3d20 6e75  u_allocator = nu
-00000070: 6c6c 0d0a 0d0a 5b6e 6c70 5d0d 0a6c 616e  ll....[nlp]..lan
-00000080: 6720 3d20 2265 6e22 0d0a 7069 7065 6c69  g = "en"..pipeli
-00000090: 6e65 203d 205b 2274 6578 7463 6174 225d  ne = ["textcat"]
-000000a0: 0d0a 6469 7361 626c 6564 203d 205b 5d0d  ..disabled = [].
-000000b0: 0a62 6566 6f72 655f 6372 6561 7469 6f6e  .before_creation
-000000c0: 203d 206e 756c 6c0d 0a61 6674 6572 5f63   = null..after_c
-000000d0: 7265 6174 696f 6e20 3d20 6e75 6c6c 0d0a  reation = null..
-000000e0: 6166 7465 725f 7069 7065 6c69 6e65 5f63  after_pipeline_c
-000000f0: 7265 6174 696f 6e20 3d20 6e75 6c6c 0d0a  reation = null..
-00000100: 6261 7463 685f 7369 7a65 203d 2031 3030  batch_size = 100
-00000110: 300d 0a74 6f6b 656e 697a 6572 203d 207b  0..tokenizer = {
-00000120: 2240 746f 6b65 6e69 7a65 7273 223a 2273  "@tokenizers":"s
-00000130: 7061 6379 2e54 6f6b 656e 697a 6572 2e76  pacy.Tokenizer.v
-00000140: 3122 7d0d 0a0d 0a5b 636f 6d70 6f6e 656e  1"}....[componen
-00000150: 7473 5d0d 0a0d 0a5b 636f 6d70 6f6e 656e  ts]....[componen
-00000160: 7473 2e74 6578 7463 6174 5d0d 0a66 6163  ts.textcat]..fac
-00000170: 746f 7279 203d 2022 7465 7874 6361 7422  tory = "textcat"
-00000180: 0d0a 7468 7265 7368 6f6c 6420 3d20 302e  ..threshold = 0.
-00000190: 350d 0a0d 0a5b 636f 6d70 6f6e 656e 7473  5....[components
-000001a0: 2e74 6578 7463 6174 2e6d 6f64 656c 5d0d  .textcat.model].
-000001b0: 0a40 6172 6368 6974 6563 7475 7265 7320  .@architectures 
-000001c0: 3d20 2273 7061 6379 2e54 6578 7443 6174  = "spacy.TextCat
-000001d0: 424f 572e 7631 220d 0a65 7863 6c75 7369  BOW.v1"..exclusi
-000001e0: 7665 5f63 6c61 7373 6573 203d 2074 7275  ve_classes = tru
-000001f0: 650d 0a6e 6772 616d 5f73 697a 6520 3d20  e..ngram_size = 
-00000200: 310d 0a6e 6f5f 6f75 7470 7574 5f6c 6179  1..no_output_lay
-00000210: 6572 203d 2066 616c 7365 0d0a 6e4f 203d  er = false..nO =
-00000220: 206e 756c 6c0d 0a0d 0a5b 636f 7270 6f72   null....[corpor
-00000230: 615d 0d0a 0d0a 5b63 6f72 706f 7261 2e64  a]....[corpora.d
-00000240: 6576 5d0d 0a40 7265 6164 6572 7320 3d20  ev]..@readers = 
-00000250: 2273 7061 6379 2e43 6f72 7075 732e 7631  "spacy.Corpus.v1
-00000260: 220d 0a70 6174 6820 3d20 247b 7061 7468  "..path = ${path
-00000270: 732e 6465 767d 0d0a 676f 6c64 5f70 7265  s.dev}..gold_pre
-00000280: 7072 6f63 203d 2066 616c 7365 0d0a 6d61  proc = false..ma
-00000290: 785f 6c65 6e67 7468 203d 2030 0d0a 6c69  x_length = 0..li
-000002a0: 6d69 7420 3d20 300d 0a61 7567 6d65 6e74  mit = 0..augment
-000002b0: 6572 203d 206e 756c 6c0d 0a0d 0a5b 636f  er = null....[co
-000002c0: 7270 6f72 612e 7472 6169 6e5d 0d0a 4072  rpora.train]..@r
-000002d0: 6561 6465 7273 203d 2022 7370 6163 792e  eaders = "spacy.
-000002e0: 436f 7270 7573 2e76 3122 0d0a 7061 7468  Corpus.v1"..path
-000002f0: 203d 2024 7b70 6174 6873 2e74 7261 696e   = ${paths.train
-00000300: 7d0d 0a67 6f6c 645f 7072 6570 726f 6320  }..gold_preproc 
-00000310: 3d20 6661 6c73 650d 0a6d 6178 5f6c 656e  = false..max_len
-00000320: 6774 6820 3d20 300d 0a6c 696d 6974 203d  gth = 0..limit =
-00000330: 2030 0d0a 6175 676d 656e 7465 7220 3d20   0..augmenter = 
-00000340: 6e75 6c6c 0d0a 0d0a 5b74 7261 696e 696e  null....[trainin
-00000350: 675d 0d0a 7365 6564 203d 2024 7b73 7973  g]..seed = ${sys
-00000360: 7465 6d2e 7365 6564 7d0d 0a67 7075 5f61  tem.seed}..gpu_a
-00000370: 6c6c 6f63 6174 6f72 203d 2024 7b73 7973  llocator = ${sys
-00000380: 7465 6d2e 6770 755f 616c 6c6f 6361 746f  tem.gpu_allocato
-00000390: 727d 0d0a 6472 6f70 6f75 7420 3d20 302e  r}..dropout = 0.
-000003a0: 310d 0a61 6363 756d 756c 6174 655f 6772  1..accumulate_gr
-000003b0: 6164 6965 6e74 203d 2031 0d0a 7061 7469  adient = 1..pati
-000003c0: 656e 6365 203d 2031 3630 300d 0a6d 6178  ence = 1600..max
-000003d0: 5f65 706f 6368 7320 3d20 300d 0a6d 6178  _epochs = 0..max
-000003e0: 5f73 7465 7073 203d 2032 3030 3030 0d0a  _steps = 20000..
-000003f0: 6576 616c 5f66 7265 7175 656e 6379 203d  eval_frequency =
-00000400: 2032 3030 0d0a 6672 6f7a 656e 5f63 6f6d   200..frozen_com
-00000410: 706f 6e65 6e74 7320 3d20 5b5d 0d0a 6465  ponents = []..de
-00000420: 765f 636f 7270 7573 203d 2022 636f 7270  v_corpus = "corp
-00000430: 6f72 612e 6465 7622 0d0a 7472 6169 6e5f  ora.dev"..train_
-00000440: 636f 7270 7573 203d 2022 636f 7270 6f72  corpus = "corpor
-00000450: 612e 7472 6169 6e22 0d0a 6265 666f 7265  a.train"..before
-00000460: 5f74 6f5f 6469 736b 203d 206e 756c 6c0d  _to_disk = null.
-00000470: 0a0d 0a5b 7472 6169 6e69 6e67 2e62 6174  ...[training.bat
-00000480: 6368 6572 5d0d 0a40 6261 7463 6865 7273  cher]..@batchers
-00000490: 203d 2022 7370 6163 792e 6261 7463 685f   = "spacy.batch_
-000004a0: 6279 5f77 6f72 6473 2e76 3122 0d0a 6469  by_words.v1"..di
-000004b0: 7363 6172 645f 6f76 6572 7369 7a65 203d  scard_oversize =
-000004c0: 2066 616c 7365 0d0a 746f 6c65 7261 6e63   false..toleranc
-000004d0: 6520 3d20 302e 320d 0a67 6574 5f6c 656e  e = 0.2..get_len
-000004e0: 6774 6820 3d20 6e75 6c6c 0d0a 0d0a 5b74  gth = null....[t
-000004f0: 7261 696e 696e 672e 6261 7463 6865 722e  raining.batcher.
-00000500: 7369 7a65 5d0d 0a40 7363 6865 6475 6c65  size]..@schedule
-00000510: 7320 3d20 2263 6f6d 706f 756e 6469 6e67  s = "compounding
-00000520: 2e76 3122 0d0a 7374 6172 7420 3d20 3130  .v1"..start = 10
-00000530: 300d 0a73 746f 7020 3d20 3130 3030 0d0a  0..stop = 1000..
-00000540: 636f 6d70 6f75 6e64 203d 2031 2e30 3031  compound = 1.001
-00000550: 0d0a 7420 3d20 302e 300d 0a0d 0a5b 7472  ..t = 0.0....[tr
-00000560: 6169 6e69 6e67 2e6c 6f67 6765 725d 0d0a  aining.logger]..
-00000570: 406c 6f67 6765 7273 203d 2022 7370 6163  @loggers = "spac
-00000580: 792e 436f 6e73 6f6c 654c 6f67 6765 722e  y.ConsoleLogger.
-00000590: 7631 220d 0a70 726f 6772 6573 735f 6261  v1"..progress_ba
-000005a0: 7220 3d20 6661 6c73 650d 0a0d 0a5b 7472  r = false....[tr
-000005b0: 6169 6e69 6e67 2e6f 7074 696d 697a 6572  aining.optimizer
-000005c0: 5d0d 0a40 6f70 7469 6d69 7a65 7273 203d  ]..@optimizers =
-000005d0: 2022 4164 616d 2e76 3122 0d0a 6265 7461   "Adam.v1"..beta
-000005e0: 3120 3d20 302e 390d 0a62 6574 6132 203d  1 = 0.9..beta2 =
-000005f0: 2030 2e39 3939 0d0a 4c32 5f69 735f 7765   0.999..L2_is_we
-00000600: 6967 6874 5f64 6563 6179 203d 2074 7275  ight_decay = tru
-00000610: 650d 0a4c 3220 3d20 302e 3031 0d0a 6772  e..L2 = 0.01..gr
-00000620: 6164 5f63 6c69 7020 3d20 312e 300d 0a75  ad_clip = 1.0..u
-00000630: 7365 5f61 7665 7261 6765 7320 3d20 6661  se_averages = fa
-00000640: 6c73 650d 0a65 7073 203d 2030 2e30 3030  lse..eps = 0.000
-00000650: 3030 3030 310d 0a6c 6561 726e 5f72 6174  00001..learn_rat
-00000660: 6520 3d20 302e 3030 310d 0a0d 0a5b 7472  e = 0.001....[tr
-00000670: 6169 6e69 6e67 2e73 636f 7265 5f77 6569  aining.score_wei
-00000680: 6768 7473 5d0d 0a63 6174 735f 7363 6f72  ghts]..cats_scor
-00000690: 6520 3d20 312e 300d 0a63 6174 735f 7363  e = 1.0..cats_sc
-000006a0: 6f72 655f 6465 7363 203d 206e 756c 6c0d  ore_desc = null.
-000006b0: 0a63 6174 735f 6d69 6372 6f5f 7020 3d20  .cats_micro_p = 
-000006c0: 6e75 6c6c 0d0a 6361 7473 5f6d 6963 726f  null..cats_micro
-000006d0: 5f72 203d 206e 756c 6c0d 0a63 6174 735f  _r = null..cats_
-000006e0: 6d69 6372 6f5f 6620 3d20 6e75 6c6c 0d0a  micro_f = null..
-000006f0: 6361 7473 5f6d 6163 726f 5f70 203d 206e  cats_macro_p = n
-00000700: 756c 6c0d 0a63 6174 735f 6d61 6372 6f5f  ull..cats_macro_
-00000710: 7220 3d20 6e75 6c6c 0d0a 6361 7473 5f6d  r = null..cats_m
-00000720: 6163 726f 5f66 203d 206e 756c 6c0d 0a63  acro_f = null..c
-00000730: 6174 735f 6d61 6372 6f5f 6175 6320 3d20  ats_macro_auc = 
-00000740: 6e75 6c6c 0d0a 6361 7473 5f66 5f70 6572  null..cats_f_per
-00000750: 5f74 7970 6520 3d20 6e75 6c6c 0d0a 6361  _type = null..ca
-00000760: 7473 5f6d 6163 726f 5f61 7563 5f70 6572  ts_macro_auc_per
-00000770: 5f74 7970 6520 3d20 6e75 6c6c 0d0a 0d0a  _type = null....
-00000780: 5b70 7265 7472 6169 6e69 6e67 5d0d 0a0d  [pretraining]...
-00000790: 0a5b 696e 6974 6961 6c69 7a65 5d0d 0a76  .[initialize]..v
-000007a0: 6563 746f 7273 203d 2024 7b70 6174 6873  ectors = ${paths
-000007b0: 2e76 6563 746f 7273 7d0d 0a69 6e69 745f  .vectors}..init_
-000007c0: 746f 6b32 7665 6320 3d20 247b 7061 7468  tok2vec = ${path
-000007d0: 732e 696e 6974 5f74 6f6b 3276 6563 7d0d  s.init_tok2vec}.
-000007e0: 0a76 6f63 6162 5f64 6174 6120 3d20 6e75  .vocab_data = nu
-000007f0: 6c6c 0d0a 6c6f 6f6b 7570 7320 3d20 6e75  ll..lookups = nu
-00000800: 6c6c 0d0a 6265 666f 7265 5f69 6e69 7420  ll..before_init 
-00000810: 3d20 6e75 6c6c 0d0a 6166 7465 725f 696e  = null..after_in
-00000820: 6974 203d 206e 756c 6c0d 0a0d 0a5b 696e  it = null....[in
-00000830: 6974 6961 6c69 7a65 2e63 6f6d 706f 6e65  itialize.compone
-00000840: 6e74 735d 0d0a 0d0a 5b69 6e69 7469 616c  nts]....[initial
-00000850: 697a 652e 746f 6b65 6e69 7a65 725d       ize.tokenizer]
+00000000: 5b70 6174 6873 5d0a 7472 6169 6e20 3d20  [paths].train = 
+00000010: 6e75 6c6c 0a64 6576 203d 206e 756c 6c0a  null.dev = null.
+00000020: 7665 6374 6f72 7320 3d20 6e75 6c6c 0a69  vectors = null.i
+00000030: 6e69 745f 746f 6b32 7665 6320 3d20 6e75  nit_tok2vec = nu
+00000040: 6c6c 0a0a 5b73 7973 7465 6d5d 0a73 6565  ll..[system].see
+00000050: 6420 3d20 300a 6770 755f 616c 6c6f 6361  d = 0.gpu_alloca
+00000060: 746f 7220 3d20 6e75 6c6c 0a0a 5b6e 6c70  tor = null..[nlp
+00000070: 5d0a 6c61 6e67 203d 2022 656e 220a 7069  ].lang = "en".pi
+00000080: 7065 6c69 6e65 203d 205b 2274 6578 7463  peline = ["textc
+00000090: 6174 225d 0a64 6973 6162 6c65 6420 3d20  at"].disabled = 
+000000a0: 5b5d 0a62 6566 6f72 655f 6372 6561 7469  [].before_creati
+000000b0: 6f6e 203d 206e 756c 6c0a 6166 7465 725f  on = null.after_
+000000c0: 6372 6561 7469 6f6e 203d 206e 756c 6c0a  creation = null.
+000000d0: 6166 7465 725f 7069 7065 6c69 6e65 5f63  after_pipeline_c
+000000e0: 7265 6174 696f 6e20 3d20 6e75 6c6c 0a62  reation = null.b
+000000f0: 6174 6368 5f73 697a 6520 3d20 3130 3030  atch_size = 1000
+00000100: 0a74 6f6b 656e 697a 6572 203d 207b 2240  .tokenizer = {"@
+00000110: 746f 6b65 6e69 7a65 7273 223a 2273 7061  tokenizers":"spa
+00000120: 6379 2e54 6f6b 656e 697a 6572 2e76 3122  cy.Tokenizer.v1"
+00000130: 7d0a 0a5b 636f 6d70 6f6e 656e 7473 5d0a  }..[components].
+00000140: 0a5b 636f 6d70 6f6e 656e 7473 2e74 6578  .[components.tex
+00000150: 7463 6174 5d0a 6661 6374 6f72 7920 3d20  tcat].factory = 
+00000160: 2274 6578 7463 6174 220a 7468 7265 7368  "textcat".thresh
+00000170: 6f6c 6420 3d20 302e 350a 0a5b 636f 6d70  old = 0.5..[comp
+00000180: 6f6e 656e 7473 2e74 6578 7463 6174 2e6d  onents.textcat.m
+00000190: 6f64 656c 5d0a 4061 7263 6869 7465 6374  odel].@architect
+000001a0: 7572 6573 203d 2022 7370 6163 792e 5465  ures = "spacy.Te
+000001b0: 7874 4361 7442 4f57 2e76 3122 0a65 7863  xtCatBOW.v1".exc
+000001c0: 6c75 7369 7665 5f63 6c61 7373 6573 203d  lusive_classes =
+000001d0: 2074 7275 650a 6e67 7261 6d5f 7369 7a65   true.ngram_size
+000001e0: 203d 2031 0a6e 6f5f 6f75 7470 7574 5f6c   = 1.no_output_l
+000001f0: 6179 6572 203d 2066 616c 7365 0a6e 4f20  ayer = false.nO 
+00000200: 3d20 6e75 6c6c 0a0a 5b63 6f72 706f 7261  = null..[corpora
+00000210: 5d0a 0a5b 636f 7270 6f72 612e 6465 765d  ]..[corpora.dev]
+00000220: 0a40 7265 6164 6572 7320 3d20 2273 7061  .@readers = "spa
+00000230: 6379 2e43 6f72 7075 732e 7631 220a 7061  cy.Corpus.v1".pa
+00000240: 7468 203d 2024 7b70 6174 6873 2e64 6576  th = ${paths.dev
+00000250: 7d0a 676f 6c64 5f70 7265 7072 6f63 203d  }.gold_preproc =
+00000260: 2066 616c 7365 0a6d 6178 5f6c 656e 6774   false.max_lengt
+00000270: 6820 3d20 300a 6c69 6d69 7420 3d20 300a  h = 0.limit = 0.
+00000280: 6175 676d 656e 7465 7220 3d20 6e75 6c6c  augmenter = null
+00000290: 0a0a 5b63 6f72 706f 7261 2e74 7261 696e  ..[corpora.train
+000002a0: 5d0a 4072 6561 6465 7273 203d 2022 7370  ].@readers = "sp
+000002b0: 6163 792e 436f 7270 7573 2e76 3122 0a70  acy.Corpus.v1".p
+000002c0: 6174 6820 3d20 247b 7061 7468 732e 7472  ath = ${paths.tr
+000002d0: 6169 6e7d 0a67 6f6c 645f 7072 6570 726f  ain}.gold_prepro
+000002e0: 6320 3d20 6661 6c73 650a 6d61 785f 6c65  c = false.max_le
+000002f0: 6e67 7468 203d 2030 0a6c 696d 6974 203d  ngth = 0.limit =
+00000300: 2030 0a61 7567 6d65 6e74 6572 203d 206e   0.augmenter = n
+00000310: 756c 6c0a 0a5b 7472 6169 6e69 6e67 5d0a  ull..[training].
+00000320: 7365 6564 203d 2024 7b73 7973 7465 6d2e  seed = ${system.
+00000330: 7365 6564 7d0a 6770 755f 616c 6c6f 6361  seed}.gpu_alloca
+00000340: 746f 7220 3d20 247b 7379 7374 656d 2e67  tor = ${system.g
+00000350: 7075 5f61 6c6c 6f63 6174 6f72 7d0a 6472  pu_allocator}.dr
+00000360: 6f70 6f75 7420 3d20 302e 310a 6163 6375  opout = 0.1.accu
+00000370: 6d75 6c61 7465 5f67 7261 6469 656e 7420  mulate_gradient 
+00000380: 3d20 310a 7061 7469 656e 6365 203d 2031  = 1.patience = 1
+00000390: 3630 300a 6d61 785f 6570 6f63 6873 203d  600.max_epochs =
+000003a0: 2030 0a6d 6178 5f73 7465 7073 203d 2032   0.max_steps = 2
+000003b0: 3030 3030 0a65 7661 6c5f 6672 6571 7565  0000.eval_freque
+000003c0: 6e63 7920 3d20 3230 300a 6672 6f7a 656e  ncy = 200.frozen
+000003d0: 5f63 6f6d 706f 6e65 6e74 7320 3d20 5b5d  _components = []
+000003e0: 0a64 6576 5f63 6f72 7075 7320 3d20 2263  .dev_corpus = "c
+000003f0: 6f72 706f 7261 2e64 6576 220a 7472 6169  orpora.dev".trai
+00000400: 6e5f 636f 7270 7573 203d 2022 636f 7270  n_corpus = "corp
+00000410: 6f72 612e 7472 6169 6e22 0a62 6566 6f72  ora.train".befor
+00000420: 655f 746f 5f64 6973 6b20 3d20 6e75 6c6c  e_to_disk = null
+00000430: 0a0a 5b74 7261 696e 696e 672e 6261 7463  ..[training.batc
+00000440: 6865 725d 0a40 6261 7463 6865 7273 203d  her].@batchers =
+00000450: 2022 7370 6163 792e 6261 7463 685f 6279   "spacy.batch_by
+00000460: 5f77 6f72 6473 2e76 3122 0a64 6973 6361  _words.v1".disca
+00000470: 7264 5f6f 7665 7273 697a 6520 3d20 6661  rd_oversize = fa
+00000480: 6c73 650a 746f 6c65 7261 6e63 6520 3d20  lse.tolerance = 
+00000490: 302e 320a 6765 745f 6c65 6e67 7468 203d  0.2.get_length =
+000004a0: 206e 756c 6c0a 0a5b 7472 6169 6e69 6e67   null..[training
+000004b0: 2e62 6174 6368 6572 2e73 697a 655d 0a40  .batcher.size].@
+000004c0: 7363 6865 6475 6c65 7320 3d20 2263 6f6d  schedules = "com
+000004d0: 706f 756e 6469 6e67 2e76 3122 0a73 7461  pounding.v1".sta
+000004e0: 7274 203d 2031 3030 0a73 746f 7020 3d20  rt = 100.stop = 
+000004f0: 3130 3030 0a63 6f6d 706f 756e 6420 3d20  1000.compound = 
+00000500: 312e 3030 310a 7420 3d20 302e 300a 0a5b  1.001.t = 0.0..[
+00000510: 7472 6169 6e69 6e67 2e6c 6f67 6765 725d  training.logger]
+00000520: 0a40 6c6f 6767 6572 7320 3d20 2273 7061  .@loggers = "spa
+00000530: 6379 2e43 6f6e 736f 6c65 4c6f 6767 6572  cy.ConsoleLogger
+00000540: 2e76 3122 0a70 726f 6772 6573 735f 6261  .v1".progress_ba
+00000550: 7220 3d20 6661 6c73 650a 0a5b 7472 6169  r = false..[trai
+00000560: 6e69 6e67 2e6f 7074 696d 697a 6572 5d0a  ning.optimizer].
+00000570: 406f 7074 696d 697a 6572 7320 3d20 2241  @optimizers = "A
+00000580: 6461 6d2e 7631 220a 6265 7461 3120 3d20  dam.v1".beta1 = 
+00000590: 302e 390a 6265 7461 3220 3d20 302e 3939  0.9.beta2 = 0.99
+000005a0: 390a 4c32 5f69 735f 7765 6967 6874 5f64  9.L2_is_weight_d
+000005b0: 6563 6179 203d 2074 7275 650a 4c32 203d  ecay = true.L2 =
+000005c0: 2030 2e30 310a 6772 6164 5f63 6c69 7020   0.01.grad_clip 
+000005d0: 3d20 312e 300a 7573 655f 6176 6572 6167  = 1.0.use_averag
+000005e0: 6573 203d 2066 616c 7365 0a65 7073 203d  es = false.eps =
+000005f0: 2030 2e30 3030 3030 3030 310a 6c65 6172   0.00000001.lear
+00000600: 6e5f 7261 7465 203d 2030 2e30 3031 0a0a  n_rate = 0.001..
+00000610: 5b74 7261 696e 696e 672e 7363 6f72 655f  [training.score_
+00000620: 7765 6967 6874 735d 0a63 6174 735f 7363  weights].cats_sc
+00000630: 6f72 6520 3d20 312e 300a 6361 7473 5f73  ore = 1.0.cats_s
+00000640: 636f 7265 5f64 6573 6320 3d20 6e75 6c6c  core_desc = null
+00000650: 0a63 6174 735f 6d69 6372 6f5f 7020 3d20  .cats_micro_p = 
+00000660: 6e75 6c6c 0a63 6174 735f 6d69 6372 6f5f  null.cats_micro_
+00000670: 7220 3d20 6e75 6c6c 0a63 6174 735f 6d69  r = null.cats_mi
+00000680: 6372 6f5f 6620 3d20 6e75 6c6c 0a63 6174  cro_f = null.cat
+00000690: 735f 6d61 6372 6f5f 7020 3d20 6e75 6c6c  s_macro_p = null
+000006a0: 0a63 6174 735f 6d61 6372 6f5f 7220 3d20  .cats_macro_r = 
+000006b0: 6e75 6c6c 0a63 6174 735f 6d61 6372 6f5f  null.cats_macro_
+000006c0: 6620 3d20 6e75 6c6c 0a63 6174 735f 6d61  f = null.cats_ma
+000006d0: 6372 6f5f 6175 6320 3d20 6e75 6c6c 0a63  cro_auc = null.c
+000006e0: 6174 735f 665f 7065 725f 7479 7065 203d  ats_f_per_type =
+000006f0: 206e 756c 6c0a 6361 7473 5f6d 6163 726f   null.cats_macro
+00000700: 5f61 7563 5f70 6572 5f74 7970 6520 3d20  _auc_per_type = 
+00000710: 6e75 6c6c 0a0a 5b70 7265 7472 6169 6e69  null..[pretraini
+00000720: 6e67 5d0a 0a5b 696e 6974 6961 6c69 7a65  ng]..[initialize
+00000730: 5d0a 7665 6374 6f72 7320 3d20 247b 7061  ].vectors = ${pa
+00000740: 7468 732e 7665 6374 6f72 737d 0a69 6e69  ths.vectors}.ini
+00000750: 745f 746f 6b32 7665 6320 3d20 247b 7061  t_tok2vec = ${pa
+00000760: 7468 732e 696e 6974 5f74 6f6b 3276 6563  ths.init_tok2vec
+00000770: 7d0a 766f 6361 625f 6461 7461 203d 206e  }.vocab_data = n
+00000780: 756c 6c0a 6c6f 6f6b 7570 7320 3d20 6e75  ull.lookups = nu
+00000790: 6c6c 0a62 6566 6f72 655f 696e 6974 203d  ll.before_init =
+000007a0: 206e 756c 6c0a 6166 7465 725f 696e 6974   null.after_init
+000007b0: 203d 206e 756c 6c0a 0a5b 696e 6974 6961   = null..[initia
+000007c0: 6c69 7a65 2e63 6f6d 706f 6e65 6e74 735d  lize.components]
+000007d0: 0a0a 5b69 6e69 7469 616c 697a 652e 746f  ..[initialize.to
+000007e0: 6b65 6e69 7a65 725d                      kenizer]
```

### Comparing `eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/meta.json` & `eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'author'": "'Vishnu'",*

 * * "'description'": "'sentiment analysis using spacy pipelines'",*

 * * "'license'": "'MIT'",*

 * * "'requirements'": '[]',*

 * * "'spacy_git_version'": "'Unknown'",*

 * * "'url'": "'https://github.com/Vishnunkumar/eng_spacysentiment'",*

 * * "'version'": "'2.1.0'"}*

```diff
@@ -1,31 +1,32 @@
 {
-    "author": "Vishnu Nandakumar",
+    "author": "Vishnu",
     "components": [
         "textcat"
     ],
-    "description": "Sentiment analysis using spacy english base model",
+    "description": "sentiment analysis using spacy pipelines",
     "disabled": [],
     "email": "vishnunkumar25@gmail.com",
     "labels": {
         "textcat": [
             "positive",
             "negative"
         ]
     },
     "lang": "eng",
-    "license": "",
+    "license": "MIT",
     "name": "spacysentiment",
     "pipeline": [
         "textcat"
     ],
-    "spacy_git_version": "c83dfa23d",
+    "requirements": [],
+    "spacy_git_version": "Unknown",
     "spacy_version": ">=3.0.9,<3.1.0",
-    "url": "https://github.com/Vishnunkumar/",
+    "url": "https://github.com/Vishnunkumar/eng_spacysentiment",
     "vectors": {
         "keys": 0,
         "name": null,
         "vectors": 0,
         "width": 0
     },
-    "version": "2.0"
+    "version": "2.1.0"
 }
```

### Comparing `eng_spacysentiment-2.0/eng_spacysentiment/eng_spacysentiment-2.0/tokenizer` & `eng_spacysentiment-2.1.0/eng_spacysentiment/eng_spacysentiment-2.1.0/tokenizer`

 * *Files identical despite different names*

### Comparing `eng_spacysentiment-2.0/eng_spacysentiment/meta.json` & `eng_spacysentiment-2.1.0/eng_spacysentiment/meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'author'": "'Vishnu'",*

 * * "'description'": "'sentiment analysis using spacy pipelines'",*

 * * "'license'": "'MIT'",*

 * * "'requirements'": '[]',*

 * * "'spacy_git_version'": "'Unknown'",*

 * * "'url'": "'https://github.com/Vishnunkumar/eng_spacysentiment'",*

 * * "'version'": "'2.1.0'"}*

```diff
@@ -1,31 +1,32 @@
 {
-    "author": "Vishnu Nandakumar",
+    "author": "Vishnu",
     "components": [
         "textcat"
     ],
-    "description": "Sentiment analysis using spacy english base model",
+    "description": "sentiment analysis using spacy pipelines",
     "disabled": [],
     "email": "vishnunkumar25@gmail.com",
     "labels": {
         "textcat": [
             "positive",
             "negative"
         ]
     },
     "lang": "eng",
-    "license": "",
+    "license": "MIT",
     "name": "spacysentiment",
     "pipeline": [
         "textcat"
     ],
-    "spacy_git_version": "c83dfa23d",
+    "requirements": [],
+    "spacy_git_version": "Unknown",
     "spacy_version": ">=3.0.9,<3.1.0",
-    "url": "https://github.com/Vishnunkumar/",
+    "url": "https://github.com/Vishnunkumar/eng_spacysentiment",
     "vectors": {
         "keys": 0,
         "name": null,
         "vectors": 0,
         "width": 0
     },
-    "version": "2.0"
+    "version": "2.1.0"
 }
```

### Comparing `eng_spacysentiment-2.0/eng_spacysentiment.egg-info/SOURCES.txt` & `eng_spacysentiment-2.1.0/eng_spacysentiment.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 MANIFEST.in
+README.md
 meta.json
 setup.py
 eng_spacysentiment/__init__.py
 eng_spacysentiment/meta.json
 eng_spacysentiment.egg-info/PKG-INFO
 eng_spacysentiment.egg-info/SOURCES.txt
 eng_spacysentiment.egg-info/dependency_links.txt
 eng_spacysentiment.egg-info/entry_points.txt
 eng_spacysentiment.egg-info/not-zip-safe
 eng_spacysentiment.egg-info/requires.txt
 eng_spacysentiment.egg-info/top_level.txt
-eng_spacysentiment/eng_spacysentiment-2.0/config.cfg
-eng_spacysentiment/eng_spacysentiment-2.0/meta.json
-eng_spacysentiment/eng_spacysentiment-2.0/tokenizer
-eng_spacysentiment/eng_spacysentiment-2.0/textcat/cfg
-eng_spacysentiment/eng_spacysentiment-2.0/textcat/model
-eng_spacysentiment/eng_spacysentiment-2.0/vocab/key2row
-eng_spacysentiment/eng_spacysentiment-2.0/vocab/lookups.bin
-eng_spacysentiment/eng_spacysentiment-2.0/vocab/strings.json
-eng_spacysentiment/eng_spacysentiment-2.0/vocab/vectors
+eng_spacysentiment/eng_spacysentiment-2.1.0/README.md
+eng_spacysentiment/eng_spacysentiment-2.1.0/config.cfg
+eng_spacysentiment/eng_spacysentiment-2.1.0/meta.json
+eng_spacysentiment/eng_spacysentiment-2.1.0/tokenizer
+eng_spacysentiment/eng_spacysentiment-2.1.0/textcat/cfg
+eng_spacysentiment/eng_spacysentiment-2.1.0/textcat/model
+eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/key2row
+eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/lookups.bin
+eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/strings.json
+eng_spacysentiment/eng_spacysentiment-2.1.0/vocab/vectors
```

### Comparing `eng_spacysentiment-2.0/meta.json` & `eng_spacysentiment-2.1.0/meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'author'": "'Vishnu'",*

 * * "'description'": "'sentiment analysis using spacy pipelines'",*

 * * "'license'": "'MIT'",*

 * * "'requirements'": '[]',*

 * * "'spacy_git_version'": "'Unknown'",*

 * * "'url'": "'https://github.com/Vishnunkumar/eng_spacysentiment'",*

 * * "'version'": "'2.1.0'"}*

```diff
@@ -1,31 +1,32 @@
 {
-    "author": "Vishnu Nandakumar",
+    "author": "Vishnu",
     "components": [
         "textcat"
     ],
-    "description": "Sentiment analysis using spacy english base model",
+    "description": "sentiment analysis using spacy pipelines",
     "disabled": [],
     "email": "vishnunkumar25@gmail.com",
     "labels": {
         "textcat": [
             "positive",
             "negative"
         ]
     },
     "lang": "eng",
-    "license": "",
+    "license": "MIT",
     "name": "spacysentiment",
     "pipeline": [
         "textcat"
     ],
-    "spacy_git_version": "c83dfa23d",
+    "requirements": [],
+    "spacy_git_version": "Unknown",
     "spacy_version": ">=3.0.9,<3.1.0",
-    "url": "https://github.com/Vishnunkumar/",
+    "url": "https://github.com/Vishnunkumar/eng_spacysentiment",
     "vectors": {
         "keys": 0,
         "name": null,
         "vectors": 0,
         "width": 0
     },
-    "version": "2.0"
+    "version": "2.1.0"
 }
```

### Comparing `eng_spacysentiment-2.0/setup.py` & `eng_spacysentiment-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 
 
 def load_meta(fp):
     with io.open(fp, encoding='utf8') as f:
         return json.load(f)
 
 
+def load_readme(fp):
+    if path.exists(fp):
+        with io.open(fp, encoding='utf8') as f:
+            return f.read()
+    return ""
+
+
 def list_files(data_dir):
     output = []
     for root, _, filenames in walk(data_dir):
         for filename in filenames:
             if not filename.startswith('.'):
                 output.append(path.join(root, filename))
     output = [path.relpath(p, path.dirname(data_dir)) for p in output]
@@ -32,31 +39,34 @@
     return requirements
 
 
 def setup_package():
     root = path.abspath(path.dirname(__file__))
     meta_path = path.join(root, 'meta.json')
     meta = load_meta(meta_path)
+    readme_path = path.join(root, 'README.md')
+    readme = load_readme(readme_path)
     model_name = str(meta['lang'] + '_' + meta['name'])
     model_dir = path.join(model_name, model_name + '-' + meta['version'])
 
     copy(meta_path, path.join(model_name))
     copy(meta_path, model_dir)
 
     setup(
         name=model_name,
         description=meta.get('description'),
+        long_description=readme,
         author=meta.get('author'),
         author_email=meta.get('email'),
         url=meta.get('url'),
         version=meta['version'],
         license=meta.get('license'),
         packages=[model_name],
         package_data={model_name: list_files(model_dir)},
         install_requires=list_requirements(meta),
         zip_safe=False,
         entry_points={'spacy_models': ['{m} = {m}'.format(m=model_name)]}
     )
 
 
 if __name__ == '__main__':
-    setup_package()
+    setup_package()
```

