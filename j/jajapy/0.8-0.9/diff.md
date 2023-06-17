# Comparing `tmp/jajapy-0.8.tar.gz` & `tmp/jajapy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jajapy-0.8.tar", last modified: Fri Oct 21 11:33:56 2022, max compression
+gzip compressed data, was "jajapy-0.9.tar", last modified: Thu Nov 24 13:37:22 2022, max compression
```

## Comparing `jajapy-0.8.tar` & `jajapy-0.9.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     1063 2022-05-31 12:18:29.000000 jajapy-0.8/LICENSE
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2911 2022-10-21 11:33:56.933762 jajapy-0.8/PKG-INFO
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2159 2022-10-11 12:01:57.000000 jajapy-0.8/README.md
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)      238 2022-10-04 13:35:56.000000 jajapy-0.8/jajapy/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/base/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     6781 2022-10-19 16:06:34.000000 jajapy-0.8/jajapy/base/BW.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)    10274 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/base/Model.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     5748 2022-10-19 10:39:46.000000 jajapy-0.8/jajapy/base/Set.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       39 2022-09-16 11:06:39.000000 jajapy-0.8/jajapy/base/__init__.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2979 2022-10-19 12:53:36.000000 jajapy-0.8/jajapy/base/tools.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/ctmc/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     9433 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/ctmc/BW_CTMC.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)    11866 2022-09-15 10:41:00.000000 jajapy-0.8/jajapy/ctmc/CTMC.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)    10503 2022-10-04 14:05:51.000000 jajapy-0.8/jajapy/ctmc/MM_CTMC_Composition.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       77 2022-05-31 12:18:29.000000 jajapy-0.8/jajapy/ctmc/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/gohmm/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     4325 2022-10-21 11:29:58.000000 jajapy-0.8/jajapy/gohmm/BW_GOHMM.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     7337 2022-09-13 11:18:43.000000 jajapy-0.8/jajapy/gohmm/GOHMM.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       44 2022-05-31 12:18:29.000000 jajapy-0.8/jajapy/gohmm/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/hmm/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     4640 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/hmm/BW_HMM.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     7796 2022-09-15 13:20:25.000000 jajapy-0.8/jajapy/hmm/HMM.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       40 2022-05-31 12:18:29.000000 jajapy-0.8/jajapy/hmm/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/mc/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     7079 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/mc/Alergia.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     4441 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/mc/BW_MC.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     6303 2022-09-16 10:36:23.000000 jajapy-0.8/jajapy/mc/MC.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       61 2022-05-31 12:18:29.000000 jajapy-0.8/jajapy/mc/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/mdp/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)    10306 2022-10-19 10:46:34.000000 jajapy-0.8/jajapy/mdp/Active_BW_MDP.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     7844 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/mdp/BW_MDP.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)    12519 2022-10-18 10:57:27.000000 jajapy-0.8/jajapy/mdp/IOAlergia.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)    19183 2022-09-30 17:34:54.000000 jajapy-0.8/jajapy/mdp/MDP.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     5000 2022-05-31 12:18:29.000000 jajapy-0.8/jajapy/mdp/Scheduler.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)      119 2022-05-31 12:18:29.000000 jajapy-0.8/jajapy/mdp/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/mgohmm/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     4798 2022-10-11 14:31:08.000000 jajapy-0.8/jajapy/mgohmm/BW_MGOHMM.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     8998 2022-09-13 11:18:43.000000 jajapy-0.8/jajapy/mgohmm/MGOHMM.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       46 2022-05-31 14:57:44.000000 jajapy-0.8/jajapy/mgohmm/__init__.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/tests/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     5896 2022-10-04 13:59:54.000000 jajapy-0.8/jajapy/tests/CTMC_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2052 2022-09-13 11:18:43.000000 jajapy-0.8/jajapy/tests/GOHMM_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2494 2022-10-04 13:59:43.000000 jajapy-0.8/jajapy/tests/HMM_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2661 2022-10-04 13:58:31.000000 jajapy-0.8/jajapy/tests/MC_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     3480 2022-10-17 15:48:56.000000 jajapy-0.8/jajapy/tests/MDP_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2246 2022-09-13 11:18:44.000000 jajapy-0.8/jajapy/tests/MGOHMM_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)        0 2022-06-05 18:01:49.000000 jajapy-0.8/jajapy/tests/__init__.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     5041 2022-10-17 15:22:39.000000 jajapy-0.8/jajapy/tests/model_converter_test.py
--rw-rw-r--   0 raphael   (1002) raphael   (1002)      767 2022-06-07 15:37:59.000000 jajapy-0.8/jajapy/tests/tools_test.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy/with_stormpy/
--rw-r--r--   0 raphael   (1002) raphael   (1002)       30 2022-09-15 13:20:25.000000 jajapy-0.8/jajapy/with_stormpy/__init__.py
--rw-r--r--   0 raphael   (1002) raphael   (1002)     9752 2022-10-17 15:15:08.000000 jajapy-0.8/jajapy/with_stormpy/model_converter.py
-drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-10-21 11:33:56.933762 jajapy-0.8/jajapy.egg-info/
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     2911 2022-10-21 11:33:56.000000 jajapy-0.8/jajapy.egg-info/PKG-INFO
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     1141 2022-10-21 11:33:56.000000 jajapy-0.8/jajapy.egg-info/SOURCES.txt
--rw-rw-r--   0 raphael   (1002) raphael   (1002)        1 2022-10-21 11:33:56.000000 jajapy-0.8/jajapy.egg-info/dependency_links.txt
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       27 2022-10-21 11:33:56.000000 jajapy-0.8/jajapy.egg-info/requires.txt
--rw-rw-r--   0 raphael   (1002) raphael   (1002)        7 2022-10-21 11:33:56.000000 jajapy-0.8/jajapy.egg-info/top_level.txt
--rw-rw-r--   0 raphael   (1002) raphael   (1002)       38 2022-10-21 11:33:56.933762 jajapy-0.8/setup.cfg
--rw-rw-r--   0 raphael   (1002) raphael   (1002)     1143 2022-10-21 11:32:54.000000 jajapy-0.8/setup.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     1063 2022-10-26 09:52:53.000000 jajapy-0.9/LICENSE
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     3013 2022-11-24 13:37:22.054676 jajapy-0.9/PKG-INFO
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     2261 2022-11-15 09:30:40.000000 jajapy-0.9/README.md
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.050676 jajapy-0.9/jajapy/
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)      238 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.050676 jajapy-0.9/jajapy/base/
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     6788 2022-11-16 14:12:50.000000 jajapy-0.9/jajapy/base/BW.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)    10635 2022-11-15 11:12:09.000000 jajapy-0.9/jajapy/base/Model.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     5559 2022-11-15 11:15:50.000000 jajapy-0.9/jajapy/base/Set.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)       39 2022-10-26 09:52:53.000000 jajapy-0.9/jajapy/base/__init__.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     2903 2022-11-10 10:46:15.000000 jajapy-0.9/jajapy/base/tools.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.050676 jajapy-0.9/jajapy/ctmc/
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     9277 2022-11-22 12:12:33.000000 jajapy-0.9/jajapy/ctmc/BW_CTMC.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)    12882 2022-11-24 09:54:05.000000 jajapy-0.9/jajapy/ctmc/CTMC.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)       42 2022-11-15 09:25:30.000000 jajapy-0.9/jajapy/ctmc/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/gohmm/
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     4325 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/gohmm/BW_GOHMM.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     7337 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/gohmm/GOHMM.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)       44 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/gohmm/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/hmm/
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     4695 2022-10-28 15:42:22.000000 jajapy-0.9/jajapy/hmm/BW_HMM.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     7796 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/hmm/HMM.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)       40 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/hmm/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/mc/
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     7447 2022-11-22 10:26:23.000000 jajapy-0.9/jajapy/mc/Alergia.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     4192 2022-11-23 10:14:27.000000 jajapy-0.9/jajapy/mc/BW_MC.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     9402 2022-11-24 09:50:41.000000 jajapy-0.9/jajapy/mc/MC.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)       61 2022-10-26 09:52:53.000000 jajapy-0.9/jajapy/mc/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/mdp/
+-rw-r--r--   0 raphael   (1002) raphael   (1002)    10299 2022-11-24 09:58:18.000000 jajapy-0.9/jajapy/mdp/Active_BW_MDP.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     7508 2022-11-24 10:15:48.000000 jajapy-0.9/jajapy/mdp/BW_MDP.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)    12651 2022-11-23 10:36:18.000000 jajapy-0.9/jajapy/mdp/IOAlergia.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)    17514 2022-11-24 10:14:55.000000 jajapy-0.9/jajapy/mdp/MDP.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     5000 2022-10-26 09:52:53.000000 jajapy-0.9/jajapy/mdp/Scheduler.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)      119 2022-10-26 09:52:53.000000 jajapy-0.9/jajapy/mdp/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/mgohmm/
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     4853 2022-11-07 11:07:20.000000 jajapy-0.9/jajapy/mgohmm/BW_MGOHMM.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     8950 2022-11-17 15:04:39.000000 jajapy-0.9/jajapy/mgohmm/MGOHMM.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)       46 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/mgohmm/__init__.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/tests/
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     4219 2022-11-23 10:57:37.000000 jajapy-0.9/jajapy/tests/CTMC_test.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     2052 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/tests/GOHMM_test.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     2494 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/tests/HMM_test.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     3973 2022-11-23 09:55:11.000000 jajapy-0.9/jajapy/tests/MC_test.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     4310 2022-11-22 13:35:26.000000 jajapy-0.9/jajapy/tests/MDP_test.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     2246 2022-10-28 15:14:43.000000 jajapy-0.9/jajapy/tests/MGOHMM_test.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)        0 2022-10-26 09:52:53.000000 jajapy-0.9/jajapy/tests/__init__.py
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     2454 2022-11-23 15:25:02.000000 jajapy-0.9/jajapy/tests/model_converter_test.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)      773 2022-11-24 13:30:49.000000 jajapy-0.9/jajapy/tests/tools_test.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.054676 jajapy-0.9/jajapy/with_stormpy/
+-rw-r--r--   0 raphael   (1002) raphael   (1002)       30 2022-10-26 09:52:53.000000 jajapy-0.9/jajapy/with_stormpy/__init__.py
+-rw-r--r--   0 raphael   (1002) raphael   (1002)     4746 2022-11-23 13:57:55.000000 jajapy-0.9/jajapy/with_stormpy/model_converter.py
+drwxrwxr-x   0 raphael   (1002) raphael   (1002)        0 2022-11-24 13:37:22.050676 jajapy-0.9/jajapy.egg-info/
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     3013 2022-11-24 13:37:22.000000 jajapy-0.9/jajapy.egg-info/PKG-INFO
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     1106 2022-11-24 13:37:22.000000 jajapy-0.9/jajapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)        1 2022-11-24 13:37:22.000000 jajapy-0.9/jajapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)       27 2022-11-24 13:37:22.000000 jajapy-0.9/jajapy.egg-info/requires.txt
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)        7 2022-11-24 13:37:22.000000 jajapy-0.9/jajapy.egg-info/top_level.txt
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)       38 2022-11-24 13:37:22.054676 jajapy-0.9/setup.cfg
+-rw-rw-r--   0 raphael   (1002) raphael   (1002)     1143 2022-11-24 13:37:16.000000 jajapy-0.9/setup.py
```

### Comparing `jajapy-0.8/LICENSE` & `jajapy-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/PKG-INFO` & `jajapy-0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jajapy
-Version: 0.8
+Version: 0.9
 Summary: Baum-Welch for all kind of Markov model
 Home-page: UNKNOWN
 Author: Raphaël Reynouard
 Author-email: raphal20@ru.is
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -44,27 +44,28 @@
 <div align="center">
 	
 | Markov Model   |      Learning Algorithm(s) |
 |-------|:-------------:|
 | HMM    | Baum-Welch for HMMs  ([ref](https://web.ece.ucsb.edu/Faculty/Rabiner/ece259/Reprints/tutorial%20on%20hmm%20and%20applications.pdf)) |
 | MC     | Baum-Welch for MCs <br /> Alergia ([ref](https://www.researchgate.net/publication/2543721_Learning_Stochastic_Regular_Grammars_by_Means_of_a_State_Merging_Method/stats)) |
 | MDP    | Baum-Welch for MDPs ([ref](https://arxiv.org/abs/2110.03014))<br /> Active Baum-Welch ([ref](https://arxiv.org/abs/2110.03014))<br /> IOAlergia ([ref](https://link.springer.com/content/pdf/10.1007/s10994-016-5565-9.pdf))|
-| CTMC   | Baum-Welch for CTMCs<br /> MM for asynchronous composition of CTMCs|
+| CTMC   | Baum-Welch for CTMCs|
 | GoHMM  | Baum-Welch for GoHMMs ([ref](http://www.inass.org/2020/2020022920.pdf)) |
 | MGoHMM | Baum-Welch for MGoHMMs |
 
 </div>
 
 `jajapy` generates by default Stormpy models (except for GoHMM and MGoHMM).
 
 ## Installation
 ``pip install jajapy``
 
 ## Requirements
-- numpy
-- scipy
-- stormpy (recommended: if stormpy is not installed, `jajapy` will generate models in jajapy format).
+- [numpy](https://numpy.org/)
+- [scipy](https://scipy.org/)
+- [alive-progress](https://github.com/rsalmei/alive-progress) 
+- [stormpy](https://github.com/moves-rwth/stormpy) (recommended: if stormpy is not installed, `jajapy` will generate models in jajapy format).
 
 ## Documentation
 Available on [readthedoc](https://jajapy.readthedocs.io/en/latest/?)
```

### Comparing `jajapy-0.8/README.md` & `jajapy-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,25 +22,26 @@
 <div align="center">
 	
 | Markov Model   |      Learning Algorithm(s) |
 |-------|:-------------:|
 | HMM    | Baum-Welch for HMMs  ([ref](https://web.ece.ucsb.edu/Faculty/Rabiner/ece259/Reprints/tutorial%20on%20hmm%20and%20applications.pdf)) |
 | MC     | Baum-Welch for MCs <br /> Alergia ([ref](https://www.researchgate.net/publication/2543721_Learning_Stochastic_Regular_Grammars_by_Means_of_a_State_Merging_Method/stats)) |
 | MDP    | Baum-Welch for MDPs ([ref](https://arxiv.org/abs/2110.03014))<br /> Active Baum-Welch ([ref](https://arxiv.org/abs/2110.03014))<br /> IOAlergia ([ref](https://link.springer.com/content/pdf/10.1007/s10994-016-5565-9.pdf))|
-| CTMC   | Baum-Welch for CTMCs<br /> MM for asynchronous composition of CTMCs|
+| CTMC   | Baum-Welch for CTMCs|
 | GoHMM  | Baum-Welch for GoHMMs ([ref](http://www.inass.org/2020/2020022920.pdf)) |
 | MGoHMM | Baum-Welch for MGoHMMs |
 
 </div>
 
 `jajapy` generates by default Stormpy models (except for GoHMM and MGoHMM).
 
 ## Installation
 ``pip install jajapy``
 
 ## Requirements
-- numpy
-- scipy
-- stormpy (recommended: if stormpy is not installed, `jajapy` will generate models in jajapy format).
+- [numpy](https://numpy.org/)
+- [scipy](https://scipy.org/)
+- [alive-progress](https://github.com/rsalmei/alive-progress) 
+- [stormpy](https://github.com/moves-rwth/stormpy) (recommended: if stormpy is not installed, `jajapy` will generate models in jajapy format).
 
 ## Documentation
 Available on [readthedoc](https://jajapy.readthedocs.io/en/latest/?)
```

### Comparing `jajapy-0.8/jajapy/base/BW.py` & `jajapy-0.9/jajapy/base/BW.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 			loglikelihood of the training set under the two last hypothesis is
 			lower than ``epsilon``. The lower this value the better the output,
 			but the longer the running time.
 		max_it: int
 			Maximal number of iterations. The algorithm will stop after `max_it`
 			iterations.
 			Default is infinity.
-		pp : str
+		pp:	str
 			Will be printed at each iteration.
 		verbose: bool
 			Print or not a small recap at the end of the learning.
 		return_data: bool
 			If set to True, a dictionary containing following values will be
 			returned alongside the hypothesis once the learning is done.
 			'learning_rounds', 'learning_time', 'training_set_loglikelihood'.
@@ -164,30 +164,30 @@
 
 		Returns
 		-------
 		Model
 			fitted model.
 		"""
 		try:
-			from ..with_stormpy import jajapyModeltoStorm, stormModeltoJajapy
+			from ..with_stormpy import jajapyModeltoStormpy, stormpyModeltoJajapy
 			stormpy_installed = True
 		except ModuleNotFoundError:
 			stormpy_installed = False
 		
 		if stormpy_output and not stormpy_installed:
 			print("WARNING: stormpy not found. The output model will not be a stormpy sparse model")
 			stormpy_output = False
 		
 		try:
 			initial_model.name
 		except AttributeError: # then initial_model is a stormpy sparse model
 			if not stormpy_installed:
 				print("ERROR: the initial model is a Storm model and Storm is not installed on the machine")
 				return False
-			initial_model = stormModeltoJajapy(initial_model)		
+			initial_model = stormpyModeltoJajapy(initial_model)		
 
 		start_time = datetime.now()
 		self.h = initial_model
 		self.nb_states = self.h.nb_states
 
 		counter = 0
 		prevloglikelihood = 10
@@ -218,14 +218,14 @@
 		if output_file:
 			self.h.save(output_file)
 		
 		if verbose:
 			self._endPrint(counter,running_time)
 
 		if stormpy_output:
-			self.h = jajapyModeltoStorm(self.h)
+			self.h = jajapyModeltoStormpy(self.h)
 
 		if return_data:
 			info = {"learning_rounds":counter,"learning_time":running_time,"training_set_loglikelihood":currentloglikelihood}
 			return self.h, info
 			
 		return self.h
```

### Comparing `jajapy-0.8/jajapy/base/Model.py` & `jajapy-0.9/jajapy/base/Model.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,17 @@
 		self.nb_states = len(matrix)
 		# initial_state can be a list of probability or an int
 		if type(initial_state) == int:
 			self.initial_state = array([0.0 for i in range(self.nb_states)])
 			self.initial_state[initial_state] = 1.0
 		else:
 			if round(sum(initial_state)) != 1.0:
-				print("Error: the sum of initial_state should be 1.0, here it's",sum(initial_state))
-				return False
+				msg = "Error: the sum of initial_state should be 1.0, here it's"
+				msg+= str(sum(initial_state))
+				raise ValueError(msg)
 			self.initial_state = array(initial_state)
 		self.matrix = matrix
 		self.name = name
 	
 	def rename(self,name: str) -> None:
 		"""
 		Change the name of the model.
@@ -120,14 +121,15 @@
 		if current == -1:
 			current = resolveRandom(self.initial_state)
 
 		while len(output) < number_steps:
 			[next_state, symbol] = self.next(current)
 			output.append(symbol)
 			current = next_state
+		
 		return output
 	
 	def generateSet(self, set_size: int, param, distribution=None, min_size=None, timed: bool=False) -> Set:
 		"""
 		Generates a set (training set / test set) containing ``set_size`` traces.
 
 		Parameters
@@ -219,15 +221,15 @@
 			loglikelihood of ``sequences`` under this model.
 		
 		Examples
 		--------
 		>>> model.logLikelihood(set1)
 		-4.442498878506513
 		"""
-		if platform != "win32":
+		if platform != "win32" and platform != "darwin":
 			return self._logLikelihood_multiproc(sequences)
 		else:
 			return self._logLikelihood_oneproc(sequences)
 
 	def _updateAlphaMatrix(self,sequence: list,
 						   common: int,
 						   alpha_matrix: list) -> array:
@@ -358,8 +360,16 @@
 			new_arr = zeros(self.nb_states)
 			for s in range(self.nb_states):
 				p = array([self.tau(ss,s,sequence[k]) for ss in range(self.nb_states)])
 				new_arr[s] = dot(prev_arr,p)
 			prev_arr = new_arr
 		if prev_arr.sum() == 0.0:
 			return 0.0
-		return log(prev_arr.sum())*times
+		return log(prev_arr.sum())*times
+	
+	def _checkStateIndex(self,s:int) -> None:
+		if type(s) != int:
+			raise TypeError('The parameter must be a valid state ID')
+		elif s < 0:
+			raise IndexError('The parameter must be a valid state ID')
+		elif s >= self.nb_states:
+			raise IndexError('This model contains only '+str(self.nb_states)+' states')
```

### Comparing `jajapy-0.8/jajapy/base/Set.py` & `jajapy-0.9/jajapy/base/Set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ast import literal_eval
 from numpy import float64, array, append
 class Set:
 	"""
 	Class representing a set (training set / test set).
 	"""
-	def __init__(self, sequences:list, times:list = None, from_MDP: bool=False, t: int = None) -> None:
+	def __init__(self, sequences:list, times:list = None, t: int = None) -> None:
 		"""
 		Creates the Set.
 
 		Parameters
 		----------
 		sequences : list
 			List of sequences of traces.
@@ -17,17 +17,14 @@
 			- an alternating sequence of actions/observations (list of str) ->MDP
 			- a sequence of timed observations (list of float) ->GOHMM
 			- a sequence of vectors of timed observations (list of list of float) ->MGOHMM
 			- an alternating sequence of waiting-times/observations (list of float and str) ->CTMC
 		times : list, optional
 			`times[i]` is the number of time `sequences[i]` appears in the set.
 			Can be omitted.
-		from_MDP : bool, optional
-			Whether or not the set has been generated by an MDP.
-			Default is False.
 		t : int, optional
 			0 if this set was generated by a HMM or a MC,
 			1 if it was generated by a MDP,
 			2 if it was generated by a GOHMM,
 			3 if it was generated by a MGOHMM,
 			4 if it was generated by a CTMC.
 		"""
@@ -36,24 +33,21 @@
 			self.times = []
 			self.type = t
 			return
 		if t != None:
 			self.type = t
 		else:
 			if type(sequences[0][0])  == float64 or type(sequences[0][0])  == float:
-				if type(sequences[0][1]) == float64 or type(sequences[0][1])  == float:
-					self.type = 2 # GOHMM
-				else:
-					self.type = 4 # CTMC
-			elif from_MDP:
-				self.type = 1 # MDP
+				self.type = 2 # GOHMM
+			elif type(sequences[0][1])  == float64 or type(sequences[0][1])  == float:
+				self.type = 4 # timed CTMC
 			elif type(sequences[0][0])  == list:
 				self.type = 3 # MGOHMM
 			else:
-				self.type = 0 # HMM or MC
+				self.type = 0 # HMM or MC or non-timed CTMC
 
 		if type(times) == type(None):
 			self.setFromList(sequences)
 		else:
 			self.sequences = sequences
 			self.times = array(times)
 	
@@ -63,15 +57,15 @@
 		
 		Parameters
 		----------
 		file_path: str
 			where to save
 		"""
 		f = open(file_path,'w')
-		f.write(str(self.type == 1)+'\n')
+		f.write(str(self.type)+'\n')
 		for i in range(len(self.sequences)):
 			f.write(str(self.sequences[i])+'\n')
 			f.write(str(self.times[i])+'\n')
 		f.close()
 
 	def setFromList(self, l: list) -> None:
 		"""
@@ -156,25 +150,23 @@
 		Returns all possible observations and all possible actions in this set.
 
 		Returns
 		-------
 		list
 			list of one list of actions and one list of observations.
 		"""
+		if self.type != 1:
+			return self.getAlphabet()
 		actions = []
 		observations = []
 		for seq in range(len(self.sequences)):
-			sequence_actions = [self.sequences[seq][i] for i in range(0,len(self.sequences[seq]),2)]
-			sequence_obs = [self.sequences[seq][i+1] for i in range(0,len(self.sequences[seq]),2)]
-			for x in sequence_actions:
-				if x not in actions:
-					actions.append(x)
-			for x in sequence_obs:
-				if x not in observations:
-					observations.append(x)
+			actions += [self.sequences[seq][i+1] for i in range(0,len(self.sequences[seq])-1,2)]
+			observations += [self.sequences[seq][i] for i in range(0,len(self.sequences[seq])-1,2)] + [self.sequences[seq][-1]]
+		actions = list(set(actions))
+		observations = list(set(observations))
 		return [actions,observations]
 	
 	def addSet(self, s2):
 		"""
 		Merges this set with another generated by the same kind of Markov model.
 
 		Parameters
@@ -210,16 +202,16 @@
 	-------
 	Set
 		a training/test set.
 	"""
 	res_set = [[],[]]
 	f = open(file_path,'r')
 	l = f.readline()
-	from_MDP = literal_eval(l[:-1])
+	t = literal_eval(l[:-1])
 	l = f.readline()
 	while l:
 		res_set[0].append(literal_eval(l[:-1]))
 		l = f.readline()
 		res_set[1].append(int(l[:-1]))
 		l = f.readline()
 	f.close()
-	return Set(res_set[0],res_set[1],from_MDP)
+	return Set(res_set[0],res_set[1],t)
```

### Comparing `jajapy-0.8/jajapy/base/tools.py` & `jajapy-0.9/jajapy/base/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from random import random
 from scipy.stats import norm
-from numpy import nditer, array, ndarray, where, nonzero
+from numpy import nditer, array, ndarray, nonzero
+from numpy.random import randint
 
 
 def normpdf(x: float, params: list, variation:float = 0.01) -> float:
 	"""
 	Returns the probability of ``x`` under a normal distribution returns of 
 	parameters ``params``. Since this probability should be 0 it returns in
 	fact the probability that the normal distribution gives us a value
@@ -109,21 +110,15 @@
 	>>> print(p)
 	[0.3155861636575178, 0.11453783121165262, 0.5686125794652406, 0.001263425665589013]
 	"""
 	if size <= 0:
 		raise ValueError("The size parameter should be higher than 0.")
 	if type(size) != int:
 		raise TypeError("The size parameter should be an int.")
-	rand = []
-	for i in range(size-1):
-		rand.append(random())
-	rand.sort()
-	rand.insert(0,0.0)
-	rand.append(1.0)
-	return [rand[i]-rand[i-1] for i in range(1,len(rand))]
+	return normalize(randint(1,11,size))
 
 def checkProbabilities(l: ndarray) -> bool:
 	"""
 	Check if a ndarray contains probabilities i.e. check if the sum of the
 	ndarray is 0.0 or 1.0. 
 
 	Parameters
@@ -132,8 +127,8 @@
 		List of probabilities
 
 	Returns
 	-------
 	bool
 		True if the sum of the list is 0.0 or 1.0.
 	"""
-	return round(l.sum(),3) == 1.0
+	return round(l.sum(),3) == 1.0 or round(l.sum(),3) == 0.0
```

### Comparing `jajapy-0.8/jajapy/ctmc/BW_CTMC.py` & `jajapy-0.9/jajapy/ctmc/BW_CTMC.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,22 +68,23 @@
 			Sequence of waiting times.
 
 		Returns
 		-------
 		2-D narray
 			array containing the beta values.
 		"""
-		len_seq = len(obs_seq)
+		len_seq = len(obs_seq)-1
 		init_arr = self.h.initial_state
 		zero_arr = zeros(shape=(len_seq*self.nb_states,))
 		alpha_matrix = append(init_arr,zero_arr).reshape(len_seq+1,self.nb_states)
 		for k in range(len_seq):
 			for s in range(self.nb_states):
 				p = array([self.h_l(ss,s,obs_seq[k])*exp(-self.h_e(ss)*times_seq[k]) for ss in range(self.nb_states)])
 				alpha_matrix[k+1,s] = dot(alpha_matrix[k],p)
+		alpha_matrix[-1] *= (array(self.h.labeling) == obs_seq[-1])
 		return alpha_matrix.T
 
 	def computeBetas_timed(self,obs_seq: list, times_seq: list) -> array:
 		"""
 		Compute the beta values for ``obs_seq`` and ``times_seq`` under the
 		current BW hypothesis.
 
@@ -95,19 +96,19 @@
 			Sequence of waiting times.
 
 		Returns
 		-------
 		2-D narray
 			array containing the beta values.
 		"""
-		len_seq = len(obs_seq)
-		init_arr = ones(self.nb_states)
+		len_seq = len(obs_seq)-1
+		init_arr = ones(self.nb_states)*(array(self.h.labeling) == obs_seq[-1])
 		zero_arr = zeros(shape=(len_seq*self.nb_states,))
 		beta_matrix = append(zero_arr,init_arr).reshape(len_seq+1,self.nb_states)
-		for k in range(len(obs_seq)-1,-1,-1):
+		for k in range(len_seq-1,-1,-1):
 			for s in range(self.nb_states):
 				p = array([self.h_l(s,ss,obs_seq[k]) for ss in range(self.nb_states)])
 				p = p * exp(-self.h_e(s)*times_seq[k])
 				beta_matrix[k,s] = dot(beta_matrix[k+1],p)
 		return beta_matrix.T
 
 	def computeAlphas_nontimed(self,sequence: list) -> array:
@@ -208,24 +209,35 @@
 		-------
 		CTMC or stormpy.SparseCtmc
 			The fitted CTMC.
 			If `stormpy_output` is set to `False` or if stormpy is not available on
 			the machine it returns a `jajapy.CTMC`, otherwise it returns a `stormpy.SparseCtmc`
 		"""
 		if type(traces) != Set:
-			traces = Set(traces, t=4)
+			traces = Set(traces)
+		
+		alphabet = traces.getAlphabet()
+		if not 'init' in alphabet:
+			if nb_states != None:
+				nb_states += 1
+			alphabet.append('init')
+			timed = type(traces.sequences[0][1]) != str
+			for s in range(len(traces.sequences)):
+				if timed:
+					traces.sequences[s].insert(0,0.5)
+				traces.sequences[s].insert(0,'init')
+		
 		if not initial_model:
 			if not nb_states:
-				print("Either nb_states or initial_model should be set")
-				return
+				raise ValueError("Either nb_states or initial_model should be set")
+
 			initial_model = CTMC_random(nb_states,
-										traces.getAlphabet(),
+										alphabet,
 										min_exit_rate_time, max_exit_rate_time,
 										self_loop, random_initial_state)
-		self.alphabet = initial_model.getAlphabet()
 		return super().fit(traces, initial_model, output_file, epsilon, max_it, pp, verbose,return_data,stormpy_output)
 
 
 	def splitTime(self,sequence: list) -> tuple:
 		"""
 		Given a trace it returns a sequence of observation and a sequence of
 		waiting times. If the given trace is non-timed the output waiting time
@@ -237,69 +249,59 @@
 			_description_
 
 		Returns
 		-------
 		tuple
 			_description_
 		"""
-		if type(sequence[0]) == float and type(sequence[1]) == str:
-			times_seq = [sequence[i] for i in range(0,len(sequence),2)]
-			obs_seq   = [sequence[i] for i in range(1,len(sequence),2)]
+		if type(sequence[1]) == float and type(sequence[0]) == str:
+			times_seq = [sequence[i] for i in range(1,len(sequence),2)]
+			obs_seq   = [sequence[i] for i in range(0,len(sequence),2)]
 		else:
 			times_seq = None
 			obs_seq = sequence
 		return (times_seq,obs_seq)
 
 	def _processWork(self,sequence: list, times: int):
 		times_seq, obs_seq = self.splitTime(sequence)
 		if times_seq == None:
 			timed = False
 		else:
 			timed = True
-
 		alpha_matrix = self.computeAlphas(obs_seq, times_seq)
 		beta_matrix  = self.computeBetas( obs_seq, times_seq)
 		proba_seq = alpha_matrix.T[-1].sum()
 		if proba_seq == 0.0:
 			return False
-		####################	
+		####################
+		if timed:
+			den = (alpha_matrix[:,:-1]*beta_matrix[:,:-1]*times_seq*times/proba_seq).sum(axis=1)	
+		else:
+			den = (alpha_matrix[:,:-1]*beta_matrix[:,:-1]*times/proba_seq).sum(axis=1)
+
+		num = zeros(shape=(self.nb_states,self.nb_states))	
 		for s in range(self.nb_states):
-			den = zeros(self.nb_states)
-			#num = zeros(shape=(self.nb_states,self.nb_states*len(self.alphabet)))
-			num = zeros(shape=(self.nb_states,self.nb_states,len(self.alphabet)))
-
-			if timed:
-				den[s] = dot(alpha_matrix[s][:-1]*beta_matrix[s][:-1]*times_seq,times/proba_seq).sum()
-			else:
-				den[s] = dot(alpha_matrix[s][:-1]*beta_matrix[s][:-1],times/proba_seq).sum()
 			for ss in range(self.nb_states):
 				if timed:
 					p = array([self.h_l(s,ss,o)*exp(-self.h_e(s)*t) for o,t in zip(obs_seq,times_seq)])
 				else:
 					p = array([self.h_l(s,ss,o) for o in obs_seq])
-				alph_bet = alpha_matrix[s][:-1]*p*beta_matrix[ss][1:]*times/proba_seq
-				for o,obs in enumerate(self.alphabet):
-					arr_dirak = [1.0 if o == obs else 0.0 for o in obs_seq]
-					num[s,ss,o] = (alph_bet*arr_dirak).sum()
-		####################			
-		num_init = alpha_matrix.T[0]*beta_matrix.T[0]*times/proba_seq
+				num[s,ss] = dot(alpha_matrix[s][:-1]*p*beta_matrix[ss][1:],times/proba_seq).sum()
 		####################
-		return [den, num, proba_seq, times, num_init]
+		return [den, num, proba_seq, times]
 
 	def _generateHhat(self,temp):
 		den = array([i[0] for i in temp]).sum(axis=0)
 		num = array([i[1] for i in temp]).sum(axis=0)
 		lst_proba=array([i[2] for i in temp])
 		lst_times=array([i[3] for i in temp])
-		lst_init =array([i[4] for i in temp]).T
 
 		currentloglikelihood = dot(log(lst_proba),lst_times)
 
 		for s in range(len(den)):
 			if den[s] == 0.0:
 				den[s] = 1.0
 				num[s] = self.h.matrix[s]
 
-		matrix = num/den[:, newaxis, newaxis]
-		initial_state = [lst_init[s].sum()/lst_init.sum() for s in range(self.nb_states)]
-		return [CTMC(matrix,self.alphabet,initial_state),currentloglikelihood]
+		matrix = num/den[:, newaxis]
+		return [CTMC(matrix,self.h.labeling),currentloglikelihood]
```

### Comparing `jajapy-0.8/jajapy/ctmc/CTMC.py` & `jajapy-0.9/jajapy/ctmc/CTMC.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,82 @@
 from numpy.random import exponential
 from ast import literal_eval
-from ..base.tools import resolveRandom, normalize, randomProbabilities
+from ..base.tools import resolveRandom, randomProbabilities
 from ..base.Set import Set
 from ..mc.MC import MC
 from ..base.Model import Model
 from math import exp, log
 from random import randint
-from numpy import array, zeros, dot, ndarray, where, reshape
+from numpy import array, zeros, dot, ndarray, vstack, hstack, newaxis, append
 from sys import platform
 from multiprocessing import cpu_count, Pool
+from random import choices
 
 class CTMC(Model):
 	"""
 	Class representing a CTMC.
 	"""
-	def __init__(self, matrix: ndarray, alphabet: list, initial_state, name: str ="unknown_MC") -> None:
+	def __init__(self, matrix: ndarray, labeling: list, name: str ="unknown_CTMC") -> None:
 		"""
 		Creates an CTMC.
 
 		Parameters
 		----------
 		matrix : ndarray
+			A (N x N) ndarray (with N the nb of states).
 			Represents the transition matrix.
-			`matrix[s1][s2][obs_ID]` is the rate associated to the transition 
-			from `s1` to `s2` seeing the observation of ID `obs_ID`.
-		alphabet: list
-			The list of all possible observations, such that:
-			`alphabet.index("obs")` is the ID of `obs`.
+			`matrix[s1][s2]` is the rate associated to the transition 
+			from `s1` to `s2`.
+		labeling: list of str
+			A list of N observations (with N the nb of states).
+			If `labeling[s] == o` then state of ID `s` is labelled by `o`.
+			Each state has exactly one label.
 		initial_state : int or list of float
 			Determine which state is the initial one (then it's the id of the
 			state), or what are the probability to start in each state (then it's
 			a list of probabilities).
 		name : str, optional
 			Name of the model.
 			Default is "unknow_CTMC"
 		"""
-		self.alphabet = alphabet
+		self.alphabet = list(set(labeling))
+		self.labeling = labeling
+
+		if not 'init' in self.labeling:
+			msg = "No initial state given: at least one"
+			msg += " state should be labelled by 'init'."
+			raise ValueError(msg)
+		initial_state = [1.0/self.labeling.count("init") if i=='init' else 0.0 for i in self.labeling]
+
 		super().__init__(matrix,initial_state,name)
+		if len(labeling) != self.nb_states:
+			raise ValueError("The length of labeling is not equal to the number of states")
+		for s in range(self.nb_states):
+			if self.e(s) == 0.0:
+				raise ValueError("State "+str(s)+" doesn't have any leaving transition.")
 
 	def e(self,s: int) -> float:
 		"""
 		Returns the exit rate of state ``s``, i.e. the sum of all the rates in
 		this state.
 
 		Returns
 		-------
 		s : int
 			A state ID.
 		float
 			An exit rate.
 		"""
-		return sum(self.matrix[s].flatten())
+		self._checkStateIndex(s)
+		return sum(self.matrix[s])
 	
 	def l(self, s1:int, s2:int, obs:str) -> float:
 		"""
-		Returns the rate associated to the transition from state `s1` to state
-		``s2`` generating observation ``obs``.
+		Returns the rate associated to the transition from state `s1`, seeing
+		`obs`, to state `s2`.
 
 		Parameters
 		----------
 		s1 : int
 			A state ID.
 		s2 : int
 			A state ID.
@@ -67,19 +84,23 @@
 			An observation.
 
 		Returns
 		-------
 		float
 			A rate.
 		"""
-		return self.matrix[s1][s2][self.alphabet.index(obs)]
+		self._checkStateIndex(s1)
+		self._checkStateIndex(s2)
+		if self.labeling[s1] != obs:
+			return 0.0
+		return self.matrix[s1][s2]
 	
 	def lkl(self, s: int, t: float) -> float:
 		"""
-		Returns the likelihood of staying in `s` state for a duration ``t``.
+		Returns the likelihood of staying in `s` state for a duration `t`.
 
 		Parameters
 		----------
 		s : int
 			A state ID.
 		t : float
 			A waiting time.
@@ -108,15 +129,15 @@
 			An observation.
 
 		Returns
 		-------
 		float
 			A probability.
 		"""
-		return self.l(s1,s2,obs)/self.e(s1)
+		return self.l(s1,s2, obs)/self.e(s1)
 	
 	def expected_time(self, s:int) -> float:
 		"""
 		Returns the expected waiting time in `s`, i.e. the inverse of
 		the exit rate.
 		
 		Parameters
@@ -127,83 +148,81 @@
 		Returns
 		-------
 		float
 			expected waiting time in this state.
 		"""
 		return 1/self.e(s)
 
-	def getAlphabet(self,state: int = -1) -> list:
+	def getLabel(self,state: int) -> str:
 		"""
-		If state is set, returns the list of all the observations we could
-		see in `state`. Otherwise it returns the alphabet of the model. 
+		Returns the label of `state`.
 
 		Parameters
 		----------
-		state : int, optional
+		state : int
 			a state ID
 
 		Returns
 		-------
-		list of str
-			list of observations
+		str
+			a label
+
+		Example
+		-------
+		>>> model.getLabel(2)
+		'Label-of-state-2'
 		"""
-		if state == -1:
-			return self.alphabet
-		else:
-			return [self.alphabet[i] for i in where(self.matrix[state].sum(axis=0) > 0.0)[0]]
-		
-	def save(self,file_path:str):
-		"""Save the model into a text file.
+		self._checkStateIndex(state)
+		return self.labeling[state]
+	
+	def getAlphabet(self) -> list:
+		"""
+		Returns the alphabet of this model.
 
-		Parameters
-		----------
-		file_path : str
-			path of the output file.
+		Returns
+		-------
+		list of str
+			The alphabet of this model
 		
-		Examples
-		--------
-		>>> model.save("my_model.txt")
+		Example
+		-------
+		>>> model.getAlphabet()
+		['a','b','c','d','done']
 		"""
-		f = open(file_path, 'w')
-		f.write("CTMC\n")
-		f.write(str(self.alphabet))
-		f.write('\n')
-		super()._save(f)
+		return self.alphabet
 
 	def _stateToString(self,state:int) -> str:
-		res = "----STATE s"+str(state)+"----\n"
+		res = "----STATE "+str(state)+"--"+self.labeling[state]+"----\n"
 		res += "Exepected waiting time: "+str(self.expected_time(state))+'\n'
 		den = self.e(state)
 		for j in range(len(self.matrix[state])):
-			for k in range(len(self.matrix[state][j])):
-				if self.matrix[state][j][k]/den > 0.0001:
-					res += "s"+str(state)+" - ("+str(self.alphabet[k])+") -> s"
-					res += str(j)+" : lambda = "+str(self.matrix[state][j][k])
-					res += '\n'
+			if self.matrix[state][j]/den > 0.0001:
+				res += "s"+str(state)+" -> s"
+				res += str(j)+" : lambda = "+str(self.matrix[state][j])+'\n'
 		return res
 	
 	def next(self,state: int) -> tuple:
 		"""
 		Return a state-observation pair according to the distributions 
 		described by matrix
+		
 		Returns
 		-------
 		output : (int, str)
 			A state-observation pair.
 		"""
 		exps = []
-		for exp_lambda in self.matrix[state].flatten():
+		for exp_lambda in self.matrix[state]:
 			if exp_lambda <= 0.0:
 				exps.append(1024)
 			else:
 				exps.append(exponential(1/exp_lambda))
-		next_index = exps.index(min(exps))
-		next_state = next_index//len(self.alphabet)
-		next_obs = self.alphabet[next_index % len(self.alphabet)]
-		return (next_state, next_obs, min(exps))
+		next_state= exps.index(min(exps))
+		next_obs = self.labeling[state]
+		return (next_obs, next_state, min(exps))
 
 	def run(self,number_steps: int, timed: bool = False) -> list:
 		"""
 		Simulates a run of length ``number_steps`` of the model and return the
 		sequence of observations generated. If ``timed`` it returns a list of
 		pairs waiting time-observation.
 		
@@ -219,49 +238,50 @@
 		output: list of str
 			trace generated by the run.
 		"""
 		output = []
 		current = resolveRandom(self.initial_state)
 		c = 0
 		while c < number_steps:
-			[next_state, symbol, time_spent] = self.next(current)
-			
+			[symbol, next_state, time_spent] = self.next(current)
+			output.append(symbol)
 			if timed:
 				output.append(time_spent)
-
-			output.append(symbol)
 			current = next_state
 			c += 1
+		output.append(self.labeling[current])
 		return output
 	
 	def _computeAlphas_timed(self, sequence: list, times: int) -> float:
-		obs_seq   = [sequence[i] for i in range(1,len(sequence),2)]
-		times_seq = [sequence[i] for i in range(0,len(sequence),2)]
-		len_seq = len(obs_seq)
+		obs_seq   = [sequence[i] for i in range(0,len(sequence),2)]
+		times_seq = [sequence[i] for i in range(1,len(sequence),2)]
+		len_seq = len(obs_seq)-1
 		prev_arr = array(self.initial_state)
 		for k in range(len_seq):
 			new_arr = zeros(self.nb_states)
 			for s in range(self.nb_states):
-				p = array([self.l(ss,s,obs_seq[k])*exp(-self.e(ss)*times_seq[k]) for ss in range(self.nb_states)])
+				p = array([self.l(ss,s,obs_seq[k])*exp(-self.e(ss)*times_seq[k]) for ss in range(self.nb_states) ])
 				new_arr[s] = dot(prev_arr,p)
 			prev_arr = new_arr
-		return log(prev_arr.sum())*times
+		last_arr = prev_arr * (array(self.labeling) == obs_seq[-1])
+		return log(last_arr.sum())*times
+
 
 	def logLikelihood(self,traces: Set) -> float:
-		if type(traces.sequences[0][0]) == str: # non-timed traces
+		if traces.type == 0: # non-timed traces
 			return super().logLikelihood(traces)
 		else: # timed traces
-			if platform != "win32":
+			if platform != "win32" and platform != "darwin":
 				p = Pool(processes = cpu_count()-1)
 				tasks = []
 				for seq,times in zip(traces.sequences,traces.times):
 					tasks.append(p.apply_async(self._computeAlphas_timed, [seq, times,]))
 				temp = [res.get() for res in tasks if res.get() != False]
 			else:
-				temp = [self._computeAlphas_timed(traces.sequences[i],traces.times[i]) for i in range(len(traces.sequences))]
+				temp = [self._computeAlphas_timed(seq,times) for seq,times in zip(traces.sequences,traces.times)]
 			return sum(temp)/sum(traces.times)
 
 	def toMC(self, name: str="unknown_MC") -> MC:
 		"""
 		Returns the equivalent untimed MC.
 
 		Parameters
@@ -274,16 +294,33 @@
 		MC
 			An equivalent untimed model.
 		"""
 		new_matrix = self.matrix
 		for i in range(self.nb_states):
 			new_matrix[i] /= self.e(i)
 
-		return MC(new_matrix,self.alphabet,self.initial_state,name)
+		return MC(new_matrix,self.labeling,name)
+
+	def save(self,file_path:str):
+		"""Save the model into a text file.
 
+		Parameters
+		----------
+		file_path : str
+			path of the output file.
+		
+		Examples
+		--------
+		>>> model.save("my_model.txt")
+		"""
+		f = open(file_path, 'w')
+		f.write("CTMC\n")
+		f.write(str(self.labeling))
+		f.write('\n')
+		super()._save(f)
 
 def loadCTMC(file_path: str) -> MC:
 	"""
 	Load an CTMC saved into a text file.
 
 	Parameters
 	----------
@@ -295,155 +332,164 @@
 	output : CTMC
 		The CTMC saved in `file_path`.
 	"""
 	f = open(file_path,'r')
 	l = f.readline()[:-1] 
 	if l != "CTMC":
 		print("ERROR: this file doesn't describe an CTMC: it describes a "+l)
-	alphabet = literal_eval(f.readline()[:-1])
+	labeling = literal_eval(f.readline()[:-1])
 	name = f.readline()[:-1]
 	initial_state = array(literal_eval(f.readline()[:-1]))
 	matrix = literal_eval(f.readline()[:-1])
 	matrix = array(matrix)
 	f.close()
-	return CTMC(matrix, alphabet, initial_state, name)
-
-
-def asynchronousComposition(m1: CTMC, m2: CTMC, name: str='unknown_composition', disjoint: bool=False) -> CTMC:
-	"""
-	Returns a CTMC equivalent to the asynchronous composition of `m1` and `m2`.
-
-	Parameters
-	----------
-	m1 : CTMC
-		First model of the composition.
-	m2 : CTMC
-		Second model of the composition.
-	name : str, optional
-		Name of the output model, by default 'unknown_composition'
-	disjoint : bool, optional
-		If True the observation generated by the composition contain 1 or 2
-		according to which model generated this observation. By default False.
-
-	Returns
-	-------
-	CTMC
-		A CTMC equivalent to the asynchronous composition of `m1` and `m2`.
-
-	"""
-
-	nb_states = m1.nb_states * m2.nb_states
-	if disjoint:
-		alphabet = [i+'1' for i in m1.alphabet] + [i+'2' for i in m2.alphabet]
-	else:
-		alphabet = list(set(m1.alphabet).union(set(m2.alphabet)))
-
-	matrix = zeros((nb_states, nb_states, len(alphabet)))
-	initial_state = zeros(nb_states)
-	for i in range(m1.nb_states):
-		for j in range(m2.nb_states):
-			initial_state[i*m2.nb_states+j] = m1.initial_state[i]*m2.initial_state[j]
-
-	for s in range(nb_states):
-		for s1 in range(m1.nb_states):
-			dest = s1*m2.nb_states+(s%m2.nb_states)
-			for i,o in enumerate(m1.alphabet):
-				if disjoint:
-					matrix[s][dest][i] = m1.matrix[s//m2.nb_states][s1][i]
-				else:
-					matrix[s][dest][alphabet.index(o)] = m1.matrix[s//m2.nb_states][s1][i]
-		for s2 in range(m2.nb_states):
-			dest = s2+s-(s%m2.nb_states)
-			for i,o in enumerate(m2.alphabet):
-				if disjoint:
-					matrix[s][dest][len(m1.alphabet)+i] = m2.matrix[s%m2.nb_states][s2][i]
-				else:
-					matrix[s][dest][alphabet.index(o)] = m2.matrix[s%m2.nb_states][s2][i]
-
-	return CTMC(matrix,alphabet,initial_state,name)
+	return CTMC(matrix, labeling, name)
 
 def CTMC_random(nb_states: int, alphabet: list, min_exit_rate_time : int,
 				max_exit_rate_time: int, self_loop: bool = True,
-				random_initial_state: bool=False) -> CTMC:
+				random_initial_state: bool=True) -> CTMC:
 	"""
 	Generates a random CTMC. All the rates will be between 0 and 1.
 	All the exit rates will be integers.
 
 	Parameters
 	----------
 	nb_states : int
 		Number of states.
 	alphabet : list of str
 		List of observations.
 	min_exit_rate_time: int
-		Minimum exit rate for the states.
+		Minimum exit rate for the states (included).
 	max_exit_rate_time: int
-		Minimum exit rate for the states.
+		Maximum exit rate for the states (included).
 	self_loop: bool, optional
 		Wether or not there will be self loop in the output model.
 		Default is True.
 	random_initial_state: bool, optional
 		If set to True we will start in each state with a random probability, otherwise we will always start in state 0.
-		Default is False.
-
+		Default is True.
+	
 	Returns
 	-------
 	CTMC
 		A pseudo-randomly generated CTMC.
+
+	Examples
+	--------
+	>>> model = CTMC_random(2,['a','b'],1,5)
+	>>> print(model)
+	Name: CTMC_random_2_states
+	Initial state: s2
+	----STATE 0--a----
+	Exepected waiting time: 2.0
+	s0 -> s0 : lambda = 0.38461538461538464
+	s0 -> s1 : lambda = 0.11538461538461539
+	----STATE 1--b----
+	Exepected waiting time: 4.0
+	s1 -> s0 : lambda = 0.13636363636363635
+	s1 -> s1 : lambda = 0.11363636363636363
+	----STATE 2--init----
+	Exepected waiting time: 1.0
+	s2 -> s0 : lambda = 0.2
+	s2 -> s1 : lambda = 0.8
 	"""
-	#lambda between 0 and 1
-	s = []
-	for j in range(nb_states):
-		s.append([])
-		for i in range(nb_states):
-			if self_loop or i != j:
-				s[j] += [i] * len(alphabet)
-	if self_loop:
-		obs = alphabet*nb_states
-	else:
-		obs = alphabet*(nb_states-1)
+	if nb_states < len(alphabet):
+		print("WARNING: the size of the alphabet is higher than the",end=" ")
+		print("number of states. Some labels will not be assigned to",end=" ")
+		print("any states.")
+	
+	if 'init' in alphabet:
+		msg =  "The label 'init' cannot be used: it is reserved for initial states."
+		raise SyntaxError(msg)
 
+	
+	labeling = alphabet[:min(len(alphabet),nb_states)] + choices(alphabet,k=nb_states-len(alphabet))
+	
 	matrix = []
 	for i in range(nb_states):
 		if self_loop:
-			random_probs = array(randomProbabilities(len(alphabet)*nb_states))
+			random_probs = array(randomProbabilities(nb_states))
 		else:
-			p = randomProbabilities(len(alphabet)*(nb_states-1))
-			random_probs = array(p[:i*len(alphabet)]+[0.0 for _ in range(len(alphabet))]+p[i*len(alphabet):])
+			p = randomProbabilities(nb_states-1)
+			random_probs.insert(i,0.0)
+		p = randomProbabilities(nb_states)
 		av_waiting_time = randint(min_exit_rate_time,max_exit_rate_time)
 		p = random_probs/av_waiting_time
-		p = reshape(p, (nb_states,len(alphabet)))
 		matrix.append(p)
-	matrix = array(matrix)
-
+	
+	labeling.append("init")
 	if random_initial_state:
-		init = randomProbabilities(nb_states)
+		matrix.append(append(randomProbabilities(nb_states),0.0))
 	else:
-		init = 0
-	return CTMC(matrix, alphabet, init,"CTMC_random_"+str(nb_states)+"_states")
+		matrix.append([1.0]+[0.0 for i in range(nb_states)])
+	
+	matrix = array(matrix)
+	return CTMC(matrix, labeling,"CTMC_random_"+str(nb_states)+"_states")
 
-def CTMC_state(transitions:list, alphabet:list, nb_states:int) -> ndarray:
+def createCTMC(transitions: list, labeling: list, initial_state, name: str ="unknown_CTMC") -> CTMC:
 	"""
-	Given the list of all transition leaving a state `s`, it generates
-	the ndarray describing this state `s` in the CTMC.matrix.
-	This method is useful while creating a model manually.
+	An user-friendly way to create a CTMC.
 
 	Parameters
 	----------
-	transitions : [ list of tuples (int, str, float)]
+	transitions : [ list of tuples (int, int, float)]
 		Each tuple represents a transition as follow: 
-		(destination state ID, observation, rate).
-	alphabet : list
-		alphabet of the model in which this state is.
-	nb_states: int
-		number of states in which this state is
-
+		(source state ID, destination state ID, rate).
+	labeling: list of str
+		A list of N observations (with N the nb of states).
+		If `labeling[s] == o` then state of ID `s` is labelled by `o`.
+		Each state has exactly one label.
+	initial_state : int or list of float
+		Determine which state is the initial one (then it's the id of the
+		state), or what are the probability to start in each state (then it's
+		a list of probabilities).
+	name : str, optional
+		Name of the model.
+		Default is "unknow_CTMC"
+	
 	Returns
 	-------
-	ndarray
-		ndarray describing this state `s` in the CTMC.matrix.
+	CTMC
+		the CTMC describes by `transitions`, `labeling`, and `initial_state`.
+	
+	Examples
+	--------
+	>>> model = createCTMC([(0,1,1.0),(1,0,0.3),(1,1,0.2)],['b','a'],0,"My_MC")
+	>>> print(model)
+	Name: My_MC
+	Initial state: s0
+	----STATE 0--b----
+	Exepected waiting time: 1.0
+	s0 -> s1 : lambda = 1.0
+	----STATE 1--a----
+	Exepected waiting time: 2.0
+	s1 -> s0 : lambda = 0.3
+	s1 -> s1 : lambda = 0.2
 	"""
+	if 'init' in labeling:
+		msg =  "The label 'init' cannot be used: it is reserved for initial states."
+		raise SyntaxError(msg)
+	
+	states = list(set([i[0] for i in transitions]+[i[1] for i in transitions]))
+	states.sort()
+	nb_states = len(states)
+	
+	if nb_states > len(labeling):
+		raise ValueError("All states are not labelled (the labeling list is too small).")
+	elif nb_states < len(labeling):
+		print("WARNING: the labeling list is bigger than the number of states")
 
-	res = zeros((nb_states,len(alphabet)))
+	res = zeros((nb_states,nb_states))
 	for t in transitions:
-		res[t[0]][alphabet.index(t[1])] = t[2]
-	return res
+		res[states.index(t[0])][states.index(t[1])] = t[2]
+	
+	labeling.append('init')
+	res = vstack((res,zeros(len(res))))
+	res = hstack((res,zeros(len(res))[:,newaxis]))
+	if type(initial_state) == int:
+		res[-1][initial_state] = 1.0
+	else:
+		if type(initial_state) == ndarray:
+			initial_state = initial_state.tolist()
+		res[-1] = array(initial_state+[0.0])
+
+	return CTMC(res, labeling, name)
```

### Comparing `jajapy-0.8/jajapy/gohmm/BW_GOHMM.py` & `jajapy-0.9/jajapy/gohmm/BW_GOHMM.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/gohmm/GOHMM.py` & `jajapy-0.9/jajapy/gohmm/GOHMM.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/hmm/BW_HMM.py` & `jajapy-0.9/jajapy/hmm/BW_HMM.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 			Default is True.
 
 		Returns
 		-------
 		HMM
 			fitted HMM.
 		"""
+		if type(traces) != Set:
+			traces = Set(traces, t=0)
 		if not initial_model:
 			if not nb_states:
 				print("Either nb_states or initial_model should be set")
 				return
 			initial_model = HMM_random(nb_states,traces.getAlphabet(),random_initial_state)
 		self.alphabet = initial_model.getAlphabet()
 		return super().fit(traces, initial_model, output_file, epsilon, max_it, pp, verbose,return_data,stormpy_output)
```

### Comparing `jajapy-0.8/jajapy/hmm/HMM.py` & `jajapy-0.9/jajapy/hmm/HMM.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/mc/Alergia.py` & `jajapy-0.9/jajapy/mc/Alergia.py`

 * *Files 21% similar despite different names*

```diff
@@ -118,24 +118,24 @@
 						if self._compatibleMerge(i,j):
 							j -= 1
 							break
 
 		m = self._toMC()
 
 		try:
-			from ..with_stormpy import jajapyModeltoStorm
+			from ..with_stormpy import jajapyModeltoStormpy
 			stormpy_installed = True
 		except ModuleNotFoundError:
 			stormpy_installed = False
 		if stormpy_output and not stormpy_installed:
 			print("WARNING: stormpy not found. The output model will not be a stormpy sparse model")
 			stormpy_output = False
 		
 		if stormpy_output:
-			return jajapyModeltoStorm(m)
+			return jajapyModeltoStormpy(m)
 		else:
 			return m
 		
 
 	def _transitionStateAction(self,state,action):
 		try:
 			return self.states_transitions[state][1][self.states_transitions[state][2].index(action)]
@@ -230,21 +230,42 @@
 
 		self.states_counter[i] += self.states_counter[j]
 		self.states_lbl[j] = None
 		self.states_transitions[j] = None
 		self.states_counter[j] = None
 
 	def _toMC(self):
-		self.nb_states = len(self.states_lbl) - self.states_lbl.count(None)
-		states = []
-		c = -1 
-		for i in range(len(self.states_transitions)):
-			if self.states_lbl[i] != None:
-				c+=1
-				self.states_transitions[i][0] = [j/self.states_counter[i] for j in self.states_transitions[i][0]]
-				self.states_transitions[i][0] = normalize(self.states_transitions[i][0])
-				self.states_transitions[i][1] = [j-self.states_lbl[:j].count(None) for j in self.states_transitions[i][1]]
-				l = list(zip(self.states_transitions[i][1], self.states_transitions[i][2], self.states_transitions[i][0]))
-				l = MC_state(l, self.alphabet, self.nb_states)
-				states.append(l)
-		states = array(states)
-		return MC(states, self.alphabet,0)
+		states = [j for j in range(len(self.states_transitions)) if self.states_lbl[j] != None]
+		nb_init= len(states)
+		# states[x] = y : y->index alergia x->index jajapy
+		labeling = [None for s in states]
+		transitions = []
+
+		for s in range(nb_init):
+			ai = states[s]
+			p = [j/self.states_counter[ai] for j in self.states_transitions[ai][0]]
+			p = normalize(p)
+			o = self.states_transitions[ai][2]
+			d = [states.index(dest) for dest in self.states_transitions[ai][1]]
+			for obs, dest, i in zip(o,d,range(len(d))):
+				if labeling[dest] == None:
+					labeling[dest] = obs
+				elif labeling[dest] != obs:
+					d[i] = len(states)
+					labeling.append(obs)
+					states.append(states[dest])
+			transitions.append([(s,d[i],p[i]) for i in range(len(p))])
+				
+		for s in range(nb_init,len(states)):
+			transitions.append([(s,i[1],i[2]) for i in transitions[states.index(states[s])]])
+		
+		for i,j in enumerate(labeling):
+			if j == None:
+				labeling[i] = ''
+				initial_state = i
+		
+		trans = []
+		for i in transitions:
+			trans += i
+
+		return createMC(trans,labeling,initial_state)
+
```

### Comparing `jajapy-0.8/jajapy/mc/BW_MC.py` & `jajapy-0.9/jajapy/mc/BW_MC.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,53 +65,54 @@
 		MC or stormpy.SparseDtmc
 			The fitted MC.
 			If `stormpy_output` is set to `False` or if stormpy is not available on
 			the machine it returns a `jajapy.MC`, otherwise it returns a `stormpy.SparseDtmc`
 		"""
 		if type(traces) != Set:
 			traces = Set(traces, t=0)
+				
+		alphabet = traces.getAlphabet()
+		if not 'init' in alphabet:
+			for s in range(len(traces.sequences)):
+				traces.sequences[s].insert(0,'init')
+		else:
+			alphabet.remove("init")
+		
 		if not initial_model:
 			if not nb_states:
-				print("Either nb_states or initial_model should be set")
-				return
-			initial_model = MC_random(nb_states,traces.getAlphabet(),random_initial_state)
-		self.alphabet = initial_model.getAlphabet()
+				raise ValueError("Either nb_states or initial_model should be set")
+			initial_model = MC_random(nb_states,alphabet,random_initial_state)
+
 		return super().fit(traces, initial_model, output_file, epsilon, max_it, pp, verbose,return_data,stormpy_output)
 
 	def _processWork(self,sequence,times):
 		alpha_matrix = self.computeAlphas(sequence)
-		beta_matrix = self.computeBetas(sequence)
+		beta_matrix  = self.computeBetas( sequence)
 		proba_seq = alpha_matrix.T[-1].sum()
-		if proba_seq != 0.0:
-			den = (alpha_matrix.T[:-1]*beta_matrix.T[:-1]*times/proba_seq).sum(axis=0)
-			num = zeros(shape=(self.nb_states,self.nb_states,len(self.alphabet)))
-			for s in range(self.nb_states):
-				for ss in range(self.nb_states):
-					p = array([self.h_tau(s,ss,o) for o in sequence])
-					alph_bet = alpha_matrix[s][:-1]*p*beta_matrix[ss][1:]*times/proba_seq
-					for o,obs in enumerate(self.alphabet):
-						arr_dirak = [1 if t == obs else 0 for t in sequence]
-						num[s,ss,o] = (alph_bet*arr_dirak).sum()
-			####################
-			num_init = alpha_matrix.T[0]*beta_matrix.T[0]*times/proba_seq
-			####################
-			return [den,num, proba_seq,times,num_init]
-		return False
+		if proba_seq == 0.0:
+			return False
+		####################
+		den = (alpha_matrix.T[:-1]*beta_matrix.T[:-1]*times/proba_seq).sum(axis=0)			
+		num = zeros(shape=(self.nb_states,self.nb_states))
+		for s in range(self.nb_states):
+			for ss in range(self.nb_states):
+				p = array([self.h_tau(s,ss,o) for o in sequence])
+				num[s,ss] = dot(alpha_matrix[s][:-1]*p*beta_matrix[ss][1:],times/proba_seq).sum()
+		####################
+		return [den,num, proba_seq,times]
 
 	def _generateHhat(self,temp):
 		den = array([i[0] for i in temp]).sum(axis=0)
 		num = array([i[1] for i in temp]).sum(axis=0)
 		lst_proba=array([i[2] for i in temp])
 		lst_times=array([i[3] for i in temp])
-		lst_init =array([i[4] for i in temp]).T
 
 		currentloglikelihood = dot(log(lst_proba),lst_times)
 
 		for s in range(len(den)):
 			if den[s] == 0.0:
 				den[s] = 1.0
 				num[s] = self.h.matrix[s]
 
-		matrix = num/den[:, newaxis, newaxis]
-		initial_state = [lst_init[s].sum()/lst_init.sum() for s in range(self.nb_states)]
-		return [MC(matrix,self.alphabet,initial_state),currentloglikelihood]
+		matrix = num/den[:, newaxis]
+		return [MC(matrix,self.h.labeling),currentloglikelihood]
```

### Comparing `jajapy-0.8/jajapy/mdp/Active_BW_MDP.py` & `jajapy-0.9/jajapy/mdp/Active_BW_MDP.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 	"""
 	def __init__(self):
 		super().__init__()
 
 	def fit(self,traces: Set, lr, nb_iterations: int, nb_sequences: int,
 			sequence_length: int = None, epsilon_greedy: float = 0.9,
 			initial_model: MDP=None, nb_states: int=None,
-			random_initial_state: bool=False, output_file: str=None,
+			random_initial_state: bool=True, output_file: str=None,
 			epsilon: float=0.01, max_it: int=inf,pp: str='',
 			verbose: bool = True, return_data: bool= False, stormpy_output: bool = False):
 		"""
 		Fits the model according to ``traces``.
 
 		Parameters
 		----------
@@ -159,16 +159,15 @@
 		Returns
 		-------
 		MDP
 			fitted MDP.
 		"""
 		if stormpy_output:
 			try:
-				#import stormpy as st
-				from ..with_stormpy import jajapyModeltoStorm
+				from ..with_stormpy import jajapyModeltoStormpy
 			except ModuleNotFoundError:
 				print("WARNING: stormpy not found. The output model will not be a stormpy sparse model")
 				stormpy_output = False
 
 		counter = 0
 		start_time = datetime.now()
 		_, info = super().fit(traces, initial_model,nb_states,
@@ -211,15 +210,15 @@
 		running_time = datetime.now()-start_time
 		running_time = running_time.total_seconds()
 
 		if verbose:
 			self._endPrint(counter, running_time)
 
 		if stormpy_output:
-			self.h = jajapyModeltoStorm(self.h)
+			self.h = jajapyModeltoStormpy(self.h)
 			
 		if return_data:
 			info = {"learning_rounds":counter,
 					"learning_time":running_time,
 					"training_set_loglikelihood":self.h.logLikelihood(total_traces)}
 			return self.h, info
 
@@ -291,16 +290,16 @@
 		else:
 			temp = array([self._computeProbas(seq, times) for seq,times in zip(traces.sequences,traces.times)])
 		temp = temp.sum(axis=0)
 		scheduler = [self.h.getActions()[argmin(temp[s])] for s in range(self.nb_states)]
 		return MemorylessScheduler(scheduler)
 
 	def _computeProbas(self,seq:list,time:int) -> array:
-		sequence_actions = [seq[i] for i in range(0,len(seq),2)]
-		sequence_obs = [seq[i+1] for i in range(0,len(seq),2)]
+		sequence_actions = [seq[i+1] for i in range(0,len(seq)-1,2)]
+		sequence_obs = [seq[i] for i in range(0,len(seq)-1,2)] + [seq[-1]]
 		alpha_matrix = self.computeAlphas(sequence_obs,sequence_actions).T[:-1].T
 		res = zeros(shape=(len(self.actions),self.nb_states))
 		fact = alpha_matrix.sum(axis=0) # fact[t] proba to generate sequence_obs[:t]
 
 		for ia,a in enumerate(self.actions):
 			arr_dirak = array([1.0 if t == a else 0.0 for t in sequence_actions])
 			arr_dirak = arr_dirak*time/fact
```

### Comparing `jajapy-0.8/jajapy/mdp/BW_MDP.py` & `jajapy-0.9/jajapy/mdp/BW_MDP.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .MDP import *
 from ..base.BW import *
 from ..base.Set import Set
-from ..base.tools import normalize
-from numpy import array, dot, append, zeros, ones, log, inf
+from numpy import array, dot, append, zeros, ones, log, inf, isnan
 
 NB_PROCESS = 11
 
 class BW_MDP(BW):
 	"""
 	Class for general Passive Baum-Welch algorithm on MDP.
 	This algorithm is described here:
@@ -70,25 +69,30 @@
 		MDP or stormpy.SparseMdp
 			The fitted MDP.
 			If `stormpy_output` is set to `False` or if stormpy is not available on
 			the machine it returns a `jajapy.MDP`, otherwise it returns a `stormpy.SparseMdp`
 		"""
 		if type(traces) != Set:
 			traces = Set(traces, t=1)
+
+		actions, alphabet = traces.getActionsObservations()
+
 		if not initial_model:
 			if not nb_states:
-				print("Either nb_states or initial_model should be set")
-				return
-			actions, observations = traces.getActionsObservations()
-			initial_model = MDP_random(nb_states,observations,actions,random_initial_state)
-		else:
-			observations = initial_model.getAlphabet()
-			actions = initial_model.getActions()
-		self.alphabet = observations
-		self.actions = actions
+				raise ValueError("Either nb_states or initial_model should be set")
+			if 'init' in alphabet:
+				alphabet.remove("init")
+			initial_model = MDP_random(nb_states,alphabet,actions,random_initial_state)
+
+		for s in range(len(traces.sequences)):
+			if traces.sequences[s][0] != 'init':
+				traces.sequences[s].insert(0,initial_model.getActions(initial_model.labeling.index("init"))[0])
+				traces.sequences[s].insert(0,'init')
+					
+		self.actions = initial_model.actions
 		return super().fit(traces, initial_model, output_file, epsilon, max_it, pp, verbose,return_data,stormpy_output)
 
 	def h_tau(self,s1: int,act: str,s2: int,obs: str) -> float:
 		"""
 		Returns the probability of moving from state ``s1`` executing `action`
 		to ``s2`` generating observation ``obs``.
 
@@ -125,20 +129,22 @@
 		Returns
 		-------
 		2-D narray
 			array containing the alpha values.
 		"""
 		len_seq = len(sequence)
 		init_arr = self.h.initial_state
-		zero_arr = zeros(shape=(len_seq*self.nb_states,))
-		alpha_matrix = append(init_arr,zero_arr).reshape(len_seq+1,self.nb_states)
-		for k in range(len_seq):
+		zero_arr = zeros(shape=((len_seq-1)*self.nb_states,))
+		alpha_matrix = append(init_arr,zero_arr).reshape(len_seq,self.nb_states)
+		for k in range(len_seq-1):
 			for s in range(self.nb_states):
 				p = array([self.h_tau(ss,sequence_actions[k],s,sequence[k]) for ss in range(self.nb_states)])
 				alpha_matrix[k+1,s] = dot(alpha_matrix[k],p)
+		
+		alpha_matrix[-1] *= (array(self.h.labeling) == sequence[-1])
 		return alpha_matrix.T
 
 	def computeBetas(self,sequence: list,sequence_actions: list) -> array:
 		"""
 		Compute the beta values for ``sequence`` under the current BW
 		hypothesis.
 
@@ -151,75 +157,62 @@
 
 		Returns
 		-------
 		2-D narray
 			array containing the beta values.
 		"""
 		len_seq = len(sequence)
-		init_arr = ones(self.nb_states)
-		zero_arr = zeros(shape=(len_seq*self.nb_states,))
-		beta_matrix = append(zero_arr,init_arr).reshape(len_seq+1,self.nb_states)
-		for k in range(len(sequence)-1,-1,-1):
+		init_arr = ones(self.nb_states)*(array(self.h.labeling) == sequence[-1])
+		zero_arr = zeros(shape=((len_seq-1)*self.nb_states,))
+		beta_matrix = append(zero_arr,init_arr).reshape(len_seq,self.nb_states)
+		for k in range(len(sequence)-2,-1,-1):
 			for s in range(self.nb_states):
 				p = array([self.h_tau(s,sequence_actions[k],ss,sequence[k]) for ss in range(self.nb_states)])
 				beta_matrix[k,s] = dot(beta_matrix[k+1],p)
 		return beta_matrix.T
 
 	def _processWork(self,sequence,times):
-		sequence_actions = [sequence[i] for i in range(0,len(sequence),2)]
-		sequence_obs = [sequence[i+1] for i in range(0,len(sequence),2)]
+		sequence_actions = [sequence[i+1] for i in range(0,len(sequence)-1,2)]
+		sequence_obs = [sequence[i] for i in range(0,len(sequence)-1,2)]+[sequence[-1]]
 		alpha_matrix = self.computeAlphas(sequence_obs,sequence_actions)
 		beta_matrix = self.computeBetas(sequence_obs,sequence_actions)
 		proba_seq = alpha_matrix.T[-1].sum()
 		if proba_seq != 0.0:
 			den = zeros(shape=(self.nb_states,len(self.actions)))
-			num = zeros(shape=(self.nb_states,len(self.actions),self.nb_states*len(self.alphabet)))	
+			num = zeros(shape=(self.nb_states,len(self.actions),self.nb_states))
+			
 			for s in range(self.nb_states):
 				for i,a in enumerate(self.actions):
-					arr_dirak = [1.0 if t == a else 0.0 for t in sequence_actions]
+					arr_dirak = array([1.0 if t == a else 0.0 for t in sequence_actions])
 					den[s,i] += dot(alpha_matrix[s][:-1]*beta_matrix[s][:-1]*arr_dirak,times/proba_seq).sum()
-				c = 0
+			
 				for ss in range(self.nb_states):
-					p = array([self.h_tau(s,a,ss,o) for o,a in zip(sequence_obs,sequence_actions)])
-					for obs in self.alphabet:
-						for ia,act in enumerate(self.actions):
-							arr_dirak = [1.0 if o == obs and a == act else 0.0 for o,a in zip(sequence_obs,sequence_actions)]
-							num[s,ia,c] = dot(alpha_matrix[s][:-1]*arr_dirak*beta_matrix[ss][1:]*p,times/proba_seq).sum()
-						c += 1
-			num_init = alpha_matrix.T[0]*beta_matrix.T[0]*times/proba_seq
-			return [den,num, proba_seq,times,num_init]
+					p = array([self.h_tau(s,a,ss,o) for o,a in zip(sequence_obs[:-1],sequence_actions)])
+					for ia,act in enumerate(self.actions):
+						arr_dirak = [1.0 if a == act else 0.0 for a in sequence_actions]
+						num[s,ia,ss] = dot(alpha_matrix[s][:-1]*arr_dirak*beta_matrix[ss][1:]*p,times/proba_seq).sum()
+			return [den,num,proba_seq,times]
 		return False
 
 	def _generateHhat(self,temp):
 		den = array([i[0] for i in temp]).sum(axis=0)
-		num = array([i[1] for i in temp]).T.sum(axis=3).T
+		if type(den) == float64: # den == 0.0
+			msg = 'The current hypothesis is not able to generate any of the '
+			msg+= 'sequence in the training set.'
+			raise ValueError(msg)
+		
+		num = array([i[1] for i in temp]).sum(axis=0)
 		lst_proba=array([i[2] for i in temp])
 		lst_times=array([i[3] for i in temp])
-		lst_init =array([i[4] for i in temp]).T
 
 		currentloglikelihood = dot(log(lst_proba),lst_times)
 
-		list_sta = []
-		for i in range(self.nb_states):
-			for _ in self.alphabet:
-				list_sta.append(i)
-		list_obs = self.alphabet*self.nb_states
-		new_states = []
-
 		for s in range(self.nb_states):
-			array_s = []
-			for j,a in enumerate(self.actions):
-				if den[s][j] != 0.0:
-					temp = list(zip(list_sta, list_obs, [num[s][j][i]/den[s][j] for i in range(len(list_sta))]))
-					temp = MDP_state({a:temp},self.h.alphabet,self.h.nb_states,[a])
-					array_s.append(temp[0])
-				else:
-					# if we have no info about action a in state s -> don't change anything
-					# this can happen specially with active learning
-					array_s.append(self.h.matrix[s][j])
-		
-			new_states.append(array_s)
+			for a in range(len(self.actions)):
+				if den[s][a] == 0.0 or isnan(den[s][a]):
+					den[s][a] = 1.0
+					num[s][a] = self.h.matrix[s][a]
+		den = den.reshape(self.nb_states,len(self.actions),1)
+		matrix = num/den
 
-		initial_state = normalize([lst_init[s].sum()/lst_init.sum() for s in range(self.nb_states)])
-		matrix = array(new_states)
-		return [MDP(matrix,self.h.alphabet,self.h.actions,initial_state), currentloglikelihood]
+		return [MDP(matrix,self.h.labeling,self.h.actions), currentloglikelihood]
```

### Comparing `jajapy-0.8/jajapy/mdp/IOAlergia.py` & `jajapy-0.9/jajapy/mdp/IOAlergia.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,20 +181,25 @@
 			A list of all possible observations
 		a : list of str
 			A list of all possible actions
 		"""
 		self.states = states
 		self.observations = o
 		self.actions = a
+		self.initial = []
 
 	def __str__(self) -> str:
 		res = ""
 		for s in self.states:
 			res += str(s)
 		return res
+	
+	def addInitialState(self,state:int) -> None:
+		if not state in self.initial:
+			self.initial.append(state)
 
 	def successor(self, state: int, action: str, obs: str) -> int:
 		"""
 		Returns the index of the state we reach after executing ``action`` in
 		``state`` and seeing ``obs``.
 
 		Parameters
@@ -356,35 +361,33 @@
 		----------
 		seq : list
 			A trace, i.e. a list of alternating action-observation.
 
 		Returns
 		-------
 		bool
-			_description_
+			True if the IOFTPA can generate the given trace ``seq``.
 		"""
-		s_current = 0
-		i_current = 0
-		path = [s_current]
-		while i_current < len(seq):
+		for s_current in self.initial:
+			i_current = 0
+			path = [s_current]
 			f = True
-			for s in self.states[s_current].successorsAction(seq[i_current]):
-				if self.states[s].observation == seq[i_current+1]:
-					s_current = s
-					path.append(s_current)
-					i_current += 2
-					f = False
-					break
+			while i_current < len(seq) and f:
+				f = False
+				for s in self.states[s_current].successorsAction(seq[i_current]):
+					if self.states[s].observation == seq[i_current+1]:
+						s_current = s
+						path.append(s_current)
+						i_current += 2
+						f = True
+						break
+				
 			if f:
-				for s in path:
-					self.states[s].pprint()
-				print()
-				print(seq)
-				return False
-		return True
+				return True
+		return False
 
 
 	def cleanMDP(self,red: list) -> MDP:
 		"""
 		Returns a MDP built from a subset of states of this IOFTPA.
 
 		Parameters
@@ -393,31 +396,27 @@
 			A list of state IDs.
 
 		Returns
 		-------
 		MDP
 			An MDP.
 		"""
-		states = []
-		for i in range(len(red)):
-			self.states[red[i]].setId(i)
-
-		for i in red:
-			new_dic = {}
-			dic = self.states[i].transitions
-			for a in dic:
-				dic[a].append([])
-				new_dic[a] = []
-				tot = sum(self.states[i].transitions[a][0])
-				for j in range(len(dic[a][0])):
-					new_dic[a].append((self.states[dic[a][1][j]].id,self.states[dic[a][1][j]].observation,dic[a][0][j]/tot))
-			states.append(MDP_state(new_dic, self.observations,len(red),self.actions))
-		matrix = array(states)
 
-		return MDP(matrix,self.observations,self.actions,0)
+		actions = self.actions
+		states = red
+		labeling = [self.states[i].observation for i in states]+['init']
+		transitions = zeros((len(states)+1,len(actions),len(states)+1))
+		
+		for si,s in enumerate([self.states[i] for i in states]):
+			for ai,a in enumerate([a for a in actions if s.actionAllowed(a)]):
+				tot = sum(s.transitions[a][0])
+				for p,s2 in zip(s.transitions[a][0],s.transitions[a][1]):
+					transitions[si][ai][states.index(s2)] = p/tot
+		transitions[-1][0][0] = 1.0
+		return MDP(transitions, labeling, actions)
 
 
 
 class IOAlergia:
 	"""
 	Class for an  IOAlergia algorithm.
 	This algorithm is described here:
@@ -438,48 +437,56 @@
 		self.observations.sort()
 		self.N = sum(sample.times)
 		self.n = len(sample.sequences[0])
 		self.t = self._buildIOFPTA()
 		self.a = self.t
 		
 	def _buildIOFPTA(self):
-		states_lbl = [[]]
-		states = [IOFPTA_state("",self.N,[])]
+		states_lbl = []
+		states = []
 		#init states_lbl and states_counter
-		for i in range(0,self.n,2):
-			for seq in range(len(self.sample.sequences)):
-				if not self.sample.sequences[seq][:i+2] in states_lbl:
-					states_lbl.append(self.sample.sequences[seq][:i+2])
-					states.append( IOFPTA_state(self.sample.sequences[seq][i+1], self.sample.times[seq], self.sample.sequences[seq][:i+2]))
+		for seq,times in zip(self.sample.sequences, self.sample.times):
+			for i in range(0,len(seq),2):
+				if not seq[:i+1] in states_lbl:
+					states_lbl.append(seq[:i+1])
+					states.append( IOFPTA_state(seq[i], times, seq[:i+1]))
 				else:
-					states[states_lbl.index(self.sample.sequences[seq][:i+2])].counterAdd(self.sample.times[seq])
+					states[states_lbl.index(seq[:i+1])].counterAdd(times)
 		#sorting states
 		states_lbl.sort()
 		for s in states:
 			s.setId(states_lbl.index(s.label))
 		states_sorted = [None]*len(states)	
 		for s in states:
 			states_sorted[s.id] = s
 		#init states_transitions
+
+		initial = []
 		for s1 in range(len(states_sorted)):
 			len_s1 = len(states_sorted[s1].label)
+			if len_s1 == 1:
+				initial.append(s1)
+				
 			s2 = s1 + 1
 			while s2 < len(states_sorted):
 				if len(states_sorted[s2].label) < len_s1 + 2: # too short
 					s2 += 1
 				elif len(states_sorted[s2].label) > len_s1 + 2: # too long
 					s2 += 1
 				elif states_sorted[s2].label[:-2] != states_sorted[s1].label: # not same prefix
 					s2 += 1
 				else: # OK
 					act = states_sorted[s2].label[-2]
 					states_sorted[s1].transitionsAdd(act, states_sorted[s2].counter, s2)
 					s2 += 1
 
-		return IOFPTA(states_sorted,self.observations,self.actions)
+		res =  IOFPTA(states_sorted,self.observations,self.actions)
+		for i in initial:
+			res.addInitialState(i)
+		return res
 
 	def fit(self,sample:Set,epsilon:float, stormpy_output: bool = True):
 		"""
 		Fits the model according to ``traces``.
 
 		Parameters
 		----------
@@ -498,15 +505,17 @@
 			The fitted MDP.
 			If `stormpy_output` is set to `False` or if stormpy is not available on
 			the machine it returns a `jajapy.MDP`, otherwise it returns a `stormpy.SparseMdp`
 		"""
 		self.actions, self.observations = sample.getActionsObservations()
 		self._initialize(sample,epsilon,self.actions,self.observations)
 		red = [0]
-		blue = self.a.states[0].successors()
+		blue = []
+		for i in self.a.initial:
+			blue += self.a.states[i].successors()
 
 		while len(blue) != 0:
 			state_b = blue[0]
 			merged = False
 			
 			for state_r in red:
 				if self.t.compatible(state_r,state_b,epsilon):
@@ -525,19 +534,19 @@
 
 			blue = list(set(blue))
 			blue.sort()
 
 		m = self.a.cleanMDP(red)
 
 		try:
-			from ..with_stormpy import jajapyModeltoStorm
+			from ..with_stormpy import jajapyModeltoStormpy
 			stormpy_installed = True
 		except ModuleNotFoundError:
 			stormpy_installed = False
 		if stormpy_output and not stormpy_installed:
 			print("WARNING: stormpy not found. The output model will not be a stormpy sparse model")
 			stormpy_output = False
 		
 		if stormpy_output:
-			return jajapyModeltoStorm(m)
+			return jajapyModeltoStormpy(m)
 		else:
 			return m
```

### Comparing `jajapy-0.8/jajapy/mdp/MDP.py` & `jajapy-0.9/jajapy/mdp/MDP.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 from ..base.tools import resolveRandom, randomProbabilities, checkProbabilities
 from math import log
 from ..base.Model import Model
 from ..base.Set import Set
 from .Scheduler import Scheduler
-from numpy.random import geometric, randint
-from numpy import array, append, dot, zeros, vsplit, ndarray, where, reshape
+from numpy.random import geometric
+from numpy import array, append, dot, zeros, vsplit, ndarray, where, reshape, vstack, append, concatenate
 from ast import literal_eval
 from multiprocessing import cpu_count, Pool
+from random import choices
 
 class MDP(Model):
 	"""
 	Class representing a MDP.
 	"""
-	def __init__(self,matrix: ndarray, alphabet: list,
-				 actions: list,initial_state,name: str="unknown_MDP"):
+	def __init__(self,matrix: ndarray, labeling: list, actions:list, name: str="unknown_MDP"):
 		"""
 		Create a MDP.
 
 		Parameters
 		----------
 		matrix : ndarray
 			Represents the transition matrix.
 			`matrix[s1][act_ID][s2][obs_ID]` is the probability of moving 
 			from `s1` to `s2` by executing action of ID `act_ID` and seeing 
 			the observation of ID `obs_ID`.
-		alphabet: list
-			The list of all possible observations, such that:
-			`alphabet.index("obs")` is the ID of `obs`.
-		alphabet: list
-			The list of all possible observations, such that:
-			`alphabet.index("obs")` is the ID of `obs`.
-		initial_state : int or list of float
-			Determine which state is the initial one (then it's the id of the
-			state), or what are the probability to start in each state (then it's
-			a list of probabilities).
+		labeling: list of str
+			A list of N observations (with N the nb of states).
+			If `labeling[s] == o` then state of ID `s` is labelled by `o`.
+			Each state has exactly one label.
+		actions: list of str
+			The list of all possible actions, such that:
+			`actions.index("act")` is the ID of `act`.
 		name : str, optional
 			Name of the model. Default is "unknow_MDP"
 		"""
 		self.actions = actions
-		self.nb_actions = len(actions)
-		self.alphabet = alphabet
+		self.nb_actions = len(self.actions)
+		self.labeling = labeling
+		self.alphabet = list(set(labeling))
+
+		if not 'init' in self.labeling:
+			msg = "No initial state given: at least one"
+			msg += " state should be labelled by 'init'."
+			raise ValueError(msg)
+		initial_state = [1.0/self.labeling.count("init") if i=='init' else 0.0 for i in self.labeling]
+
 		super().__init__(matrix,initial_state,name)
+		if len(labeling) != self.nb_states:
+			raise ValueError("The length of labeling is not equal to the number of states")
 		for i in range(self.nb_states):
 			for a in range(self.nb_actions):
-				if not checkProbabilities(matrix[i][a]) and round(matrix[i][a].sum(),3) != 0.0:
-					print("Error: the probability to take a transition from",end=" ")
-					print("state",i,"executing",actions[a],"should be",end=" ")
-					print("1.0 or 0.0, here it's",matrix[i][a].sum())
-					return False
+				if not checkProbabilities(matrix[i][a]):
+					msg = "The probability to take a transition from state "
+					msg+= str(i)+" executing action "+self.actions[a]+" should be 1.0 or 0.0, here it's "+str(matrix[i][a].sum())
+					raise ValueError(msg)
 
 	def getActions(self, state:int =-1) -> list:
 		"""
 		If state is set, returns the list of all the actions available
 		in `state`. Otherwise it returns the actions of the model. 
 
 
@@ -60,48 +66,64 @@
 		state : int, optional
 			a state ID
 
 		Returns
 		-------
 		list of str
 			list of actions
+		
+		Example
+		-------
+		>>> model.getActions()
+		['A','B','C','D']
+		>>> model.getActions(1)
+		['A','C']
 		"""
 		if state == -1:
 			return self.actions
 		else:
-			return set(self.actions[i] for i in where(self.matrix[state].sum(axis=2) > 0.0)[0])
+			return list(set(self.actions[i] for i in where(self.matrix[state].sum(axis=1) > 0.0)[0]))
 
-	def getAlphabet(self,state: int = -1, action: str = None) -> list:
+	def getAlphabet(self) -> list:
+		"""
+		Returns the alphabet of this model.
+
+		Returns
+		-------
+		list of str
+			The alphabet of this model
+		
+		Example
+		-------
+		>>> model.getAlphabet()
+		['a','b','c','d','done']
+		"""
+		return self.alphabet
+	
+	def getLabel(self,state: int) -> str:
 		"""
-		If state is set, returns the list of all the observations we could
-		see in `state`. If the action is set as well, it returns the list of 
-		all the observations we could see in `state` after executing `action`. 
-		Otherwise it returns the alphabet of the model. 
+		Returns the label of `state`.
 
 		Parameters
 		----------
-		state : int, optional
+		state : int
 			a state ID
-		action : str
-			an action
 
 		Returns
 		-------
-		list of str
-			list of observations
+		str
+			a label
+
+		Example
+		-------
+		>>> model.getLabel(2)
+		'Label-of-state-2'
 		"""
-		if state == -1:
-			return self.alphabet
-		else:
-			if action == None:
-				return [self.alphabet[i] for i in where(self.matrix[state].sum(axis=0).sum(axis=0) > 0.0)[0]]
-			elif action in self.getActions(state):
-				return [self.alphabet[i] for i in where(self.matrix[state][self.actions.index(action)].sum(axis=0) > 0.0)[0]]
-			else:
-				return []
+		self._checkStateIndex(state)
+		return self.labeling[state]
 
 
 	def tau(self,s1: int,action: str,s2: int,obs: str) -> float:
 		"""
 		Returns the probability of moving from state ``s1`` executing `action`
 		to ``s2`` generating observation ``obs``.
 
@@ -116,86 +138,102 @@
 		obs: str
 			generated observation.
 		
 		Returns
 		-------
 		float
 			A probability.
-		"""
-		if s1 < 0 or s1 > self.nb_states or not action in self.actions or not obs in self.alphabet:
+		
+		Example
+		-------
+		>>> model.tau(0,'A',1,'a')
+		0.6
+		>>> model.getLabel(0)
+		'a'
+		>>> model.tau(0,'A',1,'b')
+		0.0
+		>>> model.tau(0,'B',1,'b')
+		0.0
+		>>> model.getActions(0)
+		['A']		
+		"""
+		self._checkStateIndex(s1)
+		self._checkStateIndex(s2)
+		if obs != self.labeling[s1]:
+			return 0.0
+		if action not in self.actions:
 			return 0.0
-		return self.matrix[s1][self.actions.index(action)][s2][self.alphabet.index(obs)]
+		return self.matrix[s1][self.actions.index(action)][s2]
 	
 	def a(self,s1: int,s2: int, action: str) -> float:
 		"""
 		Returns the probability of moving from state `s1` to state `s2`,
 		just after executing `action`.
-		If `s1` or `s2` is not a valid state ID it returns 0.
-
 		Parameters
 		----------
 		s1 : int
 			ID of the source state.		
 		s2 : int
 			ID of the destination state.
 		action: str
 			an action.
 		
 		Returns
 		-------
 		float
 			Probability of moving from state `s1` to state `s2`.
-		"""
-		if s1 < 0 or s1 >= self.nb_states or s2 < 0 or s2 >= self.nb_states or action not in self.getActions(s1):
-			return 0.0
-		return self.matrix[s1][self.actions.index(action)][s2].sum(axis=1)
-	
-	def b(self, s: int, l: str, action: str) -> float:
-		"""
-		Returns the probability of generating `l` in state `s`,
-		just after executing `action`.
-		If `s` is not a valid state ID it returns 0.
-
-		Parameters
-		----------
-		s : int
-			ID of the source state.		
-		l : str
-			observation.
-		action: str
-			an action.
 		
-		Returns
+		Example
 		-------
-		float
-			probability of generating `l` in state `s`.
+		>>> model.a(0,1)
+		0.6
 		"""
-		if s < 0 or s >= self.nb_states or l not in self.alphabet or action not in self.getActions(s):
-			return 0.0
-		return round(self.matrix[s][self.actions.index(action)].sum(axis=0)[self.alphabet.index(l)],5)
+		self._checkStateIndex(s1)
+		self._checkStateIndex(s2)
+		return self.matrix[s1][self.actions.index(action)][s2]
 	
+
 	def next(self,state: int, action: str) -> tuple:
 		"""
 		Return a state-observation pair according to the distributions 
-		described by matrix
+		described by matrix.
 
 		Parameters
 		----------
 		state: int
 			source state ID.
 		action: str
 			An action.
 
 		Returns
 		-------
 		output : (int, str)
 			A state-observation pair.
+
+		Example
+		-------
+		>>> model.next(0,'A')
+		(1,'a')
+		>>> model.getLabel(0)
+		'a'
+		>>> model.next(0)
+		(1,'a')
+		>>> model.next(0)
+		(2,'a')
+		>>> model.a(0,1,'A')
+		0.6
+		>>> model.a(0,2,'A')
+		0.4
+		>>> model.next(0,'C')
+		(2,'a')
+		>>> model.a(0,2,'C')
+		1.0
 		"""
-		c = resolveRandom(self.matrix[state][self.actions.index(action)].flatten())
-		return (c//len(self.alphabet), self.alphabet[c%len(self.alphabet)])
+		c = resolveRandom(self.matrix[state][self.actions.index(action)])
+		return (c, self.labeling[state])
 			
 	def run(self,number_steps: int,scheduler: Scheduler) -> list:
 		"""
 		Simulates a run of length ``number_steps`` of the model under
 		``scheduler`` and returns the sequence of actions-observations generated.
 		
 		Parameters
@@ -214,21 +252,21 @@
 		current_len = 0
 		while current_len < number_steps:
 			action = scheduler.getAction()
 
 			while action not in self.getActions(current):
 				action = scheduler.getAction()
 			
-			res.append(action)
 			next_state, observation = self.next(current,action)
 			res.append(observation)
+			res.append(action)
 			scheduler.addObservation(observation)
-			
 			current = next_state
 			current_len += 1
+		res.append(self.labeling[current])
 		return res
 
 	def generateSet(self, set_size: int, param, scheduler: Scheduler, distribution=None, min_size=None) -> list:
 		"""
 		Generates a set (training set / test set) containing `set_size` traces
 		generated under ``scheduler``.
 
@@ -271,24 +309,15 @@
 
 			if not trace in seq:
 				seq.append(trace)
 				val.append(0)
 
 			val[seq.index(trace)] += 1
 
-		return Set(seq,val,from_MDP=True)
-	
-	def _stateToString(self,state:int) -> str:
-		res = "----STATE s"+str(state)+"----\n"
-		for ai,a in enumerate(self.actions):
-			for s in range(self.nb_states):
-				for oi,o in enumerate(self.alphabet):
-					if self.matrix[state][ai][s][oi] > 0.0001:
-						res += "s"+str(state)+" - ("+a+") -> s"+str(s)+" : "+o+" : "+str(self.matrix[state][ai][s][oi])+'\n'
-		return res
+		return Set(seq,val,t=1)
 	
 	def save(self,file_path:str):
 		"""Save the model into a text file.
 
 		Parameters
 		----------
 		file_path : str
@@ -296,19 +325,28 @@
 		
 		Examples
 		--------
 		>>> model.save("my_model.txt")
 		"""
 		f = open(file_path, 'w')
 		f.write("MDP\n")
-		f.write(str(self.alphabet))
+		f.write(str(self.labeling))
 		f.write('\n')
 		f.write(str(self.actions))
 		f.write('\n')
 		super()._save(f)
+	
+	def _stateToString(self,state:int) -> str:
+		res = "----STATE "+str(state)+"--"+self.labeling[state]+"----\n"
+		for ai,a in enumerate(self.actions):
+			for s in range(self.nb_states):
+				if self.matrix[state][ai][s] > 0.0001:
+					res += "s"+str(state)+" - ("+a+") -> s"+str(s)+" : "+str(self.matrix[state][ai][s])+'\n'
+		return res
+	
 
 	def _logLikelihood_oneproc(self,sequences: Set) -> float:
 		"""
 		Compute the average loglikelihood of a set of sequences.
 
 		Parameters
 		----------
@@ -321,28 +359,31 @@
 			loglikelihood of ``sequences`` under this model.
 		"""
 		sequences_sorted = sequences.sequences[:]
 		sequences_sorted.sort()
 		loglikelihood = 0.0
 		alpha_matrix = self._initAlphaMatrix(len(sequences_sorted[0])//2)
 		for seq in range(len(sequences_sorted)):
-			sequence_actions = [sequences_sorted[seq][i] for i in range(0,len(sequences_sorted[seq]),2)]
-			sequence_obs = [sequences_sorted[seq][i+1] for i in range(0,len(sequences_sorted[seq]),2)]
+			sequence_actions = [sequences_sorted[seq][i+1] for i in range(0,len(sequences_sorted[seq])-1,2)]
+			sequence_obs = [sequences_sorted[seq][i] for i in range(0,len(sequences_sorted[seq])-1,2)]
 			sequence = sequences_sorted[seq]
 			times = sequences.times[sequences.sequences.index(sequence)]
 			common = 0
 			if seq > 0:
 				while common < min(len(sequences_sorted[seq-1]),len(sequence)):
 					if sequences_sorted[seq-1][common] != sequence[common]:
 						break
 					common += 1
 			common = int(common/2)
 			alpha_matrix = self._updateAlphaMatrix(sequence_obs,sequence_actions,common,alpha_matrix)
-			if alpha_matrix[-1].sum() > 0:
-				loglikelihood += log(alpha_matrix[-1].sum()) * times
+			
+			last_arr = alpha_matrix[-1] * (array(self.labeling) == sequence[-1])
+			last_arr = last_arr.sum()
+			if last_arr > 0.0:
+				loglikelihood += log(last_arr) * times
 
 		return loglikelihood/sum(sequences.times)
 	
 	def _updateAlphaMatrix(self, sequence_obs: list,
 						   sequence_actions:list,
 						   common: int, alpha_matrix: list) -> array:
 		"""
@@ -412,65 +453,26 @@
 		Returns
 		-------
 		float
 			loglikelihood of ``sequence`` multiplied by ``times``.
 		"""
 		len_seq = len(sequence)
 		prev_arr = array(self.initial_state)
-		for k in range(0,len_seq,2):
+		
+		for k in range(0,len_seq-1,2):
 			new_arr = zeros(self.nb_states)
 			for s in range(self.nb_states):
-				p = array([self.tau(ss,sequence[k],s,sequence[k+1]) for ss in range(self.nb_states)])
+				p = array([self.tau(ss,sequence[k+1],s,sequence[k]) for ss in range(self.nb_states)])
 				new_arr[s] = dot(prev_arr,p)
 			prev_arr = new_arr
+		prev_arr = prev_arr*(array(self.labeling) == sequence[-1])
 		if prev_arr.sum() == 0.0:
 			return 0.0
 		return log(prev_arr.sum())*times
 
-	#-------------------------------------------
-
-	def saveToPrism(self,output_file:str) -> None:
-		"""
-		Save the MDP into a file with the Prism format.
-		WARNING: This works only if we start in a given state
-		with probability 1.0.
-
-		Parameters
-		----------
-		output_file : str 
-			Where to save the output Prism MDP.
-		"""
-		if not 1.0 in self.initial_state:
-			print("ERROR: in PRISM the initial state is deterministic (not stochastic).")
-			return None
-		f = open(output_file,'w',encoding="utf-8")
-		f.write("mdp\n")
-		f.write("\tmodule "+self.name+"\n")
-		f.write("\ts : [0.."+str(self.nb_states-1)+"] init "+str(self.initial_state.index(1.0))+";\n")
-		f.write("\tl : [0.."+str(len(self.observations()))+"] init "+str(len(self.observations()))+";\n")
-		f.write("\n")
-		for s in range(self.nb_states):
-			for a in self.getActions(s):
-				ai = self.actions.index(a)
-				f.write("\t["+a+"] s="+str(s)+" -> ")
-				res = ""
-				for s2 in range(self.nb_states):
-					for oi,o in enumerate(self.alphabet):
-						if self.matrix[s][a][s2][oi] > 0.0:
-							res += self.matrix[s][a][s2][oi]+" : (s'="+str(s2)+") & (l'="+o+") + "
-				res = res[:-3]
-				res+= ";\n"
-				f.write(res)
-		f.write("\n")
-		f.write("endmodule\n")
-
-		for l in range(len(self.alphabet)):
-			f.write('label "'+self.alphabet[l]+'" = l='+str(l)+';\n')
-		f.close()
-
 def loadMDP(file_path: str) -> MDP:
 	"""
 	Load an MDP saved into a text file.
 
 	Parameters
 	----------
 	file_path : str
@@ -480,190 +482,142 @@
 	-------
 	output : MDP
 		The MDP saved in `file_path`.
 	"""
 	f = open(file_path,'r')
 	l = f.readline()[:-1] 
 	if l != "MDP":
-		print("ERROR: this file doesn't describe an MDP: it describes a "+l)
-	alphabet = literal_eval(f.readline()[:-1])
+		msg = " this file doesn't describe an MC: it describes a "+l
+		raise ValueError(msg)
+	labeling = literal_eval(f.readline()[:-1])
 	actions = literal_eval(f.readline()[:-1])
 	name = f.readline()[:-1]
 	initial_state = array(literal_eval(f.readline()[:-1]))
 	matrix = literal_eval(f.readline()[:-1])
 	matrix = array(matrix)
 	f.close()
-	return MDP(matrix, alphabet, actions, initial_state, name)
+	return MDP(matrix, labeling, actions, name)
 
 
-def MDP_random(nb_states: int,alphabet: list,actions: list,random_initial_state: bool = False, deterministic: bool = False) -> MDP:
+def MDP_random(nb_states: int,alphabet: list, actions: list,random_initial_state: bool = True, deterministic: bool = False) -> MDP:
 	"""
 	Generate a random MDP.
 
 	Parameters
 	----------
 	number_states : int
 		Number of states.
 	alphabet : list of str
 		List of observations.
 	actions : list of str
 		List of actions.	
 	random_initial_state: bool, optional
 		If set to True we will start in each state with a random probability, otherwise we will always start in state 0.
-		Default is False.
+		Default is True.
 	deterministic: bool, optional
 		If True, the model will be determinstic: in state `s`, with action `a`, there is only one transition labelled with `o`.
 		Default is False.
 	
 	Returns
 	-------
 	MDP
 		A pseudo-randomly generated MDP.
 	"""
+	if 'init' in alphabet:
+		msg =  "The label 'init' cannot be used: it is reserved for initial states."
+		raise SyntaxError(msg)
+
+	if nb_states < len(alphabet):
+		print("WARNING: the size of the alphabet is geater than the",end=" ")
+		print("number of states. Some labels will not be assigned to",end=" ")
+		print("any states.")
+	labeling = alphabet[:min(len(alphabet),nb_states)] + choices(alphabet,k=nb_states-len(alphabet))
+	alphabet = list(set(labeling))
+
 	matrix = []
 	for s in range(nb_states):
-		matrix.append([])
-		for a in actions:
-			if not deterministic:
-				p = array(randomProbabilities(nb_states*len(alphabet)))
-				p = reshape(p, (nb_states,len(alphabet)))
-			else:
-				p = zeros((nb_states,len(alphabet)))
+		if not deterministic:
+			p = array([append(randomProbabilities(nb_states),0.0) for a in actions])
+			p = reshape(p,(len(actions),nb_states+1))
+			matrix.append(p)
+		else:
+			matrix.append([])
+			for a in actions:
+				dest = [choices(where(array(labeling) == o)[0]) for o in alphabet]
+				p = zeros(nb_states)
 				probs = randomProbabilities(len(alphabet))
-				states = randint(0,nb_states,len(alphabet))
-				for i in range(len(alphabet)):
-					p[states[i]][i] = probs[i]
-			
-			matrix[-1].append(p)
-
-	matrix = array(matrix)
+				for i,j in zip(dest,probs):
+					p[i] = j
+				matrix[-1].append(append(p,0.0))
 
 	if random_initial_state:
-		init = randomProbabilities(nb_states)
+		init = randomProbabilities(nb_states).tolist()+[0.0]
 	else:
-		init = 0
-	return MDP(matrix, alphabet, actions, init,"MDP_random_"+str(nb_states)+"_states")
-
+		init = [1.0]+[0.0 for i in range(nb_states)]
+	matrix.append(array([init for a in actions]))
+	matrix = array(matrix)
+	labeling.append('init')
+	return MDP(matrix, labeling, actions, "MDP_random_"+str(nb_states)+"_states")
 
-def MDPFileToPrism(file_path:str,output_file:str) -> None:
-	"""
-	Translate a MDP save file into a MDP Prism save file.
-	
-	Parameters
-	----------
-	file_path : str
-		The MDP save file.
-	output_file : str 
-		Where to save the output Prism MDP.
-	"""
-	m = loadMDP(file_path)
-	m.saveToPrism(output_file)
 
-def loadPrismMDP(file_path:str) -> MDP:
+def createMDP(transitions:list, labeling:list, initial_state, name: str ="unknown_MDP") -> MDP:
 	"""
-	Load an MDP saved into a text file with the Prism format.
+	An user-friendly way to create an MDP.
 
 	Parameters
 	----------
-	file_path : str
-		Location of the Prism file.
+	transitions : [ list of tuples (int, str, int, float)]
+		Each tuple represents a transition as follow: 
+		(source state ID, action, destination state ID, probability).
+	labeling: list of str
+		A list of N observations (with N the nb of states).
+		If `labeling[s] == o` then state of ID `s` is labelled by `o`.
+		Each state has exactly one label.
+	initial_state : int or list of float
+		Determine which state is the initial one (then it's the id of the
+		state), or what are the probability to start in each state (then it's
+		a list of probabilities).
+	name : str, optional
+		Name of the model.
+		Default is "unknow_MC"
 	
 	Returns
 	-------
 	MDP
-		The MDP saved in `file_path`.
-	"""
-	def readline(f):
-		l = f.readline()
-		print(l)
-		while '//' in l or l == '\n':
-			l = f.readline()
-			print(l)
-		return l
-
-	f = open(file_path)
-	readline(f)
-	l = readline(f)
-	l = l.split(' ')
-
-	states = []
-	init = int(l[-1][:-2])
-	for i in range(int(l[2][4:-1])+1):
-		states.append({})
-
-	actions = []
-	alphabet = []
-
-	l = readline(f)
-	while l[:-1] != "endmodule":
-		act = l[1]
-		actions.append(act)
-		state = int(l[l.find('=')+1:l.find('-')-1])
-		l = (' '+readline(f)).split('+')
-		states[state][act] = []
-		states[state][act].append([ float(i[1:i.find(':')-1]) for i in l ]) #add proba
-		states[state][act].append([ int(i[i.find('=')+1:i.find(')')]) for i in l ]) #add state
-
-		l = readline(f)
-	
-	actions = list(set(actions))
-
-	map_s_o = {}
-	l = readline(f)
-
-	while l:
-		l = l[:-2]
-		if not "goal" in l:
-			obs = l[l.find('"')+1:l.rfind('"')]
-			obs = obs[0].upper() + obs[1:]
-			alphabet.append(obs)
-			l = l.split('|')
-			s = [int(i[i.rfind('=')+1:]) for i in l]
-			for ss in s:
-				map_s_o[ss] = obs
-		l = readline(f)
-
-	alphabet = list(set(alphabet))
-
-	for state in range(len(states)):
-		for a in states[state]:
-			o = [ map_s_o[states[state][a][1][i]] for i in range(len(states[state][a][1])) ]
-			p = states[a][0]
-			s = states[a][1]
-			states[state][a] = list(zip(s,o,p))
-
-
-	states = [MDP_state(j,i) for i,j in enumerate(states)]
-
-	m = MDP(array(states),alphabet,actions,init,file_path[:-6])
-	return m
-
-def MDP_state(transitions:dict, alphabet:list, nb_states:int, actions: list) -> ndarray:
-	"""
-	Given the list of all transition leaving a state `s`, it generates
-	the ndarray describing this state `s` in the MDP.matrix.
-	This method is useful while creating a model manually.
-
-	Parameters
-	----------
-	transition : dict
-			transition = {action1 : [(destination_state_1,observation_1,proba_1),(destination_state_1,observation_1,proba_1)...],
-			action2 : [(destination_state_1,observation_1,proba_1),(destination_state_1,observation_1,proba_1)...],
-			...}
-	alphabet : list
-		alphabet of the model in which this state is.
-	nb_states: int
-		number of states in which this state is
-	actions : list
-		actions of the model in which this state is.
-
-	Returns
-	-------
-	ndarray
-		ndarray describing this state `s` in the MDP.matrix.
+		the MDP describes by `transitions`, `labeling`, and `initial_state`.
+	
+	Examples
+	--------
 	"""
-
-	res = zeros((len(actions),nb_states,len(alphabet)))
-	for a in transitions:
-		for t in transitions[a]:
-			res[actions.index(a)][t[0]][alphabet.index(t[1])] = t[2]
-	return res
+	if 'init' in labeling:
+		msg =  "The label 'init' cannot be used: it is reserved for initial states."
+		raise SyntaxError(msg)
+
+	states = list(set([i[0] for i in transitions]+[i[2] for i in transitions]))
+	states.sort()
+	nb_states = len(states)
+	actions = list(set([i[1] for i in transitions]))
+	actions.sort()
+	nb_actions = len(actions)
+	
+	if nb_states > len(labeling):
+		raise ValueError("all states are not labelled (the labeling list is too small).")
+	elif nb_states < len(labeling):
+		print("WARNING: the labeling list is bigger than the number of states")
+
+	res = zeros((nb_states,nb_actions,nb_states))
+	for t in transitions:
+		res[states.index(t[0])][actions.index(t[1])][states.index(t[2])] = t[3]
+	
+	labeling.append('init')
+	res = vstack((res,zeros((1,nb_actions,nb_states))))
+	res = concatenate((res,zeros((nb_states+1,nb_actions,1))),axis=2)
+	if type(initial_state) == int:
+		for a in range(nb_actions):
+			res[-1][a][initial_state] = 1.0
+	else:
+		if type(initial_state) == ndarray:
+			initial_state = initial_state.tolist()
+		for a in range(nb_actions):
+			res[-1][a] = array(initial_state+[0.0])
+	
+	return MDP(res,labeling,actions,name)
```

### Comparing `jajapy-0.8/jajapy/mdp/Scheduler.py` & `jajapy-0.9/jajapy/mdp/Scheduler.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/mgohmm/BW_MGOHMM.py` & `jajapy-0.9/jajapy/mgohmm/BW_MGOHMM.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .MGOHMM import MGOHMM, MGOHMM_random
 from ..base.BW import *
 from ..base.Set import Set
-from numpy import log, sqrt, inf, newaxis, stack, longdouble
+from numpy import log, sqrt, inf, newaxis, stack, longdouble, isnan
 
 
 class BW_MGOHMM(BW):
 	"""
 	class for general Baum-Welch algorithm on MGOHMM.
 	"""
 	def __init__(self):
@@ -79,14 +79,16 @@
 										  random_initial_state)
 		self.nb_distr = initial_model.nb_distributions
 		return super().fit(traces, initial_model, output_file, epsilon, max_it, pp, verbose, return_data)
 
 	def _processWork(self,sequence,times):
 		sequence = array(sequence)
 		alpha_matrix = self.computeAlphas(sequence,longdouble)
+		if isnan(alpha_matrix).any():
+			return False
 		beta_matrix = self.computeBetas(sequence,longdouble)
 		proba_seq = alpha_matrix.T[-1].sum()
 		if proba_seq != 0.0:
 			den = (alpha_matrix.T[:-1]*beta_matrix.T[:-1]*times/proba_seq).sum(axis=0)
 			num_a  = zeros(shape=(self.nb_states,self.nb_states))
 			num_mu = zeros(shape=(self.nb_states,self.nb_distr))
 			num_va = zeros(shape=(self.nb_states,self.nb_distr))
```

### Comparing `jajapy-0.8/jajapy/mgohmm/MGOHMM.py` & `jajapy-0.9/jajapy/mgohmm/MGOHMM.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,27 @@
 		Name of the model.
 		Default is "unknown_MGOHMM"
 	"""
 	def __init__(self,matrix,output,initial_state,name="unknown_MGOHMM"):
 		self.nb_distributions = len(output[0])
 		for i in range(len(output)):
 			if len(output[i]) != self.nb_distributions:
-				print("ERROR: all state must have as much distributions")
-				return False
+				raise ValueError("All state must have as much distributions")
+
 		self.output = array(output)
 		if min(self.output.T[1].flatten()) < 0.0:
-			print("ERROR: the sigma parameters must be positive")
-			return False
+			raise ValueError("The sigma parameters must be positive")
+
 		super().__init__(matrix,initial_state,name)
 		for i in range(self.nb_states):
 			if not checkProbabilities(matrix[i]):
-				print("Error: the probability to take a transition from state",i,"should be 1.0, here it's",matrix[i].sum())
-				return False
+				raise ValueError("The probability to take a transition from state",i,"should be 1.0, here it's",matrix[i].sum())
 
 		if len(self.output.flatten()) != self.nb_distributions*self.nb_states*2:
-			print("ERROR: all distribution must have two parameters")
-			return False
+			raise ValueError("All distribution must have two parameters")
 
 
 	def a(self,s1: int,s2: int) -> float:
 		"""
 		Returns the probability of moving from state `s1` to state `s2`.
 
 		Parameters
```

### Comparing `jajapy-0.8/jajapy/tests/GOHMM_test.py` & `jajapy-0.9/jajapy/tests/GOHMM_test.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/tests/HMM_test.py` & `jajapy-0.9/jajapy/tests/HMM_test.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/tests/MGOHMM_test.py` & `jajapy-0.9/jajapy/tests/MGOHMM_test.py`

 * *Files identical despite different names*

### Comparing `jajapy-0.8/jajapy/tests/tools_test.py` & `jajapy-0.9/jajapy/tests/tools_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 	
 	def test_randomProbabilities(var):
 		var.assertRaises(ValueError, randomProbabilities, 0)
 		var.assertRaises(TypeError, randomProbabilities, 0.2)
 		for length in range(1, 6):
 			p = randomProbabilities(length)
 			var.assertEqual(len(p),length)
-			var.assertEqual(sum(p),1.0)
+			var.assertAlmostEqual(sum(p),1.0)
 			for i in range(length):
 				var.assertGreaterEqual(p[i],0.0)
 
 
 if __name__ == "__main__":
 	unittest.main()
```

### Comparing `jajapy-0.8/jajapy.egg-info/PKG-INFO` & `jajapy-0.9/jajapy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jajapy
-Version: 0.8
+Version: 0.9
 Summary: Baum-Welch for all kind of Markov model
 Home-page: UNKNOWN
 Author: Raphaël Reynouard
 Author-email: raphal20@ru.is
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -44,27 +44,28 @@
 <div align="center">
 	
 | Markov Model   |      Learning Algorithm(s) |
 |-------|:-------------:|
 | HMM    | Baum-Welch for HMMs  ([ref](https://web.ece.ucsb.edu/Faculty/Rabiner/ece259/Reprints/tutorial%20on%20hmm%20and%20applications.pdf)) |
 | MC     | Baum-Welch for MCs <br /> Alergia ([ref](https://www.researchgate.net/publication/2543721_Learning_Stochastic_Regular_Grammars_by_Means_of_a_State_Merging_Method/stats)) |
 | MDP    | Baum-Welch for MDPs ([ref](https://arxiv.org/abs/2110.03014))<br /> Active Baum-Welch ([ref](https://arxiv.org/abs/2110.03014))<br /> IOAlergia ([ref](https://link.springer.com/content/pdf/10.1007/s10994-016-5565-9.pdf))|
-| CTMC   | Baum-Welch for CTMCs<br /> MM for asynchronous composition of CTMCs|
+| CTMC   | Baum-Welch for CTMCs|
 | GoHMM  | Baum-Welch for GoHMMs ([ref](http://www.inass.org/2020/2020022920.pdf)) |
 | MGoHMM | Baum-Welch for MGoHMMs |
 
 </div>
 
 `jajapy` generates by default Stormpy models (except for GoHMM and MGoHMM).
 
 ## Installation
 ``pip install jajapy``
 
 ## Requirements
-- numpy
-- scipy
-- stormpy (recommended: if stormpy is not installed, `jajapy` will generate models in jajapy format).
+- [numpy](https://numpy.org/)
+- [scipy](https://scipy.org/)
+- [alive-progress](https://github.com/rsalmei/alive-progress) 
+- [stormpy](https://github.com/moves-rwth/stormpy) (recommended: if stormpy is not installed, `jajapy` will generate models in jajapy format).
 
 ## Documentation
 Available on [readthedoc](https://jajapy.readthedocs.io/en/latest/?)
```

### Comparing `jajapy-0.8/jajapy.egg-info/SOURCES.txt` & `jajapy-0.9/jajapy.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 jajapy/base/BW.py
 jajapy/base/Model.py
 jajapy/base/Set.py
 jajapy/base/__init__.py
 jajapy/base/tools.py
 jajapy/ctmc/BW_CTMC.py
 jajapy/ctmc/CTMC.py
-jajapy/ctmc/MM_CTMC_Composition.py
 jajapy/ctmc/__init__.py
 jajapy/gohmm/BW_GOHMM.py
 jajapy/gohmm/GOHMM.py
 jajapy/gohmm/__init__.py
 jajapy/hmm/BW_HMM.py
 jajapy/hmm/HMM.py
 jajapy/hmm/__init__.py
```

### Comparing `jajapy-0.8/setup.py` & `jajapy-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	long_description = f.read()
 setup(
     name='jajapy',
     long_description=long_description,
     packages=find_packages(),
     install_requires=['numpy', 'scipy', 'alive-progress'],
     long_description_content_type="text/markdown",
-    version='0.8',
+    version='0.9',
     url="",
     description='Baum-Welch for all kind of Markov model',
     author='Raphaël Reynouard',
     author_email="raphal20@ru.is",
     license='MIT',
 	classifiers=[
         "Intended Audience :: Developers",
```

