# Comparing `tmp/khoj_assistant-0.6.3.dev45.tar.gz` & `tmp/khoj_assistant-0.6.3.dev53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jun  9 13:06:49 2023, max compression
+gzip compressed data, last modified: Sat Jun 17 06:58:47 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev45.tar` & `khoj_assistant-0.6.3.dev53.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/__init__.py
--rw-r--r--   0        0        0    10308 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      861 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    15746 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9707 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    12201 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4526 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4216 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3930 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5701 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6526 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5153 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    11299 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2434 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2713 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/models.py
--rw-r--r--   0        0        0     3781 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/LICENSE
--rw-r--r--   0        0        0    21788 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/README.md
--rw-r--r--   0        0        0     2759 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/pyproject.toml
--rw-r--r--   0        0        0    24096 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10845 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17706 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9707 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    12314 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4526 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     3815 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    11901 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3027 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4008 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/LICENSE
+-rw-r--r--   0        0        0    22877 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/README.md
+-rw-r--r--   0        0        0     2783 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/pyproject.toml
+-rw-r--r--   0        0        0    25217 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev53/src/khoj/configure.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Internal Packages
 from khoj.processor.conversation.gpt import summarize
 from khoj.processor.ledger.beancount_to_jsonl import BeancountToJsonl
 from khoj.processor.jsonl.jsonl_to_jsonl import JsonlToJsonl
 from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.org_mode.org_to_jsonl import OrgToJsonl
 from khoj.processor.pdf.pdf_to_jsonl import PdfToJsonl
+from khoj.processor.github.github_to_jsonl import GithubToJsonl
 from khoj.search_type import image_search, text_search
 from khoj.utils import constants, state
 from khoj.utils.config import SearchType, SearchModels, ProcessorConfigModel, ConversationProcessorConfigModel
 from khoj.utils.helpers import LRU, resolve_absolute_path, merge_dicts
 from khoj.utils.rawconfig import FullConfig, ProcessorConfig
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.word_filter import WordFilter
@@ -85,15 +86,15 @@
 
 
 def configure_search(model: SearchModels, config: FullConfig, regenerate: bool, t: state.SearchType = None):
     # Initialize Org Notes Search
     if (t == state.SearchType.Org or t == None) and config.content_type.org:
         logger.info("🦄 Setting up search for orgmode notes")
         # Extract Entries, Generate Notes Embeddings
-        model.orgmode_search = text_search.setup(
+        model.org_search = text_search.setup(
             OrgToJsonl,
             config.content_type.org,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
@@ -149,14 +150,25 @@
     if (t == state.SearchType.Image or t == None) and config.content_type.image:
         logger.info("🌄 Setting up search for images")
         # Extract Entries, Generate Image Embeddings
         model.image_search = image_search.setup(
             config.content_type.image, search_config=config.search_type.image, regenerate=regenerate
         )
 
+    if (t == state.SearchType.Github or t == None) and config.content_type.github:
+        logger.info("🐙 Setting up search for github")
+        # Extract Entries, Generate Github Embeddings
+        model.github_search = text_search.setup(
+            GithubToJsonl,
+            config.content_type.github,
+            search_config=config.search_type.asymmetric,
+            regenerate=regenerate,
+            filters=[DateFilter(), WordFilter(), FileFilter()],
+        )
+
     # Initialize External Plugin Search
     if (t == None or t in state.SearchType) and config.content_type.plugins:
         logger.info("🔌 Setting up search for plugins")
         model.plugin_search = {}
         for plugin_type, plugin_config in config.content_type.plugins.items():
             model.plugin_search[plugin_type] = text_search.setup(
                 JsonlToJsonl,
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/main.py` & `khoj_assistant-0.6.3.dev53/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # External Packages
 from PyQt6 import QtWidgets
 
 # Internal Packages
 from khoj.utils.config import ProcessorType
+from khoj.utils.config import SearchType
 
 
 class LabelledTextField(QtWidgets.QWidget):
-    def __init__(self, title, processor_type: ProcessorType = None, default_value: str = None):
+    def __init__(
+        self, title, search_type: SearchType = None, processor_type: ProcessorType = None, default_value: str = None
+    ):
         QtWidgets.QWidget.__init__(self)
         layout = QtWidgets.QHBoxLayout()
         self.setLayout(layout)
         self.processor_type = processor_type
+        self.search_type = search_type
 
         self.label = QtWidgets.QLabel()
         self.label.setText(title)
         self.label.setFixedWidth(95)
         self.label.setWordWrap(True)
         layout.addWidget(self.label)
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/main_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         # Add Settings Panels for each Search Type to Configure Window Layout
         self.search_settings_panels = []
         for search_type in SearchType:
             current_content_config = self.current_config["content-type"].get(
                 search_type, None
             ) or self.get_default_config(search_type=search_type)
             self.search_settings_panels += [self.add_settings_panel(current_content_config, search_type)]
-
         # Add Conversation Processor Panel to Configure Screen
         self.processor_settings_panels = []
         conversation_type = ProcessorType.Conversation
         if self.current_config["processor"] and conversation_type in self.current_config["processor"]:
             current_conversation_config = self.current_config["processor"][conversation_type]
         else:
             current_conversation_config = self.get_default_config(processor_type=conversation_type)
@@ -84,14 +83,16 @@
 
     def add_settings_panel(self, current_content_config: dict, search_type: SearchType):
         "Add Settings Panel for specified Search Type. Toggle Editable Search Types"
         # Get current files from config for given search type
         if search_type == SearchType.Image:
             current_content_files = current_content_config.get("input-directories", [])
             file_input_text = f"{search_type.name} Folders"
+        elif search_type == SearchType.Github:
+            return self.add_github_settings_panel(current_content_config, SearchType.Github)
         else:
             current_content_files = current_content_config.get("input-files", [])
             file_input_text = f"{search_type.name} Files"
 
         # Create widgets to display settings for given search type
         search_type_settings = QtWidgets.QWidget()
         search_type_layout = QtWidgets.QVBoxLayout(search_type_settings)
@@ -107,25 +108,58 @@
         # Add setting widgets for given search type to panel
         search_type_layout.addWidget(enable_search_type)
         search_type_layout.addWidget(input_files)
         self.wlayout.addWidget(search_type_settings)
 
         return search_type_settings
 
+    def add_github_settings_panel(self, current_content_config: dict, search_type: SearchType):
+        search_type_settings = QtWidgets.QWidget()
+        search_type_layout = QtWidgets.QVBoxLayout(search_type_settings)
+        enable_search_type = SearchCheckBox(f"Search {search_type.name}", search_type)
+        # Add labelled text input field
+        input_fields = []
+
+        fields = ["pat-token", "repo-name", "repo-owner", "repo-branch"]
+        active = False
+        for field in fields:
+            field_value = current_content_config.get(field, None)
+            input_field = LabelledTextField(field, search_type=search_type, default_value=field_value)
+            search_type_layout.addWidget(input_field)
+            input_fields += [input_field]
+            if field_value:
+                active = True
+
+        # Set enabled/disabled based on checkbox state
+        enable_search_type.setChecked(active)
+        for input_field in input_fields:
+            input_field.setEnabled(enable_search_type.isChecked())
+        enable_search_type.stateChanged.connect(lambda _: [input_field.setEnabled(enable_search_type.isChecked()) for input_field in input_fields])  # type: ignore[attr-defined]
+
+        # Add setting widgets for given search type to panel
+        search_type_layout.addWidget(enable_search_type)
+        for input_field in input_fields:
+            search_type_layout.addWidget(input_field)
+        self.wlayout.addWidget(search_type_settings)
+
+        return search_type_settings
+
     def add_processor_panel(self, current_conversation_config: dict, processor_type: ProcessorType):
         "Add Conversation Processor Panel"
         # Get current settings from config for given processor type
         current_openai_api_key = current_conversation_config.get("openai-api-key", None)
 
         # Create widgets to display settings for given processor type
         processor_type_settings = QtWidgets.QWidget()
         processor_type_layout = QtWidgets.QVBoxLayout(processor_type_settings)
         enable_conversation = ProcessorCheckBox(f"Conversation", processor_type)
         # Add file browser to set input files for given processor type
-        input_field = LabelledTextField("OpenAI API Key", processor_type, current_openai_api_key)
+        input_field = LabelledTextField(
+            "OpenAI API Key", processor_type=processor_type, default_value=current_openai_api_key
+        )
 
         # Set enabled/disabled based on checkbox state
         enable_conversation.setChecked(current_openai_api_key is not None)
         input_field.setEnabled(enable_conversation.isChecked())
         enable_conversation.stateChanged.connect(lambda _: input_field.setEnabled(enable_conversation.isChecked()))  # type: ignore[attr-defined]
 
         # Add setting widgets for given processor type to panel
@@ -181,15 +215,15 @@
             error_message.setStyleSheet("color: red")
             self.wlayout.addWidget(error_message)
 
     def update_search_settings(self):
         "Update config with search settings from UI"
         for settings_panel in self.search_settings_panels:
             for child in settings_panel.children():
-                if not isinstance(child, (SearchCheckBox, FileBrowser)):
+                if not isinstance(child, (SearchCheckBox, FileBrowser, LabelledTextField)):
                     continue
                 if isinstance(child, SearchCheckBox):
                     # Search Type Disabled
                     if not child.isChecked() and child.search_type in self.new_config["content-type"]:
                         del self.new_config["content-type"][child.search_type]
                     # Search Type (re)-Enabled
                     if child.isChecked():
@@ -203,14 +237,18 @@
                         self.new_config["content-type"][child.search_type.value]["input-directories"] = (
                             child.getPaths() if child.getPaths() != [] else None
                         )
                     else:
                         self.new_config["content-type"][child.search_type.value]["input-files"] = (
                             child.getPaths() if child.getPaths() != [] else None
                         )
+                elif isinstance(child, LabelledTextField):
+                    self.new_config["content-type"][child.search_type.value][
+                        child.label.text()
+                    ] = child.input_field.toPlainText()
 
     def update_processor_settings(self):
         "Update config with conversation settings from UI"
         for settings_panel in self.processor_settings_panels:
             for child in settings_panel.children():
                 if not isinstance(child, (ProcessorCheckBox, LabelledTextField)):
                     continue
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
                 return render_org(query, data, "music-");
             } else if (type === "image") {
                 return data.map(render_image).join('');
             } else if (type === "ledger") {
                 return render_ledger(query, data);
             } else if (type === "pdf") {
                 return render_pdf(query, data);
+            } else if (type == "github") {
+                return render_markdown(query, data);
             } else {
                 return `<div id="results-plugin">`
                     + data.map((item) => `<p>${item.entry}</p>`).join("\n")
                     + `</div>`;
             }
         }
 
@@ -292,15 +294,15 @@
         }
         #results-pdf,
         #results-plugin,
         #results-ledger {
             text-align: left;
             white-space: pre-line;
         }
-         #results-markdown {
+         #results-markdown, #results-github {
             text-align: left;
         }
         #results-music,
         #results-org {
             text-align: left;
             white-space: pre-line;
         }
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/config.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/text_to_jsonl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from abc import ABC, abstractmethod
 import hashlib
 import logging
 from typing import Callable, List, Tuple
 from khoj.utils.helpers import timer
 
 # Internal Packages
-from khoj.utils.rawconfig import Entry, TextContentConfig
+from khoj.utils.rawconfig import Entry, TextConfigBase
 
 
 logger = logging.getLogger(__name__)
 
 
 class TextToJsonl(ABC):
-    def __init__(self, config: TextContentConfig):
+    def __init__(self, config: TextConfigBase):
         self.config = config
 
     @abstractmethod
     def process(self, previous_entries: List[Entry] = None) -> List[Tuple[int, Entry]]:
         ...
 
     @staticmethod
@@ -56,16 +56,17 @@
                         heading=entry.heading,
                         file=entry.file,
                     )
                 )
 
         return chunked_entries
 
+    @staticmethod
     def mark_entries_for_update(
-        self, current_entries: List[Entry], previous_entries: List[Entry], key="compiled", logger=None
+        current_entries: List[Entry], previous_entries: List[Entry], key="compiled", logger=None
     ) -> List[Tuple[int, Entry]]:
         # Hash all current and previous entries to identify new entries
         with timer("Hash previous, current entries", logger):
             current_entry_hashes = list(map(TextToJsonl.hash_func(key), current_entries))
             previous_entry_hashes = list(map(TextToJsonl.hash_func(key), previous_entries))
 
         with timer("Identify, Mark, Combine new, existing entries", logger):
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
             if not previous_entries:
                 entries_with_ids = list(enumerate(current_entries))
             else:
-                entries_with_ids = self.mark_entries_for_update(
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
                     current_entries,
                     previous_entries,
                     key="compiled",
                     logger=logger,
                 )
 
         with timer("Write entries to JSONL file", logger):
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated transaction", logger):
             if not previous_entries:
                 entries_with_ids = list(enumerate(current_entries))
             else:
-                entries_with_ids = self.mark_entries_for_update(
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
                     current_entries, previous_entries, key="compiled", logger=logger
                 )
 
         with timer("Write transactions to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = BeancountToJsonl.convert_transaction_maps_to_jsonl(entries)
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
             if not previous_entries:
                 entries_with_ids = list(enumerate(current_entries))
             else:
-                entries_with_ids = self.mark_entries_for_update(
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
                     current_entries, previous_entries, key="compiled", logger=logger
                 )
 
         with timer("Write markdown entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = MarkdownToJsonl.convert_markdown_maps_to_jsonl(entries)
@@ -97,36 +97,46 @@
         return all_markdown_files
 
     @staticmethod
     def extract_markdown_entries(markdown_files):
         "Extract entries by heading from specified Markdown files"
 
         # Regex to extract Markdown Entries by Heading
-        markdown_heading_regex = r"^#"
 
         entries = []
         entry_to_file_map = []
         for markdown_file in markdown_files:
             with open(markdown_file, "r", encoding="utf8") as f:
                 markdown_content = f.read()
-                markdown_entries_per_file = []
-                any_headings = re.search(markdown_heading_regex, markdown_content, flags=re.MULTILINE)
-                for entry in re.split(markdown_heading_regex, markdown_content, flags=re.MULTILINE):
-                    # Add heading level as the regex split removed it from entries with headings
-                    prefix = "#" if entry.startswith("#") else "# " if any_headings else ""
-                    stripped_entry = entry.strip(empty_escape_sequences)
-                    if stripped_entry != "":
-                        markdown_entries_per_file.append(f"{prefix}{stripped_entry}")
-
-                entry_to_file_map += zip(markdown_entries_per_file, [markdown_file] * len(markdown_entries_per_file))
-                entries.extend(markdown_entries_per_file)
+                entries, entry_to_file_map = MarkdownToJsonl.process_single_markdown_file(
+                    markdown_content, markdown_file, entries, entry_to_file_map
+                )
 
         return entries, dict(entry_to_file_map)
 
     @staticmethod
+    def process_single_markdown_file(
+        markdown_content: str, markdown_file: Path, entries: List, entry_to_file_map: List
+    ):
+        markdown_heading_regex = r"^#"
+
+        markdown_entries_per_file = []
+        any_headings = re.search(markdown_heading_regex, markdown_content, flags=re.MULTILINE)
+        for entry in re.split(markdown_heading_regex, markdown_content, flags=re.MULTILINE):
+            # Add heading level as the regex split removed it from entries with headings
+            prefix = "#" if entry.startswith("#") else "# " if any_headings else ""
+            stripped_entry = entry.strip(empty_escape_sequences)
+            if stripped_entry != "":
+                markdown_entries_per_file.append(f"{prefix}{stripped_entry}")
+
+        entry_to_file_map += zip(markdown_entries_per_file, [markdown_file] * len(markdown_entries_per_file))
+        entries.extend(markdown_entries_per_file)
+        return entries, entry_to_file_map
+
+    @staticmethod
     def convert_markdown_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
         "Convert each Markdown entries into a dictionary"
         entries = []
         for parsed_entry in parsed_entries:
             entry_filename = Path(entry_to_file_map[parsed_entry])
             heading = parsed_entry.splitlines()[0] if re.search("^#+\s", parsed_entry) else ""
             # Append base filename to compiled entry for context to model
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         if not previous_entries:
             entries_with_ids = list(enumerate(current_entries))
         else:
-            entries_with_ids = self.mark_entries_for_update(
+            entries_with_ids = TextToJsonl.mark_entries_for_update(
                 current_entries, previous_entries, key="compiled", logger=logger
             )
 
         # Process Each Entry from All Notes Files
         with timer("Write org entries to JSONL file", logger):
             entries = map(lambda entry: entry[1], entries_with_ids)
             jsonl_data = self.convert_org_entries_to_jsonl(entries)
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
             if not previous_entries:
                 entries_with_ids = list(enumerate(current_entries))
             else:
-                entries_with_ids = self.mark_entries_for_update(
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
                     current_entries, previous_entries, key="compiled", logger=logger
                 )
 
         with timer("Write PDF entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = PdfToJsonl.convert_pdf_maps_to_jsonl(entries)
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev53/src/khoj/routers/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,18 @@
             detail="Content types not configured. Configure at least one content type on server and restart it.",
         )
 
     configured_content_types = state.config.content_type.dict(exclude_none=True)
     return [
         search_type.value
         for search_type in SearchType
-        if search_type.value in configured_content_types
+        if (
+            search_type.value in configured_content_types
+            and getattr(state.model, f"{search_type.value}_search") is not None
+        )
         or ("plugins" in configured_content_types and search_type.name in configured_content_types["plugins"])
     ]
 
 
 @api.get("/config/data", response_model=FullConfig)
 def get_config_data():
     return state.config
@@ -84,19 +87,19 @@
 
     # return cached results, if available
     query_cache_key = f"{user_query}-{n}-{t}-{r}-{score_threshold}-{dedupe}"
     if query_cache_key in state.query_cache:
         logger.debug(f"Return response from query cache")
         return state.query_cache[query_cache_key]
 
-    if (t == SearchType.Org or t == None) and state.model.orgmode_search:
+    if (t == SearchType.Org or t == None) and state.model.org_search:
         # query org-mode notes
         with timer("Query took", logger):
             hits, entries = text_search.query(
-                user_query, state.model.orgmode_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
+                user_query, state.model.org_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
             )
 
         # collate and return results
         with timer("Collating results took", logger):
             results = text_search.collate_results(hits, entries, results_count)
 
     elif (t == SearchType.Markdown or t == None) and state.model.markdown_search:
@@ -117,14 +120,25 @@
                 user_query, state.model.pdf_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
             )
 
         # collate and return results
         with timer("Collating results took", logger):
             results = text_search.collate_results(hits, entries, results_count)
 
+    elif (t == SearchType.Github or t == None) and state.model.github_search:
+        # query github embeddings
+        with timer("Query took", logger):
+            hits, entries = text_search.query(
+                user_query, state.model.github_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
+            )
+
+        # collate and return results
+        with timer("Collating results took", logger):
+            results = text_search.collate_results(hits, entries, results_count)
+
     elif (t == SearchType.Ledger or t == None) and state.model.ledger_search:
         # query transactions
         with timer("Query took", logger):
             hits, entries = text_search.query(
                 user_query, state.model.ledger_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
             )
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev53/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev53/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev53/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev53/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev53/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev53/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev53/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 class SearchType(str, Enum):
     Org = "org"
     Ledger = "ledger"
     Music = "music"
     Markdown = "markdown"
     Image = "image"
     Pdf = "pdf"
+    Github = "github"
 
 
 class ProcessorType(str, Enum):
     Conversation = "conversation"
 
 
 class TextSearchModel:
@@ -54,20 +55,21 @@
         self.image_embeddings = image_embeddings
         self.image_metadata_embeddings = image_metadata_embeddings
         self.image_encoder = image_encoder
 
 
 @dataclass
 class SearchModels:
-    orgmode_search: TextSearchModel = None
+    org_search: TextSearchModel = None
     ledger_search: TextSearchModel = None
     music_search: TextSearchModel = None
     markdown_search: TextSearchModel = None
     pdf_search: TextSearchModel = None
     image_search: ImageSearchModel = None
+    github_search: TextSearchModel = None
     plugin_search: Dict[str, TextSearchModel] = None
 
 
 class ConversationProcessorConfigModel:
     def __init__(self, processor_config: ConversationProcessorConfig):
         self.openai_api_key = processor_config.openai_api_key
         self.model = processor_config.model
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,22 @@
         },
         "music": {
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/music/music.jsonl.gz",
             "embeddings-file": "~/.khoj/content/music/music_embeddings.pt",
         },
+        "github": {
+            "pat-token": None,
+            "repo-name": None,
+            "repo-owner": None,
+            "repo-branch": "master",
+            "compressed-jsonl": "~/.khoj/content/github/github.jsonl.gz",
+            "embeddings-file": "~/.khoj/content/github/github_embeddings.pt",
+        },
     },
     "search-type": {
         "symmetric": {
             "encoder": "sentence-transformers/all-MiniLM-L6-v2",
             "cross-encoder": "cross-encoder/ms-marco-MiniLM-L-6-v2",
             "model_directory": "~/.khoj/search/symmetric/",
         },
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/rawconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,40 @@
 
 class ConfigBase(BaseModel):
     class Config:
         alias_generator = to_snake_case_from_dash
         allow_population_by_field_name = True
 
 
-class TextContentConfig(ConfigBase):
-    input_files: Optional[List[Path]]
-    input_filter: Optional[List[str]]
+class TextConfigBase(ConfigBase):
     compressed_jsonl: Path
     embeddings_file: Path
+
+
+class TextContentConfig(TextConfigBase):
+    input_files: Optional[List[Path]]
+    input_filter: Optional[List[str]]
     index_heading_entries: Optional[bool] = False
 
     @validator("input_filter")
     def input_filter_or_files_required(cls, input_filter, values, **kwargs):
         if is_none_or_empty(input_filter) and ("input_files" not in values or values["input_files"] is None):
             raise ValueError(
                 "Either input_filter or input_files required in all content-type.<text_search> section of Khoj config file"
             )
         return input_filter
 
 
+class GithubContentConfig(TextConfigBase):
+    pat_token: str
+    repo_name: str
+    repo_owner: str
+    repo_branch: Optional[str] = "master"
+
+
 class ImageContentConfig(ConfigBase):
     input_directories: Optional[List[Path]]
     input_filter: Optional[List[str]]
     embeddings_file: Path
     use_xmp_metadata: bool
     batch_size: int
 
@@ -53,14 +63,15 @@
 class ContentConfig(ConfigBase):
     org: Optional[TextContentConfig]
     ledger: Optional[TextContentConfig]
     image: Optional[ImageContentConfig]
     music: Optional[TextContentConfig]
     markdown: Optional[TextContentConfig]
     pdf: Optional[TextContentConfig]
+    github: Optional[GithubContentConfig]
     plugins: Optional[Dict[str, TextContentConfig]]
 
 
 class TextSearchConfig(ConfigBase):
     encoder: str
     cross_encoder: str
     encoder_type: Optional[str]
```

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev53/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/.gitignore` & `khoj_assistant-0.6.3.dev53/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/LICENSE` & `khoj_assistant-0.6.3.dev53/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev45/README.md` & `khoj_assistant-0.6.3.dev53/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,27 +59,27 @@
 - **Chat**
   - **Faster answers**: Find answers faster, smoother than search. No need to manually scan through your notes to find answers.
   - **Iterative discovery**: Iteratively explore and (re-)discover your notes
   - **Assisted creativity**: Smoothly weave across answers retrieval and content generation
 - **General**
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
-  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files and Photos
+  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files, Github repositories, and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
-- Let Khoj backend index the markdown, pdf files in the current Vault
+- Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
 - Open Khoj plugin on Obsidian via Search button on Left Pane
 - Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
 - Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
 </details>
 
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
@@ -324,14 +324,19 @@
 ### GPT API
 - The [chat](http://localhost:8000/api/chat), [answer](http://localhost:8000/api/beta/answer) and [search](http://localhost:8000/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
 - They are disabled by default
 - To use them:
   1. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   2. Interact with them from the [Khoj Swagger docs](http://locahost:8000/docs)[^2]
 
+### Use a Github Repository as a source
+Note that this plugin is currently *only* indexing Markdown files. It will ignore all other files in the repository. This is because Khoj, as it stands, is a semantic search engine. Eventually, we hope to get to a state where you can search for any file in your repository and even explain code.
+
+1. Get a [pat token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token) with `repo` and `read:org` scopes in the classic flow.
+2. Configure your settings to include the `owner` and `repo_name`. The `owner` will be the organization name if the repo is in an organization. The `repo_name` will be the name of the repository. Optionally, you can also supply a branch name. If no branch name is supplied, the `master` branch will be used.
 
 ## Performance
 
 ### Query performance
 
 - Semantic search using the bi-encoder is fairly fast at \<50 ms
 - Reranking using the cross-encoder is slower at \<2s on 15 results. Tweak `top_k` to tradeoff speed for accuracy of results
@@ -392,15 +397,15 @@
 
 ```shell
 git clone https://github.com/debanjum/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
-- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf and beancount directories
+- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf, Github repositories, and beancount directories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
 ##### 3. Run
 
 ```shell
 docker-compose up -d
 ```
@@ -454,15 +459,15 @@
    ```
    - This ensures standard code formatting fixes and other checks run automatically on every commit and push
    - Note 1: If [pre-commit](https://pre-commit.com/#intro) didn't already get installed, [install it](https://pre-commit.com/#install) via `pip install pre-commit`
    - Note 2: To run the pre-commit changes manually, use `pre-commit run --hook-stage manual --all` before creating PR
 
 #### Before Creating PR
 
-1. Run Tests
+1. Run Tests. If you get an error complaining about a missing `fast_tokenizer_file`, follow the solution [in this Github issue](https://github.com/UKPLab/sentence-transformers/issues/1659).
    ```shell
    pytest
    ```
 
 2. Run MyPy to check types
    ```shell
    mypy --config-file pyproject.toml
```

### Comparing `khoj_assistant-0.6.3.dev45/pyproject.toml` & `khoj_assistant-0.6.3.dev53/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "schedule == 1.1.0",
     "sentence-transformers == 2.2.2",
     "torch == 1.13.1",
     "uvicorn == 0.17.6",
     "aiohttp == 3.8.4",
     "langchain >= 0.0.187",
     "pypdf >= 3.9.0",
+    "llama-hub==0.0.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/debanjum/khoj#readme"
 Issues = "https://github.com/debanjum/khoj/issues"
 Discussions = "https://github.com/debanjum/khoj/discussions"
```

### Comparing `khoj_assistant-0.6.3.dev45/PKG-INFO` & `khoj_assistant-0.6.3.dev53/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev45
+Version: 0.6.3.dev53
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -24,14 +24,15 @@
 Requires-Python: <3.11,>=3.8
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: dateparser==1.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: fastapi==0.77.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: langchain>=0.0.187
+Requires-Dist: llama-hub==0.0.3
 Requires-Dist: openai>=0.27.0
 Requires-Dist: pillow==9.3.0
 Requires-Dist: pydantic>=1.9.1
 Requires-Dist: pypdf>=3.9.0
 Requires-Dist: pyqt6==6.3.1
 Requires-Dist: pyyaml==6.0
 Requires-Dist: rich>=13.3.1
@@ -114,27 +115,27 @@
 - **Chat**
   - **Faster answers**: Find answers faster, smoother than search. No need to manually scan through your notes to find answers.
   - **Iterative discovery**: Iteratively explore and (re-)discover your notes
   - **Assisted creativity**: Smoothly weave across answers retrieval and content generation
 - **General**
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
-  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files and Photos
+  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files, Github repositories, and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
-- Let Khoj backend index the markdown, pdf files in the current Vault
+- Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
 - Open Khoj plugin on Obsidian via Search button on Left Pane
 - Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
 - Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
 </details>
 
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
@@ -379,14 +380,19 @@
 ### GPT API
 - The [chat](http://localhost:8000/api/chat), [answer](http://localhost:8000/api/beta/answer) and [search](http://localhost:8000/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
 - They are disabled by default
 - To use them:
   1. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   2. Interact with them from the [Khoj Swagger docs](http://locahost:8000/docs)[^2]
 
+### Use a Github Repository as a source
+Note that this plugin is currently *only* indexing Markdown files. It will ignore all other files in the repository. This is because Khoj, as it stands, is a semantic search engine. Eventually, we hope to get to a state where you can search for any file in your repository and even explain code.
+
+1. Get a [pat token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token) with `repo` and `read:org` scopes in the classic flow.
+2. Configure your settings to include the `owner` and `repo_name`. The `owner` will be the organization name if the repo is in an organization. The `repo_name` will be the name of the repository. Optionally, you can also supply a branch name. If no branch name is supplied, the `master` branch will be used.
 
 ## Performance
 
 ### Query performance
 
 - Semantic search using the bi-encoder is fairly fast at \<50 ms
 - Reranking using the cross-encoder is slower at \<2s on 15 results. Tweak `top_k` to tradeoff speed for accuracy of results
@@ -447,15 +453,15 @@
 
 ```shell
 git clone https://github.com/debanjum/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
-- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf and beancount directories
+- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf, Github repositories, and beancount directories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
 ##### 3. Run
 
 ```shell
 docker-compose up -d
 ```
@@ -509,15 +515,15 @@
    ```
    - This ensures standard code formatting fixes and other checks run automatically on every commit and push
    - Note 1: If [pre-commit](https://pre-commit.com/#intro) didn't already get installed, [install it](https://pre-commit.com/#install) via `pip install pre-commit`
    - Note 2: To run the pre-commit changes manually, use `pre-commit run --hook-stage manual --all` before creating PR
 
 #### Before Creating PR
 
-1. Run Tests
+1. Run Tests. If you get an error complaining about a missing `fast_tokenizer_file`, follow the solution [in this Github issue](https://github.com/UKPLab/sentence-transformers/issues/1659).
    ```shell
    pytest
    ```
 
 2. Run MyPy to check types
    ```shell
    mypy --config-file pyproject.toml
```

