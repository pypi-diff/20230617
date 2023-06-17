# Comparing `tmp/brainsurf-7.0.0.tar.gz` & `tmp/brainsurf-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsurf-7.0.0.tar", last modified: Fri Jun  9 04:11:56 2023, max compression
+gzip compressed data, was "brainsurf-8.0.1.tar", last modified: Sat Jun 17 05:52:43 2023, max compression
```

## Comparing `brainsurf-7.0.0.tar` & `brainsurf-8.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.777526 brainsurf-7.0.0/
--rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-7.0.0/LICENSE
--rw-rw-rw-   0        0        0     2391 2023-06-09 04:11:56.776512 brainsurf-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-06-09 03:59:51.000000 brainsurf-7.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.435017 brainsurf-7.0.0/brainsurf/
--rw-rw-rw-   0        0        0       70 2023-06-09 04:00:14.000000 brainsurf-7.0.0/brainsurf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.530573 brainsurf-7.0.0/brainsurf/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-7.0.0/brainsurf/analysis/__init__.py
--rw-rw-rw-   0        0        0     3540 2023-06-08 16:28:08.000000 brainsurf-7.0.0/brainsurf/analysis/corelation_analysis.py
--rw-rw-rw-   0        0        0     1756 2023-05-31 17:53:43.000000 brainsurf-7.0.0/brainsurf/analysis/erp_analysis.py
--rw-rw-rw-   0        0        0     1388 2023-06-08 16:30:02.000000 brainsurf-7.0.0/brainsurf/analysis/frequency.py
--rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-7.0.0/brainsurf/analysis/multi_fractal.py
--rw-rw-rw-   0        0        0     6163 2023-06-08 18:09:22.000000 brainsurf-7.0.0/brainsurf/analysis/power_spectrum.py
--rw-rw-rw-   0        0        0     3071 2023-06-08 22:36:24.000000 brainsurf-7.0.0/brainsurf/analysis/stats_analysis.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.554545 brainsurf-7.0.0/brainsurf/cognitive/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-7.0.0/brainsurf/cognitive/__init__.py
--rw-rw-rw-   0        0        0    14202 2023-06-08 23:43:40.000000 brainsurf-7.0.0/brainsurf/cognitive/cognitive_comparision.py
--rw-rw-rw-   0        0        0     4202 2023-06-08 16:35:05.000000 brainsurf-7.0.0/brainsurf/cognitive/cognitive_indexes.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.604570 brainsurf-7.0.0/brainsurf/io/
--rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-7.0.0/brainsurf/io/__init__.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-7.0.0/brainsurf/io/csv.py
--rw-rw-rw-   0        0        0      167 2023-06-08 16:03:18.000000 brainsurf-7.0.0/brainsurf/io/df.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-7.0.0/brainsurf/io/edf.py
--rw-rw-rw-   0        0        0    13064 2023-06-09 01:08:35.000000 brainsurf-7.0.0/brainsurf/io/eeg_data.py
--rw-rw-rw-   0        0        0      213 2023-06-03 12:32:49.000000 brainsurf-7.0.0/brainsurf/io/mff.py
--rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-7.0.0/brainsurf/io/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.633976 brainsurf-7.0.0/brainsurf/machine_learning/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-7.0.0/brainsurf/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-7.0.0/brainsurf/machine_learning/eeg_binary_classification.py
--rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-7.0.0/brainsurf/machine_learning/rnn_module.py
--rw-rw-rw-   0        0        0     2813 2023-05-31 18:17:21.000000 brainsurf-7.0.0/brainsurf/machine_learning/time_series.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.668982 brainsurf-7.0.0/brainsurf/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-7.0.0/brainsurf/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-06-09 01:04:29.000000 brainsurf-7.0.0/brainsurf/preprocessing/artifact_removal.py
--rw-rw-rw-   0        0        0     3877 2023-06-08 16:16:32.000000 brainsurf-7.0.0/brainsurf/preprocessing/baseline.py
--rw-rw-rw-   0        0        0     2141 2023-06-08 16:13:30.000000 brainsurf-7.0.0/brainsurf/preprocessing/epoching.py
--rw-rw-rw-   0        0        0     5481 2023-06-08 17:33:30.000000 brainsurf-7.0.0/brainsurf/preprocessing/filtering.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.684975 brainsurf-7.0.0/brainsurf/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-7.0.0/brainsurf/utils/__init__.py
--rw-rw-rw-   0        0        0      654 2023-06-09 01:14:33.000000 brainsurf-7.0.0/brainsurf/utils/data.py
--rw-rw-rw-   0        0        0     1442 2023-06-08 16:23:07.000000 brainsurf-7.0.0/brainsurf/utils/performance.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.773512 brainsurf-7.0.0/brainsurf/visualization/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-7.0.0/brainsurf/visualization/__init__.py
--rw-rw-rw-   0        0        0    10693 2023-06-09 01:23:23.000000 brainsurf-7.0.0/brainsurf/visualization/comparative_visualize.py
--rw-rw-rw-   0        0        0     3483 2023-05-30 19:11:59.000000 brainsurf-7.0.0/brainsurf/visualization/eeg_data_visualization.py
--rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-7.0.0/brainsurf/visualization/plot_cluster.py
--rw-rw-rw-   0        0        0     1805 2023-06-08 21:00:05.000000 brainsurf-7.0.0/brainsurf/visualization/plot_coherence.py
--rw-rw-rw-   0        0        0     4274 2023-06-08 17:59:04.000000 brainsurf-7.0.0/brainsurf/visualization/plot_correlation.py
--rw-rw-rw-   0        0        0      555 2023-06-06 16:53:17.000000 brainsurf-7.0.0/brainsurf/visualization/plot_eeg_signal.py
--rw-rw-rw-   0        0        0      262 2023-06-08 17:56:49.000000 brainsurf-7.0.0/brainsurf/visualization/plot_heatmap.py
--rw-rw-rw-   0        0        0     2077 2023-06-08 18:16:20.000000 brainsurf-7.0.0/brainsurf/visualization/plot_power_spectrum.py
--rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-7.0.0/brainsurf/visualization/plot_spectogram.py
--rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-7.0.0/brainsurf/visualization/plot_time_series.py
--rw-rw-rw-   0        0        0      566 2023-06-08 16:41:38.000000 brainsurf-7.0.0/brainsurf/visualization/plot_topomap.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.469016 brainsurf-7.0.0/brainsurf.egg-info/
--rw-rw-rw-   0        0        0     2391 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 04:11:56.777526 brainsurf-7.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-06-09 04:00:27.000000 brainsurf-7.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.676858 brainsurf-8.0.1/
+-rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-8.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2391 2023-06-17 05:52:43.674854 brainsurf-8.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-06-09 03:59:51.000000 brainsurf-8.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.482919 brainsurf-8.0.1/brainsurf/
+-rw-rw-rw-   0        0        0       70 2023-06-17 05:52:29.000000 brainsurf-8.0.1/brainsurf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.550445 brainsurf-8.0.1/brainsurf/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-8.0.1/brainsurf/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-06-08 16:28:08.000000 brainsurf-8.0.1/brainsurf/analysis/corelation_analysis.py
+-rw-rw-rw-   0        0        0     1756 2023-05-31 17:53:43.000000 brainsurf-8.0.1/brainsurf/analysis/erp_analysis.py
+-rw-rw-rw-   0        0        0     1388 2023-06-08 16:30:02.000000 brainsurf-8.0.1/brainsurf/analysis/frequency.py
+-rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-8.0.1/brainsurf/analysis/multi_fractal.py
+-rw-rw-rw-   0        0        0     6144 2023-06-14 19:14:17.000000 brainsurf-8.0.1/brainsurf/analysis/power_spectrum.py
+-rw-rw-rw-   0        0        0     3071 2023-06-08 22:36:24.000000 brainsurf-8.0.1/brainsurf/analysis/stats_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.561451 brainsurf-8.0.1/brainsurf/cognitive/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-8.0.1/brainsurf/cognitive/__init__.py
+-rw-rw-rw-   0        0        0    14134 2023-06-09 04:31:07.000000 brainsurf-8.0.1/brainsurf/cognitive/cognitive_comparision.py
+-rw-rw-rw-   0        0        0     4202 2023-06-08 16:35:05.000000 brainsurf-8.0.1/brainsurf/cognitive/cognitive_indexes.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.585448 brainsurf-8.0.1/brainsurf/io/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-8.0.1/brainsurf/io/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-8.0.1/brainsurf/io/csv.py
+-rw-rw-rw-   0        0        0      167 2023-06-08 16:03:18.000000 brainsurf-8.0.1/brainsurf/io/df.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-8.0.1/brainsurf/io/edf.py
+-rw-rw-rw-   0        0        0    13064 2023-06-09 01:08:35.000000 brainsurf-8.0.1/brainsurf/io/eeg_data.py
+-rw-rw-rw-   0        0        0      213 2023-06-03 12:32:49.000000 brainsurf-8.0.1/brainsurf/io/mff.py
+-rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-8.0.1/brainsurf/io/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.599469 brainsurf-8.0.1/brainsurf/machine_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-8.0.1/brainsurf/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-8.0.1/brainsurf/machine_learning/eeg_binary_classification.py
+-rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-8.0.1/brainsurf/machine_learning/rnn_module.py
+-rw-rw-rw-   0        0        0     2813 2023-05-31 18:17:21.000000 brainsurf-8.0.1/brainsurf/machine_learning/time_series.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.616853 brainsurf-8.0.1/brainsurf/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-8.0.1/brainsurf/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-09 07:50:22.000000 brainsurf-8.0.1/brainsurf/preprocessing/artifact_removal.py
+-rw-rw-rw-   0        0        0     3877 2023-06-08 16:16:32.000000 brainsurf-8.0.1/brainsurf/preprocessing/baseline.py
+-rw-rw-rw-   0        0        0     2141 2023-06-08 16:13:30.000000 brainsurf-8.0.1/brainsurf/preprocessing/epoching.py
+-rw-rw-rw-   0        0        0     5481 2023-06-08 17:33:30.000000 brainsurf-8.0.1/brainsurf/preprocessing/filtering.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.628856 brainsurf-8.0.1/brainsurf/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-8.0.1/brainsurf/utils/__init__.py
+-rw-rw-rw-   0        0        0     3010 2023-06-17 05:50:43.000000 brainsurf-8.0.1/brainsurf/utils/data.py
+-rw-rw-rw-   0        0        0     1442 2023-06-08 16:23:07.000000 brainsurf-8.0.1/brainsurf/utils/performance.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.671861 brainsurf-8.0.1/brainsurf/visualization/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-8.0.1/brainsurf/visualization/__init__.py
+-rw-rw-rw-   0        0        0    10690 2023-06-15 18:13:21.000000 brainsurf-8.0.1/brainsurf/visualization/comparative_visualize.py
+-rw-rw-rw-   0        0        0     3483 2023-05-30 19:11:59.000000 brainsurf-8.0.1/brainsurf/visualization/eeg_data_visualization.py
+-rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-8.0.1/brainsurf/visualization/plot_cluster.py
+-rw-rw-rw-   0        0        0     1806 2023-06-09 05:03:08.000000 brainsurf-8.0.1/brainsurf/visualization/plot_coherence.py
+-rw-rw-rw-   0        0        0     4274 2023-06-08 17:59:04.000000 brainsurf-8.0.1/brainsurf/visualization/plot_correlation.py
+-rw-rw-rw-   0        0        0      555 2023-06-06 16:53:17.000000 brainsurf-8.0.1/brainsurf/visualization/plot_eeg_signal.py
+-rw-rw-rw-   0        0        0      262 2023-06-08 17:56:49.000000 brainsurf-8.0.1/brainsurf/visualization/plot_heatmap.py
+-rw-rw-rw-   0        0        0     2061 2023-06-14 18:18:48.000000 brainsurf-8.0.1/brainsurf/visualization/plot_power_spectrum.py
+-rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-8.0.1/brainsurf/visualization/plot_spectogram.py
+-rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-8.0.1/brainsurf/visualization/plot_time_series.py
+-rw-rw-rw-   0        0        0      566 2023-06-08 16:41:38.000000 brainsurf-8.0.1/brainsurf/visualization/plot_topomap.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.523456 brainsurf-8.0.1/brainsurf.egg-info/
+-rw-rw-rw-   0        0        0     2391 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 05:52:43.676858 brainsurf-8.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-06-17 05:52:34.000000 brainsurf-8.0.1/setup.py
```

### Comparing `brainsurf-7.0.0/LICENSE` & `brainsurf-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/PKG-INFO` & `brainsurf-8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 7.0.0
+Version: 8.0.1
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-7.0.0/README.md` & `brainsurf-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/analysis/corelation_analysis.py` & `brainsurf-8.0.1/brainsurf/analysis/corelation_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/analysis/erp_analysis.py` & `brainsurf-8.0.1/brainsurf/analysis/erp_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/analysis/frequency.py` & `brainsurf-8.0.1/brainsurf/analysis/frequency.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/analysis/multi_fractal.py` & `brainsurf-8.0.1/brainsurf/analysis/multi_fractal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/analysis/power_spectrum.py` & `brainsurf-8.0.1/brainsurf/analysis/power_spectrum.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import numpy as np
 from scipy.signal import welch, coherence, correlate
 import astropy as ast 
 from scipy import signal
 
-# def extract_frequency_bands(raw_data, fs=128):
-#     epoch_length = 1000  # Length of each epoch in milliseconds
-#     num_epochs = len(raw_data) // epoch_length
-#     pre_epochs = np.split(raw_data[:num_epochs * epoch_length], num_epochs)
+def extract_frequency_bands_one_channel(raw_data, fs=128):
+    epoch_length = 1000  # Length of each epoch in milliseconds
+    num_epochs = len(raw_data) // epoch_length
+    pre_epochs = np.split(raw_data[:num_epochs * epoch_length], num_epochs)
     
-#     # Initialize the dictionary to store the frequency bands
-#     data = {}
+    # Initialize the dictionary to store the frequency bands
+    data = {}
     
-#     for band in ['alpha', 'beta', 'delta', 'theta', 'gamma']:
-#         if band not in data:
-#             pre_features = []
+    for band in ['alpha', 'beta', 'delta', 'theta', 'gamma']:
+        if band not in data:
+            pre_features = []
             
-#             for epoch in pre_epochs:
-#                 f, psd = welch(epoch, fs=fs)
+            for epoch in pre_epochs:
+                f, psd = welch(epoch, fs=fs)
                 
-#                 # Adjust the frequency range based on the band
-#                 if band == 'alpha':
-#                     band_psd = psd[(f >= 8) & (f <= 13)]
-#                 elif band == 'beta':
-#                     band_psd = psd[(f >= 13) & (f <= 30)]
-#                 elif band == 'delta':
-#                     band_psd = psd[(f >= 1) & (f <= 4)]
-#                 elif band == 'theta':
-#                     band_psd = psd[(f >= 4) & (f <= 8)]
-#                 elif band == 'gamma':
-#                     band_psd = psd[(f >= 30) & (f <= 50)]
-#                 else:
-#                     raise ValueError("Invalid frequency band.")
-#                 band_power = np.mean(band_psd) if band_psd.any() else np.nan
-#                 pre_features.append(band_power)
+                # Adjust the frequency range based on the band
+                if band == 'alpha':
+                    band_psd = psd[(f >= 8) & (f <= 13)]
+                elif band == 'beta':
+                    band_psd = psd[(f >= 13) & (f <= 30)]
+                elif band == 'delta':
+                    band_psd = psd[(f >= 1) & (f <= 4)]
+                elif band == 'theta':
+                    band_psd = psd[(f >= 4) & (f <= 8)]
+                elif band == 'gamma':
+                    band_psd = psd[(f >= 30) & (f <= 50)]
+                else:
+                    raise ValueError("Invalid frequency band.")
+                band_power = np.mean(band_psd) if band_psd.any() else np.nan
+                pre_features.append(band_power)
             
-#             # Make sure the extracted features have the same length as the original data
-#             pre_features += [np.nan] * (len(raw_data) - len(pre_features))
+            # Make sure the extracted features have the same length as the original data
+            pre_features += [np.nan] * (len(raw_data) - len(pre_features))
             
-#             data[band] = pre_features
+            data[band] = pre_features
             
-#     return data
+    return data
 import pandas as pd
 import numpy as np
 from scipy.signal import welch
 
 def extract_frequency_bands(raw_data, fs=128):
     epoch_length = 1000  # Length of each epoch in milliseconds
     num_epochs = len(raw_data) // epoch_length
@@ -130,15 +130,15 @@
     for channel in range(num_channels):
         power_within_bands[channel] = {}
 
         for band_name, frequency_range in frequency_bands.items():
             freq_indices = np.where(np.logical_and(freqs >= frequency_range[0], freqs <= frequency_range[1]))
             power_within_band = np.trapz(psd[channel, freq_indices], freqs[freq_indices])
             power_within_bands[channel][band_name] = power_within_band
-
+    print(power_within_bands)
     return power_within_bands
 
 def calculate_overlapping_percentage(power_within_bands):
     num_channels = len(power_within_bands)
     overlapping_percentage = {}
 
     for channel in power_within_bands.keys():
```

### Comparing `brainsurf-7.0.0/brainsurf/analysis/stats_analysis.py` & `brainsurf-8.0.1/brainsurf/analysis/stats_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/cognitive/cognitive_comparision.py` & `brainsurf-8.0.1/brainsurf/cognitive/cognitive_comparision.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,57 +157,57 @@
     else:
         raise ValueError("Invalid test_type. Options: 'paired_ttest', 'wilcoxon'")
 
     return test_statistic, p_value
 
 
 
-# def compare_eeg_data_stats(pre_merged, post_merged):
-#     # Extract the relevant feature columns
-#     pre_eeg_raw = pre_merged['raw']
-#     pre_alpha = pre_merged['alpha']
-#     pre_beta = pre_merged['beta']
-#     pre_theta = pre_merged['theta']
-#     pre_delta = pre_merged['delta']
-
-#     post_eeg_raw = post_merged['raw']
-#     post_alpha = post_merged['alpha']
-#     post_beta = post_merged['beta']
-#     post_theta = post_merged['theta']
-#     post_delta = post_merged['delta'] 
-#     # Perform t-tests for each feature
-#     t_statistic_raw, p_value_raw = stats.ttest_ind(pre_eeg_raw, post_eeg_raw)
-#     t_statistic_alpha, p_value_alpha = stats.ttest_ind(pre_alpha, post_alpha)
-#     t_statistic_beta, p_value_beta = stats.ttest_ind(pre_beta, post_beta)
-#     t_statistic_theta, p_value_theta = stats.ttest_ind(pre_theta, post_theta)
-#     t_statistic_delta, p_value_delta = stats.ttest_ind(pre_delta, post_delta)
-#     # Perform ANOVA for each feature
-#     f_statistic_raw, p_value_anova_raw = stats.f_oneway(pre_eeg_raw, post_eeg_raw)
-#     f_statistic_alpha, p_value_anova_alpha = stats.f_oneway(pre_alpha, post_alpha)
-#     f_statistic_beta, p_value_anova_beta = stats.f_oneway(pre_beta, post_beta)
-#     f_statistic_theta, p_value_anova_theta = stats.f_oneway(pre_theta, post_theta)
-#     f_statistic_delta, p_value_anova_delta = stats.f_oneway(pre_delta, post_delta)
-
-#     # Calculate effect sizes (Cohen's d) for each feature
-#     effect_size_raw = abs(pre_eeg_raw.mean() - post_eeg_raw.mean()) / pre_eeg_raw.std()
-#     effect_size_alpha = abs(pre_alpha.mean() - post_alpha.mean()) / pre_alpha.std()
-#     effect_size_beta = abs(pre_beta.mean() - post_beta.mean()) / pre_beta.std()
-#     effect_size_theta = abs(pre_theta.mean() - post_theta.mean()) / pre_theta.std()
-#     effect_size_delta = abs(pre_delta.mean() - post_delta.mean()) / pre_delta.std()
-
-#     # Create a DataFrame to store the results
-#     results = pd.DataFrame({
-#         'Feature': ['EEG', 'Alpha', 'Beta', 'Theta', 'Delta'],
-#         'T-Stat': [t_statistic_raw, t_statistic_alpha, t_statistic_beta, t_statistic_theta, t_statistic_delta],
-#         'P-Value (T-Test)': [p_value_raw, p_value_alpha, p_value_beta, p_value_theta, p_value_delta],
-#         'F-Stat': [f_statistic_raw, f_statistic_alpha, f_statistic_beta, f_statistic_theta, f_statistic_delta],
-#         'P-Value (ANOVA)': [p_value_anova_raw, p_value_anova_alpha, p_value_anova_beta, p_value_anova_theta, p_value_anova_delta],
-#         'Effect Size': [effect_size_raw, effect_size_alpha, effect_size_beta, effect_size_theta, effect_size_delta]
-#     })
-#     return results
+def compare_eeg_data_stats_one_channel(pre_merged, post_merged):
+    # Extract the relevant feature columns
+    pre_eeg_raw = pre_merged['raw']
+    pre_alpha = pre_merged['alpha']
+    pre_beta = pre_merged['beta']
+    pre_theta = pre_merged['theta']
+    pre_delta = pre_merged['delta']
+
+    post_eeg_raw = post_merged['raw']
+    post_alpha = post_merged['alpha']
+    post_beta = post_merged['beta']
+    post_theta = post_merged['theta']
+    post_delta = post_merged['delta'] 
+    # Perform t-tests for each feature
+    t_statistic_raw, p_value_raw = stats.ttest_ind(pre_eeg_raw, post_eeg_raw)
+    t_statistic_alpha, p_value_alpha = stats.ttest_ind(pre_alpha, post_alpha)
+    t_statistic_beta, p_value_beta = stats.ttest_ind(pre_beta, post_beta)
+    t_statistic_theta, p_value_theta = stats.ttest_ind(pre_theta, post_theta)
+    t_statistic_delta, p_value_delta = stats.ttest_ind(pre_delta, post_delta)
+    # Perform ANOVA for each feature
+    f_statistic_raw, p_value_anova_raw = stats.f_oneway(pre_eeg_raw, post_eeg_raw)
+    f_statistic_alpha, p_value_anova_alpha = stats.f_oneway(pre_alpha, post_alpha)
+    f_statistic_beta, p_value_anova_beta = stats.f_oneway(pre_beta, post_beta)
+    f_statistic_theta, p_value_anova_theta = stats.f_oneway(pre_theta, post_theta)
+    f_statistic_delta, p_value_anova_delta = stats.f_oneway(pre_delta, post_delta)
+
+    # Calculate effect sizes (Cohen's d) for each feature
+    effect_size_raw = abs(pre_eeg_raw.mean() - post_eeg_raw.mean()) / pre_eeg_raw.std()
+    effect_size_alpha = abs(pre_alpha.mean() - post_alpha.mean()) / pre_alpha.std()
+    effect_size_beta = abs(pre_beta.mean() - post_beta.mean()) / pre_beta.std()
+    effect_size_theta = abs(pre_theta.mean() - post_theta.mean()) / pre_theta.std()
+    effect_size_delta = abs(pre_delta.mean() - post_delta.mean()) / pre_delta.std()
+
+    # Create a DataFrame to store the results
+    results = pd.DataFrame({
+        'Feature': ['EEG', 'Alpha', 'Beta', 'Theta', 'Delta'],
+        'T-Stat': [t_statistic_raw, t_statistic_alpha, t_statistic_beta, t_statistic_theta, t_statistic_delta],
+        'P-Value (T-Test)': [p_value_raw, p_value_alpha, p_value_beta, p_value_theta, p_value_delta],
+        'F-Stat': [f_statistic_raw, f_statistic_alpha, f_statistic_beta, f_statistic_theta, f_statistic_delta],
+        'P-Value (ANOVA)': [p_value_anova_raw, p_value_anova_alpha, p_value_anova_beta, p_value_anova_theta, p_value_anova_delta],
+        'Effect Size': [effect_size_raw, effect_size_alpha, effect_size_beta, effect_size_theta, effect_size_delta]
+    })
+    return results
 
 import pandas as pd
 from scipy import stats
 import pandas as pd
 from scipy import stats
```

### Comparing `brainsurf-7.0.0/brainsurf/cognitive/cognitive_indexes.py` & `brainsurf-8.0.1/brainsurf/cognitive/cognitive_indexes.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/io/eeg_data.py` & `brainsurf-8.0.1/brainsurf/io/eeg_data.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/machine_learning/eeg_binary_classification.py` & `brainsurf-8.0.1/brainsurf/machine_learning/eeg_binary_classification.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/machine_learning/rnn_module.py` & `brainsurf-8.0.1/brainsurf/machine_learning/rnn_module.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/machine_learning/time_series.py` & `brainsurf-8.0.1/brainsurf/machine_learning/time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/preprocessing/baseline.py` & `brainsurf-8.0.1/brainsurf/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/preprocessing/epoching.py` & `brainsurf-8.0.1/brainsurf/preprocessing/epoching.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/preprocessing/filtering.py` & `brainsurf-8.0.1/brainsurf/preprocessing/filtering.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/utils/performance.py` & `brainsurf-8.0.1/brainsurf/utils/performance.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/visualization/comparative_visualize.py` & `brainsurf-8.0.1/brainsurf/visualization/comparative_visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
- 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy import stats, signal
 from sklearn.metrics import pairwise_distances
 
 class ComparativeVisualizationFactory:
     @staticmethod
```

### Comparing `brainsurf-7.0.0/brainsurf/visualization/eeg_data_visualization.py` & `brainsurf-8.0.1/brainsurf/visualization/eeg_data_visualization.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/visualization/plot_coherence.py` & `brainsurf-8.0.1/brainsurf/visualization/plot_coherence.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ax.set_title('Coherence Plot')
     ax.set_xlabel('Frequency (Hz)')
     ax.set_ylabel('Coherence')
     plt.show()
 
 def visualize_coherence_heatmap(coherence_matrix, channel_labels):
     plt.figure(figsize=(10, 8))
-    sns.heatmap(coherence_matrix, cmap='coolwarm', annot=True, fmt=".2f", xticklabels=channel_labels, yticklabels=channel_labels)
+    sns.heatmap(coherence_matrix, cmap='coolwarm', annot=False, fmt=".2f", xticklabels=channel_labels, yticklabels=channel_labels)
     plt.xlabel('Channels')
     plt.ylabel('Channels')
     plt.title('Coherence Matrix')
     plt.show()
 
 def visualize_coherence_circular(coherence_matrix, channel_labels):
     G = nx.Graph()
```

### Comparing `brainsurf-7.0.0/brainsurf/visualization/plot_correlation.py` & `brainsurf-8.0.1/brainsurf/visualization/plot_correlation.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/visualization/plot_eeg_signal.py` & `brainsurf-8.0.1/brainsurf/visualization/plot_eeg_signal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/visualization/plot_power_spectrum.py` & `brainsurf-8.0.1/brainsurf/visualization/plot_power_spectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     plt.plot(freqs, psd)
     plt.xlabel('Frequency (Hz)')
     plt.ylabel('PSD')
     plt.title('Frequency-Domain EEG Signal')
     plt.show()
     
 
+import matplotlib.pyplot as plt
+
 def visualize_difference_plot(overlapping_df1, overlapping_df2):
     """
     Visualize the difference in overlapping percentage between two conditions/time points using a bar plot.
 
     Args:
     - overlapping_df1 (pandas.DataFrame): DataFrame containing the overlapping percentage values for condition/time point 1.
     - overlapping_df2 (pandas.DataFrame): DataFrame containing the overlapping percentage values for condition/time point 2.
@@ -51,15 +53,14 @@
     difference_df = overlapping_df1 - overlapping_df2
 
     # Calculate the mean difference for each frequency band
     mean_difference = difference_df.mean()
     
     # Plotting the mean difference
     plt.figure(figsize=(10, 6))
-    # mean_difference.plot(kind='line', marker='o')
     mean_difference.plot(kind='bar')
 
     plt.xlabel('Frequency Bands')
     plt.ylabel('Difference in Overlapping Percentage')
     plt.title('Difference in Overlapping Percentage between Conditions/Time Points')
     plt.xticks(rotation=45)
-    plt.show()
+    plt.show()
```

### Comparing `brainsurf-7.0.0/brainsurf/visualization/plot_time_series.py` & `brainsurf-8.0.1/brainsurf/visualization/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf/visualization/plot_topomap.py` & `brainsurf-8.0.1/brainsurf/visualization/plot_topomap.py`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/brainsurf.egg-info/PKG-INFO` & `brainsurf-8.0.1/brainsurf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 7.0.0
+Version: 8.0.1
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-7.0.0/brainsurf.egg-info/SOURCES.txt` & `brainsurf-8.0.1/brainsurf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainsurf-7.0.0/setup.py` & `brainsurf-8.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='brainsurf',
-    version='7.0.0',
+    version='8.0.1',
     description='EEG Signal Processing Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='preethivhiremath',
     author_email='preethivhiremath.vh@gmail.com',
     url='https://github.com/preethihiremath/brainsurf',
     packages=find_packages(),
@@ -17,14 +17,15 @@
         'numpy',
         'scipy',
         'matplotlib',
         'mne',
         'pyabf',
         'nolds',
         'pytest',
+        'pyedflib',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

