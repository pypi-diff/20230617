# Comparing `tmp/neon-utils-1.5.1a5.tar.gz` & `tmp/neon-utils-1.5.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-utils-1.5.1a5.tar", last modified: Thu Jun 15 19:40:35 2023, max compression
+gzip compressed data, was "neon-utils-1.5.1a6.tar", last modified: Sat Jun 17 01:00:00 2023, max compression
```

## Comparing `neon-utils-1.5.1a5.tar` & `neon-utils-1.5.1a6.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.889463 neon-utils-1.5.1a5/neon_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/authentication_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68315 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.889463 neon-utils-1.5.1a5/neon_utils/default_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/default_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/default_configurations/default_user_conf.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/location_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/messagebus_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/mq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/process_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.885463 neon-utils-1.5.1a5/neon_utils/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.889463 neon-utils-1.5.1a5/neon_utils/res/snd/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   428660 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/snd/loaded.wav
--rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/snd/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.885463 neon-utils-1.5.1a5/neon_utils/res/text/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.889463 neon-utils-1.5.1a5/neon_utils/res/text/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/text/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/text/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/text/en-us/stop.voc
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/text/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.889463 neon-utils-1.5.1a5/neon_utils/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/res/ui/neon_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/neon_utils/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/common_message_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/common_play_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/common_query_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/instructor_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/kiosk_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/mycroft_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/neon_fallback_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/neon_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/skills/skill_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/socket_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/validator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/neon_utils/web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.889463 neon-utils-1.5.1a5/neon_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-15 19:40:35.000000 neon-utils-1.5.1a5/neon_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-15 19:40:35.000000 neon-utils-1.5.1a5/neon_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:40:35.000000 neon-utils-1.5.1a5/neon_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 19:40:35.000000 neon-utils-1.5.1a5/neon_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-15 19:40:35.000000 neon-utils-1.5.1a5/neon_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 19:40:35.000000 neon-utils-1.5.1a5/neon_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/authentication_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/cache_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/configuration_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/file_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/language_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/location_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/log_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/message_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/messagebus_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/metric_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/mq_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    55268 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/neon_skill_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/net_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/packaging_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/parse_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/search_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/signal_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/tests/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/tests/skills/test_skill/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/skills/test_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/skills/test_skill/settingsmeta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/socket_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/user_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:40:35.893463 neon-utils-1.5.1a5/tests/valid_skill/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/valid_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/validator_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-15 19:40:30.000000 neon-utils-1.5.1a5/tests/web_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.766621 neon-utils-1.5.1a6/neon_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/authentication_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68386 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.770621 neon-utils-1.5.1a6/neon_utils/default_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/default_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/default_configurations/default_user_conf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/location_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/messagebus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/mq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/process_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.766621 neon-utils-1.5.1a6/neon_utils/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.770621 neon-utils-1.5.1a6/neon_utils/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   428660 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/snd/loaded.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/snd/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.766621 neon-utils-1.5.1a6/neon_utils/res/text/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.770621 neon-utils-1.5.1a6/neon_utils/res/text/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/text/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/text/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/text/en-us/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/text/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.770621 neon-utils-1.5.1a6/neon_utils/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/res/ui/neon_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.770621 neon-utils-1.5.1a6/neon_utils/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/common_message_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/common_play_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/common_query_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/instructor_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/kiosk_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/mycroft_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/neon_fallback_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/neon_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/skills/skill_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/socket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/validator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/neon_utils/web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.770621 neon-utils-1.5.1a6/neon_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-17 01:00:00.000000 neon-utils-1.5.1a6/neon_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-17 01:00:00.000000 neon-utils-1.5.1a6/neon_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:00:00.000000 neon-utils-1.5.1a6/neon_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-17 01:00:00.000000 neon-utils-1.5.1a6/neon_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-17 01:00:00.000000 neon-utils-1.5.1a6/neon_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 01:00:00.000000 neon-utils-1.5.1a6/neon_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/authentication_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/cache_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/configuration_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/file_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/language_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/location_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/log_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/message_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/messagebus_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/metric_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/mq_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55268 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/neon_skill_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/net_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/packaging_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/parse_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/search_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/signal_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/tests/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/tests/skills/test_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/skills/test_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/skills/test_skill/settingsmeta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/socket_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/user_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:00:00.774621 neon-utils-1.5.1a6/tests/valid_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/valid_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/validator_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-17 00:59:57.000000 neon-utils-1.5.1a6/tests/web_util_tests.py
```

### Comparing `neon-utils-1.5.1a5/LICENSE.md` & `neon-utils-1.5.1a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/PKG-INFO` & `neon-utils-1.5.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.5.1a5
+Version: 1.5.1a6
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.5.1a5/neon_utils/__init__.py` & `neon-utils-1.5.1a6/neon_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/authentication_utils.py` & `neon-utils-1.5.1a6/neon_utils/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/cache_utils.py` & `neon-utils-1.5.1a6/neon_utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/configuration_utils.py` & `neon-utils-1.5.1a6/neon_utils/configuration_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -769,45 +769,48 @@
 
 
 def get_user_config_from_mycroft_conf(user_config: dict = None) -> dict:
     """
     Populates user_config with values from mycroft.conf
     :returns: dict modified or created user config
     """
-    from ovos_config.models import MycroftUserConfig
+    from ovos_config.config import Configuration
     user_config = user_config or \
         deepcopy(NGIConfig("default_user_conf",
                            os.path.join(os.path.dirname(__file__),
                                         "default_configurations")).content)
-    mycroft_config = MycroftUserConfig()
-    LOG.debug(f"Initializing mycroft config at {mycroft_config.path}")
-    user_config["speech"]["stt_language"] = mycroft_config.get("lang", "en-us")
-    user_config["speech"]["tts_language"] = mycroft_config.get("lang", "en-us")
+    core_config = Configuration()
+    user_config["speech"]["stt_language"] = core_config.get("lang", "en-us")
+    user_config["speech"]["tts_language"] = core_config.get("lang", "en-us")
     user_config["speech"]["alt_languages"] = \
-        mycroft_config.get("secondary_langs", [])
+        core_config.get("secondary_langs", [])
     user_config["units"]["time"] = \
-        12 if mycroft_config.get("time_format", "half") == "half" else 24
-    user_config["units"]["date"] = mycroft_config.get("date_format") or "MDY"
+        12 if core_config.get("time_format", "half") == "half" else 24
+    user_config["units"]["date"] = core_config.get("date_format") or "MDY"
     user_config["units"]["measure"] = \
-        "metric" if mycroft_config.get("system_unit") == "metric" \
+        "metric" if core_config.get("system_unit") == "metric" \
         else "imperial"
 
-    if mycroft_config.get("location"):
-        user_config["location"] = {
-            "lat": str(mycroft_config["location"]["coordinate"]["latitude"]),
-            "lng": str(mycroft_config["location"]["coordinate"]["longitude"]),
-            "city": mycroft_config["location"]["city"]["name"],
-            "state": mycroft_config["location"]["city"]["state"]["name"],
-            "country": mycroft_config["location"]["city"]["state"]
-            ["country"]["name"],
-            "tz": mycroft_config["location"]["timezone"]["code"],
-            "utc": str(round(mycroft_config["location"]["timezone"]["offset"]
-                             / 3600000, 1))}
+    if core_config.get("location"):
+        loc = user_config["location"]
+        loc['lat'] = loc['lat'] or str(core_config["location"]["coordinate"]
+                                ["latitude"])
+        loc['lng'] = loc['lng'] or str(core_config["location"]["coordinate"]
+                                ["longitude"])
+        loc['city'] = loc['city'] or core_config["location"]["city"]["name"]
+        loc['state'] = loc['state'] or \
+            core_config["location"]["city"]["state"]["name"]
+        loc['country'] = loc['country'] or \
+            core_config["location"]["city"]["state"]["country"]["name"]
+        loc['tz'] = loc['tz'] or core_config["location"]["timezone"]["code"]
+        loc['utc'] = loc['utc'] or str(round(core_config["location"]["timezone"]
+                                       ["offset"] / 3600000, 1))
+
     else:
-        LOG.warning(f"No location in config: {mycroft_config.path}")
+        LOG.warning(f"No location in core configuration")
     return user_config
 
 
 def get_neon_user_config(path: Optional[str] = None) -> NGIConfig:
     """
     Returns a dict user configuration and handles any migration of
     configuration values to local config from user config
```

### Comparing `neon-utils-1.5.1a5/neon_utils/decorators.py` & `neon-utils-1.5.1a6/neon_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/default_configurations/__init__.py` & `neon-utils-1.5.1a6/neon_utils/default_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/default_configurations/default_user_conf.yml` & `neon-utils-1.5.1a6/neon_utils/default_configurations/default_user_conf.yml`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/file_utils.py` & `neon-utils-1.5.1a6/neon_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/language_utils.py` & `neon-utils-1.5.1a6/neon_utils/language_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/location_utils.py` & `neon-utils-1.5.1a6/neon_utils/location_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/log_utils.py` & `neon-utils-1.5.1a6/neon_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/logger.py` & `neon-utils-1.5.1a6/neon_utils/logger.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/message_utils.py` & `neon-utils-1.5.1a6/neon_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/messagebus_utils.py` & `neon-utils-1.5.1a6/neon_utils/messagebus_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/metrics_utils.py` & `neon-utils-1.5.1a6/neon_utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/mq_utils.py` & `neon-utils-1.5.1a6/neon_utils/mq_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/net_utils.py` & `neon-utils-1.5.1a6/neon_utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/packaging_utils.py` & `neon-utils-1.5.1a6/neon_utils/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/parse_utils.py` & `neon-utils-1.5.1a6/neon_utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/process_utils.py` & `neon-utils-1.5.1a6/neon_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/res/snd/acknowledge.mp3` & `neon-utils-1.5.1a6/neon_utils/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/res/snd/loaded.wav` & `neon-utils-1.5.1a6/neon_utils/res/snd/loaded.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/res/snd/start_listening.wav` & `neon-utils-1.5.1a6/neon_utils/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/res/ui/neon_logo.png` & `neon-utils-1.5.1a6/neon_utils/res/ui/neon_logo.png`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/search_utils.py` & `neon-utils-1.5.1a6/neon_utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/signal_utils.py` & `neon-utils-1.5.1a6/neon_utils/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/__init__.py` & `neon-utils-1.5.1a6/neon_utils/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/common_message_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/common_message_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/common_play_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/common_play_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/common_query_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/common_query_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/instructor_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/instructor_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/kiosk_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/kiosk_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/mycroft_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/mycroft_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/neon_fallback_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/neon_fallback_skill.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,26 +34,27 @@
     from ovos_workshop.skills.fallback import FallbackSkillV1 as FallbackSkill
 except ImportError:
     from ovos_workshop.skills.fallback import FallbackSkill
 
 
 class NeonFallbackSkill(FallbackSkill, NeonSkill, OVOSSkill):
     """
-    Class that extends the NeonSkill and FallbackSkill classes to provide NeonSkill functionality to any
-    Fallback skill subclassing this class.
+    Class that extends the NeonSkill and FallbackSkill classes to provide
+    NeonSkill functionality to any Fallback skill subclassing this class.
     """
     def __init__(self, *args, **kwargs):
-        NeonSkill.__init__(self, *args, **kwargs)
-
         # Manual init of OVOSSkill
         self.private_settings = None
         self._threads = []
         self._original_converse = self.converse
         self.intent_layers = IntentLayers()
         self.audio_service = None
 
         # Manual init of FallbackSkill
         #  list of fallback handlers registered by this instance
         self.instance_fallback_handlers = []
-        # "skill_id": priority (int)  overrides
-        self.fallback_config = self.config_core["skills"].get("fallbacks", {})
+        NeonSkill.__init__(self, *args, **kwargs)
 
+    @property
+    def fallback_config(self):
+        # "skill_id": priority (int)  overrides
+        return self.config_core["skills"].get("fallbacks", {})
```

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/neon_skill.py` & `neon-utils-1.5.1a6/neon_utils/skills/neon_skill.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -281,20 +281,20 @@
         if super_return:
             return super_return
         elif super_return is False:
             if self.voc_match_cache.get(lang + voc_filename):
                 return super_return
 
         LOG.warning(f"`{voc_filename}` not found, checking in neon_core")
-        from mycroft.skills.skill_data import read_vocab_file
-        from itertools import chain
-        import re
         voc = resolve_neon_resource_file(f"text/{lang}/{voc_filename}.voc")
         if not voc:
             raise FileNotFoundError(voc)
+        from mycroft.skills.skill_data import read_vocab_file
+        from itertools import chain
+        import re
         vocab = read_vocab_file(voc)
         cache_key = lang + voc_filename
         self.voc_match_cache[cache_key] = list(chain(*vocab))
         if utt:
             if exact:
                 # Check for exact match
                 return any(i.strip() == utt
```

### Comparing `neon-utils-1.5.1a5/neon_utils/skills/skill_gui.py` & `neon-utils-1.5.1a6/neon_utils/skills/skill_gui.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/socket_utils.py` & `neon-utils-1.5.1a6/neon_utils/socket_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/user_utils.py` & `neon-utils-1.5.1a6/neon_utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/validator_utils.py` & `neon-utils-1.5.1a6/neon_utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils/web_utils.py` & `neon-utils-1.5.1a6/neon_utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils.egg-info/PKG-INFO` & `neon-utils-1.5.1a6/neon_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.5.1a5
+Version: 1.5.1a6
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.5.1a5/neon_utils.egg-info/SOURCES.txt` & `neon-utils-1.5.1a6/neon_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/neon_utils.egg-info/requires.txt` & `neon-utils-1.5.1a6/neon_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/setup.py` & `neon-utils-1.5.1a6/setup.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/__init__.py` & `neon-utils-1.5.1a6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/authentication_util_tests.py` & `neon-utils-1.5.1a6/tests/authentication_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/cache_util_tests.py` & `neon-utils-1.5.1a6/tests/cache_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/configuration_util_tests.py` & `neon-utils-1.5.1a6/tests/configuration_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/file_util_tests.py` & `neon-utils-1.5.1a6/tests/file_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/language_util_tests.py` & `neon-utils-1.5.1a6/tests/language_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/location_util_tests.py` & `neon-utils-1.5.1a6/tests/location_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/log_util_tests.py` & `neon-utils-1.5.1a6/tests/log_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/message_util_tests.py` & `neon-utils-1.5.1a6/tests/message_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/messagebus_util_tests.py` & `neon-utils-1.5.1a6/tests/messagebus_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/metric_util_tests.py` & `neon-utils-1.5.1a6/tests/metric_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/mq_util_tests.py` & `neon-utils-1.5.1a6/tests/mq_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/neon_skill_tests.py` & `neon-utils-1.5.1a6/tests/neon_skill_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/net_util_tests.py` & `neon-utils-1.5.1a6/tests/net_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/packaging_util_tests.py` & `neon-utils-1.5.1a6/tests/packaging_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/parse_util_tests.py` & `neon-utils-1.5.1a6/tests/parse_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/search_util_tests.py` & `neon-utils-1.5.1a6/tests/search_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/signal_util_tests.py` & `neon-utils-1.5.1a6/tests/signal_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/skills/__init__.py` & `neon-utils-1.5.1a6/tests/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/skills/test_skill/__init__.py` & `neon-utils-1.5.1a6/tests/skills/test_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/socket_utils_tests.py` & `neon-utils-1.5.1a6/tests/socket_utils_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/user_util_tests.py` & `neon-utils-1.5.1a6/tests/user_util_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import shutil
+
 import sys
 import os
 import unittest
-from os.path import join, dirname
+
 from copy import deepcopy
+from os.path import join
 from threading import Event
-
+from unittest.mock import patch
 from ovos_bus_client import Message
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 
 
 class UserUtilTests(unittest.TestCase):
     def test_get_user_prefs(self):
@@ -67,23 +68,23 @@
 
         def wrapper(message, valid_dict):
             self.assertEqual(get_user_prefs(), valid_dict)
 
         wrapper(test_message_1, user_1)
         wrapper(test_message_2, user_2)
 
-    def test_get_default_user_config_from_mycroft_conf(self):
+    @patch("ovos_config.config.Configuration")
+    def test_get_default_user_config_from_mycroft_conf(self, config):
+        from ovos_config.models import LocalConf
         # Patch configuration for test
         test_config_dir = os.path.join(os.path.dirname(__file__),
                                        "user_util_test_config")
-        os.environ["XDG_CONFIG_HOME"] = test_config_dir
+        config.return_value = LocalConf(join(test_config_dir, "mycroft",
+                                             "mycroft.conf"))
         import importlib
-        import ovos_config
-        importlib.reload(ovos_config.locations)
-        importlib.reload(ovos_config.models)
         from neon_utils import user_utils
         importlib.reload(user_utils)
         from neon_utils.user_utils import get_default_user_config
         user_config = get_default_user_config()
         self.assertFalse(os.path.isfile(os.path.join(test_config_dir,
                                                      "ngi_user_info.yml")))
         self.assertIsInstance(user_config, dict)
@@ -92,16 +93,14 @@
                           "lng": '-95.23525',
                           "tz": 'America/Chicago',
                           "utc": '-6.0',
                           "city": 'Kirkland',
                           "state": 'Washington',
                           "country": "United States"})
 
-        os.environ.pop("XDG_CONFIG_HOME")
-
     def test_update_user_profile(self):
         from neon_utils.user_utils import update_user_profile
         from ovos_utils.messagebus import FakeBus
 
         test_config_dir = os.path.join(os.path.dirname(__file__),
                                        "user_util_test_config")
         os.environ["NEON_CONFIG_PATH"] = test_config_dir
```

### Comparing `neon-utils-1.5.1a5/tests/valid_skill/__init__.py` & `neon-utils-1.5.1a6/tests/valid_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/validator_util_tests.py` & `neon-utils-1.5.1a6/tests/validator_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a5/tests/web_util_tests.py` & `neon-utils-1.5.1a6/tests/web_util_tests.py`

 * *Files identical despite different names*

