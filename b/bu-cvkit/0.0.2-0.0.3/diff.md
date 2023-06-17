# Comparing `tmp/bu_cvkit-0.0.2.tar.gz` & `tmp/bu_cvkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu_cvkit-0.0.2.tar", last modified: Wed Apr  5 18:31:43 2023, max compression
+gzip compressed data, was "bu_cvkit-0.0.3.tar", last modified: Sat Jun 17 05:18:48 2023, max compression
```

## Comparing `bu_cvkit-0.0.2.tar` & `bu_cvkit-0.0.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.910382 bu_cvkit-0.0.2/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1068 2023-04-05 17:26:10.000000 bu_cvkit-0.0.2/LICENSE
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      478 2023-04-05 18:31:43.910382 bu_cvkit-0.0.2/PKG-INFO
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.906382 bu_cvkit-0.0.2/bu_cvkit.egg-info/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      478 2023-04-05 18:31:43.000000 bu_cvkit-0.0.2/bu_cvkit.egg-info/PKG-INFO
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2086 2023-04-05 18:31:43.000000 bu_cvkit-0.0.2/bu_cvkit.egg-info/SOURCES.txt
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)        1 2023-04-05 18:31:43.000000 bu_cvkit-0.0.2/bu_cvkit.egg-info/dependency_links.txt
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      138 2023-04-05 18:31:43.000000 bu_cvkit-0.0.2/bu_cvkit.egg-info/requires.txt
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)        6 2023-04-05 18:31:43.000000 bu_cvkit-0.0.2/bu_cvkit.egg-info/top_level.txt
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.906382 bu_cvkit-0.0.2/cvkit/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      482 2023-04-05 16:58:05.000000 bu_cvkit-0.0.2/cvkit/__init__.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.907382 bu_cvkit-0.0.2/cvkit/pose_estimation/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)       58 2023-04-03 17:32:21.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/__init__.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5304 2023-04-03 19:24:04.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/config.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.907382 bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1328 2023-04-03 19:44:11.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/__init__.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     3584 2023-04-03 15:42:52.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/cvkit_datastore.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     9062 2023-03-28 18:07:25.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/datastore_interface.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     6245 2023-04-03 19:36:57.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/deeplabcut_datastore.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5229 2023-03-28 19:28:58.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/flattened_datastore.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.907382 bu_cvkit-0.0.2/cvkit/pose_estimation/metrics/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1362 2023-03-07 20:52:59.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/metrics/mpjpe.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2931 2023-04-03 19:36:39.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/metrics/pck.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.907382 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.908382 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      668 2023-04-03 15:39:09.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/__init__.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2285 2023-04-03 15:39:09.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/distance_statistics_filter.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5015 2023-04-03 17:53:16.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/kalman_filter.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1844 2023-04-03 15:41:30.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/linear_interpolation.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1435 2023-04-03 15:39:09.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/median_distance_culling.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1345 2023-04-03 15:39:09.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/moving_average.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1519 2023-04-03 15:37:36.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/region_filter_2d.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1388 2023-04-03 15:37:27.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/velocity_filter.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.909382 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      291 2023-04-03 15:42:52.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/__init__.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2694 2023-04-03 17:33:19.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/dlt_deconstruct.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2945 2023-04-03 17:33:45.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/dlt_reconstruct.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2033 2023-04-03 15:41:30.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/generate_velocity_data.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      590 2023-03-28 18:14:55.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/post_prcessor_interface.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.909382 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/util/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      236 2023-04-03 15:42:52.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/util/__init__.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1660 2023-04-03 15:41:30.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/util/cluster_analysis.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      492 2023-04-03 15:41:30.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/util/load_file.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      538 2023-04-03 15:42:52.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/util/save_file.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.909382 bu_cvkit-0.0.2/cvkit/pose_estimation/reconstruction/
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     7004 2023-03-28 20:23:46.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/reconstruction/DLT.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5472 2023-04-03 17:32:41.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/reconstruction/EasyWand_tools.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     5707 2023-03-28 17:55:01.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/skeleton.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     4272 2023-04-05 18:14:23.000000 bu_cvkit-0.0.2/cvkit/pose_estimation/utils.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)       21 2023-03-28 17:54:30.000000 bu_cvkit-0.0.2/cvkit/utils.py
-drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-04-05 18:31:43.910382 bu_cvkit-0.0.2/cvkit/video_readers/
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      926 2023-03-28 18:00:05.000000 bu_cvkit-0.0.2/cvkit/video_readers/__init__.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     2267 2023-04-03 15:42:51.000000 bu_cvkit-0.0.2/cvkit/video_readers/cv2_reader.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     2535 2023-04-03 15:42:52.000000 bu_cvkit-0.0.2/cvkit/video_readers/deffcode_reader.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     1224 2023-03-28 18:04:41.000000 bu_cvkit-0.0.2/cvkit/video_readers/image_sequence_reader.py
--rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     1200 2023-04-03 15:42:52.000000 bu_cvkit-0.0.2/cvkit/video_readers/video_reader_interface.py
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      748 2023-04-05 18:28:57.000000 bu_cvkit-0.0.2/pyproject.toml
--rw-r--r--   0 mahirp   (372709) cs-grad   (3935)       38 2023-04-05 18:31:43.910382 bu_cvkit-0.0.2/setup.cfg
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.791781 bu_cvkit-0.0.3/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1068 2023-04-05 17:26:10.000000 bu_cvkit-0.0.3/LICENSE
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      484 2023-06-17 05:18:48.790781 bu_cvkit-0.0.3/PKG-INFO
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.787781 bu_cvkit-0.0.3/bu_cvkit.egg-info/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      484 2023-06-17 05:18:48.000000 bu_cvkit-0.0.3/bu_cvkit.egg-info/PKG-INFO
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2034 2023-06-17 05:18:48.000000 bu_cvkit-0.0.3/bu_cvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)        1 2023-06-17 05:18:48.000000 bu_cvkit-0.0.3/bu_cvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      138 2023-06-17 05:18:48.000000 bu_cvkit-0.0.3/bu_cvkit.egg-info/requires.txt
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)        6 2023-06-17 05:18:48.000000 bu_cvkit-0.0.3/bu_cvkit.egg-info/top_level.txt
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.787781 bu_cvkit-0.0.3/cvkit/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     3992 2023-06-16 11:23:47.000000 bu_cvkit-0.0.3/cvkit/__init__.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.787781 bu_cvkit-0.0.3/cvkit/pose_estimation/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)       58 2023-04-03 17:32:21.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/__init__.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5794 2023-06-16 21:10:49.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/config.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.788781 bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1328 2023-04-03 19:44:11.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/__init__.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     3585 2023-06-16 17:41:47.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/cvkit_datastore.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)    14630 2023-06-16 22:19:26.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/datastore_interface.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     6245 2023-06-16 17:41:47.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/deeplabcut_datastore.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5230 2023-06-16 17:41:47.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/flattened_datastore.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.788781 bu_cvkit-0.0.3/cvkit/pose_estimation/metrics/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1362 2023-03-07 20:52:59.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/metrics/mpjpe.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2932 2023-04-07 15:32:11.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/metrics/pck.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.788781 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.789781 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      633 2023-05-30 00:49:16.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/__init__.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     3039 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/distance_statistics_filter.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5686 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/kalman_filter.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2349 2023-06-15 22:34:35.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/linear_interpolation.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1830 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/median_distance_culling.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1826 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/moving_average.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1851 2023-06-15 21:10:10.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/region_filter_2d.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2269 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/velocity_filter.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.789781 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      276 2023-05-30 00:49:16.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/__init__.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     3006 2023-06-16 12:55:26.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/dlt_deconstruct.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     3587 2023-06-16 21:10:48.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/dlt_reconstruct.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2646 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/generate_velocity_data.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2550 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/processor_interface.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.790781 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/util/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      221 2023-05-30 00:49:16.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/util/__init__.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2073 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/util/cluster_analysis.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     1203 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/util/load_file.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      772 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/processors/util/save_file.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.790781 bu_cvkit-0.0.3/cvkit/pose_estimation/reconstruction/
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     7014 2023-05-30 01:22:14.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/reconstruction/DLT.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     5695 2023-06-16 12:48:38.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/reconstruction/EasyWand_tools.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     9359 2023-06-17 01:33:36.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/skeleton.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     5351 2023-06-16 13:42:02.000000 bu_cvkit-0.0.3/cvkit/pose_estimation/utils.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)       21 2023-03-28 17:54:30.000000 bu_cvkit-0.0.3/cvkit/utils.py
+drwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)        0 2023-06-17 05:18:48.790781 bu_cvkit-0.0.3/cvkit/video_readers/
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      926 2023-03-28 18:00:05.000000 bu_cvkit-0.0.3/cvkit/video_readers/__init__.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     2318 2023-06-16 11:08:01.000000 bu_cvkit-0.0.3/cvkit/video_readers/cv2_reader.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)     2634 2023-06-16 12:34:24.000000 bu_cvkit-0.0.3/cvkit/video_readers/decord_reader.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     2503 2023-05-17 18:04:22.000000 bu_cvkit-0.0.3/cvkit/video_readers/deffcode_reader.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     2268 2023-06-16 11:08:00.000000 bu_cvkit-0.0.3/cvkit/video_readers/image_sequence_reader.py
+-rwxr-xr-x   0 mahirp   (372709) cs-grad   (3935)     1200 2023-04-03 15:42:52.000000 bu_cvkit-0.0.3/cvkit/video_readers/video_reader_interface.py
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)      789 2023-06-17 05:18:39.000000 bu_cvkit-0.0.3/pyproject.toml
+-rw-r--r--   0 mahirp   (372709) cs-grad   (3935)       38 2023-06-17 05:18:48.791781 bu_cvkit-0.0.3/setup.cfg
```

### Comparing `bu_cvkit-0.0.2/LICENSE` & `bu_cvkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bu_cvkit-0.0.2/bu_cvkit.egg-info/SOURCES.txt` & `bu_cvkit-0.0.3/bu_cvkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,32 @@
 cvkit/pose_estimation/data_readers/__init__.py
 cvkit/pose_estimation/data_readers/cvkit_datastore.py
 cvkit/pose_estimation/data_readers/datastore_interface.py
 cvkit/pose_estimation/data_readers/deeplabcut_datastore.py
 cvkit/pose_estimation/data_readers/flattened_datastore.py
 cvkit/pose_estimation/metrics/mpjpe.py
 cvkit/pose_estimation/metrics/pck.py
-cvkit/pose_estimation/post_processors/post_prcessor_interface.py
-cvkit/pose_estimation/post_processors/filter/__init__.py
-cvkit/pose_estimation/post_processors/filter/distance_statistics_filter.py
-cvkit/pose_estimation/post_processors/filter/kalman_filter.py
-cvkit/pose_estimation/post_processors/filter/linear_interpolation.py
-cvkit/pose_estimation/post_processors/filter/median_distance_culling.py
-cvkit/pose_estimation/post_processors/filter/moving_average.py
-cvkit/pose_estimation/post_processors/filter/region_filter_2d.py
-cvkit/pose_estimation/post_processors/filter/velocity_filter.py
-cvkit/pose_estimation/post_processors/generative/__init__.py
-cvkit/pose_estimation/post_processors/generative/dlt_deconstruct.py
-cvkit/pose_estimation/post_processors/generative/dlt_reconstruct.py
-cvkit/pose_estimation/post_processors/generative/generate_velocity_data.py
-cvkit/pose_estimation/post_processors/util/__init__.py
-cvkit/pose_estimation/post_processors/util/cluster_analysis.py
-cvkit/pose_estimation/post_processors/util/load_file.py
-cvkit/pose_estimation/post_processors/util/save_file.py
+cvkit/pose_estimation/processors/processor_interface.py
+cvkit/pose_estimation/processors/filter/__init__.py
+cvkit/pose_estimation/processors/filter/distance_statistics_filter.py
+cvkit/pose_estimation/processors/filter/kalman_filter.py
+cvkit/pose_estimation/processors/filter/linear_interpolation.py
+cvkit/pose_estimation/processors/filter/median_distance_culling.py
+cvkit/pose_estimation/processors/filter/moving_average.py
+cvkit/pose_estimation/processors/filter/region_filter_2d.py
+cvkit/pose_estimation/processors/filter/velocity_filter.py
+cvkit/pose_estimation/processors/generative/__init__.py
+cvkit/pose_estimation/processors/generative/dlt_deconstruct.py
+cvkit/pose_estimation/processors/generative/dlt_reconstruct.py
+cvkit/pose_estimation/processors/generative/generate_velocity_data.py
+cvkit/pose_estimation/processors/util/__init__.py
+cvkit/pose_estimation/processors/util/cluster_analysis.py
+cvkit/pose_estimation/processors/util/load_file.py
+cvkit/pose_estimation/processors/util/save_file.py
 cvkit/pose_estimation/reconstruction/DLT.py
 cvkit/pose_estimation/reconstruction/EasyWand_tools.py
 cvkit/video_readers/__init__.py
 cvkit/video_readers/cv2_reader.py
+cvkit/video_readers/decord_reader.py
 cvkit/video_readers/deffcode_reader.py
 cvkit/video_readers/image_sequence_reader.py
 cvkit/video_readers/video_reader_interface.py
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/config.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,19 @@
 
 class AnnotationConfig:
     def __init__(self, data_dictionary):
         self.view = data_dictionary.get('view', None)
         self.annotation_file = data_dictionary['annotation_file']
         self.annotation_file_flavor = data_dictionary['annotation_file_flavor']
         self.video_file = data_dictionary['video_file']
-        assert os.path.isfile(self.video_file)
+        try:
+            assert os.path.isfile(self.video_file)
+        except:
+            print(self.video_file, "not found!")
+            exit()
         self.video_reader = data_dictionary['video_reader']
 
     def export_dict(self):
         return {'view': self.view,
                 'annotation_file': self.annotation_file,
                 'annotation_file_flavor': self.annotation_file_flavor,
                 'video_file': self.video_file,
@@ -54,14 +58,19 @@
         self.path = path
         self.data_dictionary = yml.safe_load(open(path, 'r'))
         assert 0 <= DEFAULT_THRESHOLD < 1.0
         self.project_name = self.data_dictionary.get('name', 'unnamed')
         self.output_folder = self.data_dictionary['output_folder']
         assert os.path.exists(self.output_folder)
         self.threshold = float(self.data_dictionary['Reconstruction'].get('threshold', DEFAULT_THRESHOLD))
+        self.axis_rotation_3D = np.array(
+            self.data_dictionary['Reconstruction'].get('axis_rotation_3D', np.array([1, 1, 1])))
+        if np.any(np.abs(self.axis_rotation_3D) != 1):
+            print(f"Resetting {self.axis_rotation_3D} to [1,1,1]")
+            self.axis_rotation_3D = np.array([1, 1, 1])
         self.body_parts = self.data_dictionary['body_parts']
         self.num_parts = len(self.body_parts)
         self.skeleton = self.data_dictionary['skeleton']
         self.colors = list(self.data_dictionary.get('colors', []))
         self.framerate = self.data_dictionary['Reconstruction']['framerate']
         self.annotation_views = {}
         if 'annotation' in self.data_dictionary:
@@ -93,15 +102,16 @@
                 'Reconstruction': {
                     'threshold': self.threshold,
                     'scale': self.scale,
                     'framerate': self.framerate,
                     'rotation_matrix': self.rotation_matrix.tolist(),
                     'translation_matrix': self.translation_matrix.tolist(),
                     'reconstruction_algorithm': self.reconstruction_algorithm,
-                    'computed_scale': float(self.computed_scale)
+                    'computed_scale': float(self.computed_scale),
+                    'axis_rotation_3D': self.axis_rotation_3D.tolist()
                 }
                 }
 
 
 def save_config(path, data_dict):
     out_file = ''
     for key in data_dict:
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/__init__.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/cvkit_datastore.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/cvkit_datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.data.sort_index(inplace=True)
         self.data.to_csv(path, index=False, sep=self.SEP)
 
     def delete_part(self, index, name, force_remove=False):
         if force_remove or index in self.data.index:
             self.data.loc[index, name] = pd.NA
 
-    def set_behaviour(self, index, behaviour: str) -> None:
+    def set_behaviour(self, index, behaviour: list) -> None:
         self.data.loc[index, 'behaviour'] = self.BEHAVIOUR_SEP.join(behaviour)
 
     def get_behaviour(self, index) -> list:
         if index in self.data.index and not pd.isna(self.data.loc[index, 'behaviour']):
             return self.data.loc[index, 'behaviour'].split(self.BEHAVIOUR_SEP)
         else:
             return []
@@ -59,16 +59,16 @@
         for name in self.body_parts:
             part_map[name] = convert_to_numpy(row[name])
             likelihood_map[name] = float(not all(part_map[name] == self.MAGIC_NUMBER))
         behaviour = [] if pd.isna(row['behaviour']) else row['behaviour'].split(self.BEHAVIOUR_SEP)
         return Skeleton(self.body_parts, part_map=part_map, likelihood_map=likelihood_map,
                         behaviour=behaviour)
 
-    def build_part(self, arr, name):
-        pt = convert_to_numpy(arr)
+    def build_part(self, row, name):
+        pt = convert_to_numpy(row)
         return Part(pt, name, float(not all(pt == self.MAGIC_NUMBER)))
 
     def __init__(self, body_parts, path):
         super(CVKitDataStore3D, self).__init__(body_parts, path)
         self.path = path
         if path is not None and os.path.exists(path):
             self.data = pd.read_csv(path, sep=';')
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/deeplabcut_datastore.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/deeplabcut_datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         if not self.data.index.is_monotonic_increasing:
             self.data.sort_index(inplace=True)
 
     def part_iterator(self, part):
         for index, row in self.data.loc[:, (self.scorer, part)].iterrows():
             yield index, self.build_part(row, part)
 
-    def build_part(self, arr, name):
-        return Part([arr['x'], arr['y']], name, arr['likelihood'])
+    def build_part(self, row, name):
+        return Part([row['x'], row['y']], name, row['likelihood'])
 
     def get_part_slice(self, slice_indices: list, name: str) -> np.ndarray:
         return self.data.loc[slice_indices[0]:slice_indices[1] - 1, (self.scorer, name)].apply(
             lambda x: self.build_part(x, name), axis=1).to_numpy()
 
     def set_part_slice(self, slice_indices: list, name: str, data: np.ndarray) -> None:
         self.data.loc[slice_indices[0]:slice_indices[1] - 1, (self.scorer, name, 'x')] = data[:, 0]
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/data_readers/flattened_datastore.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/data_readers/flattened_datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.data.sort_index(inplace=True)
         self.data.to_csv(path, index=False, sep=self.SEP)
 
     def delete_part(self, index, name, force_remove=False):
         if force_remove or index in self.data.index:
             self.data.loc[index, [f"{name}_{i}" for i in range(1, self.DIMENSIONS + 1)]] = pd.NA
 
-    def set_behaviour(self, index, behaviour: str) -> None:
+    def set_behaviour(self, index, behaviour: list) -> None:
         self.data.loc[index, 'behaviour'] = self.BEHAVIOUR_SEP.join(behaviour)
 
     def get_behaviour(self, index) -> list:
         if index in self.data.index and not pd.isna(self.data.loc[index, 'behaviour']):
             return self.data.loc[index, 'behaviour'].split(self.BEHAVIOUR_SEP)
         else:
             return []
@@ -91,16 +91,16 @@
                 part_map[name] = np.array([self.MAGIC_NUMBER] * self.DIMENSIONS)
             likelihood_map[name] = float(not all(part_map[name] == self.MAGIC_NUMBER))
         behaviour = [] if pd.isna(row['behaviour']) else row['behaviour'].split(self.BEHAVIOUR_SEP)
         return Skeleton(self.body_parts, part_map=part_map, likelihood_map=likelihood_map,
                         behaviour=behaviour,
                         dims=self.DIMENSIONS)
 
-    def build_part(self, arr, name):
-        pt = arr.to_numpy()
+    def build_part(self, row, name):
+        pt = row.to_numpy()
         if any(np.isnan(pt)):
             pt = np.array([self.MAGIC_NUMBER] * self.DIMENSIONS)
         return Part(pt, name, float(not all(pt == self.MAGIC_NUMBER)))
 
     def get_header_rows(self):
         header = []
         for part in self.body_parts:
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/metrics/mpjpe.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/metrics/mpjpe.py`

 * *Files identical despite different names*

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/metrics/pck.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/metrics/pck.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 @tf.function
 def distance_map(ref, points):
     return tf.vectorized_map(fn=lambda t: tf.keras.backend.sqrt(1e-9 + tf.reduce_sum(tf.keras.backend.square(ref - t))),
                              elems=points)
 
+
 def build_pck_metric(n_kps, threshold, per_kp=False):
     assert 0. < threshold < 1.0 and n_kps > 0
     if not per_kp:
         @tf.function
         def pck(y_t, y_p):
             # Expected input dimension batch x n_frames x n_keypoints x 3
             # Generate Mask for padded input
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/distance_statistics_filter.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/velocity_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,45 @@
-import numpy as np
-
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
-from cvkit.pose_estimation.utils import compute_distance_matrix
-
-
-class DistanceStatisticsFilter(PostProcessor):
-    PROCESS_NAME = "Distance Statistics Filter"
-
-    def __init__(self, distance_matrix_stats, threshold=0.5, sd_factor=1.25):
-        super(DistanceStatisticsFilter, self).__init__()
-        assert sd_factor >= 0
-        self.distance_matrix_mean = distance_matrix_stats[0]
-        self.distance_matrix_sd = distance_matrix_stats[1] * sd_factor
-        self.threshold = threshold
+from cvkit.pose_estimation.data_readers import initialize_datastore_reader
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
+from cvkit.pose_estimation.utils import magnitude
+
+
+class VelocityFilter(Processor):
+    REQUIRES_STATS = True
+    PROCESSOR_NAME = "Velocity Filter"
+    PROCESSOR_ID = "cvkit_velocity_filter"
+    META_DATA = {
+        'velocity_ds_dict': ProcessorMetaData('Velocity Data Store', ProcessorMetaData.DATA_STORE, serialize=False),
+        'global_config': ProcessorMetaData('Global Config', ProcessorMetaData.GLOBAL_CONFIG),
+        'threshold_velocity': ProcessorMetaData('Velocity Threshold', ProcessorMetaData.FLOAT)}
+    PROCESSOR_SUMMARY = "Filters body parts with velocity higher than the threshold."
+
+    def __init__(self, global_config, velocity_ds_dict, threshold_velocity):
+        super(VelocityFilter, self).__init__()
+        self.global_config = global_config
+        self.velocity_ds_dict = velocity_ds_dict
+        self._velocity_data_store = initialize_datastore_reader(self.global_config.body_parts,
+                                                                self.velocity_ds_dict['path'],
+                                                                self.velocity_ds_dict['type'])
+        self.threshold_velocity = threshold_velocity
 
     def process(self, data_store):
-        self.data_store = data_store
-        self.data_ready = False
-        self.progress = 0
-        body_parts = data_store.body_parts
-        removed_count = [0] * len(data_store.body_parts)
-        for index, skeleton in self.data_store.row_iterator():
-            self.progress = int(index / len(self.data_store) * 100)
-            if self.PRINT and self.progress % 10 == 0:
-                print(f'\r {self.PROCESS_NAME} {self.progress}% complete', end='')
-            distance_matrix = compute_distance_matrix(skeleton)
-            difference = np.absolute(self.distance_matrix_mean - distance_matrix)
-            max_score = len(skeleton) + distance_matrix.trace()
-
-            if max_score == 0:
-                continue
-            scores = np.array([max_score] * len(skeleton))
-            for i in range(len(skeleton)):
-                if distance_matrix[i][i] != -1:
-                    for j in range(len(skeleton)):
-                        if distance_matrix[i][j] != -1 and difference[i][j] < self.distance_matrix_sd[i][j]:
-                            scores[i] -= 1
-            scores = scores / max_score
-            for i, score in enumerate(scores):
-                if distance_matrix[i][i] != -1 and self.threshold < score:
-                    removed_count[i] += 1
-                    data_store.delete_part(index, body_parts[i])
-        self.data_ready = True
-        print("\nremoved: ", {body_parts[k]: removed_count[k] for k in range(len(data_store.body_parts))})
-        self.progress = 100
+        self._data_store = data_store
+        self._data_ready = False
+        self._progress = 0
+        for index in range(len(data_store)):
+            self._progress = int(index / len(self._data_store) * 100)
+            if self.PRINT and self._progress % 10 == 0:
+                print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
+            for body_part in data_store.body_parts:
+                if magnitude(self._velocity_data_store.get_part(index, body_part)) > self.threshold_velocity:
+                    data_store.delete_part(index, body_part, True)
+        if self.PRINT and self._progress % 10 == 0:
+            print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
+        self._data_ready = True
+        self._progress = 100
 
     def get_output(self):
-        if self.data_ready:
-            return self.data_store
+        if self._data_ready:
+            return self._data_store
         else:
             return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/linear_interpolation.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/linear_interpolation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
 
 
-class LinearInterpolationFilter(PostProcessor):
+class LinearInterpolationFilter(Processor):
     REQUIRES_STATS = True
-    PROCESS_NAME = "Linear Interpolation"
+    PROCESSOR_NAME = "Linear Interpolation"
+    PROCESSOR_ID = "cvkit_interpolation"
+    META_DATA = {'target_column': ProcessorMetaData('Target Part', ProcessorMetaData.BODY_PART),
+                 'threshold': ProcessorMetaData('Threshold', ProcessorMetaData.FLOAT, 0.6, 0.0, 1.0),
+                 'max_cluster_size': ProcessorMetaData('Maximum Window Size', ProcessorMetaData.INT, 10, 1)}
+    PROCESSOR_SUMMARY = "Performs linear interpolation to fill missing body parts."
+    DISTRIBUTED = True
 
     def __init__(self, target_column, threshold=0.6, max_cluster_size=10):
-        super(LinearInterpolationFilter, self).__init__(target_column)
+        super(LinearInterpolationFilter, self).__init__()
+        self.target_column = target_column
         self.threshold = threshold
         self.max_cluster_size = max_cluster_size
 
     def process(self, data_store):
-        self.data_store = data_store
-        self.data_ready = False
-        self.progress = 0
-        if not self.data_store.verify_stats():
+        self._data_store = data_store
+        self._data_ready = False
+        self._progress = 0
+        if not self._data_store.verify_stats():
             raise Exception("This process requires data-frame statistics."
                             "\nPlease run ClusterAnalysis before this one")
-        for index, candidate in enumerate(self.data_store.stats.iter_na_clusters(self.target_column)):
-            self.progress = int(index / len(self.data_store) * 100)
-            if candidate['begin'] == 0 or candidate['end'] == len(self.data_store) - 1:
+        for index, candidate in enumerate(self._data_store.stats.iter_na_clusters(self.target_column)):
+            self._progress = int(index / len(self._data_store) * 100)
+            if candidate['begin'] == 0 or candidate['end'] == len(self._data_store) - 1:
                 continue
             if candidate['end'] - candidate['begin'] < self.max_cluster_size:
-                begin = self.data_store.get_part(candidate['begin'] - 1, self.target_column)
-                end = self.data_store.get_part(candidate['end'] + 1, self.target_column)
+                begin = self._data_store.get_part(candidate['begin'] - 1, self.target_column)
+                end = self._data_store.get_part(candidate['end'] + 1, self.target_column)
                 vector = (end - begin) / (candidate['end'] - candidate['begin'] + 2)
                 current = begin + vector
                 current.likelihood = self.threshold
                 for i in range(candidate['begin'], candidate['end'] + 1):
-                    self.data_store.set_part(i, current)
+                    self._data_store.set_part(i, current)
                     current += vector
-        self.data_ready = True
-        self.progress = 100
+        self._data_ready = True
+        self._progress = 100
 
     def get_output(self):
-        if self.data_ready:
-            return self.data_store
+        if self._data_ready:
+            return self._data_store
         else:
             return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/filter/region_filter_2d.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/filter/region_filter_2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
+import numpy as np
 
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
 
-class RegionFilter2D(PostProcessor):
+
+class RegionFilter2D(Processor):
     REQUIRES_STATS = True
-    PROCESS_NAME = "2D Region Filter"
+    PROCESSOR_NAME = "2D Region Filter"
+    PROCESSOR_ID = "cvkit_2d_region_filter"
+    META_DATA = {'uncertainty_regions': ProcessorMetaData('Uncertain Regions', ProcessorMetaData.NUMPY_ARRAY)}
+    PROCESSOR_SUMMARY = "Deletes body parts lying in provided 2D regions of uncertainty."
 
-    def __init__(self, uncertainty_regions: list):
-        super(RegionFilter2D, self).__init__(None)
-        self.uncertainty_region = uncertainty_regions
+    def __init__(self, uncertainty_regions):
+        super(RegionFilter2D, self).__init__()
+        self.uncertainty_regions = uncertainty_regions
 
     def process(self, data_store):
-        self.data_store = data_store
-        self.data_ready = False
-        self.progress = 0
+        self._data_store = data_store
+        self._data_ready = False
+        self._progress = 0
+        uncertainty_regions = np.load(self.uncertainty_regions)
         for index, skeleton in data_store.row_iterator():
-            self.progress = int(index / len(self.data_store) * 100)
-            if self.PRINT and self.progress % 10 == 0:
-                print(f'\r {self.PROCESS_NAME} {self.progress}% complete', end='')
+            self._progress = int(index / len(self._data_store) * 100)
+            if self.PRINT and self._progress % 10 == 0:
+                print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
             for part in data_store.body_parts:
-                for uncertainty_region in self.uncertainty_regions:
+                for uncertainty_region in uncertainty_regions:
                     if uncertainty_region[0][0] < skeleton[part][0] < uncertainty_region[0][1] and \
                             uncertainty_region[1][
                                 0] < skeleton[part][1] < uncertainty_region[1][1]:
                         data_store.delete_part(index, part, force_remove=True)
                         break
-        if self.PRINT and self.progress % 10 == 0:
-            print(f'\r {self.PROCESS_NAME} {self.progress}% complete', end='')
-        self.data_ready = True
-        self.progress = 100
+        if self.PRINT and self._progress % 10 == 0:
+            print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
+        self._data_ready = True
+        self._progress = 100
 
     def get_output(self):
-        if self.data_ready:
-            return self.data_store
+        if self._data_ready:
+            return self._data_store
         else:
             return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/dlt_deconstruct.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/dlt_deconstruct.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 import os
 
 import numpy as np
 
-from cvkit.pose_estimation.config import PoseEstimationConfig
 from cvkit.pose_estimation import Part
+from cvkit.pose_estimation.config import PoseEstimationConfig
 from cvkit.pose_estimation.data_readers import DeeplabcutDataStore
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
 from cvkit.pose_estimation.reconstruction.DLT import DLTdecon
 from cvkit.pose_estimation.utils import rotate
 
 
-class DLTDeconstruction(PostProcessor):
-    PROCESS_NAME = "Deconstruction Process"
-
-    def __init__(self, global_config: PoseEstimationConfig, target_views, scale, file_prefix=None):
-        super(DLTDeconstruction, self).__init__(None)
-        self.body_parts = global_config.body_parts
-        self.dlt_coefficients = np.array([global_config.views[view].dlt_coefficients for view in target_views])
+class DLTDeconstruction(Processor):
+    PROCESSOR_NAME = "Deconstruction Process"
+    PROCESSOR_ID = "cvkit_3d_deconstruct"
+    META_DATA = {'global_config': ProcessorMetaData('Global Config', ProcessorMetaData.GLOBAL_CONFIG),
+                 'target_views': ProcessorMetaData('Target Views', ProcessorMetaData.VIEWS),
+                 'file_prefix': ProcessorMetaData('File Prefix', ProcessorMetaData.TEXT)}
+    PROCESSOR_SUMMARY = "Re-projects 3D data back to target 2D views."
+
+    def __init__(self, global_config: PoseEstimationConfig, target_views, file_prefix=None):
+        super(DLTDeconstruction, self).__init__()
+        self.global_config = global_config
         self.target_views = target_views
-        self.rotation_matrix = np.linalg.inv(np.array(global_config.rotation_matrix))
-        assert self.rotation_matrix.shape == (3, 3)
-        self.scale = scale
-        self.translation_matrix = np.array(global_config.translation_matrix) * self.scale
         self.file_prefix = file_prefix
         if file_prefix is not None:
             self.file_prefix = os.path.join(global_config.output_folder, file_prefix)
-        assert self.translation_matrix.shape == (3,)
 
     def process(self, data_store):
         out_files = [DeeplabcutDataStore(data_store.body_parts,
                                          f'{data_store.base_file_path if self.file_prefix is None else self.file_prefix}_{target_view}.csv')
                      for
                      target_view in self.target_views]
-        self.data_ready = False
-        self.progress = 0
+        dlt_coefficients = np.array([self.global_config.views[view].dlt_coefficients for view in self.target_views])
+        rotation_matrix = np.linalg.inv(np.array(self.global_config.rotation_matrix))
+        scale = self.global_config.computed_scale
+        translation_matrix = np.array(self.global_config.translation_matrix) * scale
+        self._data_ready = False
+        self._progress = 0
         for index, skeleton in data_store.row_iterator():
-            self.progress = int(index / len(data_store) * 100)
-            if self.PRINT and self.progress % 10 == 0:
-                print(f'\r{self.progress}% complete', end='')
+            self._progress = int(index / len(data_store) * 100)
+            if self.PRINT and self._progress % 10 == 0:
+                print(f'\r{self._progress}% complete', end='')
             for part in data_store.body_parts:
                 if skeleton[part] > 0:
-                    raw_part_3d = rotate(np.array(skeleton[part]) - self.translation_matrix, self.rotation_matrix,
-                                         self.scale, True)
-                    parts_2d = np.round(DLTdecon(self.dlt_coefficients, raw_part_3d, 3, len(self.target_views)))[0,
+                    raw_part_3d = rotate(np.array(skeleton[part]) - translation_matrix, rotation_matrix,
+                                         scale, True, multiplier=[1, 1, -1])
+                    parts_2d = np.round(DLTdecon(dlt_coefficients, raw_part_3d, 3, len(self.target_views)))[0,
                                :].reshape(len(self.target_views), 2)
                     for part_2d, data_store_2d in zip(parts_2d, out_files):
                         data_store_2d.set_part(index, Part(part_2d, part, 1.0))
-        self.progress = 100
+        self._progress = 100
         for file in out_files:
             file.save_file()
-        self.data_ready = True
+        self._data_ready = True
 
     def get_output(self):
         return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/dlt_reconstruct.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/dlt_reconstruct.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 import numpy as np
 
-from cvkit.pose_estimation.config import PoseEstimationConfig
 from cvkit.pose_estimation import Skeleton
+from cvkit.pose_estimation.config import PoseEstimationConfig
 from cvkit.pose_estimation.data_readers.cvkit_datastore import CVKitDataStore3D
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
 from cvkit.pose_estimation.reconstruction.DLT import DLTrecon
 from cvkit.pose_estimation.utils import rotate
 
 
-class DLTReconstruction(PostProcessor):
-    PROCESS_NAME = "Reconstruction"
-
-    def __init__(self, global_config: PoseEstimationConfig, source_views, data_readers, threshold,
-                 reconstruction_algorithm,
-                 scale):
-        super(DLTReconstruction, self).__init__(None)
-        self.body_parts = global_config.body_parts
+class DLTReconstruction(Processor):
+    PROCESSOR_NAME = "Reconstruction"
+    PROCESSOR_ID = "cvkit_3d_reconstruct"
+    META_DATA = {'global_config': ProcessorMetaData('Global Config', ProcessorMetaData.GLOBAL_CONFIG),
+                 'source_views': ProcessorMetaData('Source Views', ProcessorMetaData.VIEWS),
+                 'data_readers': ProcessorMetaData('DataReaders', ProcessorMetaData.FILE_MAP),
+                 'file_prefix': ProcessorMetaData('File Prefix', ProcessorMetaData.TEXT),
+                 'threshold': ProcessorMetaData('Threshold', ProcessorMetaData.FLOAT, 0.6, 0.0, 1.0)}
+    PROCESSOR_SUMMARY = "Performs 3D reconstruction from selected source views."
+
+    def __init__(self, global_config: PoseEstimationConfig, source_views, data_readers, threshold):
+        super(DLTReconstruction, self).__init__()
+        self.global_config = global_config
         self.threshold = threshold
-        self.data_readers = data_readers
-        self.dlt_coefficients = np.array([global_config.views[view].dlt_coefficients for view in source_views])
-        self.reconstruction_algorithm = reconstruction_algorithm
-        self.rotation_matrix = np.array(global_config.rotation_matrix)
-        assert self.rotation_matrix.shape == (3, 3)
-        self.scale = scale
-        self.translation_matrix = np.array(global_config.translation_matrix) * self.scale
-        assert self.translation_matrix.shape == (3,)
-        self.out_csv=None
+        self.source_views = source_views
+        self.data_readers = [data_readers[source_view] for source_view in source_views]
+        self._out_csv = None
 
     def process(self, data_store):
-        self.out_csv = CVKitDataStore3D(self.body_parts, None)
+        self._out_csv = CVKitDataStore3D(self.global_config.body_parts, None)
+        dlt_coefficients = np.array([self.global_config.views[view].dlt_coefficients for view in self.source_views])
+        rotation_matrix = np.array(self.global_config.rotation_matrix)
+        scale = self.global_config.computed_scale
+        translation_matrix = np.array(self.global_config.translation_matrix) * scale
         length = len(min(self.data_readers, key=lambda x: len(x)))
-        self.data_ready = False
-        self.progress = 0
+        self._data_ready = False
+        self._progress = 0
         for iterator in range(length):
-            self.progress = int(iterator / length * 100)
+            self._progress = int(iterator / length * 100)
             skeleton_2D = [reader.get_skeleton(iterator) for reader in self.data_readers]
             recon_data = {}
             prob_data = {}
-            for name in self.body_parts:
+            for name in self.global_config.body_parts:
                 subset = [sk[name] for sk in skeleton_2D]
-                dlt_subset = self.dlt_coefficients
+                dlt_subset = dlt_coefficients.copy()
                 indices = [subset[i].likelihood >= self.threshold for i in range(len(subset))]
-                if (self.reconstruction_algorithm == "auto_subset" and sum(indices) >= 2) or sum(indices) == len(
-                        self.data_readers):
+                if (self.global_config.reconstruction_algorithm == "auto_subset" and sum(indices) >= 2) or sum(
+                        indices) == len(
+                    self.data_readers):
                     dlt_subset = dlt_subset[indices, :]
                     subset = [element for i, element in enumerate(subset) if indices[i]]
-                    recon_data[name] = rotate(DLTrecon(3, len(subset), dlt_subset, subset), self.rotation_matrix,
-                                              self.scale) + self.translation_matrix
+                    recon_data[name] = rotate(DLTrecon(3, len(subset), dlt_subset, subset), rotation_matrix,
+                                              scale,
+                                              multiplier=self.global_config.axis_rotation_3D) + translation_matrix
                     prob_data[name] = min(subset, key=lambda x: x.likelihood).likelihood
-            skeleton_3D = Skeleton(self.body_parts, recon_data, prob_data)
-            self.out_csv.set_skeleton(iterator, skeleton_3D)
-        self.progress = 100
-        self.data_ready = True
+            skeleton_3D = Skeleton(self.global_config.body_parts, recon_data, prob_data)
+            self._out_csv.set_skeleton(iterator, skeleton_3D)
+        self._progress = 100
+        self._data_ready = True
 
     def get_output(self):
-        if self.data_ready:
-            return self.out_csv
+        if self._data_ready:
+            return self._out_csv
         else:
             return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/generative/generate_velocity_data.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/generative/generate_velocity_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import numpy as np
 
 from cvkit import MAGIC_NUMBER
 from cvkit.pose_estimation import Part
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
 
 
-class GenerateVelocity(PostProcessor):
-    PROCESS_NAME = "Generate Velocity"
-
-    def __init__(self, target_column, frame_rate, velocity_threshold, threshold=0.6):
-        super(GenerateVelocity, self).__init__(target_column)
-        self.dt = 1 / frame_rate
+class GenerateVelocity(Processor):
+    PROCESSOR_NAME = "Generate Velocity"
+    PROCESSOR_ID = "cvkit_generate_velocity"
+    META_DATA = {'target_column': ProcessorMetaData('Target Part', ProcessorMetaData.BODY_PART),
+                 'threshold': ProcessorMetaData('Threshold', ProcessorMetaData.FLOAT, 0.6, 0.0, 1.0),
+                 'velocity_threshold': ProcessorMetaData('Velocity Threshold', ProcessorMetaData.FLOAT),
+                 'framerate': ProcessorMetaData('Framerate', ProcessorMetaData.FLOAT)}
+
+    PROCESSOR_SUMMARY = "Computes velocity data for target column and stores in empty datastore"
+
+    def __init__(self, target_column, framerate, velocity_threshold, threshold=0.6):
+        super(GenerateVelocity, self).__init__()
+        self.target_column = target_column
+        self.framerate = framerate
+        self.dt = 1 / framerate
         self.threshold = threshold
         self.velocity_threshold = velocity_threshold
 
     def process(self, data_store, empty_datastore):
-        self.data_store = data_store
-        self.data_ready = False
-        self.progress = 0
+        self._data_store = data_store
+        self._data_ready = False
+        self._progress = 0
         previous_point = None
         previous_index = -1
-        for index, point in self.data_store.part_iterator(self.target_column):
-            self.progress = int(index / len(self.data_store) * 100)
-            if self.PRINT and self.progress % 10 == 0:
-                print(f'\r {self.PROCESS_NAME} {self.progress}% complete', end='')
+        for index, point in self._data_store.part_iterator(self.target_column):
+            self._progress = int(index / len(self._data_store) * 100)
+            if self.PRINT and self._progress % 10 == 0:
+                print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
             velocity = [MAGIC_NUMBER, MAGIC_NUMBER, MAGIC_NUMBER]
             flag = False
             if point > self.threshold:
                 if previous_point is not None:
                     velocity = np.subtract(point, previous_point) / ((index - previous_index) * self.dt)
                 else:
                     velocity = [0, 0, 0]
@@ -36,15 +45,15 @@
                     previous_point = point.copy()
                     previous_index = index
                 else:
                     velocity = [MAGIC_NUMBER, MAGIC_NUMBER, MAGIC_NUMBER]
             empty_datastore.set_part(index, Part(velocity, self.target_column, float(flag)))
         if self.PRINT:
             print(f'\r {self.PROCESS_NAME} 100% complete', end='')
-        self.data_ready = True
-        self.progress = 100
+        self._data_ready = True
+        self._progress = 100
 
     def get_output(self):
-        if self.data_ready:
-            return self.data_store
+        if self._data_ready:
+            return self._data_store
         else:
             return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/post_processors/util/cluster_analysis.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/processors/util/cluster_analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from cvkit.pose_estimation.data_readers import DataStoreStats
-from cvkit.pose_estimation.post_processors.post_prcessor_interface import PostProcessor
+from cvkit.pose_estimation.processors.processor_interface import Processor, ProcessorMetaData
 
 
-class ClusterAnalysis(PostProcessor):
-    PROCESS_NAME = "Data Analysis"
+class ClusterAnalysis(Processor):
+    PROCESSOR_NAME = "Data Analysis"
+    PROCESSOR_ID = "cvkit_cluster_analysis"
+    META_DATA = {'threshold': ProcessorMetaData('Threshold', ProcessorMetaData.FLOAT, 0.6, 0.0, 1.0)}
+    PROCESSOR_SUMMARY = "Generates meta-statistics of 2D/3D pose data. Provides list of clusters of accurate or missing data."
 
     def __init__(self, threshold=0.6):
         self.threshold = threshold
-        super(ClusterAnalysis, self).__init__(None)
+        super(ClusterAnalysis, self).__init__()
 
     def process(self, data_store):
-        self.data_store = data_store
-        self.data_ready = False
-        self.progress = 0
-        body_parts = self.data_store.body_parts
-        stats = DataStoreStats(body_parts)
-        for index, skeleton in self.data_store.row_iterator():
-            self.progress = int(index / len(self.data_store) * 100)
-            if self.PRINT and self.progress % 10 == 0:
-                print(f'\r {self.PROCESS_NAME} {self.progress}% complete', end='')
-            accurate = True
-            acc_count = len(data_store.body_parts)
-            for part in body_parts:
-                if skeleton[part] < self.threshold:
-                    stats.update_cluster_info(index, part)
-                    accurate = False
-                    acc_count -= 1
-            stats.add_occupancy_data(acc_count / len(data_store.body_parts))
-            if accurate:
-                stats.update_cluster_info(index, '', True)
-        if self.PRINT and self.progress % 10 == 0:
-            print(f'\r {self.PROCESS_NAME} {self.progress}% complete', end='')
-        self.data_store.set_stats(stats)
-        self.data_ready = True
-        self.progress = 100
+        self._data_store = data_store
+        self._data_ready = False
+        self._progress = 0
+        if not self._data_store.verify_stats():
+            body_parts = self._data_store.body_parts
+            stats = DataStoreStats(body_parts)
+            for index, skeleton in self._data_store.row_iterator():
+                self._progress = int(index / len(self._data_store) * 100)
+                if self.PRINT and self._progress % 10 == 0:
+                    print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
+                accurate = True
+                acc_count = len(data_store.body_parts)
+                for part in body_parts:
+                    if skeleton[part] < self.threshold:
+                        stats.update_cluster_info(index, part)
+                        accurate = False
+                        acc_count -= 1
+                stats.add_occupancy_data(acc_count / len(data_store.body_parts))
+                if accurate:
+                    stats.update_cluster_info(index, '', True)
+            if self.PRINT and self._progress % 10 == 0:
+                print(f'\r {self.PROCESS_NAME} {self._progress}% complete', end='')
+            self._data_store.set_stats(stats)
+        self._data_ready = True
+        self._progress = 100
 
     def get_output(self):
-        if self.data_ready:
-            return self.data_store
+        if self._data_ready:
+            return self._data_store
         else:
             return None
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/reconstruction/DLT.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/reconstruction/DLT.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     Reconstruction of object point from image point(s) based on the DLT parameters.
 
     This code performs 2D or 3D DLT point reconstruction with any number of views (views).
     For 3D DLT, at least two views (views) are necessary.
     Inputs:
      nd is the number of dimensions of the object space: 3 for 3D DLT and 2 for 2D DLT.
      nc is the number of views (views) used.
-     Ls (array type) are the camera calibration parameters of each camera 
+     Ls (array param_type) are the camera calibration parameters of each camera
       (is the output of DLTcalib function). The Ls parameters are given as columns
       and the Ls for different views as rows.
      uvs are the coordinates of the point in the image 2D space of each camera.
       The coordinates of the point are given as columns and the different views as rows.
     Outputs:
      xyz: point coordinates in space
     '''
@@ -126,15 +126,15 @@
     '''
     Deconstruction of object point to image point(s) based on the DLT parameters.
 
     This code performs 3D or 2D DLT point reconstruction with any number of views (views).
     Inputs:
      nd is the number of dimensions of the object space: 3 for 3D DLT and 2 for 2D DLT.
      nc is the number of views (views) used.
-     Ls (array type) are the camera calibration parameters of each camera 
+     Ls (array param_type) are the camera calibration parameters of each camera
       (is the output of DLTcalib function). The Ls parameters are given as columns
       and the Ls for different views as rows.
      xyz is point coordinates in object space, accept multiple points
     Outputs:
      uvs: the coordinates of the point in the image 2D space of each camera. 
          each inputs correspond to one 3D point
          every two columns is a pair of (u,v) in one camera view
```

### Comparing `bu_cvkit-0.0.2/cvkit/pose_estimation/reconstruction/EasyWand_tools.py` & `bu_cvkit-0.0.3/cvkit/pose_estimation/reconstruction/EasyWand_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 import numpy as np
 import pandas as pd
 from scipy.spatial.transform import Rotation
 
 from cvkit.pose_estimation import Part
 from cvkit.pose_estimation.config import PoseEstimationConfig
-from cvkit.pose_estimation.post_processors.util import ClusterAnalysis
+from cvkit.pose_estimation.processors.util import ClusterAnalysis
 from cvkit.pose_estimation.reconstruction.DLT import DLTrecon
 from cvkit.pose_estimation.utils import rotate, magnitude
 
 
 def generate_EasyWand_data(config: PoseEstimationConfig, csv_maps, common_indices, static_points_map):
-    file = open(join(config.output_folder,
-                     f'{config.project_name}_calibration_camera_order.txt'), 'w')
     os.makedirs(join(config.output_folder, 'calibration'), exist_ok=True)
+    file = open(join(config.output_folder, 'calibration',
+                     f'{config.project_name}_calibration_camera_order.txt'), 'w')
     camera_profile = open(
         join(config.output_folder, 'calibration', f'{config.project_name}_calibration_camera_profiles.txt'),
         'w')
     for i, camera in enumerate(config.views):
         file.write(f'{camera} ')
         camera_config = config.views[camera]
         profile = f'{i + 1} {camera_config.f_px} {camera_config.resolution[0]} {camera_config.resolution[1]} {camera_config.principal_point[0]} {camera_config.principal_point[1]} 1 0 0 0 0 0\n'
@@ -57,17 +57,20 @@
         x_max_2D = [config.views[view].axes['x_max'] for view in source_views]
         y_max_2D = [config.views[view].axes['y_max'] for view in source_views]
         origin = Part((DLTrecon(3, len(origin_2D), dlt_coefficients, origin_2D)), "origin", 1)
         x_max = Part((DLTrecon(3, len(x_max_2D), dlt_coefficients, x_max_2D)), "x_max", 1)
         y_max = Part((DLTrecon(3, len(y_max_2D), dlt_coefficients, y_max_2D)), "y_max", 1)
         rotation_matrix = Rotation.align_vectors([x_max - origin, y_max - origin], [[1, 0, 0], [0, 1, 0]])[
             0].as_matrix()
-        origin = Part(rotate(DLTrecon(3, len(origin_2D), dlt_coefficients, origin_2D), rotation_matrix), "origin", 1)
-        x_max = Part(rotate(DLTrecon(3, len(x_max_2D), dlt_coefficients, x_max_2D), rotation_matrix), "x_max", 1)
-        y_max = Part(rotate(DLTrecon(3, len(y_max_2D), dlt_coefficients, y_max_2D), rotation_matrix), "y_max", 1)
+        origin = Part(rotate(DLTrecon(3, len(origin_2D), dlt_coefficients, origin_2D), rotation_matrix,
+                             multiplier=config.axis_rotation_3D), "origin", 1)
+        x_max = Part(rotate(DLTrecon(3, len(x_max_2D), dlt_coefficients, x_max_2D), rotation_matrix,
+                            multiplier=config.axis_rotation_3D), "x_max", 1)
+        y_max = Part(rotate(DLTrecon(3, len(y_max_2D), dlt_coefficients, y_max_2D), rotation_matrix,
+                            multiplier=config.axis_rotation_3D), "y_max", 1)
         config.computed_scale = (config.scale / magnitude(x_max - origin) + config.scale / magnitude(
             y_max - origin)) / 2
         trans_mat = -origin
         config.rotation_matrix = rotation_matrix
         config.translation_matrix = trans_mat
     except:
         return False
@@ -91,15 +94,15 @@
     part = data_stores[0].body_parts[0]
     candidates = []
     for accurate_data in accurate_data_points:
         for index in range(accurate_data['begin'], accurate_data['end']):
             position = data_stores[0].get_part(index, part)
             x_bin, y_bin = int(position[0] / bin_size), int(position[1] / bin_size)
             if 0 <= x_bin < num_bins[0] and 0 <= y_bin < num_bins[1] and (
-                    spatial_bins[x_bin][y_bin] < 3 and index - frame_number[x_bin][y_bin] > 10):
+                    spatial_bins[x_bin][y_bin] == 0 and index - frame_number[x_bin][y_bin] > config.framerate * .1):
                 spatial_bins[x_bin][y_bin] += 1
                 frame_number[x_bin][y_bin] = index
                 candidates.append(index)
     return candidates
 
 
 def update_config_dlt_coeffs(config: PoseEstimationConfig, dlt_coefficients_file, order):
```

### Comparing `bu_cvkit-0.0.2/cvkit/video_readers/__init__.py` & `bu_cvkit-0.0.3/cvkit/video_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `bu_cvkit-0.0.2/cvkit/video_readers/cv2_reader.py` & `bu_cvkit-0.0.3/cvkit/video_readers/cv2_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import time
 from queue import Queue, Empty
 from threading import Thread
 
 import cv2
 import numpy as np
 
@@ -12,52 +13,53 @@
 
     def random_access_image(self, position):
         if 0 <= position < self.total_frames:
             stream = cv2.VideoCapture(self.video_path)
             stream.set(cv2.CAP_PROP_POS_FRAMES, position)
             ret, frame = stream.read()
             stream.release()
+            print(sys.getsizeof(frame))
             if ret:
                 return cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
 
     FLAVOR = "opencv"
 
     def __init__(self, video_path, fps, buffer_size=64):
         super().__init__(video_path, fps, buffer_size)
         self.state = 0
         self.thread = None
         self.buffer = Queue(maxsize=buffer_size)
         self.stream = cv2.VideoCapture(self.video_path)
         self.total_frames = int(self.stream.get(cv2.CAP_PROP_FRAME_COUNT))
 
     def start(self):
-        if self.thread is None:
-            with self.buffer.mutex:
-                self.buffer.queue.clear()
         self.stream.set(cv2.CAP_PROP_POS_FRAMES, self.current_index + 1)
         self.thread = Thread(target=self.fill_buffer)
         self.thread.daemon = True
         self.state = 1
         self.thread.start()
 
     def fill_buffer(self):
         while True:
             if self.state <= 0:
                 break
             if not self.buffer.full():
                 ret, frame = self.stream.read()
-                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-                self.buffer.put(frame)
+                if ret:
+                    frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                    self.buffer.put(frame)
             else:
                 time.sleep(0.01)
 
     def stop(self):
         if self.thread:
             self.state = -1
             self.thread.join()
+            with self.buffer.mutex:
+                self.buffer.queue.clear()
         self.thread = None
 
     def pause(self) -> None:
         self.state = 0
 
     def release(self):
         self.stop()
```

### Comparing `bu_cvkit-0.0.2/cvkit/video_readers/deffcode_reader.py` & `bu_cvkit-0.0.3/cvkit/video_readers/deffcode_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,14 @@
         self.buffer = Queue(maxsize=buffer_size)
         self.stream = FFdecoder(self.video_path).formulate()
         self.total_frames = json.loads(self.stream.metadata)['approx_video_nframes']
         self.stream.terminate()
         self.current_index = -1
 
     def start(self):
-        if self.thread is None:
-            with self.buffer.mutex:
-                self.buffer.queue.clear()
         ts = self.get_timestamp(self.current_index + 1)
         self.stream = FFdecoder(self.video_path, **{'-ss': ts}).formulate()
         self.thread = Thread(target=self.fill_buffer)
         self.thread.daemon = True
         self.state = 1
         self.thread.start()
 
@@ -56,14 +53,16 @@
             else:
                 time.sleep(0.01)
 
     def stop(self):
         if self.thread:
             self.state = -1
             self.thread.join()
+            with self.buffer.mutex:
+                self.buffer.queue.clear()
         self.stream.terminate()
         self.thread = None
 
     def pause(self) -> None:
         self.state = 0
 
     def release(self):
```

### Comparing `bu_cvkit-0.0.2/cvkit/video_readers/video_reader_interface.py` & `bu_cvkit-0.0.3/cvkit/video_readers/video_reader_interface.py`

 * *Files identical despite different names*

### Comparing `bu_cvkit-0.0.2/pyproject.toml` & `bu_cvkit-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "bu_cvkit"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="Mahir Patel", email="mahirp@bu.edu" },
+    { name = "Mahir Patel", email = "mahirp@bu.edu" },
 ]
 description = "A toolkit to accelerate computer vision research"
-requires-python = ">=3.10"
+requires-python = ">=3.10,<3.11"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 dependencies = ["deffcode==0.2.5",
-"filterpy==1.4.5",
-"numpy==1.24.2",
-"opencv_python_headless==4.7.0.72",
-"pandas==1.5.3",
-"PyYAML==6.0",
-"scipy==1.10.1",
-"tensorflow==2.11.0"]
+    "filterpy==1.4.5",
+    "numpy==1.24.2",
+    "opencv_python_headless==4.7.0.72",
+    "pandas==1.5.3",
+    "PyYAML==6.0",
+    "scipy==1.10.1",
+    "tensorflow==2.11.0"]
 [project.urls]
-repository = "https://github.com/mahir1010/BU-CVKit"
+repository = "https://github.com/mahir1010/BU-CVKit"
```

