# Comparing `tmp/Pytdbot-0.8.4.dev1.tar.gz` & `tmp/Pytdbot-0.8.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytdbot-0.8.4.dev1.tar", last modified: Tue Jun 13 14:39:33 2023, max compression
+gzip compressed data, was "Pytdbot-0.8.4.dev2.tar", last modified: Sat Jun 17 15:10:04 2023, max compression
```

## Comparing `Pytdbot-0.8.4.dev1.tar` & `Pytdbot-0.8.4.dev2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.500946 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 14:39:33.000000 Pytdbot-0.8.4.dev1/Pytdbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42708 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/generate_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   146663 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/handlers/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/methods/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57920 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/methods/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)   444864 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/methods/tdlibfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)  1248427 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/td_api.json
--rw-r--r--   0 runner    (1001) docker     (123)   585705 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/td_api.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/tdjson/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/tdjson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/tdjson/tdjson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.504946 Pytdbot-0.8.4.dev1/pytdbot/types/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/inline_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/remove_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/buttons/show_keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/result/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/result/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/types/update/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/update/chatActions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60488 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/types/update/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/pytdbot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/pytdbot/utils/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:39:33.508946 Pytdbot-0.8.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 14:39:31.000000 Pytdbot-0.8.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.530447 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.530447 Pytdbot-0.8.4.dev2/pytdbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42708 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.530447 Pytdbot-0.8.4.dev2/pytdbot/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/generate_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146553 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57920 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/methods/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   444864 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/methods/tdlibfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1248427 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/td_api.json
+-rw-r--r--   0 runner    (1001) docker     (123)   585705 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/td_api.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/tdjson/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/tdjson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/tdjson/tdjson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/inline_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/remove_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/show_keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/result/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/result/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/update/chatActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60488 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/pytdbot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/utils/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/setup.py
```

### Comparing `Pytdbot-0.8.4.dev1/LICENSE` & `Pytdbot-0.8.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/PKG-INFO` & `Pytdbot-0.8.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytdbot
-Version: 0.8.4.dev1
+Version: 0.8.4.dev2
 Summary: Easy-to-use asynchronous TDLib wrapper for Python.
 Home-page: https://github.com/pytdbot/client
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/pytdbot/client
 Project-URL: Tracker, https://github.com/pytdbot/client/issues
```

### Comparing `Pytdbot-0.8.4.dev1/Pytdbot.egg-info/PKG-INFO` & `Pytdbot-0.8.4.dev2/Pytdbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytdbot
-Version: 0.8.4.dev1
+Version: 0.8.4.dev2
 Summary: Easy-to-use asynchronous TDLib wrapper for Python.
 Home-page: https://github.com/pytdbot/client
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/pytdbot/client
 Project-URL: Tracker, https://github.com/pytdbot/client/issues
```

### Comparing `Pytdbot-0.8.4.dev1/Pytdbot.egg-info/SOURCES.txt` & `Pytdbot-0.8.4.dev2/Pytdbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/README.md` & `Pytdbot-0.8.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/client.py` & `Pytdbot-0.8.4.dev2/pytdbot/client.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/filters.py` & `Pytdbot-0.8.4.dev2/pytdbot/filters.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/generate_files.py` & `Pytdbot-0.8.4.dev2/pytdbot/generate_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,154 +1,145 @@
-if __name__ != "__main__":
-    exit(1)
-
-from json import loads
-import utils
-
+if __name__ == "__main__":
+    from json import loads
+    import utils
 
-with open("td_api.json") as f:
-    data = loads(f.read())
+    with open("td_api.json") as f:
+        data = loads(f.read())
 
+    def getP(params: dict):
+        nullable = []
+        non = []
+        for k, v in params.items():
+            name, _type = k, v["type"]
+            param = ""
+
+            if _type == "Bool":
+                param = f"{name}: bool"
+            elif _type.startswith("int"):
+                param = f"{name}: int"
+            elif _type == "bytes":
+                param = f"{name}: bytes"
+            elif _type.startswith("vector"):
+                param = f"{name}: list"
+            elif _type == "string":
+                param = f"{name}: str"
+            elif _type == "double":
+                param = f"{name}: float"
+            else:
+                param = f"{name}: dict"
 
-def getP(params: dict):
-    nullable = []
-    non = []
-    for k, v in params.items():
-        name, _type = k, v["type"]
-        param = ""
+            if v["is_optional"]:
+                param += " = None"
+                nullable.append(param)
+            else:
+                non.append(param)
+        if non or nullable:
+            return ", ".join(non + nullable)
 
+    def getType(_type):
         if _type == "Bool":
-            param = f"{name}: bool"
+            return "bool"
         elif _type.startswith("int"):
-            param = f"{name}: int"
+            return "int"
         elif _type == "bytes":
-            param = f"{name}: bytes"
+            return "bytes"
         elif _type.startswith("vector"):
-            param = f"{name}: list"
+            return "list"
         elif _type == "string":
-            param = f"{name}: str"
+            return "str"
         elif _type == "double":
-            param = f"{name}: float"
-        else:
-            param = f"{name}: dict"
-
-        if v["is_optional"]:
-            param += " = None"
-            nullable.append(param)
+            return "float"
         else:
-            non.append(param)
-    if non or nullable:
-        return ", ".join(non + nullable)
-
-
-def getType(_type):
-    if _type == "Bool":
-        return "bool"
-    elif _type.startswith("int"):
-        return "int"
-    elif _type == "bytes":
-        return "bytes"
-    elif _type.startswith("vector"):
-        return "list"
-    elif _type == "string":
-        return "str"
-    elif _type == "double":
-        return "float"
-    else:
-        return _type
-
-
-updates_dec = """    def on_{update_name}(
-    self: "pytdbot.Client" = None,
-    filters: "pytdbot.filters.Filter" = None,
-    position: int = None,
-) -> Callable:
-        \"\"\"{description}
-
-        Args:
-            filters (:class:`pytdbot.filters.Filter`, *optional*):
-                An update filter
-
-            position (``int``, *optional``):
-                The function position in handlers list. Defaults to ``None`` (append)
-
-        Raises:
-            :py:class:`TypeError`
-        \"\"\"
+            return _type
 
-        def decorator(func: Callable) -> Callable:
-            if hasattr(func, "_handler"):
-                return func
-            elif isinstance(self, pytdbot.Client):
-                if iscoroutinefunction(func):
-                    self.add_handler("{update_name}", func, filters, position)
+    updates_dec = """    def on_{update_name}(
+        self: "pytdbot.Client" = None,
+        filters: "pytdbot.filters.Filter" = None,
+        position: int = None,
+    ) -> Callable:
+            \"\"\"{description}
+
+            Args:
+                filters (:class:`pytdbot.filters.Filter`, *optional*):
+                    An update filter
+
+                position (``int``, *optional*):
+                    The function position in handlers list. Defaults to ``None`` (append)
+
+            Raises:
+                :py:class:`TypeError`
+            \"\"\"
+
+            def decorator(func: Callable) -> Callable:
+                if hasattr(func, "_handler"):
+                    return func
+                elif isinstance(self, pytdbot.Client):
+                    if iscoroutinefunction(func):
+                        self.add_handler("{update_name}", func, filters, position)
+                    else:
+                        raise TypeError("Handler must be async")
+                elif isinstance(self, pytdbot.filters.Filter):
+                    func._handler = Handler(func, "{update_name}", self, position)
                 else:
-                    raise TypeError("Handler must be async")
-            elif isinstance(self, pytdbot.filters.Filter):
-                func._handler = Handler(func, "{update_name}", self, position)
-            else:
-                func._handler = Handler(func, "{update_name}", filters, position)
-            return func
-
-        return decorator
+                    func._handler = Handler(func, "{update_name}", filters, position)
+                return func
 
-"""
+            return decorator
 
+    """
 
-def updates():
-    with open("handlers/updates.py", "w") as f:
-        f.write(
-            'import pytdbot\n\nfrom .handler import Handler\nfrom typing import Callable\nfrom asyncio import iscoroutinefunction\nfrom logging import getLogger\n\nlogger = getLogger(__name__)\n\n\nclass Updates:\n    """Auto generated TDLib updates"""\n\n'
-        )
-        for k, v in data["updates"].items():
+    def updates():
+        with open("handlers/updates.py", "w") as f:
             f.write(
-                updates_dec.format(
-                    update_name=k, description=utils.escape_markdown(v["description"])
-                )
+                'import pytdbot\n\nfrom .handler import Handler\nfrom typing import Callable\nfrom asyncio import iscoroutinefunction\nfrom logging import getLogger\n\nlogger = getLogger(__name__)\n\n\nclass Updates:\n    """Auto generated TDLib updates"""\n\n'
             )
-
-
-def functions():
-    with open("methods/tdlibfunctions.py", "w") as f:
-        f.write(
-            'from ..types import Result\n\nclass TDLibFunctions:\n    """Auto generated TDLib functions"""\n\n'
-        )
-        for k, v in data["functions"].items():
-            # if k.startswith("test"):
-            #     continue
-            f.write(f"    async def {k}(self")
-            if p := getP(v["args"]):
-                f.write(f",{p}" + ") -> Result:\n")
-            else:
-                f.write(") -> Result:\n")
-
-            f.write(f'        """{utils.escape_markdown(v["description"])}\n\n')
-
-            if v["args"]:
-                f.write(f"        Args:\n")
-                params = dict(
-                    sorted(v["args"].items(), key=lambda x: x[1]["is_optional"])
+            for k, v in data["updates"].items():
+                f.write(
+                    updates_dec.format(
+                        update_name=k,
+                        description=utils.escape_markdown(v["description"]),
+                    )
                 )
 
-                for _k, _v in params.items():
-                    if not _v["is_optional"]:
-                        f.write(
-                            f"            {_k} (``{getType(_v['type'])}``):\n                {utils.escape_markdown(_v['description'])}\n\n"
-                        )
-                    else:
-                        f.write(
-                            f"            {_k} (``{getType(_v['type'])}``, *optional*):\n                {utils.escape_markdown(_v['description'])}\n\n"
-                        )
+    def functions():
+        with open("methods/tdlibfunctions.py", "w") as f:
             f.write(
-                '\n        Returns:\n            :class:`~pytdbot.types.Result` (``{}``)\n        """\n\n'.format(
-                    v["type"]
-                )
+                'from ..types import Result\n\nclass TDLibFunctions:\n    """Auto generated TDLib functions"""\n\n'
             )
-            f.write(f"        data = {{'@type': '{k}',")
-            for k in v["args"]:
-                f.write(f" '{k}': {k},")
-            f.write("}\n\n        return await self.invoke(data)\n\n")
+            for k, v in data["functions"].items():
+                # if k.startswith("test"):
+                #     continue
+                f.write(f"    async def {k}(self")
+                if p := getP(v["args"]):
+                    f.write(f",{p}" + ") -> Result:\n")
+                else:
+                    f.write(") -> Result:\n")
 
+                f.write(f'        """{utils.escape_markdown(v["description"])}\n\n')
+
+                if v["args"]:
+                    f.write(f"        Args:\n")
+                    params = dict(
+                        sorted(v["args"].items(), key=lambda x: x[1]["is_optional"])
+                    )
+
+                    for _k, _v in params.items():
+                        if not _v["is_optional"]:
+                            f.write(
+                                f"            {_k} (``{getType(_v['type'])}``):\n                {utils.escape_markdown(_v['description'])}\n\n"
+                            )
+                        else:
+                            f.write(
+                                f"            {_k} (``{getType(_v['type'])}``, *optional*):\n                {utils.escape_markdown(_v['description'])}\n\n"
+                            )
+                f.write(
+                    '\n        Returns:\n            :class:`~pytdbot.types.Result` (``{}``)\n        """\n\n'.format(
+                        v["type"]
+                    )
+                )
+                f.write(f"        data = {{'@type': '{k}',")
+                for k in v["args"]:
+                    f.write(f" '{k}': {k},")
+                f.write("}\n\n        return await self.invoke(data)\n\n")
 
-if __name__ == "__main__":
     updates()
     functions()
```

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/generate_json.py` & `Pytdbot-0.8.4.dev2/pytdbot/generate_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 from json import dumps
 from sys import argv
 from re import compile
 from pathlib import Path
 
-if len(argv) != 3:
-    print("Usage: generate_json.py <TDLib_version> <Last_TDLib_commit_hash>")
-    exit(1)
-
-data = {
-    "name": "Auto-generated JSON TDLib API for Pytdbot ~ https://github.com/pytdbot/client",
-    "version": argv[1],
-    "commit_hash": argv[2],
-    "classes": {},
-    "types": {},
-    "updates": {},
-    "functions": {},
-}
-params = {}
-start = False
-is_functions = False
-description = ""
-class_regex = compile(r"//@class\s(?P<name>.*)\s@description\s(?P<description>.*)")
-description_regex = compile(r"//@description\s(?P<description>.*)$")
-parameter_regex = compile(r"@(.*?)\s+([^@]+)")
-end_param_regex = compile(r"(?P<name>\w+):(?P<type>[<\w>]+)")
-end_regex = compile(r"^(?P<name>.*?)\s(?P<params>.*)=\s(?P<type>\w+);$")
-tl = Path("td_api.tl").read_text().replace("\n//-", " ")
-
-
-def is_optional(d):
-    return (
-        "; may be null" in d
-        or "; pass null" in d
-        or "; may be empty" in d
-        or "If non-empty," in d
-    )
-
-
-for line in tl.split("\n"):
-
-    if "--functions--" in line:
-        is_functions = True
-        continue
-
-    if line.startswith("//"):
-        start = True
-
-    if line != "" and start:
-
-        if _class := class_regex.match(line):
-            data["classes"][_class.group("name").strip()] = _class.group(
-                "description"
-            ).strip()
-        elif _param := parameter_regex.findall(line):
-            for name, _description in _param:
-                if name.strip() == "description":
-                    description = _description.strip()
-                else:
-                    params[name.replace("param_", "").strip()] = _description.strip()
-        elif _end := end_regex.match(line):
-            _data = {
-                "description": description,
-                "args": {},
-                "type": _end.group("type").strip(),
-            }
-
-            for keyv in end_param_regex.finditer(_end.group("params")):
-                k, v = keyv.group("name").strip(), keyv.group("type").strip()
-                _data["args"][k] = {
-                    "description": params[k],
-                    "is_optional": is_optional(params[k]),
-                    "type": v,
+if __name__ == "__main__":
+    if len(argv) != 3:
+        print("Usage: generate_json.py <TDLib_version> <Last_TDLib_commit_hash>")
+        exit(1)
+
+    data = {
+        "name": "Auto-generated JSON TDLib API for Pytdbot ~ https://github.com/pytdbot/client",
+        "version": argv[1],
+        "commit_hash": argv[2],
+        "classes": {},
+        "types": {},
+        "updates": {},
+        "functions": {},
+    }
+    params = {}
+    start = False
+    is_functions = False
+    description = ""
+    class_regex = compile(r"//@class\s(?P<name>.*)\s@description\s(?P<description>.*)")
+    description_regex = compile(r"//@description\s(?P<description>.*)$")
+    parameter_regex = compile(r"@(.*?)\s+([^@]+)")
+    end_param_regex = compile(r"(?P<name>\w+):(?P<type>[<\w>]+)")
+    end_regex = compile(r"^(?P<name>.*?)\s(?P<params>.*)=\s(?P<type>\w+);$")
+    tl = Path("td_api.tl").read_text().replace("\n//-", " ")
+
+    def is_optional(d):
+        return (
+            "; may be null" in d
+            or "; pass null" in d
+            or "; may be empty" in d
+            or "If non-empty," in d
+        )
+
+    for line in tl.split("\n"):
+        if "--functions--" in line:
+            is_functions = True
+            continue
+
+        if line.startswith("//"):
+            start = True
+
+        if line != "" and start:
+            if _class := class_regex.match(line):
+                data["classes"][_class.group("name").strip()] = _class.group(
+                    "description"
+                ).strip()
+            elif _param := parameter_regex.findall(line):
+                for name, _description in _param:
+                    if name.strip() == "description":
+                        description = _description.strip()
+                    else:
+                        params[
+                            name.replace("param_", "").strip()
+                        ] = _description.strip()
+            elif _end := end_regex.match(line):
+                _data = {
+                    "description": description,
+                    "args": {},
+                    "type": _end.group("type").strip(),
                 }
-            if is_functions:
-                data["functions"][_end.group("name").strip()] = _data
-            elif _end.group("name").strip().startswith("update"):
-                data["updates"][_end.group("name").strip()] = _data
-            else:
-                data["types"][_end.group("name").strip()] = _data
-            params = {}
-            description = ""
-
-with open("td_api.json", "w") as f:
-    f.write(dumps(data, indent=4))
-    print(
-        "Classes: {}\nTypes: {}\nFunctions: {}\nUpdates: {}".format(
-            len(data["classes"]),
-            len(data["types"]),
-            len(data["functions"]),
-            len(data["updates"]),
+
+                for keyv in end_param_regex.finditer(_end.group("params")):
+                    k, v = keyv.group("name").strip(), keyv.group("type").strip()
+                    _data["args"][k] = {
+                        "description": params[k],
+                        "is_optional": is_optional(params[k]),
+                        "type": v,
+                    }
+                if is_functions:
+                    data["functions"][_end.group("name").strip()] = _data
+                elif _end.group("name").strip().startswith("update"):
+                    data["updates"][_end.group("name").strip()] = _data
+                else:
+                    data["types"][_end.group("name").strip()] = _data
+                params = {}
+                description = ""
+
+    with open("td_api.json", "w") as f:
+        f.write(dumps(data, indent=4))
+        print(
+            "Classes: {}\nTypes: {}\nFunctions: {}\nUpdates: {}".format(
+                len(data["classes"]),
+                len(data["types"]),
+                len(data["functions"]),
+                len(data["updates"]),
+            )
         )
-    )
```

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/handlers/decorators.py` & `Pytdbot-0.8.4.dev2/pytdbot/handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/handlers/handler.py` & `Pytdbot-0.8.4.dev2/pytdbot/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/handlers/updates.py` & `Pytdbot-0.8.4.dev2/pytdbot/handlers/updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ) -> Callable:
         """The user authorization state has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -58,15 +58,15 @@
     ) -> Callable:
         """A new message was received; can also be an outgoing message
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -92,15 +92,15 @@
     ) -> Callable:
         """A request to send a message has reached the Telegram server\. This doesn't mean that the message will be sent successfully or even that the send message request will be processed\. This update will be sent only if the option "use\_quick\_ack" is set to true\. This update may be sent multiple times for the same message
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -132,15 +132,15 @@
     ) -> Callable:
         """A message has been successfully sent
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -172,15 +172,15 @@
     ) -> Callable:
         """A message failed to send\. Be aware that some messages being sent can be irrecoverably deleted, in which case updateDeleteMessages will be received instead of this update
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -208,15 +208,15 @@
     ) -> Callable:
         """The message content has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -242,15 +242,15 @@
     ) -> Callable:
         """A message was edited\. Changes in the message content will come in a separate updateMessageContent
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -276,15 +276,15 @@
     ) -> Callable:
         """The message pinned state was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -312,15 +312,15 @@
     ) -> Callable:
         """The information about interactions with a message has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -352,15 +352,15 @@
     ) -> Callable:
         """The message content was opened\. Updates voice note messages to "listened", video note messages to "viewed" and starts the self\-destruct timer
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -392,15 +392,15 @@
     ) -> Callable:
         """A message with an unread mention was read
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -432,15 +432,15 @@
     ) -> Callable:
         """The list of unread reactions added to a message was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -472,15 +472,15 @@
     ) -> Callable:
         """A message with a live location was viewed\. When the update is received, the application is supposed to update the live location
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -512,15 +512,15 @@
     ) -> Callable:
         """A new chat has been loaded/created\. This update is guaranteed to come before the chat identifier is returned to the application\. The chat field changes will be reported through separate updates
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -546,15 +546,15 @@
     ) -> Callable:
         """The title of a chat was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -580,15 +580,15 @@
     ) -> Callable:
         """A chat photo was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -614,15 +614,15 @@
     ) -> Callable:
         """Chat permissions was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -650,15 +650,15 @@
     ) -> Callable:
         """The last message of a chat was changed\. If last\_message is null, then the last message in the chat became unknown\. Some new unknown messages might be added to the chat in this case
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -686,15 +686,15 @@
     ) -> Callable:
         """The position of a chat in a chat list has changed\. An updateChatLastMessage or updateChatDraftMessage update might be sent instead of the update
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -720,15 +720,15 @@
     ) -> Callable:
         """Incoming messages were read or the number of unread messages has been changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -754,15 +754,15 @@
     ) -> Callable:
         """Outgoing messages were read
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -788,15 +788,15 @@
     ) -> Callable:
         """The chat action bar was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -822,15 +822,15 @@
     ) -> Callable:
         """The chat available reactions were changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -862,15 +862,15 @@
     ) -> Callable:
         """A chat draft has changed\. Be aware that the update may come in the currently opened chat but with old content of the draft\. If the user has changed the content of the draft, this update mustn't be applied
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -898,15 +898,15 @@
     ) -> Callable:
         """The message sender that is selected to send messages in a chat has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -934,15 +934,15 @@
     ) -> Callable:
         """The message auto\-delete or self\-destruct timer setting for a chat was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -974,15 +974,15 @@
     ) -> Callable:
         """Notification settings for a chat were changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1014,15 +1014,15 @@
     ) -> Callable:
         """The chat pending join requests were changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1054,15 +1054,15 @@
     ) -> Callable:
         """The default chat reply markup was changed\. Can occur because new messages with reply markup were received or because an old reply markup was hidden by the user
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1090,15 +1090,15 @@
     ) -> Callable:
         """The chat background was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1124,15 +1124,15 @@
     ) -> Callable:
         """The chat theme was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1158,15 +1158,15 @@
     ) -> Callable:
         """The chat unread\_mention\_count has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1198,15 +1198,15 @@
     ) -> Callable:
         """The chat unread\_reaction\_count has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1238,15 +1238,15 @@
     ) -> Callable:
         """A chat video chat state has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1272,15 +1272,15 @@
     ) -> Callable:
         """The value of the default disable\_notification parameter, used when a message is sent to the chat, was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1312,15 +1312,15 @@
     ) -> Callable:
         """A chat content was allowed or restricted for saving
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1352,15 +1352,15 @@
     ) -> Callable:
         """Translation of chat messages was enabled or disabled
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1392,15 +1392,15 @@
     ) -> Callable:
         """A chat was marked as unread or was read
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1432,15 +1432,15 @@
     ) -> Callable:
         """A chat was blocked or unblocked
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1466,15 +1466,15 @@
     ) -> Callable:
         """A chat's has\_scheduled\_messages field has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1506,15 +1506,15 @@
     ) -> Callable:
         """The list of chat folders or a chat folder has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1540,15 +1540,15 @@
     ) -> Callable:
         """The number of online group members has changed\. This update with non\-zero number of online group members is sent only for currently opened chats\. There is no guarantee that it will be sent just after the number of online users has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1580,15 +1580,15 @@
     ) -> Callable:
         """Basic information about a topic in a forum chat was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1614,15 +1614,15 @@
     ) -> Callable:
         """Notification settings for some type of chats were updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1654,15 +1654,15 @@
     ) -> Callable:
         """A notification was changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1688,15 +1688,15 @@
     ) -> Callable:
         """A list of active notifications in a notification group has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1724,15 +1724,15 @@
     ) -> Callable:
         """Contains active notifications that was shown on previous application launches\. This update is sent only if the message database is used\. In that case it comes once before any updateNotification and updateNotificationGroup update
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1764,15 +1764,15 @@
     ) -> Callable:
         """Describes whether there are some pending notification updates\. Can be used to prevent application from killing, while there are some pending notifications
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1804,15 +1804,15 @@
     ) -> Callable:
         """Some messages were deleted
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1838,15 +1838,15 @@
     ) -> Callable:
         """A message sender activity in the chat has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1872,15 +1872,15 @@
     ) -> Callable:
         """The user went online or offline
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1906,15 +1906,15 @@
     ) -> Callable:
         """Some data of a user has changed\. This update is guaranteed to come before the user identifier is returned to the application
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1940,15 +1940,15 @@
     ) -> Callable:
         """Some data of a basic group has changed\. This update is guaranteed to come before the basic group identifier is returned to the application
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -1974,15 +1974,15 @@
     ) -> Callable:
         """Some data of a supergroup or a channel has changed\. This update is guaranteed to come before the supergroup identifier is returned to the application
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2008,15 +2008,15 @@
     ) -> Callable:
         """Some data of a secret chat has changed\. This update is guaranteed to come before the secret chat identifier is returned to the application
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2042,15 +2042,15 @@
     ) -> Callable:
         """Some data in userFullInfo has been changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2076,15 +2076,15 @@
     ) -> Callable:
         """Some data in basicGroupFullInfo has been changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2116,15 +2116,15 @@
     ) -> Callable:
         """Some data in supergroupFullInfo has been changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2156,15 +2156,15 @@
     ) -> Callable:
         """A service notification from the server was received\. Upon receiving this the application must show a popup with the content of the notification
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2196,15 +2196,15 @@
     ) -> Callable:
         """Information about a file was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2230,15 +2230,15 @@
     ) -> Callable:
         """The file generation process needs to be started by the application
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2270,15 +2270,15 @@
     ) -> Callable:
         """File generation is no longer needed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2310,15 +2310,15 @@
     ) -> Callable:
         """The state of the file download list has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2344,15 +2344,15 @@
     ) -> Callable:
         """A file was added to the file download list\. This update is sent only after file download list is loaded for the first time
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2384,15 +2384,15 @@
     ) -> Callable:
         """A file download was changed\. This update is sent only after file download list is loaded for the first time
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2418,15 +2418,15 @@
     ) -> Callable:
         """A file was removed from the file download list\. This update is sent only after file download list is loaded for the first time
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2458,15 +2458,15 @@
     ) -> Callable:
         """New call was created or information about a call was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2492,15 +2492,15 @@
     ) -> Callable:
         """Information about a group call was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2526,15 +2526,15 @@
     ) -> Callable:
         """Information about a group call participant was changed\. The updates are sent only after the group call is received through getGroupCall and only if the call is joined or being joined
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2566,15 +2566,15 @@
     ) -> Callable:
         """New call signaling data arrived
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2606,15 +2606,15 @@
     ) -> Callable:
         """Some privacy setting rules have been changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2646,15 +2646,15 @@
     ) -> Callable:
         """Number of unread messages in a chat list has changed\. This update is sent only if the message database is used
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2686,15 +2686,15 @@
     ) -> Callable:
         """Number of unread chats, i\.e\. with unread messages or marked as unread, has changed\. This update is sent only if the message database is used
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2722,15 +2722,15 @@
     ) -> Callable:
         """An option changed its value
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2756,15 +2756,15 @@
     ) -> Callable:
         """A sticker set has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2790,15 +2790,15 @@
     ) -> Callable:
         """The list of installed sticker sets was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2830,15 +2830,15 @@
     ) -> Callable:
         """The list of trending sticker sets was updated or some of them were viewed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2870,15 +2870,15 @@
     ) -> Callable:
         """The list of recently used stickers was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2904,15 +2904,15 @@
     ) -> Callable:
         """The list of favorite stickers was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2940,15 +2940,15 @@
     ) -> Callable:
         """The list of saved animations was updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -2976,15 +2976,15 @@
     ) -> Callable:
         """The list of saved notifications sounds was updated\. This update may not be sent until information about a notification sound was requested for the first time
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3016,15 +3016,15 @@
     ) -> Callable:
         """The selected background has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3056,15 +3056,15 @@
     ) -> Callable:
         """The list of available chat themes has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3090,15 +3090,15 @@
     ) -> Callable:
         """Some language pack strings have been updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3130,15 +3130,15 @@
     ) -> Callable:
         """The connection state has changed\. This update must be used only to show a human\-readable description of the connection state
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3166,15 +3166,15 @@
     ) -> Callable:
         """New terms of service must be accepted by the user\. If the terms of service are declined, then the deleteAccount method must be called with the reason "Decline ToS update"
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3200,15 +3200,15 @@
     ) -> Callable:
         """The list of users nearby has changed\. The update is guaranteed to be sent only 60 seconds after a successful searchChatsNearby request
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3234,15 +3234,15 @@
     ) -> Callable:
         """The list of bots added to attachment menu has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3274,15 +3274,15 @@
     ) -> Callable:
         """A message was sent by an opened Web App, so the Web App needs to be closed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3310,15 +3310,15 @@
     ) -> Callable:
         """The list of active emoji reactions has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3350,15 +3350,15 @@
     ) -> Callable:
         """The type of default reaction has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3390,15 +3390,15 @@
     ) -> Callable:
         """The list of supported dice emojis has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3424,15 +3424,15 @@
     ) -> Callable:
         """Some animated emoji message was clicked and a big animated sticker must be played if the message is visible on the screen\. chatActionWatchingAnimations with the text of the message needs to be sent if the sticker is played
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3464,15 +3464,15 @@
     ) -> Callable:
         """The parameters of animation search through getOption\("animation\_search\_bot\_username"\) bot has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3504,15 +3504,15 @@
     ) -> Callable:
         """The list of suggested to the user actions has changed
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3540,15 +3540,15 @@
     ) -> Callable:
         """Adding users to a chat has failed because of their privacy settings\. An invite link can be shared with the users if appropriate
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3580,15 +3580,15 @@
     ) -> Callable:
         """Autosave settings for some type of chats were updated
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3616,15 +3616,15 @@
     ) -> Callable:
         """A new incoming inline query; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3650,15 +3650,15 @@
     ) -> Callable:
         """The user has chosen a result of an inline query; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3690,15 +3690,15 @@
     ) -> Callable:
         """A new incoming callback query; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3726,15 +3726,15 @@
     ) -> Callable:
         """A new incoming callback query from a message sent via a bot; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3766,15 +3766,15 @@
     ) -> Callable:
         """A new incoming shipping query; for bots only\. Only for invoices with flexible price
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3802,15 +3802,15 @@
     ) -> Callable:
         """A new incoming pre\-checkout query; for bots only\. Contains full information about a checkout
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3842,15 +3842,15 @@
     ) -> Callable:
         """A new incoming event; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3876,15 +3876,15 @@
     ) -> Callable:
         """A new incoming query; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3910,15 +3910,15 @@
     ) -> Callable:
         """A poll was updated; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3944,15 +3944,15 @@
     ) -> Callable:
         """A user changed the answer to a poll; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -3978,15 +3978,15 @@
     ) -> Callable:
         """User rights changed in a chat; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -4012,15 +4012,15 @@
     ) -> Callable:
         """A user sent a join request to a chat; for bots only
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
@@ -4052,15 +4052,15 @@
     ) -> Callable:
         """Contains a list of updates
 
         Args:
             filters (:class:`pytdbot.filters.Filter`, *optional*):
                 An update filter
 
-            position (``int``, *optional``):
+            position (``int``, *optional*):
                 The function position in handlers list. Defaults to ``None`` (append)
 
         Raises:
             :py:class:`TypeError`
         """
 
         def decorator(func: Callable) -> Callable:
```

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/methods/methods.py` & `Pytdbot-0.8.4.dev2/pytdbot/methods/methods.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/methods/tdlibfunctions.py` & `Pytdbot-0.8.4.dev2/pytdbot/methods/tdlibfunctions.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/td_api.json` & `Pytdbot-0.8.4.dev2/pytdbot/td_api.json`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/td_api.tl` & `Pytdbot-0.8.4.dev2/pytdbot/td_api.tl`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/tdjson/tdjson.py` & `Pytdbot-0.8.4.dev2/pytdbot/tdjson/tdjson.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from ctypes.util import find_library
 from ctypes import c_int, c_double, c_void_p, c_char_p, CDLL
 from logging import getLogger
 from typing import Union
-from platform import system
-from pkg_resources import resource_filename
 
 try:
     import orjson as json
 except ImportError:
     try:
         import ujson as json
     except ImportError:
         import json
 
 logger = getLogger(__name__)
 
 
 def dumps(obj) -> bytes:
     if json.__name__ == "orjson":
-        return json.dumps(obj).decode().encode("utf-8")
+        # Null-terminated string is needed for orjson with c_char_p
+        return json.dumps(obj) + b"\0"
     else:
         return json.dumps(obj).encode("utf-8")
 
 
 class TdJson:
     def __init__(self, lib_path: str = None, verbosity: int = 2) -> None:
         """TdJson client
@@ -35,28 +34,28 @@
                 TDLib verbosity level. Defaults to ``2``
 
         Raises:
             :py:class:``ValueError``: If library not found
         """
 
         if lib_path is None:
-            # if system() == "Linux":
-            #     lib_path = find_library("tdjson") or resource_filename(
-            #         "pytdbot", "lib/libtdjson.so"
-            #     )
-            # else:
             lib_path = find_library("tdjson")
 
         if not lib_path:
             raise ValueError("TDLib library not found")
 
-        logger.debug(f'Using "{json.__name__}" module as JSON encoder')
         logger.info(f"Initializing TdJson client with library: {lib_path}")
         self._build_client(lib_path, verbosity)
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        pass
+
     def _build_client(self, lib_path: str, verbosity: int) -> None:
         """Build TdJson client
 
         Args:
             lib_path (``str``):
                 Path to shared library
 
@@ -66,18 +65,14 @@
         self._tdjson = CDLL(lib_path)
 
         # load TDLib functions from shared library
         self._td_create_client_id = self._tdjson.td_create_client_id
         self._td_create_client_id.restype = c_int
         self._td_create_client_id.argtypes = []
 
-        self._td_client_destroy = self._tdjson.td_json_client_destroy
-        self._td_client_destroy.restype = None
-        self._td_client_destroy.argtypes = [c_void_p]
-
         self._td_receive = self._tdjson.td_receive
         self._td_receive.restype = c_char_p
         self._td_receive.argtypes = [c_double]
 
         self._td_send = self._tdjson.td_send
         self._td_send.restype = None
         self._td_send.argtypes = [c_int, c_char_p]
@@ -89,15 +84,15 @@
         self.client_id = self._td_create_client_id()
 
         td_version, td_commit_hash = self.execute(
             {"@type": "getOption", "name": "version"}
         ), self.execute({"@type": "getOption", "name": "commit_hash"})
 
         logger.info(
-            f"Using TDLib {td_version['value']} ({td_commit_hash['value'][:9]})"
+            f"Using TDLib {td_version['value']} ({td_commit_hash['value'][:9]}) with {json.__name__} encoder"
         )
 
         if isinstance(verbosity, int):
             res = self.execute(
                 {"@type": "setLogVerbosityLevel", "new_verbosity_level": verbosity}
             )
 
@@ -110,20 +105,16 @@
         Args:
             timeout (``float``, *optional*):
                 The maximum number of seconds allowed to wait for new data. Defaults to 2.0
 
         Returns:
             :py:class:``dict``: An incoming update or result to a request. If no data is received, ``None`` is returned
         """
-        try:
-            if res := self._td_receive(self.client_id, c_double(timeout)):
-                return json.loads(res)
-        except Exception:
-            logger.exception("Exception while receiving")
-            raise
+        if res := self._td_receive(self.client_id, c_double(timeout)):
+            return json.loads(res)
 
     def send(self, data: dict) -> None:
         """Sends a request to TDLib
 
         Args:
             data (``dict``):
                 The request to be sent
@@ -145,11 +136,7 @@
         """
         try:
             if res := self._td_execute(dumps(data)):
                 return json.loads(res)
         except Exception:
             logger.exception("Exception while executing")
             raise
-
-    def destroy(self) -> None:
-        """Destroys the TDLib client."""
-        self._td_client_destroy(self.client_id)
```

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/__init__.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/force_reply.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/force_reply.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/inline_keyboard.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/remove_keyboard.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/remove_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/buttons/show_keyboard.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/show_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_generated.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_generated.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_local.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_local.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_file_remote.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_remote.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/inputfile/input_thumbnail.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/logstream/log_stream_file.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_file.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/result/result.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/result/result.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/update/chatActions.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/update/chatActions.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/types/update/update.py` & `Pytdbot-0.8.4.dev2/pytdbot/types/update/update.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/utils/escape.py` & `Pytdbot-0.8.4.dev2/pytdbot/utils/escape.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/pytdbot/utils/text_format.py` & `Pytdbot-0.8.4.dev2/pytdbot/utils/text_format.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev1/setup.py` & `Pytdbot-0.8.4.dev2/setup.py`

 * *Files identical despite different names*

