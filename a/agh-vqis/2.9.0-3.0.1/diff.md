# Comparing `tmp/agh_vqis-2.9.0.tar.gz` & `tmp/agh_vqis-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-2.9.0.tar", last modified: Fri Jun  9 16:44:33 2023, max compression
+gzip compressed data, was "agh_vqis-3.0.1.tar", last modified: Fri Jun 16 19:07:33 2023, max compression
```

## Comparing `agh_vqis-2.9.0.tar` & `agh_vqis-3.0.1.tar`

### file list

```diff
@@ -1,34 +1,146 @@
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.353196 agh_vqis-2.9.0/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     2802 2023-06-09 14:59:22.000000 agh_vqis-2.9.0/LICENSE
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     4702 2023-06-09 16:44:33.353196 agh_vqis-2.9.0/PKG-INFO
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     3718 2023-06-09 16:40:43.000000 agh_vqis-2.9.0/README.md
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/agh_vqis.egg-info/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     4702 2023-06-09 16:44:33.000000 agh_vqis-2.9.0/agh_vqis.egg-info/PKG-INFO
--rw-rw-r--   0 filek7    (1000) filek7    (1000)      666 2023-06-09 16:44:33.000000 agh_vqis-2.9.0/agh_vqis.egg-info/SOURCES.txt
--rw-rw-r--   0 filek7    (1000) filek7    (1000)        1 2023-06-09 16:44:33.000000 agh_vqis-2.9.0/agh_vqis.egg-info/dependency_links.txt
--rw-rw-r--   0 filek7    (1000) filek7    (1000)      205 2023-06-09 16:44:33.000000 agh_vqis-2.9.0/agh_vqis.egg-info/requires.txt
--rw-rw-r--   0 filek7    (1000) filek7    (1000)       14 2023-06-09 16:44:33.000000 agh_vqis-2.9.0/agh_vqis.egg-info/top_level.txt
--rw-rw-r--   0 filek7    (1000) filek7    (1000)       94 2023-06-09 14:59:22.000000 agh_vqis-2.9.0/pyproject.toml
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/python-cpbd/
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/python-cpbd/cpbd/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)       46 2023-06-09 16:10:26.000000 agh_vqis-2.9.0/python-cpbd/cpbd/__init__.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     7459 2023-06-09 16:10:26.000000 agh_vqis-2.9.0/python-cpbd/cpbd/compute.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     1481 2023-06-09 16:10:26.000000 agh_vqis-2.9.0/python-cpbd/cpbd/octave.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     1279 2023-06-09 16:44:33.353196 agh_vqis-2.9.0/setup.cfg
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/src/
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/src/agh_vqis/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)      356 2023-06-09 16:43:59.000000 agh_vqis-2.9.0/src/agh_vqis/__init__.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)    21441 2023-06-09 16:20:13.000000 agh_vqis-2.9.0/src/agh_vqis/__main__.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)      202 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/_governor.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     1349 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/_logger.py
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/src/agh_vqis/binaries/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)    97508 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
--rw-rw-r--   0 filek7    (1000) filek7    (1000)   127167 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
--rwxrwxr-x   0 filek7    (1000) filek7    (1000)    66424 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.349197 agh_vqis-2.9.0/src/agh_vqis/models/
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.353196 agh_vqis-2.9.0/src/agh_vqis/models/ugc/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)   779962 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/models/ugc/12k_all_set.json
--rw-rw-r--   0 filek7    (1000) filek7    (1000)   412834 2023-06-09 09:10:29.000000 agh_vqis-2.9.0/src/agh_vqis/models/ugc/9k_all_set.json
-drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:44:33.353196 agh_vqis-2.9.0/src/agh_vqis/utils/
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     4748 2023-06-09 15:48:27.000000 agh_vqis-2.9.0/src/agh_vqis/utils/helpers.py
--rw-rw-r--   0 filek7    (1000) filek7    (1000)     6368 2023-06-09 12:38:14.000000 agh_vqis-2.9.0/src/agh_vqis/utils/ugc.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.526980 agh_vqis-3.0.1/
+-rw-rw-rw-   0        0        0     2826 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7317 2023-06-16 19:07:33.526980 agh_vqis-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6309 2023-06-16 19:04:34.000000 agh_vqis-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.398168 agh_vqis-3.0.1/agh_vqis.egg-info/
+-rw-rw-rw-   0        0        0     7317 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8077 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 19:07:32.000000 agh_vqis-3.0.1/agh_vqis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.337999 agh_vqis-3.0.1/python-cpbd/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.413906 agh_vqis-3.0.1/python-cpbd/cpbd/
+-rw-rw-rw-   0        0        0       49 2023-06-09 20:24:14.000000 agh_vqis-3.0.1/python-cpbd/cpbd/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-06-09 20:24:14.000000 agh_vqis-3.0.1/python-cpbd/cpbd/compute.py
+-rw-rw-rw-   0        0        0     1540 2023-06-09 20:24:14.000000 agh_vqis-3.0.1/python-cpbd/cpbd/octave.py
+-rw-rw-rw-   0        0        0     1329 2023-06-16 19:07:33.540207 agh_vqis-3.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.337999 agh_vqis-3.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.429538 agh_vqis-3.0.1/src/agh_vqis/
+-rw-rw-rw-   0        0        0      381 2023-06-16 19:03:24.000000 agh_vqis-3.0.1/src/agh_vqis/__init__.py
+-rw-rw-rw-   0        0        0    21928 2023-06-16 19:06:30.000000 agh_vqis-3.0.1/src/agh_vqis/__main__.py
+-rw-rw-rw-   0        0        0     1349 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/src/agh_vqis/_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.445290 agh_vqis-3.0.1/src/agh_vqis/binaries/
+-rw-rw-rw-   0        0        0    97508 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
+-rwxrwxrwx   0        0        0   123613 2023-06-16 18:18:43.000000 agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
+-rw-rw-rw-   0        0        0    66424 2023-06-09 20:08:24.000000 agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:32.349617 agh_vqis-3.0.1/src/agh_vqis/models/
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.486661 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/
+-rw-rw-rw-   0        0        0    21075 2023-05-23 22:55:31.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    21723 2023-05-23 22:55:33.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    14595 2023-05-23 22:55:36.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    15027 2023-05-23 22:55:38.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    32379 2023-05-23 22:56:00.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    35763 2023-05-23 22:56:02.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:04.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:06.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:08.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    34035 2023-05-23 22:56:10.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    29643 2023-05-23 22:55:40.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
+-rw-rw-rw-   0        0        0    33747 2023-05-23 22:55:42.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
+-rw-rw-rw-   0        0        0    28059 2023-05-23 22:55:44.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-05-23 22:55:45.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
+-rw-rw-rw-   0        0        0    33531 2023-05-23 22:55:46.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
+-rw-rw-rw-   0        0        0    29355 2023-05-23 22:55:48.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
+-rw-rw-rw-   0        0        0    26691 2023-05-23 22:55:50.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
+-rw-rw-rw-   0        0        0    31803 2023-05-23 22:55:52.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-05-23 22:55:58.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    30291 2023-05-23 22:55:54.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
+-rw-rw-rw-   0        0        0    30795 2023-05-23 22:55:56.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:50.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    26907 2023-05-23 22:56:50.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    38355 2023-05-23 22:56:42.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
+-rw-rw-rw-   0        0        0    39075 2023-05-23 22:56:44.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:46.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:49.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:58.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-05-23 22:56:59.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38571 2023-05-23 22:56:51.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
+-rw-rw-rw-   0        0        0    39219 2023-05-23 22:56:55.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-05-23 22:56:56.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    37995 2023-05-23 22:56:57.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-05-23 22:57:03.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-05-23 22:57:07.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    38643 2023-05-23 22:57:00.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
+-rw-rw-rw-   0        0        0    39363 2023-05-23 22:57:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
+-rw-rw-rw-   0        0        0    38067 2023-05-23 22:57:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
+-rw-rw-rw-   0        0        0    38211 2023-05-23 22:57:02.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    36915 2023-05-23 22:56:15.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:16.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:17.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
+-rw-rw-rw-   0        0        0    28779 2023-05-23 22:56:11.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
+-rw-rw-rw-   0        0        0    29715 2023-05-23 22:56:13.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
+-rw-rw-rw-   0        0        0    30219 2023-05-23 22:56:14.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:23.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    38283 2023-05-23 22:56:25.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
+-rw-rw-rw-   0        0        0    37563 2023-05-23 22:56:26.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
+-rw-rw-rw-   0        0        0    27843 2023-05-23 22:56:18.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-05-23 22:56:19.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
+-rw-rw-rw-   0        0        0    27699 2023-05-23 22:56:20.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:30.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    37275 2023-05-23 22:56:31.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:32.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
+-rw-rw-rw-   0        0        0    29283 2023-05-23 22:56:27.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
+-rw-rw-rw-   0        0        0    27483 2023-05-23 22:56:27.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:28.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:37.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    38139 2023-05-23 22:56:38.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:40.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-05-23 22:56:33.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:32.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    17835 2023-05-23 22:57:32.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    27411 2023-05-23 22:57:28.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    25179 2023-05-23 22:57:30.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    22659 2023-05-23 22:57:31.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:34.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    17187 2023-05-23 22:57:44.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    25395 2023-05-23 22:57:33.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:34.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:51.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    16827 2023-05-23 22:57:52.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    23667 2023-05-23 22:57:49.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:08.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:09.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
+-rw-rw-rw-   0        0        0    22299 2023-05-23 22:57:10.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
+-rw-rw-rw-   0        0        0    22155 2023-05-23 22:57:14.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    19059 2023-05-23 22:57:12.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
+-rw-rw-rw-   0        0        0    18987 2023-05-23 22:57:12.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:13.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
+-rw-rw-rw-   0        0        0    23163 2023-05-23 22:57:20.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:21.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    22011 2023-05-23 22:57:15.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
+-rw-rw-rw-   0        0        0    20283 2023-05-23 22:57:16.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
+-rw-rw-rw-   0        0        0    18123 2023-05-23 22:57:17.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
+-rw-rw-rw-   0        0        0    22947 2023-05-23 22:57:25.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:26.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    22587 2023-05-23 22:57:26.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:22.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
+-rw-rw-rw-   0        0        0    21435 2023-05-23 22:57:23.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
+-rw-rw-rw-   0        0        0    18699 2023-05-23 22:57:24.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
+-rw-rw-rw-   0        0        0     4587 2023-05-23 22:57:59.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0     5739 2023-05-23 22:57:53.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
+-rw-rw-rw-   0        0        0     6459 2023-05-23 22:57:54.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
+-rw-rw-rw-   0        0        0     5307 2023-05-23 22:57:55.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
+-rw-rw-rw-   0        0        0     5811 2023-05-23 22:57:56.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
+-rw-rw-rw-   0        0        0     4947 2023-05-23 22:57:57.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
+-rw-rw-rw-   0        0        0     5379 2023-05-23 22:57:58.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
+-rw-rw-rw-   0        0        0     5163 2023-05-23 22:57:57.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
+-rw-rw-rw-   0        0        0    40443 2023-05-23 22:58:18.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    43467 2023-05-23 22:58:19.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    39435 2023-05-23 22:58:21.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    42171 2023-05-23 22:58:22.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38787 2023-05-23 22:58:23.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    42747 2023-05-23 22:58:00.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
+-rw-rw-rw-   0        0        0    39939 2023-05-23 22:58:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
+-rw-rw-rw-   0        0        0    41235 2023-05-23 22:58:01.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
+-rw-rw-rw-   0        0        0    38931 2023-05-23 22:58:02.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
+-rw-rw-rw-   0        0        0    40875 2023-05-23 22:58:03.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-05-23 22:58:16.000000 agh_vqis-3.0.1/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.506214 agh_vqis-3.0.1/src/agh_vqis/models/ugc/
+-rw-rw-rw-   0        0        0   594166 2023-06-13 12:09:35.000000 agh_vqis-3.0.1/src/agh_vqis/models/ugc/12k_all_set.json
+drwxrwxrwx   0        0        0        0 2023-06-16 19:07:33.526980 agh_vqis-3.0.1/src/agh_vqis/utils/
+-rw-rw-rw-   0        0        0     5470 2023-06-16 19:06:30.000000 agh_vqis-3.0.1/src/agh_vqis/utils/helpers.py
+-rw-rw-rw-   0        0        0      754 2023-06-09 21:13:23.000000 agh_vqis-3.0.1/src/agh_vqis/utils/resolution_cast.py
+-rw-rw-rw-   0        0        0     5735 2023-06-13 12:52:00.000000 agh_vqis-3.0.1/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-2.9.0/LICENSE` & `agh_vqis-3.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-NOTE:
-This evaluation license agreement is made between AGH University of Science and Technology in Krakow; 30 Mickiewicza Avenue 30-059 Krakow ("AGH") and You ("Licensee"). By installing, copying, or otherwise using the licensed software, you agree to be bound by the terms of this agreement. If you are accepting these terms on behalf of the Licensee, you represent and warrant that you have full authority to bind the Licensee to these terms.
-For inquiries about purchasing a full license, contact qoe@agh.edu.pl.
-
-
-EVALUATION LICENSE AGREEMENT
-
-1. SCOPE: This license agreement governs the terms and conditions of using the Python package for automatic image distortion detection ("agh-vqis" or "Software").
-
-2. EVALUATION LICENSE: AGH grants the Licensee a non-exclusive, non-transferable, non-sublicensable and revocable license to use the Software by reproducing it and running it on any number of devices, only for evaluation purposes, i.e. to allow the Licensee to become familiar with its functions before making a decision about purchasing a full license.
-
-3. DOCUMENTATION: If AGH makes any documentation available to the Licensee, the Licensee may use it for the same purposes, for which they may use the Software and make copies of it for the personnel using the Software.
-
-4. FREE OF CHARGE: Due to the nature of the license, it is granted free of charge.
-
-5. RESTRICTIONS: The Licensee may not use the Software nor its documentation for purposes not described in this agreement without separate authorization by AGH. The license does not authorize the Licensee to use the Software for production purposes, including in any commercial activity, nor to modify it, distribute it or otherwise make it available to third parties.
-
-6. THIRD PARTY COMPONENTS: To the extent that Software contains components to which a third party owns the copyright, such components are subject to license terms described in the documentation.
-
-7. PERIOD: The license is granted for an unlimited time. If the Licensee infringes intellectual property rights of AGH or breaches the obligations described in this Agreement, AGH may terminate the license with immediate effect.
-
-8. LIABILITY: Due to the nature of the license, AGH is not liable for any damages which may arise in connection with the use of the Software (e.g. due to its improper functioning, lack of expected functionality, other issues or legal defects). However, this exclusion does not apply to situations when damages arise due to intentional behaviour of AGH or when the mandatory provisions of the law do not allow to limit the liability.
-
-9. LAW AND VENUE: The License Agreement shall be governed by Polish law. Polish courts shall have jurisdiction with regard to any disputes arising from the License Agreement or in connection with it.
+NOTE:
+This evaluation license agreement is made between AGH University of Science and Technology in Krakow; 30 Mickiewicza Avenue 30-059 Krakow ("AGH") and You ("Licensee"). By installing, copying, or otherwise using the licensed software, you agree to be bound by the terms of this agreement. If you are accepting these terms on behalf of the Licensee, you represent and warrant that you have full authority to bind the Licensee to these terms.
+For inquiries about purchasing a full license, contact qoe@agh.edu.pl.
+
+
+EVALUATION LICENSE AGREEMENT
+
+1. SCOPE: This license agreement governs the terms and conditions of using the Python package for automatic image distortion detection ("agh-vqis" or "Software").
+
+2. EVALUATION LICENSE: AGH grants the Licensee a non-exclusive, non-transferable, non-sublicensable and revocable license to use the Software by reproducing it and running it on any number of devices, only for evaluation purposes, i.e. to allow the Licensee to become familiar with its functions before making a decision about purchasing a full license.
+
+3. DOCUMENTATION: If AGH makes any documentation available to the Licensee, the Licensee may use it for the same purposes, for which they may use the Software and make copies of it for the personnel using the Software.
+
+4. FREE OF CHARGE: Due to the nature of the license, it is granted free of charge.
+
+5. RESTRICTIONS: The Licensee may not use the Software nor its documentation for purposes not described in this agreement without separate authorization by AGH. The license does not authorize the Licensee to use the Software for production purposes, including in any commercial activity, nor to modify it, distribute it or otherwise make it available to third parties.
+
+6. THIRD PARTY COMPONENTS: To the extent that Software contains components to which a third party owns the copyright, such components are subject to license terms described in the documentation.
+
+7. PERIOD: The license is granted for an unlimited time. If the Licensee infringes intellectual property rights of AGH or breaches the obligations described in this Agreement, AGH may terminate the license with immediate effect.
+
+8. LIABILITY: Due to the nature of the license, AGH is not liable for any damages which may arise in connection with the use of the Software (e.g. due to its improper functioning, lack of expected functionality, other issues or legal defects). However, this exclusion does not apply to situations when damages arise due to intentional behaviour of AGH or when the mandatory provisions of the law do not allow to limit the liability.
+
+9. LAW AND VENUE: The License Agreement shall be governed by Polish law. Polish courts shall have jurisdiction with regard to any disputes arising from the License Agreement or in connection with it.
```

### Comparing `agh_vqis-2.9.0/python-cpbd/cpbd/compute.py` & `agh_vqis-3.0.1/python-cpbd/cpbd/compute.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-# coding: utf-8
-
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals
-)
-
-from math import atan2, pi
-from sys import argv
-
-import numpy as np
-from imageio import imread
-from skimage.feature import canny
-
-from cpbd.octave import sobel
-
-
-# threshold to characterize blocks as edge/non-edge blocks
-THRESHOLD = 0.002
-
-# fitting parameter
-BETA = 3.6
-
-# block size
-BLOCK_HEIGHT, BLOCK_WIDTH = (64, 64)
-
-# just noticeable widths based on the perceptual experiments
-WIDTH_JNB = np.concatenate([5*np.ones(51), 3*np.ones(205)])
-
-
-def compute(image):
-    # type: (numpy.ndarray) -> float
-    """Compute the sharpness metric for the given data."""
-
-    # convert the image to double for further processing
-    image = image.astype(np.float64)
-
-    # edge detection using canny and sobel canny edge detection is done to
-    # classify the blocks as edge or non-edge blocks and sobel edge
-    # detection is done for the purpose of edge width measurement.
-    canny_edges = canny(image)
-    sobel_edges = sobel(image)
-
-    # edge width calculation
-    marziliano_widths = marziliano_method(sobel_edges, image)
-
-    # sharpness metric calculation
-    return _calculate_sharpness_metric(image, canny_edges, marziliano_widths)
-
-
-def marziliano_method(edges, image):
-    # type: (numpy.ndarray, numpy.ndarray) -> numpy.ndarray
-    """
-    Calculate the widths of the given edges.
-
-    :return: A matrix with the same dimensions as the given image with 0's at
-        non-edge locations and edge-widths at the edge locations.
-    """
-
-    # `edge_widths` consists of zero and non-zero values. A zero value
-    # indicates that there is no edge at that position and a non-zero value
-    # indicates that there is an edge at that position and the value itself
-    # gives the edge width.
-    edge_widths = np.zeros(image.shape)
-
-    # find the gradient for the image
-    gradient_y, gradient_x = np.gradient(image)
-
-    # dimensions of the image
-    img_height, img_width = image.shape
-
-    # holds the angle information of the edges
-    edge_angles = np.zeros(image.shape)
-
-    # calculate the angle of the edges
-    for row in range(img_height):
-        for col in range(img_width):
-            if gradient_x[row, col] != 0:
-                edge_angles[row, col] = atan2(gradient_y[row, col], gradient_x[row, col]) * (180 / pi)
-            elif gradient_x[row, col] == 0 and gradient_y[row, col] == 0:
-                edge_angles[row,col] = 0
-            elif gradient_x[row, col] == 0 and gradient_y[row, col] == pi/2:
-                edge_angles[row, col] = 90
-
-
-    if np.any(edge_angles):
-
-        # quantize the angle
-        quantized_angles = 45 * np.round(edge_angles / 45)
-
-        for row in range(1, img_height - 1):
-            for col in range(1, img_width - 1):
-                if edges[row, col] == 1:
-
-                    # gradient angle = 180 or -180
-                    if quantized_angles[row, col] == 180 or quantized_angles[row, col] == -180:
-                        for margin in range(100 + 1):
-                            inner_border = (col - 1) - margin
-                            outer_border = (col - 2) - margin
-
-                            # outside image or intensity increasing from left to right
-                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) <= 0:
-                                break
-
-                        width_left = margin + 1
-
-                        for margin in range(100 + 1):
-                            inner_border = (col + 1) + margin
-                            outer_border = (col + 2) + margin
-
-                            # outside image or intensity increasing from left to right
-                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) >= 0:
-                                break
-
-                        width_right = margin + 1
-
-                        edge_widths[row, col] = width_left + width_right
-
-
-                    # gradient angle = 0
-                    if quantized_angles[row, col] == 0:
-                        for margin in range(100 + 1):
-                            inner_border = (col - 1) - margin
-                            outer_border = (col - 2) - margin
-
-                            # outside image or intensity decreasing from left to right
-                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) >= 0:
-                                break
-
-                        width_left = margin + 1
-
-                        for margin in range(100 + 1):
-                            inner_border = (col + 1) + margin
-                            outer_border = (col + 2) + margin
-
-                            # outside image or intensity decreasing from left to right
-                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) <= 0:
-                                break
-
-                        width_right = margin + 1
-
-                        edge_widths[row, col] = width_right + width_left
-
-    return edge_widths
-
-
-def _calculate_sharpness_metric(image, edges, edge_widths):
-    # type: (numpy.array, numpy.array, numpy.array) -> numpy.float64
-
-    # get the size of image
-    img_height, img_width = image.shape
-
-    total_num_edges = 0
-    hist_pblur = np.zeros(101)
-
-    # maximum block indices
-    num_blocks_vertically = int(img_height / BLOCK_HEIGHT)
-    num_blocks_horizontally = int(img_width / BLOCK_WIDTH)
-
-    #  loop over the blocks
-    for i in range(num_blocks_vertically):
-        for j in range(num_blocks_horizontally):
-
-            # get the row and col indices for the block pixel positions
-            rows = slice(BLOCK_HEIGHT * i, BLOCK_HEIGHT * (i + 1))
-            cols = slice(BLOCK_WIDTH * j, BLOCK_WIDTH * (j + 1))
-
-            if is_edge_block(edges[rows, cols], THRESHOLD):
-                block_widths = edge_widths[rows, cols]
-                # rotate block to simulate column-major boolean indexing
-                block_widths = np.rot90(np.flipud(block_widths), 3)
-                block_widths = block_widths[block_widths != 0]
-
-                block_contrast = get_block_contrast(image[rows, cols])
-                block_jnb = WIDTH_JNB[block_contrast]
-
-                # calculate the probability of blur detection at the edges
-                # detected in the block
-                prob_blur_detection = 1 - np.exp(-abs(block_widths/block_jnb) ** BETA)
-
-                # update the statistics using the block information
-                for probability in prob_blur_detection:
-                    bucket = int(round(probability * 100))
-                    hist_pblur[bucket] += 1
-                    total_num_edges += 1
-
-    # normalize the pdf
-    if total_num_edges > 0:
-        hist_pblur = hist_pblur / total_num_edges
-
-    # calculate the sharpness metric
-    return np.sum(hist_pblur[:64])
-
-
-def is_edge_block(block, threshold):
-    # type: (numpy.ndarray, float) -> bool
-    """Decide whether the given block is an edge block."""
-    return np.count_nonzero(block) > (block.size * threshold)
-
-
-def get_block_contrast(block):
-    # type: (numpy.ndarray) -> int
-    return int(np.max(block) - np.min(block))
-
-
-if __name__ == '__main__':
-    input_image = imread(argv[1], pilmode = 'L')
-    sharpness = compute(input_image)
-    print('CPBD sharpness for %s: %f' % (argv[1], sharpness))
+# coding: utf-8
+
+from __future__ import (
+    absolute_import,
+    division,
+    print_function,
+    unicode_literals
+)
+
+from math import atan2, pi
+from sys import argv
+
+import numpy as np
+from imageio import imread
+from skimage.feature import canny
+
+from cpbd.octave import sobel
+
+
+# threshold to characterize blocks as edge/non-edge blocks
+THRESHOLD = 0.002
+
+# fitting parameter
+BETA = 3.6
+
+# block size
+BLOCK_HEIGHT, BLOCK_WIDTH = (64, 64)
+
+# just noticeable widths based on the perceptual experiments
+WIDTH_JNB = np.concatenate([5*np.ones(51), 3*np.ones(205)])
+
+
+def compute(image):
+    # type: (numpy.ndarray) -> float
+    """Compute the sharpness metric for the given data."""
+
+    # convert the image to double for further processing
+    image = image.astype(np.float64)
+
+    # edge detection using canny and sobel canny edge detection is done to
+    # classify the blocks as edge or non-edge blocks and sobel edge
+    # detection is done for the purpose of edge width measurement.
+    canny_edges = canny(image)
+    sobel_edges = sobel(image)
+
+    # edge width calculation
+    marziliano_widths = marziliano_method(sobel_edges, image)
+
+    # sharpness metric calculation
+    return _calculate_sharpness_metric(image, canny_edges, marziliano_widths)
+
+
+def marziliano_method(edges, image):
+    # type: (numpy.ndarray, numpy.ndarray) -> numpy.ndarray
+    """
+    Calculate the widths of the given edges.
+
+    :return: A matrix with the same dimensions as the given image with 0's at
+        non-edge locations and edge-widths at the edge locations.
+    """
+
+    # `edge_widths` consists of zero and non-zero values. A zero value
+    # indicates that there is no edge at that position and a non-zero value
+    # indicates that there is an edge at that position and the value itself
+    # gives the edge width.
+    edge_widths = np.zeros(image.shape)
+
+    # find the gradient for the image
+    gradient_y, gradient_x = np.gradient(image)
+
+    # dimensions of the image
+    img_height, img_width = image.shape
+
+    # holds the angle information of the edges
+    edge_angles = np.zeros(image.shape)
+
+    # calculate the angle of the edges
+    for row in range(img_height):
+        for col in range(img_width):
+            if gradient_x[row, col] != 0:
+                edge_angles[row, col] = atan2(gradient_y[row, col], gradient_x[row, col]) * (180 / pi)
+            elif gradient_x[row, col] == 0 and gradient_y[row, col] == 0:
+                edge_angles[row,col] = 0
+            elif gradient_x[row, col] == 0 and gradient_y[row, col] == pi/2:
+                edge_angles[row, col] = 90
+
+
+    if np.any(edge_angles):
+
+        # quantize the angle
+        quantized_angles = 45 * np.round(edge_angles / 45)
+
+        for row in range(1, img_height - 1):
+            for col in range(1, img_width - 1):
+                if edges[row, col] == 1:
+
+                    # gradient angle = 180 or -180
+                    if quantized_angles[row, col] == 180 or quantized_angles[row, col] == -180:
+                        for margin in range(100 + 1):
+                            inner_border = (col - 1) - margin
+                            outer_border = (col - 2) - margin
+
+                            # outside image or intensity increasing from left to right
+                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) <= 0:
+                                break
+
+                        width_left = margin + 1
+
+                        for margin in range(100 + 1):
+                            inner_border = (col + 1) + margin
+                            outer_border = (col + 2) + margin
+
+                            # outside image or intensity increasing from left to right
+                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) >= 0:
+                                break
+
+                        width_right = margin + 1
+
+                        edge_widths[row, col] = width_left + width_right
+
+
+                    # gradient angle = 0
+                    if quantized_angles[row, col] == 0:
+                        for margin in range(100 + 1):
+                            inner_border = (col - 1) - margin
+                            outer_border = (col - 2) - margin
+
+                            # outside image or intensity decreasing from left to right
+                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) >= 0:
+                                break
+
+                        width_left = margin + 1
+
+                        for margin in range(100 + 1):
+                            inner_border = (col + 1) + margin
+                            outer_border = (col + 2) + margin
+
+                            # outside image or intensity decreasing from left to right
+                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) <= 0:
+                                break
+
+                        width_right = margin + 1
+
+                        edge_widths[row, col] = width_right + width_left
+
+    return edge_widths
+
+
+def _calculate_sharpness_metric(image, edges, edge_widths):
+    # type: (numpy.array, numpy.array, numpy.array) -> numpy.float64
+
+    # get the size of image
+    img_height, img_width = image.shape
+
+    total_num_edges = 0
+    hist_pblur = np.zeros(101)
+
+    # maximum block indices
+    num_blocks_vertically = int(img_height / BLOCK_HEIGHT)
+    num_blocks_horizontally = int(img_width / BLOCK_WIDTH)
+
+    #  loop over the blocks
+    for i in range(num_blocks_vertically):
+        for j in range(num_blocks_horizontally):
+
+            # get the row and col indices for the block pixel positions
+            rows = slice(BLOCK_HEIGHT * i, BLOCK_HEIGHT * (i + 1))
+            cols = slice(BLOCK_WIDTH * j, BLOCK_WIDTH * (j + 1))
+
+            if is_edge_block(edges[rows, cols], THRESHOLD):
+                block_widths = edge_widths[rows, cols]
+                # rotate block to simulate column-major boolean indexing
+                block_widths = np.rot90(np.flipud(block_widths), 3)
+                block_widths = block_widths[block_widths != 0]
+
+                block_contrast = get_block_contrast(image[rows, cols])
+                block_jnb = WIDTH_JNB[block_contrast]
+
+                # calculate the probability of blur detection at the edges
+                # detected in the block
+                prob_blur_detection = 1 - np.exp(-abs(block_widths/block_jnb) ** BETA)
+
+                # update the statistics using the block information
+                for probability in prob_blur_detection:
+                    bucket = int(round(probability * 100))
+                    hist_pblur[bucket] += 1
+                    total_num_edges += 1
+
+    # normalize the pdf
+    if total_num_edges > 0:
+        hist_pblur = hist_pblur / total_num_edges
+
+    # calculate the sharpness metric
+    return np.sum(hist_pblur[:64])
+
+
+def is_edge_block(block, threshold):
+    # type: (numpy.ndarray, float) -> bool
+    """Decide whether the given block is an edge block."""
+    return np.count_nonzero(block) > (block.size * threshold)
+
+
+def get_block_contrast(block):
+    # type: (numpy.ndarray) -> int
+    return int(np.max(block) - np.min(block))
+
+
+if __name__ == '__main__':
+    input_image = imread(argv[1], pilmode = 'L')
+    sharpness = compute(input_image)
+    print('CPBD sharpness for %s: %f' % (argv[1], sharpness))
```

### Comparing `agh_vqis-2.9.0/python-cpbd/cpbd/octave.py` & `agh_vqis-3.0.1/python-cpbd/cpbd/octave.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# coding: utf-8
-
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals,
-)
-
-import numpy as np
-from scipy.ndimage import convolve
-from skimage.filters.edges import HSOBEL_WEIGHTS
-
-
-def sobel(image):
-    # type: (numpy.ndarray) -> numpy.ndarray
-    """
-    Find edges using the Sobel approximation to the derivatives.
-
-    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l196).
-    """
-
-    h1 = np.array(HSOBEL_WEIGHTS)
-    h1 /= np.sum(abs(h1))  # normalize h1
-
-    strength2 = np.square(convolve(image, h1.T))
-
-    # Note: https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l59
-    thresh2 = 2 * np.sqrt(np.mean(strength2))
-
-    strength2[strength2 <= thresh2] = 0
-    return _simple_thinning(strength2)
-
-
-def _simple_thinning(strength):
-    # type: (numpy.ndarray) -> numpy.ndarray
-    """
-    Perform a very simple thinning.
-
-    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l512).
-    """
-    num_rows, num_cols = strength.shape
-
-    zero_column = np.zeros((num_rows, 1))
-    zero_row = np.zeros((1, num_cols))
-
-    x = (
-        (strength > np.c_[zero_column, strength[:, :-1]]) &
-        (strength > np.c_[strength[:, 1:], zero_column])
-    )
-
-    y = (
-        (strength > np.r_[zero_row, strength[:-1, :]]) &
-        (strength > np.r_[strength[1:, :], zero_row])
-    )
-
-    return x | y
-
-
+# coding: utf-8
+
+from __future__ import (
+    absolute_import,
+    division,
+    print_function,
+    unicode_literals,
+)
+
+import numpy as np
+from scipy.ndimage import convolve
+from skimage.filters.edges import HSOBEL_WEIGHTS
+
+
+def sobel(image):
+    # type: (numpy.ndarray) -> numpy.ndarray
+    """
+    Find edges using the Sobel approximation to the derivatives.
+
+    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l196).
+    """
+
+    h1 = np.array(HSOBEL_WEIGHTS)
+    h1 /= np.sum(abs(h1))  # normalize h1
+
+    strength2 = np.square(convolve(image, h1.T))
+
+    # Note: https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l59
+    thresh2 = 2 * np.sqrt(np.mean(strength2))
+
+    strength2[strength2 <= thresh2] = 0
+    return _simple_thinning(strength2)
+
+
+def _simple_thinning(strength):
+    # type: (numpy.ndarray) -> numpy.ndarray
+    """
+    Perform a very simple thinning.
+
+    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l512).
+    """
+    num_rows, num_cols = strength.shape
+
+    zero_column = np.zeros((num_rows, 1))
+    zero_row = np.zeros((1, num_cols))
+
+    x = (
+        (strength > np.c_[zero_column, strength[:, :-1]]) &
+        (strength > np.c_[strength[:, 1:], zero_column])
+    )
+
+    y = (
+        (strength > np.r_[zero_row, strength[:-1, :]]) &
+        (strength > np.r_[strength[1:, :], zero_row])
+    )
+
+    return x | y
+
+
```

### Comparing `agh_vqis-2.9.0/setup.cfg` & `agh_vqis-3.0.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,84 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6167 685f 7671 6973 0a76 6572 7369  = agh_vqis.versi
-00000020: 6f6e 203d 2032 2e39 2e30 0a61 7574 686f  on = 2.9.0.autho
-00000030: 7220 3d20 4a61 6b75 6220 4e61 7761 c582  r = Jakub Nawa..
-00000040: 612c 2046 696c 6970 204b 6f72 7573 0a61  a, Filip Korus.a
-00000050: 7574 686f 725f 656d 6169 6c20 3d20 6a61  uthor_email = ja
-00000060: 6b75 622e 6e61 7761 6c61 4061 6768 2e65  kub.nawala@agh.e
-00000070: 6475 2e70 6c2c 2066 6b6f 7275 7340 7374  du.pl, fkorus@st
-00000080: 7564 656e 742e 6167 682e 6564 752e 706c  udent.agh.edu.pl
-00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
-000000a0: 2050 7974 686f 6e20 7772 6170 7065 7220   Python wrapper 
-000000b0: 666f 7220 3138 2069 6d61 6765 2071 7561  for 18 image qua
-000000c0: 6c69 7479 2069 6e64 6963 6174 6f72 732e  lity indicators.
-000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-000000f0: 2e6d 640a 6c6f 6e67 5f64 6573 6372 6970  .md.long_descrip
-00000100: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000110: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000120: 6e0a 7572 6c20 3d20 6874 7470 733a 2f2f  n.url = https://
-00000130: 716f 652e 6167 682e 6564 752e 706c 2f69  qoe.agh.edu.pl/i
-00000140: 6e64 6963 6174 6f72 732f 0a6c 6963 656e  ndicators/.licen
-00000150: 7365 203d 2045 5641 4c55 4154 494f 4e20  se = EVALUATION 
-00000160: 4c49 4345 4e53 4520 4147 5245 454d 454e  LICENSE AGREEMEN
-00000170: 540a 6c69 6365 6e73 655f 6669 6c65 7320  T.license_files 
-00000180: 3d20 4c49 4345 4e53 450a 636c 6173 7369  = LICENSE.classi
-00000190: 6669 6572 7320 3d20 0a09 5072 6f67 7261  fiers = ..Progra
-000001a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001b0: 3a20 5079 7468 6f6e 203a 3a20 330a 0950  : Python :: 3..P
-000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001e0: 2033 2e39 0a09 5072 6f67 7261 6d6d 696e   3.9..Programmin
-000001f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000200: 7468 6f6e 203a 3a20 332e 3130 0a09 5072  thon :: 3.10..Pr
-00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000230: 332e 3131 0a09 4c69 6365 6e73 6520 3a3a  3.11..License ::
-00000240: 204f 7468 6572 2f50 726f 7072 6965 7461   Other/Proprieta
-00000250: 7279 204c 6963 656e 7365 0a09 4f70 6572  ry License..Oper
-00000260: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000270: 504f 5349 5820 3a3a 204c 696e 7578 0a09  POSIX :: Linux..
-00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000290: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
-000002a0: 2057 696e 646f 7773 0a09 4f70 6572 6174   Windows..Operat
-000002b0: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
-000002c0: 634f 530a 0949 6e74 656e 6465 6420 4175  cOS..Intended Au
-000002d0: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-000002e0: 652f 5265 7365 6172 6368 0a09 496e 7465  e/Research..Inte
-000002f0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000300: 2054 656c 6563 6f6d 6d75 6e69 6361 7469   Telecommunicati
-00000310: 6f6e 7320 496e 6475 7374 7279 0a09 546f  ons Industry..To
-00000320: 7069 6320 3a3a 204d 756c 7469 6d65 6469  pic :: Multimedi
-00000330: 6120 3a3a 2056 6964 656f 0a09 546f 7069  a :: Video..Topi
-00000340: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
-00000350: 456e 6769 6e65 6572 696e 6720 3a3a 2049  Engineering :: I
-00000360: 6d61 6765 2050 726f 6365 7373 696e 670a  mage Processing.
-00000370: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
-00000380: 6765 5f64 6972 203d 2061 6768 5f76 7169  ge_dir = agh_vqi
-00000390: 733d 7372 632f 6167 685f 7671 6973 2c63  s=src/agh_vqis,c
-000003a0: 7062 643d 7079 7468 6f6e 2d63 7062 642f  pbd=python-cpbd/
-000003b0: 6370 6264 0a70 7974 686f 6e5f 7265 7175  cpbd.python_requ
-000003c0: 6972 6573 203d 203e 3d33 2e39 0a69 6e73  ires = >=3.9.ins
-000003d0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-000003e0: 0a09 6d61 7470 6c6f 746c 6962 3e3d 332e  ..matplotlib>=3.
-000003f0: 352e 310a 096e 756d 7079 3e3d 312e 3232  5.1..numpy>=1.22
-00000400: 2e33 0a09 7061 6e64 6173 3e3d 312e 342e  .3..pandas>=1.4.
-00000410: 320a 0950 494d 533e 3d30 2e35 0a09 7363  2..PIMS>=0.5..sc
-00000420: 696b 6974 2d69 6d61 6765 3e3d 302e 3139  ikit-image>=0.19
-00000430: 2e32 0a09 736c 6963 6572 6174 6f72 3e3d  .2..slicerator>=
-00000440: 312e 312e 300a 0973 6365 6e65 6465 7465  1.1.0..scenedete
-00000450: 6374 3e3d 302e 362e 302e 330a 096f 7065  ct>=0.6.0.3..ope
-00000460: 6e63 762d 7079 7468 6f6e 3e3d 342e 362e  ncv-python>=4.6.
-00000470: 302e 3636 0a09 7867 626f 6f73 743d 3d30  0.66..xgboost==0
-00000480: 2e39 300a 0973 6369 6b69 742d 6c65 6172  .90..scikit-lear
-00000490: 6e3d 3d31 2e30 2e32 0a09 6176 3e3d 382e  n==1.0.2..av>=8.
-000004a0: 302e 330a 0966 666d 7065 672d 7079 7468  0.3..ffmpeg-pyth
-000004b0: 6f6e 3e3d 302e 322e 300a 0a5b 6f70 7469  on>=0.2.0..[opti
-000004c0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-000004d0: 5d0a 2a20 3d20 2a0a 0a5b 6567 675f 696e  ].* = *..[egg_in
-000004e0: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
-000004f0: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
+00000020: 7369 6f6e 203d 2033 2e30 2e31 0d0a 6175  sion = 3.0.1..au
+00000030: 7468 6f72 203d 204a 616b 7562 204e 6177  thor = Jakub Naw
+00000040: 61c5 8261 2c20 4669 6c69 7020 4b6f 7275  a..a, Filip Koru
+00000050: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
+00000060: 3d20 6a61 6b75 622e 6e61 7761 6c61 4061  = jakub.nawala@a
+00000070: 6768 2e65 6475 2e70 6c2c 2066 6b6f 7275  gh.edu.pl, fkoru
+00000080: 7340 7374 7564 656e 742e 6167 682e 6564  s@student.agh.ed
+00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
+000000a0: 6e20 3d20 4120 5079 7468 6f6e 2077 7261  n = A Python wra
+000000b0: 7070 6572 2066 6f72 2031 3820 696d 6167  pper for 18 imag
+000000c0: 6520 7175 616c 6974 7920 696e 6469 6361  e quality indica
+000000d0: 746f 7273 2e0d 0a6c 6f6e 675f 6465 7363  tors...long_desc
+000000e0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+000000f0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
+00000100: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+00000110: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+00000120: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
+00000130: 6874 7470 733a 2f2f 716f 652e 6167 682e  https://qoe.agh.
+00000140: 6564 752e 706c 2f69 6e64 6963 6174 6f72  edu.pl/indicator
+00000150: 732f 0d0a 6c69 6365 6e73 6520 3d20 4556  s/..license = EV
+00000160: 414c 5541 5449 4f4e 204c 4943 454e 5345  ALUATION LICENSE
+00000170: 2041 4752 4545 4d45 4e54 0d0a 6c69 6365   AGREEMENT..lice
+00000180: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
+00000190: 4e53 450d 0a63 6c61 7373 6966 6965 7273  NSE..classifiers
+000001a0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001c0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+000001d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001f0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000210: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000220: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000230: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000240: 2e31 310d 0a09 4c69 6365 6e73 6520 3a3a  .11...License ::
+00000250: 204f 7468 6572 2f50 726f 7072 6965 7461   Other/Proprieta
+00000260: 7279 204c 6963 656e 7365 0d0a 094f 7065  ry License...Ope
+00000270: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000280: 2050 4f53 4958 203a 3a20 4c69 6e75 780d   POSIX :: Linux.
+00000290: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000002a0: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
+000002b0: 3a3a 2057 696e 646f 7773 0d0a 094f 7065  :: Windows...Ope
+000002c0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000002d0: 204d 6163 4f53 0d0a 0949 6e74 656e 6465   MacOS...Intende
+000002e0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000002f0: 6965 6e63 652f 5265 7365 6172 6368 0d0a  ience/Research..
+00000300: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000310: 6365 203a 3a20 5465 6c65 636f 6d6d 756e  ce :: Telecommun
+00000320: 6963 6174 696f 6e73 2049 6e64 7573 7472  ications Industr
+00000330: 790d 0a09 546f 7069 6320 3a3a 204d 756c  y...Topic :: Mul
+00000340: 7469 6d65 6469 6120 3a3a 2056 6964 656f  timedia :: Video
+00000350: 0d0a 0954 6f70 6963 203a 3a20 5363 6965  ...Topic :: Scie
+00000360: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+00000370: 6e67 203a 3a20 496d 6167 6520 5072 6f63  ng :: Image Proc
+00000380: 6573 7369 6e67 0d0a 0d0a 5b6f 7074 696f  essing....[optio
+00000390: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+000003a0: 203d 2061 6768 5f76 7169 733d 7372 632f   = agh_vqis=src/
+000003b0: 6167 685f 7671 6973 2c63 7062 643d 7079  agh_vqis,cpbd=py
+000003c0: 7468 6f6e 2d63 7062 642f 6370 6264 0d0a  thon-cpbd/cpbd..
+000003d0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+000003e0: 3d20 3e3d 332e 390d 0a69 6e73 7461 6c6c  = >=3.9..install
+000003f0: 5f72 6571 7569 7265 7320 3d20 0d0a 096d  _requires = ...m
+00000400: 6174 706c 6f74 6c69 623e 3d33 2e35 2e31  atplotlib>=3.5.1
+00000410: 0d0a 096e 756d 7079 3e3d 312e 3232 2e33  ...numpy>=1.22.3
+00000420: 0d0a 0970 616e 6461 733e 3d31 2e34 2e32  ...pandas>=1.4.2
+00000430: 0d0a 0950 494d 533e 3d30 2e35 0d0a 0973  ...PIMS>=0.5...s
+00000440: 6369 6b69 742d 696d 6167 653e 3d30 2e31  cikit-image>=0.1
+00000450: 392e 320d 0a09 736c 6963 6572 6174 6f72  9.2...slicerator
+00000460: 3e3d 312e 312e 300d 0a09 7363 656e 6564  >=1.1.0...scened
+00000470: 6574 6563 743e 3d30 2e36 2e30 2e33 0d0a  etect>=0.6.0.3..
+00000480: 096f 7065 6e63 762d 7079 7468 6f6e 3e3d  .opencv-python>=
+00000490: 342e 362e 302e 3636 0d0a 0978 6762 6f6f  4.6.0.66...xgboo
+000004a0: 7374 3d3d 312e 372e 350d 0a09 7363 696b  st==1.7.5...scik
+000004b0: 6974 2d6c 6561 726e 3d3d 312e 302e 320d  it-learn==1.0.2.
+000004c0: 0a09 6176 3e3d 382e 302e 330d 0a09 6666  ..av>=8.0.3...ff
+000004d0: 6d70 6567 2d70 7974 686f 6e3e 3d30 2e32  mpeg-python>=0.2
+000004e0: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
+000004f0: 6163 6b61 6765 5f64 6174 615d 0d0a 2a20  ackage_data]..* 
+00000500: 3d20 2a0d 0a0d 0a5b 6567 675f 696e 666f  = *....[egg_info
+00000510: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000520: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000530: 0a                                       .
```

### Comparing `agh_vqis-2.9.0/src/agh_vqis/__main__.py` & `agh_vqis-3.0.1/src/agh_vqis/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 # Authors: Jakub Nawała <jnawala@agh.edu.pl>, Filip Korus <fkorus@student.agh.edu.pl>
 # Created: June 1, 2021
+
 import argparse
 import logging
 
 import numpy as np
-import pandas as pd
 import pims
 from cpbd.compute import compute
 from pims import PyAVVideoReader
 
 from ._logger import setup_console_and_file_logger
 from .utils import ugc
 from .utils.helpers import *
+from .utils.resolution_cast import *
 
 logger = setup_console_and_file_logger(__name__, log_file_name=f"{__name__}.log", level=logging.INFO)
 
 allowed_mm_file_extensions = ['.jpg', '.jpeg', '.png', '.ts', '.mp4', '.y4m', '.mov', '.avi', '.mkv', '.gif', '.bmp']
 
 
-def _run_agh_viqs(mm_file_path: Path, binary_path: Path, selected_vqis=32767):
+def _run_agh_vqis(mm_file_path: Path, selected_vqis=32767):
     """
     Runs 15 VQ AGH's Video Quality Indicators (VQIs) on an input video or image (identified by *video_path*) and returns
     Pandas DataFrame with results.
 
     :param mm_file_path: path to a video or image file to process
-    :param binary_path: path to a binary executable computing VQIs
     :param selected_vqis: a positive 16-bit integer stating which VQIs to run (all are run by default)
     :return: Pandas DataFrame with VQIs results or -1 if an error occurred
     """
 
-    if binary_path is None:
-        executable_file = get_executable_filename()
-        binary_path = Path('/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]), 'binaries/', executable_file)
+    executable_file = get_executable_filename()
+    binary_path = Path(str(get_current_file_location()), 'binaries/', executable_file)
 
     if not os.access(binary_path.resolve(), os.X_OK):
         logger.error(f'{str(binary_path.resolve())} file is not executable')
         return -1
 
     logger.debug('Creating working directory')
     random_folder_name = generate_uuid()
     mkdir(random_folder_name)
     yuv_file_path = Path(random_folder_name, mm_file_path.stem + '.yuv')
 
     logger.debug(f'Converting {str(mm_file_path.resolve())} to yuv format')
     convert_to_yuv(mm_file_path, yuv_file_path)
 
-    video_width, video_height, _, FPS = get_mm_file_properties(mm_file_path)
+    video_width, video_height, _, fps = get_mm_file_properties(mm_file_path)
 
     logger.debug('Calling VQIs binary file')
 
-    sfs_call_elems = [str(binary_path.resolve()), str(yuv_file_path.resolve()), str(video_width), str(video_height), str(selected_vqis), str(FPS)]
+    sfs_call_elems = [
+        str(binary_path.resolve()),
+        str(yuv_file_path.resolve()),
+        str(video_width), str(video_height),
+        str(selected_vqis),
+        str(fps)
+    ]
     system_call(sfs_call_elems, logger)
 
     logger.debug(f'{sfs_call_elems[0]} binary file was successfully executed')
 
     vqis_csv_path = Path(random_folder_name, mm_file_path.stem + '.csv')
 
     mv_file(Path('./metricsResultsCSV.csv').resolve(), vqis_csv_path.resolve())
 
-    vqis_res_df = pd.read_csv(vqis_csv_path, sep=r'\s+')
+    vqis_res_df = pd.read_csv(vqis_csv_path.resolve(), sep=r'\s+')
 
     logger.debug('Removing working directory')
     rmdir(random_folder_name)
 
     return vqis_res_df
 
 
@@ -182,16 +187,14 @@
         blur_amount = _blur_amount(frame)
         logger.debug(f"Blur Amount IQI for the {frame.frame_no}-th frame: {blur_amount:.5f}")
         blur_amount_s.loc[frame.frame_no] = blur_amount
     return blur_amount_s
 
 
 def _ugc(in_path: Path, results_vqis: pd.DataFrame):
-    _, _, FPS, _ = get_mm_file_properties(in_path)
-
     # Get a list of shots
     scene_list_out = ugc.find_scenes(str(in_path))
 
     if len(scene_list_out) == 0:
         return None
 
     shots_data = ugc.get_shots_data(scene_list_out, results_vqis)
@@ -200,37 +203,36 @@
     return [{
         'range_start': int(item['frames_range'].split(', ')[0]) - 1,
         'range_end': int(item['frames_range'].split(', ')[1]) - 1,
         'ugc': item['ugc']
     } for item in shots_data]
 
 
-def get_ugc_iqi(in_path: Path, nb_frames: int, results_vqis: pd.DataFrame):
+def get_ugc_vqi(in_path: Path, nb_frames: int, results_vqis: pd.DataFrame):
     shots = _ugc(in_path, results_vqis)
 
     if shots is None:
         return None
 
     ugc_s = pd.Series(np.zeros(nb_frames))
     for frame in range(nb_frames):
         for shot in shots:
-            if  shot['range_start'] <= frame <= shot['range_end']:
+            if shot['range_start'] <= frame <= shot['range_end']:
                 ugc_s.loc[frame] = shot['ugc']
                 break
 
     return ugc_s
 
 
-def store_results(results: dict, in_video_path: Path, out_filename_base="agh_vqis_colourfulness_blur_amount"):
+def store_results(results: dict, in_video_path: Path):
     """
     Stores results of image quality indicators (IQIs) calculated on (all) video frames of the input video.
 
     :param results: a dictionary of objects with IQIs results
     :param in_video_path: path to the input video that was processed
-    :param out_filename_base: part of an output CSV filename independent of input video filename
     :return: nothing yet
     """
     assert len(results) != 0
     # Generate a filename that reflects to what input video it belongs to
     out_filename = "_".join(["VQIs", "for", in_video_path.stem]) + ".csv"
     # Handle the case when only one type of IQI was run
     # if len(results) == 1:
@@ -254,71 +256,74 @@
 
     res.columns = res.columns.str.replace(':', '')
     res.to_csv(out_filename, index=False)
     logger.info(f"All results stored in the {out_filename} file")
     return
 
 
-def parse_user_input(cli: bool = False, options: dict = {}):
+def parse_user_input(cli: bool = False):
     """
     Parses user input (as provided through the command line).
 
     :return: nothing yet
     """
+
     parser = argparse.ArgumentParser(description="Computes image quality indicators (IQIs) for the input image or for"
                                                  " each video frame"
                                                  " from an input video. If no specific set of IQIs to compute is"
                                                  " selected, 15 AGH VQIs are run by default.")
     if cli:
         parser.add_argument("path",
                             help="Path to a multimedia file (image or video) to process or path to a folder with "
                                  "multimedia materials"
                                  " (photos or videos) to process", type=Path)
     parser.add_argument("-c", "--colourfulness", help="a flag indicating whether to run the Colourfulness image"
                                                       " quality indicator", action="store_true")
     parser.add_argument("-b", "--blur-amount", help="a flag indicating whether to run the Blur Amount image"
                                                     " quality indicator", action="store_true")
-    parser.add_argument("-u", "--ugc", help="a flag indicating whether to run the ugc video"
-                                                    " quality indicator", action="store_true")
+    parser.add_argument("-u", "--ugc", help="a flag indicating whether to run the User-Generated Content (UGC) video"
+                                            " quality indicator", action="store_true")
     parser.add_argument("-v", "--vqis", help="a flag indicating whether to run the 15 AGH video"
                                              " quality indicators (VQIs). The VQIS argument must be a number"
                                              " specifying which VQIs to run. Each VQI represents a subsequent bit"
                                              " of a 16 bits long positive integer. For example, the Blockiness VQI"
                                              " corresponds to the least significant bit of this integer. The ordering"
                                              " of the rest of VQIs is as follows (values in parentheses identify"
                                              " decimal values that correspond to the one particular bit being set in"
                                              " the 16-bit positive integer): Blockiness (1), SA (2), Letterbox (4),"
                                              " Pillarbox (8), Blockloss (16), Blur (32), TA (64), Blackout (128),"
                                              " Freezing (256), Exposure (512), Contrast (1024), Interlace (2048),"
                                              " Noise (4096), Slice (8192) and Flickering (16384)."
                                              " Please note that you can provide a value for the VQIS parameter"
                                              " in the form of a hexadecimal number."
                                              " For example, 0x7FFF means running all VQIs.")
-    parser.add_argument("-e", "--exec", help="provide here the path to the binary file running 15 AGH VQIs. The "
-                                             "default is to use the agh_vqis_binary_x86_mt binary contained in the "
-                                             "repo.", type=Path)
     args = parser.parse_args()
     # Run 15 AGH VQIs if no VQIs were selected
     if cli and not args.vqis:
         logger.info("No IQIs were selected. Running 15 AGH VQIs only.")
         args.vqis = "0x7FFF"
     return args
 
 
-def process_single_mm_file(in_path: Path, cli: bool = False, options: dict = {}, args=None):
+def process_single_mm_file(in_path: Path, cli: bool = False, options=None, args=None):
     """
     Processes single multimedia file (image or video).
 
+    :param args: user arguments namespace, as returned by argparse (after processing user input)
+    :param cli: boolean indicating if package was run from command line interface or from script, `True` value means it was run from CLI
     :param in_path: path to an input file to process
     :param options: options for executable file
     :return: status, 0 if successful, 1 otherwise
     """
 
+    if options is None:
+        options = {}
+
     if args is None:
-        args = parse_user_input(cli, options)
+        args = parse_user_input(cli)
 
     if not in_path.exists():
         logger.error(f'{str(in_path)} file does not exists')
         return -1
 
     mm_file_ext = in_path.suffix
     if mm_file_ext not in allowed_mm_file_extensions:
@@ -346,107 +351,129 @@
             not cli and VQIs.colourfulness in options and options[VQIs.colourfulness]):
         logger.info(f"Running the Colourfulness IQI on the input ({str(in_path.resolve())})")
         # s --- series
         colourfulness_s = get_colourfulness_iqi(in_path, is_video=is_input_video)
         colourfulness_s.name = "Colourfulness"
         results.update({Results.COLOURFULNESS: colourfulness_s})
 
-    run_UGC = False
+    run_ugc_iqi = False
     if is_input_video and (args.ugc or (not cli and VQIs.ugc not in options) or (
             not cli and VQIs.ugc in options and options[VQIs.ugc])):
-        run_UGC = True
+        run_ugc_iqi = True
         options[VQIs.TA] = True  # UGC indicator requires TA
         options[VQIs.SA] = True  # and SA IQIs
 
+    selected_vqis = None
     if cli and args.vqis:
-        vqis_selected = int(args.vqis, base=0)  # parse optional hexadecimal input
+        selected_vqis = int(args.vqis, base=0)  # parse optional hexadecimal input
 
     if not cli:
-        vqis_selected = get_selected_vqis(options)
+        selected_vqis = get_selected_vqis(options)
 
     vqis_res_df = None
-    # Run the mitsu_single_file.sh script on the input video or image (if requested)
     if not cli or args.vqis:
         logger.info(f"Running requested AGH VQIs on the input ({str(in_path.resolve())})")
-        agh_vqis_path = Path(options['exec']) if ('exec' in options and options['exec']) else args.exec
-        vqis_res_df = _run_agh_viqs(in_path, agh_vqis_path, vqis_selected)
+        vqis_res_df = _run_agh_vqis(in_path, selected_vqis)
         if type(vqis_res_df) is not pd.DataFrame:  # Running the VQIs failed
             return -1
 
         if (len(vqis_res_df) != int(nb_frames)) and is_input_video:
             logger.warning(
                 f"For some reason the number of frames read by ffmpeg-python does not match the number of frames read "
                 f"by binary file. You may want to check whether the results are valid.")
             logger.warning(f"This is the difference in the number of frames as indicated by the two methods: "
                            f"{np.abs(len(vqis_res_df) - int(nb_frames))}")
 
-    if run_UGC:
+    if run_ugc_iqi:
         logger.info(f"Running the UGC IQI on the input ({str(in_path.resolve())})")
-        # s --- series
-        # print(results)
 
-        ugc_s = get_ugc_iqi(in_path, int(nb_frames), vqis_res_df)
+        ugc_s = get_ugc_vqi(in_path, int(nb_frames), vqis_res_df)
         if ugc_s is None:
             logger.error(f"Error when running UGC IQI")
         else:
             ugc_s.name = "UGC"
             results.update({Results.UGC: ugc_s})
 
     if vqis_res_df is not None:
         results.update({Results.VQIS: vqis_res_df})
 
+    # python -m agh_vqis .\cr7.mp4
+
+    # options = options | {CastIQI.blur: DestResolution.p360}
+    # options = options | {CastIQI.interlace: DestResolution.p1080}
+
+    if not cli or True:
+        res_df = results[Results.VQIS]
+
+        for cast_iqi in [CastVQI.blockiness, CastVQI.interlace, CastVQI.blur, CastVQI.noise, CastVQI.contrast, CastVQI.exposure]:
+            if cast_iqi not in options:
+                continue
+
+            cast_iqi_name = cast_iqi.split('_')[-1]
+
+            dst_resolution = options[cast_iqi]
+            if is_model_available(cast_iqi_name, in_mm_file_h, dst_resolution):
+                logger.info(f'Casting {cast_iqi_name} from {in_mm_file_h}p to {dst_resolution}p.')
+                res_df[cast_iqi_name+':'] = cast(res_df[cast_iqi_name+':'], cast_iqi_name, in_mm_file_h, dst_resolution)
+            else:
+                logger.warning(f'Model for casting {cast_iqi_name} from {in_mm_file_h}p to {dst_resolution}p is not '
+                               f'available. Skipping.')
+
+        results.update({Results.VQIS: res_df})
+
     # Store all results in a single CSV file
     store_results(results, in_path)
 
     return 0
 
 
-def process_folder_w_mm_files(folder_path: Path, cli: bool = False, options: dict = {}, args=None):
+def process_folder_w_mm_files(folder_path: Path, cli: bool = False, options=None, args=None):
     """
     Processes a folder with multimedia files.
 
     TODO Consider adding recursive directory search. In other words, allow to recursively process files in all
      subdirectories.
 
+    :param options: options for executable file
+    :param cli: boolean indicating if package was run from command line interface or from script, `True` value means it was run from CLI
     :param folder_path: path to a folder with multimedia files to process
     :param args: user arguments namespace, as returned by argparse (after processing user input)
-    :return: status, 0 if successful, 1 otherwise
+    :return: status, 0 if successful,
+    1 otherwise
     """
     # Iterate over files in the folder one-by-one
+    if options is None:
+        options = {}
     for child in folder_path.iterdir():
         # Ignore subdirectories
         if child.is_dir():
             logger.info(f"Skipping a subdirectory ({str(child)})")
             continue
         # Ignore non-video and non-image files
         # TODO Add here any video or image extensions we want to support
-        if (child.suffix not in allowed_mm_file_extensions):
+        if child.suffix not in allowed_mm_file_extensions:
             logger.info(f"Not a multimedia file ({str(child)}), skipping")
             continue
         # Process a single video file
         # TODO Consider adding functionality of keeping all results in a single CSV file (as done in the legacy BATCH
         #  file)
         mm_file_path = child  # mm = multimedia
         status = process_single_mm_file(mm_file_path, cli, options, args)
     return 0
 
 
 def main():
     # TODO Implement user input processing interface that allows to choose individual VQIs from the 15 AGH VQIs in a
     #  user-friendly manner
-    args = parse_user_input(True, options={})
+    args = parse_user_input(True)
 
     in_path = args.path
     in_path = in_path.absolute()
     if not in_path.exists():
         raise FileNotFoundError(f"The path you specified ({in_path}) does not exist. Exiting.")
-    if args.exec:
-        agh_vqis_path = args.exec
-        assert agh_vqis_path.exists(), f"The binary file with 15 AGH VQIs you specified ({str(agh_vqis_path)}) " \
-                                       f"doesn't seem to exist. Quitting."
 
     if in_path.is_dir():
         logger.info(f"Processing a folder ({str(in_path)}) potentially containing a set of multimedia materials")
         status = process_folder_w_mm_files(in_path, cli=True, options={}, args=args)
     else:
         in_mm_file_path = in_path  # mm = multimedia
         status = process_single_mm_file(in_mm_file_path, cli=True, options={}, args=args)
```

### Comparing `agh_vqis-2.9.0/src/agh_vqis/_logger.py` & `agh_vqis-3.0.1/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.9.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt` & `agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.9.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt` & `agh_vqis-3.0.1/src/agh_vqis/binaries/agh_vqis_binary_x86_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.9.0/src/agh_vqis/utils/ugc.py` & `agh_vqis-3.0.1/src/agh_vqis/utils/ugc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-import sys
-import os
-import subprocess
-import csv
-import shutil
 import logging
 
 import pickle
-import xgboost as xgb
 import pandas as pd
-import numpy as np
 import platform
 from pathlib import Path
 
 # For content-aware scene detection:
 from scenedetect.detectors.content_detector import ContentDetector
 from scenedetect.scene_manager import SceneManager
 # For caching detection metrics and saving/loading to a stats file
@@ -26,15 +19,15 @@
 def find_scenes(video_path, threshold=30.0):
     """
     Detects scenes in the provided video file.
     :param video_path: full path to the analysed video
     :param threshold: threshold used by the pyscenedetect. Default 30.
     :return: List of detected scenes in the video
     """
-    # type: (str) -> List[Tuple[FrameTimecode, FrameTimecode]]
+    # type: # (str) -> List[Tuple[FrameTimecode, FrameTimecode]]
     video_manager = VideoManager([video_path])
     stats_manager = StatsManager()
     # Construct our SceneManager and pass it our StatsManager.
     scene_manager = SceneManager(stats_manager)
 
     # Add ContentDetector algorithm (each detector's constructor
     # takes detector options, e.g. threshold).
@@ -110,75 +103,63 @@
         line_count = 0
 
         # TODO: This part can be optimized!!
         # MITSU_csv = open(MITSU_output_path)
         # csv_reader = csv.reader(MITSU_csv, delimiter=delimiter)
         # for row in csv_reader:
 
-        for i in df.index:
+        for j in df.index:
             if first_frame_number <= line_count <= last_frame_number:
-                # print("test: " + str(int(row[0])) + " SA: " + row[2] + " TA: " + row[7])
-                ta_sum += float(df['TA:'][i])
-                sa_sum += float(df['SA:'][i])
+
+                ta_sum += float(df['TA:'][j])
+                sa_sum += float(df['SA:'][j])
 
             line_count += 1
 
         shot = {
             'shot_number': shot_number,
             'frames_range': "{0}, {1}".format(first_frame_number, last_frame_number),
             'TA': float(ta_sum / shot_frames_number),
             'SA': float(sa_sum / shot_frames_number)
         }
-        #print(shot)
+
         shots_data.append(shot)
         shot_number += 1
 
-        ta_sum = 0
-        sa_sum = 0
-
     return shots_data
 
 
 def video_to_cuts(df, shots_data):
     df = df.astype(float)
 
     df['Frame:'] += 1
 
     data = []
-    cuts = pd.DataFrame()
     for i in shots_data:
         frame = i['frames_range'].replace(" ", "").split(",")
-        data.append(df.iloc[int(frame[0]):int(frame[1]),:].mean())
+        data.append(df.iloc[int(frame[0]):int(frame[1]), :].mean())
 
     cuts = pd.DataFrame(data)
     cuts = cuts[['Blockiness:', 'SA:', 'Blockloss:', 'Blur:', 'TA:',
-                    'Exposure(bri):', 'Contrast:', 'Noise:', 'Slice:', 'Flickering:']]
+                 'Exposure(bri):', 'Contrast:', 'Noise:', 'Slice:', 'Flickering:']]
     cuts.columns = ['Blockiness:', 'SA:', 'Blockloss:', 'Blur:', 'TA:',
                     'Exposure(bri):', 'Contrast:', 'Noise:', 'Slice:', 'Flickering:']
     return cuts, shots_data
 
 
 def ugc(df, shots_data):
-#  input path to files where shots data are in pickle format
-#  returns updated shots_data
     cuts, shots_data = video_to_cuts(df, shots_data)
 
-    # 9k_all_set.json
-    # 12k_all_set.json
-    model_path = Path('/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]), '../models/ugc/', '12k_all_set.json')
-
-    # model_path = Path('./model.bin')
-
-    xgb_cl = pickle.load(open(str(model_path), 'rb'))  # exception thrown
-    # pickle.dump(xgb_cl, open('model.bin', 'wb'))
-    # xgb_cl = xgb.XGBRFClassifier()
-    # xgb_cl.load_model(str(model_path))
-    for count, value in enumerate(shots_data):
+    model_path = Path(
+        '/'.join(
+            __file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]),
+            '../models/ugc/',
+            '12k_all_set.json'
+    )
 
-        X = cuts[count:count+1]
-        preds = xgb_cl.predict(X)
+    xgb_cl = pickle.load(open(str(model_path), 'rb'))
 
-        # print(X)
-        # print(preds[0])
+    for count, value in enumerate(shots_data):
+        preds = xgb_cl.predict(cuts[count:count+1])
 
         value['ugc'] = 0 if int(preds[0]) == 1 else 1
     return shots_data  # 0 => not UGC, 1 => UGC
```

