# Comparing `tmp/brainsurf-8.0.1.tar.gz` & `tmp/brainsurf-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsurf-8.0.1.tar", last modified: Sat Jun 17 05:52:43 2023, max compression
+gzip compressed data, was "brainsurf-8.0.2.tar", last modified: Sat Jun 17 07:30:03 2023, max compression
```

## Comparing `brainsurf-8.0.1.tar` & `brainsurf-8.0.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.676858 brainsurf-8.0.1/
--rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-8.0.1/LICENSE
--rw-rw-rw-   0        0        0     2391 2023-06-17 05:52:43.674854 brainsurf-8.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-06-09 03:59:51.000000 brainsurf-8.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.482919 brainsurf-8.0.1/brainsurf/
--rw-rw-rw-   0        0        0       70 2023-06-17 05:52:29.000000 brainsurf-8.0.1/brainsurf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.550445 brainsurf-8.0.1/brainsurf/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-8.0.1/brainsurf/analysis/__init__.py
--rw-rw-rw-   0        0        0     3540 2023-06-08 16:28:08.000000 brainsurf-8.0.1/brainsurf/analysis/corelation_analysis.py
--rw-rw-rw-   0        0        0     1756 2023-05-31 17:53:43.000000 brainsurf-8.0.1/brainsurf/analysis/erp_analysis.py
--rw-rw-rw-   0        0        0     1388 2023-06-08 16:30:02.000000 brainsurf-8.0.1/brainsurf/analysis/frequency.py
--rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-8.0.1/brainsurf/analysis/multi_fractal.py
--rw-rw-rw-   0        0        0     6144 2023-06-14 19:14:17.000000 brainsurf-8.0.1/brainsurf/analysis/power_spectrum.py
--rw-rw-rw-   0        0        0     3071 2023-06-08 22:36:24.000000 brainsurf-8.0.1/brainsurf/analysis/stats_analysis.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.561451 brainsurf-8.0.1/brainsurf/cognitive/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-8.0.1/brainsurf/cognitive/__init__.py
--rw-rw-rw-   0        0        0    14134 2023-06-09 04:31:07.000000 brainsurf-8.0.1/brainsurf/cognitive/cognitive_comparision.py
--rw-rw-rw-   0        0        0     4202 2023-06-08 16:35:05.000000 brainsurf-8.0.1/brainsurf/cognitive/cognitive_indexes.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.585448 brainsurf-8.0.1/brainsurf/io/
--rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-8.0.1/brainsurf/io/__init__.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-8.0.1/brainsurf/io/csv.py
--rw-rw-rw-   0        0        0      167 2023-06-08 16:03:18.000000 brainsurf-8.0.1/brainsurf/io/df.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-8.0.1/brainsurf/io/edf.py
--rw-rw-rw-   0        0        0    13064 2023-06-09 01:08:35.000000 brainsurf-8.0.1/brainsurf/io/eeg_data.py
--rw-rw-rw-   0        0        0      213 2023-06-03 12:32:49.000000 brainsurf-8.0.1/brainsurf/io/mff.py
--rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-8.0.1/brainsurf/io/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.599469 brainsurf-8.0.1/brainsurf/machine_learning/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-8.0.1/brainsurf/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-8.0.1/brainsurf/machine_learning/eeg_binary_classification.py
--rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-8.0.1/brainsurf/machine_learning/rnn_module.py
--rw-rw-rw-   0        0        0     2813 2023-05-31 18:17:21.000000 brainsurf-8.0.1/brainsurf/machine_learning/time_series.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.616853 brainsurf-8.0.1/brainsurf/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-8.0.1/brainsurf/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-06-09 07:50:22.000000 brainsurf-8.0.1/brainsurf/preprocessing/artifact_removal.py
--rw-rw-rw-   0        0        0     3877 2023-06-08 16:16:32.000000 brainsurf-8.0.1/brainsurf/preprocessing/baseline.py
--rw-rw-rw-   0        0        0     2141 2023-06-08 16:13:30.000000 brainsurf-8.0.1/brainsurf/preprocessing/epoching.py
--rw-rw-rw-   0        0        0     5481 2023-06-08 17:33:30.000000 brainsurf-8.0.1/brainsurf/preprocessing/filtering.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.628856 brainsurf-8.0.1/brainsurf/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-8.0.1/brainsurf/utils/__init__.py
--rw-rw-rw-   0        0        0     3010 2023-06-17 05:50:43.000000 brainsurf-8.0.1/brainsurf/utils/data.py
--rw-rw-rw-   0        0        0     1442 2023-06-08 16:23:07.000000 brainsurf-8.0.1/brainsurf/utils/performance.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.671861 brainsurf-8.0.1/brainsurf/visualization/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-8.0.1/brainsurf/visualization/__init__.py
--rw-rw-rw-   0        0        0    10690 2023-06-15 18:13:21.000000 brainsurf-8.0.1/brainsurf/visualization/comparative_visualize.py
--rw-rw-rw-   0        0        0     3483 2023-05-30 19:11:59.000000 brainsurf-8.0.1/brainsurf/visualization/eeg_data_visualization.py
--rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-8.0.1/brainsurf/visualization/plot_cluster.py
--rw-rw-rw-   0        0        0     1806 2023-06-09 05:03:08.000000 brainsurf-8.0.1/brainsurf/visualization/plot_coherence.py
--rw-rw-rw-   0        0        0     4274 2023-06-08 17:59:04.000000 brainsurf-8.0.1/brainsurf/visualization/plot_correlation.py
--rw-rw-rw-   0        0        0      555 2023-06-06 16:53:17.000000 brainsurf-8.0.1/brainsurf/visualization/plot_eeg_signal.py
--rw-rw-rw-   0        0        0      262 2023-06-08 17:56:49.000000 brainsurf-8.0.1/brainsurf/visualization/plot_heatmap.py
--rw-rw-rw-   0        0        0     2061 2023-06-14 18:18:48.000000 brainsurf-8.0.1/brainsurf/visualization/plot_power_spectrum.py
--rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-8.0.1/brainsurf/visualization/plot_spectogram.py
--rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-8.0.1/brainsurf/visualization/plot_time_series.py
--rw-rw-rw-   0        0        0      566 2023-06-08 16:41:38.000000 brainsurf-8.0.1/brainsurf/visualization/plot_topomap.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:52:43.523456 brainsurf-8.0.1/brainsurf.egg-info/
--rw-rw-rw-   0        0        0     2391 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-17 05:52:43.000000 brainsurf-8.0.1/brainsurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 05:52:43.676858 brainsurf-8.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-06-17 05:52:34.000000 brainsurf-8.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.694925 brainsurf-8.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-8.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2391 2023-06-17 07:30:03.693927 brainsurf-8.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-06-09 03:59:51.000000 brainsurf-8.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.534638 brainsurf-8.0.2/brainsurf/
+-rw-rw-rw-   0        0        0       70 2023-06-17 07:29:52.000000 brainsurf-8.0.2/brainsurf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.594184 brainsurf-8.0.2/brainsurf/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-8.0.2/brainsurf/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-06-08 16:28:08.000000 brainsurf-8.0.2/brainsurf/analysis/corelation_analysis.py
+-rw-rw-rw-   0        0        0     1756 2023-05-31 17:53:43.000000 brainsurf-8.0.2/brainsurf/analysis/erp_analysis.py
+-rw-rw-rw-   0        0        0     1388 2023-06-08 16:30:02.000000 brainsurf-8.0.2/brainsurf/analysis/frequency.py
+-rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-8.0.2/brainsurf/analysis/multi_fractal.py
+-rw-rw-rw-   0        0        0     6144 2023-06-14 19:14:17.000000 brainsurf-8.0.2/brainsurf/analysis/power_spectrum.py
+-rw-rw-rw-   0        0        0     3071 2023-06-08 22:36:24.000000 brainsurf-8.0.2/brainsurf/analysis/stats_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.603187 brainsurf-8.0.2/brainsurf/cognitive/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-8.0.2/brainsurf/cognitive/__init__.py
+-rw-rw-rw-   0        0        0    14134 2023-06-09 04:31:07.000000 brainsurf-8.0.2/brainsurf/cognitive/cognitive_comparision.py
+-rw-rw-rw-   0        0        0     4202 2023-06-08 16:35:05.000000 brainsurf-8.0.2/brainsurf/cognitive/cognitive_indexes.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.623379 brainsurf-8.0.2/brainsurf/io/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-8.0.2/brainsurf/io/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-8.0.2/brainsurf/io/csv.py
+-rw-rw-rw-   0        0        0      167 2023-06-08 16:03:18.000000 brainsurf-8.0.2/brainsurf/io/df.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-8.0.2/brainsurf/io/edf.py
+-rw-rw-rw-   0        0        0    13064 2023-06-09 01:08:35.000000 brainsurf-8.0.2/brainsurf/io/eeg_data.py
+-rw-rw-rw-   0        0        0      213 2023-06-03 12:32:49.000000 brainsurf-8.0.2/brainsurf/io/mff.py
+-rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-8.0.2/brainsurf/io/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.633391 brainsurf-8.0.2/brainsurf/machine_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-8.0.2/brainsurf/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-8.0.2/brainsurf/machine_learning/eeg_binary_classification.py
+-rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-8.0.2/brainsurf/machine_learning/rnn_module.py
+-rw-rw-rw-   0        0        0     2813 2023-05-31 18:17:21.000000 brainsurf-8.0.2/brainsurf/machine_learning/time_series.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.647393 brainsurf-8.0.2/brainsurf/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-8.0.2/brainsurf/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-09 07:50:22.000000 brainsurf-8.0.2/brainsurf/preprocessing/artifact_removal.py
+-rw-rw-rw-   0        0        0     3877 2023-06-08 16:16:32.000000 brainsurf-8.0.2/brainsurf/preprocessing/baseline.py
+-rw-rw-rw-   0        0        0     2141 2023-06-08 16:13:30.000000 brainsurf-8.0.2/brainsurf/preprocessing/epoching.py
+-rw-rw-rw-   0        0        0     5481 2023-06-08 17:33:30.000000 brainsurf-8.0.2/brainsurf/preprocessing/filtering.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.655407 brainsurf-8.0.2/brainsurf/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-8.0.2/brainsurf/utils/__init__.py
+-rw-rw-rw-   0        0        0     3010 2023-06-17 05:50:43.000000 brainsurf-8.0.2/brainsurf/utils/data.py
+-rw-rw-rw-   0        0        0     1442 2023-06-08 16:23:07.000000 brainsurf-8.0.2/brainsurf/utils/performance.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.690919 brainsurf-8.0.2/brainsurf/visualization/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-8.0.2/brainsurf/visualization/__init__.py
+-rw-rw-rw-   0        0        0    10690 2023-06-15 18:13:21.000000 brainsurf-8.0.2/brainsurf/visualization/comparative_visualize.py
+-rw-rw-rw-   0        0        0     3483 2023-05-30 19:11:59.000000 brainsurf-8.0.2/brainsurf/visualization/eeg_data_visualization.py
+-rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-8.0.2/brainsurf/visualization/plot_cluster.py
+-rw-rw-rw-   0        0        0     1806 2023-06-09 05:03:08.000000 brainsurf-8.0.2/brainsurf/visualization/plot_coherence.py
+-rw-rw-rw-   0        0        0     4274 2023-06-08 17:59:04.000000 brainsurf-8.0.2/brainsurf/visualization/plot_correlation.py
+-rw-rw-rw-   0        0        0      555 2023-06-06 16:53:17.000000 brainsurf-8.0.2/brainsurf/visualization/plot_eeg_signal.py
+-rw-rw-rw-   0        0        0      262 2023-06-08 17:56:49.000000 brainsurf-8.0.2/brainsurf/visualization/plot_heatmap.py
+-rw-rw-rw-   0        0        0     5799 2023-06-17 07:26:10.000000 brainsurf-8.0.2/brainsurf/visualization/plot_power_spectrum.py
+-rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-8.0.2/brainsurf/visualization/plot_spectogram.py
+-rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-8.0.2/brainsurf/visualization/plot_time_series.py
+-rw-rw-rw-   0        0        0      566 2023-06-08 16:41:38.000000 brainsurf-8.0.2/brainsurf/visualization/plot_topomap.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:30:03.576200 brainsurf-8.0.2/brainsurf.egg-info/
+-rw-rw-rw-   0        0        0     2391 2023-06-17 07:30:03.000000 brainsurf-8.0.2/brainsurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2023-06-17 07:30:03.000000 brainsurf-8.0.2/brainsurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 07:30:03.000000 brainsurf-8.0.2/brainsurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-17 07:30:03.000000 brainsurf-8.0.2/brainsurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-17 07:30:03.000000 brainsurf-8.0.2/brainsurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 07:30:03.695917 brainsurf-8.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-06-17 07:29:56.000000 brainsurf-8.0.2/setup.py
```

### Comparing `brainsurf-8.0.1/LICENSE` & `brainsurf-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/PKG-INFO` & `brainsurf-8.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 8.0.1
+Version: 8.0.2
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-8.0.1/README.md` & `brainsurf-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/analysis/corelation_analysis.py` & `brainsurf-8.0.2/brainsurf/analysis/corelation_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/analysis/erp_analysis.py` & `brainsurf-8.0.2/brainsurf/analysis/erp_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/analysis/frequency.py` & `brainsurf-8.0.2/brainsurf/analysis/frequency.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/analysis/multi_fractal.py` & `brainsurf-8.0.2/brainsurf/analysis/multi_fractal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/analysis/power_spectrum.py` & `brainsurf-8.0.2/brainsurf/analysis/power_spectrum.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/analysis/stats_analysis.py` & `brainsurf-8.0.2/brainsurf/analysis/stats_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/cognitive/cognitive_comparision.py` & `brainsurf-8.0.2/brainsurf/cognitive/cognitive_comparision.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/cognitive/cognitive_indexes.py` & `brainsurf-8.0.2/brainsurf/cognitive/cognitive_indexes.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/io/eeg_data.py` & `brainsurf-8.0.2/brainsurf/io/eeg_data.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/machine_learning/eeg_binary_classification.py` & `brainsurf-8.0.2/brainsurf/machine_learning/eeg_binary_classification.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/machine_learning/rnn_module.py` & `brainsurf-8.0.2/brainsurf/machine_learning/rnn_module.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/machine_learning/time_series.py` & `brainsurf-8.0.2/brainsurf/machine_learning/time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/preprocessing/artifact_removal.py` & `brainsurf-8.0.2/brainsurf/preprocessing/artifact_removal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/preprocessing/baseline.py` & `brainsurf-8.0.2/brainsurf/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/preprocessing/epoching.py` & `brainsurf-8.0.2/brainsurf/preprocessing/epoching.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/preprocessing/filtering.py` & `brainsurf-8.0.2/brainsurf/preprocessing/filtering.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/utils/data.py` & `brainsurf-8.0.2/brainsurf/utils/data.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/utils/performance.py` & `brainsurf-8.0.2/brainsurf/utils/performance.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/comparative_visualize.py` & `brainsurf-8.0.2/brainsurf/visualization/comparative_visualize.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/eeg_data_visualization.py` & `brainsurf-8.0.2/brainsurf/visualization/eeg_data_visualization.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/plot_coherence.py` & `brainsurf-8.0.2/brainsurf/visualization/plot_coherence.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/plot_correlation.py` & `brainsurf-8.0.2/brainsurf/visualization/plot_correlation.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/plot_eeg_signal.py` & `brainsurf-8.0.2/brainsurf/visualization/plot_eeg_signal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/plot_time_series.py` & `brainsurf-8.0.2/brainsurf/visualization/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf/visualization/plot_topomap.py` & `brainsurf-8.0.2/brainsurf/visualization/plot_topomap.py`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/brainsurf.egg-info/PKG-INFO` & `brainsurf-8.0.2/brainsurf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 8.0.1
+Version: 8.0.2
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-8.0.1/brainsurf.egg-info/SOURCES.txt` & `brainsurf-8.0.2/brainsurf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainsurf-8.0.1/setup.py` & `brainsurf-8.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='brainsurf',
-    version='8.0.1',
+    version='8.0.2',
     description='EEG Signal Processing Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='preethivhiremath',
     author_email='preethivhiremath.vh@gmail.com',
     url='https://github.com/preethihiremath/brainsurf',
     packages=find_packages(),
```

