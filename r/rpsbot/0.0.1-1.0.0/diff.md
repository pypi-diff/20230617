# Comparing `tmp/rpsbot-0.0.1.tar.gz` & `tmp/rpsbot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpsbot-0.0.1.tar", last modified: Sat Jun 17 16:27:48 2023, max compression
+gzip compressed data, was "rpsbot-1.0.0.tar", last modified: Sat Jun 17 17:00:11 2023, max compression
```

## Comparing `rpsbot-0.0.1.tar` & `rpsbot-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-17 16:27:48.135545 rpsbot-0.0.1/
--rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-17 16:27:48.138544 rpsbot-0.0.1/PKG-INFO
-drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-17 16:27:48.072045 rpsbot-0.0.1/rpsbot.egg-info/
--rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-17 16:27:47.000000 rpsbot-0.0.1/rpsbot.egg-info/PKG-INFO
--rwxrwxrwx   0 elia      (1000) elia      (1000)      181 2023-06-17 16:27:47.000000 rpsbot-0.0.1/rpsbot.egg-info/SOURCES.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)        1 2023-06-17 16:27:47.000000 rpsbot-0.0.1/rpsbot.egg-info/dependency_links.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)       40 2023-06-17 16:27:47.000000 rpsbot-0.0.1/rpsbot.egg-info/entry_points.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)        7 2023-06-17 16:27:47.000000 rpsbot-0.0.1/rpsbot.egg-info/top_level.txt
--rwxrwxrwx   0 elia      (1000) elia      (1000)       63 2023-06-17 16:03:34.000000 rpsbot-0.0.1/rpsbot.py
--rwxrwxrwx   0 elia      (1000) elia      (1000)      286 2023-06-17 16:27:48.154322 rpsbot-0.0.1/setup.cfg
--rwxrwxrwx   0 elia      (1000) elia      (1000)      270 2023-06-17 16:24:19.000000 rpsbot-0.0.1/setup.py
+drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-17 17:00:11.297598 rpsbot-1.0.0/
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-17 17:00:11.300598 rpsbot-1.0.0/PKG-INFO
+drwxrwxrwx   0 elia      (1000) elia      (1000)        0 2023-06-17 17:00:11.236610 rpsbot-1.0.0/rpsbot.egg-info/
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      311 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/PKG-INFO
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      181 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)        1 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)       40 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/entry_points.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)        7 2023-06-17 17:00:10.000000 rpsbot-1.0.0/rpsbot.egg-info/top_level.txt
+-rwxrwxrwx   0 elia      (1000) elia      (1000)     1684 2023-06-17 16:58:55.000000 rpsbot-1.0.0/rpsbot.py
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      286 2023-06-17 17:00:11.316794 rpsbot-1.0.0/setup.cfg
+-rwxrwxrwx   0 elia      (1000) elia      (1000)      270 2023-06-17 16:24:19.000000 rpsbot-1.0.0/setup.py
```

