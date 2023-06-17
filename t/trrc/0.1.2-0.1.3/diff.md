# Comparing `tmp/trrc-0.1.2.tar.gz` & `tmp/trrc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trrc-0.1.2.tar", last modified: Sun Jun 11 22:23:00 2023, max compression
+gzip compressed data, was "trrc-0.1.3.tar", last modified: Sat Jun 17 14:10:02 2023, max compression
```

## Comparing `trrc-0.1.2.tar` & `trrc-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.713771 trrc-0.1.2/
--rw-r--r--   0 constantinhong   (501) staff       (20)    35149 2023-05-30 20:49:49.000000 trrc-0.1.2/LICENSE
--rw-r--r--   0 constantinhong   (501) staff       (20)    59089 2023-06-11 22:23:00.713415 trrc-0.1.2/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)    17304 2023-06-11 22:15:08.000000 trrc-0.1.2/README.md
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.702894 trrc-0.1.2/docs/
--rw-r--r--   0 constantinhong   (501) staff       (20)     4018 2023-06-04 19:36:54.000000 trrc-0.1.2/docs/trrc.1
--rw-r--r--   0 constantinhong   (501) staff       (20)     1334 2023-06-11 22:09:38.000000 trrc-0.1.2/pyproject.toml
--rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-11 22:23:00.713853 trrc-0.1.2/setup.cfg
--rw-r--r--   0 constantinhong   (501) staff       (20)     1578 2023-06-11 22:09:38.000000 trrc-0.1.2/setup.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.707266 trrc-0.1.2/tests/
--rw-r--r--   0 constantinhong   (501) staff       (20)     4620 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_cardcontentsHandle.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     1041 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_classAnkiConnect.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     3009 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_create_parser.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     2803 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_options.py
--rw-r--r--   0 constantinhong   (501) staff       (20)      806 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_pipe_redirection.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     1968 2023-05-26 00:27:04.000000 trrc-0.1.2/tests/test_regexhtml.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     9970 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_utils.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.710672 trrc-0.1.2/trrc/
--rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-01 00:15:14.000000 trrc-0.1.2/trrc/__init__.py
--rwxr-xr-x   0 constantinhong   (501) staff       (20)      354 2023-06-02 19:57:50.000000 trrc-0.1.2/trrc/__main__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     4864 2023-05-30 20:49:49.000000 trrc-0.1.2/trrc/config_opts.py
--rw-r--r--   0 constantinhong   (501) staff       (20)    23892 2023-06-11 22:12:30.000000 trrc-0.1.2/trrc/create_parser.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     7080 2023-06-11 22:09:38.000000 trrc-0.1.2/trrc/parser_opts.py
--rwxr-xr-x   0 constantinhong   (501) staff       (20)    11936 2023-06-11 22:12:30.000000 trrc-0.1.2/trrc/utils.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.712856 trrc-0.1.2/trrc.egg-info/
--rw-r--r--   0 constantinhong   (501) staff       (20)    59089 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      522 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/SOURCES.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/dependency_links.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       44 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/entry_points.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       25 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/requires.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        5 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/top_level.txt
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.849026 trrc-0.1.3/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    35149 2023-05-30 20:49:49.000000 trrc-0.1.3/LICENSE
+-rw-r--r--   0 constantinhong   (501) staff       (20)    59259 2023-06-17 14:10:02.848104 trrc-0.1.3/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)    17474 2023-06-17 14:08:58.000000 trrc-0.1.3/README.md
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.829185 trrc-0.1.3/docs/
+-rw-r--r--   0 constantinhong   (501) staff       (20)     4018 2023-06-04 19:36:54.000000 trrc-0.1.3/docs/trrc.1
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1334 2023-06-17 14:08:58.000000 trrc-0.1.3/pyproject.toml
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.826503 trrc-0.1.3/scripts/
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.829685 trrc-0.1.3/scripts/bash/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      627 2023-06-17 14:08:58.000000 trrc-0.1.3/scripts/bash/trrc
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.830191 trrc-0.1.3/scripts/zsh/
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1730 2023-06-17 14:08:58.000000 trrc-0.1.3/scripts/zsh/_trrc
+-rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-17 14:10:02.849218 trrc-0.1.3/setup.cfg
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1727 2023-06-17 14:08:58.000000 trrc-0.1.3/setup.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.836447 trrc-0.1.3/tests/
+-rw-r--r--   0 constantinhong   (501) staff       (20)     4620 2023-05-30 20:49:49.000000 trrc-0.1.3/tests/test_cardcontentsHandle.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1041 2023-05-30 20:49:49.000000 trrc-0.1.3/tests/test_classAnkiConnect.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     3009 2023-05-30 20:49:49.000000 trrc-0.1.3/tests/test_create_parser.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     2803 2023-05-30 20:49:49.000000 trrc-0.1.3/tests/test_options.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)      806 2023-05-30 20:49:49.000000 trrc-0.1.3/tests/test_pipe_redirection.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1968 2023-05-26 00:27:04.000000 trrc-0.1.3/tests/test_regexhtml.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     9970 2023-05-30 20:49:49.000000 trrc-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.841866 trrc-0.1.3/trrc/
+-rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-01 00:15:14.000000 trrc-0.1.3/trrc/__init__.py
+-rwxr-xr-x   0 constantinhong   (501) staff       (20)      354 2023-06-02 19:57:50.000000 trrc-0.1.3/trrc/__main__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     4864 2023-05-30 20:49:49.000000 trrc-0.1.3/trrc/config_opts.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)    23892 2023-06-11 22:45:52.000000 trrc-0.1.3/trrc/create_parser.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     6973 2023-06-17 14:08:58.000000 trrc-0.1.3/trrc/parser_opts.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)      827 2023-06-14 10:39:14.000000 trrc-0.1.3/trrc/some.py
+-rwxr-xr-x   0 constantinhong   (501) staff       (20)    11936 2023-06-16 16:46:43.000000 trrc-0.1.3/trrc/utils.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-17 14:10:02.846674 trrc-0.1.3/trrc.egg-info/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    59259 2023-06-17 14:10:02.000000 trrc-0.1.3/trrc.egg-info/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)      571 2023-06-17 14:10:02.000000 trrc-0.1.3/trrc.egg-info/SOURCES.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-17 14:10:02.000000 trrc-0.1.3/trrc.egg-info/dependency_links.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       44 2023-06-17 14:10:02.000000 trrc-0.1.3/trrc.egg-info/entry_points.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       25 2023-06-17 14:10:02.000000 trrc-0.1.3/trrc.egg-info/requires.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        5 2023-06-17 14:10:02.000000 trrc-0.1.3/trrc.egg-info/top_level.txt
```

### Comparing `trrc-0.1.2/LICENSE` & `trrc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/PKG-INFO` & `trrc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trrc
-Version: 0.1.2
+Version: 0.1.3
 Summary: a command-line program for creating anki card using AnkiConnect API.
 Home-page: https://github.com/Constantin1489/trrc
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -709,35 +709,37 @@
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [CONFIG_FILE](#config-file)
 * [LOCATIONS](#locations)
 * [OPTIONS](#options)
 * [FAQ](#faq)
-* [CANGELOG](#changelog)
+* [CHANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **ToRRential Card processor**(**trrc**) is a command-line unix-like program to create anki cards using AnkiConnect plugin.(Think a yt-dlp, but this program is for adding cards into Anki.)
 
 I intent to make it as a Unix-like program. Therefore it **leverages a lot of Unix concepts**.
 
-- it **supports a standard input, PIPE, redirection.** Therefore, you can add bulk cards after mangling your cards with your favorite text editors. With the benefit of unix-like program, you can make a convenient script yourself with your favorite text editors like Vim, Emacs, VScode and so on. See [Usage](#usage)
+- It **supports a standard input, PIPE, redirection.** Therefore, you can add bulk cards after mangling your cards with your favorite text editors. With the benefit of unix-like program, you can make a convenient script yourself with your favorite text editors like Vim, Emacs, VScode and so on. See [Usage](#usage)
+
+- It has **shell completions(Zsh, Bash)**.
 
 - It **adds multiple cards at once** using [`--file`](#–file-option) or [PIPE](#pipe) and so on. See [Usage](#usage)
 
 - It also **supports options for ip, port and apikey**. So even some environments you don't want to install Anki, you can add cards if your Anki is running in your home or somewhere, boundlessly.
 
 - It also supports a **rc(config) file** with a alias to reuse options you uses frequently.
 
 - you can **sync Anki** with option `--sync` of **trrc** with or without soon after adding cards.
 
 - It's **user-friendly**. In well-known cases, **trrc** provides solutions. If you
-  mistake deck name, it will print all deck name available. if your field is
+  mistake deck name, it will print all deck name available. If your field is
   wrong, it will print field of the card type used.
 
 ```sh
 # default card type is 'Basic'
 $trrc --field 'fron:bakc:tags' 'What is GPL?	The GNU General Public License is a free, copyleft license for software and other kinds of works.	LICENSE::GPL'
 #### Kinds of failures: 1
 trrc Tip: --field 'Front:Back:Tags'
@@ -782,15 +784,15 @@
 trrc "back\ttestfront\tvim" -F '\t'
 
 # you can set whatever character you want.
 trrc --IFS % '안녕%Hello%Korean'
 trrc -F @ '안녕@Hello@Korean'
 
 # you can choose only part of the fields of the card type.
-# you  can change order of the fields.
+# you can change order of the fields.
 trrc --field 'Arbitrary4thField:Arbitrary2ndFieldName:tags' 'FourthContent\tsecondContent\ttag'
 
 # to send your card to other computer(e.g.: ip is 192.168.1.230, port is 4832).
 trrc --ip 192.168.1.230 --port 4832 --file Korean_English_conversation.txt
 ```
 
 #### # To use '\t' as a tab character in an standard input argument, you need to use '$' in front of the string.
@@ -977,15 +979,15 @@
 ### --file option
 
 #### examplefile.txt
 This is an example which trrc takes. IFS is a tab which is a default IFS.
 
 ```
 Anki	Anki is a free and open-source flashcard program using spaced repetition	anki
-To make  a log message in python, What library Should I use?	logging	python::library
+To make a log message in python, What library Should I use?	logging	python::library
 ```
 * `trrc --file examplefile.txt`
 
 
 ### --read-file-in-a-content
 Let's say you are learning Rust Language.
 Save this statements in a text file called 'rust_hello.txt'
@@ -1110,15 +1112,16 @@
 
 See [iOS_shortcuts_example](docs/tips/iOS_shortcuts_setting_example/iOS_shortcuts_example.md)
 
 ## Changelog
 
 | Version | Note                     | 
 |:--------|:-------------------------|
-| HEAD    | fix sync option error handle. | 
+| HEAD    | add shell completion. | 
+| 0.1.2    | fix sync option error handle. | 
 | 0.1.1   | init                     | 
 
 ## Contribution
 
 Thank you for letting me know the bug! Please report the bug in [issue tracker](https://github.com/Constantin1489/trrc/issues).
 
 Personally I like this app as a method to add cards and use daily, so I will keep developing it. Because I'm trying to get a job, an update delivery can be slow. But after getting a job, I will learn some good clean code conventions and apply it.
@@ -1142,14 +1145,17 @@
 - [ ] windows support.
     - py2exe
     - file path (e.g.: default config file)
 - [ ] send media files directly to Anki.
 - [ ] create card from git-diff, git-show
     - option: --mode=git --header 'Optimize logging message\n		'
     - without --header, use git commit message as header.
+- [ ] support markdown, mad type and so on.
+    - --vertical?
+    - Pseudo HEREDOC mode.
 - [ ] get fields of a deck.
     - error handle.
 - [ ] support shell environment variable.
     - prefix: TRRC
     - e.g.: TRRC_deck, TRRC_tag: global tag
 - [ ] new verbose purpose.
     - -v : stdout, other logging format.
```

### Comparing `trrc-0.1.2/README.md` & `trrc-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,37 @@
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [CONFIG_FILE](#config-file)
 * [LOCATIONS](#locations)
 * [OPTIONS](#options)
 * [FAQ](#faq)
-* [CANGELOG](#changelog)
+* [CHANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **ToRRential Card processor**(**trrc**) is a command-line unix-like program to create anki cards using AnkiConnect plugin.(Think a yt-dlp, but this program is for adding cards into Anki.)
 
 I intent to make it as a Unix-like program. Therefore it **leverages a lot of Unix concepts**.
 
-- it **supports a standard input, PIPE, redirection.** Therefore, you can add bulk cards after mangling your cards with your favorite text editors. With the benefit of unix-like program, you can make a convenient script yourself with your favorite text editors like Vim, Emacs, VScode and so on. See [Usage](#usage)
+- It **supports a standard input, PIPE, redirection.** Therefore, you can add bulk cards after mangling your cards with your favorite text editors. With the benefit of unix-like program, you can make a convenient script yourself with your favorite text editors like Vim, Emacs, VScode and so on. See [Usage](#usage)
+
+- It has **shell completions(Zsh, Bash)**.
 
 - It **adds multiple cards at once** using [`--file`](#–file-option) or [PIPE](#pipe) and so on. See [Usage](#usage)
 
 - It also **supports options for ip, port and apikey**. So even some environments you don't want to install Anki, you can add cards if your Anki is running in your home or somewhere, boundlessly.
 
 - It also supports a **rc(config) file** with a alias to reuse options you uses frequently.
 
 - you can **sync Anki** with option `--sync` of **trrc** with or without soon after adding cards.
 
 - It's **user-friendly**. In well-known cases, **trrc** provides solutions. If you
-  mistake deck name, it will print all deck name available. if your field is
+  mistake deck name, it will print all deck name available. If your field is
   wrong, it will print field of the card type used.
 
 ```sh
 # default card type is 'Basic'
 $trrc --field 'fron:bakc:tags' 'What is GPL?	The GNU General Public License is a free, copyleft license for software and other kinds of works.	LICENSE::GPL'
 #### Kinds of failures: 1
 trrc Tip: --field 'Front:Back:Tags'
@@ -78,15 +80,15 @@
 trrc "back\ttestfront\tvim" -F '\t'
 
 # you can set whatever character you want.
 trrc --IFS % '안녕%Hello%Korean'
 trrc -F @ '안녕@Hello@Korean'
 
 # you can choose only part of the fields of the card type.
-# you  can change order of the fields.
+# you can change order of the fields.
 trrc --field 'Arbitrary4thField:Arbitrary2ndFieldName:tags' 'FourthContent\tsecondContent\ttag'
 
 # to send your card to other computer(e.g.: ip is 192.168.1.230, port is 4832).
 trrc --ip 192.168.1.230 --port 4832 --file Korean_English_conversation.txt
 ```
 
 #### # To use '\t' as a tab character in an standard input argument, you need to use '$' in front of the string.
@@ -273,15 +275,15 @@
 ### --file option
 
 #### examplefile.txt
 This is an example which trrc takes. IFS is a tab which is a default IFS.
 
 ```
 Anki	Anki is a free and open-source flashcard program using spaced repetition	anki
-To make  a log message in python, What library Should I use?	logging	python::library
+To make a log message in python, What library Should I use?	logging	python::library
 ```
 * `trrc --file examplefile.txt`
 
 
 ### --read-file-in-a-content
 Let's say you are learning Rust Language.
 Save this statements in a text file called 'rust_hello.txt'
@@ -406,15 +408,16 @@
 
 See [iOS_shortcuts_example](docs/tips/iOS_shortcuts_setting_example/iOS_shortcuts_example.md)
 
 ## Changelog
 
 | Version | Note                     | 
 |:--------|:-------------------------|
-| HEAD    | fix sync option error handle. | 
+| HEAD    | add shell completion. | 
+| 0.1.2    | fix sync option error handle. | 
 | 0.1.1   | init                     | 
 
 ## Contribution
 
 Thank you for letting me know the bug! Please report the bug in [issue tracker](https://github.com/Constantin1489/trrc/issues).
 
 Personally I like this app as a method to add cards and use daily, so I will keep developing it. Because I'm trying to get a job, an update delivery can be slow. But after getting a job, I will learn some good clean code conventions and apply it.
@@ -438,14 +441,17 @@
 - [ ] windows support.
     - py2exe
     - file path (e.g.: default config file)
 - [ ] send media files directly to Anki.
 - [ ] create card from git-diff, git-show
     - option: --mode=git --header 'Optimize logging message\n		'
     - without --header, use git commit message as header.
+- [ ] support markdown, mad type and so on.
+    - --vertical?
+    - Pseudo HEREDOC mode.
 - [ ] get fields of a deck.
     - error handle.
 - [ ] support shell environment variable.
     - prefix: TRRC
     - e.g.: TRRC_deck, TRRC_tag: global tag
 - [ ] new verbose purpose.
     - -v : stdout, other logging format.
```

### Comparing `trrc-0.1.2/docs/trrc.1` & `trrc-0.1.3/docs/trrc.1`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/pyproject.toml` & `trrc-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trrc"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 maintainers = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 license = {file = "LICENSE"}
```

### Comparing `trrc-0.1.2/setup.py` & `trrc-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 setup(
     name = 'trrc',
-    version = '0.1.2',
+    version = '0.1.3',
     description='a command-line program for creating anki card using AnkiConnect API.',
     author='Constantin Hong',
     author_email='hongconstantin@gmail.com',
     url='https://github.com/Constantin1489/trrc',
     maintainer='Constantin Hong',
     maintainer_email='hongconstantin@gmail.com',
     readme = "README.md",
     packages = ['trrc'],
-    data_files = [('share/man/man1', ['docs/trrc.1'])],
+    data_files = [
+        ('share/man/man1', ['docs/trrc.1']),
+        ('share/bash-completion/completions', ['scripts/bash/trrc']),
+        ('share/zsh/site-functions', ['scripts/zsh/_trrc'])
+        ],
     python_requires='>=3.9',
     install_requires=[
         "requests",
         "tomlkit",
         "tomli_w",
         ],
     project_urls = {
```

### Comparing `trrc-0.1.2/tests/test_cardcontentsHandle.py` & `trrc-0.1.3/tests/test_cardcontentsHandle.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/tests/test_classAnkiConnect.py` & `trrc-0.1.3/tests/test_classAnkiConnect.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/tests/test_create_parser.py` & `trrc-0.1.3/tests/test_create_parser.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/tests/test_options.py` & `trrc-0.1.3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/tests/test_pipe_redirection.py` & `trrc-0.1.3/tests/test_pipe_redirection.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/tests/test_regexhtml.py` & `trrc-0.1.3/tests/test_regexhtml.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/tests/test_utils.py` & `trrc-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/trrc/config_opts.py` & `trrc-0.1.3/trrc/config_opts.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/trrc/create_parser.py` & `trrc-0.1.3/trrc/create_parser.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/trrc/parser_opts.py` & `trrc-0.1.3/trrc/parser_opts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """module for parser using argparse"""
 import argparse
 import logging
 
-VERSION_MESSAGE = """trrc - ToRRential Card processor 0.1.2
+VERSION_MESSAGE = """trrc - ToRRential Card processor 0.1.3
 Copyright (C) 2023  Constantin Hong
 License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>.
 This is free software: you are free to change and redistribute it.
 There is NO WARRANTY, to the extent permitted by law."""
 
 DESCRIPTION = "A command-line unix-like program to create Anki cards using AnkiConnect API."
 
@@ -14,16 +14,15 @@
 "'cloze'. If user set --field option, then the default won't work. Even a string " \
 "contains cloze, the program will process as a field unless user set " \
 "--cloze-type"
 
 CARD_CONTENT_HELP = "A quoted string divided by IFS. The default IFS is a tab character. " \
         "Instead of a string, it can also take a file consists of strings " \
         "without '--FILE' option. A [CARD_CONTENT] of '-' stands for standa" \
-        "rd input. <<EOF in [CARD_CONTENT] will trigger Pseudo HEREDOC " \
-        "mode. See #pseudo-heredoc-mode in README."
+        "rd input."
 
 def create_parser():
     """
     create parser
     """
 
     parser = argparse.ArgumentParser(
```

### Comparing `trrc-0.1.2/trrc/utils.py` & `trrc-0.1.3/trrc/utils.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.2/trrc.egg-info/PKG-INFO` & `trrc-0.1.3/trrc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trrc
-Version: 0.1.2
+Version: 0.1.3
 Summary: a command-line program for creating anki card using AnkiConnect API.
 Home-page: https://github.com/Constantin1489/trrc
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -709,35 +709,37 @@
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [CONFIG_FILE](#config-file)
 * [LOCATIONS](#locations)
 * [OPTIONS](#options)
 * [FAQ](#faq)
-* [CANGELOG](#changelog)
+* [CHANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **ToRRential Card processor**(**trrc**) is a command-line unix-like program to create anki cards using AnkiConnect plugin.(Think a yt-dlp, but this program is for adding cards into Anki.)
 
 I intent to make it as a Unix-like program. Therefore it **leverages a lot of Unix concepts**.
 
-- it **supports a standard input, PIPE, redirection.** Therefore, you can add bulk cards after mangling your cards with your favorite text editors. With the benefit of unix-like program, you can make a convenient script yourself with your favorite text editors like Vim, Emacs, VScode and so on. See [Usage](#usage)
+- It **supports a standard input, PIPE, redirection.** Therefore, you can add bulk cards after mangling your cards with your favorite text editors. With the benefit of unix-like program, you can make a convenient script yourself with your favorite text editors like Vim, Emacs, VScode and so on. See [Usage](#usage)
+
+- It has **shell completions(Zsh, Bash)**.
 
 - It **adds multiple cards at once** using [`--file`](#–file-option) or [PIPE](#pipe) and so on. See [Usage](#usage)
 
 - It also **supports options for ip, port and apikey**. So even some environments you don't want to install Anki, you can add cards if your Anki is running in your home or somewhere, boundlessly.
 
 - It also supports a **rc(config) file** with a alias to reuse options you uses frequently.
 
 - you can **sync Anki** with option `--sync` of **trrc** with or without soon after adding cards.
 
 - It's **user-friendly**. In well-known cases, **trrc** provides solutions. If you
-  mistake deck name, it will print all deck name available. if your field is
+  mistake deck name, it will print all deck name available. If your field is
   wrong, it will print field of the card type used.
 
 ```sh
 # default card type is 'Basic'
 $trrc --field 'fron:bakc:tags' 'What is GPL?	The GNU General Public License is a free, copyleft license for software and other kinds of works.	LICENSE::GPL'
 #### Kinds of failures: 1
 trrc Tip: --field 'Front:Back:Tags'
@@ -782,15 +784,15 @@
 trrc "back\ttestfront\tvim" -F '\t'
 
 # you can set whatever character you want.
 trrc --IFS % '안녕%Hello%Korean'
 trrc -F @ '안녕@Hello@Korean'
 
 # you can choose only part of the fields of the card type.
-# you  can change order of the fields.
+# you can change order of the fields.
 trrc --field 'Arbitrary4thField:Arbitrary2ndFieldName:tags' 'FourthContent\tsecondContent\ttag'
 
 # to send your card to other computer(e.g.: ip is 192.168.1.230, port is 4832).
 trrc --ip 192.168.1.230 --port 4832 --file Korean_English_conversation.txt
 ```
 
 #### # To use '\t' as a tab character in an standard input argument, you need to use '$' in front of the string.
@@ -977,15 +979,15 @@
 ### --file option
 
 #### examplefile.txt
 This is an example which trrc takes. IFS is a tab which is a default IFS.
 
 ```
 Anki	Anki is a free and open-source flashcard program using spaced repetition	anki
-To make  a log message in python, What library Should I use?	logging	python::library
+To make a log message in python, What library Should I use?	logging	python::library
 ```
 * `trrc --file examplefile.txt`
 
 
 ### --read-file-in-a-content
 Let's say you are learning Rust Language.
 Save this statements in a text file called 'rust_hello.txt'
@@ -1110,15 +1112,16 @@
 
 See [iOS_shortcuts_example](docs/tips/iOS_shortcuts_setting_example/iOS_shortcuts_example.md)
 
 ## Changelog
 
 | Version | Note                     | 
 |:--------|:-------------------------|
-| HEAD    | fix sync option error handle. | 
+| HEAD    | add shell completion. | 
+| 0.1.2    | fix sync option error handle. | 
 | 0.1.1   | init                     | 
 
 ## Contribution
 
 Thank you for letting me know the bug! Please report the bug in [issue tracker](https://github.com/Constantin1489/trrc/issues).
 
 Personally I like this app as a method to add cards and use daily, so I will keep developing it. Because I'm trying to get a job, an update delivery can be slow. But after getting a job, I will learn some good clean code conventions and apply it.
@@ -1142,14 +1145,17 @@
 - [ ] windows support.
     - py2exe
     - file path (e.g.: default config file)
 - [ ] send media files directly to Anki.
 - [ ] create card from git-diff, git-show
     - option: --mode=git --header 'Optimize logging message\n		'
     - without --header, use git commit message as header.
+- [ ] support markdown, mad type and so on.
+    - --vertical?
+    - Pseudo HEREDOC mode.
 - [ ] get fields of a deck.
     - error handle.
 - [ ] support shell environment variable.
     - prefix: TRRC
     - e.g.: TRRC_deck, TRRC_tag: global tag
 - [ ] new verbose purpose.
     - -v : stdout, other logging format.
```

### Comparing `trrc-0.1.2/trrc.egg-info/SOURCES.txt` & `trrc-0.1.3/trrc.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 docs/trrc.1
+scripts/bash/trrc
+scripts/zsh/_trrc
 tests/test_cardcontentsHandle.py
 tests/test_classAnkiConnect.py
 tests/test_create_parser.py
 tests/test_options.py
 tests/test_pipe_redirection.py
 tests/test_regexhtml.py
 tests/test_utils.py
 trrc/__init__.py
 trrc/__main__.py
 trrc/config_opts.py
 trrc/create_parser.py
 trrc/parser_opts.py
+trrc/some.py
 trrc/utils.py
 trrc.egg-info/PKG-INFO
 trrc.egg-info/SOURCES.txt
 trrc.egg-info/dependency_links.txt
 trrc.egg-info/entry_points.txt
 trrc.egg-info/requires.txt
 trrc.egg-info/top_level.txt
```

