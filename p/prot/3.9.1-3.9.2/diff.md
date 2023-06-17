# Comparing `tmp/prot-3.9.1.tar.gz` & `tmp/prot-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prot-3.9.1.tar", last modified: Fri Jun 16 14:28:29 2023, max compression
+gzip compressed data, was "prot-3.9.2.tar", last modified: Fri Jun 16 17:50:16 2023, max compression
```

## Comparing `prot-3.9.1.tar` & `prot-3.9.2.tar`

### file list

```diff
@@ -1,213 +1,30 @@
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1069 2023-06-15 09:23:01.000000 prot-3.9.1/LICENSE
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 14:28:29.388023 prot-3.9.1/PKG-INFO
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1444 2023-06-15 09:23:01.000000 prot-3.9.1/README.md
--rw-r--r--   0 u0_a269  (10269) u0_a269  (10269)       57 2023-06-15 09:29:23.000000 prot-3.9.1/pyproject.toml
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       38 2023-06-16 14:28:29.388023 prot-3.9.1/setup.cfg
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1429 2023-06-15 09:23:01.000000 prot-3.9.1/setup.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.348023 prot-3.9.1/src/
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    48198 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4570 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/__main__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       22 2023-06-16 14:27:37.000000 prot-3.9.1/src/prot/__version__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot/bs/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      137 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5598 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2190 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bsMap.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      913 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bsPro.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1300 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bsSpaz.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    16236 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/code.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot/color/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      239 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2299 2023-06-16 11:24:46.000000 prot-3.9.1/src/prot/color/ansi.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10557 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/ansitowin32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1915 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/initialise.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5480 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/win32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6464 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/color/winterm.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.360023 prot-3.9.1/src/prot/pip/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12223 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/pip/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2355 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/pip/__main__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      797 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/pip/extra.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       18 2023-06-16 11:46:04.000000 prot-3.9.1/src/prot/pip/packagesList.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.360023 prot-3.9.1/src/prot/progress/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4883 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/progress/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2789 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/progress/bar.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1373 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/progress/counter.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1381 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/progress/spinner.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      872 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/__init__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/application/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      518 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/application/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    44504 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/application/application.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5061 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/application/current.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1349 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/application/dummy.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3699 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/application/run_in_terminal.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5918 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/prompt/auto_suggest.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    70295 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/buffer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3788 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/cache.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/clipboard/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      403 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/clipboard/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2488 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/prompt/clipboard/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1076 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/clipboard/in_memory.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1148 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/clipboard/pyperclip.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/completion/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      813 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/completion/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    11486 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3831 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/filesystem.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6962 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/completion/fuzzy_completer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3884 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/nested.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2931 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/word_completer.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/contrib/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/__init__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/completers/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       36 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/completers/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2061 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/contrib/completers/system.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/regular_languages/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3220 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    21876 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/compiler.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3238 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/completion.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3385 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/lexer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7825 2023-06-16 11:24:49.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/regex_parser.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2034 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/validation.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/ssh/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      138 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/ssh/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4365 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/ssh/server.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/telnet/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       68 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      130 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/log.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4965 2023-06-16 11:24:49.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/protocol.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     9510 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/server.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      187 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/data_structures.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    40581 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/document.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      322 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/enums.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/eventloop/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      670 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/eventloop/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4126 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/eventloop/async_context_manager.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1711 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/async_generator.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1117 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/dummy_contextvars.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5514 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/inputhook.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3251 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2008 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/win32.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.372023 prot-3.9.1/src/prot/prompt/filters/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1028 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/filters/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     9261 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/filters/app.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5733 2023-06-16 11:24:49.000000 prot-3.9.1/src/prot/prompt/filters/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1830 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/filters/cli.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      848 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/filters/utils.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.372023 prot-3.9.1/src/prot/prompt/formatted_text/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1386 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/formatted_text/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8089 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/formatted_text/ansi.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4907 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/formatted_text/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4324 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/formatted_text/html.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      756 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/formatted_text/pygments.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2747 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/formatted_text/utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7129 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/history.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.372023 prot-3.9.1/src/prot/prompt/input/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      209 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    13116 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/ansi_escape_sequences.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3269 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1522 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1831 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/posix_pipe.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3897 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/posix_utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2538 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/typeahead.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10106 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/input/vt100.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8400 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/vt100_parser.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    22331 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/input/win32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4101 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/win32_pipe.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.376023 prot-3.9.1/src/prot/prompt/key_binding/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      339 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/__init__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.376023 prot-3.9.1/src/prot/prompt/key_binding/bindings/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1736 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/auto_suggest.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7109 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/basic.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6986 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/completion.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      744 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/cpr.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    19692 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/emacs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      468 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/focus.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4946 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/mouse.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    18366 2023-06-16 11:24:52.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/named_commands.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1316 2023-06-16 11:24:51.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/open_in_editor.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2437 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/page_navigation.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5573 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/scroll.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2583 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/search.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    75426 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/vi.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2034 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    32798 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/digraphs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      889 2023-06-16 11:24:51.000000 prot-3.9.1/src/prot/prompt/key_binding/emacs_state.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    19364 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/key_bindings.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    17624 2023-06-16 11:24:53.000000 prot-3.9.1/src/prot/prompt/key_binding/key_processor.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3312 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/vi_state.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4885 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/keys.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.380023 prot-3.9.1/src/prot/prompt/layout/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3503 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    97509 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/containers.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    35014 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/controls.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6937 2023-06-16 11:24:53.000000 prot-3.9.1/src/prot/prompt/layout/dimension.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1001 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/layout/dummy.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    14083 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/layout.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10431 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/margins.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    25363 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/menus.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1043 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/layout/mouse_handlers.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    34212 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/processors.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     9766 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/screen.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2259 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/layout/utils.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.380023 prot-3.9.1/src/prot/prompt/lexers/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      372 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/lexers/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2320 2023-06-16 11:24:54.000000 prot-3.9.1/src/prot/prompt/lexers/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    11918 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/lexers/pygments.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      116 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/log.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1339 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/mouse_events.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/output/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      244 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6268 2023-06-16 11:24:54.000000 prot-3.9.1/src/prot/prompt/output/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2199 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/color_depth.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1487 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/conemu.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1902 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/output/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    21280 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/output/vt100.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    21158 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/output/win32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2794 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/windows10.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5154 2023-06-16 11:24:55.000000 prot-3.9.1/src/prot/prompt/patch_stdout.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    25837 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/renderer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6996 2023-06-16 11:24:56.000000 prot-3.9.1/src/prot/prompt/search.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1288 2023-06-16 11:24:56.000000 prot-3.9.1/src/prot/prompt/selection.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/shortcuts/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      877 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8808 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/dialogs.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      461 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    14072 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    11779 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/formatters.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    58073 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/prompt.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5770 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/utils.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/styles/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1844 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/styles/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5062 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/styles/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8409 2023-06-16 11:24:57.000000 prot-3.9.1/src/prot/prompt/styles/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4355 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/styles/named_colors.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1952 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/styles/pygments.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    13015 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/styles/style.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12433 2023-06-16 11:24:58.000000 prot-3.9.1/src/prot/prompt/styles/style_transformation.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       85 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/token.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8084 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5836 2023-06-16 11:24:57.000000 prot-3.9.1/src/prot/prompt/validation.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/src/prot/prompt/widgets/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1164 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    28649 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3372 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/dialogs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12824 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/menus.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12441 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/toolbars.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4138 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/win32_types.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/src/prot/wcwidth/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      150 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/wcwidth/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10556 2023-06-16 11:24:58.000000 prot-3.9.1/src/prot/wcwidth/table_wide.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    31378 2023-06-16 11:24:59.000000 prot-3.9.1/src/prot/wcwidth/table_zero.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/src/prot/wcwidth/tests/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       42 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/wcwidth/tests/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3941 2023-06-16 11:24:58.000000 prot-3.9.1/src/prot/wcwidth/tests/test_core.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7908 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/wcwidth/wcwidth.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot.egg-info/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/PKG-INFO
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6360 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/SOURCES.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        1 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/dependency_links.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       59 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/entry_points.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        5 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 17:50:16.659295 prot-3.9.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-01 19:48:21.000000 prot-3.9.2/LICENSE
+-rw-rw-rw-   0        0        0     2562 2023-06-16 17:50:16.659295 prot-3.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1642 2023-06-16 17:44:01.000000 prot-3.9.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:50:16.659295 prot-3.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-06-16 17:29:07.000000 prot-3.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:50:16.574594 prot-3.9.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 17:50:16.590214 prot-3.9.2/src/prot/
+-rw-rw-rw-   0        0        0    49983 2023-06-16 17:01:08.000000 prot-3.9.2/src/prot/__init__.py
+-rw-rw-rw-   0        0        0     4701 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-06-16 17:35:13.000000 prot-3.9.2/src/prot/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:50:16.605826 prot-3.9.2/src/prot/bs/
+-rw-rw-rw-   0        0        0      141 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/bs/__init__.py
+-rw-rw-rw-   0        0        0     5784 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/bs/bs.py
+-rw-rw-rw-   0        0        0     2278 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/bs/bsMap.py
+-rw-rw-rw-   0        0        0      952 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/bs/bsPro.py
+-rw-rw-rw-   0        0        0     1354 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/bs/bsSpaz.py
+-rw-rw-rw-   0        0        0    16635 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/code.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:50:16.643644 prot-3.9.2/src/prot/pip/
+-rw-rw-rw-   0        0        0    12590 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/pip/__init__.py
+-rw-rw-rw-   0        0        0     2433 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/pip/__main__.py
+-rw-rw-rw-   0        0        0      830 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/pip/extra.py
+-rw-rw-rw-   0        0        0       19 2023-06-16 16:37:17.000000 prot-3.9.2/src/prot/pip/packagesList.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:50:16.590214 prot-3.9.2/src/prot.egg-info/
+-rw-rw-rw-   0        0        0     2562 2023-06-16 17:50:16.000000 prot-3.9.2/src/prot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-16 17:50:16.000000 prot-3.9.2/src/prot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:50:16.000000 prot-3.9.2/src/prot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-16 17:50:16.000000 prot-3.9.2/src/prot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 17:50:16.000000 prot-3.9.2/src/prot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 17:50:16.000000 prot-3.9.2/src/prot.egg-info/top_level.txt
```

### Comparing `prot-3.9.1/LICENSE` & `prot-3.9.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `prot-3.9.1/PKG-INFO` & `prot-3.9.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,104 @@
-Metadata-Version: 2.1
-Name: prot
-Version: 3.9.1
-Summary: A Simple Tool That Contains Advance Functions.
-Home-page: https://github.com/SAPTeamDEV/prot
-Author: Alireza Poodineh
-Author-email: itsaeliux@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Prot - Pro Tools for Python 3
-
-[![Downloads](https://static.pepy.tech/badge/prot)](https://pepy.tech/project/prot)
-
-Modules
--------
-
- * **classes**
- * **functions**
- * **converters**
- * **settings**
-
-classes Module
---------------
-
- * **Database**
- * **OptionsDatabase**
- * **Progress**
- * **ProgressBar** (from **Progress** and **BarWidget**)
- * **LockedDict**
- * **Str**
- * **TextListFile**
- * **Widget**
-
- >* **TimeWidget**
- >* **BarWidget**
- >* **TaskWidget**
- >* **CallWidget**
- >* **ValueWidget**
- >* **LoadingWidget**
-
-functions Module
-----------------
-
- * **verifyColor**
- * **insertColor**
- * **getRandomPassword**
- * **testSpeed**
- * **getVarFromFile**
- * **checkMethods**
- * **callMethods**
- * **callMethodsWithArg**
- * **checkFileSame**
- * **splitStr**
- * **runAsMain**
- * **printMsg**
- * **printErr**
- * **printWarn**
-
-converters Module
------------------
-
- * **rst2html**
- * **dict2matrix**
- * **str2list**
- * **list2str**
- * **matrix2str**
-
-Packages
---------
-
- * **color**
- * **pip**
- * **progress**
- * **prompt**
- * **wcwidth**
-
-pip Package
------------
-
- >this is a Advanced pip Tool, this Package has a List of all pip Packages that you can Search, Download and Install them and you can Update this List anytime you want
-
- **Features**
-
- >* it has built in Packages List
- >* you can do an Offline Search
- >* can Create Offline Repositiry
- >* can do Batch Install or Download with built in List or use Custom List
- >* and more...
+Metadata-Version: 2.1
+Name: prot
+Version: 3.9.2
+Summary: A Simple Tool That Contains Advance Functions.
+Home-page: https://github.com/SAPTeamDEV/prot
+Author: Alireza Poodineh
+Author-email: itsaeliux@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Prot - Pro Tools for Python 3
+
+[![Downloads](https://static.pepy.tech/badge/prot)](https://pepy.tech/project/prot)
+
+> Note: this readme is not updated and does not reflect the latest applied patches. A huge update is under the way!
+
+Modules
+-------
+
+ * **classes**
+ * **functions**
+ * **converters**
+ * **settings**
+
+classes Module
+--------------
+
+ * **Database**
+ * **OptionsDatabase**
+ * **Progress**
+ * **ProgressBar** (from **Progress** and **BarWidget**)
+ * **LockedDict**
+ * **Str**
+ * **TextListFile**
+ * **Widget**
+
+ >* **TimeWidget**
+ >* **BarWidget**
+ >* **TaskWidget**
+ >* **CallWidget**
+ >* **ValueWidget**
+ >* **LoadingWidget**
+
+functions Module
+----------------
+
+ * **verifyColor**
+ * **insertColor**
+ * **getRandomPassword**
+ * **testSpeed**
+ * **getVarFromFile**
+ * **checkMethods**
+ * **callMethods**
+ * **callMethodsWithArg**
+ * **checkFileSame**
+ * **splitStr**
+ * **runAsMain**
+ * **printMsg**
+ * **printErr**
+ * **printWarn**
+
+converters Module
+-----------------
+
+ * **rst2html**
+ * **dict2matrix**
+ * **str2list**
+ * **list2str**
+ * **matrix2str**
+
+Packages
+--------
+
+ * **color**
+ * **pip**
+ * **progress**
+ * **prompt**
+ * **wcwidth**
+
+pip Package
+-----------
+
+ >this is a Advanced pip Tool, this Package has a List of all pip Packages that you can Search, Download and Install them and you can Update this List anytime you want
+
+ **Features**
+
+ >* it has built in Packages List
+ >* you can do an Offline Search
+ >* can Create Offline Repositiry
+ >* can do Batch Install or Download with built in List or use Custom List
+ >* and more...
```

### Comparing `prot-3.9.1/src/prot/__init__.py` & `prot-3.9.2/src/prot/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1789 +1,1789 @@
-import builtins as _builtins
-import hashlib as _hashlib
-import os as _os
-import py_compile as _py_compile
-import random as _random
-import runpy as _r
-import socket as _socket
-import sys as _sys
-import threading as _threading
-import time as _time
-from time import sleep as _sleep
-
-try:
-    from docutils.core import publish_file as _pf
-except:
-    _pf = None
-try:
-    from . import color as _c
-
-    Fore = _c.ansi.Fore
-    Back = _c.ansi.Back
-    Style = _c.ansi.Style
-    clear_line = _c.ansi.clear_line
-    clear_screen = _c.ansi.clear_screen
-    outWin32 = _c.ansitowin32.AnsiToWin32(_sys.stdout, convert=True)
-    _c = True
-except:
-    _c = False
-
-__all__ = ["status"]
-
-try:
-    from . import __version__ as _ver
-
-    __version__ = _ver.__version__
-except:
-    pass
-
-if hasattr(_sys, "runningPPF"):
-    PyProtFramework = True
-else:
-    PyProtFramework = False
-
-status = []
-
-if not _os.path.split(_os.path.split(__file__)[0])[1] == "prot":
-    status.append("unofficial")
-else:
-    status.append("official")
-
-if _os.path.split(_os.path.split(__file__)[0])[1] in ["lightprot", "protbuilder"]:
-    status.append("light")
-    try:
-        _prt = __import__("prot")
-        status.append("haveProt")
-    except:
-        _prt = None
-
-Empty = "empty"
-
-nameDict = {
-    "printMsg": "print",
-    "insertColor": "applycolors",
-    "cleanColor": "removecolors",
-    "getRandomString": "randomstring",
-    "checkFileSame": "checkfilesame",
-    "runAsMain": "runmoduleasmain",
-}
-
-colors = {
-    "foreground": {
-        "black": Fore.BLACK,
-        "red": Fore.RED,
-        "green": Fore.GREEN,
-        "yellow": Fore.YELLOW,
-        "blue": Fore.BLUE,
-        "magenta": Fore.MAGENTA,
-        "cyan": Fore.CYAN,
-        "white": Fore.WHITE,
-        "reset": Fore.RESET,
-    },
-    "background": {
-        "black": Back.BLACK,
-        "red": Back.RED,
-        "green": Back.GREEN,
-        "yellow": Back.YELLOW,
-        "blue": Back.BLUE,
-        "magenta": Back.MAGENTA,
-        "cyan": Back.CYAN,
-        "white": Back.WHITE,
-        "reset": Back.RESET,
-    },
-    "style": {
-        "bright": Style.BRIGHT,
-        "dim": Style.DIM,
-        "normal": Style.NORMAL,
-        "end": Style.RESET_ALL,
-        "clearline": clear_line(),
-        "clear": clear_screen(),
-    },
-}
-
-colorSymbols = {"foreground": "-", "background": "+", "style": "*"}
-
-charDict = {
-    "lowers": "abcdefghijklmnopqrstuvwxyz",
-    "uppers": "ABCDEFGHIJKLMNOPQRSTUVWXYZ",
-    "symbols": "./~!@#$%&*-_=+?",
-    "numbers": "0123456789",
-}
-
-patterns = ["%s =", "%s=", "as %s", "import %s", "%s,"]
-
-settingFilePath = _os.path.join(_os.path.split(__file__)[0], "settings")
-databaseFilePath = _os.path.join(_os.path.split(__file__)[0], "database")
-
-localSets = False
-
-settingVals = {
-    "repo": "default",
-    "ui": "normal",
-    "orderedBuiltinList": "on",
-    "saveDatabase": "off",
-    "colorize": "on",
-    "printMsgPrefix": "",
-    "printMsgColor": "",
-}
-
-settingChoices = {
-    "ui": ["verysmall", "small", "normal"],
-    "orderedBuiltinList": ["off", "on"],
-    "colorize": ["off", "on"],
-    "saveDatabase": ["off", "on"],
-    "printMsgColor": [color for color in colors["foreground"]],
-}
-
-settingData = None
-
-
-def prot(args=None):
-    if type(args) == list:
-        args = ["prot"] + args
-    elif type(args) == str:
-        args = ["prot"] + args.split(" ")
-    else:
-        args = _sys.argv
-    if not args[0] == "prot":
-        args[0] = "prot"
-    _sys.argv = args
-    _r._run_module_as_main(_sys.argv[0])
-
-
-def addBuiltins(obj, name=None, checkPPF=True):
-    if checkPPF and not PyProtFramework:
-        return obj
-    if name:
-        objname = name
-    else:
-        objname = obj.__name__
-    if objname in nameDict:
-        setattr(_builtins, nameDict[objname], obj)
-    else:
-        setattr(_builtins, objname, obj)
-    return obj
-
-
-def appendAll(obj, name=None):
-    global __add__
-    __all__.append(name if name else obj if type(obj) == str else obj.__name__)
-    return obj
-
-
-@appendAll
-def verifyColor(color, exceptionOnNot=True):
-    for c in colors["foreground"]:
-        if color == c:
-            return True
-    if exceptionOnNot:
-        raise ValueError("color not found.")
-    else:
-        return False
-
-
-@appendAll
-@addBuiltins
-def insertColor(string):
-    for c in colors:
-        for sc in colors[c]:
-            string = string.replace(colorSymbols[c] + sc, colors[c][sc])
-    return string
-
-
-@appendAll
-@addBuiltins
-def cleanColor(string):
-    for c in colors:
-        for sc in colors[c]:
-            string = string.replace(colorSymbols[c] + sc, "")
-    return string
-
-
-@appendAll
-@addBuiltins
-def getRandomString(Len=4, types=["lowers", "uppers", "symbols", "numbers"]):
-    if not type(types) == list:
-        raise TypeError("types argument must be a list object.")
-    string = ""
-    for r in range(Len):
-        string += _random.choice(str2list(charDict[_random.choice(types)]))
-    return string
-
-
-@appendAll
-def testSpeed(count):
-    progress = Progress(
-        maxVal=count,
-        msgForm="($VAL/$MAX) $TIME $PERC% completed",
-        replaces=[["$TIME", TimeWidget(milisec=True)]],
-        inline=True,
-    )
-    for c in range(count):
-        progress.next()
-    progress.newline()
-
-
-@appendAll
-def getVarFromFile(file, variable):
-    if type(file) == str:
-        file = open(file).read()
-    fileMap = file.splitlines()
-    for f in fileMap:
-        if f:
-            for t in patterns:
-                ct = t % variable
-                if ct in f:
-
-                    class tempCls:
-                        exec(f)
-
-                    res = getattr(tempCls, variable)
-                    return res
-
-
-@appendAll
-def checkMethods(obj):
-    for s in dir(obj):
-        printMsg(s + " : " + str(getattr(obj, s)))
-
-
-@appendAll
-def callMethods(obj):
-    for s in dir(obj):
-        try:
-            printMsg("result of " + s + "() is " + str(getattr(obj, s)()))
-        except:
-            printMsg("error in " + str(s) + "()")
-
-
-@appendAll
-def callMethodsWithArg(obj, arg):
-    for s in dir(obj):
-        try:
-            printMsg(
-                "result of " + s + "(" + str(arg) + ") is " + str(getattr(obj, s)(arg))
-            )
-        except:
-            printMsg("error in " + str(s) + "(" + str(arg) + ")")
-
-
-@appendAll
-@addBuiltins
-def checkFileSame(f1, f2):
-    try:
-        md5s = [_hashlib.md5(), _hashlib.md5()]
-        fs = [f1, f2]
-        for i in range(2):
-            f = open(fs[i], "rb")
-            block_size = 2**20
-            while True:
-                data = f.read(block_size)
-                if not data:
-                    break
-                md5s[i].update(data)
-            f.close()
-            md5s[i] = md5s[i].hexdigest()
-        return md5s[0] == md5s[1]
-    except:
-        return False
-
-
-@appendAll
-def splitStr(string, length):
-    out = []
-    try:
-        if len(string) > length:
-            splitDelay = len(string) // length
-            for i in range(splitDelay):
-                out.append(string[:length])
-                string = string[length:]
-            if not string == "":
-                out.append(string)
-        else:
-            out = [string]
-    except:
-        out = []
-    return out
-
-
-@appendAll
-def compileStr(string):
-    try:
-        if "." in string:
-            out = float(string)
-        else:
-            out = int(string)
-    except:
-        if string in ["True", "False", "None"]:
-            out = True if string == "True" else False if string == "False" else None
-        else:
-            out = str(string)
-    return out
-
-
-@appendAll
-def extractStr(string):
-    splittedList = string.split(",")
-    splittedDict = {}
-    splittedListNew = []
-    for i in splittedList:
-        if len(i.split(":")) > 1:
-            splittedDict[i.split(":")[0]] = i.split(":")[1]
-    for i in splittedList:
-        if len(i.split(":")) > 1:
-            for s in i.split(":"):
-                splittedListNew.append(s)
-        else:
-            splittedListNew.append(i)
-    if len(splittedListNew) == 0 and len(splittedDict) == 0:
-        raise ValueError("this string is not encoded.")
-    else:
-        data = Database()
-        for i in splittedListNew:
-            data.append(i)
-        for i in splittedDict:
-            data[i] = splittedDict[i]
-        return data
-
-
-@appendAll
-def pyCompile(source, usePEP=True, subfolders=False, deleteSource=False):
-    if _os.path.isdir(source):
-        for p in _os.listdir(source):
-            if _os.path.isdir(source + "/" + p):
-                if subfolders:
-                    pyCompile(source + "/" + p, usePEP, subfolders, deleteSource)
-            else:
-                pyCompile(source + "/" + p, usePEP, deleteSource=deleteSource)
-    if _os.path.exists(source):
-        if source.lower().endswith(".py"):
-            _py_compile.compile(
-                source, cfile=None if usePEP else source + "c", optimize=2
-            )
-            if deleteSource:
-                _os.remove(source)
-    else:
-        printErr("file or folder " + source + " not found.")
-        return
-
-
-@appendAll
-@addBuiltins
-def condition(string):
-    exec("res = " + string)
-    return res
-
-
-@appendAll
-@addBuiltins
-def runAsMain(args=None):
-    if type(args) == list:
-        pass
-    elif type(args) == str:
-        args = args.split(" ")
-    else:
-        args = _sys.argv
-    _sys.argv = args
-    _r._run_module_as_main(_sys.argv[0])
-
-
-@appendAll
-@addBuiltins
-def printMsg(msg="", color=None, end="\n", file=None, colorize=True, prefix=True):
-    global _c
-    try:
-        if "light" in status and "haveProt" in status and _prt is not None:
-            settings.colorize = _prt.settings.colorize
-    except:
-        pass
-    if settings.colorize == "off" or not _sys.stdout == _sys.__stdout__:
-        _c = False
-    if prefix and settings.printMsgPrefix:
-        msg = str(settings.printMsgPrefix) + str(msg)
-    else:
-        msg = str(msg)
-    if color and verifyColor(color):
-        msg = "-" + color + msg + "*end"
-    elif settings.printMsgColor:
-        msg = "-" + settings.printMsgColor + msg + "*end"
-    if colorize:
-        if settings.colorize == "off":
-            msg = cleanColor(msg)
-        elif not _os.name == "nt" or _c:
-            msg = insertColor(msg)
-        else:
-            msg = cleanColor(msg)
-    if file is None:
-        if _os.name == "nt" and _c:
-            out = outWin32
-        else:
-            out = _sys.stdout
-    else:
-        out = file
-    out.write(msg + end)
-    try:
-        out.flush()
-    except:
-        pass
-
-
-@appendAll
-def printErr(msg):
-    printMsg("ERROR: " + str(msg), color="red")
-
-
-@appendAll
-def printWarn(msg):
-    printMsg("WARNING: " + str(msg), color="yellow")
-
-
-@appendAll
-def getLocalIP():
-    sock = _socket.socket(_socket.AF_INET, _socket.SOCK_DGRAM)
-    try:
-        sock.connect(("10.255.255.255", 1))
-        ip = sock.getsockname()[0]
-    except:
-        ip = "127.0.0.1"
-    finally:
-        sock.close()
-    return ip
-
-
-@appendAll
-def checkAvail(address, timeout=0.5):
-    sock = _socket.socket()
-    sock.settimeout(timeout)
-    try:
-        sock.connect(address)
-        sock.close()
-        return True
-    except:
-        return False
-
-
-@appendAll
-def getBaseAddr(address):
-    return ".".join(address.split(".")[:3])
-
-
-@appendAll
-def netScan(port=80, timeout=0.5):
-    ports = port if type(port) == list else [port]
-    baseAddr = getBaseAddr(getLocalIP())
-    hostsAvail = []
-    for n in range(256):
-        host = baseAddr + "." + str(n)
-        for p in ports:
-            if checkAvail((host, p), timeout):
-                hostsAvail.append((host, p))
-    return hostsAvail
-
-
-@appendAll
-def netAttack(addr, times):
-    val1 = ValueWidget(" starting")
-    prog = Progress(
-        maxVal=times * 2, msgForm="$PERC% $MSG$1", replaces=[["$1", val1]], inline=True
-    )
-    for t in range(times):
-        val1.value = " connecting to " + str(addr[0]) + ":" + str(addr[1])
-        prog.next()
-        sock = _socket.socket()
-        sock.connect(addr)
-        val1.value = " disconnecting from " + str(addr[0]) + ":" + str(addr[1])
-        prog.next()
-        sock.close()
-    val1.value = ""
-    prog.show()
-    prog.newline()
-
-
-@appendAll
-@addBuiltins
-class Matrix(list):
-    def __getitem__(self, key):
-        if type(key) == int:
-            return list.__getitem__(self, key)
-        else:
-            res = self.get(key, default=Empty)
-            if res == Empty:
-                raise KeyError(key)
-            return res
-
-    def __setitem__(self, key, value):
-        self._checkValue(value)
-        if type(key) == int:
-            list.__setitem__(self, key, value)
-        else:
-            self.append([key, value])
-
-    def __init__(self, value=[]):
-        try:
-            if value:
-                self._checkValue(value)
-        except:
-            for v in value:
-                self._checkValue(v)
-        list.__init__(self, value)
-
-    def _checkValue(self, value):
-        if type(value) in [list, tuple, Matrix] and len(value) == 2:
-            return True
-        raise ValueError(
-            "value must be object of Matrix, list or tuple classes and should have only two members"
-        )
-
-    def append(self, value):
-        self._checkValue(value)
-        list.append(self, value)
-
-    def __delitem__(self, key):
-        if type(key) == int:
-            list.__delitem__(self, key)
-        for k in self:
-            try:
-                if k[0] == key:
-                    self.remove(k)
-            except:
-                pass
-
-    def get(self, key, default=None):
-        for k in self:
-            try:
-                if k[0] == key:
-                    return k[1]
-            except:
-                pass
-        return default
-
-
-@appendAll
-def rst2html(path, subdirs=False):
-    if _pf is None:
-        printErr("docutils package needed.")
-        return
-    if _os.path.isdir(path):
-        for p in _os.listdir(path):
-            if _os.path.isdir(path + "/" + p):
-                if subdirs:
-                    rst2html(path + "/" + p, True)
-            else:
-                rst2html(path + "/" + p)
-    if _os.path.exists(path):
-        if path.endswith(".rst"):
-            try:
-                _pf(
-                    source_path=path,
-                    destination_path=path.split(".rst")[0] + ".html",
-                    writer_name="html",
-                )
-            except:
-                import traceback
-
-                traceback.print_stack()
-                traceback.print_exc()
-    else:
-        printErr("file or folder " + path + " not found.")
-        return
-
-
-@appendAll
-def dict2matrix(obj):
-    if not type(obj) == dict:
-        raise TypeError("dict object is required.")
-    matrix = []
-    for m in obj:
-        if type(obj[m]) == dict:
-            matrix.append([m, dict2matrix(obj[m])])
-        else:
-            matrix.append(Matrix([m, obj[m]]))
-    return Matrix(matrix)
-
-
-@appendAll
-def str2list(string):
-    if not type(string) == str:
-        raise TypeError("str object is required.")
-    strList = []
-    for s in string:
-        strList.append(s)
-    return strList
-
-
-@appendAll
-def list2str(listObj, space=""):
-    if not type(listObj) == list:
-        raise TypeError("list object is required.")
-    string = ""
-    for s in listObj:
-        if string:
-            string += space
-        string += str(s)
-    return string
-
-
-@appendAll
-def matrix2str(mat, space=""):
-    if not type(mat) in [list, Matrix]:
-        raise TypeError("list or Matrix object is required.")
-    string = ""
-    for m in mat:
-        if string:
-            string += space
-        if type(m) in [list, Matrix]:
-            string += str(matrix2str(m))
-        elif type(m) == dict:
-            string += str(matrix2str(dict2matrix(m)))
-        else:
-            string += str(m)
-    return string
-
-
-@appendAll
-@addBuiltins
-class LoopBack(object):
-    def _back(*args, **kwargs):
-        pass
-
-    def __getattribute__(self, key):
-        try:
-            return object.__getattribute__(self, key)
-        except:
-            return self._back
-
-
-@appendAll
-@addBuiltins
-class Database(object):
-    def __getattribute__(self, val):
-        try:
-            return object.__getattribute__(self, val)
-        except:
-            return self.dict[val]
-
-    def __setattr__(self, key, val):
-        if str(key).startswith("_") or str(key) in [
-            "append",
-            "add",
-            "remove",
-            "dict",
-            "list",
-        ]:
-            object.__setattr__(self, key, val)
-        else:
-            self.dict[key] = val
-
-    def __delattr__(self, val):
-        try:
-            del self.dict[val]
-        except:
-            object.__delattr__(self, val)
-
-    def __getitem__(self, val):
-        return self.list[val] if type(val) == int else self.dict[val]
-
-    def __setitem__(self, key, val):
-        self.dict[key] = val
-
-    def __delitem__(self, val):
-        del self.dict[val]
-
-    def __repr__(self):
-        return str(object.__repr__(self)).replace(
-            str(str(object.__repr__(self)).split()[0]), "<Database"
-        )
-
-    def __init__(self, update=None):
-        self.dict = {} if not type(update) == dict else update
-        self.list = [] if not type(update) == list else update
-
-    def append(self, val):
-        self.list.append(val)
-
-    def add(self, val):
-        if len(str(val).split(":")) == 1:
-            self.list.append(val)
-        else:
-            self.dict[str(val).split(":")[0]] = str(val).split(":")[1]
-
-    def remove(self, val):
-        self.list.remove(val)
-
-
-@appendAll
-@addBuiltins
-class OptionsDatabase(Database):
-    def __getitem__(self, val):
-        return self.dict[val]
-
-    def __repr__(self):
-        return str(object.__repr__(self)).replace(
-            str(str(object.__repr__(self)).split()[0]), "<OptionsDatabase"
-        )
-
-    def __add__(self, other):
-        if not type(other) == OptionsDatabase:
-            raise TypeError(
-                f'can only concatenate OptionsDatabase (not "{type(other).__name__}") to OptionsDatabase'
-            )
-        newDict = {}
-        for k in self.dict:
-            newDict[k] = self.dict[k]
-        for k in other.dict:
-            newDict[k] = other.dict[k]
-        return OptionsDatabase(newDict)
-
-    def __init__(self, update=None, rules=None, allowExtraArgs=True):
-        self.dict = {} if not type(update) == dict else update
-        if rules:
-            for i, o in enumerate(rules):
-                if type(update) == tuple:
-                    try:
-                        if o.get("position", Empty) is Empty:
-                            self.dict[o["key"]] = update[i]
-                        else:
-                            self.dict[o["key"]] = update[o["position"]]
-                    except:
-                        raise Exception(f"argument '{o['key']}' is required.")
-                if not o["key"] in self.dict:
-                    if o.get("required", False):
-                        raise Exception(f"argument '{o['key']}' is required.")
-                    self.dict[o["key"]] = o.get("default", None)
-                if o.get("allowed", Empty) is not Empty:
-                    if not self.dict[o["key"]] in (
-                        o["allowed"] if type(o["allowed"]) == list else [o["allowed"]]
-                    ):
-                        raise Exception(f"value of argument '{o['key']}' is invalid.")
-                if o.get("denied", Empty) is not Empty:
-                    if self.dict[o["key"]] in (
-                        o["denied"] if type(o["denied"]) == list else [o["denied"]]
-                    ):
-                        raise Exception(f"value of argument '{o['key']}' is invalid.")
-                if o.get("type", Empty) is not Empty:
-                    if not type(self.dict[o["key"]]) == o["type"]:
-                        raise Exception(
-                            f"argument '{o['key']}' must be an {o['type'].__name__} object."
-                        )
-                if o.get("call", Empty) is not Empty:
-                    o["call"](self.dict[o["key"]])
-                if o.get("update", Empty) is not Empty:
-                    self.dict[o["key"]] = o["update"](self.dict[o["key"]])
-
-        if not allowExtraArgs:
-            ruleKeys = [o["key"] for o in rules]
-            for k in self.dict:
-                if not k in ruleKeys:
-                    raise Exception(f"argument '{k}' not requested.")
-
-
-@appendAll
-@addBuiltins
-class TextListFile(object):
-    def __init__(self, filePath, newFile=None):
-        self.file = open(filePath)
-        self.rawdata = self.file.read()
-        self.data = self.rawdata.splitlines()
-        if newFile:
-            self.newfile = open(newFile, "w")
-            self.mode = "w"
-        else:
-            self.newfile = None
-            self.mode = "r"
-
-    def optimize(self):
-        new = []
-        for s in self.data:
-            if s in new or not s:
-                continue
-            else:
-                new.append(s)
-        self.data = new
-
-    def commit(self):
-        if self.mode == "r":
-            raise Exception("can't write in read mode.")
-        self.newfile.write(list2str(self.data, "\n"))
-        self.newfile.flush()
-
-    def close(self):
-        if self.mode == "w":
-            self.newfile.close()
-        self.file.close()
-
-
-@appendAll
-@addBuiltins
-class TextDictFile(object):
-    def __init__(self, filePath, newFile=None, createFile=False):
-        if createFile and not _os.path.exists(filePath):
-            open(filePath, "w").close()
-            newFile = filePath
-        self.file = open(filePath)
-        self.rawdata = self.file.read()
-        lines = self.rawdata.splitlines()
-        if not self.checkFormat(lines):
-            raise TypeError("file type not supported.")
-        self.data = {}
-        for l in lines:
-            data = Database()
-            for d, v in {
-                "key": l.split(":")[0].strip(),
-                "val": l.split(":")[1].strip(),
-            }.items():
-                try:
-                    if "." in v:
-                        v = float(v)
-                    else:
-                        v = int(v)
-                except:
-                    if v in ["True", "False", "None"]:
-                        v = True if v == "True" else False if v == "False" else None
-                    else:
-                        v = str(v)
-                setattr(data, d, v)
-            self.data[data.key] = data.val
-        if newFile:
-            self.newfile = open(newFile, "w")
-            self.mode = "w"
-        else:
-            self.newfile = None
-            self.mode = "r"
-
-    def checkFormat(self, data):
-        for d in data:
-            if not d:
-                continue
-            if d.startswith("#"):
-                continue
-            if not ":" in d or not len(d.split(":")) == 2:
-                return False
-        return True
-
-    def commit(self):
-        if self.mode == "r":
-            raise Exception("can't write in read mode.")
-        self.newfile.write(list2str(self.convert(), "\n"))
-        self.newfile.flush()
-
-    def convert(self, data=None):
-        out = []
-        if not data:
-            data = self.data
-        for d in data:
-            out.append(str(d) + " : " + str(data[d]))
-        return out
-
-    def close(self):
-        if self.mode == "w" and not self.newfile.closed:
-            self.newfile.close()
-        if not self.file.closeed:
-            self.file.close()
-
-
-def load_settings():
-    global settingData
-    if localSets:
-        if not "light" in status:
-            printWarn(
-                "can't create settings file because permission denied, using default settings"
-            )
-        settingData = settingVals
-        return settingVals
-    if not _os.path.exists(settingFilePath):
-        raise FileNotFoundError("settings file not found.")
-    else:
-        settingFile = open(settingFilePath)
-        data = read_settings(settingFile.read().splitlines())
-        settingFile.close()
-        settingData = data
-        return data
-
-
-def read_settings(data):
-    out = {}
-    for d in data:
-        extract = d.split(":")
-        out[extract[0]] = extract[1]
-    return out
-
-
-def convert_settings(data):
-    string = ""
-    for s in data:
-        string += s + ":" + str(data[s]) + "\n"
-    return string
-
-
-def setup_settings():
-    global localSets
-    if "light" in status:
-        localSets = True
-        return
-    if not _os.path.exists(settingFilePath):
-        try:
-            settingFile = open(settingFilePath, "w")
-            settingFile.write(convert_settings(settingVals))
-            settingFile.flush()
-            settingFile.close()
-        except PermissionError:
-            localSets = True
-    else:
-        data = load_settings()
-        updated = False
-        for s in settingVals:
-            if not s in data:
-                data[s] = settingVals[s]
-                updated = True
-        if updated:
-            try:
-                settingFile = open(settingFilePath, "w")
-                settingFile.write(convert_settings(data))
-                settingFile.flush()
-                settingFile.close()
-            except PermissionError:
-                localSets = True
-
-
-class Settings(object):
-    def __init__(self):
-        if settingData:
-            self._data = settingData
-        else:
-            self._data = load_settings()
-
-    def _reset(self):
-        self._data = settingVals
-        self._write()
-
-    def _write(self):
-        if "light" in status:
-            return
-        global localSets
-        try:
-            self._file = open(settingFilePath, "w")
-            self._file.write(convert_settings(self._data))
-            self._file.flush()
-            self._file.close()
-        except PermissionError:
-            localSets = True
-
-    def __getattr__(self, key):
-        if not key.startswith("_"):
-            try:
-                if key == "reset":
-                    self._reset()
-                    printMsg("settings restored to default values")
-                    return
-                return self._data[key]
-            except KeyError:
-                printMsg("KeyError: " + "'" + key + "'", color="red")
-                return
-        else:
-            return object.__getattribute__(self, key)
-
-    def __setattr__(self, key, val):
-        if not key.startswith("_"):
-            if not key in settingVals:
-                printErr("option is invalid")
-                return
-            if key in settingChoices and not val in settingChoices[key]:
-                printErr("value is invalid")
-                return
-            self._data[key] = val
-            self._write()
-        else:
-            object.__setattr__(self, key, val)
-
-
-setup_settings()
-settings = appendAll(Settings(), "settings")
-
-
-class ProtectedDict(dict):
-    def __init__(self, *args, **kwargs):
-        dict.__init__(self, *args, **kwargs)
-        if settings.saveDatabase == "on" and not localSets:
-            if not _os.path.exists(databaseFilePath):
-                self.dataFile = TextDictFile(databaseFilePath, createFile=True)
-                self.dataFile.file.close()
-            else:
-                self.dataFile = TextDictFile(databaseFilePath, databaseFilePath)
-                self.dataFile.commit()
-                self.dataFile.file.close()
-                for d in self.dataFile.data:
-                    dict.__setitem__(self, d, self.dataFile.data[d])
-        else:
-            self.dataFile = None
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__}>"
-
-    def __setitem__(self, key, val):
-        raise TypeError("can't change ProtectedDict contents")
-
-    def __getitem__(self, key):
-        raise TypeError("can't see ProtectedDict contents")
-
-    def __delitem__(self, key):
-        raise TypeError("can't change ProtectedDict contents")
-
-
-@appendAll
-@addBuiltins
-class SecureDatabase(object):
-    def __init__(self, id, data={}, replace=False, clearOnDelete=False):
-        self.id = id
-        if not hasID(id) or replace:
-            setID(id, data, False)
-        self.data = getID(id)
-        self.dataType = type(self.data)
-        self.CON = clearOnDelete
-
-    def __repr__(self):
-        return self.data.__repr__()
-
-    def __str__(self):
-        return self.data.__str__()
-
-    def __add__(self, other):
-        return self.data.__add__(other)
-
-    def __format__(self):
-        return self.data.__format__()
-
-    def __len__(self):
-        return self.data.__len__()
-
-    def __eq__(self, other):
-        return self.data.__eq__(other)
-
-    def __ge__(self, other):
-        return self.data.__ge__(other)
-
-    def __gt__(self, other):
-        return self.data.__gt__(other)
-
-    def __hash__(self):
-        return self.data.__hash__()
-
-    def __iter__(self):
-        return self.data.__iter__()
-
-    def __ne__(self, other):
-        return self.data.__ne__(other)
-
-    def __truediv__(self, other):
-        return self.data.__truediv__(other)
-
-    def __rtruediv__(self, other):
-        return self.data.__rtruediv__(other)
-
-    def __div__(self, other):
-        return self.data.__div__(other)
-
-    def __sub__(self, other):
-        return self.data.__sub__(other)
-
-    def __mul__(self, other):
-        return self.data.__mul__(other)
-
-    def __rmul__(self, other):
-        return self.data.__rmul__(other)
-
-    def __rsub__(self, other):
-        return self.data.__rsub__(other)
-
-    def __le__(self, other):
-        return self.data.__le__(other)
-
-    def __lt__(self, other):
-        return self.data.__lt__(other)
-
-    def __del__(self):
-        if self.CON:
-            delID(self.id)
-
-    def __setitem__(self, key, val):
-        self.data.__setitem__(key, val)
-        self.update()
-
-    def __getitem__(self, key):
-        return self.data.__getitem__(key)
-
-    def __delitem__(self, key):
-        self.data.__delitem__(key)
-        self.update()
-
-    def __setattr__(self, key, val):
-        object.__setattr__(self, key, val)
-        if key == "data":
-            self.dataType = type(self.data)
-            self.update()
-
-    def update(self):
-        setID(self.id, self.data, False)
-
-
-@appendAll
-def getID(id, default=None):
-    global database
-    try:
-        return dict.__getitem__(database, id)
-    except KeyError:
-        return default
-
-
-@appendAll
-def hasID(id):
-    global database
-    return id in database
-
-
-@appendAll
-def setID(id, data, exceptOnDup=True):
-    global database
-    if hasID(id):
-        if exceptOnDup:
-            raise TypeError("can't set duplicate id.")
-    dict.__setitem__(database, id, data)
-    if database.dataFile is not None:
-        database.dataFile.newfile.write(
-            list2str(database.dataFile.convert({id: data})) + "\n"
-        )
-        database.dataFile.newfile.flush()
-
-
-@appendAll
-def delID(id):
-    global database
-    dict.__delitem__(database, id)
-
-
-database = ProtectedDict()
-
-
-class TimerThread(_threading.Thread):
-    def __init__(self, id, time, call, repeat=False):
-        _threading.Thread.__init__(self)
-        self.id = id
-        self.time = time
-        self.call = call
-        self.repeat = repeat
-
-    def run(self):
-        run = True
-        while run:
-            if getID(self.id, "stopped") == "stopped":
-                break
-            _time.sleep(self.time)
-            if getID(self.id, "stopped") == "stopped":
-                break
-            if callable(self.call):
-                self.call()
-            if not self.repeat:
-                run = False
-        delID(self.id)
-
-
-@appendAll
-@addBuiltins
-class Timer(object):
-    def __init__(self, time, call, repeat=False, type="background"):
-        self.type = type
-        if str(time)[-1] in ["s", "m", "h"]:
-            unit = str(time)[-1]
-            time = float(str(time)[:-1])
-            if unit in ["m", "h"]:
-                time = time * 60
-            if unit in ["h"]:
-                time = time * 60
-        time = float(time)
-        self.id = int(getRandomString(10, ["numbers"]))
-        setID(self.id, "started", False)
-        thread = TimerThread(self.id, time, call, repeat)
-        if type == "background":
-            thread.daemon = True
-            thread.start()
-        elif type == "foreground":
-            thread.run()
-        else:
-            printErr("type is invalid")
-
-    def __repr__(self):
-        return f'<{self.__class__.__name__} {getID(self.id, "stopped")} ID={str(self.id) if hasID(self.id) else str(None)}>'
-
-    def __del__(self):
-        setID(self.id, "stopped", False)
-
-
-@appendAll
-@addBuiltins
-class Call(object):
-    def __init__(self, *args, **keywds):
-        self.call = args[0]
-        self.args = args[1:]
-        self.keywds = keywds
-
-    def __call__(self, *argsExtra):
-        return self.call(*self.args + argsExtra, **self.keywds)
-
-    def __repr__(self):
-        return (
-            "<Call object call="
-            + str(self.call)
-            + " args="
-            + str(self.args)
-            + " keywds="
-            + str(self.keywds)
-            + ">"
-        )
-
-
-@appendAll
-@addBuiltins
-class Widget(object):
-    def __init__(self, progressNeeded=False):
-        self.reprMsg = "<$name Widget>".replace("$name", str(self.__class__.__name__))
-        self.progress = None
-        self._finished = False
-        self.progressNeeded = progressNeeded
-
-    def _set_progress(self, progress):
-        if not isinstance(progress, Progress):
-            raise TypeError(str(progress) + " must be instance of " + str(Progress))
-        self.progress = progress
-
-    def _finish(self):
-        self._finished = True
-
-    def __repr__(self):
-        return self.reprMsg
-
-    def __call__(self):
-        if self.progressNeeded and self.progress is None:
-            raise Exception("progress instance needed.")
-
-
-@appendAll
-@addBuiltins
-class TimeWidget(Widget):
-    def __init__(self, milisec=False, min=True, hour=True):
-        Widget.__init__(self)
-        self.milisec = milisec
-        self.min = min
-        self.hour = hour
-        self._startTime = _time.time()
-        self.startTime = int(self._startTime)
-
-    def calc_time(self):
-        _now = _time.time()
-        now = int(_now)
-        string = ""
-        if self.milisec:
-            milisec = str(_now - self._startTime).split(".")[1][:3]
-        sec = now - self.startTime
-        min = 0
-        hour = 0
-        if sec >= 60 and self.min:
-            for m in range(sec // 60):
-                sec -= 60
-                min += 1
-        if min >= 60 and self.hour:
-            for m in range(min // 60):
-                min -= 60
-                hour += 1
-        if len(str(hour)) <= 1:
-            hour = "0" + str(hour)
-        if len(str(min)) <= 1:
-            min = "0" + str(min)
-        if len(str(sec)) <= 1:
-            sec = "0" + str(sec)
-        if self.hour:
-            string += str(hour) + ":"
-        if self.min:
-            string += str(min) + ":"
-        if self.milisec:
-            sec = str(sec) + "." + milisec
-        string += str(sec)
-        return string
-
-    def __call__(self):
-        Widget.__call__(self)
-        return self.calc_time()
-
-
-@appendAll
-@addBuiltins
-class BarWidget(Widget):
-    def __init__(self, fill="█", empty="░", fillPerPercent=5, color=None):
-        Widget.__init__(self, True)
-        self.fill = fill
-        self.empty = empty
-        self.fpp = fillPerPercent
-        self.color = color
-
-    def __call__(self):
-        Widget.__call__(self)
-        return self.createBar()
-
-    def createBar(self):
-        perc = int(self.progress.calc_perc().split(".")[0])
-        bar = ""
-        filled = 0
-        if perc >= self.fpp:
-            for c in range(perc // self.fpp):
-                bar += self.fill
-                filled += 1
-        for f in range(100 // self.fpp - filled):
-            bar += self.empty
-        if self.color and verifyColor(self.color, False):
-            bar = "-" + self.color + bar + "*end"
-
-        return bar
-
-
-@appendAll
-@addBuiltins
-class TaskWidget(Widget):
-    def __init__(self, tasks={}):
-        Widget.__init__(self, True)
-        self.tasks = tasks
-        self.percTasks = {}
-        self.eventTasks = {}
-        self.firstRun = True
-        self.checkTasks()
-
-    def checkTasks(self):
-        for t in self.tasks:
-            if t == "perc":
-                self.percTasks = self.tasks[t]
-            elif t == "event":
-                self.eventTasks = self.tasks[t]
-
-    def __call__(self):
-        Widget.__call__(self)
-        return calc_task()
-
-    def calc_task(self):
-        if self.eventTasks:
-            if "onFirstShow" in self.eventTasks and self.firstRun:
-                self.firstRun = False
-                return self.eventTasks["onFirstShow"]
-            if "onFinish" in self.eventTasks and self._finished:
-                return self.eventTasks["onFinish"]
-        if self.percTasks:
-            perc = int(self.progress.calc_true_perc())
-            for p in self.percTasks:
-                if perc <= p:
-                    return self.percTasks[p]
-        return ""
-
-
-@appendAll
-@addBuiltins
-class CallWidget(Widget):
-    def __init__(self, call, progressNeeded=False):
-        Widget.__init__(self, progressNeeded)
-        self.call = call
-
-    def __call__(self):
-        Widget.__call__(self)
-        if self.progressNeeded:
-            return self.call(self.progress)
-        else:
-            return self.call()
-
-
-@appendAll
-@addBuiltins
-class ValueWidget(Widget):
-    def __init__(self, value):
-        Widget.__init__(self)
-        self.value = value
-
-    def __call__(self):
-        Widget.__call__(self)
-        return self.value
-
-
-@appendAll
-@addBuiltins
-class LoadingWidget(Widget):
-    def __init__(self, type="default"):
-        Widget.__init__(self)
-        self.type = type
-        self.index = 0
-        self.msg = None
-        self.loadingType = None
-        self.handleType()
-
-    def handleType(self):
-        typeData = self.getTypes()[self.type]
-        self.msg = typeData["data"]
-        self.loadingType = type(typeData["data"])
-        if self.loadingType == str:
-            self.msg = ProtString(self.msg)
-
-    def createMsg(self):
-        if self._finished:
-            return "done"
-        if self.loadingType == list:
-            msg = self.msg[self.index]
-            if self.index + 1 == len(self.msg):
-                self.index = 0
-            else:
-                self.index += 1
-            return msg
-        else:
-            msg = self.msg
-            end = self.msg[-1]
-            del self.msg[-1]
-            self.msg = self.msg.query
-            self.msg = ProtString(end + str(self.msg))
-            return msg
-
-    def __call__(self):
-        Widget.__call__(self)
-        return self.createMsg()
-
-    def getTypes(self):
-        return {
-            "default": {"data": ["|", "-"]},
-            "bar": {"data": "█████               "},
-            "smallbar": {"data": "███         "},
-            "verysmallbar": {"data": "██      "},
-        }
-
-
-@appendAll
-@addBuiltins
-class LockedDict(dict):
-    def __delitem__(self, val):
-        raise TypeError("dict is locked.")
-
-    def __setitem__(self, key, val):
-        raise TypeError("dict is locked.")
-
-
-@appendAll
-@addBuiltins
-class Progress(object):
-    _deafultForm = "($VAL/$MAX) $PERC% $MSG"
-
-    def __init__(
-        self,
-        val=0,
-        minVal=0,
-        maxVal=100,
-        msg="completed",
-        msgForm=None,
-        replaces=[],
-        color=None,
-        inline=False,
-    ):
-        self._finished = False
-        self.val = val
-        self.min = minVal
-        self.max = maxVal
-        self.msg = msg
-        self.inline = (
-            inline
-            if _sys.stdout == _sys.__stdout__ and (not _os.name == "nt" or _c)
-            else False
-        )
-        self.color = color
-        if not msgForm:
-            self.msgForm = self.get_default_form()
-        else:
-            self.msgForm = msgForm
-        if replaces:
-            for r in replaces:
-                if not isinstance(r[1], Widget):
-                    raise TypeError(str(r[1]) + " must be instance of Widget")
-                r[1]._set_progress(self)
-            self.extraReplaces = replaces
-        else:
-            self.extraReplaces = []
-        self.show()
-
-    def show(self):
-        replaces = self.getDefaultReplaces()
-        msg = self.do_replace(replaces)
-        if self.color and verifyColor(self.color, False):
-            msg = "-" + self.color + msg + "*end"
-        if self.inline:
-            self.printInline(msg)
-        else:
-            printMsg(msg)
-
-    def getDefaultReplaces(self):
-        return [
-            ["$VAL", self.val],
-            ["$MIN", self.min],
-            ["$MAX", self.max],
-            ["$PERC", self.calc_perc()],
-            ["$TRUE_PERC", self.calc_true_perc()],
-            ["$MSG", self.msg],
-        ]
-
-    def clear(self):
-        printMsg("\r\x1b[K", end="", prefix=False)
-
-    def printInline(self, msg):
-        self.clear()
-        printMsg(msg, end="")
-
-    def write(self, msg=""):
-        if self.inline:
-            printMsg("\n" + msg)
-        else:
-            printMsg(msg)
-
-    def newline(self):
-        if self.inline:
-            printMsg("", prefix=False)
-
-    def finish(self):
-        for r in self.extraReplaces:
-            r[1]._finish()
-        self._finished = True
-        self.newline()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.finish()
-
-    def get_default_form(self):
-        return self._deafultForm
-
-    def calc_perc(self):
-        perc = str(100 / self.max * self.val).split(".")
-        perc[1] = perc[1][:3]
-        return perc[0] + "." + perc[1]
-
-    def calc_true_perc(self):
-        perc = str(100 / self.max * self.val).split(".")[0]
-        return perc
-
-    def do_replace(self, rl):
-        cf = self.msgForm if not hasattr(self, "tempMsg") else self.tempMsg
-        for r in rl:
-            cf = cf.replace(r[0], str(r[1]))
-        for r in self.extraReplaces:
-            cf = cf.replace(r[0], str(r[1]()))
-        if "$" in cf and not hasattr(self, "tempMsg"):
-            self.tempMsg = cf
-            self.do_replace(rl)
-        else:
-            try:
-                del self.tempMsg
-            except:
-                pass
-            return cf
-
-    def update(self, val):
-        self.val = max(self.min, min(self.max, val))
-        self.show()
-
-    def next(self, val=1):
-        self.val = max(self.min, min(self.max, self.val + val))
-        self.show()
-
-
-@appendAll
-@addBuiltins
-class ProgressBar(Progress, BarWidget):
-    def __init__(
-        self,
-        val=0,
-        minVal=0,
-        maxVal=100,
-        msg="completed",
-        msgForm=None,
-        replaces=[],
-        color=None,
-        inline=False,
-        fill="█",
-        empty="░",
-        fillPerPercent=5,
-    ):
-        BarWidget.__init__(self, fill=fill, empty=empty, fillPerPercent=fillPerPercent)
-        Progress.__init__(
-            self,
-            val=val,
-            minVal=minVal,
-            maxVal=maxVal,
-            msg=msg,
-            msgForm=msgForm,
-            replaces=replaces,
-            color=color,
-            inline=inline,
-        )
-        self.progress = self
-
-    def __repr__(self):
-        return object.__repr__(self)
-
-    def getDefaultReplaces(self):
-        Progress.getDefaultReplaces(self) + [["$BAR", self()]]
-
-    def finish(self):
-        self._finish()
-        Progress.finish(self)
-
-
-@appendAll
-@addBuiltins
-class VersionString(str):
-    def __init__(self, *args, **kwargs):
-        str.__init__(self)
-        try:
-            ver = self.split(".")
-            try:
-                self.major = int(ver[0])
-            except:
-                self.major = None
-            try:
-                self.minor = int(ver[1])
-            except:
-                self.minor = None
-            try:
-                self.micro = int(ver[2])
-            except:
-                self.micro = None
-        except:
-            pass
-
-    def upgrade(self, target="default", maxMinor=9, maxMicro=9):
-        if target == "default":
-            if self.micro is not None:
-                target = "micro"
-            elif self.minor is not None:
-                target = "minor"
-            elif self.major is not None:
-                target = "major"
-        if self.micro is not None and self.micro >= maxMicro:
-            minor = True
-        else:
-            minor = False
-        if self.minor is not None and self.minor >= maxMinor:
-            major = True
-        else:
-            major = False
-        if False:
-            print(f"target: {str(target)}")
-            print(f"self.micro: {str(self.micro)}")
-            print(f"maxMicro: {str(maxMicro)}")
-            print(f"self.minor: {str(self.minor)}")
-            print(f"maxMinor: {str(maxMinor)}")
-            print(f"minor: {str(minor)}")
-            print(f"self.major: {str(self.major)}")
-            print(f"major: {str(major)}")
-        if self.micro is not None and target == "micro":
-            self.micro += 1
-        if self.minor is not None and (target == "minor" or minor) and not major:
-            if self.micro is not None:
-                self.micro = 0
-            self.minor += 1
-        if self.major is not None and (target == "major" or (major and minor)):
-            if self.micro is not None:
-                self.micro = 0
-            if self.minor is not None:
-                self.minor = 0
-            self.major += 1
-        return self.compile()
-
-    def compile(self):
-        ver = []
-        if self.major is not None:
-            ver.append(str(self.major))
-        if self.minor is not None:
-            ver.append(str(self.minor))
-        if self.micro is not None:
-            ver.append(str(self.micro))
-        return ".".join(ver)
-
-
-@appendAll
-@addBuiltins
-class ProtString(str):
-    def compile(self):
-        try:
-            if "." in self:
-                out = float(self)
-            else:
-                out = int(self)
-        except:
-            if self in ["True", "False", "None"]:
-                out = True if self == "True" else False if self == "False" else None
-            else:
-                out = str(self)
-        return out
-
-    @property
-    def type(self):
-        return self.split(".")[-1].lower()
-
-    @property
-    def has_type(self):
-        return len(self.split(".")) > 1
-
-    def extract(self):
-        splittedList = self.split(",")
-        splittedDict = {}
-        splittedListNew = []
-        for i in splittedList:
-            if len(i.split(":")) > 1:
-                splittedDict[i.split(":")[0]] = i.split(":")[1]
-        for i in splittedList:
-            if len(i.split(":")) > 1:
-                for s in i.split(":"):
-                    splittedListNew.append(s)
-            else:
-                splittedListNew.append(i)
-        if len(splittedListNew) == 0 and len(splittedDict) == 0:
-            raise ValueError("this string is not encoded.")
-        else:
-            data = Database()
-            for i in splittedListNew:
-                data.append(i)
-            for i in splittedDict:
-                data[i] = splittedDict[i]
-            return data
-
-    def __setitem__(self, index, val):
-        stringList = []
-        for string in self:
-            stringList.append(string)
-        stringList[index] = str(val)
-        compiledString = ""
-        for string in stringList:
-            compiledString += string
-        self.query = self.__class__(compiledString)
-
-    def __delitem__(self, key):
-        stringList = []
-        for string in self:
-            stringList.append(string)
-        del stringList[key]
-        compiledString = ""
-        for string in stringList:
-            compiledString += string
-        self.query = self.__class__(compiledString)
-
-    def __div__(self, other):
-        out = []
-        try:
-            if len(self) > other:
-                splitDelay = len(self) // other
-                tStr = str(self)
-                for i in range(splitDelay):
-                    out.append(tStr[:other])
-                    tStr = tStr[other:]
-                if not tStr == "":
-                    out.append(tStr)
-            else:
-                out = [self]
-        except:
-            out = []
-        return out
+import builtins as _builtins
+import hashlib as _hashlib
+import os as _os
+import py_compile as _py_compile
+import random as _random
+import runpy as _r
+import socket as _socket
+import sys as _sys
+import threading as _threading
+import time as _time
+from time import sleep as _sleep
+
+try:
+    from docutils.core import publish_file as _pf
+except:
+    _pf = None
+try:
+    import colorama as _c
+
+    Fore = _c.ansi.Fore
+    Back = _c.ansi.Back
+    Style = _c.ansi.Style
+    clear_line = _c.ansi.clear_line
+    clear_screen = _c.ansi.clear_screen
+    outWin32 = _c.ansitowin32.AnsiToWin32(_sys.stdout, convert=True)
+    _c = True
+except:
+    _c = False
+
+__all__ = ["status"]
+
+try:
+    from . import __version__ as _ver
+
+    __version__ = _ver.__version__
+except:
+    pass
+
+if hasattr(_sys, "runningPPF"):
+    PyProtFramework = True
+else:
+    PyProtFramework = False
+
+status = []
+
+if not _os.path.split(_os.path.split(__file__)[0])[1] == "prot":
+    status.append("unofficial")
+else:
+    status.append("official")
+
+if _os.path.split(_os.path.split(__file__)[0])[1] in ["lightprot", "protbuilder"]:
+    status.append("light")
+    try:
+        _prt = __import__("prot")
+        status.append("haveProt")
+    except:
+        _prt = None
+
+Empty = "empty"
+
+nameDict = {
+    "printMsg": "print",
+    "insertColor": "applycolors",
+    "cleanColor": "removecolors",
+    "getRandomString": "randomstring",
+    "checkFileSame": "checkfilesame",
+    "runAsMain": "runmoduleasmain",
+}
+
+colors = {
+    "foreground": {
+        "black": Fore.BLACK,
+        "red": Fore.RED,
+        "green": Fore.GREEN,
+        "yellow": Fore.YELLOW,
+        "blue": Fore.BLUE,
+        "magenta": Fore.MAGENTA,
+        "cyan": Fore.CYAN,
+        "white": Fore.WHITE,
+        "reset": Fore.RESET,
+    },
+    "background": {
+        "black": Back.BLACK,
+        "red": Back.RED,
+        "green": Back.GREEN,
+        "yellow": Back.YELLOW,
+        "blue": Back.BLUE,
+        "magenta": Back.MAGENTA,
+        "cyan": Back.CYAN,
+        "white": Back.WHITE,
+        "reset": Back.RESET,
+    },
+    "style": {
+        "bright": Style.BRIGHT,
+        "dim": Style.DIM,
+        "normal": Style.NORMAL,
+        "end": Style.RESET_ALL,
+        "clearline": clear_line(),
+        "clear": clear_screen(),
+    },
+}
+
+colorSymbols = {"foreground": "-", "background": "+", "style": "*"}
+
+charDict = {
+    "lowers": "abcdefghijklmnopqrstuvwxyz",
+    "uppers": "ABCDEFGHIJKLMNOPQRSTUVWXYZ",
+    "symbols": "./~!@#$%&*-_=+?",
+    "numbers": "0123456789",
+}
+
+patterns = ["%s =", "%s=", "as %s", "import %s", "%s,"]
+
+settingFilePath = _os.path.join(_os.path.split(__file__)[0], "settings")
+databaseFilePath = _os.path.join(_os.path.split(__file__)[0], "database")
+
+localSets = False
+
+settingVals = {
+    "repo": "default",
+    "ui": "normal",
+    "orderedBuiltinList": "on",
+    "saveDatabase": "off",
+    "colorize": "on",
+    "printMsgPrefix": "",
+    "printMsgColor": "",
+}
+
+settingChoices = {
+    "ui": ["verysmall", "small", "normal"],
+    "orderedBuiltinList": ["off", "on"],
+    "colorize": ["off", "on"],
+    "saveDatabase": ["off", "on"],
+    "printMsgColor": [color for color in colors["foreground"]],
+}
+
+settingData = None
+
+
+def prot(args=None):
+    if type(args) == list:
+        args = ["prot"] + args
+    elif type(args) == str:
+        args = ["prot"] + args.split(" ")
+    else:
+        args = _sys.argv
+    if not args[0] == "prot":
+        args[0] = "prot"
+    _sys.argv = args
+    _r._run_module_as_main(_sys.argv[0])
+
+
+def addBuiltins(obj, name=None, checkPPF=True):
+    if checkPPF and not PyProtFramework:
+        return obj
+    if name:
+        objname = name
+    else:
+        objname = obj.__name__
+    if objname in nameDict:
+        setattr(_builtins, nameDict[objname], obj)
+    else:
+        setattr(_builtins, objname, obj)
+    return obj
+
+
+def appendAll(obj, name=None):
+    global __add__
+    __all__.append(name if name else obj if type(obj) == str else obj.__name__)
+    return obj
+
+
+@appendAll
+def verifyColor(color, exceptionOnNot=True):
+    for c in colors["foreground"]:
+        if color == c:
+            return True
+    if exceptionOnNot:
+        raise ValueError("color not found.")
+    else:
+        return False
+
+
+@appendAll
+@addBuiltins
+def insertColor(string):
+    for c in colors:
+        for sc in colors[c]:
+            string = string.replace(colorSymbols[c] + sc, colors[c][sc])
+    return string
+
+
+@appendAll
+@addBuiltins
+def cleanColor(string):
+    for c in colors:
+        for sc in colors[c]:
+            string = string.replace(colorSymbols[c] + sc, "")
+    return string
+
+
+@appendAll
+@addBuiltins
+def getRandomString(Len=4, types=["lowers", "uppers", "symbols", "numbers"]):
+    if not type(types) == list:
+        raise TypeError("types argument must be a list object.")
+    string = ""
+    for r in range(Len):
+        string += _random.choice(str2list(charDict[_random.choice(types)]))
+    return string
+
+
+@appendAll
+def testSpeed(count):
+    progress = Progress(
+        maxVal=count,
+        msgForm="($VAL/$MAX) $TIME $PERC% completed",
+        replaces=[["$TIME", TimeWidget(milisec=True)]],
+        inline=True,
+    )
+    for c in range(count):
+        progress.next()
+    progress.newline()
+
+
+@appendAll
+def getVarFromFile(file, variable):
+    if type(file) == str:
+        file = open(file).read()
+    fileMap = file.splitlines()
+    for f in fileMap:
+        if f:
+            for t in patterns:
+                ct = t % variable
+                if ct in f:
+
+                    class tempCls:
+                        exec(f)
+
+                    res = getattr(tempCls, variable)
+                    return res
+
+
+@appendAll
+def checkMethods(obj):
+    for s in dir(obj):
+        printMsg(s + " : " + str(getattr(obj, s)))
+
+
+@appendAll
+def callMethods(obj):
+    for s in dir(obj):
+        try:
+            printMsg("result of " + s + "() is " + str(getattr(obj, s)()))
+        except:
+            printMsg("error in " + str(s) + "()")
+
+
+@appendAll
+def callMethodsWithArg(obj, arg):
+    for s in dir(obj):
+        try:
+            printMsg(
+                "result of " + s + "(" + str(arg) + ") is " + str(getattr(obj, s)(arg))
+            )
+        except:
+            printMsg("error in " + str(s) + "(" + str(arg) + ")")
+
+
+@appendAll
+@addBuiltins
+def checkFileSame(f1, f2):
+    try:
+        md5s = [_hashlib.md5(), _hashlib.md5()]
+        fs = [f1, f2]
+        for i in range(2):
+            f = open(fs[i], "rb")
+            block_size = 2**20
+            while True:
+                data = f.read(block_size)
+                if not data:
+                    break
+                md5s[i].update(data)
+            f.close()
+            md5s[i] = md5s[i].hexdigest()
+        return md5s[0] == md5s[1]
+    except:
+        return False
+
+
+@appendAll
+def splitStr(string, length):
+    out = []
+    try:
+        if len(string) > length:
+            splitDelay = len(string) // length
+            for i in range(splitDelay):
+                out.append(string[:length])
+                string = string[length:]
+            if not string == "":
+                out.append(string)
+        else:
+            out = [string]
+    except:
+        out = []
+    return out
+
+
+@appendAll
+def compileStr(string):
+    try:
+        if "." in string:
+            out = float(string)
+        else:
+            out = int(string)
+    except:
+        if string in ["True", "False", "None"]:
+            out = True if string == "True" else False if string == "False" else None
+        else:
+            out = str(string)
+    return out
+
+
+@appendAll
+def extractStr(string):
+    splittedList = string.split(",")
+    splittedDict = {}
+    splittedListNew = []
+    for i in splittedList:
+        if len(i.split(":")) > 1:
+            splittedDict[i.split(":")[0]] = i.split(":")[1]
+    for i in splittedList:
+        if len(i.split(":")) > 1:
+            for s in i.split(":"):
+                splittedListNew.append(s)
+        else:
+            splittedListNew.append(i)
+    if len(splittedListNew) == 0 and len(splittedDict) == 0:
+        raise ValueError("this string is not encoded.")
+    else:
+        data = Database()
+        for i in splittedListNew:
+            data.append(i)
+        for i in splittedDict:
+            data[i] = splittedDict[i]
+        return data
+
+
+@appendAll
+def pyCompile(source, usePEP=True, subfolders=False, deleteSource=False):
+    if _os.path.isdir(source):
+        for p in _os.listdir(source):
+            if _os.path.isdir(source + "/" + p):
+                if subfolders:
+                    pyCompile(source + "/" + p, usePEP, subfolders, deleteSource)
+            else:
+                pyCompile(source + "/" + p, usePEP, deleteSource=deleteSource)
+    if _os.path.exists(source):
+        if source.lower().endswith(".py"):
+            _py_compile.compile(
+                source, cfile=None if usePEP else source + "c", optimize=2
+            )
+            if deleteSource:
+                _os.remove(source)
+    else:
+        printErr("file or folder " + source + " not found.")
+        return
+
+
+@appendAll
+@addBuiltins
+def condition(string):
+    exec("res = " + string)
+    return res
+
+
+@appendAll
+@addBuiltins
+def runAsMain(args=None):
+    if type(args) == list:
+        pass
+    elif type(args) == str:
+        args = args.split(" ")
+    else:
+        args = _sys.argv
+    _sys.argv = args
+    _r._run_module_as_main(_sys.argv[0])
+
+
+@appendAll
+@addBuiltins
+def printMsg(msg="", color=None, end="\n", file=None, colorize=True, prefix=True):
+    global _c
+    try:
+        if "light" in status and "haveProt" in status and _prt is not None:
+            settings.colorize = _prt.settings.colorize
+    except:
+        pass
+    if settings.colorize == "off" or not _sys.stdout == _sys.__stdout__:
+        _c = False
+    if prefix and settings.printMsgPrefix:
+        msg = str(settings.printMsgPrefix) + str(msg)
+    else:
+        msg = str(msg)
+    if color and verifyColor(color):
+        msg = "-" + color + msg + "*end"
+    elif settings.printMsgColor:
+        msg = "-" + settings.printMsgColor + msg + "*end"
+    if colorize:
+        if settings.colorize == "off":
+            msg = cleanColor(msg)
+        elif not _os.name == "nt" or _c:
+            msg = insertColor(msg)
+        else:
+            msg = cleanColor(msg)
+    if file is None:
+        if _os.name == "nt" and _c:
+            out = outWin32
+        else:
+            out = _sys.stdout
+    else:
+        out = file
+    out.write(msg + end)
+    try:
+        out.flush()
+    except:
+        pass
+
+
+@appendAll
+def printErr(msg):
+    printMsg("ERROR: " + str(msg), color="red")
+
+
+@appendAll
+def printWarn(msg):
+    printMsg("WARNING: " + str(msg), color="yellow")
+
+
+@appendAll
+def getLocalIP():
+    sock = _socket.socket(_socket.AF_INET, _socket.SOCK_DGRAM)
+    try:
+        sock.connect(("10.255.255.255", 1))
+        ip = sock.getsockname()[0]
+    except:
+        ip = "127.0.0.1"
+    finally:
+        sock.close()
+    return ip
+
+
+@appendAll
+def checkAvail(address, timeout=0.5):
+    sock = _socket.socket()
+    sock.settimeout(timeout)
+    try:
+        sock.connect(address)
+        sock.close()
+        return True
+    except:
+        return False
+
+
+@appendAll
+def getBaseAddr(address):
+    return ".".join(address.split(".")[:3])
+
+
+@appendAll
+def netScan(port=80, timeout=0.5):
+    ports = port if type(port) == list else [port]
+    baseAddr = getBaseAddr(getLocalIP())
+    hostsAvail = []
+    for n in range(256):
+        host = baseAddr + "." + str(n)
+        for p in ports:
+            if checkAvail((host, p), timeout):
+                hostsAvail.append((host, p))
+    return hostsAvail
+
+
+@appendAll
+def netAttack(addr, times):
+    val1 = ValueWidget(" starting")
+    prog = Progress(
+        maxVal=times * 2, msgForm="$PERC% $MSG$1", replaces=[["$1", val1]], inline=True
+    )
+    for t in range(times):
+        val1.value = " connecting to " + str(addr[0]) + ":" + str(addr[1])
+        prog.next()
+        sock = _socket.socket()
+        sock.connect(addr)
+        val1.value = " disconnecting from " + str(addr[0]) + ":" + str(addr[1])
+        prog.next()
+        sock.close()
+    val1.value = ""
+    prog.show()
+    prog.newline()
+
+
+@appendAll
+@addBuiltins
+class Matrix(list):
+    def __getitem__(self, key):
+        if type(key) == int:
+            return list.__getitem__(self, key)
+        else:
+            res = self.get(key, default=Empty)
+            if res == Empty:
+                raise KeyError(key)
+            return res
+
+    def __setitem__(self, key, value):
+        self._checkValue(value)
+        if type(key) == int:
+            list.__setitem__(self, key, value)
+        else:
+            self.append([key, value])
+
+    def __init__(self, value=[]):
+        try:
+            if value:
+                self._checkValue(value)
+        except:
+            for v in value:
+                self._checkValue(v)
+        list.__init__(self, value)
+
+    def _checkValue(self, value):
+        if type(value) in [list, tuple, Matrix] and len(value) == 2:
+            return True
+        raise ValueError(
+            "value must be object of Matrix, list or tuple classes and should have only two members"
+        )
+
+    def append(self, value):
+        self._checkValue(value)
+        list.append(self, value)
+
+    def __delitem__(self, key):
+        if type(key) == int:
+            list.__delitem__(self, key)
+        for k in self:
+            try:
+                if k[0] == key:
+                    self.remove(k)
+            except:
+                pass
+
+    def get(self, key, default=None):
+        for k in self:
+            try:
+                if k[0] == key:
+                    return k[1]
+            except:
+                pass
+        return default
+
+
+@appendAll
+def rst2html(path, subdirs=False):
+    if _pf is None:
+        printErr("docutils package needed.")
+        return
+    if _os.path.isdir(path):
+        for p in _os.listdir(path):
+            if _os.path.isdir(path + "/" + p):
+                if subdirs:
+                    rst2html(path + "/" + p, True)
+            else:
+                rst2html(path + "/" + p)
+    if _os.path.exists(path):
+        if path.endswith(".rst"):
+            try:
+                _pf(
+                    source_path=path,
+                    destination_path=path.split(".rst")[0] + ".html",
+                    writer_name="html",
+                )
+            except:
+                import traceback
+
+                traceback.print_stack()
+                traceback.print_exc()
+    else:
+        printErr("file or folder " + path + " not found.")
+        return
+
+
+@appendAll
+def dict2matrix(obj):
+    if not type(obj) == dict:
+        raise TypeError("dict object is required.")
+    matrix = []
+    for m in obj:
+        if type(obj[m]) == dict:
+            matrix.append([m, dict2matrix(obj[m])])
+        else:
+            matrix.append(Matrix([m, obj[m]]))
+    return Matrix(matrix)
+
+
+@appendAll
+def str2list(string):
+    if not type(string) == str:
+        raise TypeError("str object is required.")
+    strList = []
+    for s in string:
+        strList.append(s)
+    return strList
+
+
+@appendAll
+def list2str(listObj, space=""):
+    if not type(listObj) == list:
+        raise TypeError("list object is required.")
+    string = ""
+    for s in listObj:
+        if string:
+            string += space
+        string += str(s)
+    return string
+
+
+@appendAll
+def matrix2str(mat, space=""):
+    if not type(mat) in [list, Matrix]:
+        raise TypeError("list or Matrix object is required.")
+    string = ""
+    for m in mat:
+        if string:
+            string += space
+        if type(m) in [list, Matrix]:
+            string += str(matrix2str(m))
+        elif type(m) == dict:
+            string += str(matrix2str(dict2matrix(m)))
+        else:
+            string += str(m)
+    return string
+
+
+@appendAll
+@addBuiltins
+class LoopBack(object):
+    def _back(*args, **kwargs):
+        pass
+
+    def __getattribute__(self, key):
+        try:
+            return object.__getattribute__(self, key)
+        except:
+            return self._back
+
+
+@appendAll
+@addBuiltins
+class Database(object):
+    def __getattribute__(self, val):
+        try:
+            return object.__getattribute__(self, val)
+        except:
+            return self.dict[val]
+
+    def __setattr__(self, key, val):
+        if str(key).startswith("_") or str(key) in [
+            "append",
+            "add",
+            "remove",
+            "dict",
+            "list",
+        ]:
+            object.__setattr__(self, key, val)
+        else:
+            self.dict[key] = val
+
+    def __delattr__(self, val):
+        try:
+            del self.dict[val]
+        except:
+            object.__delattr__(self, val)
+
+    def __getitem__(self, val):
+        return self.list[val] if type(val) == int else self.dict[val]
+
+    def __setitem__(self, key, val):
+        self.dict[key] = val
+
+    def __delitem__(self, val):
+        del self.dict[val]
+
+    def __repr__(self):
+        return str(object.__repr__(self)).replace(
+            str(str(object.__repr__(self)).split()[0]), "<Database"
+        )
+
+    def __init__(self, update=None):
+        self.dict = {} if not type(update) == dict else update
+        self.list = [] if not type(update) == list else update
+
+    def append(self, val):
+        self.list.append(val)
+
+    def add(self, val):
+        if len(str(val).split(":")) == 1:
+            self.list.append(val)
+        else:
+            self.dict[str(val).split(":")[0]] = str(val).split(":")[1]
+
+    def remove(self, val):
+        self.list.remove(val)
+
+
+@appendAll
+@addBuiltins
+class OptionsDatabase(Database):
+    def __getitem__(self, val):
+        return self.dict[val]
+
+    def __repr__(self):
+        return str(object.__repr__(self)).replace(
+            str(str(object.__repr__(self)).split()[0]), "<OptionsDatabase"
+        )
+
+    def __add__(self, other):
+        if not type(other) == OptionsDatabase:
+            raise TypeError(
+                f'can only concatenate OptionsDatabase (not "{type(other).__name__}") to OptionsDatabase'
+            )
+        newDict = {}
+        for k in self.dict:
+            newDict[k] = self.dict[k]
+        for k in other.dict:
+            newDict[k] = other.dict[k]
+        return OptionsDatabase(newDict)
+
+    def __init__(self, update=None, rules=None, allowExtraArgs=True):
+        self.dict = {} if not type(update) == dict else update
+        if rules:
+            for i, o in enumerate(rules):
+                if type(update) == tuple:
+                    try:
+                        if o.get("position", Empty) is Empty:
+                            self.dict[o["key"]] = update[i]
+                        else:
+                            self.dict[o["key"]] = update[o["position"]]
+                    except:
+                        raise Exception(f"argument '{o['key']}' is required.")
+                if not o["key"] in self.dict:
+                    if o.get("required", False):
+                        raise Exception(f"argument '{o['key']}' is required.")
+                    self.dict[o["key"]] = o.get("default", None)
+                if o.get("allowed", Empty) is not Empty:
+                    if not self.dict[o["key"]] in (
+                        o["allowed"] if type(o["allowed"]) == list else [o["allowed"]]
+                    ):
+                        raise Exception(f"value of argument '{o['key']}' is invalid.")
+                if o.get("denied", Empty) is not Empty:
+                    if self.dict[o["key"]] in (
+                        o["denied"] if type(o["denied"]) == list else [o["denied"]]
+                    ):
+                        raise Exception(f"value of argument '{o['key']}' is invalid.")
+                if o.get("type", Empty) is not Empty:
+                    if not type(self.dict[o["key"]]) == o["type"]:
+                        raise Exception(
+                            f"argument '{o['key']}' must be an {o['type'].__name__} object."
+                        )
+                if o.get("call", Empty) is not Empty:
+                    o["call"](self.dict[o["key"]])
+                if o.get("update", Empty) is not Empty:
+                    self.dict[o["key"]] = o["update"](self.dict[o["key"]])
+
+        if not allowExtraArgs:
+            ruleKeys = [o["key"] for o in rules]
+            for k in self.dict:
+                if not k in ruleKeys:
+                    raise Exception(f"argument '{k}' not requested.")
+
+
+@appendAll
+@addBuiltins
+class TextListFile(object):
+    def __init__(self, filePath, newFile=None):
+        self.file = open(filePath)
+        self.rawdata = self.file.read()
+        self.data = self.rawdata.splitlines()
+        if newFile:
+            self.newfile = open(newFile, "w")
+            self.mode = "w"
+        else:
+            self.newfile = None
+            self.mode = "r"
+
+    def optimize(self):
+        new = []
+        for s in self.data:
+            if s in new or not s:
+                continue
+            else:
+                new.append(s)
+        self.data = new
+
+    def commit(self):
+        if self.mode == "r":
+            raise Exception("can't write in read mode.")
+        self.newfile.write(list2str(self.data, "\n"))
+        self.newfile.flush()
+
+    def close(self):
+        if self.mode == "w":
+            self.newfile.close()
+        self.file.close()
+
+
+@appendAll
+@addBuiltins
+class TextDictFile(object):
+    def __init__(self, filePath, newFile=None, createFile=False):
+        if createFile and not _os.path.exists(filePath):
+            open(filePath, "w").close()
+            newFile = filePath
+        self.file = open(filePath)
+        self.rawdata = self.file.read()
+        lines = self.rawdata.splitlines()
+        if not self.checkFormat(lines):
+            raise TypeError("file type not supported.")
+        self.data = {}
+        for l in lines:
+            data = Database()
+            for d, v in {
+                "key": l.split(":")[0].strip(),
+                "val": l.split(":")[1].strip(),
+            }.items():
+                try:
+                    if "." in v:
+                        v = float(v)
+                    else:
+                        v = int(v)
+                except:
+                    if v in ["True", "False", "None"]:
+                        v = True if v == "True" else False if v == "False" else None
+                    else:
+                        v = str(v)
+                setattr(data, d, v)
+            self.data[data.key] = data.val
+        if newFile:
+            self.newfile = open(newFile, "w")
+            self.mode = "w"
+        else:
+            self.newfile = None
+            self.mode = "r"
+
+    def checkFormat(self, data):
+        for d in data:
+            if not d:
+                continue
+            if d.startswith("#"):
+                continue
+            if not ":" in d or not len(d.split(":")) == 2:
+                return False
+        return True
+
+    def commit(self):
+        if self.mode == "r":
+            raise Exception("can't write in read mode.")
+        self.newfile.write(list2str(self.convert(), "\n"))
+        self.newfile.flush()
+
+    def convert(self, data=None):
+        out = []
+        if not data:
+            data = self.data
+        for d in data:
+            out.append(str(d) + " : " + str(data[d]))
+        return out
+
+    def close(self):
+        if self.mode == "w" and not self.newfile.closed:
+            self.newfile.close()
+        if not self.file.closeed:
+            self.file.close()
+
+
+def load_settings():
+    global settingData
+    if localSets:
+        if not "light" in status:
+            printWarn(
+                "can't create settings file because permission denied, using default settings"
+            )
+        settingData = settingVals
+        return settingVals
+    if not _os.path.exists(settingFilePath):
+        raise FileNotFoundError("settings file not found.")
+    else:
+        settingFile = open(settingFilePath)
+        data = read_settings(settingFile.read().splitlines())
+        settingFile.close()
+        settingData = data
+        return data
+
+
+def read_settings(data):
+    out = {}
+    for d in data:
+        extract = d.split(":")
+        out[extract[0]] = extract[1]
+    return out
+
+
+def convert_settings(data):
+    string = ""
+    for s in data:
+        string += s + ":" + str(data[s]) + "\n"
+    return string
+
+
+def setup_settings():
+    global localSets
+    if "light" in status:
+        localSets = True
+        return
+    if not _os.path.exists(settingFilePath):
+        try:
+            settingFile = open(settingFilePath, "w")
+            settingFile.write(convert_settings(settingVals))
+            settingFile.flush()
+            settingFile.close()
+        except PermissionError:
+            localSets = True
+    else:
+        data = load_settings()
+        updated = False
+        for s in settingVals:
+            if not s in data:
+                data[s] = settingVals[s]
+                updated = True
+        if updated:
+            try:
+                settingFile = open(settingFilePath, "w")
+                settingFile.write(convert_settings(data))
+                settingFile.flush()
+                settingFile.close()
+            except PermissionError:
+                localSets = True
+
+
+class Settings(object):
+    def __init__(self):
+        if settingData:
+            self._data = settingData
+        else:
+            self._data = load_settings()
+
+    def _reset(self):
+        self._data = settingVals
+        self._write()
+
+    def _write(self):
+        if "light" in status:
+            return
+        global localSets
+        try:
+            self._file = open(settingFilePath, "w")
+            self._file.write(convert_settings(self._data))
+            self._file.flush()
+            self._file.close()
+        except PermissionError:
+            localSets = True
+
+    def __getattr__(self, key):
+        if not key.startswith("_"):
+            try:
+                if key == "reset":
+                    self._reset()
+                    printMsg("settings restored to default values")
+                    return
+                return self._data[key]
+            except KeyError:
+                printMsg("KeyError: " + "'" + key + "'", color="red")
+                return
+        else:
+            return object.__getattribute__(self, key)
+
+    def __setattr__(self, key, val):
+        if not key.startswith("_"):
+            if not key in settingVals:
+                printErr("option is invalid")
+                return
+            if key in settingChoices and not val in settingChoices[key]:
+                printErr("value is invalid")
+                return
+            self._data[key] = val
+            self._write()
+        else:
+            object.__setattr__(self, key, val)
+
+
+setup_settings()
+settings = appendAll(Settings(), "settings")
+
+
+class ProtectedDict(dict):
+    def __init__(self, *args, **kwargs):
+        dict.__init__(self, *args, **kwargs)
+        if settings.saveDatabase == "on" and not localSets:
+            if not _os.path.exists(databaseFilePath):
+                self.dataFile = TextDictFile(databaseFilePath, createFile=True)
+                self.dataFile.file.close()
+            else:
+                self.dataFile = TextDictFile(databaseFilePath, databaseFilePath)
+                self.dataFile.commit()
+                self.dataFile.file.close()
+                for d in self.dataFile.data:
+                    dict.__setitem__(self, d, self.dataFile.data[d])
+        else:
+            self.dataFile = None
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__}>"
+
+    def __setitem__(self, key, val):
+        raise TypeError("can't change ProtectedDict contents")
+
+    def __getitem__(self, key):
+        raise TypeError("can't see ProtectedDict contents")
+
+    def __delitem__(self, key):
+        raise TypeError("can't change ProtectedDict contents")
+
+
+@appendAll
+@addBuiltins
+class SecureDatabase(object):
+    def __init__(self, id, data={}, replace=False, clearOnDelete=False):
+        self.id = id
+        if not hasID(id) or replace:
+            setID(id, data, False)
+        self.data = getID(id)
+        self.dataType = type(self.data)
+        self.CON = clearOnDelete
+
+    def __repr__(self):
+        return self.data.__repr__()
+
+    def __str__(self):
+        return self.data.__str__()
+
+    def __add__(self, other):
+        return self.data.__add__(other)
+
+    def __format__(self):
+        return self.data.__format__()
+
+    def __len__(self):
+        return self.data.__len__()
+
+    def __eq__(self, other):
+        return self.data.__eq__(other)
+
+    def __ge__(self, other):
+        return self.data.__ge__(other)
+
+    def __gt__(self, other):
+        return self.data.__gt__(other)
+
+    def __hash__(self):
+        return self.data.__hash__()
+
+    def __iter__(self):
+        return self.data.__iter__()
+
+    def __ne__(self, other):
+        return self.data.__ne__(other)
+
+    def __truediv__(self, other):
+        return self.data.__truediv__(other)
+
+    def __rtruediv__(self, other):
+        return self.data.__rtruediv__(other)
+
+    def __div__(self, other):
+        return self.data.__div__(other)
+
+    def __sub__(self, other):
+        return self.data.__sub__(other)
+
+    def __mul__(self, other):
+        return self.data.__mul__(other)
+
+    def __rmul__(self, other):
+        return self.data.__rmul__(other)
+
+    def __rsub__(self, other):
+        return self.data.__rsub__(other)
+
+    def __le__(self, other):
+        return self.data.__le__(other)
+
+    def __lt__(self, other):
+        return self.data.__lt__(other)
+
+    def __del__(self):
+        if self.CON:
+            delID(self.id)
+
+    def __setitem__(self, key, val):
+        self.data.__setitem__(key, val)
+        self.update()
+
+    def __getitem__(self, key):
+        return self.data.__getitem__(key)
+
+    def __delitem__(self, key):
+        self.data.__delitem__(key)
+        self.update()
+
+    def __setattr__(self, key, val):
+        object.__setattr__(self, key, val)
+        if key == "data":
+            self.dataType = type(self.data)
+            self.update()
+
+    def update(self):
+        setID(self.id, self.data, False)
+
+
+@appendAll
+def getID(id, default=None):
+    global database
+    try:
+        return dict.__getitem__(database, id)
+    except KeyError:
+        return default
+
+
+@appendAll
+def hasID(id):
+    global database
+    return id in database
+
+
+@appendAll
+def setID(id, data, exceptOnDup=True):
+    global database
+    if hasID(id):
+        if exceptOnDup:
+            raise TypeError("can't set duplicate id.")
+    dict.__setitem__(database, id, data)
+    if database.dataFile is not None:
+        database.dataFile.newfile.write(
+            list2str(database.dataFile.convert({id: data})) + "\n"
+        )
+        database.dataFile.newfile.flush()
+
+
+@appendAll
+def delID(id):
+    global database
+    dict.__delitem__(database, id)
+
+
+database = ProtectedDict()
+
+
+class TimerThread(_threading.Thread):
+    def __init__(self, id, time, call, repeat=False):
+        _threading.Thread.__init__(self)
+        self.id = id
+        self.time = time
+        self.call = call
+        self.repeat = repeat
+
+    def run(self):
+        run = True
+        while run:
+            if getID(self.id, "stopped") == "stopped":
+                break
+            _time.sleep(self.time)
+            if getID(self.id, "stopped") == "stopped":
+                break
+            if callable(self.call):
+                self.call()
+            if not self.repeat:
+                run = False
+        delID(self.id)
+
+
+@appendAll
+@addBuiltins
+class Timer(object):
+    def __init__(self, time, call, repeat=False, type="background"):
+        self.type = type
+        if str(time)[-1] in ["s", "m", "h"]:
+            unit = str(time)[-1]
+            time = float(str(time)[:-1])
+            if unit in ["m", "h"]:
+                time = time * 60
+            if unit in ["h"]:
+                time = time * 60
+        time = float(time)
+        self.id = int(getRandomString(10, ["numbers"]))
+        setID(self.id, "started", False)
+        thread = TimerThread(self.id, time, call, repeat)
+        if type == "background":
+            thread.daemon = True
+            thread.start()
+        elif type == "foreground":
+            thread.run()
+        else:
+            printErr("type is invalid")
+
+    def __repr__(self):
+        return f'<{self.__class__.__name__} {getID(self.id, "stopped")} ID={str(self.id) if hasID(self.id) else str(None)}>'
+
+    def __del__(self):
+        setID(self.id, "stopped", False)
+
+
+@appendAll
+@addBuiltins
+class Call(object):
+    def __init__(self, *args, **keywds):
+        self.call = args[0]
+        self.args = args[1:]
+        self.keywds = keywds
+
+    def __call__(self, *argsExtra):
+        return self.call(*self.args + argsExtra, **self.keywds)
+
+    def __repr__(self):
+        return (
+            "<Call object call="
+            + str(self.call)
+            + " args="
+            + str(self.args)
+            + " keywds="
+            + str(self.keywds)
+            + ">"
+        )
+
+
+@appendAll
+@addBuiltins
+class Widget(object):
+    def __init__(self, progressNeeded=False):
+        self.reprMsg = "<$name Widget>".replace("$name", str(self.__class__.__name__))
+        self.progress = None
+        self._finished = False
+        self.progressNeeded = progressNeeded
+
+    def _set_progress(self, progress):
+        if not isinstance(progress, Progress):
+            raise TypeError(str(progress) + " must be instance of " + str(Progress))
+        self.progress = progress
+
+    def _finish(self):
+        self._finished = True
+
+    def __repr__(self):
+        return self.reprMsg
+
+    def __call__(self):
+        if self.progressNeeded and self.progress is None:
+            raise Exception("progress instance needed.")
+
+
+@appendAll
+@addBuiltins
+class TimeWidget(Widget):
+    def __init__(self, milisec=False, min=True, hour=True):
+        Widget.__init__(self)
+        self.milisec = milisec
+        self.min = min
+        self.hour = hour
+        self._startTime = _time.time()
+        self.startTime = int(self._startTime)
+
+    def calc_time(self):
+        _now = _time.time()
+        now = int(_now)
+        string = ""
+        if self.milisec:
+            milisec = str(_now - self._startTime).split(".")[1][:3]
+        sec = now - self.startTime
+        min = 0
+        hour = 0
+        if sec >= 60 and self.min:
+            for m in range(sec // 60):
+                sec -= 60
+                min += 1
+        if min >= 60 and self.hour:
+            for m in range(min // 60):
+                min -= 60
+                hour += 1
+        if len(str(hour)) <= 1:
+            hour = "0" + str(hour)
+        if len(str(min)) <= 1:
+            min = "0" + str(min)
+        if len(str(sec)) <= 1:
+            sec = "0" + str(sec)
+        if self.hour:
+            string += str(hour) + ":"
+        if self.min:
+            string += str(min) + ":"
+        if self.milisec:
+            sec = str(sec) + "." + milisec
+        string += str(sec)
+        return string
+
+    def __call__(self):
+        Widget.__call__(self)
+        return self.calc_time()
+
+
+@appendAll
+@addBuiltins
+class BarWidget(Widget):
+    def __init__(self, fill="█", empty="░", fillPerPercent=5, color=None):
+        Widget.__init__(self, True)
+        self.fill = fill
+        self.empty = empty
+        self.fpp = fillPerPercent
+        self.color = color
+
+    def __call__(self):
+        Widget.__call__(self)
+        return self.createBar()
+
+    def createBar(self):
+        perc = int(self.progress.calc_perc().split(".")[0])
+        bar = ""
+        filled = 0
+        if perc >= self.fpp:
+            for c in range(perc // self.fpp):
+                bar += self.fill
+                filled += 1
+        for f in range(100 // self.fpp - filled):
+            bar += self.empty
+        if self.color and verifyColor(self.color, False):
+            bar = "-" + self.color + bar + "*end"
+
+        return bar
+
+
+@appendAll
+@addBuiltins
+class TaskWidget(Widget):
+    def __init__(self, tasks={}):
+        Widget.__init__(self, True)
+        self.tasks = tasks
+        self.percTasks = {}
+        self.eventTasks = {}
+        self.firstRun = True
+        self.checkTasks()
+
+    def checkTasks(self):
+        for t in self.tasks:
+            if t == "perc":
+                self.percTasks = self.tasks[t]
+            elif t == "event":
+                self.eventTasks = self.tasks[t]
+
+    def __call__(self):
+        Widget.__call__(self)
+        return calc_task()
+
+    def calc_task(self):
+        if self.eventTasks:
+            if "onFirstShow" in self.eventTasks and self.firstRun:
+                self.firstRun = False
+                return self.eventTasks["onFirstShow"]
+            if "onFinish" in self.eventTasks and self._finished:
+                return self.eventTasks["onFinish"]
+        if self.percTasks:
+            perc = int(self.progress.calc_true_perc())
+            for p in self.percTasks:
+                if perc <= p:
+                    return self.percTasks[p]
+        return ""
+
+
+@appendAll
+@addBuiltins
+class CallWidget(Widget):
+    def __init__(self, call, progressNeeded=False):
+        Widget.__init__(self, progressNeeded)
+        self.call = call
+
+    def __call__(self):
+        Widget.__call__(self)
+        if self.progressNeeded:
+            return self.call(self.progress)
+        else:
+            return self.call()
+
+
+@appendAll
+@addBuiltins
+class ValueWidget(Widget):
+    def __init__(self, value):
+        Widget.__init__(self)
+        self.value = value
+
+    def __call__(self):
+        Widget.__call__(self)
+        return self.value
+
+
+@appendAll
+@addBuiltins
+class LoadingWidget(Widget):
+    def __init__(self, type="default"):
+        Widget.__init__(self)
+        self.type = type
+        self.index = 0
+        self.msg = None
+        self.loadingType = None
+        self.handleType()
+
+    def handleType(self):
+        typeData = self.getTypes()[self.type]
+        self.msg = typeData["data"]
+        self.loadingType = type(typeData["data"])
+        if self.loadingType == str:
+            self.msg = ProtString(self.msg)
+
+    def createMsg(self):
+        if self._finished:
+            return "done"
+        if self.loadingType == list:
+            msg = self.msg[self.index]
+            if self.index + 1 == len(self.msg):
+                self.index = 0
+            else:
+                self.index += 1
+            return msg
+        else:
+            msg = self.msg
+            end = self.msg[-1]
+            del self.msg[-1]
+            self.msg = self.msg.query
+            self.msg = ProtString(end + str(self.msg))
+            return msg
+
+    def __call__(self):
+        Widget.__call__(self)
+        return self.createMsg()
+
+    def getTypes(self):
+        return {
+            "default": {"data": ["|", "-"]},
+            "bar": {"data": "█████               "},
+            "smallbar": {"data": "███         "},
+            "verysmallbar": {"data": "██      "},
+        }
+
+
+@appendAll
+@addBuiltins
+class LockedDict(dict):
+    def __delitem__(self, val):
+        raise TypeError("dict is locked.")
+
+    def __setitem__(self, key, val):
+        raise TypeError("dict is locked.")
+
+
+@appendAll
+@addBuiltins
+class Progress(object):
+    _deafultForm = "($VAL/$MAX) $PERC% $MSG"
+
+    def __init__(
+        self,
+        val=0,
+        minVal=0,
+        maxVal=100,
+        msg="completed",
+        msgForm=None,
+        replaces=[],
+        color=None,
+        inline=False,
+    ):
+        self._finished = False
+        self.val = val
+        self.min = minVal
+        self.max = maxVal
+        self.msg = msg
+        self.inline = (
+            inline
+            if _sys.stdout == _sys.__stdout__ and (not _os.name == "nt" or _c)
+            else False
+        )
+        self.color = color
+        if not msgForm:
+            self.msgForm = self.get_default_form()
+        else:
+            self.msgForm = msgForm
+        if replaces:
+            for r in replaces:
+                if not isinstance(r[1], Widget):
+                    raise TypeError(str(r[1]) + " must be instance of Widget")
+                r[1]._set_progress(self)
+            self.extraReplaces = replaces
+        else:
+            self.extraReplaces = []
+        self.show()
+
+    def show(self):
+        replaces = self.getDefaultReplaces()
+        msg = self.do_replace(replaces)
+        if self.color and verifyColor(self.color, False):
+            msg = "-" + self.color + msg + "*end"
+        if self.inline:
+            self.printInline(msg)
+        else:
+            printMsg(msg)
+
+    def getDefaultReplaces(self):
+        return [
+            ["$VAL", self.val],
+            ["$MIN", self.min],
+            ["$MAX", self.max],
+            ["$PERC", self.calc_perc()],
+            ["$TRUE_PERC", self.calc_true_perc()],
+            ["$MSG", self.msg],
+        ]
+
+    def clear(self):
+        printMsg("\r\x1b[K", end="", prefix=False)
+
+    def printInline(self, msg):
+        self.clear()
+        printMsg(msg, end="")
+
+    def write(self, msg=""):
+        if self.inline:
+            printMsg("\n" + msg)
+        else:
+            printMsg(msg)
+
+    def newline(self):
+        if self.inline:
+            printMsg("", prefix=False)
+
+    def finish(self):
+        for r in self.extraReplaces:
+            r[1]._finish()
+        self._finished = True
+        self.newline()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.finish()
+
+    def get_default_form(self):
+        return self._deafultForm
+
+    def calc_perc(self):
+        perc = str(100 / self.max * self.val).split(".")
+        perc[1] = perc[1][:3]
+        return perc[0] + "." + perc[1]
+
+    def calc_true_perc(self):
+        perc = str(100 / self.max * self.val).split(".")[0]
+        return perc
+
+    def do_replace(self, rl):
+        cf = self.msgForm if not hasattr(self, "tempMsg") else self.tempMsg
+        for r in rl:
+            cf = cf.replace(r[0], str(r[1]))
+        for r in self.extraReplaces:
+            cf = cf.replace(r[0], str(r[1]()))
+        if "$" in cf and not hasattr(self, "tempMsg"):
+            self.tempMsg = cf
+            self.do_replace(rl)
+        else:
+            try:
+                del self.tempMsg
+            except:
+                pass
+            return cf
+
+    def update(self, val):
+        self.val = max(self.min, min(self.max, val))
+        self.show()
+
+    def next(self, val=1):
+        self.val = max(self.min, min(self.max, self.val + val))
+        self.show()
+
+
+@appendAll
+@addBuiltins
+class ProgressBar(Progress, BarWidget):
+    def __init__(
+        self,
+        val=0,
+        minVal=0,
+        maxVal=100,
+        msg="completed",
+        msgForm=None,
+        replaces=[],
+        color=None,
+        inline=False,
+        fill="█",
+        empty="░",
+        fillPerPercent=5,
+    ):
+        BarWidget.__init__(self, fill=fill, empty=empty, fillPerPercent=fillPerPercent)
+        Progress.__init__(
+            self,
+            val=val,
+            minVal=minVal,
+            maxVal=maxVal,
+            msg=msg,
+            msgForm=msgForm,
+            replaces=replaces,
+            color=color,
+            inline=inline,
+        )
+        self.progress = self
+
+    def __repr__(self):
+        return object.__repr__(self)
+
+    def getDefaultReplaces(self):
+        Progress.getDefaultReplaces(self) + [["$BAR", self()]]
+
+    def finish(self):
+        self._finish()
+        Progress.finish(self)
+
+
+@appendAll
+@addBuiltins
+class VersionString(str):
+    def __init__(self, *args, **kwargs):
+        str.__init__(self)
+        try:
+            ver = self.split(".")
+            try:
+                self.major = int(ver[0])
+            except:
+                self.major = None
+            try:
+                self.minor = int(ver[1])
+            except:
+                self.minor = None
+            try:
+                self.micro = int(ver[2])
+            except:
+                self.micro = None
+        except:
+            pass
+
+    def upgrade(self, target="default", maxMinor=9, maxMicro=9):
+        if target == "default":
+            if self.micro is not None:
+                target = "micro"
+            elif self.minor is not None:
+                target = "minor"
+            elif self.major is not None:
+                target = "major"
+        if self.micro is not None and self.micro >= maxMicro:
+            minor = True
+        else:
+            minor = False
+        if self.minor is not None and self.minor >= maxMinor:
+            major = True
+        else:
+            major = False
+        if False:
+            print(f"target: {str(target)}")
+            print(f"self.micro: {str(self.micro)}")
+            print(f"maxMicro: {str(maxMicro)}")
+            print(f"self.minor: {str(self.minor)}")
+            print(f"maxMinor: {str(maxMinor)}")
+            print(f"minor: {str(minor)}")
+            print(f"self.major: {str(self.major)}")
+            print(f"major: {str(major)}")
+        if self.micro is not None and target == "micro":
+            self.micro += 1
+        if self.minor is not None and (target == "minor" or minor) and not major:
+            if self.micro is not None:
+                self.micro = 0
+            self.minor += 1
+        if self.major is not None and (target == "major" or (major and minor)):
+            if self.micro is not None:
+                self.micro = 0
+            if self.minor is not None:
+                self.minor = 0
+            self.major += 1
+        return self.compile()
+
+    def compile(self):
+        ver = []
+        if self.major is not None:
+            ver.append(str(self.major))
+        if self.minor is not None:
+            ver.append(str(self.minor))
+        if self.micro is not None:
+            ver.append(str(self.micro))
+        return ".".join(ver)
+
+
+@appendAll
+@addBuiltins
+class ProtString(str):
+    def compile(self):
+        try:
+            if "." in self:
+                out = float(self)
+            else:
+                out = int(self)
+        except:
+            if self in ["True", "False", "None"]:
+                out = True if self == "True" else False if self == "False" else None
+            else:
+                out = str(self)
+        return out
+
+    @property
+    def type(self):
+        return self.split(".")[-1].lower()
+
+    @property
+    def has_type(self):
+        return len(self.split(".")) > 1
+
+    def extract(self):
+        splittedList = self.split(",")
+        splittedDict = {}
+        splittedListNew = []
+        for i in splittedList:
+            if len(i.split(":")) > 1:
+                splittedDict[i.split(":")[0]] = i.split(":")[1]
+        for i in splittedList:
+            if len(i.split(":")) > 1:
+                for s in i.split(":"):
+                    splittedListNew.append(s)
+            else:
+                splittedListNew.append(i)
+        if len(splittedListNew) == 0 and len(splittedDict) == 0:
+            raise ValueError("this string is not encoded.")
+        else:
+            data = Database()
+            for i in splittedListNew:
+                data.append(i)
+            for i in splittedDict:
+                data[i] = splittedDict[i]
+            return data
+
+    def __setitem__(self, index, val):
+        stringList = []
+        for string in self:
+            stringList.append(string)
+        stringList[index] = str(val)
+        compiledString = ""
+        for string in stringList:
+            compiledString += string
+        self.query = self.__class__(compiledString)
+
+    def __delitem__(self, key):
+        stringList = []
+        for string in self:
+            stringList.append(string)
+        del stringList[key]
+        compiledString = ""
+        for string in stringList:
+            compiledString += string
+        self.query = self.__class__(compiledString)
+
+    def __div__(self, other):
+        out = []
+        try:
+            if len(self) > other:
+                splitDelay = len(self) // other
+                tStr = str(self)
+                for i in range(splitDelay):
+                    out.append(tStr[:other])
+                    tStr = tStr[other:]
+                if not tStr == "":
+                    out.append(tStr)
+            else:
+                out = [self]
+        except:
+            out = []
+        return out
```

### Comparing `prot-3.9.1/src/prot/bs/bs.py` & `prot-3.9.2/src/prot/bs/bs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-import hashlib
-import os
-import shutil
-from base64 import b64encode
-from functools import partial
-
-from . import *
-
-treeCache = {}
-
-
-def getModel(file):
-    return file + ".bob"
-
-
-def getCollideModel(file):
-    return file + ".cob"
-
-
-def getTexture(file):
-    return file + ".texture"
-
-
-def getSound(file):
-    return file + ".ogg"
-
-
-class Material(LoopBack):
-    pass
-
-
-class Factory(object):
-    def __setattr__(self, key, value):
-        if key in ["dict", "getcontents"] or key.startswith("_"):
-            object.__setattr__(self, key, value)
-        if not hasattr(self, "dict"):
-            self.dict = {}
-        self.dict[key] = value
-
-    def __getattribute__(self, key):
-        if key in ["dict", "getcontents"] or key.startswith("_"):
-            return object.__getattribute__(self, key, value)
-        if not hasattr(self, "dict"):
-            self.dict = {}
-        return self.dict[key]
-
-    def getcontents(self, path="."):
-        files = []
-        data = {self.__class__.__name__: files}
-        for key, value in self.dict.items():
-            if type(value) == str:
-                values = [value]
-            elif type(value) in [list, tuple]:
-                values = list(value)
-            else:
-                continue
-            for fileName in values:
-                if fileName.endswith(".texture"):
-                    files += bs.getFiles(fileName.split(".")[0], path, ["ktx", "dds"])
-                else:
-                    files.append(fileName)
-        return data
-
-
-def md5sum(filename):
-    with open(filename, mode="rb") as f:
-        d = hashlib.md5()
-        for buf in iter(partial(f.read, 128), b""):
-            d.update(buf)
-    return d.hexdigest()
-
-
-def genPayloadInfo():
-    files = []
-    for root, subdirs, files_in_dir in os.walk(".", topdown=True, followlinks=False):
-        for file in files_in_dir:
-            if file.startswith(".") or file == "payload_info":
-                continue
-            files.append(os.path.join(root, file))
-
-    payloadStr = "{}\n1\n".format(len(files))
-    for file in files:
-        payloadStr += "{} {}\n".format(file.strip("./"), md5sum(file))
-
-    with open("payload_info", "w") as f:
-        f.write(payloadStr)
-        f.close()
-
-
-def getFiles(file, path=".", formats=["ogg", "ktx", "dds", "bob", "cob", "py", "pyc"]):
-    tree = makeTree(path)
-    files = []
-    for format in formats:
-        if file + "." + format in tree:
-            files.append(file + "." + format)
-    return files
-
-
-def makeTree(source=".", ignoreCache=False):
-    if source in treeCache and not ignoreCache:
-        return treeCache[source]
-    tree = {}
-    for p in os.listdir(source):
-        if os.path.isdir(os.path.join(source, p)):
-            for name, path in makeTree(os.path.join(source, p)).items():
-                tree[name] = path
-        else:
-            tree[p] = os.path.join(source, p)
-    if not ignoreCache:
-        treeCache[source] = tree
-    return tree
-
-
-def encodeFile(source):
-    ff = open("coded-" + source, "wb")
-    ff.write(
-        "import base64;exec(base64.b64decode("
-        + repr(b64encode(open(source).read()))
-        + "))"
-    )
-    ff.flush()
-
-
-def processMedia(data, path=".", divide=False, silent=False):
-    tree = makeTree(path)
-    media = os.path.join(path, "media")
-    if not os.path.isdir(media):
-        os.mkdir(media)
-    for name, files in data.items():
-        if divide:
-            media = os.path.join(media, name)
-            if not os.path.isdir(media):
-                os.mkdir(media)
-
-        audios = os.path.join(media, "audios")
-        tex = os.path.join(media, "textures")
-        texAndroid = os.path.join(tex, "android")
-        texOther = os.path.join(tex, "other")
-        models = os.path.join(media, "models")
-        scripts = os.path.join(media, "scripts")
-
-        if not os.path.isdir(audios):
-            os.mkdir(audios)
-        if not os.path.isdir(tex):
-            os.mkdir(tex)
-        if not os.path.isdir(texAndroid):
-            os.mkdir(texAndroid)
-        if not os.path.isdir(texOther):
-            os.mkdir(texOther)
-        if not os.path.isdir(models):
-            os.mkdir(models)
-        if not os.path.isdir(scripts):
-            os.mkdir(scripts)
-
-        audioFormats = ["ogg"]
-        texFormats = ["dds", "ktx"]
-        modelFormats = ["bob", "cob"]
-        scriptFormats = ["py", "pyc"]
-
-        for file in files:
-            if file in tree:
-                if file.type in audioFormats:
-                    if not silent:
-                        print(file + " -> " + audios)
-                    shutil.copy(tree[file], audios)
-                elif file.type in texFormats:
-                    if file.type == "ktx":
-                        if not silent:
-                            print(file + " -> " + texAndroid)
-                        shutil.copy(tree[file], texAndroid)
-                    else:
-                        if not silent:
-                            print(file + " -> " + texOther)
-                        shutil.copy(tree[file], texOther)
-                elif file.type in modelFormats:
-                    if not silent:
-                        print(file + " -> " + models)
-                    shutil.copy(tree[file], models)
-                elif file.type in scriptFormats:
-                    if not silent:
-                        print(file + " -> " + scripts)
-                    shutil.copy(tree[file], scripts)
-                else:
-                    printWarn("type of file " + file + " is not supported")
-            else:
-                printWarn("file " + file + " not found")
+import hashlib
+import os
+import shutil
+from base64 import b64encode
+from functools import partial
+
+from . import *
+
+treeCache = {}
+
+
+def getModel(file):
+    return file + ".bob"
+
+
+def getCollideModel(file):
+    return file + ".cob"
+
+
+def getTexture(file):
+    return file + ".texture"
+
+
+def getSound(file):
+    return file + ".ogg"
+
+
+class Material(LoopBack):
+    pass
+
+
+class Factory(object):
+    def __setattr__(self, key, value):
+        if key in ["dict", "getcontents"] or key.startswith("_"):
+            object.__setattr__(self, key, value)
+        if not hasattr(self, "dict"):
+            self.dict = {}
+        self.dict[key] = value
+
+    def __getattribute__(self, key):
+        if key in ["dict", "getcontents"] or key.startswith("_"):
+            return object.__getattribute__(self, key, value)
+        if not hasattr(self, "dict"):
+            self.dict = {}
+        return self.dict[key]
+
+    def getcontents(self, path="."):
+        files = []
+        data = {self.__class__.__name__: files}
+        for key, value in self.dict.items():
+            if type(value) == str:
+                values = [value]
+            elif type(value) in [list, tuple]:
+                values = list(value)
+            else:
+                continue
+            for fileName in values:
+                if fileName.endswith(".texture"):
+                    files += bs.getFiles(fileName.split(".")[0], path, ["ktx", "dds"])
+                else:
+                    files.append(fileName)
+        return data
+
+
+def md5sum(filename):
+    with open(filename, mode="rb") as f:
+        d = hashlib.md5()
+        for buf in iter(partial(f.read, 128), b""):
+            d.update(buf)
+    return d.hexdigest()
+
+
+def genPayloadInfo():
+    files = []
+    for root, subdirs, files_in_dir in os.walk(".", topdown=True, followlinks=False):
+        for file in files_in_dir:
+            if file.startswith(".") or file == "payload_info":
+                continue
+            files.append(os.path.join(root, file))
+
+    payloadStr = "{}\n1\n".format(len(files))
+    for file in files:
+        payloadStr += "{} {}\n".format(file.strip("./"), md5sum(file))
+
+    with open("payload_info", "w") as f:
+        f.write(payloadStr)
+        f.close()
+
+
+def getFiles(file, path=".", formats=["ogg", "ktx", "dds", "bob", "cob", "py", "pyc"]):
+    tree = makeTree(path)
+    files = []
+    for format in formats:
+        if file + "." + format in tree:
+            files.append(file + "." + format)
+    return files
+
+
+def makeTree(source=".", ignoreCache=False):
+    if source in treeCache and not ignoreCache:
+        return treeCache[source]
+    tree = {}
+    for p in os.listdir(source):
+        if os.path.isdir(os.path.join(source, p)):
+            for name, path in makeTree(os.path.join(source, p)).items():
+                tree[name] = path
+        else:
+            tree[p] = os.path.join(source, p)
+    if not ignoreCache:
+        treeCache[source] = tree
+    return tree
+
+
+def encodeFile(source):
+    ff = open("coded-" + source, "wb")
+    ff.write(
+        "import base64;exec(base64.b64decode("
+        + repr(b64encode(open(source).read()))
+        + "))"
+    )
+    ff.flush()
+
+
+def processMedia(data, path=".", divide=False, silent=False):
+    tree = makeTree(path)
+    media = os.path.join(path, "media")
+    if not os.path.isdir(media):
+        os.mkdir(media)
+    for name, files in data.items():
+        if divide:
+            media = os.path.join(media, name)
+            if not os.path.isdir(media):
+                os.mkdir(media)
+
+        audios = os.path.join(media, "audios")
+        tex = os.path.join(media, "textures")
+        texAndroid = os.path.join(tex, "android")
+        texOther = os.path.join(tex, "other")
+        models = os.path.join(media, "models")
+        scripts = os.path.join(media, "scripts")
+
+        if not os.path.isdir(audios):
+            os.mkdir(audios)
+        if not os.path.isdir(tex):
+            os.mkdir(tex)
+        if not os.path.isdir(texAndroid):
+            os.mkdir(texAndroid)
+        if not os.path.isdir(texOther):
+            os.mkdir(texOther)
+        if not os.path.isdir(models):
+            os.mkdir(models)
+        if not os.path.isdir(scripts):
+            os.mkdir(scripts)
+
+        audioFormats = ["ogg"]
+        texFormats = ["dds", "ktx"]
+        modelFormats = ["bob", "cob"]
+        scriptFormats = ["py", "pyc"]
+
+        for file in files:
+            if file in tree:
+                if file.type in audioFormats:
+                    if not silent:
+                        print(file + " -> " + audios)
+                    shutil.copy(tree[file], audios)
+                elif file.type in texFormats:
+                    if file.type == "ktx":
+                        if not silent:
+                            print(file + " -> " + texAndroid)
+                        shutil.copy(tree[file], texAndroid)
+                    else:
+                        if not silent:
+                            print(file + " -> " + texOther)
+                        shutil.copy(tree[file], texOther)
+                elif file.type in modelFormats:
+                    if not silent:
+                        print(file + " -> " + models)
+                    shutil.copy(tree[file], models)
+                elif file.type in scriptFormats:
+                    if not silent:
+                        print(file + " -> " + scripts)
+                    shutil.copy(tree[file], scripts)
+                else:
+                    printWarn("type of file " + file + " is not supported")
+            else:
+                printWarn("file " + file + " not found")
```

### Comparing `prot-3.9.1/src/prot/bs/bsMap.py` & `prot-3.9.2/src/prot/bs/bsMap.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import builtins as _builtins
-
-from . import *
-
-maps = {}
-depends = []
-
-
-class Map(object):
-    name = "Map"
-
-    @classmethod
-    def getPreviewTextureName(cls):
-        """
-        Return the name of the preview texture for this map.
-        """
-        return None
-
-    @classmethod
-    def onPreload(cls):
-        """
-        Called when the map is being preloaded;
-        it should load any media it requires to
-        class attributes on itself.
-        """
-        return None
-
-
-def registerMap(map):
-    if not map.name in maps:
-        maps[map.name] = map
-    else:
-        raise Exception(repr(map.name) + "already exists.")
-
-
-def _import(*args, **kwargs):
-    depends.append(args[0])
-    if _import.redirect:
-        return _builtins.__import(*args, **kwargs)
-
-
-def record(redirect=False):
-    if redirect:
-        _import.redirect = True
-    else:
-        _import.redirect = False
-    _builtins.__import = _builtins.__import__
-    _builtins.__import__ = _import
-
-
-def end():
-    _builtins.__import__ = _builtins.__import
-    del _builtins.__import
-    del _import.redirect
-
-
-def clear():
-    global maps
-    global depends
-    maps = {}
-    depends = []
-
-
-def getMedia(path=".", divide=False, silent=False):
-    tree = bs.makeTree(path)
-    data = {}
-    for name, obj in maps.items():
-        medias = []
-        preloads = []
-        if obj.getPreviewTextureName() is not None:
-            medias += bs.getFiles(obj.getPreviewTextureName(), path, ["ktx", "dds"])
-        if obj.onPreload() is not None:
-            for key, value in obj.onPreload().items():
-                if type(value) == str:
-                    preloads.append(value)
-                elif type(value) in [list, tuple]:
-                    preloads += list(value)
-        for preload in preloads:
-            if preload.endswith(".texture"):
-                medias += bs.getFiles(preload.split(".")[0], path, ["ktx", "dds"])
-            else:
-                medias.append(preload)
-        for depend in depends:
-            medias += bs.getFiles(depend, path, ["py", "pyc"])
-        data[name] = [ProtString(media) for media in medias]
-
-    if data:
-        bs.processMedia(data, path, divide, silent)
+import builtins as _builtins
+
+from . import *
+
+maps = {}
+depends = []
+
+
+class Map(object):
+    name = "Map"
+
+    @classmethod
+    def getPreviewTextureName(cls):
+        """
+        Return the name of the preview texture for this map.
+        """
+        return None
+
+    @classmethod
+    def onPreload(cls):
+        """
+        Called when the map is being preloaded;
+        it should load any media it requires to
+        class attributes on itself.
+        """
+        return None
+
+
+def registerMap(map):
+    if not map.name in maps:
+        maps[map.name] = map
+    else:
+        raise Exception(repr(map.name) + "already exists.")
+
+
+def _import(*args, **kwargs):
+    depends.append(args[0])
+    if _import.redirect:
+        return _builtins.__import(*args, **kwargs)
+
+
+def record(redirect=False):
+    if redirect:
+        _import.redirect = True
+    else:
+        _import.redirect = False
+    _builtins.__import = _builtins.__import__
+    _builtins.__import__ = _import
+
+
+def end():
+    _builtins.__import__ = _builtins.__import
+    del _builtins.__import
+    del _import.redirect
+
+
+def clear():
+    global maps
+    global depends
+    maps = {}
+    depends = []
+
+
+def getMedia(path=".", divide=False, silent=False):
+    tree = bs.makeTree(path)
+    data = {}
+    for name, obj in maps.items():
+        medias = []
+        preloads = []
+        if obj.getPreviewTextureName() is not None:
+            medias += bs.getFiles(obj.getPreviewTextureName(), path, ["ktx", "dds"])
+        if obj.onPreload() is not None:
+            for key, value in obj.onPreload().items():
+                if type(value) == str:
+                    preloads.append(value)
+                elif type(value) in [list, tuple]:
+                    preloads += list(value)
+        for preload in preloads:
+            if preload.endswith(".texture"):
+                medias += bs.getFiles(preload.split(".")[0], path, ["ktx", "dds"])
+            else:
+                medias.append(preload)
+        for depend in depends:
+            medias += bs.getFiles(depend, path, ["py", "pyc"])
+        data[name] = [ProtString(media) for media in medias]
+
+    if data:
+        bs.processMedia(data, path, divide, silent)
```

### Comparing `prot-3.9.1/src/prot/bs/bsPro.py` & `prot-3.9.2/src/prot/bs/bsPro.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import json
-from base64 import b64encode
-
-from . import *
-
-
-def bpp2cbpp(source):
-    with open(source) as file:
-        codesList = [row for row in file]
-    codedStr = None
-    stdStr = ""
-    for c in codesList:
-        if str(c).startswith("#  # #"):
-            codedStr = c
-        else:
-            stdStr = stdStr + c
-
-    if codedStr is not None:
-        bCodedStr = b64encode(codedStr)
-    else:
-        bCodedStr = None
-    if stdStr:
-        bStdStr = b64encode(stdStr)
-    else:
-        bStdStr = None
-    if bCodedStr is not None and bStdStr is not None:
-        fCode = bCodedStr + "\n" + bStdStr
-    else:
-        fCode = bStdStr
-    with open(source.split(".")[0] + ".cbpp", "wb") as nf:
-        nf.write(fCode)
-        nf.flush()
-
-
-def py2jbpp(source):
-    exec(open(source).read())
-    with open(source.split(".")[0] + ".jbpp", "w") as nf:
-        nf.write(json.dumps(dict))
-        nf.flush()
+import json
+from base64 import b64encode
+
+from . import *
+
+
+def bpp2cbpp(source):
+    with open(source) as file:
+        codesList = [row for row in file]
+    codedStr = None
+    stdStr = ""
+    for c in codesList:
+        if str(c).startswith("#  # #"):
+            codedStr = c
+        else:
+            stdStr = stdStr + c
+
+    if codedStr is not None:
+        bCodedStr = b64encode(codedStr)
+    else:
+        bCodedStr = None
+    if stdStr:
+        bStdStr = b64encode(stdStr)
+    else:
+        bStdStr = None
+    if bCodedStr is not None and bStdStr is not None:
+        fCode = bCodedStr + "\n" + bStdStr
+    else:
+        fCode = bStdStr
+    with open(source.split(".")[0] + ".cbpp", "wb") as nf:
+        nf.write(fCode)
+        nf.flush()
+
+
+def py2jbpp(source):
+    exec(open(source).read())
+    with open(source.split(".")[0] + ".jbpp", "w") as nf:
+        nf.write(json.dumps(dict))
+        nf.flush()
```

### Comparing `prot-3.9.1/src/prot/bs/bsSpaz.py` & `prot-3.9.2/src/prot/bs/bsSpaz.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import os
-import shutil
-
-from . import *
-
-appearances = {}
-
-
-class Appearance(Database):
-    def __init__(self, name):
-        Database.__init__(self)
-        if not name in appearances:
-            appearances[name] = self
-        else:
-            raise Exception(repr(name) + "already exists.")
-
-
-def clear():
-    global appearances
-    appearances = {}
-
-
-def getOutput(file):
-    string = ""
-    for a in appearances:
-        string += (
-            "addCharacter(" + repr(a) + ", cfg=" + str(appearances[a].dict) + ")\n"
-        )
-
-    with open(file, "w") as f:
-        f.write(string)
-        f.flush()
-
-
-def getMedia(path=".", divide=False, silent=False):
-    tree = bs.makeTree(path)
-    data = {}
-    for name, obj in appearances.items():
-        medias = []
-        for key, value in obj.dict.items():
-            if type(value) == str:
-                values = [value]
-            elif type(value) in [list, tuple]:
-                values = list(value)
-            else:
-                continue
-            for fileName in values:
-                medias += bs.getFiles(
-                    fileName, path, ["ogg", "ktx", "dds", "bob", "cob"]
-                )
-        data[name] = [ProtString(media) for media in medias]
-
-    if data:
-        bs.processMedia(data, path, divide, silent)
+import os
+import shutil
+
+from . import *
+
+appearances = {}
+
+
+class Appearance(Database):
+    def __init__(self, name):
+        Database.__init__(self)
+        if not name in appearances:
+            appearances[name] = self
+        else:
+            raise Exception(repr(name) + "already exists.")
+
+
+def clear():
+    global appearances
+    appearances = {}
+
+
+def getOutput(file):
+    string = ""
+    for a in appearances:
+        string += (
+            "addCharacter(" + repr(a) + ", cfg=" + str(appearances[a].dict) + ")\n"
+        )
+
+    with open(file, "w") as f:
+        f.write(string)
+        f.flush()
+
+
+def getMedia(path=".", divide=False, silent=False):
+    tree = bs.makeTree(path)
+    data = {}
+    for name, obj in appearances.items():
+        medias = []
+        for key, value in obj.dict.items():
+            if type(value) == str:
+                values = [value]
+            elif type(value) in [list, tuple]:
+                values = list(value)
+            else:
+                continue
+            for fileName in values:
+                medias += bs.getFiles(
+                    fileName, path, ["ogg", "ktx", "dds", "bob", "cob"]
+                )
+        data[name] = [ProtString(media) for media in medias]
+
+    if data:
+        bs.processMedia(data, path, divide, silent)
```

### Comparing `prot-3.9.1/src/prot/code.py` & `prot-3.9.2/src/prot/code.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,399 +1,399 @@
-import base64 as __cmethst__
-import os
-import random
-import sys
-
-from . import Database, list2str, printErr, printMsg, printWarn
-
-__spec__.data = Database()
-__spec__.data.codeType = [
-    {
-        "codes": [
-            "D=u*JdO7&//+g7fsH33Xk*M*$7*u_.",
-            "=ev1=5u?$?-W5gf0n%w#5_7$%h__kq",
-            "Uc20dMPeVFq/~_+#&&fXugV_i&iA3Y",
-            "S50&+z5Z46#=1-Vh6Qt9jA@J1#4=!2",
-            "_4Jb&v22749_+Ei9&Oq1_!qcu*92r0",
-            "%$/fe9/y8q-j0A02pd9kk*IDGu20%_",
-            "Lqd4_8_%PrIP9oZC&uc3?K-A~Bp34U",
-            "6~8_nf=/xcQ01GiKKd@68MVWO$.9o7",
-            "h#sFad1l-Br497W654q7Ye95e.4I4k",
-            "74&UJR@cq!_9YekY/h-n~a$/!E+Q5Z",
-            "$2#B?@5AP2IEUjxpDC@*ZYl=8+e/Ab",
-            "701a_!*E#I.778my0!z877kBxCp-z=",
-            "K*uVq-=Z*8iY59/2c+aX3_MV.@*#Z_",
-            "?2~5kA!eXu_cT--N$?T-*.+9NY947Z",
-            ".!Wjz5NVOX3j7P1.bpC79.v24ls*K9",
-            "1pr&Ll0giv/lBA$B_18!i$1@232-%/",
-            "a-@99ii9&Z84zN.kh/!8-5f&rqvj98",
-            "jvS#5d6?Rt=u!NJ1!2UDX4?*=5R%8v",
-            "ENr.T+8i37*ZKMS*UM4=jq=56*12H1",
-            "j6D-SWshO/p4Yc87wr.Hq40j81_KG7",
-            "?23g7IBa9U4/9Xc4!o%438l&/46ZuG",
-            "Z1uLv&@058Oi_$50b?ox#3N4$_t4k0",
-            "0w?Q!Gs27JY#RbW6li4zS+9&T5j_##",
-            "37UHI5Q4AFV=v0A4P!zn!e_JTc9S93",
-            "72zH338x?7s3cAe/l@.W6J%WO#Z@/$",
-            "35fy*zV5w@ACWO3=S5u#Gj5l6beN@2",
-            "RGt86&1926@69_u95=4wyXI?=kHLJ6",
-            "U1qE!OC21*r+W0nm7k.X48+6k+&$l#",
-            "MU07fwRm1HdK00UZ2Jiu$_=I5t-2$X",
-            "!1k6*a_7SD/20~*/xCn#.*C8uu.X~D",
-            "v66A4U.a$?E8W_xXR$*=@90r6_9&Dp",
-            "u+G!#4WbG$h=4.p5._9OWZ6143h.8R",
-            "Wz77@!#yZ@5W27g23?6r@2~7l515X~",
-            "3~_p9CTPrJ.H9*TG370u#3rY6~ar=@",
-            "/=t+%p7hy&nkuhnsHiK#=oG~DuAX~4",
-            "w!!x?_U6X96QpKx937jb8DFNv1.lU0",
-            "~~!Y#78T95@3fV#DrB9$@9i6I?p39%",
-            "$f@CD$Y6Ov1+1#w9.*?8I2x?bafsu.",
-            "dzkRN=7w59dk9_#e&?4L#Nj@?+Tpl!",
-            "0d6X5_81GF-+/~2?wb=0?RPXqP952q",
-            "8s2z%5r5da4vm0J8dn@Km7y0dL!*te",
-            "+b#fG7*oVs4rN*1&.G+=G1%zO?#i/2",
-            "MxKR#-6ep@#Q+29kH5883XK=AJ#.H7",
-            "&1$z4$+44E79tn?2$@_.6.bU&8?RVw",
-            "@JF+pT55ydzR_5?Y_l@6S8_a/108$#",
-            "mD3e#5~13Z6s+V_cx7nm1Y/M4U=e.0",
-            "L9_VTQ.s7U=VRbC-#J5$7CE5-*9@vm",
-            "072#3n./b11eh-Q_*Q$G_r6?!&P0PY",
-            "kMkdLA=+h%C40D8uoC7/7_!X&Mb%=4",
-            "b68cXM25q6GJ4s5N#g$062+0.WrT9_",
-            "_5=9@avDV~UKbDod9~gw1g7A_jRb5_",
-            "JI%!ln.FNWNbqmDbo8=se+dJvo.W96",
-            "gNJamX*B!l/l#p9ag9Xi3Y%dy?j!NM",
-            "e=1=1bHh&n6.Sm3J8~1zU-g&o0?2rO",
-            "?uO50+d.9.j7H8HFw0aBP21$$1qt~i",
-            "#O!6uIse=7__DL-m-h9e88HdLj2jzm",
-            "OS~+5TtfjP5-kQecPM5Q+22Vhu!kY0",
-            "DVFEX14?U~b@t476VK72O&@ap.aB@V",
-            "n5dh!H-/-0W-%8?Q3X+_=26bNt=4@D",
-            "46KKmbX-R6N~-9l=&5f1k0#E4PIm71",
-            "!b$E9Typ#p+rM?#yQB50C442*gNMUs",
-            "TomYNZ-d3&i_%ySFi72WhY3L@-d~19",
-            "B31aV2!%ASH#q=19#tF6@1~j$BO69*",
-            "@.TF_*xhfzC!BggwP7N47/*_#dZekt",
-            "K.@B#*/A*Q8I-IG1qcRqD_4O%D1s?v",
-            "lfs58h2Mn_O!@8=4ip/393?=L!0@4g",
-            "pjTb*?f4*Xn1.B3ZLV3Y30r21M@L%L",
-            "XeUh/86@F.-7Gf6&WT2cCP%7%x@~a.",
-            "-/y.W6@*+H0M~kY@s$W0YXn&$2rjoh",
-            "1y82N28LC!6_7$9k49K4X5/1$1Kw63",
-            "pXYEJ09tu0cd#9#Lf/3w4u7R0c?i3p",
-            "9l6O$4rJD9/O82*6+wwiV#sBS9EV8I",
-            "QcL&tYKh4Q$cG1tx8.uM?0hth%E8O2",
-            "6$+Q@HZElj2csmX_OzGi5A-BR8i++_",
-            "Ie/a8ph=Y_1%l=DC!du~e61A8qMUu7",
-            "_nj%KGoz9&q-5V1=~&MnfYns1E171/",
-            "hg98U6oT$3Mq==97Hk9RVu#HtM$F+i",
-            "K=N409AL8~67fpL1IcT*6-9f4B125N",
-            "&AX4U3A0~hh%4%P11%y10$batOcf!~",
-            "UaKC$b$%uzk?0#-/0Zs18q6+1s8ImF",
-            "~7e$d#7!#QSw229hdM!3xFwI1_%/.q",
-            "xE6D12326RlIxi63j$&901w--GE9.1",
-            "ZZe*?23102IhIg4U&4$48f8OJ0+03w",
-            "_kT&!9*VZ1sE-OtZ71L?x4$@P272EC",
-            "uJ35g6gHiQky+gs60_h8+f=~t1-tF7",
-            "3Lu2O7Z%ZL2#/*z9_pFY=_7e-#qGOx",
-            "I0%2Phdd~I?6/Lw#MO98Jl7A*Cbv2W",
-            "D@s0qyF$aFl8/$53GWqA=1.&av#@!1",
-            "MG4%ZmhIod-e.0eqGO#VkfER8T2ttN",
-            "2q#f@8arUE8Uu?V56c&76jWR9#!2?0",
-            "4O5MQGM&h04=cH?P1!80dt+4&!a3d/",
-            "1oBK%s9/h2j!0+d08uAT9-_v_pMu=0",
-            "fC9ioP-I9/l2?wJH42W4#1+y5r-pe7",
-            "*x3PF8!@9_Jf5NUk@u4Zp-t@Fl0d_k",
-            "M!8gu53l92*O-R0F6W9$7~H%1/-025",
-            "0Dhm.%2~0R$/Db428x3YBv7ZB4/KYF",
-            "E=E&VuP&J$snh5D8kn1vz0.4mYsNh8",
-            "974KTXO3D6xJRkV/x$4.8+Q/xBnu%.",
-            "@78/cNGHf4i3i?2A~Q0p3RXUwI5!h1",
-            "46F6u.D1K1VNlywu9A5%_!xr?1y&CU",
-        ],
-        "decoder": __cmethst__.b64decode,
-        "encoder": __cmethst__.b64encode,
-    },
-    {
-        "codes": [
-            "3#$1/0?#a783BL0M.y?FIva06-MqOo",
-            "7Kcx#x?.F77C+F3B*SSCa$$+M*l9T7",
-            "oUGl8D__QhM.6Z&FA7-a8??34&Bmwe",
-            "7#U0+p#y4T4ke4&2*9vVDgp3OGn&+~",
-            "41IUP7HO0ENnT78v9%oU=m9a7NYM42",
-            "Mo5B$Q3jlNEtnQL1!fx2j.tvbI2c?X",
-            "#3z940+Z7%aqRy_3176@66B1m4?duK",
-            "2*Y177k1XHT=u%o!cT$#7e=Nv9V_g!",
-            "bK%4?K1?nQCzT45!!Fi0j7/%Q3YzaP",
-            "RI$Sv*4$@D@+V7X9~DRtcP5_8=8=+1",
-            "UIj8$Tgi&@sRk$34H55TP5*lN2gd2O",
-            "/&B&n8s011!26u@NL?XDZ*t5LtVP39",
-            "WtPT~r5D*#10o2-p4N_JvxxgD%@8FC",
-            "Nk2u4aljuFVm%+_P~W=L8969VDi_gj",
-            "W931W7Us#&B@2-@05oTJ9d&f66!JF8",
-            "?1Q#Ue-5!CUUmB+-jes1N8NzRHtS.i",
-            "%9G$Pq7UrN1.#!6&!W056=Z-70_Nu7",
-            "P0?l#3zh5BOB8pF2JVS*pF+d79cL0k",
-            "=1%.=@/A9D-=*EX0/Y#V#d8~Tyx?7G",
-            "P?/q@An*c.%U~81_36f+~k.=-6=6I6",
-            "5vf1@_=!&92-3X?=DWW.Xxk@JU56-0",
-            "6P8h0v?+IK?4FV23n.6o8T8my!M4_?",
-            "xD~p2?Mc/zSg+EZnQ$vG338b0P.3+l",
-            "6B_BVso6Z0l$TQ.q_wdkHs?lAE=TJ8",
-            "RsmMkc96SF_VG~=FN~UHWV1?8B7bGq",
-            "89N/5C9R6!+D!C9*-!393/WS1%rSUC",
-            "/76AEesbv-y7M#sRb/6d?U+65F$bh@",
-            "=6l5d5lRK4DIF6g.!qc3MP+U8_SB8c",
-            "Qy#$&S.50TJ3X5Ht0%5CS6v!=Zjf5J",
-            "avS&8BzVQ66HLA=_UbZDs1d=O+Fj.&",
-            "&Y!D43x8=N54S*M=?NF2o9_/2J=RRM",
-            "A0Ru9mq36&.z5z!5/zMD?j7PVW~sf.",
-            "0#Acz*yNpw8aOW&72sN!lPlaZ~%%u1",
-            "Zsq61qL44!IYZ!+*/2O4/5JZ4=4T#$",
-            "_&o_V~/+M&@3%04d9gKnb-81.XJQ@D",
-            "6953~~fF?Sj7KS107-m8vc7ykeSM~0",
-            "_M5s3LxmWO6.c$3?*IDHKjMpL?4nv9",
-            "S+3=0n14Oc+Yg?h31$7X/WF~jr8/4j",
-            "P~?3.-0-8O=9%xCt+Uyg$TfyX%5537",
-            "B%z-r!nS-z4DPIb4@11#c*fI=0?5+9",
-            "lTAUgd%fy+gNZ5Il9nFj?=98+~6Z!D",
-            "Wr9G_J=s?Yqkjs*G854?y$z_Z_=*AY",
-            "-e_@qQT&#uKQY7@LSD~q%G26-!m_qA",
-            "x_UcRS85r-N/KF*Cqarr+34~5+DpGV",
-            "0+C4#@TUxFv0qK@h513Qxo1nko6t2e",
-            "&=eU/1RCy_u+r+_is9Gx~S#PmS8I=_",
-            "9@8P5kWt73$Mq7WI/tc91!/4b9?+61",
-            "P20@_G02Vy4uZ8~.249&25ZMq-n&0g",
-            "d~#.23yZ%CR1OsS5ER3V&jp/!M13Hv",
-            "N-5Ae1f/0$6H872FU_7/o7iDY!5nn*",
-            "-m0?/?RUx55.@BH$1v0-S84Y@P2~2v",
-            "uX2deXaWU2#j@2K.@$AJJl2xz2KH!4",
-            "6eeK@@p7b/!L!#?u~F7+O5A1j7V?#e",
-            "G078b!4lQ3j79AK0=8~puE!0hDCFX7",
-            "E7k98P9Vq3L3yf?v.@qWGk&KBh-y8K",
-            "l8y%f3Lts3Ze*m4=R_!0Tiw/~r9%Ag",
-            "Slj&1Fs0.las22t2R=~N6Xhk7Md0Mt",
-            "GlB1dk*j8oGYJMhb*R1?m#lpsDhGQ+",
-            "--VhH+8y#XlA@H.53o1+.X$hRcZ8_t",
-            "hnMK0=VJ-&5e6?j34D3?/8?$5$xg8~",
-            "xhz!x0wN0p47B6v4W#3UC4%4#&6Y@=",
-            "a%*vBP_&5+650R#IzR0ylQ/14$6ykY",
-            "7KZ8YP68%dPm8S6FL3?A-f0eZ-8bPo",
-            "RF%g519j1R?84%*94tc87JfL$~Obpn",
-            "wd52IW87=&066MiW$#811ikXtHiB#Z",
-            "a6Wv~3rGn-u#4$133=dN$p5g9_?f48",
-            "%0!gazTjbg/02lAj_6g!3u9*a=r%6.",
-            "792Ha3@qHBKvdg#F@dlxDaw7L8*+!l",
-            "-/zCQG-81@e9v7Z7288**+%874nK8.",
-            "/9P=x5*&23~sB-mVNk%4?.T1d6Y.$c",
-            "1hi?2I5ylhYkhwcb@&3AMb.~1_EkCe",
-            "i92eYR69wV06B&j2a.q/KEKQtKk?2c",
-            "X6wCs4s#MDF_99D1No$~O$J22A4/q2",
-            "7m50Z7+~gHD_bT&X=vT@m32/D.q!%e",
-            "846?&zK=FIQd3.~5T6O?775.bQ=IC%",
-            "ht!3yKP9/Jmbdz!ikT-Ea$gTY3t_Q5",
-            "GUTd5Qe@6/NKv5=I3_I_u$DNmaN!A~",
-            "HGJi9%wAt~CZ@5=NPe~=F.5B6vnm7o",
-            "8r0+99-4.h8A3wG75vtvTlBJ18uXdV",
-            "B&*M74*@JdIMI.~L9f$d40r+s82o5b",
-            "NMH35$Ai0d_$==3%2#HySRuSE_.Q%Q",
-            "2o!7T~e?*H0m32?5?nS2C0k01o4pG?",
-            "=6_DM5EL68E*du%DrH6/261d7G9W0j",
-            "X~00jdxTeNnxA79nBKm9RCb1L5+L2=",
-            "h-*jAKP_2_cgkm3pKpg2~NFh2bNmFn",
-            "w~PXi_?4=9K648@=r814h$gYj=._/C",
-            "~f+fh0xfH/Zcf7iVj4L!4654S0s!r9",
-            "%e27TK7uj$7J$V*&?Y~5D3W7BA.n_3",
-            "NqclBn%q4t707110/@k40957o&438g",
-            "03P/NvSP0~QUSf_/Wm/&I76zTi2Oqv",
-            "D6C72l8_997~@Gt9aK9x$74qL~xqk_",
-            "5.-J2I6w22O4&n.4y3DzF3g#w~.*-4",
-            "_4/ct4v@b231yR.ZP6~590NXh4z-iD",
-            "sUBb90-Y4EEMq469K*Kj/w5Z8GU4P_",
-            "U7o=z$0!6Ous4EE+K+3?Yh08H6+dm&",
-            "7&OI6sTl7P8k$%U$0r+6RPw7la8A9V",
-            "z272?7XO1F@#kW7nPS&5r?+3--xG17",
-            "A5u+mXY_R.f0iz?7MwP1-4d$R#I_+X",
-            "4oGa84&H5ap8HA.U983~DQ_?8QDUgh",
-            "=U9V4Bs6z+t@BS74yHPl@8d490467o",
-        ],
-        "decoder": __cmethst__.b32decode,
-        "encoder": __cmethst__.b32encode,
-    },
-    {
-        "codes": [
-            "&ABCRe05$nxlulY%UrX3@$1C5=~5H_",
-            "k2RyF9FfXXm5NKRM03_r4b*2N5..m&",
-            "B!vX7NATP6V@8F3%S7~hRm%P&+vH%2",
-            "l_1=jP6W8lk43vQZ4Ye3$Jzm1_ut$B",
-            "cmOp/*a@U*#86wSzULM++e2Us4jsZU",
-            "3*nXuaxG2BklNE&uVPPw94AK4$oA5~",
-            "pv9Qe37_T_/K_xs*?ay6fWgy1-MKVW",
-            "BZf~d80Z2gFqX2K6ViG5yt4274R4Ob",
-            ".ELB/7o!U#JSt7c%9.0*s747Agz~/7",
-            "ichai&GndO62QB449WgkD*2O0CouR~",
-            "4#0F@@=S?R#-.780Jq1N885XNeVOAw",
-            "ic@$fBtCb+Ft5M~o%lR3~wBaVYgB&@",
-            "Ad4Mc4CeW/SR1q-$&izaC+!Q@043W9",
-            "!*Mv*eTL*2R+$W7XT7@@@L+00JolBf",
-            "XK*B4#Pfu79LJ0Nlup9=$Vx3@@n!t6",
-            "hV*kcP&%j3K!b3=~E6I?gOP3=!$PqQ",
-            "4%W.o@GaUO+Oj1Z3Py1#6A3%F2z5~7",
-            "eqU#&b0_=1dc-8@/89X7RK=CItn*6~",
-            "91fqX2=tK3t9H!7&PvUg4V31JhrUrg",
-            "KX4m49q5NhZj/*8a#x&8#w8W#5MZ$+",
-            "N@B7pU2?ph$GC3JLHq/p3q!0jI%L+i",
-            "$COEn+6f?=1tR7At!8I9#.NW-rO71u",
-            "07xo/!lf*UFr33i$1?_@FH=PWwcE/#",
-            "4qe5.%Cq5R6/EE_-h0=3c90xT&ZT3!",
-            "gKP4!Q.=S9jcgho8A&1uA53xk24Go8",
-            "8@D6*-l7orPocT9_mhj84O1_i5-85!",
-            "7MoFFl0k/t~cA%H8Tg0+ELJLa1.T12",
-            "f~#3!k2D#Q1M~zP&6H7~*$3w/A48N4",
-            ".s=9_rA/*V?=Z19P1F65uiJSpl.@84",
-            "@h7=j3hd+-oLHy$%8Zw?Ha+=u118F/",
-            ".8WWn4xZd*VvU%TE5a%3OYb=_$%2Vz",
-            "U?@2VW87NE8jXf73M=~-67p#A%X?_5",
-            "=T-EZ3nv#?7M9V2Y~0EsucV@KR0&/v",
-            "63k537I35=1Qp~L_J2K1so+z.aG9Og",
-            "1$Ch#F*OrHDnHR74#90K@9=8_6Z23m",
-            "J1&R4j1uV4b2F72Y=&l#Eizr3E-%-U",
-            "RD/+!vvxOg1VR~UDbz&CJ%f+9l5LVN",
-            "m23snf5p?g3ilf9LlB.32A3JM!6g!Y",
-            "+kR8a+jF!s@pO#290qM/DZ5_hO3K4G",
-            "~6D%~F&2t=*c+acg+l17y+sQp6q#P_",
-            "96!sui9z1FG/Y9b+Z5G0zMO5CHCam=",
-            "6?7036Z-!@F2yH1Y/4rTl-#VDy?~nI",
-            "Uci!*1XeT?0*p-&8m!m3LS!@!fXmx!",
-            "Rzz%o9WZ!=4kMDS1-_Od=9-s+09fk8",
-            "&~Q6_!8T/_#67b4G.FkZ.8qaR9IS%m",
-            "4o$=9n614UnT3nP3Q~x!@9F9W8$2_d",
-            "2w/~+O*cd~dtqgC.Ma865475zo/T%Q",
-            "l9Oy16254TTb~Gd9k?irU#+8QR=7K0",
-            "!J.Y730=5GPplJGh8e7&z0*8jJWO65",
-            "@&$Y&@q#Y73z06pQ&4A.+jnx56%Tvc",
-            "~jy=Wnp#_3LiuKNV5C5eB33V!M@lC!",
-            "c5=O#+#H6d48.$A2se4!2A7wm6Tlzs",
-            "=48zt4+54TO1246r5yL!gb4Mb046W%",
-            "00cVm6-$7Ow2.#B*1@&+M45_uf73_x",
-            "wjYy$5%TO.w68E7_6T*x1C~2CstuqG",
-            ".?j5nUmd!J18t2y&467D9~3ju9~m_w",
-            "nRx/_qM//ADs4uBS32$S45Q-%nSiLH",
-            "M~FK6P2%tG$2V3hM7c6&4@$jszw@&V",
-            "+DWwppWyUr/@/C=7fz7pa%4+@-6RT9",
-            ".~38V0!SKv1LoSW67+vCC33n7%LWHZ",
-            "%T&?4A*.j6JTHI=.+_423voK3xr$D.",
-            "Qqei6cbTHa0@408Zqn8_U8xm$GfX%=",
-            "$3GkC-Z2.V_4#zs+_I6PVO&fvEc.Dw",
-            "9z-k6EnE1g%*&_vpY!91/wO1h$30JC",
-            "N%2BOL_+#8J8-CFfB-_!~%7QM73?H9",
-            "pdq9i+be&YRhes8t%3y=i5R9%#C755",
-            "8+_H9~Z--%?M3$wp323qWP*UsT7d.g",
-            "R%10jFaGS5BQTF_?Mq0_+E%gx6aJK3",
-            "=.UrzP736$t.S7q5vO+r1uxf@G9bm4",
-            "acsQ.H&/e=~6QuN/j1130x*#w738SD",
-            "vW3e_*0Zblz2-4w2V+6P9ewZ*@+2~J",
-            "yae210jf8Wd945YH2qD9iHTHgJ4-?7",
-            "5c69*-H!7$W0vh/f91@g687Kl$1Im0",
-            "5#5QRB.5IW9h*7zzxMj@@L8o6s7=82",
-            "Mgkxsi=$k1PfWBQYSFcOCo8*$8/BMe",
-            "7XvN+2v4Vo7ux9I3Ob584u7J99T8Mu",
-            "28/3%-u5d?*KpK6SK%5.f?Ug!7yKT0",
-            "!4zv3X8ElbSF8IK?69//_F+L*ZYyVl",
-            "3.oax6YRKf&zJbyf@w-pX@#n?qMxZ1",
-            "dK!8n0_-S72xqyr26R6HL$N59~o97D",
-            "Sm6SeY~mGT%j1306z=hQ@7MPcr?k2v",
-            "~A.*6Ln7am57&A/6sXJO~ih3no6J7x",
-            "X5hi7?=U35%D7j-@8wU4X9w7*z9soI",
-            "O5W/V!QO.wh6$DA92mM!+h*Wrr7Z8T",
-            "5#?!04#e5W25EH2GS-?#5fED89J75g",
-            "RRg%WpcpHz%QVd6c331$/?3?@4v=e.",
-            "1q8C&P088X7b7033gA4c-Ud&BF&ZJ/",
-            "Dr3X=sP=/L8K3G~6v?ulRVMtZ27NB5",
-            "Dj#dF/bEG*--9UR.4Me3fu262!f6*K",
-            "&TZ+qA?7JaU&rtp?e0?54-+NY21x2.",
-            "QKN657uSAk4j601?wF*5/MQ1dHUQgI",
-            "6fy?jTV+dN.Z6to_c.+8_Ds32e83QV",
-            "7QFb?hE%fE6mb01~4*2D_Pw$po_741",
-            "Vw9.2PE_t687L$=47W5wQMxTcE487#",
-            "ClL%$i16iCi1F0073ki*2G1%Z3y$&&",
-            "6Ot&/W?7fqg?65!XM433$7l4mh84x+",
-            "8@Gf6O+ip&n?qzR@EjeN8ZgB.0SsDj",
-            "~a_uwUo=+O!5tk49m96tQ/X%unFz??",
-            "0KKlGz$7wR%.VF3086n_&@454_l_7O",
-            "K0r.44XK5@N~NF*9K2+5b+Hnml_A*3",
-        ],
-        "decoder": __cmethst__.b16decode,
-        "encoder": __cmethst__.b16encode,
-    },
-]
-
-__spec__.data.compilerData = {
-    "name": "protStringCompiler",
-    "version": "1.1",
-    "codeListID": "9611699982",
-}
-
-__spec__.data.compileOptions = [
-    {"name": "type", "options": ["py", "data"], "default": "py"}
-]
-
-
-def encode(input, type="file"):
-    if type == "file":
-        pyFile = open(input)
-        pyData = pyFile.read()
-        pyFile.close()
-    elif type in ["string", "str"]:
-        pyData = input
-    else:
-        printErr("type is invalid")
-        return
-    encType = random.choice(__spec__.data.codeType)
-    encCode = random.choice(encType["codes"])
-    encFunc = encType["encoder"]
-    encData = encCode + "\n" + str(encFunc(bytes(pyData, "utf-8")))[2:-1]
-    return encData
-
-
-def encrypt(input, output):
-    encData = encode(input)
-    encFile = open(output, "w")
-    encFile.write(encData)
-    encFile.flush()
-    encFile.close()
-
-
-def execute(input, type="file"):
-    output = "exec"
-    if type.startswith("out$"):
-        output = "return"
-        type = type[4:]
-    if type == "file":
-        pyFile = open(input)
-        pyData = pyFile.read()
-        pyFile.close()
-    elif type in ["string", "str"]:
-        pyData = input
-    else:
-        printErr("type is invalid")
-        return
-    pyLines = pyData.splitlines()
-    encCode = pyLines[0]
-    encData = pyLines[-1]
-    encFunc = None
-    for t in __spec__.data.codeType:
-        for c in t["codes"]:
-            if c == encCode:
-                encFunc = t["decoder"]
-    decData = list2str(str(encFunc(bytes(encData, "utf-8")))[2:-1].splitlines(), "\n")
-    if output == "exec":
-        decFile = open("decodedfile.py", "w")
-        decFile.write(decData)
-        decFile.flush()
-        decFile.close()
-        decMod = __import__("decodedfile")
-        del decMod
-        del sys.modules["decodedfile"]
-        os.remove("decodedfile")
-    else:
-        return decData
+import base64 as __cmethst__
+import os
+import random
+import sys
+
+from . import Database, list2str, printErr, printMsg, printWarn
+
+__spec__.data = Database()
+__spec__.data.codeType = [
+    {
+        "codes": [
+            "D=u*JdO7&//+g7fsH33Xk*M*$7*u_.",
+            "=ev1=5u?$?-W5gf0n%w#5_7$%h__kq",
+            "Uc20dMPeVFq/~_+#&&fXugV_i&iA3Y",
+            "S50&+z5Z46#=1-Vh6Qt9jA@J1#4=!2",
+            "_4Jb&v22749_+Ei9&Oq1_!qcu*92r0",
+            "%$/fe9/y8q-j0A02pd9kk*IDGu20%_",
+            "Lqd4_8_%PrIP9oZC&uc3?K-A~Bp34U",
+            "6~8_nf=/xcQ01GiKKd@68MVWO$.9o7",
+            "h#sFad1l-Br497W654q7Ye95e.4I4k",
+            "74&UJR@cq!_9YekY/h-n~a$/!E+Q5Z",
+            "$2#B?@5AP2IEUjxpDC@*ZYl=8+e/Ab",
+            "701a_!*E#I.778my0!z877kBxCp-z=",
+            "K*uVq-=Z*8iY59/2c+aX3_MV.@*#Z_",
+            "?2~5kA!eXu_cT--N$?T-*.+9NY947Z",
+            ".!Wjz5NVOX3j7P1.bpC79.v24ls*K9",
+            "1pr&Ll0giv/lBA$B_18!i$1@232-%/",
+            "a-@99ii9&Z84zN.kh/!8-5f&rqvj98",
+            "jvS#5d6?Rt=u!NJ1!2UDX4?*=5R%8v",
+            "ENr.T+8i37*ZKMS*UM4=jq=56*12H1",
+            "j6D-SWshO/p4Yc87wr.Hq40j81_KG7",
+            "?23g7IBa9U4/9Xc4!o%438l&/46ZuG",
+            "Z1uLv&@058Oi_$50b?ox#3N4$_t4k0",
+            "0w?Q!Gs27JY#RbW6li4zS+9&T5j_##",
+            "37UHI5Q4AFV=v0A4P!zn!e_JTc9S93",
+            "72zH338x?7s3cAe/l@.W6J%WO#Z@/$",
+            "35fy*zV5w@ACWO3=S5u#Gj5l6beN@2",
+            "RGt86&1926@69_u95=4wyXI?=kHLJ6",
+            "U1qE!OC21*r+W0nm7k.X48+6k+&$l#",
+            "MU07fwRm1HdK00UZ2Jiu$_=I5t-2$X",
+            "!1k6*a_7SD/20~*/xCn#.*C8uu.X~D",
+            "v66A4U.a$?E8W_xXR$*=@90r6_9&Dp",
+            "u+G!#4WbG$h=4.p5._9OWZ6143h.8R",
+            "Wz77@!#yZ@5W27g23?6r@2~7l515X~",
+            "3~_p9CTPrJ.H9*TG370u#3rY6~ar=@",
+            "/=t+%p7hy&nkuhnsHiK#=oG~DuAX~4",
+            "w!!x?_U6X96QpKx937jb8DFNv1.lU0",
+            "~~!Y#78T95@3fV#DrB9$@9i6I?p39%",
+            "$f@CD$Y6Ov1+1#w9.*?8I2x?bafsu.",
+            "dzkRN=7w59dk9_#e&?4L#Nj@?+Tpl!",
+            "0d6X5_81GF-+/~2?wb=0?RPXqP952q",
+            "8s2z%5r5da4vm0J8dn@Km7y0dL!*te",
+            "+b#fG7*oVs4rN*1&.G+=G1%zO?#i/2",
+            "MxKR#-6ep@#Q+29kH5883XK=AJ#.H7",
+            "&1$z4$+44E79tn?2$@_.6.bU&8?RVw",
+            "@JF+pT55ydzR_5?Y_l@6S8_a/108$#",
+            "mD3e#5~13Z6s+V_cx7nm1Y/M4U=e.0",
+            "L9_VTQ.s7U=VRbC-#J5$7CE5-*9@vm",
+            "072#3n./b11eh-Q_*Q$G_r6?!&P0PY",
+            "kMkdLA=+h%C40D8uoC7/7_!X&Mb%=4",
+            "b68cXM25q6GJ4s5N#g$062+0.WrT9_",
+            "_5=9@avDV~UKbDod9~gw1g7A_jRb5_",
+            "JI%!ln.FNWNbqmDbo8=se+dJvo.W96",
+            "gNJamX*B!l/l#p9ag9Xi3Y%dy?j!NM",
+            "e=1=1bHh&n6.Sm3J8~1zU-g&o0?2rO",
+            "?uO50+d.9.j7H8HFw0aBP21$$1qt~i",
+            "#O!6uIse=7__DL-m-h9e88HdLj2jzm",
+            "OS~+5TtfjP5-kQecPM5Q+22Vhu!kY0",
+            "DVFEX14?U~b@t476VK72O&@ap.aB@V",
+            "n5dh!H-/-0W-%8?Q3X+_=26bNt=4@D",
+            "46KKmbX-R6N~-9l=&5f1k0#E4PIm71",
+            "!b$E9Typ#p+rM?#yQB50C442*gNMUs",
+            "TomYNZ-d3&i_%ySFi72WhY3L@-d~19",
+            "B31aV2!%ASH#q=19#tF6@1~j$BO69*",
+            "@.TF_*xhfzC!BggwP7N47/*_#dZekt",
+            "K.@B#*/A*Q8I-IG1qcRqD_4O%D1s?v",
+            "lfs58h2Mn_O!@8=4ip/393?=L!0@4g",
+            "pjTb*?f4*Xn1.B3ZLV3Y30r21M@L%L",
+            "XeUh/86@F.-7Gf6&WT2cCP%7%x@~a.",
+            "-/y.W6@*+H0M~kY@s$W0YXn&$2rjoh",
+            "1y82N28LC!6_7$9k49K4X5/1$1Kw63",
+            "pXYEJ09tu0cd#9#Lf/3w4u7R0c?i3p",
+            "9l6O$4rJD9/O82*6+wwiV#sBS9EV8I",
+            "QcL&tYKh4Q$cG1tx8.uM?0hth%E8O2",
+            "6$+Q@HZElj2csmX_OzGi5A-BR8i++_",
+            "Ie/a8ph=Y_1%l=DC!du~e61A8qMUu7",
+            "_nj%KGoz9&q-5V1=~&MnfYns1E171/",
+            "hg98U6oT$3Mq==97Hk9RVu#HtM$F+i",
+            "K=N409AL8~67fpL1IcT*6-9f4B125N",
+            "&AX4U3A0~hh%4%P11%y10$batOcf!~",
+            "UaKC$b$%uzk?0#-/0Zs18q6+1s8ImF",
+            "~7e$d#7!#QSw229hdM!3xFwI1_%/.q",
+            "xE6D12326RlIxi63j$&901w--GE9.1",
+            "ZZe*?23102IhIg4U&4$48f8OJ0+03w",
+            "_kT&!9*VZ1sE-OtZ71L?x4$@P272EC",
+            "uJ35g6gHiQky+gs60_h8+f=~t1-tF7",
+            "3Lu2O7Z%ZL2#/*z9_pFY=_7e-#qGOx",
+            "I0%2Phdd~I?6/Lw#MO98Jl7A*Cbv2W",
+            "D@s0qyF$aFl8/$53GWqA=1.&av#@!1",
+            "MG4%ZmhIod-e.0eqGO#VkfER8T2ttN",
+            "2q#f@8arUE8Uu?V56c&76jWR9#!2?0",
+            "4O5MQGM&h04=cH?P1!80dt+4&!a3d/",
+            "1oBK%s9/h2j!0+d08uAT9-_v_pMu=0",
+            "fC9ioP-I9/l2?wJH42W4#1+y5r-pe7",
+            "*x3PF8!@9_Jf5NUk@u4Zp-t@Fl0d_k",
+            "M!8gu53l92*O-R0F6W9$7~H%1/-025",
+            "0Dhm.%2~0R$/Db428x3YBv7ZB4/KYF",
+            "E=E&VuP&J$snh5D8kn1vz0.4mYsNh8",
+            "974KTXO3D6xJRkV/x$4.8+Q/xBnu%.",
+            "@78/cNGHf4i3i?2A~Q0p3RXUwI5!h1",
+            "46F6u.D1K1VNlywu9A5%_!xr?1y&CU",
+        ],
+        "decoder": __cmethst__.b64decode,
+        "encoder": __cmethst__.b64encode,
+    },
+    {
+        "codes": [
+            "3#$1/0?#a783BL0M.y?FIva06-MqOo",
+            "7Kcx#x?.F77C+F3B*SSCa$$+M*l9T7",
+            "oUGl8D__QhM.6Z&FA7-a8??34&Bmwe",
+            "7#U0+p#y4T4ke4&2*9vVDgp3OGn&+~",
+            "41IUP7HO0ENnT78v9%oU=m9a7NYM42",
+            "Mo5B$Q3jlNEtnQL1!fx2j.tvbI2c?X",
+            "#3z940+Z7%aqRy_3176@66B1m4?duK",
+            "2*Y177k1XHT=u%o!cT$#7e=Nv9V_g!",
+            "bK%4?K1?nQCzT45!!Fi0j7/%Q3YzaP",
+            "RI$Sv*4$@D@+V7X9~DRtcP5_8=8=+1",
+            "UIj8$Tgi&@sRk$34H55TP5*lN2gd2O",
+            "/&B&n8s011!26u@NL?XDZ*t5LtVP39",
+            "WtPT~r5D*#10o2-p4N_JvxxgD%@8FC",
+            "Nk2u4aljuFVm%+_P~W=L8969VDi_gj",
+            "W931W7Us#&B@2-@05oTJ9d&f66!JF8",
+            "?1Q#Ue-5!CUUmB+-jes1N8NzRHtS.i",
+            "%9G$Pq7UrN1.#!6&!W056=Z-70_Nu7",
+            "P0?l#3zh5BOB8pF2JVS*pF+d79cL0k",
+            "=1%.=@/A9D-=*EX0/Y#V#d8~Tyx?7G",
+            "P?/q@An*c.%U~81_36f+~k.=-6=6I6",
+            "5vf1@_=!&92-3X?=DWW.Xxk@JU56-0",
+            "6P8h0v?+IK?4FV23n.6o8T8my!M4_?",
+            "xD~p2?Mc/zSg+EZnQ$vG338b0P.3+l",
+            "6B_BVso6Z0l$TQ.q_wdkHs?lAE=TJ8",
+            "RsmMkc96SF_VG~=FN~UHWV1?8B7bGq",
+            "89N/5C9R6!+D!C9*-!393/WS1%rSUC",
+            "/76AEesbv-y7M#sRb/6d?U+65F$bh@",
+            "=6l5d5lRK4DIF6g.!qc3MP+U8_SB8c",
+            "Qy#$&S.50TJ3X5Ht0%5CS6v!=Zjf5J",
+            "avS&8BzVQ66HLA=_UbZDs1d=O+Fj.&",
+            "&Y!D43x8=N54S*M=?NF2o9_/2J=RRM",
+            "A0Ru9mq36&.z5z!5/zMD?j7PVW~sf.",
+            "0#Acz*yNpw8aOW&72sN!lPlaZ~%%u1",
+            "Zsq61qL44!IYZ!+*/2O4/5JZ4=4T#$",
+            "_&o_V~/+M&@3%04d9gKnb-81.XJQ@D",
+            "6953~~fF?Sj7KS107-m8vc7ykeSM~0",
+            "_M5s3LxmWO6.c$3?*IDHKjMpL?4nv9",
+            "S+3=0n14Oc+Yg?h31$7X/WF~jr8/4j",
+            "P~?3.-0-8O=9%xCt+Uyg$TfyX%5537",
+            "B%z-r!nS-z4DPIb4@11#c*fI=0?5+9",
+            "lTAUgd%fy+gNZ5Il9nFj?=98+~6Z!D",
+            "Wr9G_J=s?Yqkjs*G854?y$z_Z_=*AY",
+            "-e_@qQT&#uKQY7@LSD~q%G26-!m_qA",
+            "x_UcRS85r-N/KF*Cqarr+34~5+DpGV",
+            "0+C4#@TUxFv0qK@h513Qxo1nko6t2e",
+            "&=eU/1RCy_u+r+_is9Gx~S#PmS8I=_",
+            "9@8P5kWt73$Mq7WI/tc91!/4b9?+61",
+            "P20@_G02Vy4uZ8~.249&25ZMq-n&0g",
+            "d~#.23yZ%CR1OsS5ER3V&jp/!M13Hv",
+            "N-5Ae1f/0$6H872FU_7/o7iDY!5nn*",
+            "-m0?/?RUx55.@BH$1v0-S84Y@P2~2v",
+            "uX2deXaWU2#j@2K.@$AJJl2xz2KH!4",
+            "6eeK@@p7b/!L!#?u~F7+O5A1j7V?#e",
+            "G078b!4lQ3j79AK0=8~puE!0hDCFX7",
+            "E7k98P9Vq3L3yf?v.@qWGk&KBh-y8K",
+            "l8y%f3Lts3Ze*m4=R_!0Tiw/~r9%Ag",
+            "Slj&1Fs0.las22t2R=~N6Xhk7Md0Mt",
+            "GlB1dk*j8oGYJMhb*R1?m#lpsDhGQ+",
+            "--VhH+8y#XlA@H.53o1+.X$hRcZ8_t",
+            "hnMK0=VJ-&5e6?j34D3?/8?$5$xg8~",
+            "xhz!x0wN0p47B6v4W#3UC4%4#&6Y@=",
+            "a%*vBP_&5+650R#IzR0ylQ/14$6ykY",
+            "7KZ8YP68%dPm8S6FL3?A-f0eZ-8bPo",
+            "RF%g519j1R?84%*94tc87JfL$~Obpn",
+            "wd52IW87=&066MiW$#811ikXtHiB#Z",
+            "a6Wv~3rGn-u#4$133=dN$p5g9_?f48",
+            "%0!gazTjbg/02lAj_6g!3u9*a=r%6.",
+            "792Ha3@qHBKvdg#F@dlxDaw7L8*+!l",
+            "-/zCQG-81@e9v7Z7288**+%874nK8.",
+            "/9P=x5*&23~sB-mVNk%4?.T1d6Y.$c",
+            "1hi?2I5ylhYkhwcb@&3AMb.~1_EkCe",
+            "i92eYR69wV06B&j2a.q/KEKQtKk?2c",
+            "X6wCs4s#MDF_99D1No$~O$J22A4/q2",
+            "7m50Z7+~gHD_bT&X=vT@m32/D.q!%e",
+            "846?&zK=FIQd3.~5T6O?775.bQ=IC%",
+            "ht!3yKP9/Jmbdz!ikT-Ea$gTY3t_Q5",
+            "GUTd5Qe@6/NKv5=I3_I_u$DNmaN!A~",
+            "HGJi9%wAt~CZ@5=NPe~=F.5B6vnm7o",
+            "8r0+99-4.h8A3wG75vtvTlBJ18uXdV",
+            "B&*M74*@JdIMI.~L9f$d40r+s82o5b",
+            "NMH35$Ai0d_$==3%2#HySRuSE_.Q%Q",
+            "2o!7T~e?*H0m32?5?nS2C0k01o4pG?",
+            "=6_DM5EL68E*du%DrH6/261d7G9W0j",
+            "X~00jdxTeNnxA79nBKm9RCb1L5+L2=",
+            "h-*jAKP_2_cgkm3pKpg2~NFh2bNmFn",
+            "w~PXi_?4=9K648@=r814h$gYj=._/C",
+            "~f+fh0xfH/Zcf7iVj4L!4654S0s!r9",
+            "%e27TK7uj$7J$V*&?Y~5D3W7BA.n_3",
+            "NqclBn%q4t707110/@k40957o&438g",
+            "03P/NvSP0~QUSf_/Wm/&I76zTi2Oqv",
+            "D6C72l8_997~@Gt9aK9x$74qL~xqk_",
+            "5.-J2I6w22O4&n.4y3DzF3g#w~.*-4",
+            "_4/ct4v@b231yR.ZP6~590NXh4z-iD",
+            "sUBb90-Y4EEMq469K*Kj/w5Z8GU4P_",
+            "U7o=z$0!6Ous4EE+K+3?Yh08H6+dm&",
+            "7&OI6sTl7P8k$%U$0r+6RPw7la8A9V",
+            "z272?7XO1F@#kW7nPS&5r?+3--xG17",
+            "A5u+mXY_R.f0iz?7MwP1-4d$R#I_+X",
+            "4oGa84&H5ap8HA.U983~DQ_?8QDUgh",
+            "=U9V4Bs6z+t@BS74yHPl@8d490467o",
+        ],
+        "decoder": __cmethst__.b32decode,
+        "encoder": __cmethst__.b32encode,
+    },
+    {
+        "codes": [
+            "&ABCRe05$nxlulY%UrX3@$1C5=~5H_",
+            "k2RyF9FfXXm5NKRM03_r4b*2N5..m&",
+            "B!vX7NATP6V@8F3%S7~hRm%P&+vH%2",
+            "l_1=jP6W8lk43vQZ4Ye3$Jzm1_ut$B",
+            "cmOp/*a@U*#86wSzULM++e2Us4jsZU",
+            "3*nXuaxG2BklNE&uVPPw94AK4$oA5~",
+            "pv9Qe37_T_/K_xs*?ay6fWgy1-MKVW",
+            "BZf~d80Z2gFqX2K6ViG5yt4274R4Ob",
+            ".ELB/7o!U#JSt7c%9.0*s747Agz~/7",
+            "ichai&GndO62QB449WgkD*2O0CouR~",
+            "4#0F@@=S?R#-.780Jq1N885XNeVOAw",
+            "ic@$fBtCb+Ft5M~o%lR3~wBaVYgB&@",
+            "Ad4Mc4CeW/SR1q-$&izaC+!Q@043W9",
+            "!*Mv*eTL*2R+$W7XT7@@@L+00JolBf",
+            "XK*B4#Pfu79LJ0Nlup9=$Vx3@@n!t6",
+            "hV*kcP&%j3K!b3=~E6I?gOP3=!$PqQ",
+            "4%W.o@GaUO+Oj1Z3Py1#6A3%F2z5~7",
+            "eqU#&b0_=1dc-8@/89X7RK=CItn*6~",
+            "91fqX2=tK3t9H!7&PvUg4V31JhrUrg",
+            "KX4m49q5NhZj/*8a#x&8#w8W#5MZ$+",
+            "N@B7pU2?ph$GC3JLHq/p3q!0jI%L+i",
+            "$COEn+6f?=1tR7At!8I9#.NW-rO71u",
+            "07xo/!lf*UFr33i$1?_@FH=PWwcE/#",
+            "4qe5.%Cq5R6/EE_-h0=3c90xT&ZT3!",
+            "gKP4!Q.=S9jcgho8A&1uA53xk24Go8",
+            "8@D6*-l7orPocT9_mhj84O1_i5-85!",
+            "7MoFFl0k/t~cA%H8Tg0+ELJLa1.T12",
+            "f~#3!k2D#Q1M~zP&6H7~*$3w/A48N4",
+            ".s=9_rA/*V?=Z19P1F65uiJSpl.@84",
+            "@h7=j3hd+-oLHy$%8Zw?Ha+=u118F/",
+            ".8WWn4xZd*VvU%TE5a%3OYb=_$%2Vz",
+            "U?@2VW87NE8jXf73M=~-67p#A%X?_5",
+            "=T-EZ3nv#?7M9V2Y~0EsucV@KR0&/v",
+            "63k537I35=1Qp~L_J2K1so+z.aG9Og",
+            "1$Ch#F*OrHDnHR74#90K@9=8_6Z23m",
+            "J1&R4j1uV4b2F72Y=&l#Eizr3E-%-U",
+            "RD/+!vvxOg1VR~UDbz&CJ%f+9l5LVN",
+            "m23snf5p?g3ilf9LlB.32A3JM!6g!Y",
+            "+kR8a+jF!s@pO#290qM/DZ5_hO3K4G",
+            "~6D%~F&2t=*c+acg+l17y+sQp6q#P_",
+            "96!sui9z1FG/Y9b+Z5G0zMO5CHCam=",
+            "6?7036Z-!@F2yH1Y/4rTl-#VDy?~nI",
+            "Uci!*1XeT?0*p-&8m!m3LS!@!fXmx!",
+            "Rzz%o9WZ!=4kMDS1-_Od=9-s+09fk8",
+            "&~Q6_!8T/_#67b4G.FkZ.8qaR9IS%m",
+            "4o$=9n614UnT3nP3Q~x!@9F9W8$2_d",
+            "2w/~+O*cd~dtqgC.Ma865475zo/T%Q",
+            "l9Oy16254TTb~Gd9k?irU#+8QR=7K0",
+            "!J.Y730=5GPplJGh8e7&z0*8jJWO65",
+            "@&$Y&@q#Y73z06pQ&4A.+jnx56%Tvc",
+            "~jy=Wnp#_3LiuKNV5C5eB33V!M@lC!",
+            "c5=O#+#H6d48.$A2se4!2A7wm6Tlzs",
+            "=48zt4+54TO1246r5yL!gb4Mb046W%",
+            "00cVm6-$7Ow2.#B*1@&+M45_uf73_x",
+            "wjYy$5%TO.w68E7_6T*x1C~2CstuqG",
+            ".?j5nUmd!J18t2y&467D9~3ju9~m_w",
+            "nRx/_qM//ADs4uBS32$S45Q-%nSiLH",
+            "M~FK6P2%tG$2V3hM7c6&4@$jszw@&V",
+            "+DWwppWyUr/@/C=7fz7pa%4+@-6RT9",
+            ".~38V0!SKv1LoSW67+vCC33n7%LWHZ",
+            "%T&?4A*.j6JTHI=.+_423voK3xr$D.",
+            "Qqei6cbTHa0@408Zqn8_U8xm$GfX%=",
+            "$3GkC-Z2.V_4#zs+_I6PVO&fvEc.Dw",
+            "9z-k6EnE1g%*&_vpY!91/wO1h$30JC",
+            "N%2BOL_+#8J8-CFfB-_!~%7QM73?H9",
+            "pdq9i+be&YRhes8t%3y=i5R9%#C755",
+            "8+_H9~Z--%?M3$wp323qWP*UsT7d.g",
+            "R%10jFaGS5BQTF_?Mq0_+E%gx6aJK3",
+            "=.UrzP736$t.S7q5vO+r1uxf@G9bm4",
+            "acsQ.H&/e=~6QuN/j1130x*#w738SD",
+            "vW3e_*0Zblz2-4w2V+6P9ewZ*@+2~J",
+            "yae210jf8Wd945YH2qD9iHTHgJ4-?7",
+            "5c69*-H!7$W0vh/f91@g687Kl$1Im0",
+            "5#5QRB.5IW9h*7zzxMj@@L8o6s7=82",
+            "Mgkxsi=$k1PfWBQYSFcOCo8*$8/BMe",
+            "7XvN+2v4Vo7ux9I3Ob584u7J99T8Mu",
+            "28/3%-u5d?*KpK6SK%5.f?Ug!7yKT0",
+            "!4zv3X8ElbSF8IK?69//_F+L*ZYyVl",
+            "3.oax6YRKf&zJbyf@w-pX@#n?qMxZ1",
+            "dK!8n0_-S72xqyr26R6HL$N59~o97D",
+            "Sm6SeY~mGT%j1306z=hQ@7MPcr?k2v",
+            "~A.*6Ln7am57&A/6sXJO~ih3no6J7x",
+            "X5hi7?=U35%D7j-@8wU4X9w7*z9soI",
+            "O5W/V!QO.wh6$DA92mM!+h*Wrr7Z8T",
+            "5#?!04#e5W25EH2GS-?#5fED89J75g",
+            "RRg%WpcpHz%QVd6c331$/?3?@4v=e.",
+            "1q8C&P088X7b7033gA4c-Ud&BF&ZJ/",
+            "Dr3X=sP=/L8K3G~6v?ulRVMtZ27NB5",
+            "Dj#dF/bEG*--9UR.4Me3fu262!f6*K",
+            "&TZ+qA?7JaU&rtp?e0?54-+NY21x2.",
+            "QKN657uSAk4j601?wF*5/MQ1dHUQgI",
+            "6fy?jTV+dN.Z6to_c.+8_Ds32e83QV",
+            "7QFb?hE%fE6mb01~4*2D_Pw$po_741",
+            "Vw9.2PE_t687L$=47W5wQMxTcE487#",
+            "ClL%$i16iCi1F0073ki*2G1%Z3y$&&",
+            "6Ot&/W?7fqg?65!XM433$7l4mh84x+",
+            "8@Gf6O+ip&n?qzR@EjeN8ZgB.0SsDj",
+            "~a_uwUo=+O!5tk49m96tQ/X%unFz??",
+            "0KKlGz$7wR%.VF3086n_&@454_l_7O",
+            "K0r.44XK5@N~NF*9K2+5b+Hnml_A*3",
+        ],
+        "decoder": __cmethst__.b16decode,
+        "encoder": __cmethst__.b16encode,
+    },
+]
+
+__spec__.data.compilerData = {
+    "name": "protStringCompiler",
+    "version": "1.1",
+    "codeListID": "9611699982",
+}
+
+__spec__.data.compileOptions = [
+    {"name": "type", "options": ["py", "data"], "default": "py"}
+]
+
+
+def encode(input, type="file"):
+    if type == "file":
+        pyFile = open(input)
+        pyData = pyFile.read()
+        pyFile.close()
+    elif type in ["string", "str"]:
+        pyData = input
+    else:
+        printErr("type is invalid")
+        return
+    encType = random.choice(__spec__.data.codeType)
+    encCode = random.choice(encType["codes"])
+    encFunc = encType["encoder"]
+    encData = encCode + "\n" + str(encFunc(bytes(pyData, "utf-8")))[2:-1]
+    return encData
+
+
+def encrypt(input, output):
+    encData = encode(input)
+    encFile = open(output, "w")
+    encFile.write(encData)
+    encFile.flush()
+    encFile.close()
+
+
+def execute(input, type="file"):
+    output = "exec"
+    if type.startswith("out$"):
+        output = "return"
+        type = type[4:]
+    if type == "file":
+        pyFile = open(input)
+        pyData = pyFile.read()
+        pyFile.close()
+    elif type in ["string", "str"]:
+        pyData = input
+    else:
+        printErr("type is invalid")
+        return
+    pyLines = pyData.splitlines()
+    encCode = pyLines[0]
+    encData = pyLines[-1]
+    encFunc = None
+    for t in __spec__.data.codeType:
+        for c in t["codes"]:
+            if c == encCode:
+                encFunc = t["decoder"]
+    decData = list2str(str(encFunc(bytes(encData, "utf-8")))[2:-1].splitlines(), "\n")
+    if output == "exec":
+        decFile = open("decodedfile.py", "w")
+        decFile.write(decData)
+        decFile.flush()
+        decFile.close()
+        decMod = __import__("decodedfile")
+        del decMod
+        del sys.modules["decodedfile"]
+        os.remove("decodedfile")
+    else:
+        return decData
```

### Comparing `prot-3.9.1/src/prot/pip/__init__.py` & `prot-3.9.2/src/prot/pip/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,367 +1,367 @@
-import sys
-
-try:
-    from .packagesList import packagesList as _p
-except:
-    _p = []
-import os
-import runpy as _r
-
-from .. import *
-
-try:
-    import xmlrpc.client as xmlrpclib
-except:
-    xmlrpclib = None
-
-__version__ = str(len(_p))
-DEFAULT_REPOSITORY = "Pypi"
-
-
-def decode(file, type="txt"):
-    if type == "txt":
-        return open(file).read().splitlines()
-    else:
-        return getVarFromFile(file, "packagesList")
-
-
-def encode(data, type="txt"):
-    if type == "txt":
-        string = ""
-        for d in data:
-            string += d + "\n"
-        return string
-    else:
-        return "packagesList = " + str(data)
-
-
-def convertUpdatePackage(iFile=None, oFile=None, ofFile="txt"):
-    printMsg("converting file to " + ofFile + " format...")
-    ifFile = "txt" if not ofFile == "txt" else "py"
-    if type(iFile) == bool:
-        iFile = "PackagesList." + ifFile
-    if type(oFile) == bool:
-        oFile = "PackagesList." + ofFile
-    if not os.path.exists(iFile):
-        printErr("import argument not entered.")
-        return
-    data = decode(iFile, ifFile)
-    try:
-        open(oFile, "w").write(encode(data, ofFile))
-    except PermissionError:
-        printErr("permission denied.")
-        return
-    printMsg("converted " + iFile + " to " + oFile + ".")
-
-
-def updateBuiltinList(export=False, pList=False, fList="txt"):
-    if export and pList:
-        convertUpdatePackage(pList, export, fList)
-        return
-    if xmlrpclib is None and not pList:
-        printErr("xmlrpc is required.")
-        return
-    global _p
-    if not export:
-        printMsg("current version is " + str(len(_p)))
-    printMsg("checking for updates..." if not export else "getting list...")
-    try:
-        if pList:
-            if type(pList) == bool:
-                pList = "PackagesList.txt" if fList == "txt" else "packagesList.py"
-            if fList == "txt":
-                pl = open(pList).read().splitlines()
-            else:
-                pl = getVarFromFile(pList, "packagesList")
-        else:
-            client = xmlrpclib.ServerProxy("https://pypi.python.org/pypi")
-            pl = client.list_packages()
-    except:
-        printErr(
-            "update failed." if not export else "error occured while getting list."
-        )
-        return
-    if len(pl) <= len(_p) and not export:
-        printMsg("built in list already updated.")
-        return
-    if settings.orderedBuiltinList == "on":
-        pl.sort()
-    try:
-        if export:
-            if type(export) == bool:
-                export = "PackagesList.txt" if fList == "txt" else "packagesList.py"
-            f = open(export, "w")
-            f.write(encode(pl, fList))
-            f.flush()
-            f.close()
-        else:
-            _p = pl
-            f = open(os.path.join(os.path.split(__file__)[0], "packagesList.py"), "w")
-            f.write("packagesList = " + str(_p))
-            f.flush()
-            f.close()
-    except PermissionError:
-        printErr("permission denied.")
-        return
-    printMsg(
-        "built in list updated to version " + str(len(_p)) + "."
-        if not export
-        else "list exported to " + export + "."
-        if fList == "txt"
-        else "list exported to " + export + " with python format."
-    )
-
-
-def getLocalRepo():
-    if settings.repo == "default":
-        return DEFAULT_REPOSITORY
-    else:
-        return settings.repo
-
-
-def pip(args=None):
-    if type(args) == list:
-        args = ["prot.pip"] + args
-    elif type(args) == str:
-        args = ["prot.pip"] + args.split(" ")
-    else:
-        args = sys.argv
-    if not args[0] == "prot.pip":
-        args[0] = "prot.pip"
-    sys.argv = args
-    _r._run_module_as_main(sys.argv[0])
-
-
-def parseValue(value):
-    args = []
-    vals = []
-    for v in value:
-        if v.startswith("-"):
-            args.append(v)
-        elif v.startswith("+"):
-            args[len(args) - 1] += " " + v.replace("+", "")
-        else:
-            vals.append(v)
-    return vals, args
-
-
-def main(action, **values):
-    rules = [
-        {"key": "local", "default": False},
-        {"key": "smart", "default": False},
-        {"key": "value", "default": None},
-        {"key": "export", "default": None},
-        {"key": "list", "default": False},
-        {"key": "listContents", "default": []},
-        {"key": "builtinList", "default": False},
-        {"key": "searchList", "default": False},
-        {"key": "searchKey", "default": None},
-        {"key": "cfgFile", "default": None},
-        {"key": "cfgStr", "default": ""},
-        {"key": "cfgList", "default": []},
-    ]
-    options = OptionsDatabase(values, rules)
-    if not options.value:
-        options.value = ""
-    options.value, options.extraArgs = parseValue(options.value.split(" "))
-    options.value, options.extraArgs = list2str(options.value, " "), list2str(
-        options.extraArgs, " "
-    )
-    if options.local and type(options.local) == bool:
-        options.local = getLocalRepo()
-    if options.list and (
-        (type(options.list) == bool)
-        or ("search-" in options.list or "s-" in options.list)
-    ):
-        options.list = "bltin" if (type(options.list) == bool) else options.list
-        options.builtinList = True
-        options.searchList = (
-            True if ("search-" in options.list or "s-" in options.list) else False
-        )
-        if options.searchList:
-            options.searchKey = options.list.split("-")[1]
-    if options.smart and type(options.smart) == bool:
-        options.smart = "PackagesList.txt"
-    if options.export and type(options.export) == bool:
-        options.export = "PackagesList.txt"
-    if options.list and type(options.list) == str:
-        options.list = options.list.replace(
-            "local.", options.local + "/" if options.local else ""
-        )
-    if options.smart and type(options.smart) == str:
-        options.smart = options.smart.replace(
-            "local.", options.local + "/" if options.local else ""
-        )
-    if options.export and type(options.export) == str:
-        options.export = options.export.replace(
-            "local.", options.local + "/" if options.local else ""
-        )
-
-    if options.smart:
-        if os.path.exists(options.smart):
-            f = open(options.smart)
-            options.cfgList = f.read().splitlines()
-            f.close()
-        else:
-            options.cfgFile = open(options.smart, "w")
-        if options.cfgFile is None:
-            options.cfgFile = open(options.smart, "w")
-        options.cfgStr = ""
-        for package in options.cfgList:
-            options.cfgStr += package + "\n"
-        if options.cfgStr.splitlines():
-            options.cfgFile.write(options.cfgStr)
-            options.cfgFile.flush()
-
-    if options.list:
-        if options.builtinList:
-            options.listContents += _p
-        if options.searchList:
-            newListContents = []
-            for c in options.listContents:
-                if options.searchKey in c:
-                    newListContents.append(c)
-            options.listContents = newListContents
-        if not options.builtinList:
-            if os.path.exists(options.list):
-                options.listContents += open(options.list).read().splitlines()
-            else:
-                options.listContents.append(options.value)
-    else:
-        options.listContents.append(options.value)
-
-    if not action:
-        printErr("argument is invalid.")
-        return
-    if action in ["install", "download", "wheel"]:
-        VAL1 = ValueWidget(0)
-        VAL2 = ValueWidget(0)
-        form = (
-            "$1 ignored, $2 $MSG $BAR"
-            if settings.ui in ["small", "verysmall"]
-            else "$TIME ($VAL/$MAX) $1 ignored, $2 $MSG $BAR $PERC% completed"
-        )
-        progress = Progress(
-            maxVal=len(options.listContents),
-            msg=action + "ed",
-            msgForm=form,
-            replaces=[
-                ["$TIME", TimeWidget(hour=False)],
-                [
-                    "$BAR",
-                    BarWidget(fillPerPercent=10 if settings.ui == "verysmall" else 5),
-                ],
-                ["$1", VAL1],
-                ["$2", VAL2],
-            ],
-            inline=True,
-        )
-        for c in range(len(options.listContents)):
-            value = options.listContents[c]
-            if value is None:
-                progress.newline()
-                printErr("name not entered.")
-                VAL1.value += 1
-                progress.update(c + 1)
-                continue
-            if (
-                options.value
-                and not " " in options.value
-                and not options.value.startswith("-")
-            ):
-                if not options.value in value:
-                    VAL1.value += 1
-                    progress.update(c + 1)
-                    continue
-            elif options.value and " " in options.value:
-                for v in options.value.split(" "):
-                    if not v.startswith("-"):
-                        if not options.value in value:
-                            VAL1.value += 1
-                            progress.update(c + 1)
-                            continue
-            if options.smart:
-                if value in options.cfgList:
-                    VAL1.value += 1
-                    progress.update(c + 1)
-                    continue
-            progress.newline()
-            try:
-                if options.local:
-                    runAsMain(
-                        str(
-                            "pip "
-                            + action
-                            + "$VAL"
-                            + "$EX"
-                            + " --no-index -f "
-                            + options.local
-                        )
-                        .replace("$VAL", (" " + value if value else ""))
-                        .replace(
-                            "$EX",
-                            (" " + options.extraArgs) if options.extraArgs else "",
-                        )
-                    )
-                else:
-                    runAsMain(
-                        str("pip " + action + "$VAL" + "$EX")
-                        .replace("$VAL", (" " + value if value else ""))
-                        .replace(
-                            "$EX",
-                            (" " + options.extraArgs) if options.extraArgs else "",
-                        )
-                    )
-            except:
-                pass
-            if options.smart:
-                options.cfgList.append(value)
-                options.cfgFile.write(value + "\n")
-                options.cfgFile.flush()
-            VAL2.value += 1
-            progress.update(c + 1)
-        progress.newline()
-        if options.smart:
-            options.cfgFile.close()
-
-    elif action == "search":
-        searchResult = []
-        if options.value in options.listContents:
-            options.listContents.remove(options.value)
-        if options.listContents:
-            for p in options.listContents:
-                if options.value:
-                    if options.value in p:
-                        searchResult.append(p)
-                else:
-                    searchResult.append(p)
-        elif options.local:
-            for f in os.listdir(options.local):
-                if f.endswith(".tar.gz") or f.endswith(".whl") or f.endswith(".zip"):
-                    if options.value:
-                        if options.value in f:
-                            searchResult.append(f)
-                    else:
-                        searchResult.append(f)
-        else:
-            try:
-                runAsMain("pip " + action + " " + options.value)
-            except:
-                pass
-        if options.export:
-            f = open(options.export, "w")
-            ss = ""
-            for p in searchResult:
-                ss += p + "\n"
-            f.write(ss)
-            f.flush()
-            f.close()
-            printMsg("search result exported to " + options.export)
-        else:
-            for p in searchResult:
-                printMsg(p, colorize=False)
-    elif action == "version":
-        printMsg(len(_p))
-    else:
-        printErr("argument is invalid.")
-        return
+import sys
+
+try:
+    from .packagesList import packagesList as _p
+except:
+    _p = []
+import os
+import runpy as _r
+
+from .. import *
+
+try:
+    import xmlrpc.client as xmlrpclib
+except:
+    xmlrpclib = None
+
+__version__ = str(len(_p))
+DEFAULT_REPOSITORY = "Pypi"
+
+
+def decode(file, type="txt"):
+    if type == "txt":
+        return open(file).read().splitlines()
+    else:
+        return getVarFromFile(file, "packagesList")
+
+
+def encode(data, type="txt"):
+    if type == "txt":
+        string = ""
+        for d in data:
+            string += d + "\n"
+        return string
+    else:
+        return "packagesList = " + str(data)
+
+
+def convertUpdatePackage(iFile=None, oFile=None, ofFile="txt"):
+    printMsg("converting file to " + ofFile + " format...")
+    ifFile = "txt" if not ofFile == "txt" else "py"
+    if type(iFile) == bool:
+        iFile = "PackagesList." + ifFile
+    if type(oFile) == bool:
+        oFile = "PackagesList." + ofFile
+    if not os.path.exists(iFile):
+        printErr("import argument not entered.")
+        return
+    data = decode(iFile, ifFile)
+    try:
+        open(oFile, "w").write(encode(data, ofFile))
+    except PermissionError:
+        printErr("permission denied.")
+        return
+    printMsg("converted " + iFile + " to " + oFile + ".")
+
+
+def updateBuiltinList(export=False, pList=False, fList="txt"):
+    if export and pList:
+        convertUpdatePackage(pList, export, fList)
+        return
+    if xmlrpclib is None and not pList:
+        printErr("xmlrpc is required.")
+        return
+    global _p
+    if not export:
+        printMsg("current version is " + str(len(_p)))
+    printMsg("checking for updates..." if not export else "getting list...")
+    try:
+        if pList:
+            if type(pList) == bool:
+                pList = "PackagesList.txt" if fList == "txt" else "packagesList.py"
+            if fList == "txt":
+                pl = open(pList).read().splitlines()
+            else:
+                pl = getVarFromFile(pList, "packagesList")
+        else:
+            client = xmlrpclib.ServerProxy("https://pypi.python.org/pypi")
+            pl = client.list_packages()
+    except:
+        printErr(
+            "update failed." if not export else "error occured while getting list."
+        )
+        return
+    if len(pl) <= len(_p) and not export:
+        printMsg("built in list already updated.")
+        return
+    if settings.orderedBuiltinList == "on":
+        pl.sort()
+    try:
+        if export:
+            if type(export) == bool:
+                export = "PackagesList.txt" if fList == "txt" else "packagesList.py"
+            f = open(export, "w")
+            f.write(encode(pl, fList))
+            f.flush()
+            f.close()
+        else:
+            _p = pl
+            f = open(os.path.join(os.path.split(__file__)[0], "packagesList.py"), "w")
+            f.write("packagesList = " + str(_p))
+            f.flush()
+            f.close()
+    except PermissionError:
+        printErr("permission denied.")
+        return
+    printMsg(
+        "built in list updated to version " + str(len(_p)) + "."
+        if not export
+        else "list exported to " + export + "."
+        if fList == "txt"
+        else "list exported to " + export + " with python format."
+    )
+
+
+def getLocalRepo():
+    if settings.repo == "default":
+        return DEFAULT_REPOSITORY
+    else:
+        return settings.repo
+
+
+def pip(args=None):
+    if type(args) == list:
+        args = ["prot.pip"] + args
+    elif type(args) == str:
+        args = ["prot.pip"] + args.split(" ")
+    else:
+        args = sys.argv
+    if not args[0] == "prot.pip":
+        args[0] = "prot.pip"
+    sys.argv = args
+    _r._run_module_as_main(sys.argv[0])
+
+
+def parseValue(value):
+    args = []
+    vals = []
+    for v in value:
+        if v.startswith("-"):
+            args.append(v)
+        elif v.startswith("+"):
+            args[len(args) - 1] += " " + v.replace("+", "")
+        else:
+            vals.append(v)
+    return vals, args
+
+
+def main(action, **values):
+    rules = [
+        {"key": "local", "default": False},
+        {"key": "smart", "default": False},
+        {"key": "value", "default": None},
+        {"key": "export", "default": None},
+        {"key": "list", "default": False},
+        {"key": "listContents", "default": []},
+        {"key": "builtinList", "default": False},
+        {"key": "searchList", "default": False},
+        {"key": "searchKey", "default": None},
+        {"key": "cfgFile", "default": None},
+        {"key": "cfgStr", "default": ""},
+        {"key": "cfgList", "default": []},
+    ]
+    options = OptionsDatabase(values, rules)
+    if not options.value:
+        options.value = ""
+    options.value, options.extraArgs = parseValue(options.value.split(" "))
+    options.value, options.extraArgs = list2str(options.value, " "), list2str(
+        options.extraArgs, " "
+    )
+    if options.local and type(options.local) == bool:
+        options.local = getLocalRepo()
+    if options.list and (
+        (type(options.list) == bool)
+        or ("search-" in options.list or "s-" in options.list)
+    ):
+        options.list = "bltin" if (type(options.list) == bool) else options.list
+        options.builtinList = True
+        options.searchList = (
+            True if ("search-" in options.list or "s-" in options.list) else False
+        )
+        if options.searchList:
+            options.searchKey = options.list.split("-")[1]
+    if options.smart and type(options.smart) == bool:
+        options.smart = "PackagesList.txt"
+    if options.export and type(options.export) == bool:
+        options.export = "PackagesList.txt"
+    if options.list and type(options.list) == str:
+        options.list = options.list.replace(
+            "local.", options.local + "/" if options.local else ""
+        )
+    if options.smart and type(options.smart) == str:
+        options.smart = options.smart.replace(
+            "local.", options.local + "/" if options.local else ""
+        )
+    if options.export and type(options.export) == str:
+        options.export = options.export.replace(
+            "local.", options.local + "/" if options.local else ""
+        )
+
+    if options.smart:
+        if os.path.exists(options.smart):
+            f = open(options.smart)
+            options.cfgList = f.read().splitlines()
+            f.close()
+        else:
+            options.cfgFile = open(options.smart, "w")
+        if options.cfgFile is None:
+            options.cfgFile = open(options.smart, "w")
+        options.cfgStr = ""
+        for package in options.cfgList:
+            options.cfgStr += package + "\n"
+        if options.cfgStr.splitlines():
+            options.cfgFile.write(options.cfgStr)
+            options.cfgFile.flush()
+
+    if options.list:
+        if options.builtinList:
+            options.listContents += _p
+        if options.searchList:
+            newListContents = []
+            for c in options.listContents:
+                if options.searchKey in c:
+                    newListContents.append(c)
+            options.listContents = newListContents
+        if not options.builtinList:
+            if os.path.exists(options.list):
+                options.listContents += open(options.list).read().splitlines()
+            else:
+                options.listContents.append(options.value)
+    else:
+        options.listContents.append(options.value)
+
+    if not action:
+        printErr("argument is invalid.")
+        return
+    if action in ["install", "download", "wheel"]:
+        VAL1 = ValueWidget(0)
+        VAL2 = ValueWidget(0)
+        form = (
+            "$1 ignored, $2 $MSG $BAR"
+            if settings.ui in ["small", "verysmall"]
+            else "$TIME ($VAL/$MAX) $1 ignored, $2 $MSG $BAR $PERC% completed"
+        )
+        progress = Progress(
+            maxVal=len(options.listContents),
+            msg=action + "ed",
+            msgForm=form,
+            replaces=[
+                ["$TIME", TimeWidget(hour=False)],
+                [
+                    "$BAR",
+                    BarWidget(fillPerPercent=10 if settings.ui == "verysmall" else 5),
+                ],
+                ["$1", VAL1],
+                ["$2", VAL2],
+            ],
+            inline=True,
+        )
+        for c in range(len(options.listContents)):
+            value = options.listContents[c]
+            if value is None:
+                progress.newline()
+                printErr("name not entered.")
+                VAL1.value += 1
+                progress.update(c + 1)
+                continue
+            if (
+                options.value
+                and not " " in options.value
+                and not options.value.startswith("-")
+            ):
+                if not options.value in value:
+                    VAL1.value += 1
+                    progress.update(c + 1)
+                    continue
+            elif options.value and " " in options.value:
+                for v in options.value.split(" "):
+                    if not v.startswith("-"):
+                        if not options.value in value:
+                            VAL1.value += 1
+                            progress.update(c + 1)
+                            continue
+            if options.smart:
+                if value in options.cfgList:
+                    VAL1.value += 1
+                    progress.update(c + 1)
+                    continue
+            progress.newline()
+            try:
+                if options.local:
+                    runAsMain(
+                        str(
+                            "pip "
+                            + action
+                            + "$VAL"
+                            + "$EX"
+                            + " --no-index -f "
+                            + options.local
+                        )
+                        .replace("$VAL", (" " + value if value else ""))
+                        .replace(
+                            "$EX",
+                            (" " + options.extraArgs) if options.extraArgs else "",
+                        )
+                    )
+                else:
+                    runAsMain(
+                        str("pip " + action + "$VAL" + "$EX")
+                        .replace("$VAL", (" " + value if value else ""))
+                        .replace(
+                            "$EX",
+                            (" " + options.extraArgs) if options.extraArgs else "",
+                        )
+                    )
+            except:
+                pass
+            if options.smart:
+                options.cfgList.append(value)
+                options.cfgFile.write(value + "\n")
+                options.cfgFile.flush()
+            VAL2.value += 1
+            progress.update(c + 1)
+        progress.newline()
+        if options.smart:
+            options.cfgFile.close()
+
+    elif action == "search":
+        searchResult = []
+        if options.value in options.listContents:
+            options.listContents.remove(options.value)
+        if options.listContents:
+            for p in options.listContents:
+                if options.value:
+                    if options.value in p:
+                        searchResult.append(p)
+                else:
+                    searchResult.append(p)
+        elif options.local:
+            for f in os.listdir(options.local):
+                if f.endswith(".tar.gz") or f.endswith(".whl") or f.endswith(".zip"):
+                    if options.value:
+                        if options.value in f:
+                            searchResult.append(f)
+                    else:
+                        searchResult.append(f)
+        else:
+            try:
+                runAsMain("pip " + action + " " + options.value)
+            except:
+                pass
+        if options.export:
+            f = open(options.export, "w")
+            ss = ""
+            for p in searchResult:
+                ss += p + "\n"
+            f.write(ss)
+            f.flush()
+            f.close()
+            printMsg("search result exported to " + options.export)
+        else:
+            for p in searchResult:
+                printMsg(p, colorize=False)
+    elif action == "version":
+        printMsg(len(_p))
+    else:
+        printErr("argument is invalid.")
+        return
```

### Comparing `prot-3.9.1/src/prot/pip/__main__.py` & `prot-3.9.2/src/prot/pip/__main__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import sys
-
-from .. import *
-from . import *
-
-exit = False
-if "light" in status:
-    printErr("command line interface not available in light version")
-    exit = True
-
-if __name__ == "__main__" and not exit:
-    localRepo = False
-    action = None
-    value = None
-    pList = False
-    iList = False
-    eList = False
-    fList = "txt"
-    smart = False
-    export = False
-    for a in sys.argv[1:]:
-        if action == "update" and ("--export" in a or "-e" in a):
-            if ":" in a:
-                eList = a.split(":")[1]
-            else:
-                eList = True
-        elif action == "update" and ("--import" in a or "-i" in a):
-            if ":" in a:
-                iList = a.split(":")[1]
-            else:
-                iList = True
-        elif action == "update" and ("--format" in a or "-f" in a):
-            fList = "py"
-        elif "--list" in a and not pList:
-            if ":" in a:
-                pList = a.split(":")[1]
-            else:
-                pList = True
-        elif "--local" in a or "-l" in a and not localRepo:
-            if ":" in a:
-                localRepo = a.split(":")[1]
-            else:
-                localRepo = True
-        elif "--smart" in a or "-s" in a and not smart:
-            if ":" in a:
-                smart = a.split(":")[1]
-            else:
-                smart = True
-        elif "--export" in a or "-e" in a and not export:
-            if ":" in a:
-                export = a.split(":")[1]
-            else:
-                export = True
-        elif a in ["search", "s"] and not action:
-            action = "search"
-        elif a in ["install", "i"] and not action:
-            action = "install"
-        elif a in ["download", "d"] and not action:
-            action = "download"
-        elif a in ["wheel", "w"] and not action:
-            action = "wheel"
-        elif a in ["update", "u"] and not action:
-            action = "update"
-        elif a in ["version", "v"] and not action:
-            action = "version"
-        else:
-            if value is None:
-                value = ""
-            if value:
-                value += " "
-            value += a
-
-    if action == "update":
-        updateBuiltinList(eList, iList, fList)
-    else:
-        main(
-            action, value=value, local=localRepo, list=pList, smart=smart, export=export
-        )
+import sys
+
+from .. import *
+from . import *
+
+exit = False
+if "light" in status:
+    printErr("command line interface not available in light version")
+    exit = True
+
+if __name__ == "__main__" and not exit:
+    localRepo = False
+    action = None
+    value = None
+    pList = False
+    iList = False
+    eList = False
+    fList = "txt"
+    smart = False
+    export = False
+    for a in sys.argv[1:]:
+        if action == "update" and ("--export" in a or "-e" in a):
+            if ":" in a:
+                eList = a.split(":")[1]
+            else:
+                eList = True
+        elif action == "update" and ("--import" in a or "-i" in a):
+            if ":" in a:
+                iList = a.split(":")[1]
+            else:
+                iList = True
+        elif action == "update" and ("--format" in a or "-f" in a):
+            fList = "py"
+        elif "--list" in a and not pList:
+            if ":" in a:
+                pList = a.split(":")[1]
+            else:
+                pList = True
+        elif "--local" in a or "-l" in a and not localRepo:
+            if ":" in a:
+                localRepo = a.split(":")[1]
+            else:
+                localRepo = True
+        elif "--smart" in a or "-s" in a and not smart:
+            if ":" in a:
+                smart = a.split(":")[1]
+            else:
+                smart = True
+        elif "--export" in a or "-e" in a and not export:
+            if ":" in a:
+                export = a.split(":")[1]
+            else:
+                export = True
+        elif a in ["search", "s"] and not action:
+            action = "search"
+        elif a in ["install", "i"] and not action:
+            action = "install"
+        elif a in ["download", "d"] and not action:
+            action = "download"
+        elif a in ["wheel", "w"] and not action:
+            action = "wheel"
+        elif a in ["update", "u"] and not action:
+            action = "update"
+        elif a in ["version", "v"] and not action:
+            action = "version"
+        else:
+            if value is None:
+                value = ""
+            if value:
+                value += " "
+            value += a
+
+    if action == "update":
+        updateBuiltinList(eList, iList, fList)
+    else:
+        main(
+            action, value=value, local=localRepo, list=pList, smart=smart, export=export
+        )
```

### Comparing `prot-3.9.1/src/prot.egg-info/PKG-INFO` & `prot-3.9.2/src/prot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,104 @@
-Metadata-Version: 2.1
-Name: prot
-Version: 3.9.1
-Summary: A Simple Tool That Contains Advance Functions.
-Home-page: https://github.com/SAPTeamDEV/prot
-Author: Alireza Poodineh
-Author-email: itsaeliux@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Prot - Pro Tools for Python 3
-
-[![Downloads](https://static.pepy.tech/badge/prot)](https://pepy.tech/project/prot)
-
-Modules
--------
-
- * **classes**
- * **functions**
- * **converters**
- * **settings**
-
-classes Module
---------------
-
- * **Database**
- * **OptionsDatabase**
- * **Progress**
- * **ProgressBar** (from **Progress** and **BarWidget**)
- * **LockedDict**
- * **Str**
- * **TextListFile**
- * **Widget**
-
- >* **TimeWidget**
- >* **BarWidget**
- >* **TaskWidget**
- >* **CallWidget**
- >* **ValueWidget**
- >* **LoadingWidget**
-
-functions Module
-----------------
-
- * **verifyColor**
- * **insertColor**
- * **getRandomPassword**
- * **testSpeed**
- * **getVarFromFile**
- * **checkMethods**
- * **callMethods**
- * **callMethodsWithArg**
- * **checkFileSame**
- * **splitStr**
- * **runAsMain**
- * **printMsg**
- * **printErr**
- * **printWarn**
-
-converters Module
------------------
-
- * **rst2html**
- * **dict2matrix**
- * **str2list**
- * **list2str**
- * **matrix2str**
-
-Packages
---------
-
- * **color**
- * **pip**
- * **progress**
- * **prompt**
- * **wcwidth**
-
-pip Package
------------
-
- >this is a Advanced pip Tool, this Package has a List of all pip Packages that you can Search, Download and Install them and you can Update this List anytime you want
-
- **Features**
-
- >* it has built in Packages List
- >* you can do an Offline Search
- >* can Create Offline Repositiry
- >* can do Batch Install or Download with built in List or use Custom List
- >* and more...
+Metadata-Version: 2.1
+Name: prot
+Version: 3.9.2
+Summary: A Simple Tool That Contains Advance Functions.
+Home-page: https://github.com/SAPTeamDEV/prot
+Author: Alireza Poodineh
+Author-email: itsaeliux@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Prot - Pro Tools for Python 3
+
+[![Downloads](https://static.pepy.tech/badge/prot)](https://pepy.tech/project/prot)
+
+> Note: this readme is not updated and does not reflect the latest applied patches. A huge update is under the way!
+
+Modules
+-------
+
+ * **classes**
+ * **functions**
+ * **converters**
+ * **settings**
+
+classes Module
+--------------
+
+ * **Database**
+ * **OptionsDatabase**
+ * **Progress**
+ * **ProgressBar** (from **Progress** and **BarWidget**)
+ * **LockedDict**
+ * **Str**
+ * **TextListFile**
+ * **Widget**
+
+ >* **TimeWidget**
+ >* **BarWidget**
+ >* **TaskWidget**
+ >* **CallWidget**
+ >* **ValueWidget**
+ >* **LoadingWidget**
+
+functions Module
+----------------
+
+ * **verifyColor**
+ * **insertColor**
+ * **getRandomPassword**
+ * **testSpeed**
+ * **getVarFromFile**
+ * **checkMethods**
+ * **callMethods**
+ * **callMethodsWithArg**
+ * **checkFileSame**
+ * **splitStr**
+ * **runAsMain**
+ * **printMsg**
+ * **printErr**
+ * **printWarn**
+
+converters Module
+-----------------
+
+ * **rst2html**
+ * **dict2matrix**
+ * **str2list**
+ * **list2str**
+ * **matrix2str**
+
+Packages
+--------
+
+ * **color**
+ * **pip**
+ * **progress**
+ * **prompt**
+ * **wcwidth**
+
+pip Package
+-----------
+
+ >this is a Advanced pip Tool, this Package has a List of all pip Packages that you can Search, Download and Install them and you can Update this List anytime you want
+
+ **Features**
+
+ >* it has built in Packages List
+ >* you can do an Offline Search
+ >* can Create Offline Repositiry
+ >* can do Batch Install or Download with built in List or use Custom List
+ >* and more...
```

