# Comparing `tmp/wordle-aid-2.1.tar.gz` & `tmp/wordle-aid-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordle-aid-2.1.tar", last modified: Sat Nov  5 03:01:51 2022, max compression
+gzip compressed data, was "wordle-aid-2.2.tar", last modified: Sat Jun 17 04:51:48 2023, max compression
```

## Comparing `wordle-aid-2.1.tar` & `wordle-aid-2.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-11-05 03:01:51.837119 wordle-aid-2.1/
--rw-r--r--   0 mark      (1000) mark      (1000)     8550 2022-11-05 03:01:51.837119 wordle-aid-2.1/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     8153 2022-11-05 02:30:26.000000 wordle-aid-2.1/README.md
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2022-11-05 03:01:51.837119 wordle-aid-2.1/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)      970 2022-11-05 01:53:11.000000 wordle-aid-2.1/setup.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-11-05 03:01:51.837119 wordle-aid-2.1/wordle_aid.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     8550 2022-11-05 03:01:51.000000 wordle-aid-2.1/wordle_aid.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      238 2022-11-05 03:01:51.000000 wordle-aid-2.1/wordle_aid.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-11-05 03:01:51.000000 wordle-aid-2.1/wordle_aid.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       47 2022-11-05 03:01:51.000000 wordle-aid-2.1/wordle_aid.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       15 2022-11-05 03:01:51.000000 wordle-aid-2.1/wordle_aid.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2022-11-05 03:01:51.000000 wordle-aid-2.1/wordle_aid.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     7222 2022-11-05 01:27:37.000000 wordle-aid-2.1/wordle_aid.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-17 04:51:48.307960 wordle-aid-2.2/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-06-17 04:40:47.000000 wordle-aid-2.2/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       66 2022-09-05 00:17:49.000000 wordle-aid-2.2/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2023-06-17 04:48:21.000000 wordle-aid-2.2/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)     8603 2023-06-17 04:51:48.304627 wordle-aid-2.2/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     8200 2023-06-17 04:49:09.000000 wordle-aid-2.2/README.md
+-rw-r--r--   0 mark      (1000) mark      (1000)      836 2023-06-17 04:48:06.000000 wordle-aid-2.2/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-06-17 04:51:48.307960 wordle-aid-2.2/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)    33247 2022-04-07 04:43:10.000000 wordle-aid-2.2/wordle-example.png
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-17 04:51:48.304627 wordle-aid-2.2/wordle_aid.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     8603 2023-06-17 04:51:48.000000 wordle-aid-2.2/wordle_aid.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      291 2023-06-17 04:51:48.000000 wordle-aid-2.2/wordle_aid.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-17 04:51:48.000000 wordle-aid-2.2/wordle_aid.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-06-17 04:51:48.000000 wordle-aid-2.2/wordle_aid.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       61 2023-06-17 04:51:48.000000 wordle-aid-2.2/wordle_aid.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-06-17 04:51:48.000000 wordle-aid-2.2/wordle_aid.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     7710 2023-06-17 04:48:13.000000 wordle-aid-2.2/wordle_aid.py
```

### Comparing `wordle-aid-2.1/PKG-INFO` & `wordle-aid-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: wordle-aid
-Version: 2.1
+Version: 2.2
 Summary: CLI program to filter word choices to aid solving Wordle game problems
-Home-page: https://github.com/bulletmark/wordle-aid
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
+Project-URL: Homepage, https://github.com/bulletmark/wordle-aid
 Keywords: wordle
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ## WORDLE-AID
 [![PyPi](https://img.shields.io/pypi/v/wordle-aid)](https://pypi.org/project/wordle-aid/)
@@ -230,15 +229,15 @@
 ```
 
 ## Command Line Options
 
 Type `wordle-aid -h` to view the usage summary:
 
 ```
-usage: wordle-aid [-h] [-v VOWELS] [-u] [-s] [-r RANDOM] words [words ...]
+usage: wordle-aid [-h] [-v VOWELS] [-u] [-s] [-r RANDOM] [-V] [words ...]
 
 CLI program to filter word choices to aid solving Wordle game problems.
 
 positional arguments:
   words                 list of attempted words. Upper case letter is right
                         letter but wrong place. Lower case letter is wrong
                         letter anywhere. Last word is wildcards for current
@@ -251,14 +250,15 @@
                         vowels
   -u, --unique          exclude words with non-unique letters
   -s, --solve           solve to final given word, starting with earlier given
                         words (if any)
   -r RANDOM, --random RANDOM
                         choose word for solver at each step randomly from
                         given number (or %) of top candidates, default=1
+  -V, --version         show wordle-aid version
 ```
 
 ## License
 
 Copyright (C) 2022 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `wordle-aid-2.1/README.md` & `wordle-aid-2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 ```
 
 ## Command Line Options
 
 Type `wordle-aid -h` to view the usage summary:
 
 ```
-usage: wordle-aid [-h] [-v VOWELS] [-u] [-s] [-r RANDOM] words [words ...]
+usage: wordle-aid [-h] [-v VOWELS] [-u] [-s] [-r RANDOM] [-V] [words ...]
 
 CLI program to filter word choices to aid solving Wordle game problems.
 
 positional arguments:
   words                 list of attempted words. Upper case letter is right
                         letter but wrong place. Lower case letter is wrong
                         letter anywhere. Last word is wildcards for current
@@ -238,14 +238,15 @@
                         vowels
   -u, --unique          exclude words with non-unique letters
   -s, --solve           solve to final given word, starting with earlier given
                         words (if any)
   -r RANDOM, --random RANDOM
                         choose word for solver at each step randomly from
                         given number (or %) of top candidates, default=1
+  -V, --version         show wordle-aid version
 ```
 
 ## License
 
 Copyright (C) 2022 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `wordle-aid-2.1/wordle_aid.egg-info/PKG-INFO` & `wordle-aid-2.2/wordle_aid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: wordle-aid
-Version: 2.1
+Version: 2.2
 Summary: CLI program to filter word choices to aid solving Wordle game problems
-Home-page: https://github.com/bulletmark/wordle-aid
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
+Project-URL: Homepage, https://github.com/bulletmark/wordle-aid
 Keywords: wordle
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ## WORDLE-AID
 [![PyPi](https://img.shields.io/pypi/v/wordle-aid)](https://pypi.org/project/wordle-aid/)
@@ -230,15 +229,15 @@
 ```
 
 ## Command Line Options
 
 Type `wordle-aid -h` to view the usage summary:
 
 ```
-usage: wordle-aid [-h] [-v VOWELS] [-u] [-s] [-r RANDOM] words [words ...]
+usage: wordle-aid [-h] [-v VOWELS] [-u] [-s] [-r RANDOM] [-V] [words ...]
 
 CLI program to filter word choices to aid solving Wordle game problems.
 
 positional arguments:
   words                 list of attempted words. Upper case letter is right
                         letter but wrong place. Lower case letter is wrong
                         letter anywhere. Last word is wildcards for current
@@ -251,14 +250,15 @@
                         vowels
   -u, --unique          exclude words with non-unique letters
   -s, --solve           solve to final given word, starting with earlier given
                         words (if any)
   -r RANDOM, --random RANDOM
                         choose word for solver at each step randomly from
                         given number (or %) of top candidates, default=1
+  -V, --version         show wordle-aid version
 ```
 
 ## License
 
 Copyright (C) 2022 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `wordle-aid-2.1/wordle_aid.py` & `wordle-aid-2.2/wordle_aid.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 from string import ascii_lowercase
 from collections import Counter, deque
 from random import randint
 
 # 3rd party package
 from spellchecker import SpellChecker
 
-NON = '.'
-VALIDS = set(ascii_lowercase)
-VOWELS = set('aeiou')
+nonchar = '.'
+valids = set(ascii_lowercase)
+vowels = set('aeiou')
 
 # Load list of words from spellchecker
-WORDS = SpellChecker()
+words = SpellChecker()
 
 def get_words(guesses: list, wordmask: str, args: Namespace) -> list:
     'Get list of candidate words + frequencies for given guesses and mask'
     wordlen = len(wordmask)
-    includes = set(wordmask) & VALIDS
-    includes_must = [(p, c) for p, c in enumerate(wordmask) if c in VALIDS]
+    includes = set(wordmask) & valids
+    includes_must = [(p, c) for p, c in enumerate(wordmask) if c in valids]
 
     excludes = set()
     includes_not = []
     counts = []
 
     # Iterate over previous word guesses given on command line ..
     for word in guesses:
         word_count = Counter()
         if len(word) != wordlen:
             sys.exit(f'Word "{word}" must be length {wordlen}')
 
         for pos, csrc in enumerate(word):
             c = csrc.lower()
-            if c not in VALIDS:
+            if c not in valids:
                 sys.exit(f'Word "{word}" has invalid character "{csrc}"')
 
             if c != wordmask[pos]:
                 includes_not.append((pos, c))
 
             if c == csrc:
                 excludes.add(c)
@@ -60,32 +60,32 @@
     # Only bother with chars having multiple (>1) counts
     includes_count = {k: v for k, v in includes_count.items() if v > 1}
 
     excludes -= includes
     candidates = {}
 
     # Iterate over words from dictionary and apply filters ..
-    for word in WORDS:
+    for word in words:
         # Ensure word has required length
         if len(word) != wordlen:
             continue
 
         # Create set() of chars for efficient subsequent checks
         wordset = set(word)
 
         # Ensure word has only valid chars
-        if not wordset.issubset(VALIDS):
+        if not wordset.issubset(valids):
             continue
 
         # If option specified, ensure has unique chars
         if args.unique and len(wordset) != wordlen:
             continue
 
         # If option specified, ensure has required number of vowels
-        if args.vowels and len(wordset & VOWELS) < args.vowels:
+        if args.vowels and len(wordset & vowels) < args.vowels:
             continue
 
         # Ensure has no excluded chars, and has all required includes
         if not wordset.isdisjoint(excludes) or not includes <= wordset:
             continue
 
         # Ensure does not have chars in positions where they must be excluded
@@ -99,15 +99,15 @@
         # Ensure has required multiples of relevant chars
         for c, v in includes_count.items():
             if word.count(c) < v:
                 break
         else:
             # This word is a candidate. If it is in the list twice then
             # record higher frequency.
-            freq = WORDS[word]
+            freq = words[word]
             existing_freq = candidates.get(word, 0)
             if existing_freq < freq:
                 candidates[word] = freq
 
     # Output list of all (word, freq) candidates out in frequency order
     return [(word, candidates[word])
             for word in sorted(candidates, key=candidates.get)]
@@ -124,32 +124,32 @@
     n = randint(1, min(max(1, n), nlen))
     return cands[-n][0]
 
 def score(word: str, target: str) -> str:
     'Score given word against target, returns:'
     ' upper case = letter in correct place'
     ' lower case = letter in incorrect place'
-    ' NON = letter not in word'
+    ' nonchar = letter not in word'
     res = []
     remain = Counter(target)
     for c, t in zip(word, target):
         if c not in target:
-            c = NON
+            c = nonchar
         elif c == t:
             remain[c] -= 1
             c = c.upper()
 
         res.append(c)
 
     nres = []
     for c in res:
         if c.islower():
             remain[c] -= 1
             if remain[c] < 0:
-                c = NON
+                c = nonchar
 
         nres.append(c)
 
     return ''.join(nres)
 
 # This is defined as a standalone function so it could be called as an
 # API for simulation runs etc by providing args_list and stream.
@@ -164,34 +164,53 @@
             help='exclude words with non-unique letters')
     opt.add_argument('-s', '--solve', action='store_true',
             help='solve to final given word, starting with earlier '
                      'given words (if any)')
     opt.add_argument('-r', '--random', default='1',
             help='choose word for solver at each step randomly from given '
                      'number (or %%) of top candidates, default=%(default)s')
-    opt.add_argument('words', nargs='+',
+    opt.add_argument('-V', '--version', action='store_true',
+            help=f'show {opt.prog} version')
+    opt.add_argument('words', nargs='*',
             help='list of attempted words. Upper case letter is right '
             'letter but wrong place. '
             'Lower case letter is wrong letter anywhere. Last word is '
             'wildcards for current matches.')
 
     args = opt.parse_args(args_list)
 
+    if args.version:
+        try:
+            from importlib.metadata import version
+        except ImportError:
+            from importlib_metadata import version
+
+        try:
+            ver = version(opt.prog)
+        except Exception:
+            ver = 'unknown'
+
+        print(ver)
+        return
+
+    if not args.words:
+        opt.error('Must enter words')
+
     guesses = args.words[:-1]
     wordmask = args.words[-1]
     wordmask_l = wordmask.lower()
 
     if not args.solve:
         # Just run normal aid tool
         for word, freq in get_words(guesses, wordmask_l, args):
             print(word, freq, file=fp)
         return
 
     # Else run solver ..
-    if not set(wordmask_l).issubset(VALIDS):
+    if not set(wordmask_l).issubset(valids):
         sys.exit(f'Invalid word {wordmask} to solve')
 
     res = '.' * len(wordmask_l)
     guesses = deque(guesses)
     nguesses = []
 
     for count in itertools.count(1):
```

