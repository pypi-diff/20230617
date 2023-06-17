# Comparing `tmp/deltachat-1.97.0.tar.gz` & `tmp/deltachat-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-1.97.0.tar", last modified: Sun Oct 16 14:31:02 2022, max compression
+gzip compressed data, was "deltachat-1.99.0.tar", last modified: Sun Nov  6 19:06:06 2022, max compression
```

## Comparing `deltachat-1.97.0.tar` & `deltachat-1.99.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.324892 deltachat-1.97.0/
--rw-r--r--   0 root         (0) root         (0)       52 2022-10-16 13:39:59.000000 deltachat-1.97.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2986 2022-10-16 13:39:59.000000 deltachat-1.97.0/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    16726 2022-10-16 13:39:59.000000 deltachat-1.97.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2022-10-16 13:39:59.000000 deltachat-1.97.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5191 2022-10-16 14:31:02.324892 deltachat-1.97.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4356 2022-10-16 13:39:59.000000 deltachat-1.97.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.312893 deltachat-1.97.0/doc/
--rw-r--r--   0 root         (0) root         (0)     6984 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.312893 deltachat-1.97.0/doc/_static/
--rw-r--r--   0 root         (0) root         (0)      225 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/_static/custom.css
--rwxr-xr-x   0 root         (0) root         (0)     7185 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/_static/delta-chat.svg
--rw-r--r--   0 root         (0) root         (0)    15086 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/_static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.312893 deltachat-1.97.0/doc/_templates/
--rw-r--r--   0 root         (0) root         (0)      552 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/_templates/globaltoc.html
--rw-r--r--   0 root         (0) root         (0)       31 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/_templates/sidebarintro.html
--rw-r--r--   0 root         (0) root         (0)      529 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/api.rst
--rw-r--r--   0 root         (0) root         (0)      121 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     8933 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1718 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/examples.rst
--rw-r--r--   0 root         (0) root         (0)      720 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)       28 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/install.rst
--rw-r--r--   0 root         (0) root         (0)      267 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/lapi.rst
--rw-r--r--   0 root         (0) root         (0)      348 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/links.rst
--rw-r--r--   0 root         (0) root         (0)     5094 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/make.bat
--rw-r--r--   0 root         (0) root         (0)      891 2022-10-16 13:39:59.000000 deltachat-1.97.0/doc/plugins.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.312893 deltachat-1.97.0/examples/
--rw-r--r--   0 root         (0) root         (0)      967 2022-10-16 13:39:59.000000 deltachat-1.97.0/examples/echo_and_quit.py
--rw-r--r--   0 root         (0) root         (0)     1793 2022-10-16 13:39:59.000000 deltachat-1.97.0/examples/group_tracking.py
--rw-r--r--   0 root         (0) root         (0)     2557 2022-10-16 13:39:59.000000 deltachat-1.97.0/examples/test_examples.py
--rwxr-xr-x   0 root         (0) root         (0)      972 2022-10-16 13:39:59.000000 deltachat-1.97.0/install_python_bindings.py
--rw-r--r--   0 root         (0) root         (0)      395 2022-10-16 13:39:59.000000 deltachat-1.97.0/mypy.ini
--rw-r--r--   0 root         (0) root         (0)     1373 2022-10-16 13:39:59.000000 deltachat-1.97.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-16 14:31:02.324892 deltachat-1.97.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      120 2022-10-16 13:39:59.000000 deltachat-1.97.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.304892 deltachat-1.97.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.316892 deltachat-1.97.0/src/deltachat/
--rw-r--r--   0 root         (0) root         (0)     1798 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6775 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/_build.py
--rw-r--r--   0 root         (0) root         (0)    30265 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/account.py
--rw-r--r--   0 root         (0) root         (0)    22522 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/chat.py
--rw-r--r--   0 root         (0) root         (0)      282 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/const.py
--rw-r--r--   0 root         (0) root         (0)     3599 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/contact.py
--rw-r--r--   0 root         (0) root         (0)     1539 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/cutil.py
--rw-r--r--   0 root         (0) root         (0)     7851 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/direct_imap.py
--rw-r--r--   0 root         (0) root         (0)    11303 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/events.py
--rw-r--r--   0 root         (0) root         (0)     3772 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/hookspec.py
--rw-r--r--   0 root         (0) root         (0)    18408 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/message.py
--rw-r--r--   0 root         (0) root         (0)      806 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/props.py
--rw-r--r--   0 root         (0) root         (0)     1469 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/provider.py
--rw-r--r--   0 root         (0) root         (0)    25416 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/testplugin.py
--rw-r--r--   0 root         (0) root         (0)     3395 2022-10-16 13:39:59.000000 deltachat-1.97.0/src/deltachat/tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.320892 deltachat-1.97.0/src/deltachat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5191 2022-10-16 14:31:02.000000 deltachat-1.97.0/src/deltachat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1707 2022-10-16 14:31:02.000000 deltachat-1.97.0/src/deltachat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-16 14:31:02.000000 deltachat-1.97.0/src/deltachat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2022-10-16 14:31:02.000000 deltachat-1.97.0/src/deltachat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-10-16 14:31:02.000000 deltachat-1.97.0/src/deltachat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-10-16 14:31:02.000000 deltachat-1.97.0/src/deltachat.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.320892 deltachat-1.97.0/tests/
--rw-r--r--   0 root         (0) root         (0)      501 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/auditwheels.py
--rw-r--r--   0 root         (0) root         (0)      414 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/bench_test_setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.320892 deltachat-1.97.0/tests/data/
--rw-r--r--   0 root         (0) root         (0)     2776 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/d.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-16 14:31:02.324892 deltachat-1.97.0/tests/data/key/
--rw-r--r--   0 root         (0) root         (0)      632 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/alice-public.asc
--rw-r--r--   0 root         (0) root         (0)      731 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/alice-secret.asc
--rw-r--r--   0 root         (0) root         (0)     1717 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/bob-public.asc
--rw-r--r--   0 root         (0) root         (0)     3482 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/bob-secret.asc
--rw-r--r--   0 root         (0) root         (0)     1721 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/charlie-public.asc
--rw-r--r--   0 root         (0) root         (0)     3486 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/charlie-secret.asc
--rw-r--r--   0 root         (0) root         (0)     1717 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/dom-public.asc
--rw-r--r--   0 root         (0) root         (0)     3482 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/dom-secret.asc
--rw-r--r--   0 root         (0) root         (0)     1721 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/elena-public.asc
--rw-r--r--   0 root         (0) root         (0)     3486 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/elena-secret.asc
--rw-r--r--   0 root         (0) root         (0)     1721 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/fiona-public.asc
--rw-r--r--   0 root         (0) root         (0)     3482 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/key/fiona-secret.asc
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/data/r.txt
--rw-r--r--   0 root         (0) root         (0)     4465 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/stress_test_db.py
--rw-r--r--   0 root         (0) root         (0)    19864 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/test_0_complex_or_slow.py
--rw-r--r--   0 root         (0) root         (0)    76491 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/test_1_online.py
--rw-r--r--   0 root         (0) root         (0)     4367 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/test_2_increation.py
--rw-r--r--   0 root         (0) root         (0)    30306 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/test_3_offline.py
--rw-r--r--   0 root         (0) root         (0)     7590 2022-10-16 13:39:59.000000 deltachat-1.97.0/tests/test_4_lowlevel.py
--rw-r--r--   0 root         (0) root         (0)     1834 2022-10-16 13:39:59.000000 deltachat-1.97.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.405572 deltachat-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)       52 2022-11-06 18:13:17.000000 deltachat-1.99.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2986 2022-11-06 18:13:17.000000 deltachat-1.99.0/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    16726 2022-11-06 18:13:17.000000 deltachat-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2022-11-06 18:13:17.000000 deltachat-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5191 2022-11-06 19:06:06.405572 deltachat-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4356 2022-11-06 18:13:17.000000 deltachat-1.99.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.385571 deltachat-1.99.0/doc/
+-rw-r--r--   0 root         (0) root         (0)     6984 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.385571 deltachat-1.99.0/doc/_static/
+-rw-r--r--   0 root         (0) root         (0)      225 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/_static/custom.css
+-rwxr-xr-x   0 root         (0) root         (0)     7185 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/_static/delta-chat.svg
+-rw-r--r--   0 root         (0) root         (0)    15086 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/_static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.385571 deltachat-1.99.0/doc/_templates/
+-rw-r--r--   0 root         (0) root         (0)      552 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/_templates/globaltoc.html
+-rw-r--r--   0 root         (0) root         (0)       31 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/_templates/sidebarintro.html
+-rw-r--r--   0 root         (0) root         (0)      529 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/api.rst
+-rw-r--r--   0 root         (0) root         (0)      121 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     8933 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/examples.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/install.rst
+-rw-r--r--   0 root         (0) root         (0)      267 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/lapi.rst
+-rw-r--r--   0 root         (0) root         (0)      348 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/links.rst
+-rw-r--r--   0 root         (0) root         (0)     5094 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/make.bat
+-rw-r--r--   0 root         (0) root         (0)      891 2022-11-06 18:13:17.000000 deltachat-1.99.0/doc/plugins.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.389572 deltachat-1.99.0/examples/
+-rw-r--r--   0 root         (0) root         (0)      967 2022-11-06 18:13:17.000000 deltachat-1.99.0/examples/echo_and_quit.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2022-11-06 18:13:17.000000 deltachat-1.99.0/examples/group_tracking.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2022-11-06 18:13:17.000000 deltachat-1.99.0/examples/test_examples.py
+-rwxr-xr-x   0 root         (0) root         (0)      972 2022-11-06 18:13:17.000000 deltachat-1.99.0/install_python_bindings.py
+-rw-r--r--   0 root         (0) root         (0)      395 2022-11-06 18:13:17.000000 deltachat-1.99.0/mypy.ini
+-rw-r--r--   0 root         (0) root         (0)     1373 2022-11-06 18:13:17.000000 deltachat-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-06 19:06:06.405572 deltachat-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      120 2022-11-06 18:13:17.000000 deltachat-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.381571 deltachat-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.393571 deltachat-1.99.0/src/deltachat/
+-rw-r--r--   0 root         (0) root         (0)     1798 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6775 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/_build.py
+-rw-r--r--   0 root         (0) root         (0)    30265 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/account.py
+-rw-r--r--   0 root         (0) root         (0)    22522 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/chat.py
+-rw-r--r--   0 root         (0) root         (0)      282 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/const.py
+-rw-r--r--   0 root         (0) root         (0)     3599 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/cutil.py
+-rw-r--r--   0 root         (0) root         (0)     7851 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/direct_imap.py
+-rw-r--r--   0 root         (0) root         (0)    11303 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/events.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/hookspec.py
+-rw-r--r--   0 root         (0) root         (0)    18408 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/message.py
+-rw-r--r--   0 root         (0) root         (0)      806 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/props.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25416 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/testplugin.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2022-11-06 18:13:17.000000 deltachat-1.99.0/src/deltachat/tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.393571 deltachat-1.99.0/src/deltachat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5191 2022-11-06 19:06:06.000000 deltachat-1.99.0/src/deltachat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1707 2022-11-06 19:06:06.000000 deltachat-1.99.0/src/deltachat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-06 19:06:06.000000 deltachat-1.99.0/src/deltachat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2022-11-06 19:06:06.000000 deltachat-1.99.0/src/deltachat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2022-11-06 19:06:06.000000 deltachat-1.99.0/src/deltachat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-11-06 19:06:06.000000 deltachat-1.99.0/src/deltachat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.401572 deltachat-1.99.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      501 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/auditwheels.py
+-rw-r--r--   0 root         (0) root         (0)      414 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/bench_test_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.401572 deltachat-1.99.0/tests/data/
+-rw-r--r--   0 root         (0) root         (0)     2776 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/d.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 19:06:06.405572 deltachat-1.99.0/tests/data/key/
+-rw-r--r--   0 root         (0) root         (0)      632 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/alice-public.asc
+-rw-r--r--   0 root         (0) root         (0)      731 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/alice-secret.asc
+-rw-r--r--   0 root         (0) root         (0)     1717 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/bob-public.asc
+-rw-r--r--   0 root         (0) root         (0)     3482 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/bob-secret.asc
+-rw-r--r--   0 root         (0) root         (0)     1721 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/charlie-public.asc
+-rw-r--r--   0 root         (0) root         (0)     3486 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/charlie-secret.asc
+-rw-r--r--   0 root         (0) root         (0)     1717 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/dom-public.asc
+-rw-r--r--   0 root         (0) root         (0)     3482 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/dom-secret.asc
+-rw-r--r--   0 root         (0) root         (0)     1721 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/elena-public.asc
+-rw-r--r--   0 root         (0) root         (0)     3486 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/elena-secret.asc
+-rw-r--r--   0 root         (0) root         (0)     1721 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/fiona-public.asc
+-rw-r--r--   0 root         (0) root         (0)     3482 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/key/fiona-secret.asc
+-rw-r--r--   0 root         (0) root         (0)        7 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/data/r.txt
+-rw-r--r--   0 root         (0) root         (0)     4465 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/stress_test_db.py
+-rw-r--r--   0 root         (0) root         (0)    19864 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/test_0_complex_or_slow.py
+-rw-r--r--   0 root         (0) root         (0)    76491 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/test_1_online.py
+-rw-r--r--   0 root         (0) root         (0)     4367 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/test_2_increation.py
+-rw-r--r--   0 root         (0) root         (0)    30306 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/test_3_offline.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2022-11-06 18:13:17.000000 deltachat-1.99.0/tests/test_4_lowlevel.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2022-11-06 18:13:17.000000 deltachat-1.99.0/tox.ini
```

### Comparing `deltachat-1.97.0/CHANGELOG` & `deltachat-1.99.0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/LICENSE` & `deltachat-1.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/PKG-INFO` & `deltachat-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat
-Version: 1.97.0
+Version: 1.99.0
 Summary: Python bindings for the Delta Chat Core library using CFFI against the Rust-implemented libdeltachat
 Author: holger krekel, Floris Bruynooghe, Bjoern Petersen and contributors
 Project-URL: Home, https://github.com/deltachat/deltachat-core-rust/
 Project-URL: Bug Tracker, https://github.com/deltachat/deltachat-core-rust/issues
 Project-URL: Documentation, https://py.delta.chat/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `deltachat-1.97.0/README.rst` & `deltachat-1.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/Makefile` & `deltachat-1.99.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/_static/delta-chat.svg` & `deltachat-1.99.0/doc/_static/delta-chat.svg`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/_static/favicon.ico` & `deltachat-1.99.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/_templates/globaltoc.html` & `deltachat-1.99.0/doc/_templates/globaltoc.html`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/api.rst` & `deltachat-1.99.0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/conf.py` & `deltachat-1.99.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/examples.rst` & `deltachat-1.99.0/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/index.rst` & `deltachat-1.99.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/make.bat` & `deltachat-1.99.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/doc/plugins.rst` & `deltachat-1.99.0/doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/examples/echo_and_quit.py` & `deltachat-1.99.0/examples/echo_and_quit.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/examples/group_tracking.py` & `deltachat-1.99.0/examples/group_tracking.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/examples/test_examples.py` & `deltachat-1.99.0/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/install_python_bindings.py` & `deltachat-1.99.0/install_python_bindings.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/pyproject.toml` & `deltachat-1.99.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/__init__.py` & `deltachat-1.99.0/src/deltachat/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/_build.py` & `deltachat-1.99.0/src/deltachat/_build.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/account.py` & `deltachat-1.99.0/src/deltachat/account.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/chat.py` & `deltachat-1.99.0/src/deltachat/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/contact.py` & `deltachat-1.99.0/src/deltachat/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/cutil.py` & `deltachat-1.99.0/src/deltachat/cutil.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/direct_imap.py` & `deltachat-1.99.0/src/deltachat/direct_imap.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/events.py` & `deltachat-1.99.0/src/deltachat/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         return ev
 
     def iter_events(self, timeout=None, check_error=True):
         while 1:
             yield self.get(timeout=timeout, check_error=check_error)
 
     def get_matching(self, event_name_regex, check_error=True, timeout=None):
-        rex = re.compile("(?:{}).*".format(event_name_regex))
+        rex = re.compile("^(?:{})$".format(event_name_regex))
         for ev in self.iter_events(timeout=timeout, check_error=check_error):
             if rex.match(ev.name):
                 return ev
 
     def get_info_contains(self, regex: str) -> FFIEvent:
         rex = re.compile(regex)
         while 1:
```

### Comparing `deltachat-1.97.0/src/deltachat/hookspec.py` & `deltachat-1.99.0/src/deltachat/hookspec.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/message.py` & `deltachat-1.99.0/src/deltachat/message.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/props.py` & `deltachat-1.99.0/src/deltachat/props.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/provider.py` & `deltachat-1.99.0/src/deltachat/provider.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/testplugin.py` & `deltachat-1.99.0/src/deltachat/testplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat/tracker.py` & `deltachat-1.99.0/src/deltachat/tracker.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/src/deltachat.egg-info/PKG-INFO` & `deltachat-1.99.0/src/deltachat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat
-Version: 1.97.0
+Version: 1.99.0
 Summary: Python bindings for the Delta Chat Core library using CFFI against the Rust-implemented libdeltachat
 Author: holger krekel, Floris Bruynooghe, Bjoern Petersen and contributors
 Project-URL: Home, https://github.com/deltachat/deltachat-core-rust/
 Project-URL: Bug Tracker, https://github.com/deltachat/deltachat-core-rust/issues
 Project-URL: Documentation, https://py.delta.chat/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `deltachat-1.97.0/src/deltachat.egg-info/SOURCES.txt` & `deltachat-1.99.0/src/deltachat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/d.png` & `deltachat-1.99.0/tests/data/d.png`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/alice-public.asc` & `deltachat-1.99.0/tests/data/key/alice-public.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/alice-secret.asc` & `deltachat-1.99.0/tests/data/key/alice-secret.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/bob-public.asc` & `deltachat-1.99.0/tests/data/key/bob-public.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/bob-secret.asc` & `deltachat-1.99.0/tests/data/key/bob-secret.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/charlie-public.asc` & `deltachat-1.99.0/tests/data/key/charlie-public.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/charlie-secret.asc` & `deltachat-1.99.0/tests/data/key/charlie-secret.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/dom-public.asc` & `deltachat-1.99.0/tests/data/key/dom-public.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/dom-secret.asc` & `deltachat-1.99.0/tests/data/key/dom-secret.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/elena-public.asc` & `deltachat-1.99.0/tests/data/key/elena-public.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/elena-secret.asc` & `deltachat-1.99.0/tests/data/key/elena-secret.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/fiona-public.asc` & `deltachat-1.99.0/tests/data/key/fiona-public.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/data/key/fiona-secret.asc` & `deltachat-1.99.0/tests/data/key/fiona-secret.asc`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/stress_test_db.py` & `deltachat-1.99.0/tests/stress_test_db.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/test_0_complex_or_slow.py` & `deltachat-1.99.0/tests/test_0_complex_or_slow.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/test_1_online.py` & `deltachat-1.99.0/tests/test_1_online.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/test_2_increation.py` & `deltachat-1.99.0/tests/test_2_increation.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/test_3_offline.py` & `deltachat-1.99.0/tests/test_3_offline.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tests/test_4_lowlevel.py` & `deltachat-1.99.0/tests/test_4_lowlevel.py`

 * *Files identical despite different names*

### Comparing `deltachat-1.97.0/tox.ini` & `deltachat-1.99.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     mypy
     auditwheels
 
 [testenv]
 commands = 
     pytest -n6 --extra-info --reruns 2 --reruns-delay 5 -v -rsXx --ignored --strict-tls {posargs: tests examples}
     pip wheel . -w {toxworkdir}/wheelhouse --no-deps
+setenv =
+# Avoid stack overflow when Rust core is built without optimizations.
+    RUST_MIN_STACK=8388608
 passenv = 
     DCC_RS_DEV
     DCC_RS_TARGET
     DCC_NEW_TMP_EMAIL 
     CARGO_TARGET_DIR
     RUSTC_WRAPPER
 deps =
```

